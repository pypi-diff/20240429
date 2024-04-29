# Comparing `tmp/python-rucaptcha-6.1.2.tar.gz` & `tmp/python_rucaptcha-6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-rucaptcha-6.1.2.tar", last modified: Wed Jan  3 21:00:38 2024, max compression
+gzip compressed data, was "python_rucaptcha-6.2.tar", last modified: Mon Apr 29 16:58:03 2024, max compression
```

## Comparing `python-rucaptcha-6.1.2.tar` & `python_rucaptcha-6.2.tar`

### file list

```diff
@@ -1,44 +1,75 @@
-drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-01-03 21:00:38.935282 python-rucaptcha-6.1.2/
--rw-r--r--   0 homea     (1000) homea     (1000)     6711 2024-01-03 21:00:38.935282 python-rucaptcha-6.1.2/PKG-INFO
-drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-01-03 21:00:38.935282 python-rucaptcha-6.1.2/python_rucaptcha/
--rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-08-07 00:04:54.000000 python-rucaptcha-6.1.2/python_rucaptcha/__init__.py
--rw-r--r--   0 homea     (1000) homea     (1000)       22 2024-01-03 18:42:16.000000 python-rucaptcha-6.1.2/python_rucaptcha/__version__.py
--rw-r--r--   0 homea     (1000) homea     (1000)     3625 2023-12-08 01:06:23.000000 python-rucaptcha-6.1.2/python_rucaptcha/amazon_waf.py
--rw-r--r--   0 homea     (1000) homea     (1000)     5600 2023-12-08 01:10:22.000000 python-rucaptcha-6.1.2/python_rucaptcha/audio_captcha.py
--rw-rw-r--   0 homea     (1000) homea     (1000)    10648 2023-12-13 17:08:05.000000 python-rucaptcha-6.1.2/python_rucaptcha/bounding_box_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4973 2023-12-08 01:06:23.000000 python-rucaptcha-6.1.2/python_rucaptcha/capy_puzzle.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4818 2023-12-06 15:44:04.000000 python-rucaptcha-6.1.2/python_rucaptcha/control.py
--rw-rw-r--   0 homea     (1000) homea     (1000)     9911 2023-12-13 17:28:05.000000 python-rucaptcha-6.1.2/python_rucaptcha/coordinates_captcha.py
-drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-01-03 21:00:38.935282 python-rucaptcha-6.1.2/python_rucaptcha/core/
--rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-08-07 00:04:54.000000 python-rucaptcha-6.1.2/python_rucaptcha/core/__init__.py
--rw-r--r--   0 homea     (1000) homea     (1000)     9315 2023-12-08 15:52:15.000000 python-rucaptcha-6.1.2/python_rucaptcha/core/base.py
--rw-r--r--   0 homea     (1000) homea     (1000)      553 2023-12-08 00:41:48.000000 python-rucaptcha-6.1.2/python_rucaptcha/core/config.py
--rw-r--r--   0 homea     (1000) homea     (1000)     3552 2024-01-03 17:56:50.000000 python-rucaptcha-6.1.2/python_rucaptcha/core/enums.py
--rw-r--r--   0 homea     (1000) homea     (1000)     2680 2023-12-06 16:42:40.000000 python-rucaptcha-6.1.2/python_rucaptcha/core/result_handler.py
--rw-r--r--   0 homea     (1000) homea     (1000)     1739 2023-12-14 13:52:15.000000 python-rucaptcha-6.1.2/python_rucaptcha/core/serializer.py
--rw-rw-r--   0 homea     (1000) homea     (1000)     4028 2023-12-08 16:18:54.000000 python-rucaptcha-6.1.2/python_rucaptcha/cutcaptcha.py
--rw-rw-r--   0 homea     (1000) homea     (1000)     3909 2023-12-10 20:45:24.000000 python-rucaptcha-6.1.2/python_rucaptcha/cyber_siara_captcha.py
--rw-rw-r--   0 homea     (1000) homea     (1000)     4140 2023-12-10 15:44:52.000000 python-rucaptcha-6.1.2/python_rucaptcha/datadome_captcha.py
--rw-rw-r--   0 homea     (1000) homea     (1000)    11837 2023-12-13 17:14:39.000000 python-rucaptcha-6.1.2/python_rucaptcha/draw_around_captcha.py
--rw-rw-r--   0 homea     (1000) homea     (1000)     4232 2024-01-03 17:59:23.000000 python-rucaptcha-6.1.2/python_rucaptcha/friendly_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     3496 2023-12-08 01:06:23.000000 python-rucaptcha-6.1.2/python_rucaptcha/fun_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     8583 2023-12-13 23:09:36.000000 python-rucaptcha-6.1.2/python_rucaptcha/gee_test.py
--rw-rw-r--   0 homea     (1000) homea     (1000)     9001 2023-12-13 17:40:40.000000 python-rucaptcha-6.1.2/python_rucaptcha/grid_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     3732 2023-12-08 01:07:51.000000 python-rucaptcha-6.1.2/python_rucaptcha/hcaptcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     8391 2023-12-07 21:35:13.000000 python-rucaptcha-6.1.2/python_rucaptcha/image_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4017 2023-12-08 01:09:26.000000 python-rucaptcha-6.1.2/python_rucaptcha/key_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4064 2023-12-08 01:06:23.000000 python-rucaptcha-6.1.2/python_rucaptcha/lemin_captcha.py
--rw-rw-r--   0 homea     (1000) homea     (1000)     3415 2023-12-11 01:15:38.000000 python-rucaptcha-6.1.2/python_rucaptcha/mt_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     6083 2023-12-08 01:11:14.000000 python-rucaptcha-6.1.2/python_rucaptcha/re_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     6225 2023-12-07 21:55:48.000000 python-rucaptcha-6.1.2/python_rucaptcha/rotate_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     3708 2023-12-06 16:37:43.000000 python-rucaptcha-6.1.2/python_rucaptcha/text_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     3686 2023-12-08 01:06:23.000000 python-rucaptcha-6.1.2/python_rucaptcha/turnstile.py
-drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-01-03 21:00:38.935282 python-rucaptcha-6.1.2/python_rucaptcha.egg-info/
--rw-r--r--   0 homea     (1000) homea     (1000)     6711 2024-01-03 21:00:38.000000 python-rucaptcha-6.1.2/python_rucaptcha.egg-info/PKG-INFO
--rw-rw-r--   0 homea     (1000) homea     (1000)     1284 2024-01-03 21:00:38.000000 python-rucaptcha-6.1.2/python_rucaptcha.egg-info/SOURCES.txt
--rw-rw-r--   0 homea     (1000) homea     (1000)        1 2024-01-03 21:00:38.000000 python-rucaptcha-6.1.2/python_rucaptcha.egg-info/dependency_links.txt
--rw-rw-r--   0 homea     (1000) homea     (1000)        1 2024-01-03 18:26:24.000000 python-rucaptcha-6.1.2/python_rucaptcha.egg-info/not-zip-safe
--rw-rw-r--   0 homea     (1000) homea     (1000)       64 2024-01-03 21:00:38.000000 python-rucaptcha-6.1.2/python_rucaptcha.egg-info/requires.txt
--rw-rw-r--   0 homea     (1000) homea     (1000)       17 2024-01-03 21:00:38.000000 python-rucaptcha-6.1.2/python_rucaptcha.egg-info/top_level.txt
--rw-rw-r--   0 homea     (1000) homea     (1000)       38 2024-01-03 21:00:38.935282 python-rucaptcha-6.1.2/setup.cfg
--rw-r--r--   0 homea     (1000) homea     (1000)     4175 2024-01-03 18:02:48.000000 python-rucaptcha-6.1.2/setup.py
+drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-04-29 16:58:03.229532 python_rucaptcha-6.2/
+-rw-rw-r--   0 homea     (1000) homea     (1000)     1063 2023-04-28 18:48:47.000000 python_rucaptcha-6.2/LICENSE
+-rw-rw-r--   0 homea     (1000) homea     (1000)       25 2021-01-10 17:03:02.000000 python_rucaptcha-6.2/MANIFEST.in
+-rw-r--r--   0 homea     (1000) homea     (1000)     8827 2024-04-29 16:58:03.229532 python_rucaptcha-6.2/PKG-INFO
+-rw-r--r--   0 homea     (1000) homea     (1000)     7068 2024-04-25 22:18:05.000000 python_rucaptcha-6.2/README.md
+-rw-r--r--   0 homea     (1000) homea     (1000)     2581 2024-04-29 16:49:57.000000 python_rucaptcha-6.2/pyproject.toml
+-rw-rw-r--   0 homea     (1000) homea     (1000)       38 2024-04-29 16:58:03.229532 python_rucaptcha-6.2/setup.cfg
+drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-04-29 16:58:03.220532 python_rucaptcha-6.2/src/
+drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-04-29 16:58:03.224532 python_rucaptcha-6.2/src/python_rucaptcha/
+-rw-r--r--   0 homea     (1000) homea     (1000)       61 2024-04-29 16:50:38.000000 python_rucaptcha-6.2/src/python_rucaptcha/__init__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)       20 2024-04-29 16:51:36.000000 python_rucaptcha-6.2/src/python_rucaptcha/__version__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3625 2023-12-08 01:06:23.000000 python_rucaptcha-6.2/src/python_rucaptcha/amazon_waf.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     3701 2024-04-29 16:24:14.000000 python_rucaptcha-6.2/src/python_rucaptcha/atb_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     5600 2023-12-08 01:10:22.000000 python_rucaptcha-6.2/src/python_rucaptcha/audio_captcha.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)    10648 2023-12-13 17:08:05.000000 python_rucaptcha-6.2/src/python_rucaptcha/bounding_box_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4973 2023-12-08 01:06:23.000000 python_rucaptcha-6.2/src/python_rucaptcha/capy_puzzle.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4988 2024-04-29 15:18:24.000000 python_rucaptcha-6.2/src/python_rucaptcha/control.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     9911 2023-12-13 17:28:05.000000 python_rucaptcha-6.2/src/python_rucaptcha/coordinates_captcha.py
+drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-04-29 16:58:03.225532 python_rucaptcha-6.2/src/python_rucaptcha/core/
+-rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-08-07 00:04:54.000000 python_rucaptcha-6.2/src/python_rucaptcha/core/__init__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     9315 2023-12-08 15:52:15.000000 python_rucaptcha-6.2/src/python_rucaptcha/core/base.py
+-rw-r--r--   0 homea     (1000) homea     (1000)      553 2023-12-08 00:41:48.000000 python_rucaptcha-6.2/src/python_rucaptcha/core/config.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3797 2024-04-29 16:22:42.000000 python_rucaptcha-6.2/src/python_rucaptcha/core/enums.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     2680 2023-12-06 16:42:40.000000 python_rucaptcha-6.2/src/python_rucaptcha/core/result_handler.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     1739 2023-12-14 13:52:15.000000 python_rucaptcha-6.2/src/python_rucaptcha/core/serializer.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     4028 2023-12-08 16:18:54.000000 python_rucaptcha-6.2/src/python_rucaptcha/cutcaptcha.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     3909 2023-12-10 20:45:24.000000 python_rucaptcha-6.2/src/python_rucaptcha/cyber_siara_captcha.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     4140 2023-12-10 15:44:52.000000 python_rucaptcha-6.2/src/python_rucaptcha/datadome_captcha.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)    11837 2023-12-13 17:14:39.000000 python_rucaptcha-6.2/src/python_rucaptcha/draw_around_captcha.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     4232 2024-01-03 17:59:23.000000 python_rucaptcha-6.2/src/python_rucaptcha/friendly_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3496 2023-12-08 01:06:23.000000 python_rucaptcha-6.2/src/python_rucaptcha/fun_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     8583 2023-12-13 23:09:36.000000 python_rucaptcha-6.2/src/python_rucaptcha/gee_test.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     9001 2023-12-13 17:40:40.000000 python_rucaptcha-6.2/src/python_rucaptcha/grid_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3732 2023-12-08 01:07:51.000000 python_rucaptcha-6.2/src/python_rucaptcha/hcaptcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     8391 2023-12-07 21:35:13.000000 python_rucaptcha-6.2/src/python_rucaptcha/image_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4017 2023-12-08 01:09:26.000000 python_rucaptcha-6.2/src/python_rucaptcha/key_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4064 2023-12-08 01:06:23.000000 python_rucaptcha-6.2/src/python_rucaptcha/lemin_captcha.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     3415 2023-12-11 01:15:38.000000 python_rucaptcha-6.2/src/python_rucaptcha/mt_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     6083 2023-12-08 01:11:14.000000 python_rucaptcha-6.2/src/python_rucaptcha/re_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     6225 2023-12-07 21:55:48.000000 python_rucaptcha-6.2/src/python_rucaptcha/rotate_captcha.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     3620 2024-04-29 15:30:36.000000 python_rucaptcha-6.2/src/python_rucaptcha/tencent.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3708 2023-12-06 16:37:43.000000 python_rucaptcha-6.2/src/python_rucaptcha/text_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3686 2023-12-08 01:06:23.000000 python_rucaptcha-6.2/src/python_rucaptcha/turnstile.py
+drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-04-29 16:58:03.229532 python_rucaptcha-6.2/src/python_rucaptcha.egg-info/
+-rw-r--r--   0 homea     (1000) homea     (1000)     8827 2024-04-29 16:58:03.000000 python_rucaptcha-6.2/src/python_rucaptcha.egg-info/PKG-INFO
+-rw-rw-r--   0 homea     (1000) homea     (1000)     2072 2024-04-29 16:58:03.000000 python_rucaptcha-6.2/src/python_rucaptcha.egg-info/SOURCES.txt
+-rw-rw-r--   0 homea     (1000) homea     (1000)        1 2024-04-29 16:58:03.000000 python_rucaptcha-6.2/src/python_rucaptcha.egg-info/dependency_links.txt
+-rw-rw-r--   0 homea     (1000) homea     (1000)       62 2024-04-29 16:58:03.000000 python_rucaptcha-6.2/src/python_rucaptcha.egg-info/requires.txt
+-rw-rw-r--   0 homea     (1000) homea     (1000)       17 2024-04-29 16:58:03.000000 python_rucaptcha-6.2/src/python_rucaptcha.egg-info/top_level.txt
+drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-04-29 16:58:03.228532 python_rucaptcha-6.2/tests/
+-rw-r--r--   0 homea     (1000) homea     (1000)     3245 2023-12-11 23:11:07.000000 python_rucaptcha-6.2/tests/test_amazon.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     8101 2023-12-07 22:03:12.000000 python_rucaptcha-6.2/tests/test_audio.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     7125 2023-12-13 17:28:08.000000 python_rucaptcha-6.2/tests/test_bounding_box.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4050 2023-12-11 23:11:07.000000 python_rucaptcha-6.2/tests/test_capypuzzle.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3543 2023-12-07 22:03:13.000000 python_rucaptcha-6.2/tests/test_control.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     7124 2023-12-13 17:38:00.000000 python_rucaptcha-6.2/tests/test_coordinates.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3715 2023-12-08 15:25:47.000000 python_rucaptcha-6.2/tests/test_core.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     5478 2023-12-13 17:23:28.000000 python_rucaptcha-6.2/tests/test_cutcaptcha.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     3567 2023-12-10 20:45:19.000000 python_rucaptcha-6.2/tests/test_cybersiara.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     5102 2023-12-11 01:16:30.000000 python_rucaptcha-6.2/tests/test_datadome.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     7105 2023-12-13 17:41:42.000000 python_rucaptcha-6.2/tests/test_draw_around.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     4772 2024-01-03 18:41:37.000000 python_rucaptcha-6.2/tests/test_friendly_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4633 2023-12-11 23:11:07.000000 python_rucaptcha-6.2/tests/test_funcaptcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     8153 2023-12-11 23:11:07.000000 python_rucaptcha-6.2/tests/test_geetest.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     7011 2023-12-13 17:38:55.000000 python_rucaptcha-6.2/tests/test_grid.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4346 2023-12-11 23:11:07.000000 python_rucaptcha-6.2/tests/test_hcaptcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     8362 2023-12-13 17:41:42.000000 python_rucaptcha-6.2/tests/test_image.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     7479 2023-12-13 18:20:42.000000 python_rucaptcha-6.2/tests/test_key_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4954 2023-12-11 23:11:07.000000 python_rucaptcha-6.2/tests/test_lemin.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     2379 2023-12-11 01:20:17.000000 python_rucaptcha-6.2/tests/test_mtcaptcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4467 2023-12-11 23:11:07.000000 python_rucaptcha-6.2/tests/test_recaptcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     8744 2023-12-07 22:02:03.000000 python_rucaptcha-6.2/tests/test_rotate.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     2661 2024-04-29 16:39:51.000000 python_rucaptcha-6.2/tests/test_tencent.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     2597 2023-12-11 23:11:12.000000 python_rucaptcha-6.2/tests/test_text.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4822 2023-12-11 23:11:07.000000 python_rucaptcha-6.2/tests/test_turnstile.py
```

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/amazon_waf.py` & `python_rucaptcha-6.2/src/python_rucaptcha/amazon_waf.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/audio_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/audio_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/bounding_box_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/bounding_box_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/capy_puzzle.py` & `python_rucaptcha-6.2/src/python_rucaptcha/capy_puzzle.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/control.py` & `python_rucaptcha-6.2/src/python_rucaptcha/control.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,17 @@
         Returns:
             Dict with full server response
 
         Notes:
             https://rucaptcha.com/api-docs/get-balance
             https://rucaptcha.com/api-docs/report-correct
             https://rucaptcha.com/api-docs/report-incorrect
+            https://2captcha.com/api-docs/get-balance
+            https://2captcha.com/api-docs/report-correct
+            https://2captcha.com/api-docs/report-incorrect
         """
 
         super().__init__(method=ControlEnm.control, *args, **kwargs)
 
     def reportCorrect(self, id: int) -> dict:
         """
         reportCorrect method
```

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/coordinates_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/coordinates_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/core/base.py` & `python_rucaptcha-6.2/src/python_rucaptcha/core/base.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/core/config.py` & `python_rucaptcha-6.2/src/python_rucaptcha/core/config.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/core/enums.py` & `python_rucaptcha-6.2/src/python_rucaptcha/core/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,7 +145,17 @@
 class GridCaptchaEnm(str, MyEnum):
     GridTask = "GridTask"
 
 
 class FriendlyCaptchaEnm(str, MyEnum):
     FriendlyCaptchaTaskProxyless = "FriendlyCaptchaTaskProxyless"
     FriendlyCaptchaTask = "FriendlyCaptchaTask"
+
+
+class TencentEnm(str, MyEnum):
+    TencentTask = "TencentTask"
+    TencentTaskProxyless = "TencentTaskProxyless"
+
+
+class atbCaptchaEnm(str, MyEnum):
+    AtbCaptchaTask = "AtbCaptchaTask"
+    AtbCaptchaTaskProxyless = "AtbCaptchaTaskProxyless"
```

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/core/result_handler.py` & `python_rucaptcha-6.2/src/python_rucaptcha/core/result_handler.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/core/serializer.py` & `python_rucaptcha-6.2/src/python_rucaptcha/core/serializer.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/cutcaptcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/cutcaptcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/cyber_siara_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/cyber_siara_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/datadome_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/datadome_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/draw_around_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/draw_around_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/friendly_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/friendly_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/fun_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/gee_test.py` & `python_rucaptcha-6.2/src/python_rucaptcha/gee_test.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/grid_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/grid_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/hcaptcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/image_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/image_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/key_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/key_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/lemin_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/lemin_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/mt_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/mt_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/re_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/re_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/rotate_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/rotate_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/text_captcha.py` & `python_rucaptcha-6.2/src/python_rucaptcha/text_captcha.py`

 * *Files identical despite different names*

### Comparing `python-rucaptcha-6.1.2/python_rucaptcha/turnstile.py` & `python_rucaptcha-6.2/src/python_rucaptcha/turnstile.py`

 * *Files identical despite different names*

