# Comparing `tmp/qg_toolkit-1.0.12.tar.gz` & `tmp/qg_toolkit-1.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qg_toolkit-1.0.12.tar", max compression
+gzip compressed data, was "qg_toolkit-1.0.13.tar", max compression
```

## Comparing `qg_toolkit-1.0.12.tar` & `qg_toolkit-1.0.13.tar`

### file list

```diff
@@ -1,74 +1,81 @@
--rw-r--r--   0        0        0      816 2024-04-29 07:39:30.192925 qg_toolkit-1.0.12/pyproject.toml
--rw-r--r--   0        0        0       94 2024-04-28 01:55:09.875818 qg_toolkit-1.0.12/qg_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 01:55:09.876818 qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/__init__.py
--rw-r--r--   0        0        0       94 2024-04-28 01:55:09.876818 qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_fullpage/__init__.py
--rw-r--r--   0        0        0     5190 2024-04-28 01:55:09.877828 qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py
--rw-r--r--   0        0        0     5433 2024-04-28 01:55:09.877828 qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js
--rw-r--r--   0        0        0     2288 2024-04-28 01:55:09.877828 qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py
--rw-r--r--   0        0        0       94 2024-04-28 01:55:09.878819 qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/__init__.py
--rw-r--r--   0        0        0     2723 2024-04-28 01:55:09.878819 qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/gap.py
--rw-r--r--   0        0        0    35544 2024-04-28 01:55:09.879819 qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py
--rw-r--r--   0        0        0    51280 2024-04-28 01:55:09.880829 qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png
--rw-r--r--   0        0        0     4818 2024-04-28 01:55:09.880829 qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png
--rw-r--r--   0        0        0     9121 2024-04-28 01:55:09.881818 qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png
--rw-r--r--   0        0        0  1793853 2024-04-28 01:55:09.890818 qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json
--rw-r--r--   0        0        0     2362 2024-04-28 01:55:09.890818 qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js
--rw-r--r--   0        0        0     2349 2024-04-28 01:55:09.891818 qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/mian.py
--rw-r--r--   0        0        0     1043 2024-04-28 01:55:09.891818 qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/trace.py
--rw-r--r--   0        0        0     2764 2024-04-29 07:27:04.914712 qg_toolkit-1.0.12/qg_toolkit/qgalxe/GeetestFullPageV4.py
--rw-r--r--   0        0        0       96 2024-04-28 01:55:09.892818 qg_toolkit-1.0.12/qg_toolkit/qtweepy/__init__.py
--rw-r--r--   0        0        0      103 2024-04-28 01:55:09.892818 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/__init__.py
--rw-r--r--   0        0        0     4912 2024-04-28 06:26:10.954966 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/account_checker.py
--rw-r--r--   0        0        0     2251 2024-04-28 01:55:09.893817 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/follow_each_other.py
--rw-r--r--   0        0        0        0 2024-04-28 06:38:00.187702 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/input-output/BAD_TOKEN.txt
--rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/input-output/CONSENT_LOCKED.txt
--rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/input-output/GOOD.txt
--rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/input-output/LOCKED.txt
--rw-r--r--   0        0        0       44 2024-04-28 06:37:01.438691 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/input-output/PROXIES.txt
--rw-r--r--   0        0        0        0 2024-04-28 06:38:00.187702 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/input-output/SUSPENDED.txt
--rw-r--r--   0        0        0       40 2024-04-28 06:38:00.187702 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/input-output/UNKNOWN.txt
--rw-r--r--   0        0        0     3622 2024-04-28 01:55:09.894817 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/mavia.py
--rw-r--r--   0        0        0     2373 2024-04-28 01:55:09.895818 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/set_2fa.py
--rw-r--r--   0        0        0     3081 2024-04-28 01:55:09.895818 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py
--rw-r--r--   0        0        0      697 2024-04-28 01:55:09.895818 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/uploading_images.py
--rw-r--r--   0        0        0     2253 2024-04-28 01:55:09.896820 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/voter.py
--rw-r--r--   0        0        0     3120 2024-04-28 01:55:09.896820 qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/xai.py
--rw-r--r--   0        0        0      687 2024-04-28 01:55:09.896820 qg_toolkit-1.0.12/qg_toolkit/qtweepy/pyproject.toml
--rw-r--r--   0        0        0     8720 2024-04-28 01:55:09.892818 qg_toolkit-1.0.12/qg_toolkit/qtweepy/README.md
--rw-r--r--   0        0        0      132 2024-04-28 01:55:09.897831 qg_toolkit-1.0.12/qg_toolkit/qtweepy/tea.yaml
--rw-r--r--   0        0        0      732 2024-04-28 01:55:09.897831 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 01:55:09.897831 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/_capsolver/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 01:55:09.897831 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/_capsolver/core/__init__.py
--rw-r--r--   0        0        0     8883 2024-04-28 01:55:09.898831 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py
--rw-r--r--   0        0        0     1054 2024-04-28 01:55:09.898831 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py
--rw-r--r--   0        0        0     1741 2024-04-28 01:55:09.899826 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py
--rw-r--r--   0        0        0     2602 2024-04-28 01:55:09.899826 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py
--rw-r--r--   0        0        0    10974 2024-04-28 01:55:09.900819 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py
--rw-r--r--   0        0        0     3248 2024-04-28 01:55:09.900819 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/account.py
--rw-r--r--   0        0        0      141 2024-04-28 01:55:09.900819 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/base/__init__.py
--rw-r--r--   0        0        0      500 2024-04-28 01:55:09.901826 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/base/client.py
--rw-r--r--   0        0        0     2175 2024-04-28 01:55:09.901826 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/base/session.py
--rw-r--r--   0        0        0    70738 2024-04-28 01:55:09.902820 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/client.py
--rw-r--r--   0        0        0      267 2024-04-28 01:55:09.902820 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/enums.py
--rw-r--r--   0        0        0     5322 2024-04-28 01:55:09.903823 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/errors.py
--rw-r--r--   0        0        0     4695 2024-04-28 01:55:09.903823 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/models.py
--rw-r--r--   0        0        0      665 2024-04-28 01:55:09.903823 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/utils/__init__.py
--rw-r--r--   0        0        0     1152 2024-04-28 01:55:09.904830 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/utils/file.py
--rw-r--r--   0        0        0     2140 2024-04-28 01:55:09.904830 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/utils/html.py
--rw-r--r--   0        0        0     1061 2024-04-28 01:55:09.904830 qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/utils/other.py
--rw-r--r--   0        0        0        0 2024-04-28 01:55:09.905829 qg_toolkit-1.0.12/qg_toolkit/test/test.py
--rw-r--r--   0        0        0       96 2024-04-28 01:55:09.905829 qg_toolkit-1.0.12/qg_toolkit/tools/__init__.py
--rw-r--r--   0        0        0      279 2024-04-28 01:55:09.905829 qg_toolkit-1.0.12/qg_toolkit/tools/demo.yaml
--rw-r--r--   0        0        0     5905 2024-04-29 06:52:45.801970 qg_toolkit-1.0.12/qg_toolkit/tools/qg_airdrop.py
--rw-r--r--   0        0        0      985 2024-04-28 01:55:09.906829 qg_toolkit-1.0.12/qg_toolkit/tools/qg_crypto.py
--rw-r--r--   0        0        0    36347 2024-04-29 06:52:45.801970 qg_toolkit-1.0.12/qg_toolkit/tools/qg_eth.py
--rw-r--r--   0        0        0     3594 2024-04-28 01:55:09.907829 qg_toolkit-1.0.12/qg_toolkit/tools/qg_file.py
--rw-r--r--   0        0        0      300 2024-04-28 01:55:09.908828 qg_toolkit-1.0.12/qg_toolkit/tools/qg_models.py
--rw-r--r--   0        0        0      741 2024-04-28 01:55:09.908828 qg_toolkit-1.0.12/qg_toolkit/tools/qg_random.py
--rw-r--r--   0        0        0     6168 2024-04-29 06:52:45.802969 qg_toolkit-1.0.12/qg_toolkit/tools/qg_solana.py
--rw-r--r--   0        0        0     2764 2024-04-28 01:55:09.908828 qg_toolkit-1.0.12/qg_toolkit/tools/qg_starknet.py
--rw-r--r--   0        0        0     3241 2024-04-28 01:55:09.909829 qg_toolkit-1.0.12/qg_toolkit/tools/qproxy.py
--rw-r--r--   0        0        0     6068 2024-04-28 01:55:09.909829 qg_toolkit-1.0.12/qg_toolkit/tools/rpc.py
--rw-r--r--   0        0        0       38 2024-04-22 02:07:22.831782 qg_toolkit-1.0.12/README.md
--rw-r--r--   0        0        0      133 2024-04-29 07:39:30.190911 qg_toolkit-1.0.12/tea.yaml
--rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 qg_toolkit-1.0.12/PKG-INFO
+-rw-r--r--   0        0        0      835 2024-04-29 10:08:21.902960 qg_toolkit-1.0.13/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-28 01:55:09.875818 qg_toolkit-1.0.13/qg_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 01:55:09.876818 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-28 01:55:09.876818 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_fullpage/__init__.py
+-rw-r--r--   0        0        0     5190 2024-04-28 01:55:09.877828 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py
+-rw-r--r--   0        0        0     5433 2024-04-28 01:55:09.877828 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js
+-rw-r--r--   0        0        0     2288 2024-04-28 01:55:09.877828 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py
+-rw-r--r--   0        0        0       94 2024-04-28 01:55:09.878819 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/__init__.py
+-rw-r--r--   0        0        0     2723 2024-04-28 01:55:09.878819 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/gap.py
+-rw-r--r--   0        0        0    35544 2024-04-28 01:55:09.879819 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py
+-rw-r--r--   0        0        0    51280 2024-04-28 01:55:09.880829 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png
+-rw-r--r--   0        0        0     4818 2024-04-28 01:55:09.880829 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png
+-rw-r--r--   0        0        0     9121 2024-04-28 01:55:09.881818 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png
+-rw-r--r--   0        0        0  1793853 2024-04-28 01:55:09.890818 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json
+-rw-r--r--   0        0        0     2362 2024-04-28 01:55:09.890818 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js
+-rw-r--r--   0        0        0     2349 2024-04-28 01:55:09.891818 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/mian.py
+-rw-r--r--   0        0        0     1043 2024-04-28 01:55:09.891818 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/trace.py
+-rw-r--r--   0        0        0   101354 2024-04-29 10:07:07.022169 qg_toolkit-1.0.13/qg_toolkit/qgalxe/galxe.py
+-rw-r--r--   0        0        0     2750 2024-04-29 09:53:39.862145 qg_toolkit-1.0.13/qg_toolkit/qgalxe/GeetestFullPageV4.py
+-rw-r--r--   0        0        0       96 2024-04-28 01:55:09.892818 qg_toolkit-1.0.13/qg_toolkit/qtweepy/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-28 01:55:09.892818 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/__init__.py
+-rw-r--r--   0        0        0     4912 2024-04-28 06:26:10.954966 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/account_checker.py
+-rw-r--r--   0        0        0     2251 2024-04-28 01:55:09.893817 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/follow_each_other.py
+-rw-r--r--   0        0        0        0 2024-04-28 06:38:00.187702 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/input-output/BAD_TOKEN.txt
+-rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/input-output/CONSENT_LOCKED.txt
+-rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/input-output/GOOD.txt
+-rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/input-output/LOCKED.txt
+-rw-r--r--   0        0        0       44 2024-04-28 06:37:01.438691 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/input-output/PROXIES.txt
+-rw-r--r--   0        0        0        0 2024-04-28 06:38:00.187702 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/input-output/SUSPENDED.txt
+-rw-r--r--   0        0        0       40 2024-04-28 06:38:00.187702 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/input-output/UNKNOWN.txt
+-rw-r--r--   0        0        0     3622 2024-04-28 01:55:09.894817 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/mavia.py
+-rw-r--r--   0        0        0     2373 2024-04-28 01:55:09.895818 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/set_2fa.py
+-rw-r--r--   0        0        0     3081 2024-04-28 01:55:09.895818 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py
+-rw-r--r--   0        0        0      697 2024-04-28 01:55:09.895818 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/uploading_images.py
+-rw-r--r--   0        0        0     2253 2024-04-28 01:55:09.896820 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/voter.py
+-rw-r--r--   0        0        0     3120 2024-04-28 01:55:09.896820 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/xai.py
+-rw-r--r--   0        0        0      687 2024-04-28 01:55:09.896820 qg_toolkit-1.0.13/qg_toolkit/qtweepy/pyproject.toml
+-rw-r--r--   0        0        0     8720 2024-04-28 01:55:09.892818 qg_toolkit-1.0.13/qg_toolkit/qtweepy/README.md
+-rw-r--r--   0        0        0      132 2024-04-28 01:55:09.897831 qg_toolkit-1.0.13/qg_toolkit/qtweepy/tea.yaml
+-rw-r--r--   0        0        0      732 2024-04-28 01:55:09.897831 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 01:55:09.897831 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 01:55:09.897831 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/__init__.py
+-rw-r--r--   0        0        0     8883 2024-04-28 01:55:09.898831 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py
+-rw-r--r--   0        0        0     1054 2024-04-28 01:55:09.898831 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py
+-rw-r--r--   0        0        0     1741 2024-04-28 01:55:09.899826 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py
+-rw-r--r--   0        0        0     2602 2024-04-28 01:55:09.899826 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py
+-rw-r--r--   0        0        0    10974 2024-04-28 01:55:09.900819 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py
+-rw-r--r--   0        0        0     3248 2024-04-28 01:55:09.900819 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/account.py
+-rw-r--r--   0        0        0      141 2024-04-28 01:55:09.900819 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/base/__init__.py
+-rw-r--r--   0        0        0      500 2024-04-28 01:55:09.901826 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/base/client.py
+-rw-r--r--   0        0        0     2175 2024-04-28 01:55:09.901826 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/base/session.py
+-rw-r--r--   0        0        0    70738 2024-04-28 01:55:09.902820 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/client.py
+-rw-r--r--   0        0        0      267 2024-04-28 01:55:09.902820 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/enums.py
+-rw-r--r--   0        0        0     5322 2024-04-28 01:55:09.903823 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/errors.py
+-rw-r--r--   0        0        0     4695 2024-04-28 01:55:09.903823 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/models.py
+-rw-r--r--   0        0        0      665 2024-04-28 01:55:09.903823 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/__init__.py
+-rw-r--r--   0        0        0     1152 2024-04-28 01:55:09.904830 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/file.py
+-rw-r--r--   0        0        0     2140 2024-04-28 01:55:09.904830 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/html.py
+-rw-r--r--   0        0        0     1061 2024-04-28 01:55:09.904830 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/other.py
+-rw-r--r--   0        0        0      279 2024-04-28 01:55:09.905829 qg_toolkit-1.0.13/qg_toolkit/test/demo.yaml
+-rw-r--r--   0        0        0        0 2024-04-28 01:55:09.905829 qg_toolkit-1.0.13/qg_toolkit/test/test.py
+-rw-r--r--   0        0        0       96 2024-04-28 01:55:09.905829 qg_toolkit-1.0.13/qg_toolkit/tools/__init__.py
+-rw-r--r--   0        0        0     5264 2024-04-29 10:04:50.990411 qg_toolkit-1.0.13/qg_toolkit/tools/cui_qiu_client.py
+-rw-r--r--   0        0        0     1245 2024-04-29 09:52:12.132611 qg_toolkit-1.0.13/qg_toolkit/tools/date_util.py
+-rw-r--r--   0        0        0    12289 2024-04-29 09:59:28.288628 qg_toolkit-1.0.13/qg_toolkit/tools/discord.py
+-rw-r--r--   0        0        0     5905 2024-04-29 06:52:45.801970 qg_toolkit-1.0.13/qg_toolkit/tools/qg_airdrop.py
+-rw-r--r--   0        0        0      985 2024-04-28 01:55:09.906829 qg_toolkit-1.0.13/qg_toolkit/tools/qg_crypto.py
+-rw-r--r--   0        0        0    36155 2024-04-29 07:53:05.424108 qg_toolkit-1.0.13/qg_toolkit/tools/qg_eth.py
+-rw-r--r--   0        0        0     3594 2024-04-28 01:55:09.907829 qg_toolkit-1.0.13/qg_toolkit/tools/qg_file.py
+-rw-r--r--   0        0        0      300 2024-04-28 01:55:09.908828 qg_toolkit-1.0.13/qg_toolkit/tools/qg_models.py
+-rw-r--r--   0        0        0      741 2024-04-28 01:55:09.908828 qg_toolkit-1.0.13/qg_toolkit/tools/qg_random.py
+-rw-r--r--   0        0        0     6168 2024-04-29 06:52:45.802969 qg_toolkit-1.0.13/qg_toolkit/tools/qg_solana.py
+-rw-r--r--   0        0        0     2764 2024-04-28 01:55:09.908828 qg_toolkit-1.0.13/qg_toolkit/tools/qg_starknet.py
+-rw-r--r--   0        0        0     3241 2024-04-28 01:55:09.909829 qg_toolkit-1.0.13/qg_toolkit/tools/qproxy.py
+-rw-r--r--   0        0        0     1239 2024-04-29 10:01:18.869266 qg_toolkit-1.0.13/qg_toolkit/tools/random_tool.py
+-rw-r--r--   0        0        0     6068 2024-04-28 01:55:09.909829 qg_toolkit-1.0.13/qg_toolkit/tools/rpc.py
+-rw-r--r--   0        0        0    72044 2024-04-29 09:56:23.770716 qg_toolkit-1.0.13/qg_toolkit/tools/twitter.py
+-rw-r--r--   0        0        0     4085 2024-02-09 00:42:50.310936 qg_toolkit-1.0.13/qg_toolkit/tools/yescaptcha.py
+-rw-r--r--   0        0        0       38 2024-04-22 02:07:22.831782 qg_toolkit-1.0.13/README.md
+-rw-r--r--   0        0        0      133 2024-04-29 10:08:30.493855 qg_toolkit-1.0.13/tea.yaml
+-rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 qg_toolkit-1.0.13/PKG-INFO
```

### Comparing `qg_toolkit-1.0.12/pyproject.toml` & `qg_toolkit-1.0.13/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qg_toolkit"
-version = "1.0.12"
+version = "1.0.13"
 description = "qg_toolkit for Python!"
 authors = ["qg <qg@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qg_toolkit"}]
 include = [{path = "tea.yaml"}]
 
 
@@ -28,14 +28,15 @@
 pillow= "^10.3.0"
 ImageHash= "^4.3.1"
 PyYAML= "^6.0.1"
 PySocks= "^1.7.1"
 websockets= "11.0.3"
 web3="^6.17.2"
 playwright="1.43.0"
+capsolver="1.0.7"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py` & `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js` & `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py` & `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/gap.py` & `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/gap.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py` & `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png` & `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png` & `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png` & `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json` & `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js` & `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/mian.py` & `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/mian.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/geetest_captcha/geetest4_slide/trace.py` & `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/trace.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qgalxe/GeetestFullPageV4.py` & `qg_toolkit-1.0.13/qg_toolkit/qgalxe/GeetestFullPageV4.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import time
 
-import faker
 import requests
 from faker import Faker
 from loguru import logger
 from playwright.sync_api import sync_playwright
 
 
 class GeetestFullPageV4:
```

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/account_checker.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/account_checker.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/follow_each_other.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/follow_each_other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/mavia.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/mavia.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/set_2fa.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/set_2fa.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/uploading_images.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/uploading_images.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/voter.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/voter.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/examples/xai.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/xai.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/pyproject.toml` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/README.md` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/README.md`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/__init__.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/account.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/account.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/base/session.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/base/session.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/client.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/client.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/errors.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/errors.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/models.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/models.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/utils/__init__.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/utils/file.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/utils/html.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/html.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/qtweepy/twitter/utils/other.py` & `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/tools/qg_airdrop.py` & `qg_toolkit-1.0.13/qg_toolkit/tools/qg_airdrop.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/tools/qg_crypto.py` & `qg_toolkit-1.0.13/qg_toolkit/tools/qg_crypto.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/tools/qg_eth.py` & `qg_toolkit-1.0.13/qg_toolkit/tools/qg_eth.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,17 +35,17 @@
                 web3 = getattr(self, f"{name}_w3", None)
                 if web3 is None:
                     self.add_chain(name)
                     self.add_balance(name)
             chains_info = []
             for chain_name, web3_instance in self.chain_instances.items():
                 chains_info.append(f"{chain_name}余额:{self.get_balance_by_chain(chain_name)}")
-            print(f"【{self.index}】【{self.address}】余额情况 {','.join(chains_info)}")
+            logger.info(f"【{self.index}】【{self.address}】余额情况 {','.join(chains_info)}")
         except Exception as e:
-            print(e)
+            logger.error(e)
             raise Exception("初始化失败！")
 
     def add_chain(self, chain_name):
         endpoint = endpoints.get(chain_name)
         if endpoint:
             web3 = Web3(Web3.HTTPProvider(endpoint))
             self.chain_instances[chain_name] = web3
@@ -85,23 +85,23 @@
         data = balance_of_method_id + self.address.lower()[2:].zfill(64)
         token_balance = w3.eth.call({
             'to': Web3.to_checksum_address(contract_address),
             'data': data
         })
         hex_balance = binascii.hexlify(token_balance).decode()
         balance = Web3.from_wei(int(hex_balance, 16), 'wei')
-        print(f'【{self.index}】【{self.address}】【合约代币：{contract_address}】余额：{balance}')
+        logger.info(f'【{self.index}】【{self.address}】【合约代币：{contract_address}】余额：{balance}')
         return balance
 
     def get_token_by_w3(self, w3, to_address):
         """
         查询指定代币的余额
         """
         balance = Web3.from_wei(w3.eth.get_balance(Web3.to_checksum_address(to_address)), 'ether')
-        print(f'【{self.index}】【{self.address}】余额：{balance}')
+        logger.info(f'【{self.index}】【{self.address}】余额：{balance}')
         return balance
 
     def get_token_balance_by_abi(self, w3, contract_address):
         ERC20_ABI = [
             {
                 "constant": True,
                 "inputs": [{"name": "_owner", "type": "address"}],
@@ -124,15 +124,15 @@
         # 获取代币合约实例
         contract = w3.eth.contract(address=Web3.to_checksum_address(contract_address), abi=ERC20_ABI)
         # 获取代币余额
         balance = contract.functions.balanceOf(Web3.to_checksum_address(self.address)).call()
         # 将余额转换为代币单位（以太为例，小数点18位）
         decimals = contract.functions.decimals().call()
         balance_in_units = balance / (10 ** decimals)
-        print(f'【{self.address}】【合约代币：{contract_address}】余额：{balance_in_units}')
+        logger.info(f'【{self.address}】【合约代币：{contract_address}】余额：{balance_in_units}')
         return balance_in_units
 
     def get_that_token_balance_by_abi(self, w3, contract_address, addr):
         ERC20_ABI = [
             {
                 "constant": True,
                 "inputs": [{"name": "_owner", "type": "address"}],
@@ -155,15 +155,15 @@
         # 获取代币合约实例
         contract = w3.eth.contract(address=contract_address, abi=ERC20_ABI)
         # 获取代币余额
         balance = contract.functions.balanceOf(Web3.to_checksum_address(addr)).call()
         # 将余额转换为代币单位（以太为例，小数点18位）
         decimals = contract.functions.decimals().call()
         balance_in_units = balance / (10 ** decimals)
-        print(f'【{addr}】【合约代币：{contract_address}】余额：{balance_in_units}')
+        logger.info(f'【{addr}】【合约代币：{contract_address}】余额：{balance_in_units}')
         return balance_in_units
 
     def get_token_by_w3_and_address(self, w3, contract_address, addr):
         abi_json = [{"anonymous": False, "inputs": [{"indexed": False, "internalType": "uint256", "name": "id", "type": "uint256"},
                                                     {"indexed": False, "internalType": "address", "name": "to", "type": "address"},
                                                     {"indexed": False, "internalType": "uint256", "name": "amount", "type": "uint256"},
                                                     {"indexed": False, "internalType": "string", "name": "data", "type": "string"}],
@@ -231,15 +231,15 @@
         # 获取代币合约实例
         contract = w3.eth.contract(address=Web3.to_checksum_address(contract_address), abi=abi_json)
         # 获取代币余额
         balance = contract.functions.balanceOf(Web3.to_checksum_address(addr)).call()
         # 将余额转换为代币单位（以太为例，小数点18位）
         # decimals = contract.functions.decimals().call()
         # balance_in_units = balance / (10 ** decimals)
-        print(f'【{addr}】【合约代币：{contract_address}】余额：{balance}')
+        logger.info(f'【{addr}】【合约代币：{contract_address}】余额：{balance}')
         return balance
 
     def tranfer_token_by_abi(self, qw3, contract_address, to_address, val):
         """
         转任意代币(注意单位！！！)
         """
         # 合约 ABI
@@ -257,15 +257,15 @@
         ]
         # 创建合约对象
         contract = qw3.eth.contract(address=contract_address, abi=abi)
         # 转账操作
         tx_hash = contract.functions.transfer(Web3.to_checksum_address(to_address), val).transact({'from': Web3.to_checksum_address(self.address)})
         # 等待交易确认
         tx_receipt = qw3.eth.waitForTransactionReceipt(tx_hash)
-        print(f"Token【{contract_address}】转给【{to_address}】成功,数量: {val}， hash: {tx_hash}")
+        logger.info(f"Token【{contract_address}】转给【{to_address}】成功,数量: {val}， hash: {tx_hash}")
 
     def get_721_nfts(self, wb3, contract_address, addr=None):
         """
         获取某个账号上的NFT（包括元数据）
         """
         if not addr:
             addr = self.address
@@ -304,56 +304,56 @@
             token_uri = nft_contract.functions.tokenURI(token_id).call()
             if "application/json" in str(token_uri):
                 # 解码 Base64 编码的字符串为字节数据
                 decoded_utf8 = base64.b64decode(token_uri.split('base64,')[1]).decode('utf-8')
                 # 解析 UTF-8 字符串为 JSON 对象
                 token_uri = json.loads(decoded_utf8)
             nft_metadata_list.append({"token_id": token_id, "token_uri": token_uri})
-        print("NFT Metadata for", addr, ":", nft_metadata_list)
+        logger.info("NFT Metadata for", addr, ":", nft_metadata_list)
         return nft_metadata_list
 
     def save_balance_info(self, log_name="余额情况"):
         balance_info = ""
         chains_info = []
         for chain_name, web3_instance in self.chain_instances.items():
             balance_info = f"{balance_info}----【{chain_name}】余额----{self.get_balance_from_attr(chain_name)}"
             chains_info.append(f"{chain_name}余额:{self.get_balance_from_attr(chain_name)}")
-        print(f"【{self.index}】【{self.address}】余额情况 {','.join(chains_info)}")
+        logger.info(f"【{self.index}】【{self.address}】余额情况 {','.join(chains_info)}")
         with open(f"{log_name}.txt", 'a', encoding='utf-8') as f:
             f.write(
                 f'{self.index}----{self.address}----{self.private_key}----{self.mnemonic if self.mnemonic else "无"}----{balance_info}\n')
             f.close()
 
     def sign_msg(self, w3, msg):
         # 消息签名
         message = encode_defunct(text=msg)
         signed_message = w3.eth.account.sign_message(message, private_key=self.private_key)
         signed_data = signed_message.signature
-        # print("签名后:" + signed_data.hex())
+        # logger.info("签名后:" + signed_data.hex())
         return signed_data.hex()
 
     def sign_msg_v2(self, msg):
         # 消息签名
         message = encode_defunct(text=msg)
         signed_message = w3.eth.account.sign_message(message, private_key=self.private_key)
         signed_data = signed_message.signature
-        # print("签名后:" + signed_data.hex())
+        # logger.info("签名后:" + signed_data.hex())
         return signed_data.hex()
 
     def sign_712(self, data):
         encoded_message = encode_typed_data(data)
         signed_message = Account.sign_message(encoded_message, private_key=self.private_key)
-        # print('Signature:', signed_message.signature.hex())
+        # logger.info('Signature:', signed_message.signature.hex())
         return signed_message.signature.hex()
 
     @retry(tries=5, delay=1, backoff=2, max_delay=5)
     def get_data(self, chain_name, req_type, *params):
         url = f"{bases.get(chain_name)}{apis.get(req_type).format(*params)}&page=1&offset=1000&sort=asc"
         resp = requests.Session().get(url)
-        # print(resp.json())
+        # logger.info(resp.json())
         if "Too Many Requests" in resp.text or "Max rate limit reached, please use API Key for higher rate limit" in resp.text:
             raise Exception("重试！")
         return resp.json()['result']
 
     @classmethod
     def check_tx_found_in_txs(cls, txs, to_addr, search_data=None):
         """
@@ -384,15 +384,15 @@
         # gas limit偏移
         max_estimated_gas = estimated_gas + gas_limit_offset
         # gas price偏移
         max_fee_per_gas = gas_price + Decimal(gas_price_offset)
         max_priority_fee_per_gas = gas_price + Decimal(gas_price_offset - 0.001)
         # 计算预估手续费
         estimated_fee_eth = (Decimal(max_estimated_gas) * max_fee_per_gas) / 1000000000
-        print(
+        logger.info(
             f"目标地址【{tx['to']}】:预估Gas:{estimated_gas},预估Gas Price:{gas_price}Gwei,预估手续费:{estimated_fee_eth}Eth")
         # if estimated_fee_eth > fee_eth:
         #     raise Exception(f"手续费：{estimated_fee_eth}过高！跳过！")
         gas_info = {
             "gas": estimated_gas,
             "maxFeePerGas": Web3.to_wei(max_fee_per_gas, "gwei"),  # 最大矿工费用
             'maxPriorityFeePerGas': Web3.to_wei(max_priority_fee_per_gas, 'gwei'),  # 最大优先矿工费用
@@ -439,15 +439,15 @@
 
     def sent_tx_with_assembled(self, w3, to_address, value, input_data, action_name, gas_limit_offset=0.0, gas_price_offset=0.1, fee_eth=0.03,
                                is_wait_tx=True):
         """
         组装参数并发送交易
         """
         nonce = w3.eth.get_transaction_count(Web3.to_checksum_address(self.address), 'pending')
-        print(f'{self.address} nonce:{nonce}')
+        logger.info(f'{self.address} nonce:{nonce}')
         tx = {
             'from': Web3.to_checksum_address(self.address),
             'to': Web3.to_checksum_address(to_address),
             'value': Web3.to_wei(value, 'ether'),
             'data': input_data.lower(),
             # 'nonce': w3.eth.get_transaction_count(Web3.to_checksum_address(self.address)),
             'nonce': nonce,
@@ -456,25 +456,25 @@
         }
         try:
             self.assemble_tx_with_gas(w3, tx, gas_limit_offset=gas_limit_offset, gas_price_offset=gas_price_offset,
                                       fee_eth=fee_eth)
             tx_hash = self.send_tx(w3, tx, to_address, action_name, is_wait_tx)
             return tx_hash
         except Exception as e:
-            print(f"【{self.index}】【{self.address}】动作【{action_name}】预估会失败，跳过！报文：{e}")
+            logger.info(f"【{self.index}】【{self.address}】动作【{action_name}】预估会失败，跳过！报文：{e}")
             return None
 
     def sent_tx_with_assembled_by_type0(self, w3, to_address, value, input_data, action_name, gas=None, gas_price=None, is_wait_tx=True,
                                         is_estimated_tx=False):
         """
         组装参数并发送交易
         """
         try:
             nonce = w3.eth.get_transaction_count(Web3.to_checksum_address(self.address), 'pending')
-            print(f'【{self.index}】【{self.address}】 nonce: {nonce}')
+            logger.info(f'【{self.index}】【{self.address}】 nonce: {nonce}')
             tx = {
                 'from': Web3.to_checksum_address(self.address),
                 'to': Web3.to_checksum_address(to_address),
                 'value': Web3.to_wei(value, 'ether'),
                 # 'nonce': w3.eth.get_transaction_count(Web3.to_checksum_address(self.address)),
                 'nonce': nonce,
                 'chainId': w3.eth.chain_id,
@@ -490,18 +490,18 @@
                 estimated_gas, gas_price = QGEth.get_current_gas_info(w3, tx)
                 tx.update({
                     "gas": estimated_gas,
                     'gasPrice': Web3.to_wei(gas_price, "gwei")
                 })
             if is_estimated_tx:
                 estimated_gas = w3.eth.estimate_gas(tx)
-            print(f"【{self.index}】【{self.address}】动作【{action_name}】tx:{tx}")
+            logger.info(f"【{self.index}】【{self.address}】动作【{action_name}】tx:{tx}")
             return self.send_tx(w3, tx, to_address, action_name, is_wait_tx)
         except Exception as e:
-            print(f"【{self.index}】【{self.address}】动作【{action_name}】预估会失败，跳过！报文：{e}")
+            logger.info(f"【{self.index}】【{self.address}】动作【{action_name}】预估会失败，跳过！报文：{e}")
 
     def sent_with_full_tx(self, w3, to_address, value, input_data, gas, action_name):
         """
         组装完整tx并发送交易(不计算gas)
         """
         tx = {
             'from': Web3.to_checksum_address(self.address),
@@ -515,48 +515,41 @@
             # "maxFeePerGas": Web3.to_wei("1.000000019", "gwei"),  # 最大矿工费用
             # 'maxPriorityFeePerGas': Web3.to_wei("1", "gwei"),  # 最大优先矿工费用
             'type': 0
         }
         try:
             self.send_tx(w3, tx, to_address, action_name)
         except Exception as e:
-            print(f"【{self.index}】【{self.address}】动作【{action_name}】预估会失败，跳过！报文：{e}")
+            logger.info(f"【{self.index}】【{self.address}】动作【{action_name}】预估会失败，跳过！报文：{e}")
 
     @staticmethod
     def decode_param(input_data):
         if len(input_data) < 10:
-            print("全空调用")
+            logger.info("全空调用")
             return
-        method_id = input_data[:10]
-        remaining = input_data[10:]
+        method_id, remaining = input_data[:10], input_data[10:]
         params_hex = [remaining[i:i + 64] for i in range(0, len(remaining), 64)]
-        index = 0
-        print(f"函数方法:{method_id}")
-        for param_hex in params_hex:
-            if param_hex[:7] == '0000000' and param_hex[-7:] == "0000000":
-                print(f"参数{index},占位类型:{param_hex}")
-            elif param_hex[:7] == '0000000' and param_hex[-7:] != "0000000" and param_hex[24:28] == '0000':
-                print(f"参数{index},数字类型: 解码后:{int(param_hex, 16)},原码: {param_hex}")
-            elif param_hex[:7] == '0000000' and param_hex[-7:] != "0000000" and param_hex[24:28] != '0000':
-                print(f"参数{index},地址类型: 解码后：0x{param_hex[24:]},原码: {param_hex}")
-            elif param_hex[:7] != '0000000':
+        logger.info(f"函数方法:{method_id}")
+        for index, param_hex in enumerate(params_hex):
+            type_info, decoded_value = '', ''
+            if param_hex[:7] == '0000000':
+                if param_hex[-7:] == "0000000":
+                    type_info = '占位类型'
+                elif param_hex[24:28] == '0000':
+                    type_info, decoded_value = '数字类型', f"解码后:{int(param_hex, 16)}"
+                else:
+                    type_info, decoded_value = '地址类型', f"解码后：0x{param_hex[24:]}"
+            else:
                 try:
-                    # byteStr = bytes.fromhex(param_hex)
-                    # # decode_str = byteStr.decode('utf-8')
-                    # decode_str = byteStr.decode('gb2312')
-                    decode_str = binascii.unhexlify(param_hex).decode()
-                    # print(decode_str)
+                    decoded_value = binascii.unhexlify(param_hex).decode()
                 except Exception as e:
-                    decode_str = param_hex
-                print(f"参数{index},字符类型:解码后:{decode_str},原码: {param_hex}")
-            else:
-                print(f"空类型参！{param_hex}")
-            index = index + 1
-
-        print(f"{'==' * 50}")
+                    decoded_value = param_hex
+                type_info, decoded_value = '字符类型', f"解码后:{decoded_value}"
+            logger.info(f"参数{str(index).ljust(2)}, {type_info}: {decoded_value}, 原码: {param_hex}")
+        logger.info('=' * 100)
 
     @staticmethod
     def extract_parameters(input_data):
         def decode_param_value(param_value):
             # 如果参数值长度超过 40 位，则认为是 uint256
             if '0' * 40 in param_value:
                 return int(param_value, 16)
@@ -585,16 +578,16 @@
             param_value = params_data[:param_length]
             decoded_value = decode_param_value(param_value)
             params.append(decoded_value)
 
             # 剩余参数
             params_data = params_data[param_length:]
 
-        print("函数选择器：", function_selector)
-        print("参数值列表：", params)
+        logger.info("函数选择器：", function_selector)
+        logger.info("参数值列表：", params)
         return function_selector, params
 
     @staticmethod
     def log(log_name, info):
         # 获取调用方的文件路径
         caller_file = inspect.stack()[-1].filename
         # 构建 logs 目录的完整路径
@@ -605,25 +598,25 @@
             f.write(f'{info}')
             f.close()
     @staticmethod
     def create_with_mnemonic():
         """创建一个钱包带私钥和助记词"""
         Account.enable_unaudited_hdwallet_features()
         acct, mnemonic = Account.create_with_mnemonic()
-        # print(acct.address)
+        # logger.info(acct.address)
         acct1 = Account.from_mnemonic(mnemonic)
-        # print(acct1.address, Web3.toHex(acct1.key), mnemonic)
+        # logger.info(acct1.address, Web3.toHex(acct1.key), mnemonic)
         return acct1.address, Web3.to_hex(acct1.key), mnemonic
 
     @staticmethod
     def generate_wallet(num, filename='生成的ETH钱包.txt'):
         for i in range(num):
             addr,key,mn = QGEth.create_with_mnemonic()
             log = f'{addr}----{key}----{mn}'
-            print(log)
+            logger.info(log)
             QGFile.save_to_file(f'{filename}', log)
 
     def random_str(self, length):
         """指定长度的随机字符"""
         str = "abcdefghijklmnopqrstuvwxyz"
         return "".join(random.choice(str) for i in range(length))
 
@@ -636,14 +629,14 @@
     QGEth.decode_param(p1)
     QGEth.decode_param(p2)
     QGEth.decode_param(p3)
     QGEth.decode_param(p4)
     import json
     # time1 = (datetime.utcnow() + timedelta(hours=8, minutes=5)).timestamp()
     # timestamp = hex(int(time1))[2:].rjust(64, '0')
-    # print(time1,timestamp)
+    # logger.info(time1,timestamp)
     # hex_string = "0x53f4fd5c293f9def2d949ad6b282ad348967195adc0c7c23e3fdf11c193f57e0"
     #
     # # 去掉前缀 "0x" 后再处理
     # clean_hex_string = hex_string[2:] if hex_string.startswith("0x") else hex_string
     # result_string = bytes.fromhex(clean_hex_string).decode('utf-8', 'ignore')
-    # print(result_string)
+    # logger.info(result_string)
```

### Comparing `qg_toolkit-1.0.12/qg_toolkit/tools/qg_file.py` & `qg_toolkit-1.0.13/qg_toolkit/tools/qg_file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/tools/qg_random.py` & `qg_toolkit-1.0.13/qg_toolkit/tools/qg_random.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/tools/qg_solana.py` & `qg_toolkit-1.0.13/qg_toolkit/tools/qg_solana.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/tools/qg_starknet.py` & `qg_toolkit-1.0.13/qg_toolkit/tools/qg_starknet.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/tools/qproxy.py` & `qg_toolkit-1.0.13/qg_toolkit/tools/qproxy.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/qg_toolkit/tools/rpc.py` & `qg_toolkit-1.0.13/qg_toolkit/tools/rpc.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.12/PKG-INFO` & `qg_toolkit-1.0.13/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: qg_toolkit
-Version: 1.0.12
+Version: 1.0.13
 Summary: qg_toolkit for Python!
 Author: qg
 Author-email: qg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ImageHash (>=4.3.1,<5.0.0)
 Requires-Dist: PySocks (>=1.7.1,<2.0.0)
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: aiohttp (>=3.9,<4.0)
 Requires-Dist: beautifulsoup4 (>=4,<5)
+Requires-Dist: capsolver (==1.0.7)
 Requires-Dist: curl_cffi (==0.6.2)
 Requires-Dist: loguru (>=0.7,<0.8)
 Requires-Dist: lxml (>=5,<6)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: playwright (==1.43.0)
 Requires-Dist: pycryptodome (>=3.20.0,<4.0.0)
 Requires-Dist: pydantic (>=2,<3)
```

