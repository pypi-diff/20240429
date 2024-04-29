# Comparing `tmp/qg_toolkit-1.0.8.tar.gz` & `tmp/qg_toolkit-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qg_toolkit-1.0.8.tar", max compression
+gzip compressed data, was "qg_toolkit-1.0.9.tar", max compression
```

## Comparing `qg_toolkit-1.0.8.tar` & `qg_toolkit-1.0.9.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0      794 2024-04-27 12:36:37.386302 qg_toolkit-1.0.8/pyproject.toml
--rw-r--r--   0        0        0       94 2024-04-27 10:53:56.731750 qg_toolkit-1.0.8/qg_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 18:53:34.039466 qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/__init__.py
--rw-r--r--   0        0        0       94 2024-04-27 10:54:32.432326 qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_fullpage/__init__.py
--rw-r--r--   0        0        0     5190 2024-04-24 18:53:34.040467 qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py
--rw-r--r--   0        0        0     5433 2024-04-24 18:53:34.040467 qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js
--rw-r--r--   0        0        0     2288 2024-04-27 11:00:05.704720 qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py
--rw-r--r--   0        0        0       94 2024-04-27 10:54:37.081886 qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/__init__.py
--rw-r--r--   0        0        0     2723 2024-04-24 18:53:34.042468 qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/gap.py
--rw-r--r--   0        0        0    35544 2024-04-26 20:18:37.986103 qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py
--rw-r--r--   0        0        0    51280 2024-04-24 18:53:34.044476 qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png
--rw-r--r--   0        0        0     4818 2024-04-24 18:53:34.045475 qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png
--rw-r--r--   0        0        0     9121 2024-04-24 18:53:34.045475 qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png
--rw-r--r--   0        0        0  1793853 2024-04-24 18:53:34.058465 qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json
--rw-r--r--   0        0        0     2362 2024-04-24 18:53:34.059468 qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js
--rw-r--r--   0        0        0     2349 2024-04-27 11:14:05.254088 qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/mian.py
--rw-r--r--   0        0        0     1043 2024-04-24 18:53:34.060469 qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/trace.py
--rw-r--r--   0        0        0       96 2024-04-27 10:54:21.799092 qg_toolkit-1.0.8/qg_toolkit/qtweepy/__init__.py
--rw-r--r--   0        0        0      103 2024-04-27 10:52:23.199431 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/__init__.py
--rw-r--r--   0        0        0     4880 2024-04-27 10:52:23.276729 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/account_checker.py
--rw-r--r--   0        0        0     2251 2024-04-27 10:52:23.208431 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/follow_each_other.py
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.415935 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/input-output/BAD_TOKEN.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/input-output/CONSENT_LOCKED.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/input-output/GOOD.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/input-output/LOCKED.txt
--rw-r--r--   0        0        0       46 2024-04-27 05:31:06.618786 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/input-output/PROXIES.txt
--rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/input-output/SUSPENDED.txt
--rw-r--r--   0        0        0       40 2024-04-27 05:31:12.415935 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/input-output/UNKNOWN.txt
--rw-r--r--   0        0        0     3622 2024-04-27 10:52:23.284728 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/mavia.py
--rw-r--r--   0        0        0     2373 2024-04-27 10:52:23.217431 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/set_2fa.py
--rw-r--r--   0        0        0     3081 2024-04-27 10:52:23.184432 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py
--rw-r--r--   0        0        0      697 2024-04-27 10:52:23.174431 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/uploading_images.py
--rw-r--r--   0        0        0     2253 2024-04-27 10:52:23.159432 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/voter.py
--rw-r--r--   0        0        0     3120 2024-04-27 10:52:23.191432 qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/xai.py
--rw-r--r--   0        0        0      687 2024-04-20 19:57:03.446998 qg_toolkit-1.0.8/qg_toolkit/qtweepy/pyproject.toml
--rw-r--r--   0        0        0     8720 2024-04-20 19:48:15.063903 qg_toolkit-1.0.8/qg_toolkit/qtweepy/README.md
--rw-r--r--   0        0        0      132 2024-04-24 18:22:26.184000 qg_toolkit-1.0.8/qg_toolkit/qtweepy/tea.yaml
--rw-r--r--   0        0        0      732 2024-04-20 19:48:15.068902 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/_capsolver/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/_capsolver/core/__init__.py
--rw-r--r--   0        0        0     8883 2024-04-20 19:48:15.070903 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py
--rw-r--r--   0        0        0     1054 2024-04-20 19:48:15.070903 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py
--rw-r--r--   0        0        0     1741 2024-04-20 19:48:15.071903 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py
--rw-r--r--   0        0        0     2602 2024-04-20 19:48:15.071903 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py
--rw-r--r--   0        0        0    10974 2024-04-20 19:48:15.072903 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py
--rw-r--r--   0        0        0     3248 2024-04-20 19:48:15.072903 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/account.py
--rw-r--r--   0        0        0      141 2024-04-20 19:48:15.072903 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/base/__init__.py
--rw-r--r--   0        0        0      500 2024-04-20 19:48:15.074292 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/base/client.py
--rw-r--r--   0        0        0     2175 2024-04-27 10:52:23.255728 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/base/session.py
--rw-r--r--   0        0        0    70738 2024-04-20 19:48:15.075686 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/client.py
--rw-r--r--   0        0        0      267 2024-04-20 19:48:15.076283 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/enums.py
--rw-r--r--   0        0        0     5322 2024-04-20 19:48:15.076811 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/errors.py
--rw-r--r--   0        0        0     4695 2024-04-20 19:48:15.076811 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/models.py
--rw-r--r--   0        0        0      665 2024-04-20 19:48:15.077920 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/utils/__init__.py
--rw-r--r--   0        0        0     1152 2024-04-20 19:48:15.077920 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/utils/file.py
--rw-r--r--   0        0        0     2140 2024-04-20 19:48:15.078463 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/utils/html.py
--rw-r--r--   0        0        0     1061 2024-04-20 19:48:15.078992 qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/utils/other.py
--rw-r--r--   0        0        0        0 2024-04-27 11:06:09.049630 qg_toolkit-1.0.8/qg_toolkit/test/test.py
--rw-r--r--   0        0        0       96 2024-04-27 10:54:04.685704 qg_toolkit-1.0.8/qg_toolkit/tools/__init__.py
--rw-r--r--   0        0        0      279 2024-04-24 18:54:00.529601 qg_toolkit-1.0.8/qg_toolkit/tools/demo.yaml
--rw-r--r--   0        0        0     5454 2024-04-27 10:53:33.237906 qg_toolkit-1.0.8/qg_toolkit/tools/qg_airdrop.py
--rw-r--r--   0        0        0      985 2024-04-20 20:27:34.147592 qg_toolkit-1.0.8/qg_toolkit/tools/qg_crypto.py
--rw-r--r--   0        0        0    35579 2024-04-27 12:36:08.773113 qg_toolkit-1.0.8/qg_toolkit/tools/qg_eth.py
--rw-r--r--   0        0        0     3594 2024-04-20 20:29:00.648873 qg_toolkit-1.0.8/qg_toolkit/tools/qg_file.py
--rw-r--r--   0        0        0      300 2024-04-24 18:53:34.062471 qg_toolkit-1.0.8/qg_toolkit/tools/qg_models.py
--rw-r--r--   0        0        0      741 2024-04-20 20:24:22.248041 qg_toolkit-1.0.8/qg_toolkit/tools/qg_random.py
--rw-r--r--   0        0        0     6135 2024-04-27 11:03:13.085956 qg_toolkit-1.0.8/qg_toolkit/tools/qg_solana.py
--rw-r--r--   0        0        0     2764 2024-04-24 18:21:31.477405 qg_toolkit-1.0.8/qg_toolkit/tools/qg_starknet.py
--rw-r--r--   0        0        0     3241 2024-04-20 19:48:15.080086 qg_toolkit-1.0.8/qg_toolkit/tools/qproxy.py
--rw-r--r--   0        0        0     6050 2024-04-20 21:14:04.319021 qg_toolkit-1.0.8/qg_toolkit/tools/rpc.py
--rw-r--r--   0        0        0       38 2024-04-20 19:50:56.436133 qg_toolkit-1.0.8/README.md
--rw-r--r--   0        0        0      132 2024-04-27 12:36:37.381304 qg_toolkit-1.0.8/tea.yaml
--rw-r--r--   0        0        0     1249 1970-01-01 00:00:00.000000 qg_toolkit-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      794 2024-04-29 05:12:31.684232 qg_toolkit-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-27 10:53:56.731750 qg_toolkit-1.0.9/qg_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 18:53:34.039466 qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-27 10:54:32.432326 qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_fullpage/__init__.py
+-rw-r--r--   0        0        0     5190 2024-04-24 18:53:34.040467 qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py
+-rw-r--r--   0        0        0     5433 2024-04-24 18:53:34.040467 qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js
+-rw-r--r--   0        0        0     2288 2024-04-27 11:00:05.704720 qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py
+-rw-r--r--   0        0        0       94 2024-04-27 10:54:37.081886 qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/__init__.py
+-rw-r--r--   0        0        0     2723 2024-04-24 18:53:34.042468 qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/gap.py
+-rw-r--r--   0        0        0    35544 2024-04-26 20:18:37.986103 qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py
+-rw-r--r--   0        0        0    51280 2024-04-24 18:53:34.044476 qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png
+-rw-r--r--   0        0        0     4818 2024-04-24 18:53:34.045475 qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png
+-rw-r--r--   0        0        0     9121 2024-04-24 18:53:34.045475 qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png
+-rw-r--r--   0        0        0  1793853 2024-04-24 18:53:34.058465 qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json
+-rw-r--r--   0        0        0     2362 2024-04-24 18:53:34.059468 qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js
+-rw-r--r--   0        0        0     2349 2024-04-27 11:14:05.254088 qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/mian.py
+-rw-r--r--   0        0        0     1043 2024-04-24 18:53:34.060469 qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/trace.py
+-rw-r--r--   0        0        0       96 2024-04-27 10:54:21.799092 qg_toolkit-1.0.9/qg_toolkit/qtweepy/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-27 10:52:23.199431 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/__init__.py
+-rw-r--r--   0        0        0     4880 2024-04-27 10:52:23.276729 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/account_checker.py
+-rw-r--r--   0        0        0     2251 2024-04-27 10:52:23.208431 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/follow_each_other.py
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.415935 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/input-output/BAD_TOKEN.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/input-output/CONSENT_LOCKED.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/input-output/GOOD.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/input-output/LOCKED.txt
+-rw-r--r--   0        0        0       46 2024-04-27 05:31:06.618786 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/input-output/PROXIES.txt
+-rw-r--r--   0        0        0        0 2024-04-27 05:31:12.416935 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/input-output/SUSPENDED.txt
+-rw-r--r--   0        0        0       40 2024-04-27 05:31:12.415935 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/input-output/UNKNOWN.txt
+-rw-r--r--   0        0        0     3622 2024-04-27 10:52:23.284728 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/mavia.py
+-rw-r--r--   0        0        0     2373 2024-04-27 10:52:23.217431 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/set_2fa.py
+-rw-r--r--   0        0        0     3081 2024-04-27 10:52:23.184432 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py
+-rw-r--r--   0        0        0      697 2024-04-27 10:52:23.174431 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/uploading_images.py
+-rw-r--r--   0        0        0     2253 2024-04-27 10:52:23.159432 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/voter.py
+-rw-r--r--   0        0        0     3120 2024-04-27 10:52:23.191432 qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/xai.py
+-rw-r--r--   0        0        0      687 2024-04-20 19:57:03.446998 qg_toolkit-1.0.9/qg_toolkit/qtweepy/pyproject.toml
+-rw-r--r--   0        0        0     8720 2024-04-20 19:48:15.063903 qg_toolkit-1.0.9/qg_toolkit/qtweepy/README.md
+-rw-r--r--   0        0        0      132 2024-04-24 18:22:26.184000 qg_toolkit-1.0.9/qg_toolkit/qtweepy/tea.yaml
+-rw-r--r--   0        0        0      732 2024-04-20 19:48:15.068902 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/_capsolver/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 19:48:15.069903 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/_capsolver/core/__init__.py
+-rw-r--r--   0        0        0     8883 2024-04-20 19:48:15.070903 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py
+-rw-r--r--   0        0        0     1054 2024-04-20 19:48:15.070903 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py
+-rw-r--r--   0        0        0     1741 2024-04-20 19:48:15.071903 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py
+-rw-r--r--   0        0        0     2602 2024-04-20 19:48:15.071903 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py
+-rw-r--r--   0        0        0    10974 2024-04-20 19:48:15.072903 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py
+-rw-r--r--   0        0        0     3248 2024-04-20 19:48:15.072903 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/account.py
+-rw-r--r--   0        0        0      141 2024-04-20 19:48:15.072903 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/base/__init__.py
+-rw-r--r--   0        0        0      500 2024-04-20 19:48:15.074292 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/base/client.py
+-rw-r--r--   0        0        0     2175 2024-04-27 10:52:23.255728 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/base/session.py
+-rw-r--r--   0        0        0    70738 2024-04-20 19:48:15.075686 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/client.py
+-rw-r--r--   0        0        0      267 2024-04-20 19:48:15.076283 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/enums.py
+-rw-r--r--   0        0        0     5322 2024-04-20 19:48:15.076811 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/errors.py
+-rw-r--r--   0        0        0     4695 2024-04-20 19:48:15.076811 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/models.py
+-rw-r--r--   0        0        0      665 2024-04-20 19:48:15.077920 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/utils/__init__.py
+-rw-r--r--   0        0        0     1152 2024-04-20 19:48:15.077920 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/utils/file.py
+-rw-r--r--   0        0        0     2140 2024-04-20 19:48:15.078463 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/utils/html.py
+-rw-r--r--   0        0        0     1061 2024-04-20 19:48:15.078992 qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/utils/other.py
+-rw-r--r--   0        0        0        0 2024-04-27 11:06:09.049630 qg_toolkit-1.0.9/qg_toolkit/test/test.py
+-rw-r--r--   0        0        0       96 2024-04-27 10:54:04.685704 qg_toolkit-1.0.9/qg_toolkit/tools/__init__.py
+-rw-r--r--   0        0        0      279 2024-04-24 18:54:00.529601 qg_toolkit-1.0.9/qg_toolkit/tools/demo.yaml
+-rw-r--r--   0        0        0     5732 2024-04-29 05:10:03.481116 qg_toolkit-1.0.9/qg_toolkit/tools/qg_airdrop.py
+-rw-r--r--   0        0        0      985 2024-04-20 20:27:34.147592 qg_toolkit-1.0.9/qg_toolkit/tools/qg_crypto.py
+-rw-r--r--   0        0        0    35579 2024-04-27 12:36:08.773113 qg_toolkit-1.0.9/qg_toolkit/tools/qg_eth.py
+-rw-r--r--   0        0        0     3594 2024-04-20 20:29:00.648873 qg_toolkit-1.0.9/qg_toolkit/tools/qg_file.py
+-rw-r--r--   0        0        0      300 2024-04-24 18:53:34.062471 qg_toolkit-1.0.9/qg_toolkit/tools/qg_models.py
+-rw-r--r--   0        0        0      741 2024-04-20 20:24:22.248041 qg_toolkit-1.0.9/qg_toolkit/tools/qg_random.py
+-rw-r--r--   0        0        0     6135 2024-04-27 11:03:13.085956 qg_toolkit-1.0.9/qg_toolkit/tools/qg_solana.py
+-rw-r--r--   0        0        0     2764 2024-04-24 18:21:31.477405 qg_toolkit-1.0.9/qg_toolkit/tools/qg_starknet.py
+-rw-r--r--   0        0        0     3241 2024-04-20 19:48:15.080086 qg_toolkit-1.0.9/qg_toolkit/tools/qproxy.py
+-rw-r--r--   0        0        0     6068 2024-04-27 13:05:30.422039 qg_toolkit-1.0.9/qg_toolkit/tools/rpc.py
+-rw-r--r--   0        0        0       38 2024-04-20 19:50:56.436133 qg_toolkit-1.0.9/README.md
+-rw-r--r--   0        0        0      132 2024-04-29 05:12:36.026108 qg_toolkit-1.0.9/tea.yaml
+-rw-r--r--   0        0        0     1249 1970-01-01 00:00:00.000000 qg_toolkit-1.0.9/PKG-INFO
```

### Comparing `qg_toolkit-1.0.8/pyproject.toml` & `qg_toolkit-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qg_toolkit"
-version = "1.0.8"
+version = "1.0.9"
 description = "qg_toolkit for Python!"
 authors = ["qg <qg@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qg_toolkit"}]
 include = [{path = "tea.yaml"}]
```

### Comparing `qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py` & `qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_fullpage/geetest_v4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js` & `qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_fullpage/jiyan.js`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py` & `qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_fullpage/mian.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/gap.py` & `qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/gap.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py` & `qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/geetest_slide_v4.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png` & `qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/img/bg.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png` & `qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/img/show_image.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png` & `qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/img/slide.png`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json` & `qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/img/tracks.json`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js` & `qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/jiyan.js`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/mian.py` & `qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/mian.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/geetest_captcha/geetest4_slide/trace.py` & `qg_toolkit-1.0.9/qg_toolkit/geetest_captcha/geetest4_slide/trace.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/account_checker.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/account_checker.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/follow_each_other.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/follow_each_other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/mavia.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/mavia.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/set_2fa.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/set_2fa.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/set_avatars_and_banners.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/uploading_images.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/uploading_images.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/voter.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/voter.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/examples/xai.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/examples/xai.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/pyproject.toml` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/README.md` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/README.md`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/__init__.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/_capsolver/core/base.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/_capsolver/core/config.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/_capsolver/core/enum.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/_capsolver/core/serializer.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/_capsolver/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/account.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/account.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/base/session.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/base/session.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/client.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/client.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/errors.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/errors.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/models.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/models.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/utils/__init__.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/utils/file.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/utils/file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/utils/html.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/utils/html.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/qtweepy/twitter/utils/other.py` & `qg_toolkit-1.0.9/qg_toolkit/qtweepy/twitter/utils/other.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/tools/qg_airdrop.py` & `qg_toolkit-1.0.9/qg_toolkit/tools/qg_airdrop.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import concurrent.futures
 import copy
+import random
 from threading import Lock
 
 from web3 import Web3
 
 from qg_toolkit.tools.qg_eth import QGEth
 from qg_toolkit.tools.qg_file import QGFile
 
@@ -24,36 +25,39 @@
         self.w3 = getattr(self, f"{self.chain_name}_w3", None)
         self.w3_balance = getattr(self, f"{self.chain_name}_balance", None)
         self.fenpei()
 
     @property
     def contract_map(self):
         return {
-            "polygon": "0xDCB4a16EB4F5F8214962357c96584F6955B9b525",
-            "bsc": "0x0Ff88bdD9BE134F29dD660C4F220DD1e392e49E4",
-            "opbnb": "0x501Ab65Ec2E89aB6e9CBfE6eE3AED423995b1aef",
-            "goerli": "0x9680D1e126bBeF521F97b6FFB2fe39Da5c88C290",
-            "sepolia": "0xEf50B70800f0D5D89b7a0056A0746845C2Dbe7b7",
-            "linea": "0x2Ce164CbdBFb8fA0BEbf1f2dCD2F364481Fa86d3",
-            "mantle": "0x601074C151C229d04D339F807817e8cB87E6CF1e",
-            "berachain": "0xaB06c32FCE992B423F17e57BCC78C1cA80dd7AaA",
-            "blast": "0x8B4a4AA2fD4bB59eBBEB987D229A3eb01f987E7b",
-            "zeta": "0xBc4A4b3846C3F2F8085689F0A4A09D76627b6c2E",
-            "holesky": "0x42d5f4D80dC931644627127385F51F07eb8a485D",
-            "xter": "0x7347Ae5a53F7b80A7eF6654E3b8eA0c0E396a4D3"
+            "polygon": ["0xDCB4a16EB4F5F8214962357c96584F6955B9b525"],
+            "opbnb": ["0x501Ab65Ec2E89aB6e9CBfE6eE3AED423995b1aef"],
+            "goerli": ["0x9680D1e126bBeF521F97b6FFB2fe39Da5c88C290"],
+            "sepolia": ["0xEf50B70800f0D5D89b7a0056A0746845C2Dbe7b7"],
+            "linea": ["0x2Ce164CbdBFb8fA0BEbf1f2dCD2F364481Fa86d3"],
+            "mantle": ["0x601074C151C229d04D339F807817e8cB87E6CF1e"],
+            "berachain": ["0xaB06c32FCE992B423F17e57BCC78C1cA80dd7AaA"],
+            "blast": ["0x8B4a4AA2fD4bB59eBBEB987D229A3eb01f987E7b"],
+            "zeta": ["0xBc4A4b3846C3F2F8085689F0A4A09D76627b6c2E"],
+            "holesky": [
+                "0x42d5f4D80dC931644627127385F51F07eb8a485D","0x88B0D9b5046021313f96d4d83feF78b65bF92Ac9",
+                "0x0760EB9694606121A8cfF688C4F70F92a0BA003c","0xd6e6414e7a41816f212A308Ed1252CD473484596",
+                "0xcF8DdFBC496Ca726f9bB3489f1Fcc992E137471f","0x9324Ca1DBbE42E5176F33eAbe53a38599bA15a6B"
+            ],
+            "xter": ["0x7347Ae5a53F7b80A7eF6654E3b8eA0c0E396a4D3"]
         }
 
     def batch_send_eth_by_lian(self):
         print(f'【{self.address}】【{self.index}】接收地址数量：{len(self.receiver_accounts)}')
         if len(self.receiver_accounts) == 0:
             return
         address_arr = self.receiver_accounts
         value = self.per_value
         action_name = "batch_send_eth_by_lian"
-        to_address = self.contract_map.get(self.chain_name) or None
+        to_address = self.contract_map.get(random.choice(self.chain_name)) or None
         if to_address is None:
             return
         hex_value = hex(Web3.to_wei(value, "ether"))[2:].rjust(64, '0')
         length = len(address_arr)
         if length == 0:
             return
         length_hex = hex(length)[2:].rjust(64, '0')
@@ -91,17 +95,17 @@
             self.receiver_accounts = rs[:can_num]
             rs = rs[can_num:]
         QGAirDrop.lock.release()
         print(f'{self.address} 分配账号数量{len(self.receiver_accounts)}:{self.receiver_accounts}')
 
 
 def qg_task(index, address, private_key, mnemonic):
-    chain_name = "opbnb"
+    chain_name = "holesky"
     # 每个号空投多少
-    per_value = "0.00015"
+    per_value = "0.08"
     # 给自己号剩余多少
     left_value = 1
     # 是否检查接收者余额
     is_check_receiver = True
     # 检查接收者余额是否大于N
     check_balance = 0.0001
     batch = QGAirDrop(index=index, address=address, private_key=private_key, mnemonic=mnemonic,
```

### Comparing `qg_toolkit-1.0.8/qg_toolkit/tools/qg_crypto.py` & `qg_toolkit-1.0.9/qg_toolkit/tools/qg_crypto.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/tools/qg_eth.py` & `qg_toolkit-1.0.9/qg_toolkit/tools/qg_eth.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/tools/qg_file.py` & `qg_toolkit-1.0.9/qg_toolkit/tools/qg_file.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/tools/qg_random.py` & `qg_toolkit-1.0.9/qg_toolkit/tools/qg_random.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/tools/qg_solana.py` & `qg_toolkit-1.0.9/qg_toolkit/tools/qg_solana.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/tools/qg_starknet.py` & `qg_toolkit-1.0.9/qg_toolkit/tools/qg_starknet.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/tools/qproxy.py` & `qg_toolkit-1.0.9/qg_toolkit/tools/qproxy.py`

 * *Files identical despite different names*

### Comparing `qg_toolkit-1.0.8/qg_toolkit/tools/rpc.py` & `qg_toolkit-1.0.9/qg_toolkit/tools/rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     "zeta3": "https://zetachain-athens-evm.blockpi.network/v1/rpc/public/api",
     # "zeta3": "https://rpc.ankr.com/zetachain_evm_athens_testnet/995de8736b54e4c2b5ec62771fe384c27c9715835a9ccf0d0fd11c8eaf985095/api",
     "bsc_test": "https://api-testnet.bscscan.com/api",
     "opbnb": "https://opbnb-mainnet.nodereal.io/v1/b4876385e7ec46cd9da933f2a83d969c",
     "polygon": "https://api.polygonscan.com/api",
     "berachain": "https://api.routescan.io/v2/network/testnet/evm/80085/etherscan/api",
     "blast": "https://api.routescan.io/v2/network/testnet/evm/168587773/etherscan/api",
-    "holesky": "https://holesky.etherscan.io/api",
+    "holesky": "https://ethereum-holesky-beacon-api.publicnode.com",
     "xter": "https://xterscan.io/api"
 }
 
 apis = {
     "get_account_tx_list": "?module=account&action=txlist&address={}",
     "get_tx_info": "?module=transaction&action=gettxinfo&txhash={}"
 }
```

### Comparing `qg_toolkit-1.0.8/PKG-INFO` & `qg_toolkit-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qg_toolkit
-Version: 1.0.8
+Version: 1.0.9
 Summary: qg_toolkit for Python!
 Author: qg
 Author-email: qg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

