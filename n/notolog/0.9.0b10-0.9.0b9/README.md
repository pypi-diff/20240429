# Comparing `tmp/notolog-0.9.0b10.tar.gz` & `tmp/notolog-0.9.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notolog-0.9.0b10.tar", last modified: Mon Apr 29 04:05:19 2024, max compression
+gzip compressed data, was "notolog-0.9.0b9.tar", last modified: Mon Apr 29 01:03:37 2024, max compression
```

## Comparing `notolog-0.9.0b10.tar` & `notolog-0.9.0b9.tar`

### file list

```diff
@@ -1,311 +1,312 @@
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.592651 notolog-0.9.0b10/
--rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-04-28 21:48:22.000000 notolog-0.9.0b10/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      119 2024-04-29 03:37:45.000000 notolog-0.9.0b10/MANIFEST.in
--rw-r--r--   0 vadikus    (501) staff       (20)    15934 2024-04-29 04:05:19.591344 notolog-0.9.0b10/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    14450 2024-04-29 01:01:37.000000 notolog-0.9.0b10/README.md
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.271943 notolog-0.9.0b10/app/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3493 2024-04-28 22:15:01.000000 notolog-0.9.0b10/app/app_config.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.273699 notolog-0.9.0b10/app/assets/
--rw-r--r--   0 vadikus    (501) staff       (20)     4238 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/notolog-example-image.png
--rw-r--r--   0 vadikus    (501) staff       (20)    88269 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/notolog-logo.png
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.226861 notolog-0.9.0b10/app/assets/themes/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.286463 notolog-0.9.0b10/app/assets/themes/calligraphy/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2145 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      903 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6307 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.313719 notolog-0.9.0b10/app/assets/themes/default/
--rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/editor.css
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.388227 notolog-0.9.0b10/app/assets/themes/default/icons/
--rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/arrow-clockwise.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/arrow-repeat.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/balloon-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/balloon.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/bandaid-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/bandaid.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/box-arrow-up-right.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/box-arrow-up.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/caret-down-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/caret-up-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/code-slash.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/cursor-text.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/eyedropper.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/eyeglasses.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/file-earmark-lock2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/file-earmark-plus-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/file-earmark-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/file-earmark.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/filetype-html.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/filetype-md.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/filetype-txt.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/floppy2-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/floppy2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/folder-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/folder-symlink.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/folder.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/github.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/link-45deg.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/linkedin.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/pencil-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/power.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/quote.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/robot.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/share-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/shield-lock-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/shield-lock.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/star-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/star.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/three-dots.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/trash3-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/trash3.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/twitter-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/type-bold.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/type-italic.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/type-strikethrough.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/type-underline.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/x-circle-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/x-square-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/x-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     2250 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      739 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     7957 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.398582 notolog-0.9.0b10/app/assets/themes/noir_dark/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2357 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     1328 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6410 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.413591 notolog-0.9.0b10/app/assets/themes/strawberry/
--rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      739 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     7940 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/viewer.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/edit_widget.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/editor_state.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.421800 notolog-0.9.0b10/app/encrypt/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/encrypt/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4267 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/encrypt/enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6133 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/encrypt/enc_new_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)      551 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/encrypt/enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4229 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/encrypt/enc_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3149 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/encrypt/enc_password_reset_dialog.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.426868 notolog-0.9.0b10/app/enums/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/enums/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1855 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/enums/ai_model_names.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6229 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/enums/colors.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1335 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/enums/languages.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1365 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/enums/themes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2866 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/etree_extension.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.428229 notolog-0.9.0b10/app/exceptions/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/exceptions/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/exceptions/file_header_empty_exception.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6945 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/file_system_watcher.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.434431 notolog-0.9.0b10/app/helpers/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/helpers/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/helpers/clipboard_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2437 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/helpers/file_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/helpers/theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)      696 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/helpers/tooltip_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7167 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/helpers/update_helper.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.438514 notolog-0.9.0b10/app/highlight/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/highlight/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8594 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/highlight/main_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)    47898 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/highlight/md_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8007 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/highlight/view_highlighter.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.439981 notolog-0.9.0b10/app/lexemes/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/lexemes/__init__.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.442471 notolog-0.9.0b10/app/lexemes/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      164 2024-04-29 00:12:00.000000 notolog-0.9.0b10/app/lexemes/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3221 2024-04-28 22:06:29.000000 notolog-0.9.0b10/app/lexemes/__pycache__/lexemes.cpython-39.pyc
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.449431 notolog-0.9.0b10/app/lexemes/de/
--rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/de/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/de/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6547 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/de/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/de/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3514 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/de/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/de/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/de/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.459138 notolog-0.9.0b10/app/lexemes/en/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.470093 notolog-0.9.0b10/app/lexemes/en/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      883 2024-04-28 22:11:17.000000 notolog-0.9.0b10/app/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6660 2024-04-28 22:11:17.000000 notolog-0.9.0b10/app/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5428 2024-04-28 22:11:17.000000 notolog-0.9.0b10/app/lexemes/en/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2083 2024-04-28 22:11:17.000000 notolog-0.9.0b10/app/lexemes/en/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3248 2024-04-28 22:11:17.000000 notolog-0.9.0b10/app/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-04-28 22:11:17.000000 notolog-0.9.0b10/app/lexemes/en/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2492 2024-04-28 22:11:17.000000 notolog-0.9.0b10/app/lexemes/en/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/en/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/en/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6009 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/en/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/en/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3351 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/en/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/en/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/en/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.478342 notolog-0.9.0b10/app/lexemes/es/
--rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/es/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/es/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6517 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/es/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/es/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3615 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/es/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/es/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/es/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.486162 notolog-0.9.0b10/app/lexemes/fr/
--rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/fr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/fr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6677 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/fr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/fr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3690 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/fr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/fr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/fr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.492552 notolog-0.9.0b10/app/lexemes/ge/
--rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ge/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ge/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9689 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ge/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ge/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5310 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ge/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ge/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ge/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.499423 notolog-0.9.0b10/app/lexemes/it/
--rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/it/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/it/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6327 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/it/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/it/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3562 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/it/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/it/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/it/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.505811 notolog-0.9.0b10/app/lexemes/ja/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.517116 notolog-0.9.0b10/app/lexemes/ja/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)     1020 2024-04-28 22:06:30.000000 notolog-0.9.0b10/app/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     8452 2024-04-28 22:06:30.000000 notolog-0.9.0b10/app/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6809 2024-04-28 22:06:30.000000 notolog-0.9.0b10/app/lexemes/ja/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2411 2024-04-28 22:06:30.000000 notolog-0.9.0b10/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3780 2024-04-28 22:06:30.000000 notolog-0.9.0b10/app/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1301 2024-04-28 22:06:30.000000 notolog-0.9.0b10/app/lexemes/ja/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3047 2024-04-28 22:06:30.000000 notolog-0.9.0b10/app/lexemes/ja/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ja/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ja/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7209 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ja/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ja/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3747 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ja/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ja/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ja/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.526296 notolog-0.9.0b10/app/lexemes/ko/
--rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ko/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/ko/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6733 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/ko/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/ko/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3414 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/ko/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ko/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/ko/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.533207 notolog-0.9.0b10/app/lexemes/la/
--rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/la/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/la/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6204 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/la/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/la/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3505 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/la/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/la/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/la/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3739 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/lexemes.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.539032 notolog-0.9.0b10/app/lexemes/pt/
--rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/pt/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/pt/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6315 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/pt/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/pt/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3574 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/pt/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/pt/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/pt/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.545516 notolog-0.9.0b10/app/lexemes/ru/
--rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ru/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ru/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7899 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ru/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ru/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4504 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ru/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ru/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ru/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.551915 notolog-0.9.0b10/app/lexemes/zh/
--rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/zh/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/zh/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5738 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/zh/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/zh/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3256 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/zh/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/zh/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/zh/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)   177102 2024-04-29 04:00:35.000000 notolog-0.9.0b10/app/notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)    11239 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5968 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/theme.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.575529 notolog-0.9.0b10/app/ui/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7920 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/about_popup.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16871 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2134 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3311 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/common_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)      977 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/enum_combo_box.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5635 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/file_system_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7063 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/line_numbers.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2526 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/rename_file_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/rotating_label.py
--rw-r--r--   0 vadikus    (501) staff       (20)    35991 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3207 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/sort_filter_proxy_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6831 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4313 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/vertical_line_spacer.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/view_decorator.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16031 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/view_processor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2253 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/view_widget.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2521 2024-04-29 03:37:45.000000 notolog-0.9.0b10/main.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.590396 notolog-0.9.0b10/notolog.egg-info/
--rw-r--r--   0 vadikus    (501) staff       (20)    15934 2024-04-29 04:05:19.000000 notolog-0.9.0b10/notolog.egg-info/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)     9693 2024-04-29 04:05:19.000000 notolog-0.9.0b10/notolog.egg-info/SOURCES.txt
--rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-04-29 04:05:19.000000 notolog-0.9.0b10/notolog.egg-info/dependency_links.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-29 04:05:19.000000 notolog-0.9.0b10/notolog.egg-info/entry_points.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      367 2024-04-29 04:05:19.000000 notolog-0.9.0b10/notolog.egg-info/requires.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       15 2024-04-29 04:05:19.000000 notolog-0.9.0b10/notolog.egg-info/top_level.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-29 04:05:19.592872 notolog-0.9.0b10/setup.cfg
--rw-r--r--   0 vadikus    (501) staff       (20)     1650 2024-04-29 03:47:58.000000 notolog-0.9.0b10/setup.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.589373 notolog-0.9.0b10/tests/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b10/tests/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5975 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2305 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9197 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3962 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_html_view.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5810 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_lexemes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5645 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1154 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4971 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4053 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6182 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_themes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.632904 notolog-0.9.0b9/
+-rw-r--r--   0 vadikus    (501) staff       (20)     8552 2024-04-29 00:55:10.000000 notolog-0.9.0b9/Examples.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-04-28 21:48:22.000000 notolog-0.9.0b9/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      124 2024-04-29 00:40:08.000000 notolog-0.9.0b9/MANIFEST.in
+-rw-r--r--   0 vadikus    (501) staff       (20)    15920 2024-04-29 01:03:37.631481 notolog-0.9.0b9/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    14450 2024-04-29 01:01:37.000000 notolog-0.9.0b9/README.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     2529 2024-04-28 22:15:02.000000 notolog-0.9.0b9/main.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:36.536623 notolog-0.9.0b9/notolog/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3493 2024-04-28 22:15:01.000000 notolog-0.9.0b9/notolog/app_config.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:36.542473 notolog-0.9.0b9/notolog/assets/
+-rw-r--r--   0 vadikus    (501) staff       (20)     4238 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/notolog-example-image.png
+-rw-r--r--   0 vadikus    (501) staff       (20)    88269 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/notolog-logo.png
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:36.508688 notolog-0.9.0b9/notolog/assets/themes/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:36.555940 notolog-0.9.0b9/notolog/assets/themes/calligraphy/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/calligraphy/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-04-28 21:48:26.000000 notolog-0.9.0b9/notolog/assets/themes/calligraphy/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/calligraphy/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/calligraphy/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2145 2024-04-28 21:48:26.000000 notolog-0.9.0b9/notolog/assets/themes/calligraphy/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      903 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/calligraphy/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/calligraphy/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6307 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/calligraphy/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/calligraphy/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/calligraphy/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/calligraphy/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/calligraphy/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:36.578642 notolog-0.9.0b9/notolog/assets/themes/default/
+-rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/editor.css
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.007521 notolog-0.9.0b9/notolog/assets/themes/default/icons/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/arrow-clockwise.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/arrow-repeat.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/balloon-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/balloon.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/bandaid-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/bandaid.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/box-arrow-up-right.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/box-arrow-up.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/caret-down-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/caret-up-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/code-slash.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/cursor-text.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/eyedropper.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/eyeglasses.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/file-earmark-lock2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/file-earmark-plus-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/file-earmark-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/file-earmark.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/filetype-html.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/filetype-md.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/filetype-txt.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/floppy2-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/floppy2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/folder-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/folder-symlink.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/folder.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/github.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/link-45deg.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/linkedin.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/pencil-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/power.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/quote.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/robot.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/share-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/shield-lock-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/shield-lock.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/star-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/star.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/three-dots.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/trash3-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/trash3.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/twitter-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/type-bold.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/type-italic.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/type-strikethrough.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/type-underline.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/x-circle-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/x-square-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/icons/x-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     2250 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      739 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     7957 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/default/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.105486 notolog-0.9.0b9/notolog/assets/themes/noir_dark/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/noir_dark/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/noir_dark/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/noir_dark/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/noir_dark/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2357 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/noir_dark/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     1328 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/noir_dark/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/noir_dark/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6410 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/noir_dark/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/noir_dark/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/noir_dark/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/noir_dark/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/noir_dark/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.124138 notolog-0.9.0b9/notolog/assets/themes/strawberry/
+-rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/strawberry/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/strawberry/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/strawberry/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/strawberry/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/strawberry/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      739 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/strawberry/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/strawberry/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     7940 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/strawberry/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/strawberry/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/strawberry/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/strawberry/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/assets/themes/strawberry/viewer.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/edit_widget.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/editor_state.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.242287 notolog-0.9.0b9/notolog/encrypt/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/encrypt/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4267 2024-04-28 21:48:25.000000 notolog-0.9.0b9/notolog/encrypt/enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6133 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/encrypt/enc_new_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      551 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/encrypt/enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4229 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/encrypt/enc_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3149 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/encrypt/enc_password_reset_dialog.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.258916 notolog-0.9.0b9/notolog/enums/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/enums/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1855 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/enums/ai_model_names.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6229 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/enums/colors.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1335 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/enums/languages.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1365 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/enums/themes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2866 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/etree_extension.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.260829 notolog-0.9.0b9/notolog/exceptions/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/exceptions/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/exceptions/file_header_empty_exception.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6945 2024-04-28 21:48:26.000000 notolog-0.9.0b9/notolog/file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/file_system_watcher.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.297255 notolog-0.9.0b9/notolog/helpers/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:26.000000 notolog-0.9.0b9/notolog/helpers/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-04-28 21:48:26.000000 notolog-0.9.0b9/notolog/helpers/clipboard_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2437 2024-04-28 21:48:26.000000 notolog-0.9.0b9/notolog/helpers/file_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-04-28 21:48:26.000000 notolog-0.9.0b9/notolog/helpers/theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      696 2024-04-28 21:48:26.000000 notolog-0.9.0b9/notolog/helpers/tooltip_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7167 2024-04-28 21:48:26.000000 notolog-0.9.0b9/notolog/helpers/update_helper.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.302652 notolog-0.9.0b9/notolog/highlight/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/highlight/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8594 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/highlight/main_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    47898 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/highlight/md_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8007 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/highlight/view_highlighter.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.305920 notolog-0.9.0b9/notolog/lexemes/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/lexemes/__init__.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.308850 notolog-0.9.0b9/notolog/lexemes/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      164 2024-04-29 00:12:00.000000 notolog-0.9.0b9/notolog/lexemes/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3221 2024-04-28 22:06:29.000000 notolog-0.9.0b9/notolog/lexemes/__pycache__/lexemes.cpython-39.pyc
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.320623 notolog-0.9.0b9/notolog/lexemes/de/
+-rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/de/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/de/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6547 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/de/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/de/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3514 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/de/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/de/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/de/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.333626 notolog-0.9.0b9/notolog/lexemes/en/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.345342 notolog-0.9.0b9/notolog/lexemes/en/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      883 2024-04-28 22:11:17.000000 notolog-0.9.0b9/notolog/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6660 2024-04-28 22:11:17.000000 notolog-0.9.0b9/notolog/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5428 2024-04-28 22:11:17.000000 notolog-0.9.0b9/notolog/lexemes/en/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2083 2024-04-28 22:11:17.000000 notolog-0.9.0b9/notolog/lexemes/en/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3248 2024-04-28 22:11:17.000000 notolog-0.9.0b9/notolog/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-04-28 22:11:17.000000 notolog-0.9.0b9/notolog/lexemes/en/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2492 2024-04-28 22:11:17.000000 notolog-0.9.0b9/notolog/lexemes/en/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/en/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/en/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6009 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/en/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/en/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3351 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/en/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/en/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/en/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.352806 notolog-0.9.0b9/notolog/lexemes/es/
+-rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/es/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/es/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6517 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/es/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/es/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3615 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/es/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/es/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/es/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.360306 notolog-0.9.0b9/notolog/lexemes/fr/
+-rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/fr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/fr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6677 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/fr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/fr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3690 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/fr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/fr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/fr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.367191 notolog-0.9.0b9/notolog/lexemes/ge/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ge/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ge/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9689 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ge/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ge/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5310 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ge/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ge/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ge/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.375659 notolog-0.9.0b9/notolog/lexemes/it/
+-rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/it/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/it/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6327 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/it/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/it/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3562 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/it/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/it/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/it/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.381984 notolog-0.9.0b9/notolog/lexemes/ja/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.467906 notolog-0.9.0b9/notolog/lexemes/ja/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1020 2024-04-28 22:06:30.000000 notolog-0.9.0b9/notolog/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     8452 2024-04-28 22:06:30.000000 notolog-0.9.0b9/notolog/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6809 2024-04-28 22:06:30.000000 notolog-0.9.0b9/notolog/lexemes/ja/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2411 2024-04-28 22:06:30.000000 notolog-0.9.0b9/notolog/lexemes/ja/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3780 2024-04-28 22:06:30.000000 notolog-0.9.0b9/notolog/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1301 2024-04-28 22:06:30.000000 notolog-0.9.0b9/notolog/lexemes/ja/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3047 2024-04-28 22:06:30.000000 notolog-0.9.0b9/notolog/lexemes/ja/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ja/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ja/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7209 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ja/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ja/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3747 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ja/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ja/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ja/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.479699 notolog-0.9.0b9/notolog/lexemes/ko/
+-rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ko/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/ko/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6733 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/ko/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/ko/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3414 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/ko/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ko/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/ko/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.496400 notolog-0.9.0b9/notolog/lexemes/la/
+-rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/la/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/la/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6204 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/la/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/la/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3505 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/la/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/la/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/lexemes/la/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3739 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/lexemes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.503626 notolog-0.9.0b9/notolog/lexemes/pt/
+-rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/pt/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/pt/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6315 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/pt/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/pt/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3574 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/pt/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/pt/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/pt/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.514222 notolog-0.9.0b9/notolog/lexemes/ru/
+-rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ru/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ru/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7899 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ru/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ru/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4504 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ru/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ru/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/ru/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.578549 notolog-0.9.0b9/notolog/lexemes/zh/
+-rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/zh/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/zh/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5738 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/zh/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/zh/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3256 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/zh/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/zh/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-04-28 21:48:23.000000 notolog-0.9.0b9/notolog/lexemes/zh/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)   176983 2024-04-29 00:59:34.000000 notolog-0.9.0b9/notolog/notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    11239 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5968 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/theme.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.599486 notolog-0.9.0b9/notolog/ui/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/ui/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7920 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/ui/about_popup.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16871 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/ui/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2134 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/ui/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3311 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/ui/common_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      977 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/ui/enum_combo_box.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5635 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/ui/file_system_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7063 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/ui/line_numbers.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2526 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/ui/rename_file_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/ui/rotating_label.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    35991 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/ui/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3207 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/ui/sort_filter_proxy_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6831 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/ui/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4313 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/ui/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-04-28 21:48:22.000000 notolog-0.9.0b9/notolog/ui/vertical_line_spacer.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/view_decorator.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16031 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/view_processor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2253 2024-04-28 21:48:24.000000 notolog-0.9.0b9/notolog/view_widget.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.629998 notolog-0.9.0b9/notolog.egg-info/
+-rw-r--r--   0 vadikus    (501) staff       (20)    15920 2024-04-29 01:03:36.000000 notolog-0.9.0b9/notolog.egg-info/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    10721 2024-04-29 01:03:36.000000 notolog-0.9.0b9/notolog.egg-info/SOURCES.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-04-29 01:03:36.000000 notolog-0.9.0b9/notolog.egg-info/dependency_links.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-29 01:03:36.000000 notolog-0.9.0b9/notolog.egg-info/entry_points.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      367 2024-04-29 01:03:36.000000 notolog-0.9.0b9/notolog.egg-info/requires.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       19 2024-04-29 01:03:36.000000 notolog-0.9.0b9/notolog.egg-info/top_level.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-29 01:03:37.633434 notolog-0.9.0b9/setup.cfg
+-rw-r--r--   0 vadikus    (501) staff       (20)     1500 2024-04-29 01:03:33.000000 notolog-0.9.0b9/setup.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 01:03:37.628777 notolog-0.9.0b9/tests/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b9/tests/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5983 2024-04-28 21:48:22.000000 notolog-0.9.0b9/tests/test_enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2309 2024-04-28 21:48:22.000000 notolog-0.9.0b9/tests/test_enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9205 2024-04-28 21:48:22.000000 notolog-0.9.0b9/tests/test_file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3974 2024-04-28 21:48:22.000000 notolog-0.9.0b9/tests/test_html_view.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5814 2024-04-28 21:48:22.000000 notolog-0.9.0b9/tests/test_lexemes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5661 2024-04-28 21:48:22.000000 notolog-0.9.0b9/tests/test_notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1158 2024-04-28 21:48:22.000000 notolog-0.9.0b9/tests/test_settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4975 2024-04-28 21:48:22.000000 notolog-0.9.0b9/tests/test_text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4073 2024-04-28 21:48:22.000000 notolog-0.9.0b9/tests/test_theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6186 2024-04-28 21:48:22.000000 notolog-0.9.0b9/tests/test_themes.py
```

### Comparing `notolog-0.9.0b10/LICENSE` & `notolog-0.9.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/PKG-INFO` & `notolog-0.9.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.0b10
+Version: 0.9.0b9
 Summary: Notolog Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
-License: MIT
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `notolog-0.9.0b10/README.md` & `notolog-0.9.0b9/README.md`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/app_config.py` & `notolog-0.9.0b9/notolog/app_config.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/notolog-example-image.png` & `notolog-0.9.0b9/notolog/assets/notolog-example-image.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/notolog-logo.png` & `notolog-0.9.0b9/notolog/assets/notolog-logo.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/calligraphy/about_popup.css` & `notolog-0.9.0b9/notolog/assets/themes/calligraphy/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/calligraphy/default.ini` & `notolog-0.9.0b9/notolog/assets/themes/calligraphy/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/calligraphy/md.ini` & `notolog-0.9.0b9/notolog/assets/themes/calligraphy/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/calligraphy/settings_dialog.css` & `notolog-0.9.0b9/notolog/assets/themes/calligraphy/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/calligraphy/styles.css` & `notolog-0.9.0b9/notolog/assets/themes/calligraphy/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/calligraphy/tree_view.css` & `notolog-0.9.0b9/notolog/assets/themes/calligraphy/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/about_popup.css` & `notolog-0.9.0b9/notolog/assets/themes/default/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/default.ini` & `notolog-0.9.0b9/notolog/assets/themes/default/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/LICENSE` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/arrow-repeat.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/arrow-repeat.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/balloon-fill.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/balloon-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/balloon.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/balloon.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/bandaid-fill.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/bandaid-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/bandaid.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/bandaid.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/box-arrow-up-right.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/box-arrow-up-right.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/box-arrow-up.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/box-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/cursor-text.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/cursor-text.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/filetype-html.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/filetype-html.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/filetype-md.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/filetype-md.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/filetype-txt.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/filetype-txt.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/floppy2.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/floppy2.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/folder-symlink.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/folder-symlink.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/folder.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/github.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/github.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/link-45deg.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/link-45deg.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/linkedin.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/linkedin.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/pencil-square.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/pencil-square.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/quote.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/quote.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/robot.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/robot.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/shield-lock-fill.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/shield-lock-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/shield-lock.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/shield-lock.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/star.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/star.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/trash3-fill.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/trash3-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/trash3.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/trash3.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/type-strikethrough.svg` & `notolog-0.9.0b9/notolog/assets/themes/default/icons/type-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/md.ini` & `notolog-0.9.0b9/notolog/assets/themes/default/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/settings_dialog.css` & `notolog-0.9.0b9/notolog/assets/themes/default/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/styles.css` & `notolog-0.9.0b9/notolog/assets/themes/default/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/tree_view.css` & `notolog-0.9.0b9/notolog/assets/themes/default/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/noir_dark/about_popup.css` & `notolog-0.9.0b9/notolog/assets/themes/noir_dark/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/noir_dark/default.ini` & `notolog-0.9.0b9/notolog/assets/themes/noir_dark/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/noir_dark/md.ini` & `notolog-0.9.0b9/notolog/assets/themes/noir_dark/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/noir_dark/settings_dialog.css` & `notolog-0.9.0b9/notolog/assets/themes/noir_dark/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/noir_dark/styles.css` & `notolog-0.9.0b9/notolog/assets/themes/noir_dark/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/noir_dark/tree_view.css` & `notolog-0.9.0b9/notolog/assets/themes/noir_dark/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/strawberry/about_popup.css` & `notolog-0.9.0b9/notolog/assets/themes/strawberry/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/strawberry/default.ini` & `notolog-0.9.0b9/notolog/assets/themes/strawberry/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/strawberry/md.ini` & `notolog-0.9.0b9/notolog/assets/themes/strawberry/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/strawberry/settings_dialog.css` & `notolog-0.9.0b9/notolog/assets/themes/strawberry/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/strawberry/styles.css` & `notolog-0.9.0b9/notolog/assets/themes/strawberry/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/strawberry/tree_view.css` & `notolog-0.9.0b9/notolog/assets/themes/strawberry/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/edit_widget.py` & `notolog-0.9.0b9/notolog/edit_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/editor_state.py` & `notolog-0.9.0b9/notolog/editor_state.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/encrypt/enc_helper.py` & `notolog-0.9.0b9/notolog/encrypt/enc_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/encrypt/enc_new_password_dialog.py` & `notolog-0.9.0b9/notolog/encrypt/enc_new_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/encrypt/enc_password.py` & `notolog-0.9.0b9/notolog/encrypt/enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/encrypt/enc_password_dialog.py` & `notolog-0.9.0b9/notolog/encrypt/enc_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/encrypt/enc_password_reset_dialog.py` & `notolog-0.9.0b9/notolog/encrypt/enc_password_reset_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/enums/ai_model_names.py` & `notolog-0.9.0b9/notolog/enums/ai_model_names.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/enums/colors.py` & `notolog-0.9.0b9/notolog/enums/colors.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/enums/languages.py` & `notolog-0.9.0b9/notolog/enums/languages.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/enums/themes.py` & `notolog-0.9.0b9/notolog/enums/themes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/etree_extension.py` & `notolog-0.9.0b9/notolog/etree_extension.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/file_header.py` & `notolog-0.9.0b9/notolog/file_header.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/file_system_watcher.py` & `notolog-0.9.0b9/notolog/file_system_watcher.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/helpers/file_helper.py` & `notolog-0.9.0b9/notolog/helpers/file_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/helpers/theme_helper.py` & `notolog-0.9.0b9/notolog/helpers/theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/helpers/tooltip_helper.py` & `notolog-0.9.0b9/notolog/helpers/tooltip_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/helpers/update_helper.py` & `notolog-0.9.0b9/notolog/helpers/update_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/highlight/main_highlighter.py` & `notolog-0.9.0b9/notolog/highlight/main_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/highlight/md_highlighter.py` & `notolog-0.9.0b9/notolog/highlight/md_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/highlight/view_highlighter.py` & `notolog-0.9.0b9/notolog/highlight/view_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/__pycache__/lexemes.cpython-39.pyc` & `notolog-0.9.0b9/notolog/lexemes/__pycache__/lexemes.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/de/ai_assistant.py` & `notolog-0.9.0b9/notolog/lexemes/de/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/de/color_picker_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/de/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/de/common.py` & `notolog-0.9.0b9/notolog/lexemes/de/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/de/main_menu.py` & `notolog-0.9.0b9/notolog/lexemes/de/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/de/settings_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/de/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/de/statusbar.py` & `notolog-0.9.0b9/notolog/lexemes/de/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/de/toolbar.py` & `notolog-0.9.0b9/notolog/lexemes/de/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.0b9/notolog/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.0b9/notolog/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/__pycache__/common.cpython-39.pyc` & `notolog-0.9.0b9/notolog/lexemes/en/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.0b9/notolog/lexemes/en/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.0b9/notolog/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.0b9/notolog/lexemes/en/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.0b9/notolog/lexemes/en/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/ai_assistant.py` & `notolog-0.9.0b9/notolog/lexemes/en/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/color_picker_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/en/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/common.py` & `notolog-0.9.0b9/notolog/lexemes/en/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/main_menu.py` & `notolog-0.9.0b9/notolog/lexemes/en/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/settings_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/en/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/statusbar.py` & `notolog-0.9.0b9/notolog/lexemes/en/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/toolbar.py` & `notolog-0.9.0b9/notolog/lexemes/en/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/es/ai_assistant.py` & `notolog-0.9.0b9/notolog/lexemes/es/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/es/color_picker_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/es/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/es/common.py` & `notolog-0.9.0b9/notolog/lexemes/es/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/es/main_menu.py` & `notolog-0.9.0b9/notolog/lexemes/es/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/es/settings_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/es/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/es/statusbar.py` & `notolog-0.9.0b9/notolog/lexemes/es/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/es/toolbar.py` & `notolog-0.9.0b9/notolog/lexemes/es/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/fr/ai_assistant.py` & `notolog-0.9.0b9/notolog/lexemes/fr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/fr/color_picker_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/fr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/fr/common.py` & `notolog-0.9.0b9/notolog/lexemes/fr/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/fr/main_menu.py` & `notolog-0.9.0b9/notolog/lexemes/fr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/fr/settings_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/fr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/fr/statusbar.py` & `notolog-0.9.0b9/notolog/lexemes/fr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/fr/toolbar.py` & `notolog-0.9.0b9/notolog/lexemes/fr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ge/ai_assistant.py` & `notolog-0.9.0b9/notolog/lexemes/ge/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ge/color_picker_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/ge/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ge/common.py` & `notolog-0.9.0b9/notolog/lexemes/ge/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ge/main_menu.py` & `notolog-0.9.0b9/notolog/lexemes/ge/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ge/settings_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/ge/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ge/statusbar.py` & `notolog-0.9.0b9/notolog/lexemes/ge/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ge/toolbar.py` & `notolog-0.9.0b9/notolog/lexemes/ge/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/it/ai_assistant.py` & `notolog-0.9.0b9/notolog/lexemes/it/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/it/color_picker_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/it/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/it/common.py` & `notolog-0.9.0b9/notolog/lexemes/it/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/it/main_menu.py` & `notolog-0.9.0b9/notolog/lexemes/it/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/it/settings_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/it/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/it/statusbar.py` & `notolog-0.9.0b9/notolog/lexemes/it/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/it/toolbar.py` & `notolog-0.9.0b9/notolog/lexemes/it/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.0b9/notolog/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.0b9/notolog/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/__pycache__/common.cpython-39.pyc` & `notolog-0.9.0b9/notolog/lexemes/ja/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.0b9/notolog/lexemes/ja/__pycache__/main_menu.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.0b9/notolog/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.0b9/notolog/lexemes/ja/__pycache__/statusbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.0b9/notolog/lexemes/ja/__pycache__/toolbar.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/ai_assistant.py` & `notolog-0.9.0b9/notolog/lexemes/ja/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/color_picker_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/ja/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/common.py` & `notolog-0.9.0b9/notolog/lexemes/ja/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/main_menu.py` & `notolog-0.9.0b9/notolog/lexemes/ja/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/settings_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/ja/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/statusbar.py` & `notolog-0.9.0b9/notolog/lexemes/ja/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/toolbar.py` & `notolog-0.9.0b9/notolog/lexemes/ja/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ko/ai_assistant.py` & `notolog-0.9.0b9/notolog/lexemes/ko/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ko/color_picker_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/ko/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ko/common.py` & `notolog-0.9.0b9/notolog/lexemes/ko/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ko/main_menu.py` & `notolog-0.9.0b9/notolog/lexemes/ko/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ko/settings_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/ko/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ko/statusbar.py` & `notolog-0.9.0b9/notolog/lexemes/ko/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ko/toolbar.py` & `notolog-0.9.0b9/notolog/lexemes/ko/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/la/ai_assistant.py` & `notolog-0.9.0b9/notolog/lexemes/la/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/la/color_picker_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/la/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/la/common.py` & `notolog-0.9.0b9/notolog/lexemes/la/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/la/main_menu.py` & `notolog-0.9.0b9/notolog/lexemes/la/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/la/settings_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/la/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/la/statusbar.py` & `notolog-0.9.0b9/notolog/lexemes/la/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/la/toolbar.py` & `notolog-0.9.0b9/notolog/lexemes/la/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/lexemes.py` & `notolog-0.9.0b9/notolog/lexemes/lexemes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/pt/ai_assistant.py` & `notolog-0.9.0b9/notolog/lexemes/pt/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/pt/color_picker_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/pt/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/pt/common.py` & `notolog-0.9.0b9/notolog/lexemes/pt/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/pt/main_menu.py` & `notolog-0.9.0b9/notolog/lexemes/pt/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/pt/settings_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/pt/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/pt/statusbar.py` & `notolog-0.9.0b9/notolog/lexemes/pt/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/pt/toolbar.py` & `notolog-0.9.0b9/notolog/lexemes/pt/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ru/ai_assistant.py` & `notolog-0.9.0b9/notolog/lexemes/ru/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ru/color_picker_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/ru/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ru/common.py` & `notolog-0.9.0b9/notolog/lexemes/ru/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ru/main_menu.py` & `notolog-0.9.0b9/notolog/lexemes/ru/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ru/settings_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/ru/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ru/statusbar.py` & `notolog-0.9.0b9/notolog/lexemes/ru/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ru/toolbar.py` & `notolog-0.9.0b9/notolog/lexemes/ru/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/zh/ai_assistant.py` & `notolog-0.9.0b9/notolog/lexemes/zh/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/zh/color_picker_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/zh/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/zh/common.py` & `notolog-0.9.0b9/notolog/lexemes/zh/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/zh/main_menu.py` & `notolog-0.9.0b9/notolog/lexemes/zh/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/zh/settings_dialog.py` & `notolog-0.9.0b9/notolog/lexemes/zh/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/zh/statusbar.py` & `notolog-0.9.0b9/notolog/lexemes/zh/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/zh/toolbar.py` & `notolog-0.9.0b9/notolog/lexemes/zh/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/notolog_editor.py` & `notolog-0.9.0b9/notolog/notolog_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,35 +24,34 @@
 - Version: 0.9.0b0
 """
 
 """
 Main UI class to set up the application's UI and to process any user actions.
 """
 
-# Core classes
 from .settings import Settings
+from .ui.settings_dialog import SettingsDialog
 from .app_config import AppConfig
 from .file_header import FileHeader
 from .edit_widget import EditWidget
 from .view_widget import ViewWidget
 from .view_processor import ViewProcessor
 from .view_decorator import ViewDecorator
+from .ui.ai_assistant import AIAssistant
+from .ui.about_popup import AboutPopup
 
 # UI
 from .ui.file_system_model import FileSystemModel
 from .ui.sort_filter_proxy_model import SortFilterProxyModel
 from .ui.toolbar import ToolBar
 from .ui.statusbar import StatusBar
 from .ui.line_numbers import LineNumbers
 from .ui.common_dialog import CommonDialog
 from .ui.rename_file_dialog import RenameFileDialog
 from .ui.color_picker_dialog import ColorPickerDialog
-from .ui.settings_dialog import SettingsDialog
-from .ui.ai_assistant import AIAssistant
-from .ui.about_popup import AboutPopup
 
 # Highlight
 from .highlight.md_highlighter import MdHighlighter
 from .highlight.view_highlighter import ViewHighlighter
 
 # Encrypt
 from .encrypt.enc_helper import EncHelper
@@ -67,17 +66,14 @@
 from .helpers.clipboard_helper import ClipboardHelper
 from .helpers.update_helper import UpdateHelper
 from .helpers.file_helper import res_path, size_f, save_file
 
 # Lexemes
 from .lexemes.lexemes import Lexemes
 
-# Editor state
-from .editor_state import EditorState, Mode, Source, Encryption
-
 from PySide6.QtCore import Qt, QDir, QPoint, QTimer, QSize
 from PySide6.QtCore import QRegularExpression, QItemSelectionModel, QFileSystemWatcher
 from PySide6.QtGui import QGuiApplication, QIcon, QAction, QColor, QTextDocument, QShortcut
 from PySide6.QtGui import QKeySequence, QTextCursor, QFont, QTextBlock, QDesktopServices, QPalette
 from PySide6.QtWidgets import QWidget, QMainWindow, QVBoxLayout, QSplitter, QListView, QTextBrowser
 from PySide6.QtWidgets import QPlainTextEdit, QToolButton, QSizePolicy, QStatusBar, QCheckBox, QToolBar
 from PySide6.QtWidgets import QLabel, QLineEdit, QPushButton, QMenu, QDialog, QMessageBox, QStyle
@@ -92,20 +88,22 @@
 # Custom markdown extension to process element tree
 from .etree_extension import ElementTreeExtension
 
 # Emojis support
 import emoji
 
 import os
+import math
 import asyncio
-from pkg_resources import resource_filename
+
 from typing import Union, Optional, Callable, List, Dict, Any
 
 import logging
 
+from .editor_state import EditorState, Mode, Source, Encryption
 
 """
 To change content scale ratio use either:
     # View widget
     view_widget = self.get_view_widget()  # type: Union[ViewWidget, QTextBrowser]
     view_widget.setZoomFactor(float(self.scale))
 Or
@@ -3557,22 +3555,22 @@
         Helper: Default page when nothing else to show.
         """
         if (not ignore_settings
                 and self.settings.file_path is not None
                 and os.path.isfile(self.settings.file_path)):
             file_path = self.settings.file_path
         else:
-            # Default README.md file should be in the package
-            file_path = resource_filename('notolog', 'README.md')
+            # Default file should be in the package
+            script_dir = os.path.dirname(os.path.realpath(__file__))
+            package_dir = os.path.dirname(script_dir)
+            file_path = os.path.join(package_dir, 'README.md')
             # Fallback option
             if not os.path.isfile(file_path):
-                script_dir = os.path.dirname(os.path.realpath(__file__))
-                parent_dir = os.path.dirname(script_dir)
-                file_path = os.path.join(parent_dir, 'docs', 'Examples.md')
-            # file_path = res_path('README.md')  # Not working well with venv
+                file_path = os.path.join(package_dir, 'Examples.md')
+            # file_path = res_path('README.md')
         # If no file exist then try to load any file
         if file_path is not None and not os.path.isfile(file_path):
             file_path = self.get_any_file()
         if file_path is not None:
             return self.load_file(file_path)
         # The last fallback is try to create a new empty file
         return self.action_new_file()
```

### Comparing `notolog-0.9.0b10/app/settings.py` & `notolog-0.9.0b9/notolog/settings.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/text_block_data.py` & `notolog-0.9.0b9/notolog/text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/theme.py` & `notolog-0.9.0b9/notolog/theme.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/about_popup.py` & `notolog-0.9.0b9/notolog/ui/about_popup.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/ai_assistant.py` & `notolog-0.9.0b9/notolog/ui/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/color_picker_dialog.py` & `notolog-0.9.0b9/notolog/ui/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/common_dialog.py` & `notolog-0.9.0b9/notolog/ui/common_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/enum_combo_box.py` & `notolog-0.9.0b9/notolog/ui/enum_combo_box.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/file_system_model.py` & `notolog-0.9.0b9/notolog/ui/file_system_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/line_numbers.py` & `notolog-0.9.0b9/notolog/ui/line_numbers.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/rename_file_dialog.py` & `notolog-0.9.0b9/notolog/ui/rename_file_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/rotating_label.py` & `notolog-0.9.0b9/notolog/ui/rotating_label.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/settings_dialog.py` & `notolog-0.9.0b9/notolog/ui/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/sort_filter_proxy_model.py` & `notolog-0.9.0b9/notolog/ui/sort_filter_proxy_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/statusbar.py` & `notolog-0.9.0b9/notolog/ui/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/toolbar.py` & `notolog-0.9.0b9/notolog/ui/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/view_decorator.py` & `notolog-0.9.0b9/notolog/view_decorator.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/view_processor.py` & `notolog-0.9.0b9/notolog/view_processor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/view_widget.py` & `notolog-0.9.0b9/notolog/view_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/main.py` & `notolog-0.9.0b9/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 Author: Vadim Bakhrenkov
 License: MIT License
 """
 
 from PySide6.QtWidgets import QStyleFactory
 from qasync import QEventLoop, QApplication
 
-from app.app_config import AppConfig
-from app.notolog_editor import NotologEditor
+from notolog.app_config import AppConfig
+from notolog.notolog_editor import NotologEditor
 
 import platform
 import logging
 import asyncio
 import sys
```

### Comparing `notolog-0.9.0b10/notolog.egg-info/PKG-INFO` & `notolog-0.9.0b9/notolog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.0b10
+Version: 0.9.0b9
 Summary: Notolog Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
-License: MIT
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `notolog-0.9.0b10/setup.py` & `notolog-0.9.0b9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 
 # Read the contents of README file
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='notolog',
-    version='0.9.0b10',
+    version='0.9.0b9',
     description='Notolog Markdown Editor',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/notolog/notolog-editor',
     author='Vadim Bakhrenkov',
-    license='MIT',
     py_modules=['main'],
     entry_points={
         'console_scripts': [
             'notolog=main:main',
         ],
     },
     classifiers=[
@@ -29,18 +28,14 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3 :: Only',
     ],
     packages=find_packages(),  # Find all packages in the directory
     include_package_data=True,  # Include data files specified in MANIFEST.in
-    # package_data={
-    #    'notolog': ['docs/*.md'],
-    # },
-    # data_files=[('notolog-res', ['README.md'])],  # New dir with a content
     python_requires='>=3.9, <4',
     install_requires=[line.strip() for line in open("requirements.txt", "r")],
-    project_urls={
+    project_urls={  # Optional
         'Bug Reports': 'https://github.com/notolog/notolog-editor/issues',
         'Source': 'https://github.com/notolog/notolog-editor/',
     },
 )
```

### Comparing `notolog-0.9.0b10/tests/test_enc_helper.py` & `notolog-0.9.0b9/tests/test_enc_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # tests/test_enc_helper.py
-from app.encrypt.enc_helper import EncHelper
-from app.encrypt.enc_password import EncPassword
+from notolog.encrypt.enc_helper import EncHelper
+from notolog.encrypt.enc_password import EncPassword
 
 from cryptography.fernet import Fernet
 
 from logging import Logger
 
 import pytest
```

### Comparing `notolog-0.9.0b10/tests/test_enc_password.py` & `notolog-0.9.0b9/tests/test_enc_password.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # tests/test_enc_password.py
-from app.encrypt.enc_password import EncPassword
+from notolog.encrypt.enc_password import EncPassword
 
 import pytest
 
 
 class TestEncPassword:
 
     @pytest.fixture(scope="function", autouse=True)
```

### Comparing `notolog-0.9.0b10/tests/test_file_header.py` & `notolog-0.9.0b9/tests/test_file_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # tests/test_file_header.py
 
-from app.file_header import FileHeader
+from notolog.file_header import FileHeader
 
-from app.exceptions.file_header_empty_exception import FileHeaderEmptyException
+from notolog.exceptions.file_header_empty_exception import FileHeaderEmptyException
 
 from logging import Logger
 
 import pytest
 
 
 class TestFileHeader:
```

### Comparing `notolog-0.9.0b10/tests/test_html_view.py` & `notolog-0.9.0b9/tests/test_html_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # tests/test_html_view.py
 from PySide6.QtGui import QTextDocument, QFont
 
-from app.highlight.view_highlighter import ViewHighlighter
-from app.view_processor import ViewProcessor
-from app.view_decorator import ViewDecorator
+from notolog.highlight.view_highlighter import ViewHighlighter
+from notolog.view_processor import ViewProcessor
+from notolog.view_decorator import ViewDecorator
 
 import pytest
 
 
 class TestHtmlView:
 
     @pytest.fixture(scope="function", autouse=True)
```

### Comparing `notolog-0.9.0b10/tests/test_lexemes.py` & `notolog-0.9.0b9/tests/test_lexemes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # tests/test_lexemes.py
 
-from app.lexemes.lexemes import Lexemes
+from notolog.lexemes.lexemes import Lexemes
 
 from logging import Logger
 
 import pytest
 import os
```

### Comparing `notolog-0.9.0b10/tests/test_notolog_editor.py` & `notolog-0.9.0b9/tests/test_notolog_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # tests/test_notolog_editor.py
 
-from app.notolog_editor import NotologEditor
-from app.settings import Settings
-from app.editor_state import Mode
-from app.lexemes.lexemes import Lexemes
+from notolog.notolog_editor import NotologEditor
+from notolog.settings import Settings
+from notolog.editor_state import Mode
+from notolog.lexemes.lexemes import Lexemes
 
 import pytest
 
 import os
 
 
 class TestNotologEditor:
```

### Comparing `notolog-0.9.0b10/tests/test_settings.py` & `notolog-0.9.0b9/tests/test_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # tests/test_settings.py
-from app.settings import Settings
+from notolog.settings import Settings
 
 import pytest
 
 class TestSettings():
 
     def test_settings_defaults(self):
         obj = Settings()
```

### Comparing `notolog-0.9.0b10/tests/test_text_block_data.py` & `notolog-0.9.0b9/tests/test_text_block_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # tests/test_text_block_data.py
-from app.text_block_data import TextBlockData
+from notolog.text_block_data import TextBlockData
 
 import pytest
 
 
 class TestTextBlockData:
 
     @pytest.fixture(scope="class", autouse=True)
```

### Comparing `notolog-0.9.0b10/tests/test_theme_helper.py` & `notolog-0.9.0b9/tests/test_theme_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # tests/test_themes.py
 
-from app.helpers.theme_helper import ThemeHelper
-from app.enums.themes import Themes
-from app.theme import Theme
-from app.settings import Settings
-from app.app_config import AppConfig
+from notolog.helpers.theme_helper import ThemeHelper
+from notolog.enums.themes import Themes
+from notolog.theme import Theme
+from notolog.settings import Settings
+from notolog.app_config import AppConfig
 
 from logging import Logger
 
 import os
 import pytest
```

### Comparing `notolog-0.9.0b10/tests/test_themes.py` & `notolog-0.9.0b9/tests/test_themes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # tests/test_themes.py
 
-from app.theme import Theme
+from notolog.theme import Theme
 
 from logging import Logger
 
 import pytest
 import os
```

