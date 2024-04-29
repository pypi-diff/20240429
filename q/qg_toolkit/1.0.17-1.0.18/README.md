# Comparing `tmp/qg_toolkit-1.0.17.tar.gz` & `tmp/qg_toolkit-1.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qg_toolkit-1.0.17.tar", max compression
+gzip compressed data, was "qg_toolkit-1.0.18.tar", max compression
```

## Comparing `qg_toolkit-1.0.17.tar` & `qg_toolkit-1.0.18.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      854 2024-04-29 11:10:10.373103 qg_toolkit-1.0.17/pyproject.toml
--rw-r--r--   0        0        0       94 2024-04-28 01:55:09.875818 qg_toolkit-1.0.17/qg_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 01:55:09.876818 qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/__init__.py
--rw-r--r--   0        0        0       94 2024-04-28 01:55:09.876818 qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_fullpage/__init__.py
--rw-r--r--   0        0        0     5190 2024-04-28 01:55:09.877828 qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py
--rw-r--r--   0        0        0     5433 2024-04-28 01:55:09.877828 qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js
--rw-r--r--   0        0        0     2288 2024-04-28 01:55:09.877828 qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py
--rw-r--r--   0        0        0       94 2024-04-28 01:55:09.878819 qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/__init__.py
--rw-r--r--   0        0        0     2723 2024-04-28 01:55:09.878819 qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/gap.py
--rw-r--r--   0        0        0    37946 2024-04-29 10:59:40.417027 qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py
--rw-r--r--   0        0        0    51280 2024-04-28 01:55:09.880829 qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png
--rw-r--r--   0        0        0     4818 2024-04-28 01:55:09.880829 qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png
--rw-r--r--   0        0        0     9121 2024-04-28 01:55:09.881818 qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png
--rw-r--r--   0        0        0  1793853 2024-04-28 01:55:09.890818 qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json
--rw-r--r--   0        0        0     2362 2024-04-28 01:55:09.890818 qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js
--rw-r--r--   0        0        0     2349 2024-04-28 01:55:09.891818 qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/mian.py
--rw-r--r--   0        0        0     1043 2024-04-28 01:55:09.891818 qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/trace.py
--rw-r--r--   0        0        0   101372 2024-04-29 10:29:45.977586 qg_toolkit-1.0.17/qg_toolkit/qgalxe/galxe.py
--rw-r--r--   0        0        0     2750 2024-04-29 09:53:39.862145 qg_toolkit-1.0.17/qg_toolkit/qgalxe/GeetestFullPageV4.py
--rw-r--r--   0        0        0     3782 2024-04-29 11:08:24.626823 qg_toolkit-1.0.17/qg_toolkit/qgalxe/GeetestSlideV4.py
--rw-r--r--   0        0        0       96 2024-04-28 01:55:09.892818 qg_toolkit-1.0.17/qg_toolkit/qtweepy/__init__.py
--rw-r--r--   0        0        0      103 2024-04-28 01:55:09.892818 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/__init__.py
--rw-r--r--   0        0        0     4912 2024-04-28 06:26:10.954966 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/account_checker.py
--rw-r--r--   0        0        0     2251 2024-04-28 01:55:09.893817 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/follow_each_other.py
--rw-r--r--   0        0        0        0 2024-04-28 06:38:00.187702 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/input-output/BAD_TOKEN.txt
--rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/input-output/CONSENT_LOCKED.txt
--rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/input-output/GOOD.txt
--rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/input-output/LOCKED.txt
--rw-r--r--   0        0        0       44 2024-04-28 06:37:01.438691 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/input-output/PROXIES.txt
--rw-r--r--   0        0        0        0 2024-04-28 06:38:00.187702 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/input-output/SUSPENDED.txt
--rw-r--r--   0        0        0       40 2024-04-28 06:38:00.187702 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/input-output/UNKNOWN.txt
--rw-r--r--   0        0        0     3622 2024-04-28 01:55:09.894817 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/mavia.py
--rw-r--r--   0        0        0     2373 2024-04-28 01:55:09.895818 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/set_2fa.py
--rw-r--r--   0        0        0     3081 2024-04-28 01:55:09.895818 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py
--rw-r--r--   0        0        0      697 2024-04-28 01:55:09.895818 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/uploading_images.py
--rw-r--r--   0        0        0     2253 2024-04-28 01:55:09.896820 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/voter.py
--rw-r--r--   0        0        0     3120 2024-04-28 01:55:09.896820 qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/xai.py
--rw-r--r--   0        0        0      687 2024-04-28 01:55:09.896820 qg_toolkit-1.0.17/qg_toolkit/qtweepy/pyproject.toml
--rw-r--r--   0        0        0     8720 2024-04-28 01:55:09.892818 qg_toolkit-1.0.17/qg_toolkit/qtweepy/README.md
--rw-r--r--   0        0        0      132 2024-04-28 01:55:09.897831 qg_toolkit-1.0.17/qg_toolkit/qtweepy/tea.yaml
--rw-r--r--   0        0        0      732 2024-04-28 01:55:09.897831 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 01:55:09.897831 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/_capsolver/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 01:55:09.897831 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/_capsolver/core/__init__.py
--rw-r--r--   0        0        0     8883 2024-04-28 01:55:09.898831 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py
--rw-r--r--   0        0        0     1054 2024-04-28 01:55:09.898831 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py
--rw-r--r--   0        0        0     1741 2024-04-28 01:55:09.899826 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py
--rw-r--r--   0        0        0     2602 2024-04-28 01:55:09.899826 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py
--rw-r--r--   0        0        0    10974 2024-04-28 01:55:09.900819 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py
--rw-r--r--   0        0        0     3248 2024-04-28 01:55:09.900819 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/account.py
--rw-r--r--   0        0        0      141 2024-04-28 01:55:09.900819 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/base/__init__.py
--rw-r--r--   0        0        0      500 2024-04-28 01:55:09.901826 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/base/client.py
--rw-r--r--   0        0        0     2175 2024-04-28 01:55:09.901826 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/base/session.py
--rw-r--r--   0        0        0    70738 2024-04-28 01:55:09.902820 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/client.py
--rw-r--r--   0        0        0      267 2024-04-28 01:55:09.902820 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/enums.py
--rw-r--r--   0        0        0     5322 2024-04-28 01:55:09.903823 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/errors.py
--rw-r--r--   0        0        0     4695 2024-04-28 01:55:09.903823 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/models.py
--rw-r--r--   0        0        0      665 2024-04-28 01:55:09.903823 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/utils/__init__.py
--rw-r--r--   0        0        0     1152 2024-04-28 01:55:09.904830 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/utils/file.py
--rw-r--r--   0        0        0     2140 2024-04-28 01:55:09.904830 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/utils/html.py
--rw-r--r--   0        0        0     1061 2024-04-28 01:55:09.904830 qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/utils/other.py
--rw-r--r--   0        0        0      279 2024-04-28 01:55:09.905829 qg_toolkit-1.0.17/qg_toolkit/test/demo.yaml
--rw-r--r--   0        0        0        0 2024-04-28 01:55:09.905829 qg_toolkit-1.0.17/qg_toolkit/test/test.py
--rw-r--r--   0        0        0       96 2024-04-28 01:55:09.905829 qg_toolkit-1.0.17/qg_toolkit/tools/__init__.py
--rw-r--r--   0        0        0     5264 2024-04-29 10:04:50.990411 qg_toolkit-1.0.17/qg_toolkit/tools/cui_qiu_client.py
--rw-r--r--   0        0        0     1245 2024-04-29 09:52:12.132611 qg_toolkit-1.0.17/qg_toolkit/tools/date_util.py
--rw-r--r--   0        0        0    12289 2024-04-29 09:59:28.288628 qg_toolkit-1.0.17/qg_toolkit/tools/discord.py
--rw-r--r--   0        0        0     5905 2024-04-29 06:52:45.801970 qg_toolkit-1.0.17/qg_toolkit/tools/qg_airdrop.py
--rw-r--r--   0        0        0      985 2024-04-28 01:55:09.906829 qg_toolkit-1.0.17/qg_toolkit/tools/qg_crypto.py
--rw-r--r--   0        0        0    36155 2024-04-29 07:53:05.424108 qg_toolkit-1.0.17/qg_toolkit/tools/qg_eth.py
--rw-r--r--   0        0        0     3594 2024-04-28 01:55:09.907829 qg_toolkit-1.0.17/qg_toolkit/tools/qg_file.py
--rw-r--r--   0        0        0      300 2024-04-28 01:55:09.908828 qg_toolkit-1.0.17/qg_toolkit/tools/qg_models.py
--rw-r--r--   0        0        0      741 2024-04-28 01:55:09.908828 qg_toolkit-1.0.17/qg_toolkit/tools/qg_random.py
--rw-r--r--   0        0        0     6168 2024-04-29 06:52:45.802969 qg_toolkit-1.0.17/qg_toolkit/tools/qg_solana.py
--rw-r--r--   0        0        0     2764 2024-04-28 01:55:09.908828 qg_toolkit-1.0.17/qg_toolkit/tools/qg_starknet.py
--rw-r--r--   0        0        0     3241 2024-04-28 01:55:09.909829 qg_toolkit-1.0.17/qg_toolkit/tools/qproxy.py
--rw-r--r--   0        0        0     1239 2024-04-29 10:01:18.869266 qg_toolkit-1.0.17/qg_toolkit/tools/random_tool.py
--rw-r--r--   0        0        0     6068 2024-04-28 01:55:09.909829 qg_toolkit-1.0.17/qg_toolkit/tools/rpc.py
--rw-r--r--   0        0        0    72044 2024-04-29 09:56:23.770716 qg_toolkit-1.0.17/qg_toolkit/tools/twitter.py
--rw-r--r--   0        0        0     4085 2024-02-09 00:42:50.310936 qg_toolkit-1.0.17/qg_toolkit/tools/yescaptcha.py
--rw-r--r--   0        0        0       38 2024-04-22 02:07:22.831782 qg_toolkit-1.0.17/README.md
--rw-r--r--   0        0        0      133 2024-04-29 11:10:10.376110 qg_toolkit-1.0.17/tea.yaml
--rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 qg_toolkit-1.0.17/PKG-INFO
+-rw-r--r--   0        0        0      854 2024-04-29 17:18:57.900555 qg_toolkit-1.0.18/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-27 10:53:56.731750 qg_toolkit-1.0.18/qg_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 18:53:34.039466 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-27 10:54:32.432326 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_fullpage/__init__.py
+-rw-r--r--   0        0        0     5190 2024-04-24 18:53:34.040467 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py
+-rw-r--r--   0        0        0     5433 2024-04-24 18:53:34.040467 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js
+-rw-r--r--   0        0        0     2288 2024-04-27 11:00:05.704720 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py
+-rw-r--r--   0        0        0       94 2024-04-27 10:54:37.081886 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/__init__.py
+-rw-r--r--   0        0        0     2723 2024-04-24 18:53:34.042468 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/gap.py
+-rw-r--r--   0        0        0    37946 2024-04-29 17:00:55.850149 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py
+-rw-r--r--   0        0        0    51280 2024-04-24 18:53:34.044476 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png
+-rw-r--r--   0        0        0     4818 2024-04-24 18:53:34.045475 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png
+-rw-r--r--   0        0        0     9121 2024-04-24 18:53:34.045475 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png
+-rw-r--r--   0        0        0  1793853 2024-04-24 18:53:34.058465 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json
+-rw-r--r--   0        0        0     2362 2024-04-24 18:53:34.059468 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js
+-rw-r--r--   0        0        0     2349 2024-04-27 11:14:05.254088 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/mian.py
+-rw-r--r--   0        0        0     1043 2024-04-24 18:53:34.060469 qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/trace.py
+-rw-r--r--   0        0        0   101372 2024-04-29 17:00:55.853150 qg_toolkit-1.0.18/qg_toolkit/qgalxe/galxe.py
+-rw-r--r--   0        0        0     2750 2024-04-29 17:00:55.851150 qg_toolkit-1.0.18/qg_toolkit/qgalxe/GeetestFullPageV4.py
+-rw-r--r--   0        0        0     3795 2024-04-29 17:00:55.851150 qg_toolkit-1.0.18/qg_toolkit/qgalxe/GeetestSlideV4.py
+-rw-r--r--   0        0        0       96 2024-04-27 10:54:21.799092 qg_toolkit-1.0.18/qg_toolkit/qtweepy/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-27 10:52:23.199431 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/__init__.py
+-rw-r--r--   0        0        0     4912 2024-04-29 17:00:55.853150 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/account_checker.py
+-rw-r--r--   0        0        0     2251 2024-04-27 10:52:23.208431 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/follow_each_other.py
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.415935 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/input-output/BAD_TOKEN.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/input-output/CONSENT_LOCKED.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/input-output/GOOD.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/input-output/LOCKED.txt
+-rw-r--r--   0        0        0       44 2024-04-29 17:00:55.854150 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/input-output/PROXIES.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/input-output/SUSPENDED.txt
+-rw-r--r--   0        0        0       40 2024-04-27 05:31:12.415935 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/input-output/UNKNOWN.txt
+-rw-r--r--   0        0        0     3622 2024-04-27 10:52:23.284728 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/mavia.py
+-rw-r--r--   0        0        0     2373 2024-04-27 10:52:23.217431 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/set_2fa.py
+-rw-r--r--   0        0        0     3081 2024-04-27 10:52:23.184432 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py
+-rw-r--r--   0        0        0      697 2024-04-27 10:52:23.174431 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/uploading_images.py
+-rw-r--r--   0        0        0     2253 2024-04-27 10:52:23.159432 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/voter.py
+-rw-r--r--   0        0        0     3120 2024-04-27 10:52:23.191432 qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/xai.py
+-rw-r--r--   0        0        0      687 2024-04-20 19:57:03.446998 qg_toolkit-1.0.18/qg_toolkit/qtweepy/pyproject.toml
+-rw-r--r--   0        0        0     8720 2024-04-20 19:48:15.063903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/README.md
+-rw-r--r--   0        0        0      132 2024-04-24 18:22:26.184000 qg_toolkit-1.0.18/qg_toolkit/qtweepy/tea.yaml
+-rw-r--r--   0        0        0      732 2024-04-20 19:48:15.068902 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/__init__.py
+-rw-r--r--   0        0        0     8883 2024-04-20 19:48:15.070903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py
+-rw-r--r--   0        0        0     1054 2024-04-20 19:48:15.070903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py
+-rw-r--r--   0        0        0     1741 2024-04-20 19:48:15.071903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py
+-rw-r--r--   0        0        0     2602 2024-04-20 19:48:15.071903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py
+-rw-r--r--   0        0        0    10974 2024-04-20 19:48:15.072903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py
+-rw-r--r--   0        0        0     3248 2024-04-20 19:48:15.072903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/account.py
+-rw-r--r--   0        0        0      141 2024-04-20 19:48:15.072903 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/base/__init__.py
+-rw-r--r--   0        0        0      500 2024-04-20 19:48:15.074292 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/base/client.py
+-rw-r--r--   0        0        0     2175 2024-04-27 10:52:23.255728 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/base/session.py
+-rw-r--r--   0        0        0    70738 2024-04-20 19:48:15.075686 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/client.py
+-rw-r--r--   0        0        0      267 2024-04-20 19:48:15.076283 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/enums.py
+-rw-r--r--   0        0        0     5322 2024-04-20 19:48:15.076811 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/errors.py
+-rw-r--r--   0        0        0     4695 2024-04-20 19:48:15.076811 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/models.py
+-rw-r--r--   0        0        0      665 2024-04-20 19:48:15.077920 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/__init__.py
+-rw-r--r--   0        0        0     1152 2024-04-20 19:48:15.077920 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/file.py
+-rw-r--r--   0        0        0     2140 2024-04-20 19:48:15.078463 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/html.py
+-rw-r--r--   0        0        0     1061 2024-04-20 19:48:15.078992 qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/other.py
+-rw-r--r--   0        0        0      279 2024-04-29 17:00:55.855149 qg_toolkit-1.0.18/qg_toolkit/test/demo.yaml
+-rw-r--r--   0        0        0        0 2024-04-27 11:06:09.049630 qg_toolkit-1.0.18/qg_toolkit/test/test.py
+-rw-r--r--   0        0        0       96 2024-04-27 10:54:04.685704 qg_toolkit-1.0.18/qg_toolkit/tools/__init__.py
+-rw-r--r--   0        0        0     5391 2024-04-29 17:18:03.385731 qg_toolkit-1.0.18/qg_toolkit/tools/cui_qiu_client.py
+-rw-r--r--   0        0        0     1245 2024-04-29 17:00:55.856150 qg_toolkit-1.0.18/qg_toolkit/tools/date_util.py
+-rw-r--r--   0        0        0    12289 2024-04-29 17:00:55.857149 qg_toolkit-1.0.18/qg_toolkit/tools/discord.py
+-rw-r--r--   0        0        0     5905 2024-04-29 05:37:22.967370 qg_toolkit-1.0.18/qg_toolkit/tools/qg_airdrop.py
+-rw-r--r--   0        0        0      985 2024-04-20 20:27:34.147592 qg_toolkit-1.0.18/qg_toolkit/tools/qg_crypto.py
+-rw-r--r--   0        0        0    36155 2024-04-29 17:00:55.858150 qg_toolkit-1.0.18/qg_toolkit/tools/qg_eth.py
+-rw-r--r--   0        0        0     3641 2024-04-29 17:18:33.161050 qg_toolkit-1.0.18/qg_toolkit/tools/qg_file.py
+-rw-r--r--   0        0        0      300 2024-04-24 18:53:34.062471 qg_toolkit-1.0.18/qg_toolkit/tools/qg_models.py
+-rw-r--r--   0        0        0      741 2024-04-20 20:24:22.248041 qg_toolkit-1.0.18/qg_toolkit/tools/qg_random.py
+-rw-r--r--   0        0        0     6168 2024-04-29 05:55:33.712699 qg_toolkit-1.0.18/qg_toolkit/tools/qg_solana.py
+-rw-r--r--   0        0        0     2764 2024-04-24 18:21:31.477405 qg_toolkit-1.0.18/qg_toolkit/tools/qg_starknet.py
+-rw-r--r--   0        0        0     3241 2024-04-20 19:48:15.080086 qg_toolkit-1.0.18/qg_toolkit/tools/qproxy.py
+-rw-r--r--   0        0        0     1239 2024-04-29 17:00:55.858150 qg_toolkit-1.0.18/qg_toolkit/tools/random_tool.py
+-rw-r--r--   0        0        0     6068 2024-04-27 13:05:30.422039 qg_toolkit-1.0.18/qg_toolkit/tools/rpc.py
+-rw-r--r--   0        0        0    72567 2024-04-29 17:16:01.332559 qg_toolkit-1.0.18/qg_toolkit/tools/twitter.py
+-rw-r--r--   0        0        0     4182 2024-04-29 17:16:29.644862 qg_toolkit-1.0.18/qg_toolkit/tools/yescaptcha.py
+-rw-r--r--   0        0        0       38 2024-04-20 19:50:56.436133 qg_toolkit-1.0.18/README.md
+-rw-r--r--   0        0        0      133 2024-04-29 17:18:57.893558 qg_toolkit-1.0.18/tea.yaml
+-rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 qg_toolkit-1.0.18/PKG-INFO
```

### Comparing `qg_toolkit-1.0.17/pyproject.toml` & `qg_toolkit-1.0.18/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qg_toolkit"
-version = "1.0.17"
+version = "1.0.18"
 description = "qg_toolkit for Python!"
 authors = ["qg <qg@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qg_toolkit"}]
 include = [{path = "tea.yaml"}]
```

### Comparing `qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py` & `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js` & `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py` & `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/gap.py` & `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/gap.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py` & `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png` & `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png` & `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png` & `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json` & `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js` & `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/mian.py` & `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/mian.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/geetest_captcha/geetest4_slide/trace.py` & `qg_toolkit-1.0.18/qg_toolkit/geetest_captcha/geetest4_slide/trace.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qgalxe/galxe.py` & `qg_toolkit-1.0.18/qg_toolkit/qgalxe/galxe.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qgalxe/GeetestFullPageV4.py` & `qg_toolkit-1.0.18/qg_toolkit/qgalxe/GeetestFullPageV4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qgalxe/GeetestSlideV4.py` & `qg_toolkit-1.0.18/qg_toolkit/qgalxe/GeetestSlideV4.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,14 @@
             return None
 
     def solve_captcha(self, url=None) -> Union[str, None]:
         if url is None:
             return None
         return self.get_captcha(url)
 
-
-if __name__ == '__main__':
-    gt = GeetestSlideV4()
-    for _ in range(10):
-        gt.solve_captcha(
-            url = 'https://gcaptcha4.geetest.com/verify?callback=geetest_1714388895377&captcha_id=a7ea5725ff59be6a27d8db0d05a1bf09&client_type=web&lot_number=935469a676134c8a89998513a6692c89&payload=_b-sD20eax9oEJvmoMxvFPDC8WTZafY4krFYMddesP3be1zPV3xye8FjcTq0_uP_rmIBBbVvrcjuotejPtAN1bDUKUR8uzpQw3ZRo4BYjxjlNS2Qy0TgXDfw2cmhZVtjl_euFv2XpFsThDN7hYo1mttSrox9uWhxWO6sc5g3s7c1XX-KgZocOJhYYBsxbgTo7Uc8FKlakNIs-VHF3bPXo7yvIAP02ipj5jUkVXNcVl-SzMY2O1dF8cE5QKH_oQlHue7thDQgmKUsGeeaH-_N7E7jzrYvWAwvLvNO2eo9KGu1bx7nsMWnzhzUw0nNBBDn4jZ2NqH7zELDxMCH2emvmWD978R8yuf3pY77Po2mhshpUkDVVe_3rLanDYCT8LpvAjzAYeMEmE8gimMcEgnIIug93zS1dAL6AnoOnFPpRWdcdly9BT1k2BXBSDsm_Dc4clPw5iNSlwvakxlYfDFNAL-Uudvf-aTnfG06uzmvqA23iY0k0i-RPZ3rGyn0wlBgtVq_vKuO5Kd4kn4MajhFRYTyIwAEZt7b4MY-aCGM6VovuIFtql2BtmKr9maoic0lUMh2ueiEEkQDv7yuxDyGm7G6FE_cBeoLFB1irBaKYmUczrP1qPTcPfRJnmTw_GTIiMnnyeJj4kzEUkQ-hEvoMsRq9V0leg6szU8PZfXTByndIVbLzjQ9Youa3CVIDSwAB75DZGvhPj4P3DbAZYhceyDIn5oB3x2AFaRwAVP9CuNr19ljOXiMDDyMYtbeVZtmyg0gPDoMPz81GL-LHc31oVjtzuXWcMy8sEkPmQFOrdAovrYtbvbuRaBPzBva-BGUUNhRU6pJ_RdWtfUQvWCBJRTPsQ52KfEMipmcACOvVeo%3D&process_token=4b88013bdf66814aa8bb33f197a7699e99299720a0a705c320acc6cc3f93d43d&payload_protocol=1&pt=1&w=77714321393fd537dbb657a2e944e5c73874fe11abd6602f631765b395dfc156feda7a3e803c1be9b97f8b208790fc23440ced449aad6b757195a8166e9ee01893017ab26370dd70e6a9a0d203811e52baf8757b67da9739061d79cd231f2de6a9d2306cd8fc7f5ec4367f36d5c85169cb93383394775211a9cbf28db2f8bac126884c2d70fbce1f187a13b9feea4a9dfa11e9654a3c50711313741cd4ff5daa8784c56e8b7ee800aeb0ec5239e0291892d31fea403ed7b51327d0d46cefcaa795dcfe803103b3c3af7dbe5315b44b8a47d38fd3ef949f31028b5801b41d550de97cf95ab6ea0c65fa7221d265870bb844873ff4948e2d2a8e84cd53946942e4036307fde947515029ba671db386e55221509efb296c35ba8dccf39de723cfc87c1ae9bdba3eccc08d5f2847b76fd052e44d1508c3cc307e90b049eaac7d5dee0fb1a35f364e7397d9b51d2d1bdb7beffd6acf7b6ff819f01762542ae3f37599b4ac9d9f06ef9bb376eeb36c90e27fca53b931b2ff50936e5f6b9b1290b1a65fe23065ef4011052c932db9df1859b1b606da565232021bd5aee4a863c2456618aea0b47050e299d764a886ec615b41fc6b5907c2220258e014ba836e38feb4f7ab78970aa5bf8e402a0d55d806ba2506cf346c4059d3e008c9fbcffa7c01bee7fb4c4aace94b92bc37edb60fb3a5433e1d967bf4a0bf92073da684a51341106f706b390a9eea51ae3c2c87390672434cfa14a5778c7e4242822fdeeb9ba501704a4ad9ced7a304921f858c2067d084fd2a5387f09dae2394bd6061c5aa2a468a')
-        time.sleep(2)
+#
+# if __name__ == '__main__':
+#     gt = GeetestSlideV4()
+#     for _ in range(10):
+#         gt.solve_captcha(
+#             url = 'https://gcaptcha4.geetest.com/verify?callback=geetest_1714388895377&captcha_id=a7ea5725ff59be6a27d8db0d05a1bf09&client_type=web&lot_number=935469a676134c8a89998513a6692c89&payload=_b-sD20eax9oEJvmoMxvFPDC8WTZafY4krFYMddesP3be1zPV3xye8FjcTq0_uP_rmIBBbVvrcjuotejPtAN1bDUKUR8uzpQw3ZRo4BYjxjlNS2Qy0TgXDfw2cmhZVtjl_euFv2XpFsThDN7hYo1mttSrox9uWhxWO6sc5g3s7c1XX-KgZocOJhYYBsxbgTo7Uc8FKlakNIs-VHF3bPXo7yvIAP02ipj5jUkVXNcVl-SzMY2O1dF8cE5QKH_oQlHue7thDQgmKUsGeeaH-_N7E7jzrYvWAwvLvNO2eo9KGu1bx7nsMWnzhzUw0nNBBDn4jZ2NqH7zELDxMCH2emvmWD978R8yuf3pY77Po2mhshpUkDVVe_3rLanDYCT8LpvAjzAYeMEmE8gimMcEgnIIug93zS1dAL6AnoOnFPpRWdcdly9BT1k2BXBSDsm_Dc4clPw5iNSlwvakxlYfDFNAL-Uudvf-aTnfG06uzmvqA23iY0k0i-RPZ3rGyn0wlBgtVq_vKuO5Kd4kn4MajhFRYTyIwAEZt7b4MY-aCGM6VovuIFtql2BtmKr9maoic0lUMh2ueiEEkQDv7yuxDyGm7G6FE_cBeoLFB1irBaKYmUczrP1qPTcPfRJnmTw_GTIiMnnyeJj4kzEUkQ-hEvoMsRq9V0leg6szU8PZfXTByndIVbLzjQ9Youa3CVIDSwAB75DZGvhPj4P3DbAZYhceyDIn5oB3x2AFaRwAVP9CuNr19ljOXiMDDyMYtbeVZtmyg0gPDoMPz81GL-LHc31oVjtzuXWcMy8sEkPmQFOrdAovrYtbvbuRaBPzBva-BGUUNhRU6pJ_RdWtfUQvWCBJRTPsQ52KfEMipmcACOvVeo%3D&process_token=4b88013bdf66814aa8bb33f197a7699e99299720a0a705c320acc6cc3f93d43d&payload_protocol=1&pt=1&w=77714321393fd537dbb657a2e944e5c73874fe11abd6602f631765b395dfc156feda7a3e803c1be9b97f8b208790fc23440ced449aad6b757195a8166e9ee01893017ab26370dd70e6a9a0d203811e52baf8757b67da9739061d79cd231f2de6a9d2306cd8fc7f5ec4367f36d5c85169cb93383394775211a9cbf28db2f8bac126884c2d70fbce1f187a13b9feea4a9dfa11e9654a3c50711313741cd4ff5daa8784c56e8b7ee800aeb0ec5239e0291892d31fea403ed7b51327d0d46cefcaa795dcfe803103b3c3af7dbe5315b44b8a47d38fd3ef949f31028b5801b41d550de97cf95ab6ea0c65fa7221d265870bb844873ff4948e2d2a8e84cd53946942e4036307fde947515029ba671db386e55221509efb296c35ba8dccf39de723cfc87c1ae9bdba3eccc08d5f2847b76fd052e44d1508c3cc307e90b049eaac7d5dee0fb1a35f364e7397d9b51d2d1bdb7beffd6acf7b6ff819f01762542ae3f37599b4ac9d9f06ef9bb376eeb36c90e27fca53b931b2ff50936e5f6b9b1290b1a65fe23065ef4011052c932db9df1859b1b606da565232021bd5aee4a863c2456618aea0b47050e299d764a886ec615b41fc6b5907c2220258e014ba836e38feb4f7ab78970aa5bf8e402a0d55d806ba2506cf346c4059d3e008c9fbcffa7c01bee7fb4c4aace94b92bc37edb60fb3a5433e1d967bf4a0bf92073da684a51341106f706b390a9eea51ae3c2c87390672434cfa14a5778c7e4242822fdeeb9ba501704a4ad9ced7a304921f858c2067d084fd2a5387f09dae2394bd6061c5aa2a468a')
+#         time.sleep(2)
```

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/account_checker.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/account_checker.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/follow_each_other.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/follow_each_other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/mavia.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/mavia.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/set_2fa.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/set_2fa.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/uploading_images.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/uploading_images.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/voter.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/voter.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/examples/xai.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/examples/xai.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/pyproject.toml` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/README.md` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/README.md`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/__init__.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/account.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/account.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/base/session.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/base/session.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/client.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/client.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/errors.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/errors.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/models.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/models.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/utils/__init__.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/utils/file.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/utils/html.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/html.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/qtweepy/twitter/utils/other.py` & `qg_toolkit-1.0.18/qg_toolkit/qtweepy/twitter/utils/other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/tools/cui_qiu_client.py` & `qg_toolkit-1.0.18/qg_toolkit/tools/cui_qiu_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 
 import requests
+from loguru import logger
 
 from qg_toolkit.tools.date_util import DateTool
 
 
 class CuiQiuClient:
     """脆球客户端"""
 
@@ -36,15 +37,15 @@
             'token': self.token,
             'domain_id': self.domain_id,
             'page': '1',
             'limit': '20',
             'mail': mail
         }
         response = requests.request("POST", url, data=payload)
-        print(response.text)
+        logger.info(response.text)
         return response.json()['data']
 
     def aliases_mail(self, mail=""):
         """根据邮箱名获取邮箱id"""
         url = "https://domain-api.cuiqiu.com/v1/aliases/mail"
         data = {
             'page': '1',
@@ -54,15 +55,15 @@
             'domainId': self.domain_id,
             'sort_value': 'id',
             'sort_type': 'desc',
             'domain_id': self.domain_id,
             'token': self.token,
         }
         response = requests.post(url, data=data)
-        print(response.text)
+        logger.info(response.text)
 
     def box_list(self, to_mail="", title=None):
         """获取邮件列表"""
         url = "https://domain-open-api.cuiqiu.com/v1/box/list"
         try:
             payload = {
                 'token': self.token,
@@ -75,15 +76,15 @@
                 'page': '1',
                 'limit': '20'
             }
             headers = {}
             response = requests.request("POST", url, headers=headers, data=payload)
             return response.json()["data"]["list"]
         except Exception as e:
-            print(e)
+            logger.info(e)
             return None
 
     def box_detail(self, box_id):
         """获取邮件详情"""
         url = "https://domain-open-api.cuiqiu.com/v1/box/detail"
         payload = {
             'token': self.token,
@@ -100,44 +101,44 @@
         payload = {
             'token': self.token,
             'page': '1',
             'limit': '10'
         }
         headers = {}
         response = requests.request("POST", url, headers=headers, data=payload)
-        print(response.text)
+        logger.info(response.text)
 
     def search_cq_email(self, my_mail, title, cs=20):
         """job 管理"""
         for x in range(cs):
-            print(f"开始第{x + 1}次尝试查找邮箱")
+            logger.info(f"【{my_mail}】：开始第{x + 1}次尝试查找邮箱")
             box_list = self.box_list(my_mail, title)
-            print(str(box_list))
             if box_list:
+                logger.info(str(box_list))
                 box_list = list(filter(lambda x: title in x['subject'], box_list))
-                print(f"{my_mail}找到收件啦啦！")
+                logger.info(f"【{my_mail}】找到收件啦啦！")
                 box_info = self.box_detail(box_list[0]["id"])
                 return box_info["content"]["body"]
                 # soup = BeautifulSoup(box_info["content"]["body"], features="lxml")
                 # code = soup.find('h1').text
-                # print(f"【{my_mail}】验证地址：{code}")
+                # logger.info(f"【{my_mail}】验证地址：{code}")
             time.sleep(5)
         return None
 
     def search_cq_email_v2(self, my_mail, title, cs=20):
         """job 管理"""
         if "gmailiil.com" not in my_mail:
             return None
         for x in range(cs):
             time.sleep(5)
-            print(f"开始第{x + 1}次尝试查找邮箱")
+            logger.info(f"开始第{x + 1}次尝试查找邮箱")
             box_list = self.box_list(my_mail)
-            print(str(box_list))
+            logger.info(str(box_list))
             if box_list:
                 box_list = list(filter(lambda x: title in x['subject'], box_list))
-                print(f"{my_mail}找到收件啦啦！")
+                logger.info(f"{my_mail}找到收件啦啦！")
                 box_info = self.box_detail(box_list[0]["id"])
                 return box_info["content"]["body"]
                 # soup = BeautifulSoup(box_info["content"]["body"], features="lxml")
                 # code = soup.find('h1').text
-                # print(f"【{my_mail}】验证地址：{code}")
+                # logger.info(f"【{my_mail}】验证地址：{code}")
         return None
```

### Comparing `qg_toolkit-1.0.17/qg_toolkit/tools/date_util.py` & `qg_toolkit-1.0.18/qg_toolkit/tools/date_util.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/tools/discord.py` & `qg_toolkit-1.0.18/qg_toolkit/tools/discord.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/tools/qg_airdrop.py` & `qg_toolkit-1.0.18/qg_toolkit/tools/qg_airdrop.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/tools/qg_crypto.py` & `qg_toolkit-1.0.18/qg_toolkit/tools/qg_crypto.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/tools/qg_eth.py` & `qg_toolkit-1.0.18/qg_toolkit/tools/qg_eth.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/tools/qg_file.py` & `qg_toolkit-1.0.18/qg_toolkit/tools/qg_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from urllib.parse import urlparse, parse_qs
 import yaml
 import csv
 
+from loguru import logger
+
 
 class QGFile:
     @staticmethod
     def save_to_file(file_path, log):
         with open(file_path, 'a', encoding='utf-8') as f:
             f.write(f'{log}\n')
             f.close()
@@ -61,15 +63,15 @@
                 data_list = all_list[1:]
                 array_obj = []
                 for data in data_list:
                     obj = {}
                     for i, attr in enumerate(head_list, start=0):
                         obj[attr] = data[i]
                     array_obj.append(obj)
-                # print(array_obj)
+                # logger.info(array_obj)
                 return array_obj
             else:
                 return all_list
 
     @staticmethod
     def to_yaml(wallet_path, dis_path, tw_path, to_path):
         """往文件修改新增"""
@@ -88,15 +90,15 @@
 
             else:
                 obj = {
                 }
                 full_data['accounts'].append(obj)
         with open(to_path, 'w') as file:
             yaml.dump(full_data, file)
-        print("数据已成功修改并写回到YAML文件。")
+        logger.info("数据已成功修改并写回到YAML文件。")
 
     @staticmethod
     def save_to_yaml(to_path, full_data):
         with open(to_path, 'w') as file:
             yaml.dump(full_data, file)
-        print("数据已成功修改并写回到YAML文件。")
+        logger.info("数据已成功修改并写回到YAML文件。")
```

### Comparing `qg_toolkit-1.0.17/qg_toolkit/tools/qg_random.py` & `qg_toolkit-1.0.18/qg_toolkit/tools/qg_random.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/tools/qg_solana.py` & `qg_toolkit-1.0.18/qg_toolkit/tools/qg_solana.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/tools/qg_starknet.py` & `qg_toolkit-1.0.18/qg_toolkit/tools/qg_starknet.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/tools/qproxy.py` & `qg_toolkit-1.0.18/qg_toolkit/tools/qproxy.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/tools/random_tool.py` & `qg_toolkit-1.0.18/qg_toolkit/tools/random_tool.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/tools/rpc.py` & `qg_toolkit-1.0.18/qg_toolkit/tools/rpc.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.17/qg_toolkit/tools/twitter.py` & `qg_toolkit-1.0.18/qg_toolkit/tools/twitter.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import copy
 import re
 
 import requests
 from bs4 import BeautifulSoup
 
 from qg_toolkit.tools.qg_file import QGFile
-
+from loguru import logger
 
 class QTwitter:
     headers1 = {
         'authority': 'twitter.com',
         'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
         'accept-language': 'zh-CN,zh;q=0.9',
         'cache-control': 'no-cache',
@@ -78,15 +78,15 @@
         if not flow_token:
             return
 
         params = {
             'c_name': 'ui_metrics',
         }
         response = self.session.get('https://twitter.com/i/js_inst', params=params)
-        # print(response.text)
+        # logger.info(response.text)
         #  输入账户
         response = self.login_flow_input_username_or_email(flow_token, self.email)
         flow_token = response.json()["flow_token"]
         if "你的账号存在异常登录活动。" in response.text:
             response = self.login_flow_check_username(flow_token)
             flow_token = response.json()["flow_token"]
         response = self.login_flow_input_password(flow_token)
@@ -116,30 +116,30 @@
             flow_token = response.json()["flow_token"]
             self.login_flow_phone_check(flow_token)
             # flow_token = response.json()["flow_token"]
         if "使用代码生成器应用生成" in response.text:
             flow_token = response.json()["flow_token"]
             self.input_google_code(flow_token)
         if "我们已发送了一个确认码至" in response.text:
-            print(f"【{self.username}】【{self.index}】此号完犊子完犊子咯~~~~~~~~~：{response.text}")
+            logger.info(f"【{self.username}】【{self.index}】此号完犊子完犊子咯~~~~~~~~~：{response.text}")
             return False
         self.refresh_by_session()
         # self.login_flow_get_ct0()
         # self.refresh_session()
         return True
 
     def start_login_flow(self):
         response = self.session.get('https://twitter.com/i/flow/login', headers=self.headers1)
         # 获取gt 大作用！！
         match = re.search(r'gt=(\d+);', response.text)
         gt = match.group(1) if match and match.group(1) else None
         if gt:
-            print(f"【{self.username}】【{self.index}】1.获取gt:{gt}")
+            logger.info(f"【{self.username}】【{self.index}】1.获取gt:{gt}")
         else:
-            print(f"【{self.username}】【{self.index}】1.未找到gt变量")
+            logger.info(f"【{self.username}】【{self.index}】1.未找到gt变量")
             return None
         # 2
         headers = copy.deepcopy(self.headers2)
         headers.update({
             'x-guest-token': f'{gt}'
         })
         self.session.headers.update(headers)
@@ -196,15 +196,15 @@
                 'user_recommendations_list': 4,
                 'user_recommendations_urt': 1,
                 'wait_spinner': 3,
                 'web_modal': 1,
             },
         }
         response = self.session.post('https://api.twitter.com/1.1/onboarding/task.json', params=params, json=json_data)
-        print(f"【{self.username}】【{self.index}】2.初始化登录流程：{response.text}")
+        logger.info(f"【{self.username}】【{self.index}】2.初始化登录流程：{response.text}")
         flow_token = response.json()["flow_token"]
         # 3.验证js
         json_data = {
             'flow_token': f'{flow_token}',
             'subtask_inputs': [
                 {
                     'subtask_id': 'LoginJsInstrumentationSubtask',
@@ -212,15 +212,15 @@
                         'response': '{"rf":{"a93fc5dc9ac246e9693c684ed79f29af46b3c64b81cd8ddd06372ee7a1751e1f":-140,"a9249513374b27e807794b9a44f32ad40494fbb4a36a32552970cdb67b892842":227,"ad9257164e44687140e434566d67e9fbe37f48aef43044e47c6ec4aec71a1022":15,"e420bb0dcbb032939891d227470ddcf0a437c99175b5e2b348d4e65a92420261":-1},"s":"ELKPLcGDfEOjJGHw63rXBEBNQuqBffo5w3a2D6hMpBa59t_pLlnShErv0VqgWkpYQZQlw0kdeLRw4sTrABFS0wM_t1ku94n7EzsX2mxIRkYqpVpjXH4anI3YHr9E-cxghN10I1Cz8xM1NsduN5Fb6Gfvs4frvU_6BRjdwyMnvotWRXlByqrL0L7Pf8MTxdO3ZmZZSnbpnyG4z_XMBfLziRzUCUG2WsY88jqDTV2_Ery6H6ybchxEj9vRKc5RgjJ9Ayl8mKJvxdHYo6Ses8w4GBRMVNmCHXHAayxEyQ9XKo8gOOqyHQswKVhfSYGpX6Kf-HH4j4JmnYVBrl9Z1U-TSgAAAYl-msQU"}',
                         'link': 'next_link',
                     },
                 },
             ],
         }
         response = self.session.post('https://api.twitter.com/1.1/onboarding/task.json', json=json_data)
-        print(f"【{self.username}】【{self.index}】3.验证js：{response.text}")
+        logger.info(f"【{self.username}】【{self.index}】3.验证js：{response.text}")
         flow_token = response.json()["flow_token"]
         return flow_token
 
     def login_flow_input_username_or_email(self, flow_token, username_or_email):
         # 3 输入账户 username
         json_data = {
             'flow_token': f'{flow_token}',
@@ -240,15 +240,15 @@
                         ],
                         'link': 'next_link',
                     },
                 },
             ],
         }
         response = self.session.post('https://api.twitter.com/1.1/onboarding/task.json', json=json_data)
-        print(f"【{self.username}】【{self.index}】登录流程->输入账号或者邮箱：{response.text}")
+        logger.info(f"【{self.username}】【{self.index}】登录流程->输入账号或者邮箱：{response.text}")
         return response
 
     def login_flow_check_username(self, flow_token):
         json_data = {
             'flow_token': f'{flow_token}',
             'subtask_inputs': [
                 {
@@ -257,15 +257,15 @@
                         'text': f'{self.username}',
                         'link': 'next_link',
                     },
                 },
             ],
         }
         response = self.session.post('https://api.twitter.com/1.1/onboarding/task.json', json=json_data)
-        print(f"【{self.username}】【{self.index}】登录流程->验证账号名：{response.text}")
+        logger.info(f"【{self.username}】【{self.index}】登录流程->验证账号名：{response.text}")
         return response
 
     def login_flow_input_password(self, flow_token):
         json_data = {
             'flow_token': f'{flow_token}',
             'subtask_inputs': [
                 {
@@ -274,15 +274,15 @@
                         'password': f'{self.password}',
                         'link': 'next_link',
                     },
                 },
             ],
         }
         response = self.session.post('https://api.twitter.com/1.1/onboarding/task.json', json=json_data)
-        print(f"【{self.username}】【{self.index}】6.输入密码：{response.text}")
+        logger.info(f"【{self.username}】【{self.index}】6.输入密码：{response.text}")
         return response
 
     def login_flow_duplication_check(self, flow_token):
         json_data = {
             'flow_token': f'{flow_token}',
             'subtask_inputs': [
                 {
@@ -290,15 +290,15 @@
                     'check_logged_in_account': {
                         'link': 'AccountDuplicationCheck_false',
                     },
                 },
             ],
         }
         response = self.session.post('https://api.twitter.com/1.1/onboarding/task.json', json=json_data)
-        print(f"【{self.username}】【{self.index}】7.校验登录：{response.text}")
+        logger.info(f"【{self.username}】【{self.index}】7.校验登录：{response.text}")
         return response
 
     def login_flow_phone_check(self, flow_token):
         json_data = {
             'flow_token': f'{flow_token}',
             'subtask_inputs': [
                 {
@@ -307,15 +307,15 @@
                         'text': f'{self.phone}',
                         'link': 'next_link',
                     },
                 },
             ],
         }
         response = self.session.post('https://api.twitter.com/1.1/onboarding/task.json', json=json_data)
-        print(f"【{self.username}】【{self.index}】8.输入手机号验证：{response.text}")
+        logger.info(f"【{self.username}】【{self.index}】8.输入手机号验证：{response.text}")
 
     def login_flow_email_check(self, flow_token):
         json_data = {
             'flow_token': f'{flow_token}',
             'subtask_inputs': [
                 {
                     'subtask_id': 'LoginAcid',
@@ -323,30 +323,30 @@
                         'text': f'{self.phone}',
                         'link': 'next_link',
                     },
                 },
             ],
         }
         response = self.session.post('https://api.twitter.com/1.1/onboarding/task.json', json=json_data)
-        print(f"【{self.username}】【{self.index}】8.输入手机号验证：{response.text}")
+        logger.info(f"【{self.username}】【{self.index}】8.输入手机号验证：{response.text}")
 
     def google_author(self):
         import pyotp
         import time
         # 替换为您的谷歌身份验证器密钥
         secret_key = f"{self.phone}"
         # 创建一个TOTP对象
         totp = pyotp.TOTP(secret_key)
         # 获取当前时间戳
         current_time = int(time.time())
         # 获取谷歌验证码
         otp = totp.at(current_time)
         # 获取谷歌验证码的有效期剩余秒数
         remaining_seconds = totp.interval - (current_time % totp.interval)
-        print(f"谷歌验证码:{otp}", f"有效期剩余秒数:{remaining_seconds}")
+        logger.info(f"谷歌验证码:{otp}", f"有效期剩余秒数:{remaining_seconds}")
         return otp
 
     def input_google_code(self, flow_token):
         json_data = {
             'flow_token': f'{flow_token}',
             'subtask_inputs': [
                 {
@@ -355,15 +355,15 @@
                         'text': f'{self.google_author()}',
                         'link': 'next_link',
                     },
                 },
             ],
         }
         response = self.session.post('https://api.twitter.com/1.1/onboarding/task.json', json=json_data)
-        print(f"【{self.username}】【{self.index}】8.输入谷歌验证码验证：{response.text}")
+        logger.info(f"【{self.username}】【{self.index}】8.输入谷歌验证码验证：{response.text}")
 
     def login_flow_get_ct0(self):
         params = {
             'variables': '{"withCommunitiesMemberships":true,"withSubscribedTab":true,"withCommunitiesCreation":true}',
             'features': '{"responsive_web_graphql_exclude_directive_enabled":true,"verified_phone_label_enabled":false,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"responsive_web_graphql_timeline_navigation_enabled":true}',
             'fieldToggles': '{"withAuxiliaryUserLabels":false}',
         }
@@ -376,21 +376,21 @@
             'x-csrf-token': f'{self.session.cookies.get("ct0")}',
             # 'x-guest-token': f'{gt}',
             'x-twitter-active-user': 'yes',
             'x-twitter-client-language': 'zh-cn',
         })
         response = self.session.get('https://twitter.com/i/api/graphql/5wNTkTJmk8GZlJmd2rL7eQ/Viewer', params=params, cookies=cookies)
         self.token_info = self.session.cookies.get_dict()
-        print(f"【{self.username}】【{self.index}】9.获取关键参数ct0：{response.text}")
+        logger.info(f"【{self.username}】【{self.index}】9.获取关键参数ct0：{response.text}")
 
     def save_user_token_info(self, filename):
         cookies_dict = self.session.cookies.get_dict()
         result = f"{self.index}----{self.email}----{self.username}----{self.password}----{self.phone}----{cookies_dict}"
         with open(f"{filename}", 'a', encoding='utf-8') as f1:
-            print(f"{result}")
+            logger.info(f"{result}")
             f1.write(f'{result}\n')
 
     def refresh_session(self):
         # if self.token_info.get("ct0"):
         #     return True
         cookies = {
             'auth_token': f'{self.token_info["auth_token"]}',
@@ -416,24 +416,24 @@
             'category': 'perftown',
             'log': '[{"description":"rweb:urt:notifications:fetch_Top:success","product":"rweb","duration_ms":667},{"description":"rweb:urt:notifications:fetch_Top:format:success","product":"rweb","duration_ms":667}]',
         }
         s = requests.Session()
         s.headers.update(headers)
         s.cookies.update(cookies)
         response = s.post('https://api.twitter.com/1.1/jot/client_event.json', data=data)
-        # print(f'【{self.index}】【{self.token_info["username"]}】：{response.status_code}')
+        # logger.info(f'【{self.index}】【{self.token_info["username"]}】：{response.status_code}')
         if response.status_code != 200:
-            print(f'【{self.index}】【{self.token_info["username"]}】已过期或者被冻结: {response.status_code}')
+            logger.info(f'【{self.index}】【{self.token_info["username"]}】已过期或者被冻结: {response.status_code}')
             if "ct0" in self.token_info:
                 self.token_info.pop("ct0")
             return False
         else:
             self.token_info["ct0"] = s.cookies.get("ct0")
             self.tw_ok = True
-            # print(f'【{self.index}】【{self.token_info["username"]}】刷新session成功！')
+            # logger.info(f'【{self.index}】【{self.token_info["username"]}】刷新session成功！')
             return True
             # account["twitter"] = twitter_info1
 
     def verify_tw(self, auth_token, ct0=None):
         cookies = {
             'auth_token': f'{auth_token}',
         }
@@ -461,29 +461,29 @@
             })
         data = {
             'debug': 'true',
             'log': '[{"_category_":"client_event","format_version":2,"triggered_on":1708871665825,"profile_id":"1366019760710955009","position":0,"items":[{"item_type":3,"id":"1366019760710955009","is_viewer_follows_user":false,"is_user_follows_viewer":false,"is_viewer_super_following_user":false,"is_viewer_super_followed_by_user":false,"is_user_super_followable":false}],"event_namespace":{"page":"me","section":"sidebar","component":"unified_events","action":"impression","client":"m5"},"client_event_sequence_start_timestamp":1708870835759,"client_event_sequence_number":156,"client_app_id":"3033300"}]',
         }
         response = requests.post('https://twitter.com/i/api/1.1/jot/client_event.json', cookies=cookies, headers=headers, data=data)
         if response.status_code != 200:
-            print(f'【{self.username}】已过期或者被冻结: {response.status_code}')
+            logger.info(f'【{self.username}】已过期或者被冻结: {response.status_code}')
             return -1
         else:
             if "This request requires a matching csrf cookie and header." in response.text:
-                print(f'【{self.username}】推特疑似正常，继续验证: {response.status_code}')
+                logger.info(f'【{self.username}】推特疑似正常，继续验证: {response.status_code}')
                 ct0 = response.cookies.get("ct0")
                 return self.verify_tw(auth_token, ct0)
             elif "temporarily locked" in response.text:
-                print(f'【{self.username}】推特被临时冻结: {response.status_code}，报文:{response.text}')
+                logger.info(f'【{self.username}】推特被临时冻结: {response.status_code}，报文:{response.text}')
                 return -2
             elif "is not permitted to access this feature" in response.text:
-                print(f'【{self.username}】推特被完全冻结: {response.status_code}，报文:{response.text}')
+                logger.info(f'【{self.username}】推特被完全冻结: {response.status_code}，报文:{response.text}')
                 return -3
             else:
-                print(f'【{self.username}】推特真的正常:{response.status_code}，报文:{response.text}')
+                logger.info(f'【{self.username}】推特真的正常:{response.status_code}，报文:{response.text}')
                 return 1
 
     def refresh_by_session(self):
         # if self.token_info.get("ct0"):
         #     return True
         cookies = {
             'auth_token': f'{self.session.cookies.get("auth_token")}',
@@ -508,23 +508,23 @@
         data = {
             'category': 'perftown',
             'log': '[{"description":"rweb:urt:notifications:fetch_Top:success","product":"rweb","duration_ms":667},{"description":"rweb:urt:notifications:fetch_Top:format:success","product":"rweb","duration_ms":667}]',
         }
         self.session.headers.update(headers)
         self.session.cookies.update(cookies)
         response = self.session.post('https://api.twitter.com/1.1/jot/client_event.json', data=data)
-        # print(f'【{self.index}】【{self.token_info["username"]}】：{response.status_code}')
+        # logger.info(f'【{self.index}】【{self.token_info["username"]}】：{response.status_code}')
         if response.status_code != 200:
-            print(f'【{self.index}】【{self.token_info["username"]}】已过期或者被冻结: {response.status_code}')
+            logger.info(f'【{self.index}】【{self.token_info["username"]}】已过期或者被冻结: {response.status_code}')
             self.token_info.pop("ct0")
             return False
         else:
             # self.token_info["ct0"] = s.cookies.get("ct0")
             self.token_info = self.session.cookies.get_dict()
-            # print(f'【{self.index}】【{self.token_info["username"]}】刷新session成功！')
+            # logger.info(f'【{self.index}】【{self.token_info["username"]}】刷新session成功！')
             return True
             # account["twitter"] = twitter_info1
 
     def inbox_initial_state(self):
         cookies = {
             'kdt': f'{self.token_info.get("kdt")}',
             'auth_token': f'{self.token_info.get("auth_token")}',
@@ -575,18 +575,18 @@
             'supports_reactions': 'true',
             'include_ext_edit_control': 'true',
             'ext': 'mediaColor,altText,mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,superFollowMetadata,unmentionInfo,editControl',
         }
 
         response = self.session.get('https://twitter.com/i/api/1.1/dm/inbox_initial_state.json', params=params, cookies=cookies, headers=headers)
         if "You are not currently active" in response.text:
-            print(f'【{self.username}】被完全冻结，GG啦！')
+            logger.info(f'【{self.username}】被完全冻结，GG啦！')
             return False
         elif 'this account is temporarily locked' in response.text:
-            print(f'【{self.username}】被临时冻结，需要手动解冻！')
+            logger.info(f'【{self.username}】被临时冻结，需要手动解冻！')
             return False
         else:
             return True
 
     def get_tweet_detail_by_id(self, tweet_id):
         tw_info = self.tw_map.get(f'{tweet_id}', None)
         if tw_info:
@@ -617,29 +617,29 @@
             'fieldToggles': '{"withAuxiliaryUserLabels":false}',
         }
         response = self.session.get('https://twitter.com/i/api/graphql/xc8f1g7BYqr6VTzTbvNlGw/UserByScreenName', params=params)
         if "UserUnavailable" not in response.text:
             user_info = response.json()["data"]["user"]["result"]["legacy"]
             friends_count = user_info["friends_count"]
             followers_count = user_info["followers_count"]
-            print(f'【{self.username}】【{self.index}】查询用户【{username}】,粉丝数：{friends_count},关注数：{followers_count}')
+            logger.info(f'【{self.username}】【{self.index}】查询用户【{username}】,粉丝数：{friends_count},关注数：{followers_count}')
             return response.json()
         else:
-            print(f'【{self.username}】【{self.index}】查询用户【{username}】,报文:{response.text}')
+            logger.info(f'【{self.username}】【{self.index}】查询用户【{username}】,报文:{response.text}')
             return None
 
     def follow_by_name(self, username):
         """根据用户名关注"""
         if not username or username == self.username:
             return
         userinfo = self.get_user_by_screen_name(username)
         if not userinfo:
             return False
         if "following" in str(userinfo):
-            print(f'【{self.username}】【{self.index}】已经关注过【{username}】')
+            logger.info(f'【{self.username}】【{self.index}】已经关注过【{username}】')
             return True
         headers = {
             'authority': 'twitter.com',
             'accept': '*/*',
             'accept-language': 'zh-CN,zh;q=0.9',
             'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
             'cache-control': 'no-cache',
@@ -664,18 +664,18 @@
             'include_ext_verified_type': '1',
             'include_ext_profile_image_shape': '1',
             'skip_status': '1',
             'user_id': f'{userinfo["data"]["user"]["result"]["rest_id"]}',
         }
         response = self.session.post('https://twitter.com/i/api/1.1/friendships/create.json', data=data, headers=headers)
         if "UserUnavailable" not in response.text:
-            print(f'【{self.username}】【{self.index}】关注【{username}】成功,报文:{response.text}')
+            logger.info(f'【{self.username}】【{self.index}】关注【{username}】成功,报文:{response.text}')
             return True
         else:
-            print(f'【{self.username}】【{self.index}】关注【{username}】失败,报文:{response.text}')
+            logger.info(f'【{self.username}】【{self.index}】关注【{username}】失败,报文:{response.text}')
             return False
 
     def unfollow_by_name(self, username):
         """根据用户名取消关注"""
         userinfo = self.get_user_by_screen_name(username)
         if not userinfo:
             return
@@ -706,17 +706,17 @@
             'include_ext_profile_image_shape': '1',
             'skip_status': '1',
             'user_id': f'{userinfo["data"]["user"]["result"]["rest_id"]}',
         }
         response = self.session.post('https://twitter.com/i/api/1.1/friendships/destroy.json', headers=headers,
                                      data=data)
         if response.status_code == 200:
-            print(f'【{self.username}】【{self.index}】取关成功,报文:{response.text}')
+            logger.info(f'【{self.username}】【{self.index}】取关成功,报文:{response.text}')
         else:
-            print(f'【{self.username}】【{self.index}】取关失败,报文:{response.text}')
+            logger.info(f'【{self.username}】【{self.index}】取关失败,报文:{response.text}')
 
     # 发推
     def tweet(self, content):
         json_data = {
             'variables': {
                 'tweet_text': f'{content} \n ',
                 'dark_request': False,
@@ -755,18 +755,18 @@
         response = self.session.post(
             'https://twitter.com/i/api/graphql/SoVnbfCycZ7fERGCwpZkYA/CreateTweet',
             json=json_data,
         )
         if "errors" not in response.text and response.status_code != 404:
             result = response.json()['data']['create_tweet']['tweet_results']['result']
             tweet_url = f'https://twitter.com/{result["core"]["user_results"]["result"]["legacy"]["screen_name"]}/status/{result["rest_id"]}'
-            print(f'【{self.username}】【{self.index}】发推成功,推文链接：{tweet_url},报文:{response.text}')
+            logger.info(f'【{self.username}】【{self.index}】发推成功,推文链接：{tweet_url},报文:{response.text}')
             return tweet_url
         else:
-            print(f'【{self.username}】【{self.index}】发推失败,报文:{response.text}')
+            logger.info(f'【{self.username}】【{self.index}】发推失败,报文:{response.text}')
             return None
 
     def reply_tweet(self, tweet_id, content):
         """回复留言指定推特"""
         json_data = {
             'variables': {
                 'tweet_text': f'{content}',
@@ -810,126 +810,126 @@
         }
 
         response = self.session.post(
             'https://twitter.com/i/api/graphql/SoVnbfCycZ7fERGCwpZkYA/CreateTweet',
             json=json_data,
         )
         if response.status_code == 200:
-            print(f'【{self.username}】【{self.index}】回复推特成功,报文:{response.text}')
+            logger.info(f'【{self.username}】【{self.index}】回复推特成功,报文:{response.text}')
             return f'https://twitter.com/{self.username}/status/{response.json()["data"]["create_tweet"]["tweet_results"]["result"]["rest_id"]}'
         else:
-            print(f'【{self.username}】【{self.index}】回复推特失败,报文:{response.text}')
+            logger.info(f'【{self.username}】【{self.index}】回复推特失败,报文:{response.text}')
             return None
 
     def retweet(self, tweet_id, tw_info=None):
         """转推指定推特"""
         if not tw_info:
             tw_info = self.get_tweet_detail_by_id(tweet_id)
         if not tw_info:
-            # print(f'【{self.username}】【{self.index}】推特:{tweet_id},不存在！跳过！')
+            # logger.info(f'【{self.username}】【{self.index}】推特:{tweet_id},不存在！跳过！')
             json_data = {
                 'variables': {
                     'tweet_id': f'{tweet_id}',
                     'dark_request': False,
                 },
                 'queryId': 'ojPdsZsimiJrUGLR1sjUtA',
             }
             response = self.session.post(
                 'https://twitter.com/i/api/graphql/ojPdsZsimiJrUGLR1sjUtA/CreateRetweet',
                 json=json_data,
             )
             if response.status_code == 200:
                 if "have already retweeted this Tweet" in response.text:
-                    print(f'【{self.username}】【{self.index}】推特:{tweet_id},已经转推过！')
+                    logger.info(f'【{self.username}】【{self.index}】推特:{tweet_id},已经转推过！')
                 else:
-                    print(f'【{self.username}】【{self.index}】推特:{tweet_id},转推成功,报文:{response.text}')
+                    logger.info(f'【{self.username}】【{self.index}】推特:{tweet_id},转推成功,报文:{response.text}')
             else:
-                print(f'【{self.username}】【{self.index}】转推失败,报文:{response.text}')
+                logger.info(f'【{self.username}】【{self.index}】转推失败,报文:{response.text}')
             return
         if tw_info["retweeted"]:
-            print(f'【{self.username}】【{self.index}】推特:{tweet_id},已经转推过！跳过！')
+            logger.info(f'【{self.username}】【{self.index}】推特:{tweet_id},已经转推过！跳过！')
             return
         json_data = {
             'variables': {
                 'tweet_id': f'{tweet_id}',
                 'dark_request': False,
             },
             'queryId': 'ojPdsZsimiJrUGLR1sjUtA',
         }
         response = self.session.post(
             'https://twitter.com/i/api/graphql/ojPdsZsimiJrUGLR1sjUtA/CreateRetweet',
             json=json_data,
         )
         if response.status_code == 200:
             if "have already retweeted this Tweet" in response.text:
-                print(f'【{self.username}】【{self.index}】推特:{tweet_id},已经转推过！')
+                logger.info(f'【{self.username}】【{self.index}】推特:{tweet_id},已经转推过！')
             else:
-                print(f'【{self.username}】【{self.index}】推特:{tweet_id},转推成功,报文:{response.text}')
+                logger.info(f'【{self.username}】【{self.index}】推特:{tweet_id},转推成功,报文:{response.text}')
         else:
-            print(f'【{self.username}】【{self.index}】转推失败,报文:{response.text}')
+            logger.info(f'【{self.username}】【{self.index}】转推失败,报文:{response.text}')
 
     def like(self, tweet_id, tw_info=None):
         if not tw_info:
             tw_info = self.get_tweet_detail_by_id(tweet_id)
         if not tw_info:
-            # print(f'【{self.username}】【{self.index}】推特:{tweet_id},不存在！跳过！')
+            # logger.info(f'【{self.username}】【{self.index}】推特:{tweet_id},不存在！跳过！')
             json_data = {
                 'variables': {
                     'tweet_id': f'{tweet_id}',
                 },
                 'queryId': 'lI07N6Otwv1PhnEgXILM7A',
             }
             response = self.session.post(
                 'https://twitter.com/i/api/graphql/lI07N6Otwv1PhnEgXILM7A/FavoriteTweet',
                 json=json_data,
             )
             if response.status_code == 200:
                 if "already favorited tweet" in response.text:
-                    print(f'【{self.username}】【{self.index}】推特:{tweet_id},已经like过！')
+                    logger.info(f'【{self.username}】【{self.index}】推特:{tweet_id},已经like过！')
                 else:
-                    print(f'【{self.username}】【{self.index}】喜欢推特成功,报文:{response.text}')
+                    logger.info(f'【{self.username}】【{self.index}】喜欢推特成功,报文:{response.text}')
             else:
-                print(f'【{self.username}】【{self.index}】喜欢推特失败,报文:{response.text}')
+                logger.info(f'【{self.username}】【{self.index}】喜欢推特失败,报文:{response.text}')
             return
         if tw_info["favorited"]:
-            print(f'【{self.username}】【{self.index}】推特:{tweet_id},已经like过！跳过！')
+            logger.info(f'【{self.username}】【{self.index}】推特:{tweet_id},已经like过！跳过！')
             return
         json_data = {
             'variables': {
                 'tweet_id': f'{tweet_id}',
             },
             'queryId': 'lI07N6Otwv1PhnEgXILM7A',
         }
         response = self.session.post(
             'https://twitter.com/i/api/graphql/lI07N6Otwv1PhnEgXILM7A/FavoriteTweet',
             json=json_data,
         )
         if response.status_code == 200:
             if "already favorited tweet" in response.text:
-                print(f'【{self.username}】【{self.index}】推特:{tweet_id},已经like过！')
+                logger.info(f'【{self.username}】【{self.index}】推特:{tweet_id},已经like过！')
             else:
-                print(f'【{self.username}】【{self.index}】喜欢推特成功,报文:{response.text}')
+                logger.info(f'【{self.username}】【{self.index}】喜欢推特成功,报文:{response.text}')
         else:
-            print(f'【{self.username}】【{self.index}】喜欢推特失败,报文:{response.text}')
+            logger.info(f'【{self.username}】【{self.index}】喜欢推特失败,报文:{response.text}')
 
     def retweet_and_like(self, tweet_id):
         """转推并且喜欢指定推特"""
         tw_info = self.get_tweet_detail_by_id(tweet_id)
         if not tw_info:
-            print(f'【{self.username}】【{self.index}】推特:{tweet_id},不存在！跳过！')
+            logger.info(f'【{self.username}】【{self.index}】推特:{tweet_id},不存在！跳过！')
             return
         if tw_info["retweeted"]:
-            print(f'【{self.username}】【{self.index}】推特:{tweet_id},已经转推过！跳过！')
+            logger.info(f'【{self.username}】【{self.index}】推特:{tweet_id},已经转推过！跳过！')
         else:
-            # print(f'【{self.username}】【{self.index}】推特:{tweet_id},未转推,开始转推！')
+            # logger.info(f'【{self.username}】【{self.index}】推特:{tweet_id},未转推,开始转推！')
             self.retweet(tweet_id, tw_info)
         if tw_info["favorited"]:
-            print(f'【{self.username}】【{self.index}】推特:{tweet_id},已经like过！跳过！')
+            logger.info(f'【{self.username}】【{self.index}】推特:{tweet_id},已经like过！跳过！')
         else:
-            # print(f'【{self.username}】【{self.index}】推特:{tweet_id},未like,开始like！')
+            # logger.info(f'【{self.username}】【{self.index}】推特:{tweet_id},未like,开始like！')
             self.like(tweet_id, tw_info)
 
     def change_password(self, new_password):
         """修改密码"""
         cookies = {
             'kdt': f'{self.token_info.get("kdt")}',
             'auth_token': f'{self.token_info.get("auth_token")}',
@@ -959,17 +959,17 @@
             'password': f'{new_password}',
             'password_confirmation': f'{new_password}',
         }
         response = self.session.post('https://twitter.com/i/api/i/account/change_password.json', headers=headers,
                                      cookies=cookies, data=data)
         if response.status_code == 200:
             self.password = new_password
-            print(f'【{self.username}】修改密码成功,报文:{response.text}')
+            logger.info(f'【{self.username}】修改密码成功,报文:{response.text}')
         else:
-            print(f'【{self.username}】修改密码失败,报文:{response.text}')
+            logger.info(f'【{self.username}】修改密码失败,报文:{response.text}')
 
     def set_no_pro(self):
         cookies = {
             'kdt': f'{self.token_info.get("kdt")}',
             'auth_token': f'{self.token_info.get("auth_token")}',
             'ct0': f'{self.token_info.get("ct0")}',
         }
@@ -1004,17 +1004,17 @@
             'x-csrf-token': f'{self.token_info.get("ct0")}',
             'x-twitter-active-user': 'yes',
             'x-twitter-auth-type': 'OAuth2Session',
             'x-twitter-client-language': 'zh-cn',
         }
         response = self.session.post('https://api.twitter.com/1.1/account/settings.json', cookies=cookies, headers=headers, data=data)
         if response.status_code == 200:
-            print(f'【{self.username}】设置帖子公开成功,报文:{response.text}')
+            logger.info(f'【{self.username}】设置帖子公开成功,报文:{response.text}')
         else:
-            print(f'【{self.username}】设置帖子公开失败,报文:{response.text}')
+            logger.info(f'【{self.username}】设置帖子公开失败,报文:{response.text}')
 
     def authorize(self, params):
         """
         授权推特
         """
         cookies = {
             'kdt': f'{self.token_info.get("kdt")}',
@@ -1031,26 +1031,26 @@
             'x-client-transaction-id': 'tTLaZPJGhndMIE7MAPffR+tQFmeJC9XAwNnVEC0MWJVfzL6JAB4vtK9qN/uCLZA9i0z5wrXbszyivxg5H19LKSKyCU55tA',
             'x-csrf-token': f'{self.token_info.get("ct0")}',
             'x-twitter-active-user': 'yes',
             'x-twitter-auth-type': 'OAuth2Session',
             'x-twitter-client-language': 'zh-cn',
         }
         response = self.session.get('https://twitter.com/i/api/2/oauth2/authorize', params=params, cookies=cookies, headers=headers)
-        # print(response.text)
+        # logger.info(response.text)
         auth_code = response.json()['auth_code']
         data = {
             'approval': 'true',
             'code': f'{auth_code}',
         }
         response = self.session.post('https://twitter.com/i/api/2/oauth2/authorize', headers=headers, cookies=cookies, data=data)
         if response.status_code == 200:
-            print(f'推特授权成功！！')
+            logger.info(f'推特授权成功！！')
             return auth_code
         else:
-            print(f'推特授权失败！！')
+            logger.info(f'推特授权失败！！')
             return None
 
     def authorize_v1(self, params):
         """推特的第一个版本的授权"""
         cookies = {
             # 'kdt': f'{self.token_info.get("kdt")}',
             'auth_token': f'{self.token_info.get("auth_token")}',
@@ -1084,26 +1084,26 @@
         authenticity_token = soup.find("input", {"name": "authenticity_token"}).get("value")
         data = {
             'authenticity_token': authenticity_token,
             'redirect_after_login': f'https://api.twitter.com/oauth/authorize?oauth_token={oauth_token}',
             'oauth_token': oauth_token,
         }
         response = new_sw1.post('https://api.twitter.com/oauth/authorize', cookies=cookies, headers=headers, data=data)
-        # print(response.status_code, 2)
+        # logger.info(response.status_code, 2)
         soup = BeautifulSoup(response.text, 'html.parser')
         a_tag = soup.find('a', class_='maintain-context')
         oauth_verifier = ""
         if a_tag:
             href = a_tag['href']
-            print(f'【{self.index}】【{self.username}】提取回调链接:{href}')
+            logger.info(f'【{self.index}】【{self.username}】提取回调链接:{href}')
             # requests.Session().get(href)
             paramxs = QGFile.url_params_to_object(href)
             oauth_verifier = paramxs["oauth_verifier"]
         else:
-            print("未找到指定的<a>标签")
+            logger.info("未找到指定的<a>标签")
         return oauth_verifier
 
     def authorize_v1_1(self, params):
         """推特的第一个版本的授权"""
         cookies = {
             # 'kdt': f'{self.token_info.get("kdt")}',
             'auth_token': f'{self.token_info.get("auth_token")}',
@@ -1137,27 +1137,27 @@
         authenticity_token = soup.find("input", {"name": "authenticity_token"}).get("value")
         data = {
             'authenticity_token': authenticity_token,
             'redirect_after_login': f'https://api.twitter.com/oauth/authorize?oauth_token={oauth_token}',
             'oauth_token': oauth_token,
         }
         response = new_sw1.post('https://api.twitter.com/oauth/authorize', cookies=cookies, headers=headers, data=data)
-        # print(response.status_code, 2)
+        # logger.info(response.status_code, 2)
         soup = BeautifulSoup(response.text, 'html.parser')
         a_tag = soup.find('a', class_='maintain-context')
         oauth_verifier = ""
         if a_tag:
             href = a_tag['href']
-            # print(f'【{self.index}】【{self.username}】提取回调链接:{href}')
+            # logger.info(f'【{self.index}】【{self.username}】提取回调链接:{href}')
             requests.Session().get(href)
             params = QGFile.url_params_to_object(href)
             oauth_verifier = params["oauth_verifier"]
             return oauth_verifier, href
         else:
-            print("未找到指定的<a>标签")
+            logger.info("未找到指定的<a>标签")
 
     def authorize_v1_2(self, params):
         """推特的第一个版本的授权"""
         cookies = {
             # 'kdt': f'{self.token_info.get("kdt")}',
             'auth_token': f'{self.token_info.get("auth_token")}',
             'ct0': f'{self.token_info.get("ct0")}',
@@ -1179,21 +1179,21 @@
         }
         new_sw1 = requests.Session()
         response = new_sw1.get('https://api.twitter.com/oauth/authenticate', params=params, cookies=cookies, headers=headers)
         soup = BeautifulSoup(response.text, 'html.parser')
         a_tag = soup.find('a', class_='maintain-context')
         if a_tag:
             href = a_tag['href']
-            # print(f'【{self.index}】【{self.username}】提取回调链接:{href}')
+            # logger.info(f'【{self.index}】【{self.username}】提取回调链接:{href}')
             requests.Session().get(href)
             params = QGFile.url_params_to_object(href)
             oauth_verifier = params["oauth_verifier"]
             return oauth_verifier, href
         else:
-            print("未找到指定的<a>标签")
+            logger.info("未找到指定的<a>标签")
 
     def authorize_v1_3(self, params):
         """推特的第一个版本的授权"""
         cookies = {
             # 'kdt': f'{self.token_info.get("kdt")}',
             'auth_token': f'{self.token_info.get("auth_token")}',
             'ct0': f'{self.token_info.get("ct0")}',
@@ -1224,26 +1224,26 @@
         authenticity_token = soup.find("input", {"name": "authenticity_token"}).get("value")
         data = {
             'authenticity_token': authenticity_token,
             'redirect_after_login': f'https://api.twitter.com/oauth/authorize?oauth_token={oauth_token}',
             'oauth_token': oauth_token,
         }
         response = new_sw1.post('https://api.twitter.com/oauth/authorize', cookies=cookies, headers=headers, data=data)
-        # print(response.status_code, 2)
+        # logger.info(response.status_code, 2)
         soup = BeautifulSoup(response.text, 'html.parser')
         a_tag = soup.find('a', class_='maintain-context')
         if a_tag:
             href = a_tag['href']
-            print(f'【{self.index}】【{self.username}】提取回调链接:{href}')
+            logger.info(f'【{self.index}】【{self.username}】提取回调链接:{href}')
             # requests.Session().get(href)
             paramxs = QGFile.url_params_to_object(href)
             oauth_verifier = paramxs["oauth_verifier"]
             return oauth_verifier, href
         else:
-            print("未找到指定的<a>标签")
+            logger.info("未找到指定的<a>标签")
         return None
 
     def authorize_v2(self, params):
         """推特的第二个版本的授权"""
         cookies = {
             'kdt': f'{self.token_info.get("kdt")}',
             'auth_token': f'{self.token_info.get("auth_token")}',
@@ -1259,15 +1259,15 @@
             'x-client-transaction-id': 'tTLaZPJGhndMIE7MAPffR+tQFmeJC9XAwNnVEC0MWJVfzL6JAB4vtK9qN/uCLZA9i0z5wrXbszyivxg5H19LKSKyCU55tA',
             'x-csrf-token': f'{self.token_info.get("ct0")}',
             'x-twitter-active-user': 'yes',
             'x-twitter-auth-type': 'OAuth2Session',
             'x-twitter-client-language': 'zh-cn',
         }
         response = self.session.get('https://twitter.com/i/api/2/oauth2/authorize', params=params, cookies=cookies, headers=headers)
-        print(f'【{self.index}】【{self.username}】授权推特步骤2:{response.text}')
+        logger.info(f'【{self.index}】【{self.username}】授权推特步骤2:{response.text}')
         auth_code = response.json()['auth_code']
         headers = {
             'authority': 'twitter.com',
             'accept': '*/*',
             'accept-language': 'zh-CN,zh;q=0.9',
             'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
             'cache-control': 'no-cache',
@@ -1284,15 +1284,15 @@
             'x-twitter-client-language': 'zh-cn',
         }
         data = {
             'approval': 'true',
             'code': f'{auth_code}',
         }
         response = self.session.post('https://twitter.com/i/api/2/oauth2/authorize', headers=headers, data=data)
-        print(f'【{self.index}】【{self.username}】授权推特步骤3:{response.text}')
+        logger.info(f'【{self.index}】【{self.username}】授权推特步骤3:{response.text}')
         return auth_code
 
     def access(self):
         """解冻"""
         headers = {
             'authority': 'twitter.com',
             'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
@@ -1324,17 +1324,17 @@
             'authenticity_token': f'{authenticity_token}',
             'assignment_token': f'{assignment_token}',
             'lang': 'en',
             'flow': '',
         }
         response = requests.post('https://twitter.com/account/access', cookies=cookies, headers=headers, data=data, allow_redirects=False)
         if response.status_code == 302:
-            print("解冻成功！")
+            logger.info("解冻成功！")
         else:
-            print("解冻失败！")
+            logger.info("解冻失败！")
 
 
 def qg_task(index, em, un, pw, ph, token_info):
     qt = QTwitter(index=index, email=em, password=pw, username=un, phone=ph, token_info=token_info)
     # # 邮箱登录的方式
     # qt.login_by_email()
     # # 用户名登录的方式
```

### Comparing `qg_toolkit-1.0.17/qg_toolkit/tools/yescaptcha.py` & `qg_toolkit-1.0.18/qg_toolkit/tools/yescaptcha.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 import requests
-
+from loguru import logger
 
 class YesCaptcha:
     requests.packages.urllib3.disable_warnings()
     headers = {
         'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Safari/537.36',
     }
 
@@ -27,25 +27,25 @@
                 "websiteURL": self.website_url,
                 "websiteKey": self.website_key,
                 "type": self.task_type
             }
         }
         if args:
             data["task"].update(args)
-        # print(f'传参：{data}')
+        # logger.info(f'传参：{data}')
         try:
             # 发送JSON格式的数据
             result = requests.post(url, json=data, verify=False, headers=self.headers).json()
             taskId = result.get('taskId')
             if taskId is not None:
                 return taskId
-            print(result)
+            logger.info(result)
 
         except Exception as e:
-            print(e)
+            logger.info(e)
 
     def get_response(self, taskID: str):
         """
         第二步：使用taskId获取response
         :param taskID: string
         :return response: string 识别结果
         """
@@ -60,18 +60,18 @@
                     "taskId": taskID
                 }
                 result = requests.post(url, json=data, verify=False, headers=self.headers).json()
                 solution = result.get('solution', {})
                 if solution:
                     response = solution.get('gRecaptchaResponse')
                     if response:
-                        print(result)
+                        logger.info(result)
                         return response
             except Exception as e:
-                print(e)
+                logger.info(e)
             times += 3
             time.sleep(3)
 
     def get_response2(self, taskID: str):
         """
         第二步：使用taskId获取response
         :param taskID: string
@@ -85,33 +85,33 @@
                 data = {
                     "clientKey": self.client_key,
                     "taskId": taskID
                 }
                 result = requests.post(url, json=data, verify=False, headers=self.headers).json()
                 solution = result.get('solution', {})
                 if solution:
-                    print(result)
+                    logger.info(result)
                     return solution
                     # response = solution.get('gRecaptchaResponse')
                     # if response:
-                    #     print(result)
+                    #     logger.info(result)
                     #     return response
             except Exception as e:
-                print(e)
+                logger.info(e)
             times += 3
             time.sleep(3)
 
     def get_recaptcha(self, args=None):
         taskId = self.create_task(args)
-        print('创建任务:', taskId)
+        logger.info('创建任务:', taskId)
         if taskId is not None:
             response = self.get_response(taskId)
-            print('识别结果:', response)
+            logger.info('识别结果:', response)
             return response
 
     def get_solution(self, args=None):
         taskId = self.create_task(args)
-        print('创建任务:', taskId)
+        logger.info('创建任务:', taskId)
         if taskId is not None:
             solution = self.get_response2(taskId)
-            print('识别结果:', solution)
+            logger.info('识别结果:', solution)
             return solution
```

### Comparing `qg_toolkit-1.0.17/PKG-INFO` & `qg_toolkit-1.0.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qg_toolkit
-Version: 1.0.17
+Version: 1.0.18
 Summary: qg_toolkit for Python!
 Author: qg
 Author-email: qg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

