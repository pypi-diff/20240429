# Comparing `tmp/qg_toolkit-1.0.13.tar.gz` & `tmp/qg_toolkit-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qg_toolkit-1.0.13.tar", max compression
+gzip compressed data, was "qg_toolkit-1.0.14.tar", max compression
```

## Comparing `qg_toolkit-1.0.13.tar` & `qg_toolkit-1.0.14.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0      835 2024-04-29 10:08:21.902960 qg_toolkit-1.0.13/pyproject.toml
--rw-r--r--   0        0        0       94 2024-04-28 01:55:09.875818 qg_toolkit-1.0.13/qg_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 01:55:09.876818 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/__init__.py
--rw-r--r--   0        0        0       94 2024-04-28 01:55:09.876818 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_fullpage/__init__.py
--rw-r--r--   0        0        0     5190 2024-04-28 01:55:09.877828 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py
--rw-r--r--   0        0        0     5433 2024-04-28 01:55:09.877828 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js
--rw-r--r--   0        0        0     2288 2024-04-28 01:55:09.877828 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py
--rw-r--r--   0        0        0       94 2024-04-28 01:55:09.878819 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/__init__.py
--rw-r--r--   0        0        0     2723 2024-04-28 01:55:09.878819 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/gap.py
--rw-r--r--   0        0        0    35544 2024-04-28 01:55:09.879819 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py
--rw-r--r--   0        0        0    51280 2024-04-28 01:55:09.880829 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png
--rw-r--r--   0        0        0     4818 2024-04-28 01:55:09.880829 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png
--rw-r--r--   0        0        0     9121 2024-04-28 01:55:09.881818 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png
--rw-r--r--   0        0        0  1793853 2024-04-28 01:55:09.890818 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json
--rw-r--r--   0        0        0     2362 2024-04-28 01:55:09.890818 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js
--rw-r--r--   0        0        0     2349 2024-04-28 01:55:09.891818 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/mian.py
--rw-r--r--   0        0        0     1043 2024-04-28 01:55:09.891818 qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/trace.py
--rw-r--r--   0        0        0   101354 2024-04-29 10:07:07.022169 qg_toolkit-1.0.13/qg_toolkit/qgalxe/galxe.py
--rw-r--r--   0        0        0     2750 2024-04-29 09:53:39.862145 qg_toolkit-1.0.13/qg_toolkit/qgalxe/GeetestFullPageV4.py
--rw-r--r--   0        0        0       96 2024-04-28 01:55:09.892818 qg_toolkit-1.0.13/qg_toolkit/qtweepy/__init__.py
--rw-r--r--   0        0        0      103 2024-04-28 01:55:09.892818 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/__init__.py
--rw-r--r--   0        0        0     4912 2024-04-28 06:26:10.954966 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/account_checker.py
--rw-r--r--   0        0        0     2251 2024-04-28 01:55:09.893817 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/follow_each_other.py
--rw-r--r--   0        0        0        0 2024-04-28 06:38:00.187702 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/input-output/BAD_TOKEN.txt
--rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/input-output/CONSENT_LOCKED.txt
--rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/input-output/GOOD.txt
--rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/input-output/LOCKED.txt
--rw-r--r--   0        0        0       44 2024-04-28 06:37:01.438691 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/input-output/PROXIES.txt
--rw-r--r--   0        0        0        0 2024-04-28 06:38:00.187702 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/input-output/SUSPENDED.txt
--rw-r--r--   0        0        0       40 2024-04-28 06:38:00.187702 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/input-output/UNKNOWN.txt
--rw-r--r--   0        0        0     3622 2024-04-28 01:55:09.894817 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/mavia.py
--rw-r--r--   0        0        0     2373 2024-04-28 01:55:09.895818 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/set_2fa.py
--rw-r--r--   0        0        0     3081 2024-04-28 01:55:09.895818 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py
--rw-r--r--   0        0        0      697 2024-04-28 01:55:09.895818 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/uploading_images.py
--rw-r--r--   0        0        0     2253 2024-04-28 01:55:09.896820 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/voter.py
--rw-r--r--   0        0        0     3120 2024-04-28 01:55:09.896820 qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/xai.py
--rw-r--r--   0        0        0      687 2024-04-28 01:55:09.896820 qg_toolkit-1.0.13/qg_toolkit/qtweepy/pyproject.toml
--rw-r--r--   0        0        0     8720 2024-04-28 01:55:09.892818 qg_toolkit-1.0.13/qg_toolkit/qtweepy/README.md
--rw-r--r--   0        0        0      132 2024-04-28 01:55:09.897831 qg_toolkit-1.0.13/qg_toolkit/qtweepy/tea.yaml
--rw-r--r--   0        0        0      732 2024-04-28 01:55:09.897831 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 01:55:09.897831 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 01:55:09.897831 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/__init__.py
--rw-r--r--   0        0        0     8883 2024-04-28 01:55:09.898831 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py
--rw-r--r--   0        0        0     1054 2024-04-28 01:55:09.898831 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py
--rw-r--r--   0        0        0     1741 2024-04-28 01:55:09.899826 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py
--rw-r--r--   0        0        0     2602 2024-04-28 01:55:09.899826 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py
--rw-r--r--   0        0        0    10974 2024-04-28 01:55:09.900819 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py
--rw-r--r--   0        0        0     3248 2024-04-28 01:55:09.900819 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/account.py
--rw-r--r--   0        0        0      141 2024-04-28 01:55:09.900819 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/base/__init__.py
--rw-r--r--   0        0        0      500 2024-04-28 01:55:09.901826 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/base/client.py
--rw-r--r--   0        0        0     2175 2024-04-28 01:55:09.901826 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/base/session.py
--rw-r--r--   0        0        0    70738 2024-04-28 01:55:09.902820 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/client.py
--rw-r--r--   0        0        0      267 2024-04-28 01:55:09.902820 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/enums.py
--rw-r--r--   0        0        0     5322 2024-04-28 01:55:09.903823 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/errors.py
--rw-r--r--   0        0        0     4695 2024-04-28 01:55:09.903823 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/models.py
--rw-r--r--   0        0        0      665 2024-04-28 01:55:09.903823 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/__init__.py
--rw-r--r--   0        0        0     1152 2024-04-28 01:55:09.904830 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/file.py
--rw-r--r--   0        0        0     2140 2024-04-28 01:55:09.904830 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/html.py
--rw-r--r--   0        0        0     1061 2024-04-28 01:55:09.904830 qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/other.py
--rw-r--r--   0        0        0      279 2024-04-28 01:55:09.905829 qg_toolkit-1.0.13/qg_toolkit/test/demo.yaml
--rw-r--r--   0        0        0        0 2024-04-28 01:55:09.905829 qg_toolkit-1.0.13/qg_toolkit/test/test.py
--rw-r--r--   0        0        0       96 2024-04-28 01:55:09.905829 qg_toolkit-1.0.13/qg_toolkit/tools/__init__.py
--rw-r--r--   0        0        0     5264 2024-04-29 10:04:50.990411 qg_toolkit-1.0.13/qg_toolkit/tools/cui_qiu_client.py
--rw-r--r--   0        0        0     1245 2024-04-29 09:52:12.132611 qg_toolkit-1.0.13/qg_toolkit/tools/date_util.py
--rw-r--r--   0        0        0    12289 2024-04-29 09:59:28.288628 qg_toolkit-1.0.13/qg_toolkit/tools/discord.py
--rw-r--r--   0        0        0     5905 2024-04-29 06:52:45.801970 qg_toolkit-1.0.13/qg_toolkit/tools/qg_airdrop.py
--rw-r--r--   0        0        0      985 2024-04-28 01:55:09.906829 qg_toolkit-1.0.13/qg_toolkit/tools/qg_crypto.py
--rw-r--r--   0        0        0    36155 2024-04-29 07:53:05.424108 qg_toolkit-1.0.13/qg_toolkit/tools/qg_eth.py
--rw-r--r--   0        0        0     3594 2024-04-28 01:55:09.907829 qg_toolkit-1.0.13/qg_toolkit/tools/qg_file.py
--rw-r--r--   0        0        0      300 2024-04-28 01:55:09.908828 qg_toolkit-1.0.13/qg_toolkit/tools/qg_models.py
--rw-r--r--   0        0        0      741 2024-04-28 01:55:09.908828 qg_toolkit-1.0.13/qg_toolkit/tools/qg_random.py
--rw-r--r--   0        0        0     6168 2024-04-29 06:52:45.802969 qg_toolkit-1.0.13/qg_toolkit/tools/qg_solana.py
--rw-r--r--   0        0        0     2764 2024-04-28 01:55:09.908828 qg_toolkit-1.0.13/qg_toolkit/tools/qg_starknet.py
--rw-r--r--   0        0        0     3241 2024-04-28 01:55:09.909829 qg_toolkit-1.0.13/qg_toolkit/tools/qproxy.py
--rw-r--r--   0        0        0     1239 2024-04-29 10:01:18.869266 qg_toolkit-1.0.13/qg_toolkit/tools/random_tool.py
--rw-r--r--   0        0        0     6068 2024-04-28 01:55:09.909829 qg_toolkit-1.0.13/qg_toolkit/tools/rpc.py
--rw-r--r--   0        0        0    72044 2024-04-29 09:56:23.770716 qg_toolkit-1.0.13/qg_toolkit/tools/twitter.py
--rw-r--r--   0        0        0     4085 2024-02-09 00:42:50.310936 qg_toolkit-1.0.13/qg_toolkit/tools/yescaptcha.py
--rw-r--r--   0        0        0       38 2024-04-22 02:07:22.831782 qg_toolkit-1.0.13/README.md
--rw-r--r--   0        0        0      133 2024-04-29 10:08:30.493855 qg_toolkit-1.0.13/tea.yaml
--rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 qg_toolkit-1.0.13/PKG-INFO
+-rw-r--r--   0        0        0      856 2024-04-29 10:16:44.900633 qg_toolkit-1.0.14/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-28 01:55:09.875818 qg_toolkit-1.0.14/qg_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 01:55:09.876818 qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-28 01:55:09.876818 qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_fullpage/__init__.py
+-rw-r--r--   0        0        0     5190 2024-04-28 01:55:09.877828 qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py
+-rw-r--r--   0        0        0     5433 2024-04-28 01:55:09.877828 qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js
+-rw-r--r--   0        0        0     2288 2024-04-28 01:55:09.877828 qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py
+-rw-r--r--   0        0        0       94 2024-04-28 01:55:09.878819 qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/__init__.py
+-rw-r--r--   0        0        0     2723 2024-04-28 01:55:09.878819 qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/gap.py
+-rw-r--r--   0        0        0    35544 2024-04-28 01:55:09.879819 qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py
+-rw-r--r--   0        0        0    51280 2024-04-28 01:55:09.880829 qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png
+-rw-r--r--   0        0        0     4818 2024-04-28 01:55:09.880829 qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png
+-rw-r--r--   0        0        0     9121 2024-04-28 01:55:09.881818 qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png
+-rw-r--r--   0        0        0  1793853 2024-04-28 01:55:09.890818 qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json
+-rw-r--r--   0        0        0     2362 2024-04-28 01:55:09.890818 qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js
+-rw-r--r--   0        0        0     2349 2024-04-28 01:55:09.891818 qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/mian.py
+-rw-r--r--   0        0        0     1043 2024-04-28 01:55:09.891818 qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/trace.py
+-rw-r--r--   0        0        0   101354 2024-04-29 10:07:07.022169 qg_toolkit-1.0.14/qg_toolkit/qgalxe/galxe.py
+-rw-r--r--   0        0        0     2750 2024-04-29 09:53:39.862145 qg_toolkit-1.0.14/qg_toolkit/qgalxe/GeetestFullPageV4.py
+-rw-r--r--   0        0        0       96 2024-04-28 01:55:09.892818 qg_toolkit-1.0.14/qg_toolkit/qtweepy/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-28 01:55:09.892818 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/__init__.py
+-rw-r--r--   0        0        0     4912 2024-04-28 06:26:10.954966 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/account_checker.py
+-rw-r--r--   0        0        0     2251 2024-04-28 01:55:09.893817 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/follow_each_other.py
+-rw-r--r--   0        0        0        0 2024-04-28 06:38:00.187702 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/input-output/BAD_TOKEN.txt
+-rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/input-output/CONSENT_LOCKED.txt
+-rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/input-output/GOOD.txt
+-rw-r--r--   0        0        0        0 2024-04-28 06:38:00.188701 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/input-output/LOCKED.txt
+-rw-r--r--   0        0        0       44 2024-04-28 06:37:01.438691 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/input-output/PROXIES.txt
+-rw-r--r--   0        0        0        0 2024-04-28 06:38:00.187702 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/input-output/SUSPENDED.txt
+-rw-r--r--   0        0        0       40 2024-04-28 06:38:00.187702 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/input-output/UNKNOWN.txt
+-rw-r--r--   0        0        0     3622 2024-04-28 01:55:09.894817 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/mavia.py
+-rw-r--r--   0        0        0     2373 2024-04-28 01:55:09.895818 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/set_2fa.py
+-rw-r--r--   0        0        0     3081 2024-04-28 01:55:09.895818 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py
+-rw-r--r--   0        0        0      697 2024-04-28 01:55:09.895818 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/uploading_images.py
+-rw-r--r--   0        0        0     2253 2024-04-28 01:55:09.896820 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/voter.py
+-rw-r--r--   0        0        0     3120 2024-04-28 01:55:09.896820 qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/xai.py
+-rw-r--r--   0        0        0      687 2024-04-28 01:55:09.896820 qg_toolkit-1.0.14/qg_toolkit/qtweepy/pyproject.toml
+-rw-r--r--   0        0        0     8720 2024-04-28 01:55:09.892818 qg_toolkit-1.0.14/qg_toolkit/qtweepy/README.md
+-rw-r--r--   0        0        0      132 2024-04-28 01:55:09.897831 qg_toolkit-1.0.14/qg_toolkit/qtweepy/tea.yaml
+-rw-r--r--   0        0        0      732 2024-04-28 01:55:09.897831 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 01:55:09.897831 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/_capsolver/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 01:55:09.897831 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/_capsolver/core/__init__.py
+-rw-r--r--   0        0        0     8883 2024-04-28 01:55:09.898831 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py
+-rw-r--r--   0        0        0     1054 2024-04-28 01:55:09.898831 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py
+-rw-r--r--   0        0        0     1741 2024-04-28 01:55:09.899826 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py
+-rw-r--r--   0        0        0     2602 2024-04-28 01:55:09.899826 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py
+-rw-r--r--   0        0        0    10974 2024-04-28 01:55:09.900819 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py
+-rw-r--r--   0        0        0     3248 2024-04-28 01:55:09.900819 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/account.py
+-rw-r--r--   0        0        0      141 2024-04-28 01:55:09.900819 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/base/__init__.py
+-rw-r--r--   0        0        0      500 2024-04-28 01:55:09.901826 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/base/client.py
+-rw-r--r--   0        0        0     2175 2024-04-28 01:55:09.901826 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/base/session.py
+-rw-r--r--   0        0        0    70738 2024-04-28 01:55:09.902820 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/client.py
+-rw-r--r--   0        0        0      267 2024-04-28 01:55:09.902820 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/enums.py
+-rw-r--r--   0        0        0     5322 2024-04-28 01:55:09.903823 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/errors.py
+-rw-r--r--   0        0        0     4695 2024-04-28 01:55:09.903823 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/models.py
+-rw-r--r--   0        0        0      665 2024-04-28 01:55:09.903823 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/utils/__init__.py
+-rw-r--r--   0        0        0     1152 2024-04-28 01:55:09.904830 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/utils/file.py
+-rw-r--r--   0        0        0     2140 2024-04-28 01:55:09.904830 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/utils/html.py
+-rw-r--r--   0        0        0     1061 2024-04-28 01:55:09.904830 qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/utils/other.py
+-rw-r--r--   0        0        0      279 2024-04-28 01:55:09.905829 qg_toolkit-1.0.14/qg_toolkit/test/demo.yaml
+-rw-r--r--   0        0        0        0 2024-04-28 01:55:09.905829 qg_toolkit-1.0.14/qg_toolkit/test/test.py
+-rw-r--r--   0        0        0       96 2024-04-28 01:55:09.905829 qg_toolkit-1.0.14/qg_toolkit/tools/__init__.py
+-rw-r--r--   0        0        0     5264 2024-04-29 10:04:50.990411 qg_toolkit-1.0.14/qg_toolkit/tools/cui_qiu_client.py
+-rw-r--r--   0        0        0     1245 2024-04-29 09:52:12.132611 qg_toolkit-1.0.14/qg_toolkit/tools/date_util.py
+-rw-r--r--   0        0        0    12289 2024-04-29 09:59:28.288628 qg_toolkit-1.0.14/qg_toolkit/tools/discord.py
+-rw-r--r--   0        0        0     5905 2024-04-29 06:52:45.801970 qg_toolkit-1.0.14/qg_toolkit/tools/qg_airdrop.py
+-rw-r--r--   0        0        0      985 2024-04-28 01:55:09.906829 qg_toolkit-1.0.14/qg_toolkit/tools/qg_crypto.py
+-rw-r--r--   0        0        0    36155 2024-04-29 07:53:05.424108 qg_toolkit-1.0.14/qg_toolkit/tools/qg_eth.py
+-rw-r--r--   0        0        0     3594 2024-04-28 01:55:09.907829 qg_toolkit-1.0.14/qg_toolkit/tools/qg_file.py
+-rw-r--r--   0        0        0      300 2024-04-28 01:55:09.908828 qg_toolkit-1.0.14/qg_toolkit/tools/qg_models.py
+-rw-r--r--   0        0        0      741 2024-04-28 01:55:09.908828 qg_toolkit-1.0.14/qg_toolkit/tools/qg_random.py
+-rw-r--r--   0        0        0     6168 2024-04-29 06:52:45.802969 qg_toolkit-1.0.14/qg_toolkit/tools/qg_solana.py
+-rw-r--r--   0        0        0     2764 2024-04-28 01:55:09.908828 qg_toolkit-1.0.14/qg_toolkit/tools/qg_starknet.py
+-rw-r--r--   0        0        0     3241 2024-04-28 01:55:09.909829 qg_toolkit-1.0.14/qg_toolkit/tools/qproxy.py
+-rw-r--r--   0        0        0     1239 2024-04-29 10:01:18.869266 qg_toolkit-1.0.14/qg_toolkit/tools/random_tool.py
+-rw-r--r--   0        0        0     6068 2024-04-28 01:55:09.909829 qg_toolkit-1.0.14/qg_toolkit/tools/rpc.py
+-rw-r--r--   0        0        0    72044 2024-04-29 09:56:23.770716 qg_toolkit-1.0.14/qg_toolkit/tools/twitter.py
+-rw-r--r--   0        0        0     4085 2024-02-09 00:42:50.310936 qg_toolkit-1.0.14/qg_toolkit/tools/yescaptcha.py
+-rw-r--r--   0        0        0       38 2024-04-22 02:07:22.831782 qg_toolkit-1.0.14/README.md
+-rw-r--r--   0        0        0      133 2024-04-29 10:16:44.903632 qg_toolkit-1.0.14/tea.yaml
+-rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 qg_toolkit-1.0.14/PKG-INFO
```

### Comparing `qg_toolkit-1.0.13/pyproject.toml` & `qg_toolkit-1.0.14/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qg_toolkit"
-version = "1.0.13"
+version = "1.0.14"
 description = "qg_toolkit for Python!"
 authors = ["qg <qg@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qg_toolkit"}]
 include = [{path = "tea.yaml"}]
 
 
@@ -28,15 +28,17 @@
 pillow= "^10.3.0"
 ImageHash= "^4.3.1"
 PyYAML= "^6.0.1"
 PySocks= "^1.7.1"
 websockets= "11.0.3"
 web3="^6.17.2"
 playwright="1.43.0"
-capsolver="1.0.7"
+capsolver="^1.0.7"
+faker="^24.11.0"
+
 
 [tool.poetry.group.dev.dependencies]
 black = "^24"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py` & `qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js` & `qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py` & `qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/gap.py` & `qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/gap.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py` & `qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png` & `qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png` & `qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png` & `qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json` & `qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js` & `qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/mian.py` & `qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/mian.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/geetest_captcha/geetest4_slide/trace.py` & `qg_toolkit-1.0.14/qg_toolkit/geetest_captcha/geetest4_slide/trace.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qgalxe/galxe.py` & `qg_toolkit-1.0.14/qg_toolkit/qgalxe/galxe.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qgalxe/GeetestFullPageV4.py` & `qg_toolkit-1.0.14/qg_toolkit/qgalxe/GeetestFullPageV4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/account_checker.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/account_checker.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/follow_each_other.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/follow_each_other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/mavia.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/mavia.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/set_2fa.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/set_2fa.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/uploading_images.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/uploading_images.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/voter.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/voter.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/examples/xai.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/examples/xai.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/pyproject.toml` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/README.md` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/README.md`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/__init__.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/account.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/account.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/base/session.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/base/session.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/client.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/client.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/errors.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/errors.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/models.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/models.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/__init__.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/file.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/utils/file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/html.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/utils/html.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/qtweepy/twitter/utils/other.py` & `qg_toolkit-1.0.14/qg_toolkit/qtweepy/twitter/utils/other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/tools/cui_qiu_client.py` & `qg_toolkit-1.0.14/qg_toolkit/tools/cui_qiu_client.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/tools/date_util.py` & `qg_toolkit-1.0.14/qg_toolkit/tools/date_util.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/tools/discord.py` & `qg_toolkit-1.0.14/qg_toolkit/tools/discord.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/tools/qg_airdrop.py` & `qg_toolkit-1.0.14/qg_toolkit/tools/qg_airdrop.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/tools/qg_crypto.py` & `qg_toolkit-1.0.14/qg_toolkit/tools/qg_crypto.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/tools/qg_eth.py` & `qg_toolkit-1.0.14/qg_toolkit/tools/qg_eth.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/tools/qg_file.py` & `qg_toolkit-1.0.14/qg_toolkit/tools/qg_file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/tools/qg_random.py` & `qg_toolkit-1.0.14/qg_toolkit/tools/qg_random.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/tools/qg_solana.py` & `qg_toolkit-1.0.14/qg_toolkit/tools/qg_solana.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/tools/qg_starknet.py` & `qg_toolkit-1.0.14/qg_toolkit/tools/qg_starknet.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/tools/qproxy.py` & `qg_toolkit-1.0.14/qg_toolkit/tools/qproxy.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/tools/random_tool.py` & `qg_toolkit-1.0.14/qg_toolkit/tools/random_tool.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/tools/rpc.py` & `qg_toolkit-1.0.14/qg_toolkit/tools/rpc.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/tools/twitter.py` & `qg_toolkit-1.0.14/qg_toolkit/tools/twitter.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/qg_toolkit/tools/yescaptcha.py` & `qg_toolkit-1.0.14/qg_toolkit/tools/yescaptcha.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.13/PKG-INFO` & `qg_toolkit-1.0.14/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: qg_toolkit
-Version: 1.0.13
+Version: 1.0.14
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
-Requires-Dist: capsolver (==1.0.7)
+Requires-Dist: capsolver (>=1.0.7,<2.0.0)
 Requires-Dist: curl_cffi (==0.6.2)
+Requires-Dist: faker (>=24.11.0,<25.0.0)
 Requires-Dist: loguru (>=0.7,<0.8)
 Requires-Dist: lxml (>=5,<6)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: playwright (==1.43.0)
 Requires-Dist: pycryptodome (>=3.20.0,<4.0.0)
 Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: pyotp (>=2,<3)
```

