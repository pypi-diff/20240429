# Comparing `tmp/ns_asphalt9-3.4.1.tar.gz` & `tmp/ns_asphalt9-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_asphalt9-3.4.1.tar", last modified: Mon Apr 29 11:09:04 2024, max compression
+gzip compressed data, was "ns_asphalt9-3.4.2.tar", last modified: Mon Apr 29 11:42:30 2024, max compression
```

## Comparing `ns_asphalt9-3.4.1.tar` & `ns_asphalt9-3.4.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.185722 ns_asphalt9-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-29 11:09:04.185722 ns_asphalt9-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.173721 ns_asphalt9-3.4.1/ns_asphalt9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.177722 ns_asphalt9-3.4.1/ns_asphalt9/core/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.181722 ns_asphalt9-3.4.1/ns_asphalt9/core/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/actions/autocode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/capture.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.181722 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47865 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.181722 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/console.png
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 runner    (1001) docker     (127)   202347 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/record.png
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward.png
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward1.png
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward2.png
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward3.png
--rw-r--r--   0 runner    (1001) docker     (127)   116019 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward_qrcode.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/screen.png
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    20338 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/reset_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.185722 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/error_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/lifo_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/online_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/page_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/process_record_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/thread_lifo_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    43083 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    27139 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data_win.py
--rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.185722 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-29 11:09:04.000000 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-29 11:09:04.000000 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:09:04.000000 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 11:09:04.000000 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:09:03.000000 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-29 11:09:04.000000 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 11:09:04.000000 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-29 11:09:04.189722 ns_asphalt9-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.185722 ns_asphalt9-3.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/tests/test_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:42:30.108762 ns_asphalt9-3.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-29 11:42:30.108762 ns_asphalt9-3.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:42:30.096762 ns_asphalt9-3.4.2/ns_asphalt9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:42:30.100762 ns_asphalt9-3.4.2/ns_asphalt9/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:42:30.100762 ns_asphalt9-3.4.2/ns_asphalt9/core/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/actions/autocode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:42:30.100762 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47865 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:42:30.104762 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/console.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 runner    (1001) docker     (127)   202347 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/record.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/reward.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/reward1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/reward2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/reward3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   116019 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/reward_qrcode.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/screen.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20338 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/reset_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:42:30.108762 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/error_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/lifo_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/online_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/page_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/process_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/thread_lifo_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43083 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/track_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/track_navi_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/track_navi_data_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/track_navi_data_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27139 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/core/utils/track_navi_data_win.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/ns_asphalt9/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:42:30.108762 ns_asphalt9-3.4.2/ns_asphalt9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-29 11:42:30.000000 ns_asphalt9-3.4.2/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-29 11:42:30.000000 ns_asphalt9-3.4.2/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:42:30.000000 ns_asphalt9-3.4.2/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 11:42:30.000000 ns_asphalt9-3.4.2/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:42:29.000000 ns_asphalt9-3.4.2/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-29 11:42:30.000000 ns_asphalt9-3.4.2/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 11:42:30.000000 ns_asphalt9-3.4.2/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-29 11:42:30.108762 ns_asphalt9-3.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:42:30.108762 ns_asphalt9-3.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-29 11:42:25.000000 ns_asphalt9-3.4.2/tests/test_pages.py
```

### Comparing `ns_asphalt9-3.4.1/LICENSE` & `ns_asphalt9-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/PKG-INFO` & `ns_asphalt9-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 3.4.1
+Version: 3.4.2
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-3.4.1/README.md` & `ns_asphalt9-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/actions/__init__.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/actions/autocode.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/actions/autocode.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/actions/common.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/actions/common.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/actions/enter_page.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/actions/process_race.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/actions/select_car.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/cache.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/capture.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/capture.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/consts.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/consts.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/controller.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/controller.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/event.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/event.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/globals.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/globals.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/gui/app.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/console.png` & `ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/console.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/record.png` & `ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/record.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward.png` & `ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/reward.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward1.png` & `ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/reward1.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward2.png` & `ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/reward2.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward3.png` & `ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/reward3.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward_qrcode.jpeg` & `ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/reward_qrcode.jpeg`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/screen.png` & `ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/screen.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-3.4.2/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/ocr.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/ocr.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/page_factory.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/pages.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/pages.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/reset_data.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/reset_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/tasks.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/tasks.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/test.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/test.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/count.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/count.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/credits.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/credits.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/error_process.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/error_process.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/lifo_queue.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/lifo_queue.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/notify.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/notify.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/online_tracker.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/online_tracker.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/page_stack.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/page_stack.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/process_record_data.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/process_record_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/thread_lifo_queue.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/thread_lifo_queue.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_data.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/track_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/track_navi_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data_update.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/track_navi_data_update.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data_v2.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/track_navi_data_v2.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data_win.py` & `ns_asphalt9-3.4.2/ns_asphalt9/core/utils/track_navi_data_win.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9/main.py` & `ns_asphalt9-3.4.2/ns_asphalt9/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,15 +493,15 @@
     cap.set(cv2.CAP_PROP_FPS, int(fps))
 
     if not cap.isOpened():
         logger.info("无法打开视频设备")
     # 循环读取视频帧并显示
     while True:
         # 读取一帧图像
-        if G.video_setting_queue.not_empty():
+        if not G.video_setting_queue.empty():
             # 重新设置视频参数
             setting = G.video_setting_queue.get()
             setting_device_id = setting["设备"]
             setting_fps = setting["帧率"]
             setting_w, setting_h = setting["分辨率"].split("*")
             try:
                 if setting_device_id != device:
```

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-3.4.2/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 3.4.1
+Version: 3.4.2
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-3.4.1/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-3.4.2/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.1/setup.cfg` & `ns_asphalt9-3.4.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 3.4.1
+version = 3.4.2
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

### Comparing `ns_asphalt9-3.4.1/tests/test_pages.py` & `ns_asphalt9-3.4.2/tests/test_pages.py`

 * *Files identical despite different names*

