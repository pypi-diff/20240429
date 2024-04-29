# Comparing `tmp/ns_asphalt9-3.4.0.tar.gz` & `tmp/ns_asphalt9-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_asphalt9-3.4.0.tar", last modified: Sun Apr 28 17:02:37 2024, max compression
+gzip compressed data, was "ns_asphalt9-3.4.1.tar", last modified: Mon Apr 29 11:09:04 2024, max compression
```

## Comparing `ns_asphalt9-3.4.0.tar` & `ns_asphalt9-3.4.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.826328 ns_asphalt9-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-28 17:02:37.826328 ns_asphalt9-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.814328 ns_asphalt9-3.4.0/ns_asphalt9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.818328 ns_asphalt9-3.4.0/ns_asphalt9/core/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.822328 ns_asphalt9-3.4.0/ns_asphalt9/core/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/actions/autocode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/capture.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.822328 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45507 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.822328 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/console.png
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 runner    (1001) docker     (127)   202347 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/record.png
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward.png
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward1.png
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward2.png
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward3.png
--rw-r--r--   0 runner    (1001) docker     (127)   116019 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward_qrcode.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/screen.png
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    20338 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/reset_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.826328 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/error_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/lifo_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/online_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/page_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/process_record_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/thread_lifo_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    43083 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    27139 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data_win.py
--rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/ns_asphalt9/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.826328 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-28 17:02:37.000000 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-28 17:02:37.000000 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:02:37.000000 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-28 17:02:37.000000 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:02:37.000000 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-28 17:02:37.000000 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 17:02:37.000000 ns_asphalt9-3.4.0/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-28 17:02:37.830328 ns_asphalt9-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:02:37.826328 ns_asphalt9-3.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-28 17:02:33.000000 ns_asphalt9-3.4.0/tests/test_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.185722 ns_asphalt9-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-29 11:09:04.185722 ns_asphalt9-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.173721 ns_asphalt9-3.4.1/ns_asphalt9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.177722 ns_asphalt9-3.4.1/ns_asphalt9/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.181722 ns_asphalt9-3.4.1/ns_asphalt9/core/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/actions/autocode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.181722 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47865 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.181722 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/console.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 runner    (1001) docker     (127)   202347 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/record.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   116019 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward_qrcode.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/screen.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20338 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/reset_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.185722 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/error_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/lifo_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/online_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/page_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/process_record_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/thread_lifo_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43083 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27139 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data_win.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/ns_asphalt9/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.185722 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-29 11:09:04.000000 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-29 11:09:04.000000 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:09:04.000000 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 11:09:04.000000 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:09:03.000000 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-29 11:09:04.000000 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 11:09:04.000000 ns_asphalt9-3.4.1/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-29 11:09:04.189722 ns_asphalt9-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:09:04.185722 ns_asphalt9-3.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-29 11:08:58.000000 ns_asphalt9-3.4.1/tests/test_pages.py
```

### Comparing `ns_asphalt9-3.4.0/LICENSE` & `ns_asphalt9-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/PKG-INFO` & `ns_asphalt9-3.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 3.4.0
+Version: 3.4.1
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-3.4.0/README.md` & `ns_asphalt9-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/actions/__init__.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/actions/autocode.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/actions/autocode.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/actions/common.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/actions/common.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/actions/enter_page.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/actions/process_race.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/actions/select_car.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/cache.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/capture.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/capture.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/consts.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/consts.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/controller.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/controller.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/event.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/event.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/globals.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/globals.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 notify_queue = queue.Queue()
 
 frame_queue = LIFOQueue()
 
 task_queue = queue.Queue()
 video_queue = queue.Queue(maxsize=10)
 
+# 视频设置队列
+video_setting_queue = queue.Queue()
+
 CONFIG = None
 
 # 回放停止事件
 G_REPLAY_RUN = threading.Event()
 G_REPLAY_STOP = threading.Event()
 
 G_OCR_PROGRESS = threading.Event()
```

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -517,15 +517,15 @@
             pady=20,
             sticky="",
         )
 
         self.record_mode_option = customtkinter.CTkOptionMenu(
             record_group_frame,
             dynamic_resizing=False,
-            values=["普通", "导航"],
+            values=["脚本", "导航"],
             width=120,
             height=28,
             button_color="black",
             fg_color="black",
             text_color="white",
             button_hover_color=("gray70", "gray30"),
             command=self.save_settings,
@@ -597,21 +597,23 @@
             columnspan=1,
             padx=20,
             pady=20,
             sticky="",
         )
 
         def update_replay_options(**kwargs):
-            # 指定文件路径
-            path = "./record"
-            if not os.path.exists(path):
-                os.makedirs(path)
-            entries = os.listdir(path)
-            files = [f for f in entries if os.path.isfile(os.path.join(path, f))]
-            return files
+            root_path = "./record"
+            if not os.path.exists(root_path):
+                os.makedirs(root_path)
+            file_list = []
+            for root, _, files in os.walk(root_path):
+                for file in files:
+                    if file.endswith((".json", ".py")):
+                        file_list.append(os.path.join(root, file))
+            return file_list
 
         self.replay_file_option = customtkinter.CTkOptionMenu(
             replay_group_frame,
             dynamic_resizing=False,
             values=update_replay_options(),
             width=120,
             height=28,
@@ -731,15 +733,28 @@
         """配置页"""
         self.setting_modules = {}
         self.settings = customtkinter.CTkScrollableFrame(
             self, corner_radius=0, fg_color="transparent"
         )
 
         for row, label_text in enumerate(
-            ["模式", "任务", "多一", "多二", "寻车", "传奇寻车", "多三", "大奖赛", "通知", "自定义", "重置"]
+            [
+                "模式",
+                "任务",
+                "多一",
+                "多二",
+                "寻车",
+                "传奇寻车",
+                "多三",
+                "大奖赛",
+                "通知",
+                "自定义",
+                "视频设置",
+                "手柄设置",
+            ]
         ):
             label = customtkinter.CTkLabel(master=self.settings, text=f"{label_text}:")
             label.grid(
                 row=row,
                 column=0,
                 columnspan=1,
                 padx=10,
@@ -785,16 +800,16 @@
             key="自定义",
             add_event_position=True,
             add_event_type=True,
             add_reset_type=True,
             add_feature_option=True,
             car_num=8,
         )
-        # 通知配置
-        # self._build_reset(row=10)
+        # 视频配置
+        self._build_video(row=10)
 
     def _build_mode(self):
         """模式设置选项"""
         self.mode = tkinter.StringVar()
         self.mode_buttons = customtkinter.CTkSegmentedButton(
             self.settings,
             variable=self.mode,
@@ -928,17 +943,17 @@
             row=row, column=1, columnspan=2, padx=(20, 0), pady=(20, 0), sticky="nsew"
         )
         self._build_navi_box(frame, key)
         base_row = 1
         if add_event_position:
             car_hunt_position = customtkinter.CTkLabel(master=frame, text="位置:")
             car_hunt_position.grid(row=1, column=0, padx=(15, 10), pady=(10, 10))
-            position_option = customtkinter.CTkOptionMenu(
+            position_option = customtkinter.CTkComboBox(
                 frame,
-                dynamic_resizing=False,
+                # dynamic_resizing=False,
                 values=[str(i) for i in range(0, 20)],
                 width=100,
                 height=28,
                 command=self.save_settings,
             )
 
             position_option.grid(row=1, column=1, padx=(10, 10), pady=(10, 10))
@@ -1102,60 +1117,109 @@
         if self.settings_data and "通知" in self.settings_data:
             host_input.insert(0, self.settings_data["通知"]["Host"])
             key_input.insert(0, self.settings_data["通知"]["Key"])
 
         self.setting_modules["通知"]["Host"] = host_input
         self.setting_modules["通知"]["Key"] = key_input
 
-    def _build_reset(self, row=8):
-        """重置配置"""
-
-        reset_setting_frame = customtkinter.CTkFrame(self.settings, width=340)
-        reset_setting_frame.grid(
+    def _build_video(self, row=8):
+        """视频配置"""
+        self.setting_modules["视频"] = {}
+        video_setting_frame = customtkinter.CTkFrame(self.settings, width=340)
+        video_setting_frame.grid(
             row=10, column=1, columnspan=2, padx=(20, 0), pady=(20, 20), sticky="nsew"
         )
-        reset_button = customtkinter.CTkButton(
-            text="重置配置",
-            command=self.reset_settings,
-            master=reset_setting_frame,
-            width=200,
+
+        device_label = customtkinter.CTkLabel(master=video_setting_frame, text="设备:")
+        device_label.grid(row=0, column=0, padx=(15, 10), pady=(10, 10))
+
+        device_option = customtkinter.CTkOptionMenu(
+            video_setting_frame,
+            dynamic_resizing=False,
+            values=[str(i) for i in range(4)],
+            width=100,
+            height=28,
+            command=self.save_settings,
+        )
+        device_option.grid(row=0, column=1, padx=(10, 10), pady=(10, 10))
+
+        frame_label = customtkinter.CTkLabel(master=video_setting_frame, text="帧率:")
+        frame_label.grid(row=1, column=0, padx=(15, 10), pady=(10, 10))
+
+        frame_option = customtkinter.CTkOptionMenu(
+            video_setting_frame,
+            dynamic_resizing=False,
+            values=["20", "60", "30", "25", "10"],
+            width=100,
             height=28,
+            command=self.save_settings,
         )
-        reset_button.grid(row=1, column=1, padx=(10, 10), pady=(10, 10))
+        frame_option.grid(row=1, column=1, padx=(10, 10), pady=(10, 10))
 
-    def reset_settings(self):
-        os.remove("./settings.json")
-        self.settings_data = None
-        self.save_settings()
+        resolution_label = customtkinter.CTkLabel(
+            master=video_setting_frame, text="分辨率:"
+        )
+        resolution_label.grid(row=2, column=0, padx=(15, 10), pady=(10, 10))
+
+        resolution_option = customtkinter.CTkOptionMenu(
+            video_setting_frame,
+            dynamic_resizing=False,
+            values=[
+                "640*480",
+                "720*480",
+                "720*576",
+                "800*600",
+                "1024*768",
+                "1280*720",
+                "1280*960",
+                "1280*1024",
+                "1360*768",
+                "1600*1200",
+                "1920*1080",
+            ],
+            width=100,
+            height=28,
+            command=self.save_settings,
+        )
+        resolution_option.grid(row=2, column=1, padx=(10, 10), pady=(10, 10))
+
+        if self.settings_data and "视频" in self.settings_data:
+            device_option.set(self.settings_data["视频"]["设备"])
+            frame_option.set(self.settings_data["视频"]["帧率"])
+            resolution_option.set(self.settings_data["视频"]["分辨率"])
+
+        self.setting_modules["视频"]["设备"] = device_option
+        self.setting_modules["视频"]["帧率"] = frame_option
+        self.setting_modules["视频"]["分辨率"] = resolution_option
 
     def _build_car_position(
         self, frame, module_container, data_container, base_row, num=6
     ):
         """车库位置配置"""
         car_position = customtkinter.CTkLabel(master=frame, text="车库位置:")
         car_position.grid(row=base_row, column=0, padx=(15, 10), pady=(10, 10))
         row = customtkinter.CTkLabel(master=frame, text="row")
         row.grid(row=base_row, column=1, padx=(0, 0), pady=(10, 10), sticky="nsew")
         col = customtkinter.CTkLabel(master=frame, text="col")
         col.grid(row=base_row, column=2, padx=(0, 10), pady=(10, 10), sticky="nsew")
         module_container["车库位置"] = []
 
         for r in range(num):
-            option1 = customtkinter.CTkOptionMenu(
+            option1 = customtkinter.CTkComboBox(
                 frame,
-                dynamic_resizing=False,
+                # dynamic_resizing=False,
                 values=[str(i) for i in range(0, 3)],
                 width=100,
                 height=28,
                 command=self.save_settings,
             )
 
-            option2 = customtkinter.CTkOptionMenu(
+            option2 = customtkinter.CTkComboBox(
                 frame,
-                dynamic_resizing=False,
+                # dynamic_resizing=False,
                 values=[str(i) for i in range(0, 40)],
                 width=100,
                 height=28,
                 command=self.save_settings,
             )
 
             option1.grid(row=r + base_row + 1, column=1, padx=(10, 10), pady=(10, 10))
@@ -1188,14 +1252,16 @@
                 return res
             elif isinstance(objs, list):
                 res = []
                 for obj in objs:
                     res.append(get_value(obj))
                 return res
             elif isinstance(objs, str):
+                if objs.isdigit():
+                    return int(objs)
                 return objs
             else:
                 return objs.get()
 
         def convert_dict_values(data):
             if isinstance(data, dict):
                 for key, value in data.items():
```

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/console.png` & `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/console.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/record.png` & `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/record.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward.png` & `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward1.png` & `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward1.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward2.png` & `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward2.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward3.png` & `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward3.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/reward_qrcode.jpeg` & `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/reward_qrcode.jpeg`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/screen.png` & `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/screen.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-3.4.1/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/ocr.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/ocr.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/page_factory.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/pages.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/pages.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/reset_data.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/reset_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/tasks.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/tasks.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/test.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/test.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/count.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/count.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/credits.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/credits.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/error_process.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/error_process.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/lifo_queue.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/lifo_queue.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/notify.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/notify.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/online_tracker.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/online_tracker.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/page_stack.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/page_stack.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/process_record_data.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/process_record_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/thread_lifo_queue.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/thread_lifo_queue.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_data.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data_update.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data_update.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data_v2.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data_v2.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/core/utils/track_navi_data_win.py` & `ns_asphalt9-3.4.1/ns_asphalt9/core/utils/track_navi_data_win.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9/main.py` & `ns_asphalt9-3.4.1/ns_asphalt9/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -157,15 +157,15 @@
                     record_data = []
 
             elif "start_replay" in command:
                 _, filename, replay_times = command.split(" ")
                 logger.info(f"开始回放 {filename} 回放次数 {replay_times}")
 
                 if filename.endswith(".py"):
-                    with open(os.path.join("./record", filename)) as file:
+                    with open(filename) as file:
                         replay_text = file.read()
 
                     def replay_worker(replay_text, replay_times):
                         try:
                             for index in range(int(replay_times)):
                                 if not G.G_REPLAY_RUN.is_set():
                                     break
@@ -180,15 +180,15 @@
                         target=replay_worker,
                         args=(replay_text, replay_times),
                         daemon=True,
                     )
                     t.start()
 
                 else:
-                    with open(os.path.join("./record", filename)) as file:
+                    with open(filename) as file:
                         navi_data = json.load(file)
                     logger.info(f"Load navi data {navi_data}")
 
                     def replay_navi_worker(navi_data):
                         processed_data = []
                         showed_progress = [-1]
                         last_button = None
@@ -344,15 +344,18 @@
                                 "event_type": command["action"],
                                 "control_data": control_data,
                             }
                         )
                     G.input_packet["packet"] = packet
                 else:
                     logger.info("Received config update message.")
+                    if G.CONFIG is None or G.CONFIG["视频"] != command["视频"]:
+                        G.video_setting_queue.put(command["视频"])
                     G.CONFIG = command
+
             except Exception as err:
                 logger.info(
                     f"{command} process err = {err} traceback = {traceback.format_exc()}"
                 )
         else:
             logger.info(f"{command} command not support!")
 
@@ -475,25 +478,51 @@
     except subprocess.CalledProcessError:
         output = "Package not found."
 
     logger.info(output)
 
 
 def stream_worker():
-    cap = cv2.VideoCapture("/dev/video0")
+    device = "/dev/video0"
+    width = "640"
+    height = "480"
+    fps = "20"
+    cap = cv2.VideoCapture(device)
     cap.set(cv2.CAP_PROP_FOURCC, cv2.VideoWriter_fourcc(*"MJPG"))
-    cap.set(cv2.CAP_PROP_FRAME_WIDTH, 640)
-    cap.set(cv2.CAP_PROP_FRAME_HEIGHT, 480)
-    cap.set(cv2.CAP_PROP_FPS, 20)
+    cap.set(cv2.CAP_PROP_FRAME_WIDTH, int(width))
+    cap.set(cv2.CAP_PROP_FRAME_HEIGHT, int(height))
+    cap.set(cv2.CAP_PROP_FPS, int(fps))
 
     if not cap.isOpened():
         logger.info("无法打开视频设备")
     # 循环读取视频帧并显示
     while True:
         # 读取一帧图像
+        if G.video_setting_queue.not_empty():
+            # 重新设置视频参数
+            setting = G.video_setting_queue.get()
+            setting_device_id = setting["设备"]
+            setting_fps = setting["帧率"]
+            setting_w, setting_h = setting["分辨率"].split("*")
+            try:
+                if setting_device_id != device:
+                    cap = cv2.VideoCapture(device)
+                    cap.set(cv2.CAP_PROP_FOURCC, cv2.VideoWriter_fourcc(*"MJPG"))
+                if setting_h != height:
+                    cap.set(cv2.CAP_PROP_FRAME_HEIGHT, int(setting_h))
+                    height = setting_h
+                if setting_w != width:
+                    cap.set(cv2.CAP_PROP_FRAME_WIDTH, int(setting_w))
+                    width = setting_w
+                if setting_fps != fps:
+                    cap.set(cv2.CAP_PROP_FPS, int(setting_fps))
+                    fps = setting_fps
+            except Exception as err:
+                logger.info(f"设置视频参数时发生错误: {err}")
+
         ret, frame = cap.read()
         # 如果正确读取帧，ret为True
         if not ret:
             logger.info("无法获取视频帧")
             continue
         # 显示帧
         G.frame_queue.push(frame)
```

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-3.4.1/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 3.4.0
+Version: 3.4.1
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-3.4.0/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-3.4.1/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-3.4.0/setup.cfg` & `ns_asphalt9-3.4.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 3.4.0
+version = 3.4.1
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

### Comparing `ns_asphalt9-3.4.0/tests/test_pages.py` & `ns_asphalt9-3.4.1/tests/test_pages.py`

 * *Files identical despite different names*

