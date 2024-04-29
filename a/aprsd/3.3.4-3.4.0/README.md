# Comparing `tmp/aprsd-3.3.4.tar.gz` & `tmp/aprsd-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aprsd-3.3.4.tar", last modified: Sun Apr 21 16:35:29 2024, max compression
+gzip compressed data, was "aprsd-3.4.0.tar", last modified: Mon Apr 29 13:33:48 2024, max compression
```

## Comparing `aprsd-3.3.4.tar` & `aprsd-3.4.0.tar`

### file list

```diff
@@ -1,260 +1,255 @@
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.886592 aprsd-3.3.4/
--rw-r--r--   0 I530566    (501) staff       (20)      269 2021-08-30 17:18:20.000000 aprsd-3.3.4/.coveragerc
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.007507 aprsd-3.3.4/.github/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.071145 aprsd-3.3.4/.github/workflows/
--rw-r--r--   0 I530566    (501) staff       (20)     3534 2024-02-09 02:07:13.000000 aprsd-3.3.4/.github/workflows/codeql.yml
--rw-r--r--   0 I530566    (501) staff       (20)     1461 2024-02-07 13:55:16.000000 aprsd-3.3.4/.github/workflows/manual_build.yml
--rw-r--r--   0 I530566    (501) staff       (20)     1622 2024-02-07 13:54:43.000000 aprsd-3.3.4/.github/workflows/master-build.yml
--rw-r--r--   0 I530566    (501) staff       (20)      524 2023-11-17 18:02:52.000000 aprsd-3.3.4/.github/workflows/python.yml
--rw-r--r--   0 I530566    (501) staff       (20)     1252 2024-02-07 13:55:03.000000 aprsd-3.3.4/.github/workflows/release_build.yml
--rw-r--r--   0 I530566    (501) staff       (20)      501 2024-02-26 15:11:29.000000 aprsd-3.3.4/.pre-commit-config.yaml
--rw-r--r--   0 I530566    (501) staff       (20)      574 2023-06-14 13:31:16.000000 aprsd-3.3.4/.readthedocs.yaml
--rw-r--r--   0 I530566    (501) staff       (20)      467 2024-04-21 16:35:25.000000 aprsd-3.3.4/AUTHORS
--rw-r--r--   0 I530566    (501) staff       (20)    28156 2024-04-21 16:35:25.000000 aprsd-3.3.4/ChangeLog
--rw-r--r--   0 I530566    (501) staff       (20)      801 2023-10-30 12:19:57.000000 aprsd-3.3.4/INSTALL.txt
--rw-r--r--   0 I530566    (501) staff       (20)    10142 2021-08-13 16:31:50.000000 aprsd-3.3.4/LICENSE
--rw-r--r--   0 I530566    (501) staff       (20)       94 2021-08-13 16:31:50.000000 aprsd-3.3.4/MANIFEST.in
--rw-r--r--   0 I530566    (501) staff       (20)     2737 2024-03-06 17:59:56.000000 aprsd-3.3.4/Makefile
--rw-r--r--   0 I530566    (501) staff       (20)    23963 2024-04-21 16:35:29.886339 aprsd-3.3.4/PKG-INFO
--rw-r--r--   0 I530566    (501) staff       (20)    20703 2024-02-28 21:10:10.000000 aprsd-3.3.4/README.rst
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.075258 aprsd-3.3.4/aprsd/
--rw-r--r--   0 I530566    (501) staff       (20)      631 2022-12-12 18:34:05.000000 aprsd-3.3.4/aprsd/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     4568 2024-03-12 14:35:42.000000 aprsd-3.3.4/aprsd/cli_helper.py
--rw-r--r--   0 I530566    (501) staff       (20)    10072 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/client.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.118767 aprsd-3.3.4/aprsd/clients/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:06.000000 aprsd-3.3.4/aprsd/clients/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     7156 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/clients/aprsis.py
--rw-r--r--   0 I530566    (501) staff       (20)     2066 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/clients/fake.py
--rw-r--r--   0 I530566    (501) staff       (20)     3393 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/clients/kiss.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.123178 aprsd-3.3.4/aprsd/cmds/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.3.4/aprsd/cmds/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     1763 2023-07-08 21:30:26.000000 aprsd-3.3.4/aprsd/cmds/completion.py
--rw-r--r--   0 I530566    (501) staff       (20)     4369 2024-01-19 16:29:18.000000 aprsd-3.3.4/aprsd/cmds/dev.py
--rw-r--r--   0 I530566    (501) staff       (20)     5489 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/cmds/fetch_stats.py
--rw-r--r--   0 I530566    (501) staff       (20)     2801 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/cmds/healthcheck.py
--rw-r--r--   0 I530566    (501) staff       (20)    10667 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/cmds/list_plugins.py
--rw-r--r--   0 I530566    (501) staff       (20)     6241 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/cmds/listen.py
--rw-r--r--   0 I530566    (501) staff       (20)     4716 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/cmds/send_message.py
--rw-r--r--   0 I530566    (501) staff       (20)     3777 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/cmds/server.py
--rw-r--r--   0 I530566    (501) staff       (20)    20205 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/cmds/webchat.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.126503 aprsd-3.3.4/aprsd/conf/
--rw-r--r--   0 I530566    (501) staff       (20)     1725 2023-07-16 20:28:21.000000 aprsd-3.3.4/aprsd/conf/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     3029 2023-10-06 19:44:29.000000 aprsd-3.3.4/aprsd/conf/client.py
--rw-r--r--   0 I530566    (501) staff       (20)     8122 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/conf/common.py
--rw-r--r--   0 I530566    (501) staff       (20)     1424 2024-03-06 19:18:34.000000 aprsd-3.3.4/aprsd/conf/log.py
--rw-r--r--   0 I530566    (501) staff       (20)     2701 2022-12-29 19:14:43.000000 aprsd-3.3.4/aprsd/conf/opts.py
--rw-r--r--   0 I530566    (501) staff       (20)     6253 2023-11-30 21:01:05.000000 aprsd-3.3.4/aprsd/conf/plugin_common.py
--rw-r--r--   0 I530566    (501) staff       (20)     2332 2022-12-29 19:16:10.000000 aprsd-3.3.4/aprsd/conf/plugin_email.py
--rw-r--r--   0 I530566    (501) staff       (20)      502 2022-12-12 18:34:08.000000 aprsd-3.3.4/aprsd/exception.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.127600 aprsd-3.3.4/aprsd/log/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2023-07-16 20:28:22.000000 aprsd-3.3.4/aprsd/log/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     2698 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/log/log.py
--rw-r--r--   0 I530566    (501) staff       (20)     5039 2024-04-21 16:31:18.000000 aprsd-3.3.4/aprsd/main.py
--rw-r--r--   0 I530566    (501) staff       (20)      134 2022-12-20 22:38:48.000000 aprsd-3.3.4/aprsd/messaging.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.132222 aprsd-3.3.4/aprsd/packets/
--rw-r--r--   0 I530566    (501) staff       (20)      434 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/packets/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)    22655 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/packets/core.py
--rw-r--r--   0 I530566    (501) staff       (20)     2444 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/packets/packet_list.py
--rw-r--r--   0 I530566    (501) staff       (20)     1071 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/packets/seen_list.py
--rw-r--r--   0 I530566    (501) staff       (20)     3005 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/packets/tracker.py
--rw-r--r--   0 I530566    (501) staff       (20)     2880 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/packets/watch_list.py
--rw-r--r--   0 I530566    (501) staff       (20)    16435 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/plugin.py
--rw-r--r--   0 I530566    (501) staff       (20)     2507 2023-11-30 21:01:05.000000 aprsd-3.3.4/aprsd/plugin_utils.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.136824 aprsd-3.3.4/aprsd/plugins/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:08.000000 aprsd-3.3.4/aprsd/plugins/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)    23073 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/plugins/email.py
--rw-r--r--   0 I530566    (501) staff       (20)     1573 2024-01-09 14:05:51.000000 aprsd-3.3.4/aprsd/plugins/fortune.py
--rw-r--r--   0 I530566    (501) staff       (20)     6464 2023-11-30 21:01:05.000000 aprsd-3.3.4/aprsd/plugins/location.py
--rw-r--r--   0 I530566    (501) staff       (20)     1969 2022-12-29 19:14:43.000000 aprsd-3.3.4/aprsd/plugins/notify.py
--rw-r--r--   0 I530566    (501) staff       (20)      763 2022-12-29 19:18:50.000000 aprsd-3.3.4/aprsd/plugins/ping.py
--rw-r--r--   0 I530566    (501) staff       (20)     2458 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/plugins/query.py
--rw-r--r--   0 I530566    (501) staff       (20)     3496 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/plugins/time.py
--rw-r--r--   0 I530566    (501) staff       (20)      849 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/plugins/version.py
--rw-r--r--   0 I530566    (501) staff       (20)    13356 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/plugins/weather.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.139169 aprsd-3.3.4/aprsd/rpc/
--rw-r--r--   0 I530566    (501) staff       (20)      343 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/rpc/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     4641 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/rpc/client.py
--rw-r--r--   0 I530566    (501) staff       (20)     2750 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/rpc/server.py
--rw-r--r--   0 I530566    (501) staff       (20)     7101 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/stats.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.143638 aprsd-3.3.4/aprsd/threads/
--rw-r--r--   0 I530566    (501) staff       (20)      319 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/threads/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     2270 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/threads/aprsd.py
--rw-r--r--   0 I530566    (501) staff       (20)     4250 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/threads/keep_alive.py
--rw-r--r--   0 I530566    (501) staff       (20)     2036 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/threads/log_monitor.py
--rw-r--r--   0 I530566    (501) staff       (20)     1702 2024-03-08 16:48:51.000000 aprsd-3.3.4/aprsd/threads/registry.py
--rw-r--r--   0 I530566    (501) staff       (20)    12592 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/threads/rx.py
--rw-r--r--   0 I530566    (501) staff       (20)     7694 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/threads/tx.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.147600 aprsd-3.3.4/aprsd/utils/
--rw-r--r--   0 I530566    (501) staff       (20)     4159 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/utils/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     1156 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/utils/counter.py
--rw-r--r--   0 I530566    (501) staff       (20)     3265 2022-12-12 18:34:08.000000 aprsd-3.3.4/aprsd/utils/fuzzyclock.py
--rw-r--r--   0 I530566    (501) staff       (20)     1871 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/utils/json.py
--rw-r--r--   0 I530566    (501) staff       (20)     3401 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/utils/objectstore.py
--rw-r--r--   0 I530566    (501) staff       (20)     1111 2023-09-28 16:16:17.000000 aprsd-3.3.4/aprsd/utils/ring_buffer.py
--rw-r--r--   0 I530566    (501) staff       (20)     5558 2023-09-20 13:44:26.000000 aprsd-3.3.4/aprsd/utils/trace.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.148299 aprsd-3.3.4/aprsd/web/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.3.4/aprsd/web/__init__.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.148849 aprsd-3.3.4/aprsd/web/admin/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.3.4/aprsd/web/admin/__init__.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.010954 aprsd-3.3.4/aprsd/web/admin/static/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.218983 aprsd-3.3.4/aprsd/web/admin/static/css/
--rw-r--r--   0 I530566    (501) staff       (20)     1282 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/css/index.css
--rw-r--r--   0 I530566    (501) staff       (20)     3467 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/static/css/prism.css
--rw-r--r--   0 I530566    (501) staff       (20)      644 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/css/tabs.css
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.426050 aprsd-3.3.4/aprsd/web/admin/static/images/
--rw-r--r--   0 I530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/images/Untitled.png
--rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-16-0.png
--rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-16-1.png
--rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-64-0.png
--rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-64-1.png
--rw-r--r--   0 I530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-64-2.png
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.451118 aprsd-3.3.4/aprsd/web/admin/static/js/
--rw-r--r--   0 I530566    (501) staff       (20)     7360 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/static/js/charts.js
--rw-r--r--   0 I530566    (501) staff       (20)    10244 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/static/js/echarts.js
--rw-r--r--   0 I530566    (501) staff       (20)      658 2024-04-04 20:35:29.000000 aprsd-3.3.4/aprsd/web/admin/static/js/logs.js
--rw-r--r--   0 I530566    (501) staff       (20)     6799 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/static/js/main.js
--rw-r--r--   0 I530566    (501) staff       (20)    64705 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/static/js/prism.js
--rw-r--r--   0 I530566    (501) staff       (20)     3852 2022-12-29 19:14:44.000000 aprsd-3.3.4/aprsd/web/admin/static/js/send-message.js
--rw-r--r--   0 I530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/admin/static/js/tabs.js
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.456261 aprsd-3.3.4/aprsd/web/admin/static/json-viewer/
--rw-r--r--   0 I530566    (501) staff       (20)     1080 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/static/json-viewer/jquery.json-viewer.css
--rw-r--r--   0 I530566    (501) staff       (20)     5020 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/static/json-viewer/jquery.json-viewer.js
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.460214 aprsd-3.3.4/aprsd/web/admin/templates/
--rw-r--r--   0 I530566    (501) staff       (20)     8553 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/admin/templates/index.html
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.014206 aprsd-3.3.4/aprsd/web/chat/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.014016 aprsd-3.3.4/aprsd/web/chat/static/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.487822 aprsd-3.3.4/aprsd/web/chat/static/css/
--rw-r--r--   0 I530566    (501) staff       (20)     1847 2023-09-26 14:47:10.000000 aprsd-3.3.4/aprsd/web/chat/static/css/chat.css
--rw-r--r--   0 I530566    (501) staff       (20)     1056 2024-02-20 00:24:44.000000 aprsd-3.3.4/aprsd/web/chat/static/css/index.css
--rw-r--r--   0 I530566    (501) staff       (20)   174659 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/css/style.css.map
--rw-r--r--   0 I530566    (501) staff       (20)      720 2023-09-13 01:18:30.000000 aprsd-3.3.4/aprsd/web/chat/static/css/tabs.css
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.504690 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/
--rw-r--r--   0 I530566    (501) staff       (20)   232949 2023-11-17 16:39:36.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/bootstrap.min.css
--rw-r--r--   0 I530566    (501) staff       (20)   883712 2023-11-17 16:39:36.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/font.woff2
--rw-r--r--   0 I530566    (501) staff       (20)      549 2023-11-17 16:39:36.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/google-fonts.css
--rw-r--r--   0 I530566    (501) staff       (20)    36536 2020-03-03 19:15:00.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/jquery-ui.css
--rw-r--r--   0 I530566    (501) staff       (20)     4887 2023-09-13 16:05:37.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/jquery.toast.css
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.012894 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.013058 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.013218 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.579514 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/
--rw-r--r--   0 I530566    (501) staff       (20)    72376 2023-06-25 03:32:57.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff
--rw-r--r--   0 I530566    (501) staff       (20)    44380 2023-06-22 11:02:18.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff2
--rw-r--r--   0 I530566    (501) staff       (20)    72456 2023-06-25 03:32:58.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff
--rw-r--r--   0 I530566    (501) staff       (20)    43760 2023-06-22 11:02:18.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff2
--rw-r--r--   0 I530566    (501) staff       (20)   101648 2023-06-25 03:32:58.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff
--rw-r--r--   0 I530566    (501) staff       (20)    78268 2023-06-22 11:02:18.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff2
--rw-r--r--   0 I530566    (501) staff       (20)    16276 2023-06-25 03:32:58.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff
--rw-r--r--   0 I530566    (501) staff       (20)    13224 2023-06-22 11:02:18.000000 aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff2
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.600280 aprsd-3.3.4/aprsd/web/chat/static/images/
--rw-r--r--   0 I530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/images/Untitled.png
--rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-16-0.png
--rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-16-1.png
--rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-64-0.png
--rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-64-1.png
--rw-r--r--   0 I530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-64-2.png
--rw-r--r--   0 I530566    (501) staff       (20)     1197 2024-02-06 18:50:32.000000 aprsd-3.3.4/aprsd/web/chat/static/images/globe.svg
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.615918 aprsd-3.3.4/aprsd/web/chat/static/js/
--rw-r--r--   0 I530566    (501) staff       (20)     2302 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/chat/static/js/gps.js
--rw-r--r--   0 I530566    (501) staff       (20)     1226 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/chat/static/js/main.js
--rw-r--r--   0 I530566    (501) staff       (20)    18620 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/chat/static/js/send-message.js
--rw-r--r--   0 I530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.3.4/aprsd/web/chat/static/js/tabs.js
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.737622 aprsd-3.3.4/aprsd/web/chat/static/js/upstream/
--rw-r--r--   0 I530566    (501) staff       (20)    80664 2023-11-17 16:39:36.000000 aprsd-3.3.4/aprsd/web/chat/static/js/upstream/bootstrap.bundle.min.js
--rw-r--r--   0 I530566    (501) staff       (20)    87533 2023-11-17 16:39:36.000000 aprsd-3.3.4/aprsd/web/chat/static/js/upstream/jquery-3.7.1.min.js
--rw-r--r--   0 I530566    (501) staff       (20)   253669 2023-08-22 16:42:48.000000 aprsd-3.3.4/aprsd/web/chat/static/js/upstream/jquery-ui.min.js
--rw-r--r--   0 I530566    (501) staff       (20)    12989 2023-09-13 16:05:37.000000 aprsd-3.3.4/aprsd/web/chat/static/js/upstream/jquery.toast.js
--rw-r--r--   0 I530566    (501) staff       (20)   403125 2023-08-22 16:42:48.000000 aprsd-3.3.4/aprsd/web/chat/static/js/upstream/semantic.min.js
--rw-r--r--   0 I530566    (501) staff       (20)    64274 2023-08-22 16:42:48.000000 aprsd-3.3.4/aprsd/web/chat/static/js/upstream/socket.io.min.js
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.740945 aprsd-3.3.4/aprsd/web/chat/static/json-viewer/
--rw-r--r--   0 I530566    (501) staff       (20)     1080 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/chat/static/json-viewer/jquery.json-viewer.css
--rw-r--r--   0 I530566    (501) staff       (20)     5020 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/chat/static/json-viewer/jquery.json-viewer.js
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.746215 aprsd-3.3.4/aprsd/web/chat/templates/
--rw-r--r--   0 I530566    (501) staff       (20)     6566 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/web/chat/templates/index.html
--rw-r--r--   0 I530566    (501) staff       (20)    10080 2024-04-21 15:40:03.000000 aprsd-3.3.4/aprsd/wsgi.py
--rw-r--r--   0 I530566    (501) staff       (20)     1599 2021-08-13 16:31:50.000000 aprsd-3.3.4/aprsd-lnav.json
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.885368 aprsd-3.3.4/aprsd.egg-info/
--rw-r--r--   0 I530566    (501) staff       (20)    23963 2024-04-21 16:35:25.000000 aprsd-3.3.4/aprsd.egg-info/PKG-INFO
--rw-r--r--   0 I530566    (501) staff       (20)     6307 2024-04-21 16:35:28.000000 aprsd-3.3.4/aprsd.egg-info/SOURCES.txt
--rw-r--r--   0 I530566    (501) staff       (20)        1 2024-04-21 16:35:25.000000 aprsd-3.3.4/aprsd.egg-info/dependency_links.txt
--rw-r--r--   0 I530566    (501) staff       (20)      171 2024-04-21 16:35:25.000000 aprsd-3.3.4/aprsd.egg-info/entry_points.txt
--rw-r--r--   0 I530566    (501) staff       (20)        1 2024-04-21 16:35:25.000000 aprsd-3.3.4/aprsd.egg-info/not-zip-safe
--rw-r--r--   0 I530566    (501) staff       (20)       46 2024-04-21 16:35:25.000000 aprsd-3.3.4/aprsd.egg-info/pbr.json
--rw-r--r--   0 I530566    (501) staff       (20)     1301 2024-04-21 16:35:25.000000 aprsd-3.3.4/aprsd.egg-info/requires.txt
--rw-r--r--   0 I530566    (501) staff       (20)        6 2024-04-21 16:35:25.000000 aprsd-3.3.4/aprsd.egg-info/top_level.txt
--rw-r--r--   0 I530566    (501) staff       (20)      221 2023-06-22 11:54:27.000000 aprsd-3.3.4/dev-requirements.in
--rw-r--r--   0 I530566    (501) staff       (20)     3712 2024-04-21 15:40:03.000000 aprsd-3.3.4/dev-requirements.txt
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.785011 aprsd-3.3.4/docker/
--rw-r--r--   0 I530566    (501) staff       (20)     1670 2024-04-21 15:40:03.000000 aprsd-3.3.4/docker/Dockerfile
--rw-r--r--   0 I530566    (501) staff       (20)     1611 2024-04-21 15:40:03.000000 aprsd-3.3.4/docker/Dockerfile-dev
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.795298 aprsd-3.3.4/docker/bin/
--rwxr-xr-x   0 I530566    (501) staff       (20)     1454 2024-02-25 20:05:31.000000 aprsd-3.3.4/docker/bin/admin.sh
--rwxr-xr-x   0 I530566    (501) staff       (20)     1212 2024-02-25 20:05:31.000000 aprsd-3.3.4/docker/bin/listen.sh
--rwxr-xr-x   0 I530566    (501) staff       (20)     1168 2024-02-25 20:03:37.000000 aprsd-3.3.4/docker/bin/run.sh
--rwxr-xr-x   0 I530566    (501) staff       (20)     2581 2023-04-17 19:01:56.000000 aprsd-3.3.4/docker/build.sh
--rw-r--r--   0 I530566    (501) staff       (20)      327 2022-11-22 00:10:29.000000 aprsd-3.3.4/docker/docker-compose.yml
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.847712 aprsd-3.3.4/docs/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.853362 aprsd-3.3.4/docs/_static/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.3.4/docs/_static/.keep
--rw-r--r--   0 I530566    (501) staff       (20)    77895 2021-08-30 17:18:20.000000 aprsd-3.3.4/docs/_static/aprsd_overview.png
--rw-r--r--   0 I530566    (501) staff       (20)    30397 2021-08-30 17:18:20.000000 aprsd-3.3.4/docs/_static/aprsd_overview.svg
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.853731 aprsd-3.3.4/docs/_templates/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.3.4/docs/_templates/.keep
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.872140 aprsd-3.3.4/docs/apidoc/
--rw-r--r--   0 I530566    (501) staff       (20)      477 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.clients.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1514 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.cmds.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1044 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.conf.rst
--rw-r--r--   0 I530566    (501) staff       (20)      969 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.packets.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1523 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.plugins.rst
--rw-r--r--   0 I530566    (501) staff       (20)      447 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.rpc.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1529 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.rst
--rw-r--r--   0 I530566    (501) staff       (20)      934 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.threads.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1075 2023-09-01 18:43:06.000000 aprsd-3.3.4/docs/apidoc/aprsd.utils.rst
--rw-r--r--   0 I530566    (501) staff       (20)      168 2023-09-01 18:43:07.000000 aprsd-3.3.4/docs/apidoc/aprsd.web.admin.rst
--rw-r--r--   0 I530566    (501) staff       (20)      225 2023-09-01 18:43:07.000000 aprsd-3.3.4/docs/apidoc/aprsd.web.rst
--rw-r--r--   0 I530566    (501) staff       (20)       52 2023-09-01 18:43:07.000000 aprsd-3.3.4/docs/apidoc/modules.rst
--rw-r--r--   0 I530566    (501) staff       (20)     2997 2021-08-30 17:18:20.000000 aprsd-3.3.4/docs/aprsd.drawio
--rw-r--r--   0 I530566    (501) staff       (20)    19792 2023-01-01 19:57:28.000000 aprsd-3.3.4/docs/changelog.rst
--rw-r--r--   0 I530566    (501) staff       (20)      520 2022-12-12 18:34:04.000000 aprsd-3.3.4/docs/clean_docs.py
--rw-r--r--   0 I530566    (501) staff       (20)     5565 2022-12-29 19:14:44.000000 aprsd-3.3.4/docs/conf.py
--rw-r--r--   0 I530566    (501) staff       (20)     8611 2022-12-29 19:14:44.000000 aprsd-3.3.4/docs/configure.rst
--rw-r--r--   0 I530566    (501) staff       (20)      545 2021-08-13 16:31:50.000000 aprsd-3.3.4/docs/index.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1553 2021-08-13 16:31:50.000000 aprsd-3.3.4/docs/install.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1366 2021-08-13 16:31:50.000000 aprsd-3.3.4/docs/links.rst
--rw-r--r--   0 I530566    (501) staff       (20)     1613 2022-12-29 19:14:44.000000 aprsd-3.3.4/docs/plugin.rst
--rw-r--r--   0 I530566    (501) staff       (20)    20002 2023-01-01 19:57:28.000000 aprsd-3.3.4/docs/readme.rst
--rw-r--r--   0 I530566    (501) staff       (20)     2778 2021-08-13 16:31:50.000000 aprsd-3.3.4/docs/server.rst
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.015647 aprsd-3.3.4/examples/
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.874911 aprsd-3.3.4/examples/plugins/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.3.4/examples/plugins/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)      409 2023-06-14 15:27:00.000000 aprsd-3.3.4/examples/plugins/example_plugin.py
--rw-r--r--   0 I530566    (501) staff       (20)       95 2021-08-30 17:18:20.000000 aprsd-3.3.4/gray.conf
--rw-r--r--   0 I530566    (501) staff       (20)      538 2023-08-07 15:02:58.000000 aprsd-3.3.4/pyproject.toml
--rw-r--r--   0 I530566    (501) staff       (20)      510 2024-04-21 15:40:03.000000 aprsd-3.3.4/requirements.in
--rw-r--r--   0 I530566    (501) staff       (20)     4026 2024-04-21 16:30:08.000000 aprsd-3.3.4/requirements.txt
--rw-r--r--   0 I530566    (501) staff       (20)     1245 2024-04-21 16:35:29.890498 aprsd-3.3.4/setup.cfg
--rw-r--r--   0 I530566    (501) staff       (20)     1015 2022-12-12 18:34:08.000000 aprsd-3.3.4/setup.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.877884 aprsd-3.3.4/tests/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.3.4/tests/__init__.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.879293 aprsd-3.3.4/tests/cmds/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:07.000000 aprsd-3.3.4/tests/cmds/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     1810 2023-07-16 20:28:22.000000 aprsd-3.3.4/tests/cmds/test_send_message.py
--rw-r--r--   0 I530566    (501) staff       (20)     2645 2024-04-21 15:40:03.000000 aprsd-3.3.4/tests/cmds/test_webchat.py
--rw-r--r--   0 I530566    (501) staff       (20)     1674 2024-04-21 15:40:03.000000 aprsd-3.3.4/tests/fake.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.882798 aprsd-3.3.4/tests/plugins/
--rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.3.4/tests/plugins/__init__.py
--rw-r--r--   0 I530566    (501) staff       (20)     1112 2022-12-29 19:14:44.000000 aprsd-3.3.4/tests/plugins/test_fortune.py
--rw-r--r--   0 I530566    (501) staff       (20)     4012 2023-06-22 13:42:11.000000 aprsd-3.3.4/tests/plugins/test_location.py
--rw-r--r--   0 I530566    (501) staff       (20)     5895 2022-12-29 19:14:44.000000 aprsd-3.3.4/tests/plugins/test_notify.py
--rw-r--r--   0 I530566    (501) staff       (20)     1395 2022-12-29 19:14:44.000000 aprsd-3.3.4/tests/plugins/test_ping.py
--rw-r--r--   0 I530566    (501) staff       (20)     1696 2024-04-21 15:40:03.000000 aprsd-3.3.4/tests/plugins/test_query.py
--rw-r--r--   0 I530566    (501) staff       (20)     1458 2022-12-29 19:14:44.000000 aprsd-3.3.4/tests/plugins/test_time.py
--rw-r--r--   0 I530566    (501) staff       (20)      970 2024-04-21 15:40:03.000000 aprsd-3.3.4/tests/plugins/test_version.py
--rw-r--r--   0 I530566    (501) staff       (20)     7613 2024-04-21 15:40:03.000000 aprsd-3.3.4/tests/plugins/test_weather.py
--rw-r--r--   0 I530566    (501) staff       (20)      942 2022-12-29 19:14:44.000000 aprsd-3.3.4/tests/test_email.py
--rw-r--r--   0 I530566    (501) staff       (20)      558 2022-12-29 19:14:44.000000 aprsd-3.3.4/tests/test_main.py
--rw-r--r--   0 I530566    (501) staff       (20)     3070 2024-04-21 15:40:03.000000 aprsd-3.3.4/tests/test_packets.py
--rw-r--r--   0 I530566    (501) staff       (20)     6486 2024-04-21 15:40:03.000000 aprsd-3.3.4/tests/test_plugin.py
-drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-21 16:35:29.884758 aprsd-3.3.4/tools/
--rwxr-xr-x   0 I530566    (501) staff       (20)      586 2021-08-13 16:31:50.000000 aprsd-3.3.4/tools/fast8.sh
--rw-r--r--   0 I530566    (501) staff       (20)     2635 2024-04-21 15:40:03.000000 aprsd-3.3.4/tox.ini
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.534193 aprsd-3.4.0/
+-rw-r--r--   0 I530566    (501) staff       (20)      269 2021-08-30 17:18:20.000000 aprsd-3.4.0/.coveragerc
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.848166 aprsd-3.4.0/.github/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.884773 aprsd-3.4.0/.github/workflows/
+-rw-r--r--   0 I530566    (501) staff       (20)     3534 2024-02-09 02:07:13.000000 aprsd-3.4.0/.github/workflows/codeql.yml
+-rw-r--r--   0 I530566    (501) staff       (20)     1461 2024-02-07 13:55:16.000000 aprsd-3.4.0/.github/workflows/manual_build.yml
+-rw-r--r--   0 I530566    (501) staff       (20)     1622 2024-02-07 13:54:43.000000 aprsd-3.4.0/.github/workflows/master-build.yml
+-rw-r--r--   0 I530566    (501) staff       (20)      524 2023-11-17 18:02:52.000000 aprsd-3.4.0/.github/workflows/python.yml
+-rw-r--r--   0 I530566    (501) staff       (20)     1252 2024-02-07 13:55:03.000000 aprsd-3.4.0/.github/workflows/release_build.yml
+-rw-r--r--   0 I530566    (501) staff       (20)      501 2024-02-26 15:11:29.000000 aprsd-3.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 I530566    (501) staff       (20)      574 2023-06-14 13:31:16.000000 aprsd-3.4.0/.readthedocs.yaml
+-rw-r--r--   0 I530566    (501) staff       (20)      467 2024-04-29 13:33:44.000000 aprsd-3.4.0/AUTHORS
+-rw-r--r--   0 I530566    (501) staff       (20)    31862 2024-04-29 13:33:43.000000 aprsd-3.4.0/ChangeLog
+-rw-r--r--   0 I530566    (501) staff       (20)      801 2023-10-30 12:19:57.000000 aprsd-3.4.0/INSTALL.txt
+-rw-r--r--   0 I530566    (501) staff       (20)    10142 2021-08-13 16:31:50.000000 aprsd-3.4.0/LICENSE
+-rw-r--r--   0 I530566    (501) staff       (20)       94 2021-08-13 16:31:50.000000 aprsd-3.4.0/MANIFEST.in
+-rw-r--r--   0 I530566    (501) staff       (20)     2737 2024-03-06 17:59:56.000000 aprsd-3.4.0/Makefile
+-rw-r--r--   0 I530566    (501) staff       (20)    23904 2024-04-29 13:33:48.533966 aprsd-3.4.0/PKG-INFO
+-rw-r--r--   0 I530566    (501) staff       (20)    20703 2024-02-28 21:10:10.000000 aprsd-3.4.0/README.rst
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.887891 aprsd-3.4.0/aprsd/
+-rw-r--r--   0 I530566    (501) staff       (20)      631 2022-12-12 18:34:05.000000 aprsd-3.4.0/aprsd/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4568 2024-03-12 14:35:42.000000 aprsd-3.4.0/aprsd/cli_helper.py
+-rw-r--r--   0 I530566    (501) staff       (20)    13225 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/client.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.894721 aprsd-3.4.0/aprsd/clients/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:06.000000 aprsd-3.4.0/aprsd/clients/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     7257 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/clients/aprsis.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2059 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/clients/fake.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3350 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/clients/kiss.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.899720 aprsd-3.4.0/aprsd/cmds/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.4.0/aprsd/cmds/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)      799 2024-04-23 20:14:18.000000 aprsd-3.4.0/aprsd/cmds/completion.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4369 2024-01-19 16:29:18.000000 aprsd-3.4.0/aprsd/cmds/dev.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4988 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/cmds/fetch_stats.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2628 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/cmds/healthcheck.py
+-rw-r--r--   0 I530566    (501) staff       (20)    10653 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/cmds/list_plugins.py
+-rw-r--r--   0 I530566    (501) staff       (20)     7143 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/cmds/listen.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4711 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/cmds/send_message.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4437 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/cmds/server.py
+-rw-r--r--   0 I530566    (501) staff       (20)    20370 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/cmds/webchat.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.903203 aprsd-3.4.0/aprsd/conf/
+-rw-r--r--   0 I530566    (501) staff       (20)     1725 2023-07-16 20:28:21.000000 aprsd-3.4.0/aprsd/conf/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3029 2023-10-06 19:44:29.000000 aprsd-3.4.0/aprsd/conf/client.py
+-rw-r--r--   0 I530566    (501) staff       (20)     9013 2024-04-24 17:55:16.000000 aprsd-3.4.0/aprsd/conf/common.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1424 2024-03-06 19:18:34.000000 aprsd-3.4.0/aprsd/conf/log.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2701 2022-12-29 19:14:43.000000 aprsd-3.4.0/aprsd/conf/opts.py
+-rw-r--r--   0 I530566    (501) staff       (20)     6253 2023-11-30 21:01:05.000000 aprsd-3.4.0/aprsd/conf/plugin_common.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2332 2022-12-29 19:16:10.000000 aprsd-3.4.0/aprsd/conf/plugin_email.py
+-rw-r--r--   0 I530566    (501) staff       (20)      502 2022-12-12 18:34:08.000000 aprsd-3.4.0/aprsd/exception.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.905068 aprsd-3.4.0/aprsd/log/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2023-07-16 20:28:22.000000 aprsd-3.4.0/aprsd/log/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3408 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/log/log.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4673 2024-04-23 20:14:18.000000 aprsd-3.4.0/aprsd/main.py
+-rw-r--r--   0 I530566    (501) staff       (20)      134 2022-12-20 22:38:48.000000 aprsd-3.4.0/aprsd/messaging.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.908091 aprsd-3.4.0/aprsd/packets/
+-rw-r--r--   0 I530566    (501) staff       (20)      510 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/packets/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1636 2024-04-24 14:47:16.000000 aprsd-3.4.0/aprsd/packets/collector.py
+-rw-r--r--   0 I530566    (501) staff       (20)    27400 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/packets/core.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4545 2024-04-24 17:55:51.000000 aprsd-3.4.0/aprsd/packets/log.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3518 2024-04-24 15:29:18.000000 aprsd-3.4.0/aprsd/packets/packet_list.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1543 2024-04-24 17:49:49.000000 aprsd-3.4.0/aprsd/packets/seen_list.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3165 2024-04-24 17:49:49.000000 aprsd-3.4.0/aprsd/packets/tracker.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3789 2024-04-24 20:27:35.000000 aprsd-3.4.0/aprsd/packets/watch_list.py
+-rw-r--r--   0 I530566    (501) staff       (20)    17359 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/plugin.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2507 2023-11-30 21:01:05.000000 aprsd-3.4.0/aprsd/plugin_utils.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.911626 aprsd-3.4.0/aprsd/plugins/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:08.000000 aprsd-3.4.0/aprsd/plugins/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)    23627 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/plugins/email.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1573 2024-01-09 14:05:51.000000 aprsd-3.4.0/aprsd/plugins/fortune.py
+-rw-r--r--   0 I530566    (501) staff       (20)     6464 2023-11-30 21:01:05.000000 aprsd-3.4.0/aprsd/plugins/location.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1969 2022-12-29 19:14:43.000000 aprsd-3.4.0/aprsd/plugins/notify.py
+-rw-r--r--   0 I530566    (501) staff       (20)      763 2022-12-29 19:18:50.000000 aprsd-3.4.0/aprsd/plugins/ping.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3535 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/plugins/time.py
+-rw-r--r--   0 I530566    (501) staff       (20)      839 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/plugins/version.py
+-rw-r--r--   0 I530566    (501) staff       (20)    13333 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/plugins/weather.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.913255 aprsd-3.4.0/aprsd/stats/
+-rw-r--r--   0 I530566    (501) staff       (20)      884 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/stats/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1256 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/stats/app.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1219 2024-04-24 15:54:04.000000 aprsd-3.4.0/aprsd/stats/collector.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.918206 aprsd-3.4.0/aprsd/threads/
+-rw-r--r--   0 I530566    (501) staff       (20)      274 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/threads/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3292 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/threads/aprsd.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4798 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/threads/keep_alive.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3462 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/threads/log_monitor.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1702 2024-03-08 16:48:51.000000 aprsd-3.4.0/aprsd/threads/registry.py
+-rw-r--r--   0 I530566    (501) staff       (20)    13431 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/threads/rx.py
+-rw-r--r--   0 I530566    (501) staff       (20)      959 2024-04-24 16:16:39.000000 aprsd-3.4.0/aprsd/threads/stats.py
+-rw-r--r--   0 I530566    (501) staff       (20)     8307 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/threads/tx.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.920415 aprsd-3.4.0/aprsd/utils/
+-rw-r--r--   0 I530566    (501) staff       (20)     4547 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/utils/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1202 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/utils/counter.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3265 2022-12-12 18:34:08.000000 aprsd-3.4.0/aprsd/utils/fuzzyclock.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2487 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/utils/json.py
+-rw-r--r--   0 I530566    (501) staff       (20)     3541 2024-04-24 20:28:23.000000 aprsd-3.4.0/aprsd/utils/objectstore.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1111 2023-09-28 16:16:17.000000 aprsd-3.4.0/aprsd/utils/ring_buffer.py
+-rw-r--r--   0 I530566    (501) staff       (20)     5558 2023-09-20 13:44:26.000000 aprsd-3.4.0/aprsd/utils/trace.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.920888 aprsd-3.4.0/aprsd/web/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.4.0/aprsd/web/__init__.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.921165 aprsd-3.4.0/aprsd/web/admin/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.4.0/aprsd/web/admin/__init__.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.851055 aprsd-3.4.0/aprsd/web/admin/static/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.009339 aprsd-3.4.0/aprsd/web/admin/static/css/
+-rw-r--r--   0 I530566    (501) staff       (20)     1282 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/admin/static/css/index.css
+-rw-r--r--   0 I530566    (501) staff       (20)     2671 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/web/admin/static/css/prism.css
+-rw-r--r--   0 I530566    (501) staff       (20)      644 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/admin/static/css/tabs.css
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.024339 aprsd-3.4.0/aprsd/web/admin/static/images/
+-rw-r--r--   0 I530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/admin/static/images/Untitled.png
+-rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/admin/static/images/aprs-symbols-16-0.png
+-rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/admin/static/images/aprs-symbols-16-1.png
+-rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/admin/static/images/aprs-symbols-64-0.png
+-rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/admin/static/images/aprs-symbols-64-1.png
+-rw-r--r--   0 I530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/admin/static/images/aprs-symbols-64-2.png
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.049996 aprsd-3.4.0/aprsd/web/admin/static/js/
+-rw-r--r--   0 I530566    (501) staff       (20)     7354 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/web/admin/static/js/charts.js
+-rw-r--r--   0 I530566    (501) staff       (20)    11738 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/web/admin/static/js/echarts.js
+-rw-r--r--   0 I530566    (501) staff       (20)      658 2024-04-04 20:35:29.000000 aprsd-3.4.0/aprsd/web/admin/static/js/logs.js
+-rw-r--r--   0 I530566    (501) staff       (20)     8128 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/web/admin/static/js/main.js
+-rw-r--r--   0 I530566    (501) staff       (20)    27861 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/web/admin/static/js/prism.js
+-rw-r--r--   0 I530566    (501) staff       (20)     3852 2022-12-29 19:14:44.000000 aprsd-3.4.0/aprsd/web/admin/static/js/send-message.js
+-rw-r--r--   0 I530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/admin/static/js/tabs.js
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.056899 aprsd-3.4.0/aprsd/web/admin/templates/
+-rw-r--r--   0 I530566    (501) staff       (20)     9083 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/web/admin/templates/index.html
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.853175 aprsd-3.4.0/aprsd/web/chat/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.852829 aprsd-3.4.0/aprsd/web/chat/static/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.081664 aprsd-3.4.0/aprsd/web/chat/static/css/
+-rw-r--r--   0 I530566    (501) staff       (20)     1847 2023-09-26 14:47:10.000000 aprsd-3.4.0/aprsd/web/chat/static/css/chat.css
+-rw-r--r--   0 I530566    (501) staff       (20)     1056 2024-02-20 00:24:44.000000 aprsd-3.4.0/aprsd/web/chat/static/css/index.css
+-rw-r--r--   0 I530566    (501) staff       (20)   174659 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/chat/static/css/style.css.map
+-rw-r--r--   0 I530566    (501) staff       (20)      720 2023-09-13 01:18:30.000000 aprsd-3.4.0/aprsd/web/chat/static/css/tabs.css
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.097438 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/
+-rw-r--r--   0 I530566    (501) staff       (20)   232949 2023-11-17 16:39:36.000000 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/bootstrap.min.css
+-rw-r--r--   0 I530566    (501) staff       (20)   883712 2023-11-17 16:39:36.000000 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/font.woff2
+-rw-r--r--   0 I530566    (501) staff       (20)      549 2023-11-17 16:39:36.000000 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/google-fonts.css
+-rw-r--r--   0 I530566    (501) staff       (20)    36536 2020-03-03 19:15:00.000000 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/jquery-ui.css
+-rw-r--r--   0 I530566    (501) staff       (20)     4887 2023-09-13 16:05:37.000000 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/jquery.toast.css
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.852175 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.852315 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.852462 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.123665 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/
+-rw-r--r--   0 I530566    (501) staff       (20)    72376 2023-06-25 03:32:57.000000 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff
+-rw-r--r--   0 I530566    (501) staff       (20)    44380 2023-06-22 11:02:18.000000 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff2
+-rw-r--r--   0 I530566    (501) staff       (20)    72456 2023-06-25 03:32:58.000000 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff
+-rw-r--r--   0 I530566    (501) staff       (20)    43760 2023-06-22 11:02:18.000000 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff2
+-rw-r--r--   0 I530566    (501) staff       (20)   101648 2023-06-25 03:32:58.000000 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff
+-rw-r--r--   0 I530566    (501) staff       (20)    78268 2023-06-22 11:02:18.000000 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff2
+-rw-r--r--   0 I530566    (501) staff       (20)    16276 2023-06-25 03:32:58.000000 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff
+-rw-r--r--   0 I530566    (501) staff       (20)    13224 2023-06-22 11:02:18.000000 aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff2
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.147006 aprsd-3.4.0/aprsd/web/chat/static/images/
+-rw-r--r--   0 I530566    (501) staff       (20)    37797 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/chat/static/images/Untitled.png
+-rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/chat/static/images/aprs-symbols-16-0.png
+-rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/chat/static/images/aprs-symbols-16-1.png
+-rw-r--r--   0 I530566    (501) staff       (20)    52962 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/chat/static/images/aprs-symbols-64-0.png
+-rw-r--r--   0 I530566    (501) staff       (20)    48951 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/chat/static/images/aprs-symbols-64-1.png
+-rw-r--r--   0 I530566    (501) staff       (20)    40716 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/chat/static/images/aprs-symbols-64-2.png
+-rw-r--r--   0 I530566    (501) staff       (20)     1197 2024-02-06 18:50:32.000000 aprsd-3.4.0/aprsd/web/chat/static/images/globe.svg
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.161880 aprsd-3.4.0/aprsd/web/chat/static/js/
+-rw-r--r--   0 I530566    (501) staff       (20)     2370 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/web/chat/static/js/gps.js
+-rw-r--r--   0 I530566    (501) staff       (20)     1259 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/web/chat/static/js/main.js
+-rw-r--r--   0 I530566    (501) staff       (20)    18851 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/web/chat/static/js/send-message.js
+-rw-r--r--   0 I530566    (501) staff       (20)      889 2022-11-23 18:33:33.000000 aprsd-3.4.0/aprsd/web/chat/static/js/tabs.js
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.301240 aprsd-3.4.0/aprsd/web/chat/static/js/upstream/
+-rw-r--r--   0 I530566    (501) staff       (20)    80664 2023-11-17 16:39:36.000000 aprsd-3.4.0/aprsd/web/chat/static/js/upstream/bootstrap.bundle.min.js
+-rw-r--r--   0 I530566    (501) staff       (20)    87533 2023-11-17 16:39:36.000000 aprsd-3.4.0/aprsd/web/chat/static/js/upstream/jquery-3.7.1.min.js
+-rw-r--r--   0 I530566    (501) staff       (20)   253669 2023-08-22 16:42:48.000000 aprsd-3.4.0/aprsd/web/chat/static/js/upstream/jquery-ui.min.js
+-rw-r--r--   0 I530566    (501) staff       (20)    12989 2023-09-13 16:05:37.000000 aprsd-3.4.0/aprsd/web/chat/static/js/upstream/jquery.toast.js
+-rw-r--r--   0 I530566    (501) staff       (20)   403125 2023-08-22 16:42:48.000000 aprsd-3.4.0/aprsd/web/chat/static/js/upstream/semantic.min.js
+-rw-r--r--   0 I530566    (501) staff       (20)    64274 2023-08-22 16:42:48.000000 aprsd-3.4.0/aprsd/web/chat/static/js/upstream/socket.io.min.js
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.307675 aprsd-3.4.0/aprsd/web/chat/templates/
+-rw-r--r--   0 I530566    (501) staff       (20)     6633 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/web/chat/templates/index.html
+-rw-r--r--   0 I530566    (501) staff       (20)     8720 2024-04-21 16:39:49.000000 aprsd-3.4.0/aprsd/wsgi.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1599 2021-08-13 16:31:50.000000 aprsd-3.4.0/aprsd-lnav.json
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.533132 aprsd-3.4.0/aprsd.egg-info/
+-rw-r--r--   0 I530566    (501) staff       (20)    23904 2024-04-29 13:33:44.000000 aprsd-3.4.0/aprsd.egg-info/PKG-INFO
+-rw-r--r--   0 I530566    (501) staff       (20)     6110 2024-04-29 13:33:47.000000 aprsd-3.4.0/aprsd.egg-info/SOURCES.txt
+-rw-r--r--   0 I530566    (501) staff       (20)        1 2024-04-29 13:33:44.000000 aprsd-3.4.0/aprsd.egg-info/dependency_links.txt
+-rw-r--r--   0 I530566    (501) staff       (20)      171 2024-04-29 13:33:44.000000 aprsd-3.4.0/aprsd.egg-info/entry_points.txt
+-rw-r--r--   0 I530566    (501) staff       (20)        1 2024-04-29 13:33:44.000000 aprsd-3.4.0/aprsd.egg-info/not-zip-safe
+-rw-r--r--   0 I530566    (501) staff       (20)       46 2024-04-29 13:33:44.000000 aprsd-3.4.0/aprsd.egg-info/pbr.json
+-rw-r--r--   0 I530566    (501) staff       (20)     1272 2024-04-29 13:33:44.000000 aprsd-3.4.0/aprsd.egg-info/requires.txt
+-rw-r--r--   0 I530566    (501) staff       (20)        6 2024-04-29 13:33:44.000000 aprsd-3.4.0/aprsd.egg-info/top_level.txt
+-rw-r--r--   0 I530566    (501) staff       (20)      221 2023-06-22 11:54:27.000000 aprsd-3.4.0/dev-requirements.in
+-rw-r--r--   0 I530566    (501) staff       (20)     3641 2024-04-23 19:19:29.000000 aprsd-3.4.0/dev-requirements.txt
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.320435 aprsd-3.4.0/docker/
+-rw-r--r--   0 I530566    (501) staff       (20)     1690 2024-04-24 23:03:18.000000 aprsd-3.4.0/docker/Dockerfile
+-rw-r--r--   0 I530566    (501) staff       (20)     1650 2024-04-24 23:03:03.000000 aprsd-3.4.0/docker/Dockerfile-dev
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.335907 aprsd-3.4.0/docker/bin/
+-rwxr-xr-x   0 I530566    (501) staff       (20)     1454 2024-02-25 20:05:31.000000 aprsd-3.4.0/docker/bin/admin.sh
+-rwxr-xr-x   0 I530566    (501) staff       (20)     1212 2024-02-25 20:05:31.000000 aprsd-3.4.0/docker/bin/listen.sh
+-rwxr-xr-x   0 I530566    (501) staff       (20)     1168 2024-02-25 20:03:37.000000 aprsd-3.4.0/docker/bin/run.sh
+-rwxr-xr-x   0 I530566    (501) staff       (20)     1318 2024-04-24 23:36:02.000000 aprsd-3.4.0/docker/bin/setup.sh
+-rwxr-xr-x   0 I530566    (501) staff       (20)     2581 2024-04-23 19:02:55.000000 aprsd-3.4.0/docker/build.sh
+-rw-r--r--   0 I530566    (501) staff       (20)      327 2022-11-22 00:10:29.000000 aprsd-3.4.0/docker/docker-compose.yml
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.374220 aprsd-3.4.0/docs/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.481394 aprsd-3.4.0/docs/_static/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.4.0/docs/_static/.keep
+-rw-r--r--   0 I530566    (501) staff       (20)    77895 2021-08-30 17:18:20.000000 aprsd-3.4.0/docs/_static/aprsd_overview.png
+-rw-r--r--   0 I530566    (501) staff       (20)    30397 2021-08-30 17:18:20.000000 aprsd-3.4.0/docs/_static/aprsd_overview.svg
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.482509 aprsd-3.4.0/docs/_templates/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2021-08-13 16:31:50.000000 aprsd-3.4.0/docs/_templates/.keep
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.511161 aprsd-3.4.0/docs/apidoc/
+-rw-r--r--   0 I530566    (501) staff       (20)      477 2023-09-01 18:43:06.000000 aprsd-3.4.0/docs/apidoc/aprsd.clients.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1514 2023-09-01 18:43:06.000000 aprsd-3.4.0/docs/apidoc/aprsd.cmds.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1044 2023-09-01 18:43:06.000000 aprsd-3.4.0/docs/apidoc/aprsd.conf.rst
+-rw-r--r--   0 I530566    (501) staff       (20)      969 2023-09-01 18:43:06.000000 aprsd-3.4.0/docs/apidoc/aprsd.packets.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1523 2023-09-01 18:43:06.000000 aprsd-3.4.0/docs/apidoc/aprsd.plugins.rst
+-rw-r--r--   0 I530566    (501) staff       (20)      447 2023-09-01 18:43:06.000000 aprsd-3.4.0/docs/apidoc/aprsd.rpc.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1529 2023-09-01 18:43:06.000000 aprsd-3.4.0/docs/apidoc/aprsd.rst
+-rw-r--r--   0 I530566    (501) staff       (20)      934 2023-09-01 18:43:06.000000 aprsd-3.4.0/docs/apidoc/aprsd.threads.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1075 2023-09-01 18:43:06.000000 aprsd-3.4.0/docs/apidoc/aprsd.utils.rst
+-rw-r--r--   0 I530566    (501) staff       (20)      168 2023-09-01 18:43:07.000000 aprsd-3.4.0/docs/apidoc/aprsd.web.admin.rst
+-rw-r--r--   0 I530566    (501) staff       (20)      225 2023-09-01 18:43:07.000000 aprsd-3.4.0/docs/apidoc/aprsd.web.rst
+-rw-r--r--   0 I530566    (501) staff       (20)       52 2023-09-01 18:43:07.000000 aprsd-3.4.0/docs/apidoc/modules.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     2997 2021-08-30 17:18:20.000000 aprsd-3.4.0/docs/aprsd.drawio
+-rw-r--r--   0 I530566    (501) staff       (20)    19792 2023-01-01 19:57:28.000000 aprsd-3.4.0/docs/changelog.rst
+-rw-r--r--   0 I530566    (501) staff       (20)      520 2022-12-12 18:34:04.000000 aprsd-3.4.0/docs/clean_docs.py
+-rw-r--r--   0 I530566    (501) staff       (20)     5565 2022-12-29 19:14:44.000000 aprsd-3.4.0/docs/conf.py
+-rw-r--r--   0 I530566    (501) staff       (20)     8611 2022-12-29 19:14:44.000000 aprsd-3.4.0/docs/configure.rst
+-rw-r--r--   0 I530566    (501) staff       (20)      545 2021-08-13 16:31:50.000000 aprsd-3.4.0/docs/index.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1553 2021-08-13 16:31:50.000000 aprsd-3.4.0/docs/install.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1366 2021-08-13 16:31:50.000000 aprsd-3.4.0/docs/links.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     1613 2022-12-29 19:14:44.000000 aprsd-3.4.0/docs/plugin.rst
+-rw-r--r--   0 I530566    (501) staff       (20)    20002 2023-01-01 19:57:28.000000 aprsd-3.4.0/docs/readme.rst
+-rw-r--r--   0 I530566    (501) staff       (20)     2778 2021-08-13 16:31:50.000000 aprsd-3.4.0/docs/server.rst
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:47.854542 aprsd-3.4.0/examples/
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.514649 aprsd-3.4.0/examples/plugins/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.4.0/examples/plugins/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)      409 2023-06-14 15:27:00.000000 aprsd-3.4.0/examples/plugins/example_plugin.py
+-rw-r--r--   0 I530566    (501) staff       (20)       95 2021-08-30 17:18:20.000000 aprsd-3.4.0/gray.conf
+-rw-r--r--   0 I530566    (501) staff       (20)      538 2023-08-07 15:02:58.000000 aprsd-3.4.0/pyproject.toml
+-rw-r--r--   0 I530566    (501) staff       (20)      481 2024-04-23 19:52:30.000000 aprsd-3.4.0/requirements.in
+-rw-r--r--   0 I530566    (501) staff       (20)     3938 2024-04-23 19:19:24.000000 aprsd-3.4.0/requirements.txt
+-rw-r--r--   0 I530566    (501) staff       (20)     1245 2024-04-29 13:33:48.536793 aprsd-3.4.0/setup.cfg
+-rw-r--r--   0 I530566    (501) staff       (20)     1015 2022-12-12 18:34:08.000000 aprsd-3.4.0/setup.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.521418 aprsd-3.4.0/tests/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:04.000000 aprsd-3.4.0/tests/__init__.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.523985 aprsd-3.4.0/tests/cmds/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:07.000000 aprsd-3.4.0/tests/cmds/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1810 2023-07-16 20:28:22.000000 aprsd-3.4.0/tests/cmds/test_send_message.py
+-rw-r--r--   0 I530566    (501) staff       (20)     2568 2024-04-21 16:39:49.000000 aprsd-3.4.0/tests/cmds/test_webchat.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1852 2024-04-21 16:39:49.000000 aprsd-3.4.0/tests/fake.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.530084 aprsd-3.4.0/tests/plugins/
+-rw-r--r--   0 I530566    (501) staff       (20)        0 2022-12-12 18:34:05.000000 aprsd-3.4.0/tests/plugins/__init__.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1112 2022-12-29 19:14:44.000000 aprsd-3.4.0/tests/plugins/test_fortune.py
+-rw-r--r--   0 I530566    (501) staff       (20)     4012 2023-06-22 13:42:11.000000 aprsd-3.4.0/tests/plugins/test_location.py
+-rw-r--r--   0 I530566    (501) staff       (20)     5895 2022-12-29 19:14:44.000000 aprsd-3.4.0/tests/plugins/test_notify.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1395 2022-12-29 19:14:44.000000 aprsd-3.4.0/tests/plugins/test_ping.py
+-rw-r--r--   0 I530566    (501) staff       (20)     1458 2022-12-29 19:14:44.000000 aprsd-3.4.0/tests/plugins/test_time.py
+-rw-r--r--   0 I530566    (501) staff       (20)      921 2024-04-21 16:39:49.000000 aprsd-3.4.0/tests/plugins/test_version.py
+-rw-r--r--   0 I530566    (501) staff       (20)     7607 2024-04-21 16:39:49.000000 aprsd-3.4.0/tests/plugins/test_weather.py
+-rw-r--r--   0 I530566    (501) staff       (20)      942 2022-12-29 19:14:44.000000 aprsd-3.4.0/tests/test_email.py
+-rw-r--r--   0 I530566    (501) staff       (20)      558 2022-12-29 19:14:44.000000 aprsd-3.4.0/tests/test_main.py
+-rw-r--r--   0 I530566    (501) staff       (20)    10221 2024-04-21 16:39:49.000000 aprsd-3.4.0/tests/test_packets.py
+-rw-r--r--   0 I530566    (501) staff       (20)     6356 2024-04-21 16:39:49.000000 aprsd-3.4.0/tests/test_plugin.py
+drwxr-xr-x   0 I530566    (501) staff       (20)        0 2024-04-29 13:33:48.532627 aprsd-3.4.0/tools/
+-rwxr-xr-x   0 I530566    (501) staff       (20)      586 2021-08-13 16:31:50.000000 aprsd-3.4.0/tools/fast8.sh
+-rw-r--r--   0 I530566    (501) staff       (20)     2676 2024-04-21 16:39:49.000000 aprsd-3.4.0/tox.ini
```

### Comparing `aprsd-3.3.4/.github/workflows/codeql.yml` & `aprsd-3.4.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/.github/workflows/manual_build.yml` & `aprsd-3.4.0/.github/workflows/manual_build.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/.github/workflows/master-build.yml` & `aprsd-3.4.0/.github/workflows/master-build.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/.github/workflows/python.yml` & `aprsd-3.4.0/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/.github/workflows/release_build.yml` & `aprsd-3.4.0/.github/workflows/release_build.yml`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/.readthedocs.yaml` & `aprsd-3.4.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/ChangeLog` & `aprsd-3.4.0/docs/changelog.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,311 +1,10 @@
 CHANGES
 =======
 
-v3.3.4
-------
-
-* Fixed entry\_points
-* Fix for entry\_points where python < 3.10
-
-v3.3.3
-------
-
-* Fix for sample-config warning
-
-v3.3.2
-------
-
-* Changelog for 3.3.2
-* Remove warning during sample-config
-* Removed print in utils
-
-v3.3.1
-------
-
-* Updates for 3.3.1
-* Fixed failure with fetch-stats
-* Fixed problem with list-plugins
-
-v3.3.0
-------
-
-* Changelog for 3.3.0
-* sample-config fix
-* Fixed registry url post
-* Changed processpkt message
-* Fixed RegistryThread not sending requests
-* use log.setup\_logging
-* Disable debug logs for aprslib
-* Make registry thread sleep
-* Put threads first after date/time
-* Replace slow rich logging with loguru
-* Updated requirements
-* Fixed pep8
-* Added list-extensions and updated README.rst
-* Change defaults for beacon and registry
-* Add log info for Beacon and Registry threads
-* fixed frequency\_seconds to IntOpt
-* fixed references to conf
-* changed the default packet timeout to 5 minutes
-* Fixed default service registry url
-* fix pep8 failures
-* py311 fails in github
-* Don't send uptime to registry
-* Added sending software string to registry
-* add py310 gh actions
-* Added the new APRS Registry thread
-* Added installing extensions to Docker run
-* Cleanup some logs
-* Added BeaconPacket
-* updated requirements files
-* removed some unneeded code
-* Added iterator to objectstore
-* Added some missing classes to threads
-* Added support for loading extensions
-* Added location for callsign tabs in webchat
-* updated gitignore
-* Create codeql.yml
-* update github action branchs to v8
-* Added Location info on webchat interface
-* Updated dev test-plugin command
-* Update requirements.txt
-* Update for v3.2.3
-
-v3.2.3
-------
-
-* Force fortune path during setup test
-* added /usr/games to path
-* Added fortune to Dockerfile-dev
-* Added missing fortune app
-* aprsd: main.py: Fix premature return in sample\_config
-* Update weather.py  because you can't sort icons by penis
-* Update weather.py  both weather plugins have new Ww regex
-* Update weather.py
-* Fixed a bug with OWMWeatherPlugin
-* Rework Location Plugin
-
-v3.2.2
-------
-
-* Update for v3.2.2 release
-* Fix for types
-* Fix wsgi for prod
-* pep8 fixes
-* remove python 3.12 from github builds
-* Fixed datetime access in core.py
-* removed invalid reference to config.py
-* Updated requirements
-* Reworked the admin graphs
-* Test new packet serialization
-* Try to localize js libs and css for no internet
-* Normalize listen --aprs-login
-* Bump werkzeug from 2.3.7 to 3.0.1
-* Update INSTALL with new conf files
-* Bump urllib3 from 2.0.6 to 2.0.7
-
-v3.2.1
-------
-
-* Changelog for 3.2.1
-* Update index.html disable form autocomplete
-* Update the packet\_dupe\_timeout warning
-* Update the webchat paths
-* Changed the path option to a ListOpt
-* Fixed default path for tcp\_kiss client
-* Set a default password for admin
-* Fix path for KISS clients
-* Added packet\_dupe\_timeout conf
-* Add ability to change path on every TX packet
-* Make Packet objects hashable
-* Bump urllib3 from 2.0.4 to 2.0.6
-* Don't process AckPackets as dupes
-* Fixed another msgNo int issue
-* Fixed issue with packet tracker and msgNO Counter
-* Fixed import of Mutablemapping
-* pep8 fixes
-* rewrote packet\_list and drop dupe packets
-* Log a warning on dupe
-* Fix for dupe packets
-
-v3.2.0
-------
-
-* Update Changelog for 3.2.0
-* minor cleanup prior to release
-* Webchat: fix input maxlength
-* WebChat: cleanup some console.logs
-* WebChat: flash a dupe message
-* Webchat: Fix issue accessing msg.id
-* Webchat: Fix chat css on older browsers
-* WebChat: new tab should get focus
-* Bump gevent from 23.9.0.post1 to 23.9.1
-* Webchat: Fix pep8 errors
-* Webchat: Added tab notifications and raw packet
-* WebChat: Prevent sending message without callsign
-* WebChat: fixed content area scrolling
-* Webchat: tweaks to UI for expanding chat
-* Webchat: Fixed bug deleteing first tab
-* Ensure Keepalive doesn't reset client at startup
-* Ensure parse\_delta\_str doesn't puke
-* WebChat: Send GPS Beacon working
-* webchat: got active tab onclick working
-* webchat: set to\_call to value of tab when selected
-* Center the webchat input form
-* Update index.html to use chat.css
-* Deleted webchat mobile pages
-* Added close X on webchat tabs
-* Reworked webchat with new UI
-* Updated the webchat UI to look like iMessage
-* Restore previous conversations in webchat
-* Remove VIM from Dockerfile
-* recreate client during reset()
-* updated github workflows
-* Updated documentation build
-* Removed admin\_web.py
-* Removed some RPC server log noise
-* Fixed admin page packet date
-* RPC Server logs the client IP on failed auth
-* Start keepalive thread first
-* fixed an issue in the mobile webchat
-* Added dupe checkig code to webchat mobile
-* click on the div after added
-* Webchat suppress to display of dupe messages
-* Convert webchat internet urls to local static urls
-* Make use of webchat gps config options
-* Added new webchat config section
-* fixed webchat logging.logformat typeoh
-
-v3.1.3
-------
-
-* prep for 3.1.3
-* Forcefully allow development webchat flask
-
-v3.1.2
-------
-
-* Updated Changelog for 3.1.2
-* Added support for ThirdParty packet types
-* Disable the Send GPS Beacon button
-* Removed adhoc ssl support in webchat
-
-v3.1.1
-------
-
-* Updated Changelog for v3.1.1
-* Fixed pep8 failures
-* re-enable USWeatherPlugin to use mapClick
-* Fix sending packets over KISS interface
-* Use config web\_ip for running admin ui from module
-* remove loop log
-* Max out the client reconnect backoff to 5
-* Update the Dockerfile
-
-v3.1.0
-------
-
-* Changelog updates for v3.1.0
-* Use CONF.admin.web\_port for single launch web admin
-* Fixed sio namespace registration
-* Update Dockerfile-dev to include uwsgi
-* Fixed pep8
-* change port to 8000
-* replacement of flask-socketio with python-socketio
-* Change how fetch-stats gets it's defaults
-* Ensure fetch-stats ip is a string
-* Add info logging for rpc server calls
-* updated wsgi config default /config/aprsd.conf
-* Added timing after each thread loop
-* Update docker bin/admin.sh
-* Removed flask-classful from webchat
-* Remove flask pinning
-* removed linux/arm/v8
-* Update master build to include linux/arm/v8
-* Update Dockerfile-dev to fix plugin permissions
-* update manual build github
-* Update requirements for upgraded cryptography
-* Added more libs for Dockerfile-dev
-* Replace Dockerfile-dev with python3 slim
-* Moved logging to log for wsgi.py
-* Changed weather plugin regex pattern
-* Limit the float values to 3 decimal places
-* Fixed rain numbers from aprslib
-* Fixed rpc client initialization
-* Fix in for aprslib issue #80
-* Try and fix Dockerfile-dev
-* Fixed pep8 errors
-* Populate stats object with threads info
-* added counts to the fetch-stats table
-* Added the fetch-stats command
-* Replace ratelimiter with rush
-* Added some utilities to Dockerfile-dev
-* add arm64 for manual github build
-* Added manual master build
-* Update master-build.yml
-* Add github manual trigger for master build
-* Fixed unit tests for Location plugin
-* USe new tox and update githubworkflows
-* Updated requirements
-* force tox to 4.3.5
-* Update github workflows
-* Fixed pep8 violation
-* Added rpc server for listen
-* Update location plugin and reworked requirements
-* Fixed .readthedocs.yaml format
-* Add .readthedocs.yaml
-* Example plugin wrong function
-* Ensure conf is imported for threads/tx
-* Update Dockerfile to help build cryptography
-
-v3.0.3
-------
-
-* Update Changelog to 3.0.3
-* cleanup some debug messages
-* Fixed loading of plugins for server
-* Don't load help plugin for listen command
-* Added listen args
-* Change listen command plugins
-* Added listen.sh for docker
-* Update Listen command
-* Update Dockerfile
-* Add ratelimiting for acks and other packets
-
-v3.0.2
-------
-
-* Update Changelog for 3.0.2
-* Import RejectPacket
-
-v3.0.1
-------
-
-* 3.0.1
-* Add support to Reject messages
-* Update Docker builds for 3.0.0
-
-v3.0.0
-------
-
-* Update Changelog for 3.0.0
-* Ensure server command main thread doesn't exit
-* Fixed save directory default
-* Fixed pep8 failure
-* Cleaned up KISS interfaces use of old config
-* reworked usage of importlib.metadata
-* Added new docs files for 3.0.0
-* Removed url option from healthcheck in dev
-* Updated Healthcheck to use rpc to call aprsd
-* Updated docker/bin/run.sh to use new conf
-* Added ObjectPacket
-* Update regex processing and regex for plugins
-* Change ordering of starting up of server command
-* Update documentation and README
 * Decouple admin web interface from server command
 * Dockerfile now produces aprsd.conf
 * Fix some unit tests and loading of CONF w/o file
 * Added missing conf
 * Removed references to old custom config
 * Convert config to oslo\_config
 * Added rain formatting unit tests to WeatherPacket
```

### Comparing `aprsd-3.3.4/INSTALL.txt` & `aprsd-3.4.0/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/LICENSE` & `aprsd-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/Makefile` & `aprsd-3.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/PKG-INFO` & `aprsd-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd
-Version: 3.3.4
+Version: 3.4.0
 Summary: Amateur radio APRS daemon which listens for messages and responds
 Home-page: http://aprsd.readthedocs.org
 Author: Craig Lamparter
 Author-email: something@somewhere.com
 License: Apache
 Project-URL: Source, https://github.com/craigerl/aprsd
 Project-URL: Tracker, https://github.com/craigerl/aprsd/issues
@@ -27,76 +27,74 @@
 Requires-Dist: blinker==1.7.0
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: click==8.1.7
 Requires-Dist: click-completion==0.5.2
 Requires-Dist: click-params==0.5.0
 Requires-Dist: commonmark==0.9.1
-Requires-Dist: dacite2==2.0.0
 Requires-Dist: dataclasses==0.6
 Requires-Dist: dataclasses-json==0.6.4
 Requires-Dist: debtcollector==3.0.0
 Requires-Dist: deprecated==1.2.14
 Requires-Dist: dnspython==2.6.1
-Requires-Dist: eventlet==0.35.2
-Requires-Dist: flask==3.0.2
+Requires-Dist: eventlet==0.36.1
+Requires-Dist: flask==3.0.3
 Requires-Dist: flask-httpauth==4.8.0
 Requires-Dist: flask-socketio==5.3.6
 Requires-Dist: geographiclib==2.0
 Requires-Dist: geopy==2.4.1
 Requires-Dist: gevent==24.2.1
 Requires-Dist: greenlet==3.0.3
 Requires-Dist: h11==0.14.0
-Requires-Dist: idna==3.6
+Requires-Dist: idna==3.7
 Requires-Dist: imapclient==3.0.1
-Requires-Dist: importlib-metadata==7.0.1
-Requires-Dist: itsdangerous==2.1.2
+Requires-Dist: importlib-metadata==7.1.0
+Requires-Dist: itsdangerous==2.2.0
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: kiss3==8.0.0
 Requires-Dist: loguru==0.7.2
 Requires-Dist: markupsafe==2.1.5
 Requires-Dist: marshmallow==3.21.1
 Requires-Dist: mypy-extensions==1.0.0
 Requires-Dist: netaddr==1.2.1
 Requires-Dist: oslo-config==9.4.0
 Requires-Dist: oslo-i18n==6.3.0
-Requires-Dist: packaging==23.2
+Requires-Dist: packaging==24.0
 Requires-Dist: pbr==6.0.0
-Requires-Dist: pluggy==1.4.0
-Requires-Dist: plumbum==1.8.2
+Requires-Dist: pluggy==1.5.0
 Requires-Dist: pygments==2.17.2
 Requires-Dist: pyserial==3.5
 Requires-Dist: pyserial-asyncio==0.6
 Requires-Dist: python-engineio==4.9.0
-Requires-Dist: python-socketio==5.11.1
+Requires-Dist: python-socketio==5.11.2
 Requires-Dist: pytz==2024.1
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: rfc3986==2.0.0
 Requires-Dist: rich==12.6.0
-Requires-Dist: rpyc==6.0.0
 Requires-Dist: rush==2021.4.0
 Requires-Dist: shellingham==1.5.4
 Requires-Dist: simple-websocket==1.0.0
 Requires-Dist: six==1.16.0
 Requires-Dist: soupsieve==2.5
 Requires-Dist: stevedore==5.2.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: thesmuggler==1.0.1
-Requires-Dist: typing-extensions==4.10.0
+Requires-Dist: typing-extensions==4.11.0
 Requires-Dist: typing-inspect==0.9.0
+Requires-Dist: tzlocal==5.2
 Requires-Dist: update-checker==0.18.0
 Requires-Dist: urllib3==2.2.1
 Requires-Dist: validators==0.22.0
-Requires-Dist: werkzeug==3.0.1
+Requires-Dist: werkzeug==3.0.2
 Requires-Dist: wrapt==1.16.0
 Requires-Dist: wsproto==1.2.0
-Requires-Dist: zipp==3.17.0
+Requires-Dist: zipp==3.18.1
 Requires-Dist: zope-event==5.0
-Requires-Dist: zope-interface==6.2
+Requires-Dist: zope-interface==6.3
 
 ===============================================
 APRSD - Ham radio APRS-IS Message plugin server
 ===============================================
 
 KM6LYW and WB4BOR
 ____________________
```

### Comparing `aprsd-3.3.4/README.rst` & `aprsd-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/__init__.py` & `aprsd-3.4.0/aprsd/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/cli_helper.py` & `aprsd-3.4.0/aprsd/cli_helper.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/client.py` & `aprsd-3.4.0/aprsd/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import abc
+import datetime
 import logging
+import threading
 import time
 
 import aprslib
 from aprslib.exceptions import LoginError
 from oslo_config import cfg
+import wrapt
 
 from aprsd import exception
 from aprsd.clients import aprsis, fake, kiss
-from aprsd.packets import core, packet_list
-from aprsd.utils import trace
+from aprsd.packets import core
+from aprsd.utils import singleton, trace
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 TRANSPORT_APRSIS = "aprsis"
 TRANSPORT_TCPKISS = "tcpkiss"
 TRANSPORT_SERIALKISS = "serialkiss"
@@ -21,54 +24,98 @@
 
 # Main must create this from the ClientFactory
 # object such that it's populated with the
 # Correct config
 factory = None
 
 
+@singleton
+class APRSClientStats:
+
+    lock = threading.Lock()
+
+    @wrapt.synchronized(lock)
+    def stats(self, serializable=False):
+        client = factory.create()
+        stats = {
+            "transport": client.transport(),
+            "filter": client.filter,
+            "connected": client.connected,
+        }
+
+        if client.transport() == TRANSPORT_APRSIS:
+            stats["server_string"] = client.client.server_string
+            keepalive = client.client.aprsd_keepalive
+            if serializable:
+                keepalive = keepalive.isoformat()
+            stats["server_keepalive"] = keepalive
+        elif client.transport() == TRANSPORT_TCPKISS:
+            stats["host"] = CONF.kiss_tcp.host
+            stats["port"] = CONF.kiss_tcp.port
+        elif client.transport() == TRANSPORT_SERIALKISS:
+            stats["device"] = CONF.kiss_serial.device
+        return stats
+
+
 class Client:
     """Singleton client class that constructs the aprslib connection."""
 
     _instance = None
     _client = None
 
     connected = False
-    server_string = None
     filter = None
+    lock = threading.Lock()
 
     def __new__(cls, *args, **kwargs):
         """This magic turns this into a singleton."""
         if cls._instance is None:
             cls._instance = super().__new__(cls)
             # Put any initialization here.
+            cls._instance._create_client()
         return cls._instance
 
+    @abc.abstractmethod
+    def stats(self) -> dict:
+        pass
+
     def set_filter(self, filter):
         self.filter = filter
         if self._client:
             self._client.set_filter(filter)
 
     @property
     def client(self):
         if not self._client:
-            LOG.info("Creating APRS client")
-            self._client = self.setup_connection()
-            if self.filter:
-                LOG.info("Creating APRS client filter")
-                self._client.set_filter(self.filter)
+            self._create_client()
         return self._client
 
+    def _create_client(self):
+        self._client = self.setup_connection()
+        if self.filter:
+            LOG.info("Creating APRS client filter")
+            self._client.set_filter(self.filter)
+
+    def stop(self):
+        if self._client:
+            LOG.info("Stopping client connection.")
+            self._client.stop()
+
     def send(self, packet: core.Packet):
-        packet_list.PacketList().tx(packet)
+        """Send a packet to the network."""
         self.client.send(packet)
 
+    @wrapt.synchronized(lock)
     def reset(self):
         """Call this to force a rebuild/reconnect."""
+        LOG.info("Resetting client connection.")
         if self._client:
+            self._client.close()
             del self._client
+            self._create_client()
         else:
             LOG.warning("Client not initialized, nothing to reset.")
 
         # Recreate the client
         LOG.info(f"Creating new client {self.client}")
 
     @abc.abstractmethod
@@ -85,19 +132,46 @@
     def transport():
         pass
 
     @abc.abstractmethod
     def decode_packet(self, *args, **kwargs):
         pass
 
+    @abc.abstractmethod
+    def consumer(self, callback, blocking=False, immortal=False, raw=False):
+        pass
+
+    @abc.abstractmethod
+    def is_alive(self):
+        pass
+
+    @abc.abstractmethod
+    def close(self):
+        pass
+
 
 class APRSISClient(Client):
 
     _client = None
 
+    def __init__(self):
+        max_timeout = {"hours": 0.0, "minutes": 2, "seconds": 0}
+        self.max_delta = datetime.timedelta(**max_timeout)
+
+    def stats(self) -> dict:
+        stats = {}
+        if self.is_configured():
+            stats = {
+                "server_string": self._client.server_string,
+                "sever_keepalive": self._client.aprsd_keepalive,
+                "filter": self.filter,
+            }
+
+        return stats
+
     @staticmethod
     def is_enabled():
         # Defaults to True if the enabled flag is non existent
         try:
             return CONF.aprs_network.enabled
         except KeyError:
             return False
@@ -121,68 +195,93 @@
                 raise exception.MissingConfigOptionException(
                     "aprs_network.host is not set.",
                 )
 
             return True
         return True
 
+    def _is_stale_connection(self):
+        delta = datetime.datetime.now() - self._client.aprsd_keepalive
+        if delta > self.max_delta:
+            LOG.error(f"Connection is stale, last heard {delta} ago.")
+            return True
+
     def is_alive(self):
         if self._client:
-            return self._client.is_alive()
+            return self._client.is_alive() and not self._is_stale_connection()
         else:
+            LOG.warning(f"APRS_CLIENT {self._client} alive? NO!!!")
             return False
 
+    def close(self):
+        if self._client:
+            self._client.stop()
+            self._client.close()
+
     @staticmethod
     def transport():
         return TRANSPORT_APRSIS
 
     def decode_packet(self, *args, **kwargs):
         """APRS lib already decodes this."""
-        return core.Packet.factory(args[0])
+        return core.factory(args[0])
 
     def setup_connection(self):
         user = CONF.aprs_network.login
         password = CONF.aprs_network.password
         host = CONF.aprs_network.host
         port = CONF.aprs_network.port
-        connected = False
+        self.connected = False
         backoff = 1
         aprs_client = None
-        while not connected:
+        while not self.connected:
             try:
-                LOG.info("Creating aprslib client")
+                LOG.info(f"Creating aprslib client({host}:{port}) and logging in {user}.")
                 aprs_client = aprsis.Aprsdis(user, passwd=password, host=host, port=port)
                 # Force the log to be the same
                 aprs_client.logger = LOG
                 aprs_client.connect()
-                connected = True
+                self.connected = True
                 backoff = 1
             except LoginError as e:
                 LOG.error(f"Failed to login to APRS-IS Server '{e}'")
-                connected = False
+                self.connected = False
                 time.sleep(backoff)
             except Exception as e:
                 LOG.error(f"Unable to connect to APRS-IS server. '{e}' ")
-                connected = False
+                self.connected = False
                 time.sleep(backoff)
                 # Don't allow the backoff to go to inifinity.
                 if backoff > 5:
                     backoff = 5
                 else:
                     backoff += 1
                 continue
-        LOG.debug(f"Logging in to APRS-IS with user '{user}'")
         self._client = aprs_client
         return aprs_client
 
+    def consumer(self, callback, blocking=False, immortal=False, raw=False):
+        self._client.consumer(
+            callback, blocking=blocking,
+            immortal=immortal, raw=raw,
+        )
+
 
 class KISSClient(Client):
 
     _client = None
 
+    def stats(self) -> dict:
+        stats = {}
+        if self.is_configured():
+            return {
+                "transport": self.transport(),
+            }
+        return stats
+
     @staticmethod
     def is_enabled():
         """Return if tcp or serial KISS is enabled."""
         if CONF.kiss_serial.enabled:
             return True
 
         if CONF.kiss_tcp.enabled:
@@ -213,14 +312,18 @@
 
     def is_alive(self):
         if self._client:
             return self._client.is_alive()
         else:
             return False
 
+    def close(self):
+        if self._client:
+            self._client.stop()
+
     @staticmethod
     def transport():
         if CONF.kiss_serial.enabled:
             return TRANSPORT_SERIALKISS
 
         if CONF.kiss_tcp.enabled:
             return TRANSPORT_TCPKISS
@@ -234,41 +337,52 @@
         # frame.header._source._ch = False
         # payload = str(frame.payload.decode())
         # msg = f"{str(frame.header)}:{payload}"
         # msg = frame.tnc2
         # LOG.debug(f"Decoding {msg}")
 
         raw = aprslib.parse(str(frame))
-        packet = core.Packet.factory(raw)
+        packet = core.factory(raw)
         if isinstance(packet, core.ThirdParty):
             return packet.subpacket
         else:
             return packet
 
     def setup_connection(self):
         self._client = kiss.KISS3Client()
+        self.connected = True
         return self._client
 
+    def consumer(self, callback, blocking=False, immortal=False, raw=False):
+        self._client.consumer(callback)
+
 
 class APRSDFakeClient(Client, metaclass=trace.TraceWrapperMetaclass):
 
+    def stats(self) -> dict:
+        return {}
+
     @staticmethod
     def is_enabled():
         if CONF.fake_client.enabled:
             return True
         return False
 
     @staticmethod
     def is_configured():
         return APRSDFakeClient.is_enabled()
 
     def is_alive(self):
         return True
 
+    def close(self):
+        pass
+
     def setup_connection(self):
+        self.connected = True
         return fake.APRSDFakeClient()
 
     @staticmethod
     def transport():
         return TRANSPORT_FAKE
 
     def decode_packet(self, *args, **kwargs):
@@ -300,15 +414,14 @@
                 key = TRANSPORT_APRSIS
             elif KISSClient.is_enabled():
                 key = KISSClient.transport()
             elif APRSDFakeClient.is_enabled():
                 key = TRANSPORT_FAKE
 
         builder = self._builders.get(key)
-        LOG.debug(f"Creating client {key}")
         if not builder:
             raise ValueError(key)
         return builder()
 
     def is_client_enabled(self):
         """Make sure at least one client is enabled."""
         enabled = False
```

### Comparing `aprsd-3.3.4/aprsd/clients/aprsis.py` & `aprsd-3.4.0/aprsd/clients/aprsis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,36 @@
+import datetime
 import logging
 import select
 import threading
 
 import aprslib
 from aprslib import is_py3
 from aprslib.exceptions import (
     ConnectionDrop, ConnectionError, GenericError, LoginError, ParseError,
     UnknownFormat,
 )
 import wrapt
 
 import aprsd
-from aprsd import stats
 from aprsd.packets import core
 
 
 LOG = logging.getLogger("APRSD")
 
 
 class Aprsdis(aprslib.IS):
     """Extend the aprslib class so we can exit properly."""
 
     # flag to tell us to stop
     thread_stop = False
 
+    # date for last time we heard from the server
+    aprsd_keepalive = datetime.datetime.now()
+
     # timeout in seconds
     select_timeout = 1
     lock = threading.Lock()
 
     def stop(self):
         self.thread_stop = True
         LOG.info("Shutdown Aprsdis client.")
@@ -138,15 +141,14 @@
             if self.passwd == "-1":
                 self.logger.info("Login successful (receive only)")
             else:
                 self.logger.info("Login successful")
 
             self.logger.info(f"Connected to {server_string}")
             self.server_string = server_string
-            stats.APRSDStats().set_aprsis_server(server_string)
 
         except LoginError as e:
             self.logger.error(str(e))
             self.close()
             raise
         except Exception as e:
             self.close()
@@ -172,21 +174,22 @@
 
         line = b""
 
         while True and not self.thread_stop:
             try:
                 for line in self._socket_readlines(blocking):
                     if line[0:1] != b"#":
+                        self.aprsd_keepalive = datetime.datetime.now()
                         if raw:
                             callback(line)
                         else:
                             callback(self._parse(line))
                     else:
                         self.logger.debug("Server: %s", line.decode("utf8"))
-                        stats.APRSDStats().set_aprsis_keepalive()
+                        self.aprsd_keepalive = datetime.datetime.now()
             except ParseError as exp:
                 self.logger.log(
                     11,
                     "%s\n    Packet: %s",
                     exp,
                     exp.packet,
                 )
```

### Comparing `aprsd-3.3.4/aprsd/clients/fake.py` & `aprsd-3.4.0/aprsd/clients/fake.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,11 +63,11 @@
         )
 
     def consumer(self, callback, blocking=False, immortal=False, raw=False):
         LOG.debug("Start non blocking FAKE consumer")
         # Generate packets here?
         raw = "GTOWN>APDW16,WIDE1-1,WIDE2-1:}KM6LYW-9>APZ100,TCPIP,GTOWN*::KM6LYW   :KM6LYW: 19 Miles SW"
         pkt_raw = aprslib.parse(raw)
-        pkt = core.Packet.factory(pkt_raw)
+        pkt = core.factory(pkt_raw)
         callback(packet=pkt)
         LOG.debug(f"END blocking FAKE consumer {self}")
         time.sleep(8)
```

### Comparing `aprsd-3.3.4/aprsd/clients/kiss.py` & `aprsd-3.4.0/aprsd/clients/kiss.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                 "frame": frame,
             }
             self._parse_callback(**kwargs)
         except Exception as ex:
             LOG.error("Failed to parse bytes received from KISS interface.")
             LOG.exception(ex)
 
-    def consumer(self, callback, blocking=False, immortal=False, raw=False):
+    def consumer(self, callback):
         LOG.debug("Start blocking KISS consumer")
         self._parse_callback = callback
         self.kiss.read(callback=self.parse_frame, min_frames=None)
         LOG.debug(f"END blocking KISS consumer {self.kiss}")
 
     def send(self, packet):
         """Send an APRS Message object."""
```

### Comparing `aprsd-3.3.4/aprsd/cmds/dev.py` & `aprsd-3.4.0/aprsd/cmds/dev.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/cmds/fetch_stats.py` & `aprsd-3.4.0/aprsd/cmds/fetch_stats.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,160 +1,156 @@
-# Fetch active stats from a remote running instance of aprsd server
-# This uses the RPC server to fetch the stats from the remote server.
-
+# Fetch active stats from a remote running instance of aprsd admin web interface.
 import logging
 
 import click
 from oslo_config import cfg
+import requests
 from rich.console import Console
 from rich.table import Table
 
 # local imports here
 import aprsd
 from aprsd import cli_helper
 from aprsd.main import cli
-from aprsd.rpc import client as rpc_client
 
 
 # setup the global logger
 # log.basicConfig(level=log.DEBUG) # level=10
 LOG = logging.getLogger("APRSD")
 CONF = cfg.CONF
 
 
 @cli.command()
 @cli_helper.add_options(cli_helper.common_options)
 @click.option(
     "--host", type=str,
     default=None,
-    help="IP address of the remote aprsd server to fetch stats from.",
+    help="IP address of the remote aprsd admin web ui fetch stats from.",
 )
 @click.option(
     "--port", type=int,
     default=None,
-    help="Port of the remote aprsd server rpc port to fetch stats from.",
-)
-@click.option(
-    "--magic-word", type=str,
-    default=None,
-    help="Magic word of the remote aprsd server rpc port to fetch stats from.",
+    help="Port of the remote aprsd web admin interface to fetch stats from.",
 )
 @click.pass_context
 @cli_helper.process_standard_options
-def fetch_stats(ctx, host, port, magic_word):
-    """Fetch stats from a remote running instance of aprsd server."""
-    LOG.info(f"APRSD Fetch-Stats started version: {aprsd.__version__}")
+def fetch_stats(ctx, host, port):
+    """Fetch stats from a APRSD admin web interface."""
+    console = Console()
+    console.print(f"APRSD Fetch-Stats started version: {aprsd.__version__}")
 
     CONF.log_opt_values(LOG, logging.DEBUG)
     if not host:
-        host = CONF.rpc_settings.ip
+        host = CONF.admin.web_ip
     if not port:
-        port = CONF.rpc_settings.port
-    if not magic_word:
-        magic_word = CONF.rpc_settings.magic_word
+        port = CONF.admin.web_port
 
-    msg = f"Fetching stats from {host}:{port} with magic word '{magic_word}'"
-    console = Console()
+    msg = f"Fetching stats from {host}:{port}"
     console.print(msg)
     with console.status(msg):
-        client = rpc_client.RPCClient(host, port, magic_word)
-        stats = client.get_stats_dict()
-        if stats:
-            console.print_json(data=stats)
-        else:
-            LOG.error(f"Failed to fetch stats via RPC aprsd server at {host}:{port}")
+        response = requests.get(f"http://{host}:{port}/stats", timeout=120)
+        if not response:
+            console.print(
+                f"Failed to fetch stats from {host}:{port}?",
+                style="bold red",
+            )
             return
+
+        stats = response.json()
+        if not stats:
+            console.print(
+                f"Failed to fetch stats from aprsd admin ui at {host}:{port}",
+                style="bold red",
+            )
+            return
+
     aprsd_title = (
         "APRSD "
-        f"[bold cyan]v{stats['aprsd']['version']}[/] "
-        f"Callsign [bold green]{stats['aprsd']['callsign']}[/] "
-        f"Uptime [bold yellow]{stats['aprsd']['uptime']}[/]"
+        f"[bold cyan]v{stats['APRSDStats']['version']}[/] "
+        f"Callsign [bold green]{stats['APRSDStats']['callsign']}[/] "
+        f"Uptime [bold yellow]{stats['APRSDStats']['uptime']}[/]"
     )
 
-    console.rule(f"Stats from {host}:{port} with magic word '{magic_word}'")
+    console.rule(f"Stats from {host}:{port}")
     console.print("\n\n")
     console.rule(aprsd_title)
 
     # Show the connection to APRS
     # It can be a connection to an APRS-IS server or a local TNC via KISS or KISSTCP
     if "aprs-is" in stats:
-        title = f"APRS-IS Connection {stats['aprs-is']['server']}"
+        title = f"APRS-IS Connection {stats['APRSClientStats']['server_string']}"
         table = Table(title=title)
         table.add_column("Key")
         table.add_column("Value")
-        for key, value in stats["aprs-is"].items():
+        for key, value in stats["APRSClientStats"].items():
             table.add_row(key, value)
         console.print(table)
 
     threads_table = Table(title="Threads")
     threads_table.add_column("Name")
     threads_table.add_column("Alive?")
-    for name, alive in stats["aprsd"]["threads"].items():
+    for name, alive in stats["APRSDThreadList"].items():
         threads_table.add_row(name, str(alive))
 
     console.print(threads_table)
 
-    msgs_table = Table(title="Messages")
-    msgs_table.add_column("Key")
-    msgs_table.add_column("Value")
-    for key, value in stats["messages"].items():
-        msgs_table.add_row(key, str(value))
-
-    console.print(msgs_table)
-
     packet_totals = Table(title="Packet Totals")
     packet_totals.add_column("Key")
     packet_totals.add_column("Value")
-    packet_totals.add_row("Total Received", str(stats["packets"]["total_received"]))
-    packet_totals.add_row("Total Sent", str(stats["packets"]["total_sent"]))
-    packet_totals.add_row("Total Tracked", str(stats["packets"]["total_tracked"]))
+    packet_totals.add_row("Total Received", str(stats["PacketList"]["rx"]))
+    packet_totals.add_row("Total Sent", str(stats["PacketList"]["tx"]))
     console.print(packet_totals)
 
     # Show each of the packet types
     packets_table = Table(title="Packets By Type")
     packets_table.add_column("Packet Type")
     packets_table.add_column("TX")
     packets_table.add_column("RX")
-    for key, value in stats["packets"]["by_type"].items():
+    for key, value in stats["PacketList"]["packets"].items():
         packets_table.add_row(key, str(value["tx"]), str(value["rx"]))
 
     console.print(packets_table)
 
     if "plugins" in stats:
-        count = len(stats["plugins"])
+        count = len(stats["PluginManager"])
         plugins_table = Table(title=f"Plugins ({count})")
         plugins_table.add_column("Plugin")
         plugins_table.add_column("Enabled")
         plugins_table.add_column("Version")
         plugins_table.add_column("TX")
         plugins_table.add_column("RX")
-        for key, value in stats["plugins"].items():
+        plugins = stats["PluginManager"]
+        for key, value in plugins.items():
             plugins_table.add_row(
                 key,
-                str(stats["plugins"][key]["enabled"]),
-                stats["plugins"][key]["version"],
-                str(stats["plugins"][key]["tx"]),
-                str(stats["plugins"][key]["rx"]),
+                str(plugins[key]["enabled"]),
+                plugins[key]["version"],
+                str(plugins[key]["tx"]),
+                str(plugins[key]["rx"]),
             )
 
         console.print(plugins_table)
 
-    if "seen_list" in stats["aprsd"]:
-        count = len(stats["aprsd"]["seen_list"])
+    seen_list = stats.get("SeenList")
+
+    if seen_list:
+        count = len(seen_list)
         seen_table = Table(title=f"Seen List ({count})")
         seen_table.add_column("Callsign")
         seen_table.add_column("Message Count")
         seen_table.add_column("Last Heard")
-        for key, value in stats["aprsd"]["seen_list"].items():
+        for key, value in seen_list.items():
             seen_table.add_row(key, str(value["count"]), value["last"])
 
         console.print(seen_table)
 
-    if "watch_list" in stats["aprsd"]:
-        count = len(stats["aprsd"]["watch_list"])
+    watch_list = stats.get("WatchList")
+
+    if watch_list:
+        count = len(watch_list)
         watch_table = Table(title=f"Watch List ({count})")
         watch_table.add_column("Callsign")
         watch_table.add_column("Last Heard")
-        for key, value in stats["aprsd"]["watch_list"].items():
+        for key, value in watch_list.items():
             watch_table.add_row(key, value["last"])
 
         console.print(watch_table)
```

### Comparing `aprsd-3.3.4/aprsd/cmds/list_plugins.py` & `aprsd-3.4.0/aprsd/cmds/list_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from rich.text import Text
 from thesmuggler import smuggle
 
 from aprsd import cli_helper
 from aprsd import plugin as aprsd_plugin
 from aprsd.main import cli
 from aprsd.plugins import (
-    email, fortune, location, notify, ping, query, time, version, weather,
+    email, fortune, location, notify, ping, time, version, weather,
 )
 
 
 LOG = logging.getLogger("APRSD")
 PYPI_URL = "https://pypi.org/search/"
 
 
@@ -118,15 +118,15 @@
 def get_installed_extensions():
     # installed plugins
     plugins, extensions = _get_installed_aprsd_items()
     return extensions
 
 
 def show_built_in_plugins(console):
-    modules = [email, fortune, location, notify, ping, query, time, version, weather]
+    modules = [email, fortune, location, notify, ping, time, version, weather]
     plugins = []
 
     for module in modules:
         entries = inspect.getmembers(module, inspect.isclass)
         for entry in entries:
             cls = entry[1]
             if issubclass(cls, aprsd_plugin.APRSDPluginBase):
```

### Comparing `aprsd-3.3.4/aprsd/cmds/listen.py` & `aprsd-3.4.0/aprsd/cmds/listen.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,18 +11,22 @@
 
 import click
 from oslo_config import cfg
 from rich.console import Console
 
 # local imports here
 import aprsd
-from aprsd import cli_helper, client, packets, plugin, stats, threads
+from aprsd import cli_helper, client, packets, plugin, threads
 from aprsd.main import cli
-from aprsd.rpc import server as rpc_server
-from aprsd.threads import rx
+from aprsd.packets import collector as packet_collector
+from aprsd.packets import log as packet_log
+from aprsd.packets import seen_list
+from aprsd.stats import collector
+from aprsd.threads import keep_alive, rx
+from aprsd.threads import stats as stats_thread
 
 
 # setup the global logger
 # log.basicConfig(level=log.DEBUG) # level=10
 LOG = logging.getLogger("APRSD")
 CONF = cfg.CONF
 console = Console()
@@ -33,15 +37,15 @@
     if "subprocess" not in str(frame):
         LOG.info(
             "Ctrl+C, Sending all threads exit! Can take up to 10 seconds {}".format(
                 datetime.datetime.now(),
             ),
         )
         time.sleep(5)
-        LOG.info(stats.APRSDStats())
+        LOG.info(collector.Collector().collect())
 
 
 class APRSDListenThread(rx.APRSDRXThread):
     def __init__(self, packet_queue, packet_filter=None, plugin_manager=None):
         super().__init__(packet_queue)
         self.packet_filter = packet_filter
         self.plugin_manager = plugin_manager
@@ -49,37 +53,41 @@
             LOG.info(f"Plugins {self.plugin_manager.get_message_plugins()}")
 
     def process_packet(self, *args, **kwargs):
         packet = self._client.decode_packet(*args, **kwargs)
         filters = {
             packets.Packet.__name__: packets.Packet,
             packets.AckPacket.__name__: packets.AckPacket,
+            packets.BeaconPacket.__name__: packets.BeaconPacket,
             packets.GPSPacket.__name__: packets.GPSPacket,
             packets.MessagePacket.__name__: packets.MessagePacket,
             packets.MicEPacket.__name__: packets.MicEPacket,
+            packets.ObjectPacket.__name__: packets.ObjectPacket,
+            packets.StatusPacket.__name__: packets.StatusPacket,
+            packets.ThirdPartyPacket.__name__: packets.ThirdPartyPacket,
             packets.WeatherPacket.__name__: packets.WeatherPacket,
+            packets.UnknownPacket.__name__: packets.UnknownPacket,
         }
 
         if self.packet_filter:
             filter_class = filters[self.packet_filter]
             if isinstance(packet, filter_class):
-                packet.log(header="RX")
+                packet_log.log(packet)
                 if self.plugin_manager:
                     # Don't do anything with the reply
                     # This is the listen only command.
                     self.plugin_manager.run(packet)
         else:
+            packet_log.log(packet)
             if self.plugin_manager:
                 # Don't do anything with the reply.
                 # This is the listen only command.
                 self.plugin_manager.run(packet)
-            else:
-                packet.log(header="RX")
 
-        packets.PacketList().rx(packet)
+        packet_collector.PacketCollector().rx(packet)
 
 
 @cli.command()
 @cli_helper.add_options(cli_helper.common_options)
 @click.option(
     "--aprs-login",
     envvar="APRS_LOGIN",
@@ -92,19 +100,24 @@
     show_envvar=True,
     help="the APRS-IS password for APRS_LOGIN",
 )
 @click.option(
     "--packet-filter",
     type=click.Choice(
         [
-            packets.Packet.__name__,
             packets.AckPacket.__name__,
+            packets.BeaconPacket.__name__,
             packets.GPSPacket.__name__,
             packets.MicEPacket.__name__,
             packets.MessagePacket.__name__,
+            packets.ObjectPacket.__name__,
+            packets.RejectPacket.__name__,
+            packets.StatusPacket.__name__,
+            packets.ThirdPartyPacket.__name__,
+            packets.UnknownPacket.__name__,
             packets.WeatherPacket.__name__,
         ],
         case_sensitive=False,
     ),
     help="Filter by packet type",
 )
 @click.option(
@@ -155,14 +168,15 @@
 
     # CONF.aprs_network.login = aprs_login
     # config["aprs"]["password"] = aprs_password
 
     LOG.info(f"APRSD Listen Started version: {aprsd.__version__}")
 
     CONF.log_opt_values(LOG, logging.DEBUG)
+    collector.Collector()
 
     # Try and load saved MsgTrack list
     LOG.debug("Loading saved MsgTrack object.")
 
     # Initialize the client factory and create
     # The correct client object ready for use
     client.ClientFactory.setup()
@@ -175,40 +189,42 @@
     LOG.info("Creating client connection")
     aprs_client = client.factory.create()
     LOG.info(aprs_client)
 
     LOG.debug(f"Filter by '{filter}'")
     aprs_client.set_filter(filter)
 
-    keepalive = threads.KeepAliveThread()
-    keepalive.start()
+    keepalive = keep_alive.KeepAliveThread()
+    # keepalive.start()
 
-    if CONF.rpc_settings.enabled:
-        rpc = rpc_server.APRSDRPCThread()
-        rpc.start()
+    if not CONF.enable_seen_list:
+        # just deregister the class from the packet collector
+        packet_collector.PacketCollector().unregister(seen_list.SeenList)
 
     pm = None
     pm = plugin.PluginManager()
     if load_plugins:
         LOG.info("Loading plugins")
         pm.setup_plugins(load_help_plugin=False)
     else:
         LOG.warning(
             "Not Loading any plugins use --load-plugins to load what's "
             "defined in the config file.",
         )
+    stats = stats_thread.APRSDStatsStoreThread()
+    stats.start()
 
     LOG.debug("Create APRSDListenThread")
     listen_thread = APRSDListenThread(
         packet_queue=threads.packet_queue,
         packet_filter=packet_filter,
         plugin_manager=pm,
     )
     LOG.debug("Start APRSDListenThread")
     listen_thread.start()
+
+    keepalive.start()
     LOG.debug("keepalive Join")
     keepalive.join()
     LOG.debug("listen_thread Join")
     listen_thread.join()
-
-    if CONF.rpc_settings.enabled:
-        rpc.join()
+    stats.join()
```

### Comparing `aprsd-3.3.4/aprsd/cmds/send_message.py` & `aprsd-3.4.0/aprsd/cmds/send_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import click
 from oslo_config import cfg
 
 import aprsd
 from aprsd import cli_helper, client, packets
 from aprsd import conf  # noqa : F401
 from aprsd.main import cli
+from aprsd.packets import collector
 from aprsd.threads import tx
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 
 
@@ -72,15 +73,14 @@
             click.echo("Must set --aprs_login or APRS_LOGIN")
             ctx.exit(-1)
             return
         else:
             aprs_login = CONF.aprs_network.login
 
     if not aprs_password:
-        LOG.warning(CONF.aprs_network.password)
         if not CONF.aprs_network.password:
             click.echo("Must set --aprs-password or APRS_PASSWORD")
             ctx.exit(-1)
             return
         else:
             aprs_password = CONF.aprs_network.password
 
@@ -100,15 +100,15 @@
     got_ack = False
     got_response = False
 
     def rx_packet(packet):
         global got_ack, got_response
         cl = client.factory.create()
         packet = cl.decode_packet(packet)
-        packets.PacketList().rx(packet)
+        collector.PacketCollector().rx(packet)
         packet.log("RX")
         # LOG.debug("Got packet back {}".format(packet))
         if isinstance(packet, packets.AckPacket):
             got_ack = True
         else:
             got_response = True
             from_call = packet.from_call
```

### Comparing `aprsd-3.3.4/aprsd/cmds/server.py` & `aprsd-3.4.0/aprsd/cmds/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 from oslo_config import cfg
 
 import aprsd
 from aprsd import cli_helper, client
 from aprsd import main as aprsd_main
 from aprsd import packets, plugin, threads, utils
 from aprsd.main import cli
-from aprsd.rpc import server as rpc_server
-from aprsd.threads import registry, rx, tx
+from aprsd.packets import collector as packet_collector
+from aprsd.packets import seen_list
+from aprsd.threads import keep_alive, log_monitor, registry, rx
+from aprsd.threads import stats as stats_thread
+from aprsd.threads import tx
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 
 
 # main() ###
@@ -43,14 +46,22 @@
     else:
         LOG.info(msg)
     LOG.info(f"APRSD Started version: {aprsd.__version__}")
 
     # Initialize the client factory and create
     # The correct client object ready for use
     client.ClientFactory.setup()
+    if not client.factory.is_client_enabled():
+        LOG.error("No Clients are enabled in config.")
+        sys.exit(-1)
+
+    # Creates the client object
+    LOG.info("Creating client connection")
+    aprs_client = client.factory.create()
+    LOG.info(aprs_client)
 
     # Create the initial PM singleton and Register plugins
     # We register plugins first here so we can register each
     # plugins config options, so we can dump them all in the
     # log file output.
     LOG.info("Loading Plugin Manager and registering plugins")
     plugin_manager = plugin.PluginManager()
@@ -83,47 +94,53 @@
     # Now load the msgTrack from disk if any
     packets.PacketList()
     if flush:
         LOG.debug("Deleting saved MsgTrack.")
         packets.PacketTrack().flush()
         packets.WatchList().flush()
         packets.SeenList().flush()
+        packets.PacketList().flush()
     else:
         # Try and load saved MsgTrack list
         LOG.debug("Loading saved MsgTrack object.")
         packets.PacketTrack().load()
         packets.WatchList().load()
         packets.SeenList().load()
+        packets.PacketList().load()
 
-    keepalive = threads.KeepAliveThread()
+    keepalive = keep_alive.KeepAliveThread()
     keepalive.start()
 
+    if not CONF.enable_seen_list:
+        # just deregister the class from the packet collector
+        packet_collector.PacketCollector().unregister(seen_list.SeenList)
+
+    stats_store_thread = stats_thread.APRSDStatsStoreThread()
+    stats_store_thread.start()
+
     rx_thread = rx.APRSDPluginRXThread(
         packet_queue=threads.packet_queue,
     )
     process_thread = rx.APRSDPluginProcessPacketThread(
         packet_queue=threads.packet_queue,
     )
     rx_thread.start()
     process_thread.start()
 
-    packets.PacketTrack().restart()
     if CONF.enable_beacon:
         LOG.info("Beacon Enabled.  Starting Beacon thread.")
         bcn_thread = tx.BeaconSendThread()
         bcn_thread.start()
 
     if CONF.aprs_registry.enabled:
         LOG.info("Registry Enabled.  Starting Registry thread.")
         registry_thread = registry.APRSRegistryThread()
         registry_thread.start()
 
-    if CONF.rpc_settings.enabled:
-        rpc = rpc_server.APRSDRPCThread()
-        rpc.start()
-        log_monitor = threads.log_monitor.LogMonitorThread()
-        log_monitor.start()
+    if CONF.admin.web_enabled:
+        log_monitor_thread = log_monitor.LogMonitorThread()
+        log_monitor_thread.start()
 
     rx_thread.join()
     process_thread.join()
 
     return 0
```

### Comparing `aprsd-3.3.4/aprsd/cmds/webchat.py` & `aprsd-3.4.0/aprsd/cmds/webchat.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,38 +3,36 @@
 import logging
 import math
 import signal
 import sys
 import threading
 import time
 
-from aprslib import util as aprslib_util
 import click
 import flask
 from flask import request
 from flask_httpauth import HTTPBasicAuth
 from flask_socketio import Namespace, SocketIO
 from geopy.distance import geodesic
 from oslo_config import cfg
 from werkzeug.security import check_password_hash, generate_password_hash
 import wrapt
 
 import aprsd
 from aprsd import (
     cli_helper, client, packets, plugin_utils, stats, threads, utils,
 )
-from aprsd.log import log
 from aprsd.main import cli
 from aprsd.threads import aprsd as aprsd_threads
-from aprsd.threads import rx, tx
+from aprsd.threads import keep_alive, rx, tx
 from aprsd.utils import trace
 
 
 CONF = cfg.CONF
-LOG = logging.getLogger("APRSD")
+LOG = logging.getLogger()
 auth = HTTPBasicAuth()
 users = {}
 socketio = None
 
 # List of callsigns that we don't want to track/fetch their location
 callsign_no_track = [
     "REPEAT", "WB4BOR-11", "APDW16", "WXNOW", "WXBOT", "BLN0", "BLN1", "BLN2",
@@ -61,15 +59,15 @@
         f"Can take up to 10 seconds {datetime.datetime.now()}",
     )
     threads.APRSDThreadList().stop_all()
     if "subprocess" not in str(frame):
         time.sleep(1.5)
         # packets.WatchList().save()
         # packets.SeenList().save()
-        LOG.info(stats.APRSDStats())
+        LOG.info(stats.stats_collector.collect())
         LOG.info("Telling flask to bail.")
         signal.signal(signal.SIGTERM, sys.exit(0))
 
 
 class SentMessages:
 
     _instance = None
@@ -331,15 +329,14 @@
                 "ack", msg,
                 namespace="/sendmsg",
             )
         self.got_ack = True
 
     def process_our_message_packet(self, packet: packets.MessagePacket):
         global callsign_locations
-        LOG.info(f"process MessagePacket {repr(packet)}")
         # ok lets see if we have the location for the
         # person we just sent a message to.
         from_call = packet.get("from_call").upper()
         if from_call == "REPEAT":
             # We got a message from REPEAT.  Is this a location message?
             message = packet.get("message_text")
             if message.startswith("^ld^"):
@@ -377,15 +374,15 @@
 
 
 def _get_transport(stats):
     if CONF.aprs_network.enabled:
         transport = "aprs-is"
         aprs_connection = (
             "APRS-IS Server: <a href='http://status.aprs2.net' >"
-            "{}</a>".format(stats["stats"]["aprs-is"]["server"])
+            "{}</a>".format(stats["APRSClientStats"]["server_string"])
         )
     elif client.KISSClient.is_enabled():
         transport = client.KISSClient.transport()
         if transport == client.TRANSPORT_TCPKISS:
             aprs_connection = (
                 "TCPKISS://{}:{}".format(
                     CONF.kiss_tcp.host,
@@ -418,15 +415,15 @@
 def index():
     stats = _stats()
 
     # For development
     html_template = "index.html"
     LOG.debug(f"Template {html_template}")
 
-    transport, aprs_connection = _get_transport(stats)
+    transport, aprs_connection = _get_transport(stats["stats"])
     LOG.debug(f"transport {transport} aprs_connection {aprs_connection}")
 
     stats["transport"] = transport
     stats["aprs_connection"] = aprs_connection
     LOG.debug(f"initial stats = {stats}")
     latitude = CONF.webchat.latitude
     if latitude:
@@ -453,35 +450,36 @@
     LOG.debug(request)
     msgs = SentMessages()
     info = msgs.get_all()
     return json.dumps(info)
 
 
 def _stats():
-    stats_obj = stats.APRSDStats()
     now = datetime.datetime.now()
 
     time_format = "%m-%d-%Y %H:%M:%S"
-    stats_dict = stats_obj.stats()
+    stats_dict = stats.stats_collector.collect(serializable=True)
     # Webchat doesnt need these
-    if "watch_list" in stats_dict["aprsd"]:
-        del stats_dict["aprsd"]["watch_list"]
-    if "seen_list" in stats_dict["aprsd"]:
-        del stats_dict["aprsd"]["seen_list"]
-    if "threads" in stats_dict["aprsd"]:
-        del stats_dict["aprsd"]["threads"]
-    # del stats_dict["email"]
-    # del stats_dict["plugins"]
-    # del stats_dict["messages"]
+    if "WatchList" in stats_dict:
+        del stats_dict["WatchList"]
+    if "SeenList" in stats_dict:
+        del stats_dict["SeenList"]
+    if "APRSDThreadList" in stats_dict:
+        del stats_dict["APRSDThreadList"]
+    if "PacketList" in stats_dict:
+        del stats_dict["PacketList"]
+    if "EmailStats" in stats_dict:
+        del stats_dict["EmailStats"]
+    if "PluginManager" in stats_dict:
+        del stats_dict["PluginManager"]
 
     result = {
         "time": now.strftime(time_format),
         "stats": stats_dict,
     }
-
     return result
 
 
 @flask_app.route("/stats")
 def get_stats():
     return json.dumps(_stats())
 
@@ -537,26 +535,35 @@
         socketio.emit(
             "sent", obj,
             namespace="/sendmsg",
         )
 
     def on_gps(self, data):
         LOG.debug(f"WS on_GPS: {data}")
-        lat = aprslib_util.latitude_to_ddm(data["latitude"])
-        long = aprslib_util.longitude_to_ddm(data["longitude"])
-        LOG.debug(f"Lat DDM {lat}")
-        LOG.debug(f"Long DDM {long}")
+        lat = data["latitude"]
+        long = data["longitude"]
+        LOG.debug(f"Lat {lat}")
+        LOG.debug(f"Long {long}")
+        path = data.get("path", None)
+        if not path:
+            path = []
+        elif "," in path:
+            path_opts = path.split(",")
+            path = [x.strip() for x in path_opts]
+        else:
+            path = [path]
 
         tx.send(
-            packets.GPSPacket(
+            packets.BeaconPacket(
                 from_call=CONF.callsign,
                 to_call="APDW16",
                 latitude=lat,
                 longitude=long,
                 comment="APRSD WebChat Beacon",
+                path=path,
             ),
             direct=True,
         )
 
     def handle_message(self, data):
         LOG.debug(f"WS Data {data}")
 
@@ -568,16 +575,14 @@
         populate_callsign_location(data["callsign"])
 
 
 @trace.trace
 def init_flask(loglevel, quiet):
     global socketio, flask_app
 
-    log.setup_logging(loglevel, quiet)
-
     socketio = SocketIO(
         flask_app, logger=False, engineio_logger=False,
         async_mode="threading",
     )
 
     socketio.on_namespace(
         SendMessageNamespace(
@@ -620,15 +625,15 @@
     level, msg = utils._check_version()
     if level:
         LOG.warning(msg)
     else:
         LOG.info(msg)
     LOG.info(f"APRSD Started version: {aprsd.__version__}")
 
-    CONF.log_opt_values(LOG, logging.DEBUG)
+    CONF.log_opt_values(logging.getLogger(), logging.DEBUG)
     user = CONF.admin.user
     users[user] = generate_password_hash(CONF.admin.password)
     if not port:
         port = CONF.webchat.web_port
 
     # Initialize the client factory and create
     # The correct client object ready for use
@@ -643,15 +648,15 @@
         sys.exit(-1)
 
     packets.PacketList()
     packets.PacketTrack()
     packets.WatchList()
     packets.SeenList()
 
-    keepalive = threads.KeepAliveThread()
+    keepalive = keep_alive.KeepAliveThread()
     LOG.info("Start KeepAliveThread")
     keepalive.start()
 
     socketio = init_flask(loglevel, quiet)
     rx_thread = rx.APRSDPluginRXThread(
         packet_queue=threads.packet_queue,
     )
```

### Comparing `aprsd-3.3.4/aprsd/conf/__init__.py` & `aprsd-3.4.0/aprsd/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/conf/client.py` & `aprsd-3.4.0/aprsd/conf/client.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/conf/common.py` & `aprsd-3.4.0/aprsd/conf/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,18 +11,14 @@
     name="admin",
     title="Admin web interface settings",
 )
 watch_list_group = cfg.OptGroup(
     name="watch_list",
     title="Watch List settings",
 )
-rpc_group = cfg.OptGroup(
-    name="rpc_settings",
-    title="RPC Settings for admin <--> web",
-)
 webchat_group = cfg.OptGroup(
     name="webchat",
     title="Settings specific to the webchat command",
 )
 
 registry_group = cfg.OptGroup(
     name="aprs_registry",
@@ -97,14 +93,53 @@
         help="Latitude for the GPS Beacon button.  If not set, the button will not be enabled.",
     ),
     cfg.StrOpt(
         "longitude",
         default=None,
         help="Longitude for the GPS Beacon button.  If not set, the button will not be enabled.",
     ),
+    cfg.StrOpt(
+        "log_packet_format",
+        choices=["compact", "multiline", "both"],
+        default="compact",
+        help="When logging packets 'compact' will use a single line formatted for each packet."
+             "'multiline' will use multiple lines for each packet and is the traditional format."
+             "both will log both compact and multiline.",
+    ),
+    cfg.IntOpt(
+        "default_packet_send_count",
+        default=3,
+        help="The number of times to send a non ack packet before giving up.",
+    ),
+    cfg.IntOpt(
+        "default_ack_send_count",
+        default=3,
+        help="The number of times to send an ack packet in response to recieving a packet.",
+    ),
+    cfg.IntOpt(
+        "packet_list_maxlen",
+        default=100,
+        help="The maximum number of packets to store in the packet list.",
+    ),
+    cfg.IntOpt(
+        "packet_list_stats_maxlen",
+        default=20,
+        help="The maximum number of packets to send in the stats dict for admin ui.",
+    ),
+    cfg.BoolOpt(
+        "enable_seen_list",
+        default=True,
+        help="Enable the Callsign seen list tracking feature.  This allows aprsd to keep track of "
+             "callsigns that have been seen and when they were last seen.",
+    ),
+    cfg.BoolOpt(
+        "enable_packet_logging",
+        default=True,
+        help="Set this to False, to disable logging of packets to the log file.",
+    ),
 ]
 
 watch_list_opts = [
     cfg.BoolOpt(
         "enabled",
         default=False,
         help="Enable the watch list feature.  Still have to enable "
@@ -134,15 +169,15 @@
 
 admin_opts = [
     cfg.BoolOpt(
         "web_enabled",
         default=False,
         help="Enable the Admin Web Interface",
     ),
-    cfg.IPOpt(
+    cfg.StrOpt(
         "web_ip",
         default="0.0.0.0",
         help="The ip address to listen on",
     ),
     cfg.PortOpt(
         "web_port",
         default=8001,
@@ -157,36 +192,14 @@
         "password",
         default="password",
         secret=True,
         help="Admin interface password",
     ),
 ]
 
-rpc_opts = [
-    cfg.BoolOpt(
-        "enabled",
-        default=True,
-        help="Enable RPC calls",
-    ),
-    cfg.StrOpt(
-        "ip",
-        default="localhost",
-        help="The ip address to listen on",
-    ),
-    cfg.PortOpt(
-        "port",
-        default=18861,
-        help="The port to listen on",
-    ),
-    cfg.StrOpt(
-        "magic_word",
-        default=APRSD_DEFAULT_MAGIC_WORD,
-        help="Magic word to authenticate requests between client/server",
-    ),
-]
 
 enabled_plugins_opts = [
     cfg.ListOpt(
         "enabled_plugins",
         default=[
             "aprsd.plugins.email.EmailPlugin",
             "aprsd.plugins.fortune.FortunePlugin",
@@ -201,15 +214,15 @@
         help="Comma separated list of enabled plugins for APRSD."
              "To enable installed external plugins add them here."
              "The full python path to the class name must be used",
     ),
 ]
 
 webchat_opts = [
-    cfg.IPOpt(
+    cfg.StrOpt(
         "web_ip",
         default="0.0.0.0",
         help="The ip address to listen on",
     ),
     cfg.PortOpt(
         "web_port",
         default=8001,
@@ -221,14 +234,19 @@
         help="Latitude for the GPS Beacon button.  If not set, the button will not be enabled.",
     ),
     cfg.StrOpt(
         "longitude",
         default=None,
         help="Longitude for the GPS Beacon button.  If not set, the button will not be enabled.",
     ),
+    cfg.BoolOpt(
+        "disable_url_request_logging",
+        default=False,
+        help="Disable the logging of url requests in the webchat command.",
+    ),
 ]
 
 registry_opts = [
     cfg.BoolOpt(
         "enabled",
         default=False,
         help="Enable sending aprs registry information.  This will let the "
@@ -264,24 +282,21 @@
 def register_opts(config):
     config.register_opts(aprsd_opts)
     config.register_opts(enabled_plugins_opts)
     config.register_group(admin_group)
     config.register_opts(admin_opts, group=admin_group)
     config.register_group(watch_list_group)
     config.register_opts(watch_list_opts, group=watch_list_group)
-    config.register_group(rpc_group)
-    config.register_opts(rpc_opts, group=rpc_group)
     config.register_group(webchat_group)
     config.register_opts(webchat_opts, group=webchat_group)
     config.register_group(registry_group)
     config.register_opts(registry_opts, group=registry_group)
 
 
 def list_opts():
     return {
         "DEFAULT": (aprsd_opts + enabled_plugins_opts),
         admin_group.name: admin_opts,
         watch_list_group.name: watch_list_opts,
-        rpc_group.name: rpc_opts,
         webchat_group.name: webchat_opts,
         registry_group.name: registry_opts,
     }
```

### Comparing `aprsd-3.3.4/aprsd/conf/log.py` & `aprsd-3.4.0/aprsd/conf/log.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/conf/opts.py` & `aprsd-3.4.0/aprsd/conf/opts.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/conf/plugin_common.py` & `aprsd-3.4.0/aprsd/conf/plugin_common.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/conf/plugin_email.py` & `aprsd-3.4.0/aprsd/conf/plugin_email.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/log/log.py` & `aprsd-3.4.0/aprsd/log/log.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 from logging.handlers import QueueHandler
 import queue
 import sys
 
 from loguru import logger
 from oslo_config import cfg
 
-from aprsd import conf
+from aprsd.conf import log as conf_log
 
 
 CONF = cfg.CONF
-LOG = logging.getLogger("APRSD")
+# LOG = logging.getLogger("APRSD")
+LOG = logger
 logging_queue = queue.Queue()
 
 
 class InterceptHandler(logging.Handler):
     def emit(self, record):
         # get corresponding Loguru level if it exists
         try:
@@ -34,64 +35,85 @@
 # Setup the log faciility
 # to disable log to stdout, but still log to file
 # use the --quiet option on the cmdln
 def setup_logging(loglevel=None, quiet=False):
     if not loglevel:
         log_level = CONF.logging.log_level
     else:
-        log_level = conf.log.LOG_LEVELS[loglevel]
+        log_level = conf_log.LOG_LEVELS[loglevel]
 
     # intercept everything at the root logger
     logging.root.handlers = [InterceptHandler()]
     logging.root.setLevel(log_level)
 
     imap_list = [
         "imapclient.imaplib", "imaplib", "imapclient",
         "imapclient.util",
     ]
     aprslib_list = [
         "aprslib",
         "aprslib.parsing",
         "aprslib.exceptions",
     ]
+    webserver_list = [
+        "werkzeug",
+        "werkzeug._internal",
+        "socketio",
+        "urllib3.connectionpool",
+    ]
 
     # We don't really want to see the aprslib parsing debug output.
-    disable_list = imap_list + aprslib_list
+    disable_list = imap_list + aprslib_list + webserver_list
 
     # remove every other logger's handlers
     # and propagate to root logger
     for name in logging.root.manager.loggerDict.keys():
         logging.getLogger(name).handlers = []
         if name in disable_list:
             logging.getLogger(name).propagate = False
         else:
             logging.getLogger(name).propagate = True
 
+    if CONF.webchat.disable_url_request_logging:
+        for name in webserver_list:
+            logging.getLogger(name).handlers = []
+            logging.getLogger(name).propagate = True
+            logging.getLogger(name).setLevel(logging.ERROR)
+
     handlers = [
         {
-            "sink": sys.stdout, "serialize": False,
+            "sink": sys.stdout,
+            "serialize": False,
             "format": CONF.logging.logformat,
+            "colorize": True,
+            "level": log_level,
         },
     ]
     if CONF.logging.logfile:
         handlers.append(
             {
-                "sink": CONF.logging.logfile, "serialize": False,
+                "sink": CONF.logging.logfile,
+                "serialize": False,
                 "format": CONF.logging.logformat,
+                "colorize": False,
+                "level": log_level,
             },
         )
 
     if CONF.email_plugin.enabled and CONF.email_plugin.debug:
         for name in imap_list:
             logging.getLogger(name).propagate = True
 
     if CONF.admin.web_enabled:
         qh = QueueHandler(logging_queue)
         handlers.append(
             {
                 "sink": qh, "serialize": False,
                 "format": CONF.logging.logformat,
+                "level": log_level,
+                "colorize": False,
             },
         )
 
     # configure loguru
     logger.configure(handlers=handlers)
+    logger.level("DEBUG", color="<fg #BABABA>")
```

### Comparing `aprsd-3.3.4/aprsd/main.py` & `aprsd-3.4.0/aprsd/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,47 +20,33 @@
 #
 
 # python included libs
 import datetime
 import importlib.metadata as imp
 from importlib.metadata import version as metadata_version
 import logging
-import os
 import signal
 import sys
 import time
 
 import click
-import click_completion
 from oslo_config import cfg, generator
 
 # local imports here
 import aprsd
-from aprsd import cli_helper, packets, stats, threads, utils
+from aprsd import cli_helper, packets, threads, utils
+from aprsd.stats import collector
 
 
 # setup the global logger
 # log.basicConfig(level=log.DEBUG) # level=10
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 flask_enabled = False
-rpc_serv = None
-
-
-def custom_startswith(string, incomplete):
-    """A custom completion match that supports case insensitive matching."""
-    if os.environ.get("_CLICK_COMPLETION_COMMAND_CASE_INSENSITIVE_COMPLETE"):
-        string = string.lower()
-        incomplete = incomplete.lower()
-    return string.startswith(incomplete)
-
-
-click_completion.core.startswith = custom_startswith
-click_completion.init()
 
 
 @click.group(cls=cli_helper.AliasedGroup, context_settings=CONTEXT_SETTINGS)
 @click.version_option()
 @click.pass_context
 def cli(ctx):
     pass
@@ -92,15 +78,16 @@
                 datetime.datetime.now(),
             ),
         )
         time.sleep(1.5)
         packets.PacketTrack().save()
         packets.WatchList().save()
         packets.SeenList().save()
-        LOG.info(stats.APRSDStats())
+        packets.PacketList().save()
+        LOG.info(collector.Collector().collect())
         # signal.signal(signal.SIGTERM, sys.exit(0))
         # sys.exit(0)
 
     if flask_enabled:
         signal.signal(signal.SIGTERM, sys.exit(0))
```

### Comparing `aprsd-3.3.4/aprsd/packets/core.py` & `aprsd-3.4.0/aprsd/packets/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,44 @@
-import abc
-from dataclasses import asdict, dataclass, field
+from dataclasses import dataclass, field
 from datetime import datetime
 import logging
 import re
 import time
 # Due to a failure in python 3.8
-from typing import List
+from typing import Any, List, Optional, Type, TypeVar, Union
 
-import dacite
-from dataclasses_json import dataclass_json
+from aprslib import util as aprslib_util
+from dataclasses_json import (
+    CatchAll, DataClassJsonMixin, Undefined, dataclass_json,
+)
+from loguru import logger
 
 from aprsd.utils import counter
 
 
-LOG = logging.getLogger("APRSD")
+# For mypy to be happy
+A = TypeVar("A", bound="DataClassJsonMixin")
+Json = Union[dict, list, str, int, float, bool, None]
 
+LOG = logging.getLogger()
+LOGU = logger
+
+PACKET_TYPE_BULLETIN = "bulletin"
 PACKET_TYPE_MESSAGE = "message"
 PACKET_TYPE_ACK = "ack"
 PACKET_TYPE_REJECT = "reject"
 PACKET_TYPE_MICE = "mic-e"
-PACKET_TYPE_WX = "weather"
+PACKET_TYPE_WX = "wx"
+PACKET_TYPE_WEATHER = "weather"
 PACKET_TYPE_OBJECT = "object"
 PACKET_TYPE_UNKNOWN = "unknown"
 PACKET_TYPE_STATUS = "status"
 PACKET_TYPE_BEACON = "beacon"
 PACKET_TYPE_THIRDPARTY = "thirdparty"
+PACKET_TYPE_TELEMETRY = "telemetry-message"
 PACKET_TYPE_UNCOMPRESSED = "uncompressed"
 
 NO_DATE = datetime(1900, 10, 24)
 
 
 def _init_timestamp():
     """Build a unix style timestamp integer"""
@@ -48,483 +58,434 @@
     we use this workaround.
     """
     c = counter.PacketCounter()
     c.increment()
     return c.value
 
 
-def factory_from_dict(packet_dict):
-    pkt_type = get_packet_type(packet_dict)
-    if pkt_type:
-        cls = TYPE_LOOKUP[pkt_type]
-        return cls.from_dict(packet_dict)
-
+def _translate_fields(raw: dict) -> dict:
+    translate_fields = {
+        "from": "from_call",
+        "to": "to_call",
+    }
+    # First translate some fields
+    for key in translate_fields:
+        if key in raw:
+            raw[translate_fields[key]] = raw[key]
+            del raw[key]
+
+    # addresse overrides to_call
+    if "addresse" in raw:
+        raw["to_call"] = raw["addresse"]
 
-def factory_from_json(packet_dict):
-    pkt_type = get_packet_type(packet_dict)
-    if pkt_type:
-        return TYPE_LOOKUP[pkt_type].from_json(packet_dict)
+    return raw
 
 
 @dataclass_json
 @dataclass(unsafe_hash=True)
-class Packet(metaclass=abc.ABCMeta):
-    from_call: str = field(default=None)
-    to_call: str = field(default=None)
-    addresse: str = field(default=None)
-    format: str = field(default=None)
-    msgNo: str = field(default_factory=_init_msgNo)   # noqa: N815
-    packet_type: str = field(default=None)
+class Packet:
+    _type: str = field(default="Packet", hash=False)
+    from_call: Optional[str] = field(default=None)
+    to_call: Optional[str] = field(default=None)
+    addresse: Optional[str] = field(default=None)
+    format: Optional[str] = field(default=None)
+    msgNo: Optional[str] = field(default=None)   # noqa: N815
+    ackMsgNo: Optional[str] = field(default=None)   # noqa: N815
+    packet_type: Optional[str] = field(default=None)
     timestamp: float = field(default_factory=_init_timestamp, compare=False, hash=False)
     # Holds the raw text string to be sent over the wire
     # or holds the raw string from input packet
-    raw: str = field(default=None, compare=False, hash=False)
+    raw: Optional[str] = field(default=None, compare=False, hash=False)
     raw_dict: dict = field(repr=False, default_factory=lambda: {}, compare=False, hash=False)
     # Built by calling prepare().  raw needs this built first.
-    payload: str = field(default=None)
+    payload: Optional[str] = field(default=None)
 
     # Fields related to sending packets out
     send_count: int = field(repr=False, default=0, compare=False, hash=False)
     retry_count: int = field(repr=False, default=3, compare=False, hash=False)
-    # last_send_time: datetime = field(
-    #    metadata=dc_json_config(
-    #        encoder=datetime.isoformat,
-    #        decoder=datetime.fromisoformat,
-    #    ),
-    #    repr=True,
-    #    default_factory=_init_send_time,
-    #    compare=False,
-    #    hash=False
-    # )
     last_send_time: float = field(repr=False, default=0, compare=False, hash=False)
-    last_send_attempt: int = field(repr=False, default=0, compare=False, hash=False)
 
     # Do we allow this packet to be saved to send later?
     allow_delay: bool = field(repr=False, default=True, compare=False, hash=False)
     path: List[str] = field(default_factory=list, compare=False, hash=False)
-    via: str = field(default=None, compare=False, hash=False)
-
-    def __post__init__(self):
-        LOG.warning(f"POST INIT {self}")
+    via: Optional[str] = field(default=None, compare=False, hash=False)
 
-    @property
-    def json(self):
-        """
-        get the json formated string
-        """
-        return self.to_json()
-
-    def get(self, key, default=None):
+    def get(self, key: str, default: Optional[str] = None):
         """Emulate a getter on a dict."""
         if hasattr(self, key):
             return getattr(self, key)
         else:
             return default
 
     @property
-    def key(self):
+    def key(self) -> str:
         """Build a key for finding this packet in a dict."""
         return f"{self.from_call}:{self.addresse}:{self.msgNo}"
 
-    def update_timestamp(self):
+    def update_timestamp(self) -> None:
         self.timestamp = _init_timestamp()
 
-    def prepare(self):
+    @property
+    def human_info(self) -> str:
+        """Build a human readable string for this packet.
+
+        This doesn't include the from to and type, but just
+        the human readable payload.
+        """
+        self.prepare()
+        msg = self._filter_for_send(self.raw).rstrip("\n")
+        return msg
+
+    def prepare(self) -> None:
         """Do stuff here that is needed prior to sending over the air."""
         # now build the raw message for sending
+        if not self.msgNo:
+            self.msgNo = _init_msgNo()
         self._build_payload()
         self._build_raw()
 
-    def _build_payload(self):
+    def _build_payload(self) -> None:
         """The payload is the non headers portion of the packet."""
-        msg = self._filter_for_send().rstrip("\n")
+        if not self.to_call:
+            raise ValueError("to_call isn't set. Must set to_call before calling prepare()")
+
+        # The base packet class has no real payload
         self.payload = (
             f":{self.to_call.ljust(9)}"
-            f":{msg}"
         )
 
-    def _build_raw(self):
+    def _build_raw(self) -> None:
         """Build the self.raw which is what is sent over the air."""
         self.raw = "{}>APZ100:{}".format(
             self.from_call,
             self.payload,
         )
 
-    @staticmethod
-    def factory(raw_packet):
-        """Factory method to create a packet from a raw packet string."""
-        raw = raw_packet
-        raw["raw_dict"] = raw.copy()
-        translate_fields = {
-            "from": "from_call",
-            "to": "to_call",
-        }
-        # First translate some fields
-        for key in translate_fields:
-            if key in raw:
-                raw[translate_fields[key]] = raw[key]
-                del raw[key]
-
-        if "addresse" in raw:
-            raw["to_call"] = raw["addresse"]
-
-        packet_type = get_packet_type(raw)
-        raw["packet_type"] = packet_type
-        class_name = TYPE_LOOKUP[packet_type]
-        if packet_type == PACKET_TYPE_THIRDPARTY:
-            # We have an encapsulated packet!
-            # So we need to decode it and return the inner packet
-            # as the packet we are going to process.
-            # This is a recursive call to the factory
-            subpacket_raw = raw["subpacket"]
-            subpacket = Packet.factory(subpacket_raw)
-            del raw["subpacket"]
-            # raw["subpacket"] = subpacket
-            packet = dacite.from_dict(data_class=class_name, data=raw)
-            packet.subpacket = subpacket
-            return packet
-
-        if packet_type == PACKET_TYPE_UNKNOWN:
-            # Try and figure it out here
-            if "latitude" in raw:
-                class_name = GPSPacket
-
-        if packet_type == PACKET_TYPE_WX:
-            # the weather information is in a dict
-            # this brings those values out to the outer dict
-
-            for key in raw["weather"]:
-                raw[key] = raw["weather"][key]
-
-            # If we have the broken aprslib, then we need to
-            # Convert the course and speed to wind_speed and wind_direction
-            # aprslib issue #80
-            # https://github.com/rossengeorgiev/aprs-python/issues/80
-            # Wind speed and course is option in the SPEC.
-            # For some reason aprslib multiplies the speed by 1.852.
-            if "wind_speed" not in raw and "wind_direction" not in raw:
-                # Most likely this is the broken aprslib
-                # So we need to convert the wind_gust speed
-                raw["wind_gust"] = round(raw.get("wind_gust", 0) / 0.44704, 3)
-            if "wind_speed" not in raw:
-                wind_speed = raw.get("speed")
-                if wind_speed:
-                    raw["wind_speed"] = round(wind_speed / 1.852, 3)
-                    raw["weather"]["wind_speed"] = raw["wind_speed"]
-                if "speed" in raw:
-                    del raw["speed"]
-                # Let's adjust the rain numbers as well, since it's wrong
-                raw["rain_1h"] = round((raw.get("rain_1h", 0) / .254) * .01, 3)
-                raw["weather"]["rain_1h"] = raw["rain_1h"]
-                raw["rain_24h"] = round((raw.get("rain_24h", 0) / .254) * .01, 3)
-                raw["weather"]["rain_24h"] = raw["rain_24h"]
-                raw["rain_since_midnight"] = round((raw.get("rain_since_midnight", 0) / .254) * .01, 3)
-                raw["weather"]["rain_since_midnight"] = raw["rain_since_midnight"]
-
-            if "wind_direction" not in raw:
-                wind_direction = raw.get("course")
-                if wind_direction:
-                    raw["wind_direction"] = wind_direction
-                    raw["weather"]["wind_direction"] = raw["wind_direction"]
-                if "course" in raw:
-                    del raw["course"]
-
-        return dacite.from_dict(data_class=class_name, data=raw)
-
-    def log(self, header=None):
-        """LOG a packet to the logfile."""
-        asdict(self)
-        log_list = ["\n"]
-        name = self.__class__.__name__
-        if header:
-            if "tx" in header.lower():
-                log_list.append(
-                    f"{header}________({name}  "
-                    f"TX:{self.send_count+1} of {self.retry_count})",
-                )
-            else:
-                log_list.append(f"{header}________({name})")
-        # log_list.append(f"  Packet  : {self.__class__.__name__}")
-        log_list.append(f"  Raw     : {self.raw}")
-        if self.to_call:
-            log_list.append(f"  To      : {self.to_call}")
-        if self.from_call:
-            log_list.append(f"  From    : {self.from_call}")
-        if hasattr(self, "path") and self.path:
-            log_list.append(f"  Path    : {'=>'.join(self.path)}")
-        if hasattr(self, "via") and self.via:
-            log_list.append(f"  VIA     : {self.via}")
-
-        elif isinstance(self, MessagePacket):
-            log_list.append(f"  Message : {self.message_text}")
-
-        if hasattr(self, "comment") and self.comment:
-            log_list.append(f"  Comment : {self.comment}")
-
-        if self.msgNo:
-            log_list.append(f"  Msg #   : {self.msgNo}")
-        log_list.append(f"{header}________({name})")
-
-        LOG.info("\n".join(log_list))
-        LOG.debug(repr(self))
-
-    def _filter_for_send(self) -> str:
+    def _filter_for_send(self, msg) -> str:
         """Filter and format message string for FCC."""
         # max?  ftm400 displays 64, raw msg shows 74
         # and ftm400-send is max 64.  setting this to
         # 67 displays 64 on the ftm400. (+3 {01 suffix)
         # feature req: break long ones into two msgs
-        message = self.raw[:67]
+        if not msg:
+            return ""
+
+        message = msg[:67]
         # We all miss George Carlin
-        return re.sub("fuck|shit|cunt|piss|cock|bitch", "****", message)
+        return re.sub(
+            "fuck|shit|cunt|piss|cock|bitch", "****",
+            message, flags=re.IGNORECASE,
+        )
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Show the raw version of the packet"""
         self.prepare()
+        if not self.raw:
+            raise ValueError("self.raw is unset")
         return self.raw
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """Build the repr version of the packet."""
         repr = (
             f"{self.__class__.__name__}:"
             f" From: {self.from_call}  "
-            " To: "
+            f"   To: {self.to_call}"
         )
-
         return repr
 
 
+@dataclass_json
 @dataclass(unsafe_hash=True)
 class AckPacket(Packet):
-    response: str = field(default=None)
-
-    def __post__init__(self):
-        if self.response:
-            LOG.warning("Response set!")
+    _type: str = field(default="AckPacket", hash=False)
 
     def _build_payload(self):
-        self.payload = f":{self.to_call.ljust(9)}:ack{self.msgNo}"
+        self.payload = f":{self.to_call: <9}:ack{self.msgNo}"
 
 
+@dataclass_json
+@dataclass(unsafe_hash=True)
+class BulletinPacket(Packet):
+    _type: str = "BulletinPacket"
+    # Holds the encapsulated packet
+    bid: Optional[str] = field(default="1")
+    message_text: Optional[str] = field(default=None)
+
+    @property
+    def key(self) -> str:
+        """Build a key for finding this packet in a dict."""
+        return f"{self.from_call}:BLN{self.bid}"
+
+    @property
+    def human_info(self) -> str:
+        return f"BLN{self.bid} {self.message_text}"
+
+    def _build_payload(self) -> None:
+        self.payload = (
+            f":BLN{self.bid:<9}"
+            f":{self.message_text}"
+        )
+
+
+@dataclass_json
 @dataclass(unsafe_hash=True)
 class RejectPacket(Packet):
-    response: str = field(default=None)
+    _type: str = field(default="RejectPacket", hash=False)
+    response: Optional[str] = field(default=None)
 
     def __post__init__(self):
         if self.response:
             LOG.warning("Response set!")
 
     def _build_payload(self):
-        self.payload = f":{self.to_call.ljust(9)} :rej{self.msgNo}"
+        self.payload = f":{self.to_call: <9}:rej{self.msgNo}"
 
 
 @dataclass_json
 @dataclass(unsafe_hash=True)
 class MessagePacket(Packet):
-    message_text: str = field(default=None)
+    _type: str = field(default="MessagePacket", hash=False)
+    message_text: Optional[str] = field(default=None)
 
-    def _filter_for_send(self) -> str:
-        """Filter and format message string for FCC."""
-        # max?  ftm400 displays 64, raw msg shows 74
-        # and ftm400-send is max 64.  setting this to
-        # 67 displays 64 on the ftm400. (+3 {01 suffix)
-        # feature req: break long ones into two msgs
-        message = self.message_text[:67]
-        # We all miss George Carlin
-        return re.sub("fuck|shit|cunt|piss|cock|bitch", "****", message)
+    @property
+    def human_info(self) -> str:
+        self.prepare()
+        return self._filter_for_send(self.message_text).rstrip("\n")
 
     def _build_payload(self):
         self.payload = ":{}:{}{{{}".format(
             self.to_call.ljust(9),
-            self._filter_for_send().rstrip("\n"),
+            self._filter_for_send(self.message_text).rstrip("\n"),
             str(self.msgNo),
         )
 
 
+@dataclass_json
 @dataclass(unsafe_hash=True)
 class StatusPacket(Packet):
-    status: str = field(default=None)
+    _type: str = field(default="StatusPacket", hash=False)
+    status: Optional[str] = field(default=None)
     messagecapable: bool = field(default=False)
-    comment: str = field(default=None)
+    comment: Optional[str] = field(default=None)
+    raw_timestamp: Optional[str] = field(default=None)
 
     def _build_payload(self):
-        raise NotImplementedError
+        self.payload = ":{}:{}{{{}".format(
+            self.to_call.ljust(9),
+            self._filter_for_send(self.status).rstrip("\n"),
+            str(self.msgNo),
+        )
 
+    @property
+    def human_info(self) -> str:
+        self.prepare()
+        return self.status
 
+
+@dataclass_json
 @dataclass(unsafe_hash=True)
 class GPSPacket(Packet):
+    _type: str = field(default="GPSPacket", hash=False)
     latitude: float = field(default=0.00)
     longitude: float = field(default=0.00)
     altitude: float = field(default=0.00)
     rng: float = field(default=0.00)
     posambiguity: int = field(default=0)
-    comment: str = field(default=None)
+    messagecapable: bool = field(default=False)
+    comment: Optional[str] = field(default=None)
     symbol: str = field(default="l")
     symbol_table: str = field(default="/")
-
-    def decdeg2dms(self, degrees_decimal):
-        is_positive = degrees_decimal >= 0
-        degrees_decimal = abs(degrees_decimal)
-        minutes, seconds = divmod(degrees_decimal * 3600, 60)
-        degrees, minutes = divmod(minutes, 60)
-        degrees = degrees if is_positive else -degrees
-
-        degrees = str(int(degrees)).replace("-", "0")
-        minutes = str(int(minutes)).replace("-", "0")
-        seconds = str(int(round(seconds * 0.01, 2) * 100))
-
-        return {"degrees": degrees, "minutes": minutes, "seconds": seconds}
-
-    def decdeg2dmm_m(self, degrees_decimal):
-        is_positive = degrees_decimal >= 0
-        degrees_decimal = abs(degrees_decimal)
-        minutes, seconds = divmod(degrees_decimal * 3600, 60)
-        degrees, minutes = divmod(minutes, 60)
-        degrees = degrees if is_positive else -degrees
-
-        degrees = abs(int(degrees))
-        minutes = int(round(minutes + (seconds / 60), 2))
-        hundredths = round(seconds / 60, 2)
-
-        return {
-            "degrees": degrees, "minutes": minutes, "seconds": seconds,
-            "hundredths": hundredths,
-        }
-
-    def convert_latitude(self, degrees_decimal):
-        det = self.decdeg2dmm_m(degrees_decimal)
-        if degrees_decimal > 0:
-            direction = "N"
-        else:
-            direction = "S"
-
-        degrees = str(det.get("degrees")).zfill(2)
-        minutes = str(det.get("minutes")).zfill(2)
-        seconds = det.get("seconds")
-        hun = det.get("hundredths")
-        hundredths = f"{hun:.2f}".split(".")[1]
-
-        LOG.debug(
-            f"LAT degress {degrees}  minutes {str(minutes)} "
-            f"seconds {seconds} hundredths {hundredths} direction {direction}",
-        )
-
-        lat = f"{degrees}{str(minutes)}.{hundredths}{direction}"
-        return lat
-
-    def convert_longitude(self, degrees_decimal):
-        det = self.decdeg2dmm_m(degrees_decimal)
-        if degrees_decimal > 0:
-            direction = "E"
-        else:
-            direction = "W"
-
-        degrees = str(det.get("degrees")).zfill(3)
-        minutes = str(det.get("minutes")).zfill(2)
-        seconds = det.get("seconds")
-        hun = det.get("hundredths")
-        hundredths = f"{hun:.2f}".split(".")[1]
-
-        LOG.debug(
-            f"LON degress {degrees}  minutes {str(minutes)} "
-            f"seconds {seconds} hundredths {hundredths} direction {direction}",
-        )
-
-        lon = f"{degrees}{str(minutes)}.{hundredths}{direction}"
-        return lon
+    raw_timestamp: Optional[str] = field(default=None)
+    object_name: Optional[str] = field(default=None)
+    object_format: Optional[str] = field(default=None)
+    alive: Optional[bool] = field(default=None)
+    course: Optional[int] = field(default=None)
+    speed: Optional[float] = field(default=None)
+    phg: Optional[str] = field(default=None)
+    phg_power: Optional[int] = field(default=None)
+    phg_height: Optional[float] = field(default=None)
+    phg_gain: Optional[int] = field(default=None)
+    phg_dir: Optional[str] = field(default=None)
+    phg_range: Optional[float] = field(default=None)
+    phg_rate: Optional[int] = field(default=None)
+    # http://www.aprs.org/datum.txt
+    daodatumbyte: Optional[str] = field(default=None)
 
     def _build_time_zulu(self):
         """Build the timestamp in UTC/zulu."""
         if self.timestamp:
-            local_dt = datetime.fromtimestamp(self.timestamp)
-        else:
-            local_dt = datetime.now()
-            self.timestamp = datetime.timestamp(local_dt)
-
-        utc_offset_timedelta = datetime.utcnow() - local_dt
-        result_utc_datetime = local_dt + utc_offset_timedelta
-        time_zulu = result_utc_datetime.strftime("%d%H%M")
-        return time_zulu
+            return datetime.utcfromtimestamp(self.timestamp).strftime("%d%H%M")
 
     def _build_payload(self):
         """The payload is the non headers portion of the packet."""
         time_zulu = self._build_time_zulu()
-        lat = self.latitude
-        long = self.longitude
-        self.payload = (
-            f"@{time_zulu}z{lat}{self.symbol_table}"
-            f"{long}{self.symbol}"
-        )
+        lat = aprslib_util.latitude_to_ddm(self.latitude)
+        long = aprslib_util.longitude_to_ddm(self.longitude)
+        payload = [
+            "@" if self.timestamp else "!",
+            time_zulu,
+            lat,
+            self.symbol_table,
+            long,
+            self.symbol,
+        ]
 
         if self.comment:
-            self.payload = f"{self.payload}{self.comment}"
+            payload.append(self._filter_for_send(self.comment))
+
+        self.payload = "".join(payload)
 
     def _build_raw(self):
         self.raw = (
             f"{self.from_call}>{self.to_call},WIDE2-1:"
             f"{self.payload}"
         )
 
+    @property
+    def human_info(self) -> str:
+        h_str = []
+        h_str.append(f"Lat:{self.latitude:03.3f}")
+        h_str.append(f"Lon:{self.longitude:03.3f}")
+        if self.altitude:
+            h_str.append(f"Altitude {self.altitude:03.0f}")
+        if self.speed:
+            h_str.append(f"Speed {self.speed:03.0f}MPH")
+        if self.course:
+            h_str.append(f"Course {self.course:03.0f}")
+        if self.rng:
+            h_str.append(f"RNG {self.rng:03.0f}")
+        if self.phg:
+            h_str.append(f"PHG {self.phg}")
+
+        return " ".join(h_str)
 
+
+@dataclass_json
 @dataclass(unsafe_hash=True)
 class BeaconPacket(GPSPacket):
+    _type: str = field(default="BeaconPacket", hash=False)
+
     def _build_payload(self):
         """The payload is the non headers portion of the packet."""
         time_zulu = self._build_time_zulu()
-        lat = self.convert_latitude(self.latitude)
-        long = self.convert_longitude(self.longitude)
+        lat = aprslib_util.latitude_to_ddm(self.latitude)
+        lon = aprslib_util.longitude_to_ddm(self.longitude)
 
         self.payload = (
             f"@{time_zulu}z{lat}{self.symbol_table}"
-            f"{long}{self.symbol}APRSD Beacon"
+            f"{lon}"
         )
 
+        if self.comment:
+            comment = self._filter_for_send(self.comment)
+            self.payload = f"{self.payload}{self.symbol}{comment}"
+        else:
+            self.payload = f"{self.payload}{self.symbol}APRSD Beacon"
+
     def _build_raw(self):
         self.raw = (
             f"{self.from_call}>APZ100:"
             f"{self.payload}"
         )
 
+    @property
+    def key(self) -> str:
+        """Build a key for finding this packet in a dict."""
+        if self.raw_timestamp:
+            return f"{self.from_call}:{self.raw_timestamp}"
+        else:
+            return f"{self.from_call}:{self.human_info.replace(' ','')}"
+
+    @property
+    def human_info(self) -> str:
+        h_str = []
+        h_str.append(f"Lat:{self.latitude:03.3f}")
+        h_str.append(f"Lon:{self.longitude:03.3f}")
+        h_str.append(f"{self.comment}")
+        return " ".join(h_str)
+
 
-@dataclass
+@dataclass_json
+@dataclass(unsafe_hash=True)
 class MicEPacket(GPSPacket):
+    _type: str = field(default="MicEPacket", hash=False)
     messagecapable: bool = False
-    mbits: str = None
-    mtype: str = None
+    mbits: Optional[str] = None
+    mtype: Optional[str] = None
+    telemetry: Optional[dict] = field(default=None)
     # in MPH
     speed: float = 0.00
     # 0 to 360
     course: int = 0
 
-    def _build_payload(self):
-        raise NotImplementedError
+    @property
+    def key(self) -> str:
+        """Build a key for finding this packet in a dict."""
+        return f"{self.from_call}:{self.human_info.replace(' ', '')}"
+
+    @property
+    def human_info(self) -> str:
+        h_info = super().human_info
+        return f"{h_info} {self.mbits} mbits"
 
 
-@dataclass
+@dataclass_json
+@dataclass(unsafe_hash=True)
+class TelemetryPacket(GPSPacket):
+    _type: str = field(default="TelemetryPacket", hash=False)
+    messagecapable: bool = False
+    mbits: Optional[str] = None
+    mtype: Optional[str] = None
+    telemetry: Optional[dict] = field(default=None)
+    tPARM: Optional[list[str]] = field(default=None)  # noqa: N815
+    tUNIT: Optional[list[str]] = field(default=None)  # noqa: N815
+    # in MPH
+    speed: float = 0.00
+    # 0 to 360
+    course: int = 0
+
+    @property
+    def key(self) -> str:
+        """Build a key for finding this packet in a dict."""
+        if self.raw_timestamp:
+            return f"{self.from_call}:{self.raw_timestamp}"
+        else:
+            return f"{self.from_call}:{self.human_info.replace(' ','')}"
+
+    @property
+    def human_info(self) -> str:
+        h_info = super().human_info
+        return f"{h_info} {self.telemetry}"
+
+
+@dataclass_json
+@dataclass(unsafe_hash=True)
 class ObjectPacket(GPSPacket):
+    _type: str = field(default="ObjectPacket", hash=False)
     alive: bool = True
-    raw_timestamp: str = None
+    raw_timestamp: Optional[str] = None
     symbol: str = field(default="r")
     # in MPH
     speed: float = 0.00
     # 0 to 360
     course: int = 0
 
     def _build_payload(self):
         time_zulu = self._build_time_zulu()
-        lat = self.convert_latitude(self.latitude)
-        long = self.convert_longitude(self.longitude)
+        lat = aprslib_util.latitude_to_ddm(self.latitude)
+        long = aprslib_util.longitude_to_ddm(self.longitude)
 
         self.payload = (
             f"*{time_zulu}z{lat}{self.symbol_table}"
             f"{long}{self.symbol}"
         )
 
         if self.comment:
-            self.payload = f"{self.payload}{self.comment}"
+            comment = self._filter_for_send(self.comment)
+            self.payload = f"{self.payload}{comment}"
 
     def _build_raw(self):
         """
         REPEAT builds packets like
         reply = "{}>APZ100:;{:9s}*{}z{}r{:.3f}MHz {} {}".format(
                 fromcall, callsign, time_zulu, latlon, freq, uplink_tone, offset,
             )
@@ -534,29 +495,104 @@
         """
 
         self.raw = (
             f"{self.from_call}>APZ100:;{self.to_call:9s}"
             f"{self.payload}"
         )
 
+    @property
+    def human_info(self) -> str:
+        h_info = super().human_info
+        return f"{h_info} {self.comment}"
+
 
-@dataclass()
-class WeatherPacket(GPSPacket):
+@dataclass(unsafe_hash=True)
+class WeatherPacket(GPSPacket, DataClassJsonMixin):
+    _type: str = field(default="WeatherPacket", hash=False)
     symbol: str = "_"
     wind_speed: float = 0.00
     wind_direction: int = 0
     wind_gust: float = 0.00
     temperature: float = 0.00
     # in inches.  1.04 means 1.04 inches
     rain_1h: float = 0.00
     rain_24h: float = 0.00
     rain_since_midnight: float = 0.00
     humidity: int = 0
     pressure: float = 0.00
-    comment: str = None
+    comment: Optional[str] = field(default=None)
+    luminosity: Optional[int] = field(default=None)
+    wx_raw_timestamp: Optional[str] = field(default=None)
+    course: Optional[int] = field(default=None)
+    speed: Optional[float] = field(default=None)
+
+    def _translate(self, raw: dict) -> dict:
+        for key in raw["weather"]:
+            raw[key] = raw["weather"][key]
+
+        # If we have the broken aprslib, then we need to
+        # Convert the course and speed to wind_speed and wind_direction
+        # aprslib issue #80
+        # https://github.com/rossengeorgiev/aprs-python/issues/80
+        # Wind speed and course is option in the SPEC.
+        # For some reason aprslib multiplies the speed by 1.852.
+        if "wind_speed" not in raw and "wind_direction" not in raw:
+            # Most likely this is the broken aprslib
+            # So we need to convert the wind_gust speed
+            raw["wind_gust"] = round(raw.get("wind_gust", 0) / 0.44704, 3)
+        if "wind_speed" not in raw:
+            wind_speed = raw.get("speed")
+            if wind_speed:
+                raw["wind_speed"] = round(wind_speed / 1.852, 3)
+                raw["weather"]["wind_speed"] = raw["wind_speed"]
+            if "speed" in raw:
+                del raw["speed"]
+            # Let's adjust the rain numbers as well, since it's wrong
+            raw["rain_1h"] = round((raw.get("rain_1h", 0) / .254) * .01, 3)
+            raw["weather"]["rain_1h"] = raw["rain_1h"]
+            raw["rain_24h"] = round((raw.get("rain_24h", 0) / .254) * .01, 3)
+            raw["weather"]["rain_24h"] = raw["rain_24h"]
+            raw["rain_since_midnight"] = round((raw.get("rain_since_midnight", 0) / .254) * .01, 3)
+            raw["weather"]["rain_since_midnight"] = raw["rain_since_midnight"]
+
+        if "wind_direction" not in raw:
+            wind_direction = raw.get("course")
+            if wind_direction:
+                raw["wind_direction"] = wind_direction
+                raw["weather"]["wind_direction"] = raw["wind_direction"]
+            if "course" in raw:
+                del raw["course"]
+
+        del raw["weather"]
+        return raw
+
+    @classmethod
+    def from_dict(cls: Type[A], kvs: Json, *, infer_missing=False) -> A:
+        """Create from a dictionary that has come directly from aprslib parse"""
+        raw = cls._translate(cls, kvs)  # type: ignore
+        return super().from_dict(raw)
+
+    @property
+    def key(self) -> str:
+        """Build a key for finding this packet in a dict."""
+        if self.raw_timestamp:
+            return f"{self.from_call}:{self.raw_timestamp}"
+        elif self.wx_raw_timestamp:
+            return f"{self.from_call}:{self.wx_raw_timestamp}"
+
+    @property
+    def human_info(self) -> str:
+        h_str = []
+        h_str.append(f"Temp {self.temperature:03.0f}F")
+        h_str.append(f"Humidity {self.humidity}%")
+        h_str.append(f"Wind {self.wind_speed:03.0f}MPH@{self.wind_direction}")
+        h_str.append(f"Pressure {self.pressure}mb")
+        h_str.append(f"Rain {self.rain_24h}in/24hr")
+
+        return " ".join(h_str)
 
     def _build_payload(self):
         """Build an uncompressed weather packet
 
         Format =
 
        _CSE/SPDgXXXtXXXrXXXpXXXPXXXhXXbXXXXX%type NEW FORMAT APRS793 June 97
@@ -599,90 +635,189 @@
             f"P{self.rain_since_midnight*100:03.0f}",
             # Humidity
             f"h{self.humidity:02d}",
             # Barometric pressure (in tenths of millibars/tenths of hPascal)
             f"b{self.pressure:05.0f}",
         ]
         if self.comment:
-            contents.append(self.comment)
+            comment = self.filter_for_send(self.comment)
+            contents.append(comment)
         self.payload = "".join(contents)
 
     def _build_raw(self):
 
         self.raw = (
             f"{self.from_call}>{self.to_call},WIDE1-1,WIDE2-1:"
             f"{self.payload}"
         )
 
 
-class ThirdParty(Packet):
+@dataclass(unsafe_hash=True)
+class ThirdPartyPacket(Packet, DataClassJsonMixin):
+    _type: str = "ThirdPartyPacket"
     # Holds the encapsulated packet
-    subpacket: Packet = field(default=None, compare=True, hash=False)
+    subpacket: Optional[type[Packet]] = field(default=None, compare=True, hash=False)
 
     def __repr__(self):
         """Build the repr version of the packet."""
         repr_str = (
             f"{self.__class__.__name__}:"
             f" From: {self.from_call}  "
             f" To: {self.to_call}  "
             f" Subpacket: {repr(self.subpacket)}"
         )
 
         return repr_str
 
+    @classmethod
+    def from_dict(cls: Type[A], kvs: Json, *, infer_missing=False) -> A:
+        obj = super().from_dict(kvs)
+        obj.subpacket = factory(obj.subpacket)  # type: ignore
+        return obj
+
+    @property
+    def key(self) -> str:
+        """Build a key for finding this packet in a dict."""
+        return f"{self.from_call}:{self.subpacket.key}"
+
+    @property
+    def human_info(self) -> str:
+        sub_info = self.subpacket.human_info
+        return f"{self.from_call}->{self.to_call} {sub_info}"
+
+
+@dataclass_json(undefined=Undefined.INCLUDE)
+@dataclass(unsafe_hash=True)
+class UnknownPacket:
+    """Catchall Packet for things we don't know about.
 
-TYPE_LOOKUP = {
+    All of the unknown attributes are stored in the unknown_fields
+    """
+    unknown_fields: CatchAll
+    _type: str = "UnknownPacket"
+    from_call: Optional[str] = field(default=None)
+    to_call: Optional[str] = field(default=None)
+    msgNo: str = field(default_factory=_init_msgNo)   # noqa: N815
+    format: Optional[str] = field(default=None)
+    raw: Optional[str] = field(default=None)
+    raw_dict: dict = field(repr=False, default_factory=lambda: {}, compare=False, hash=False)
+    path: List[str] = field(default_factory=list, compare=False, hash=False)
+    packet_type: Optional[str] = field(default=None)
+    via: Optional[str] = field(default=None, compare=False, hash=False)
+
+    @property
+    def key(self) -> str:
+        """Build a key for finding this packet in a dict."""
+        return f"{self.from_call}:{self.packet_type}:{self.to_call}"
+
+    @property
+    def human_info(self) -> str:
+        return str(self.unknown_fields)
+
+
+TYPE_LOOKUP: dict[str, type[Packet]] = {
+    PACKET_TYPE_BULLETIN: BulletinPacket,
     PACKET_TYPE_WX: WeatherPacket,
+    PACKET_TYPE_WEATHER: WeatherPacket,
     PACKET_TYPE_MESSAGE: MessagePacket,
     PACKET_TYPE_ACK: AckPacket,
     PACKET_TYPE_REJECT: RejectPacket,
     PACKET_TYPE_MICE: MicEPacket,
     PACKET_TYPE_OBJECT: ObjectPacket,
     PACKET_TYPE_STATUS: StatusPacket,
-    PACKET_TYPE_BEACON: GPSPacket,
-    PACKET_TYPE_UNKNOWN: Packet,
-    PACKET_TYPE_THIRDPARTY: ThirdParty,
+    PACKET_TYPE_BEACON: BeaconPacket,
+    PACKET_TYPE_UNKNOWN: UnknownPacket,
+    PACKET_TYPE_THIRDPARTY: ThirdPartyPacket,
+    PACKET_TYPE_TELEMETRY: TelemetryPacket,
 }
 
 
-def get_packet_type(packet: dict):
+def get_packet_type(packet: dict) -> str:
     """Decode the packet type from the packet."""
 
-    pkt_format = packet.get("format", None)
-    msg_response = packet.get("response", None)
+    pkt_format = packet.get("format")
+    msg_response = packet.get("response")
     packet_type = PACKET_TYPE_UNKNOWN
     if pkt_format == "message" and msg_response == "ack":
         packet_type = PACKET_TYPE_ACK
     elif pkt_format == "message" and msg_response == "rej":
         packet_type = PACKET_TYPE_REJECT
     elif pkt_format == "message":
         packet_type = PACKET_TYPE_MESSAGE
     elif pkt_format == "mic-e":
         packet_type = PACKET_TYPE_MICE
     elif pkt_format == "object":
         packet_type = PACKET_TYPE_OBJECT
     elif pkt_format == "status":
         packet_type = PACKET_TYPE_STATUS
+    elif pkt_format == PACKET_TYPE_BULLETIN:
+        packet_type = PACKET_TYPE_BULLETIN
     elif pkt_format == PACKET_TYPE_BEACON:
         packet_type = PACKET_TYPE_BEACON
+    elif pkt_format == PACKET_TYPE_TELEMETRY:
+        packet_type = PACKET_TYPE_TELEMETRY
+    elif pkt_format == PACKET_TYPE_WX:
+        packet_type = PACKET_TYPE_WEATHER
     elif pkt_format == PACKET_TYPE_UNCOMPRESSED:
-        if packet.get("symbol", None) == "_":
-            packet_type = PACKET_TYPE_WX
+        if packet.get("symbol") == "_":
+            packet_type = PACKET_TYPE_WEATHER
     elif pkt_format == PACKET_TYPE_THIRDPARTY:
         packet_type = PACKET_TYPE_THIRDPARTY
 
     if packet_type == PACKET_TYPE_UNKNOWN:
         if "latitude" in packet:
             packet_type = PACKET_TYPE_BEACON
+        else:
+            packet_type = PACKET_TYPE_UNKNOWN
     return packet_type
 
 
-def is_message_packet(packet):
+def is_message_packet(packet: dict) -> bool:
     return get_packet_type(packet) == PACKET_TYPE_MESSAGE
 
 
-def is_ack_packet(packet):
+def is_ack_packet(packet: dict) -> bool:
     return get_packet_type(packet) == PACKET_TYPE_ACK
 
 
-def is_mice_packet(packet):
+def is_mice_packet(packet: dict[Any, Any]) -> bool:
     return get_packet_type(packet) == PACKET_TYPE_MICE
+
+
+def factory(raw_packet: dict[Any, Any]) -> type[Packet]:
+    """Factory method to create a packet from a raw packet string."""
+    raw = raw_packet
+    if "_type" in raw:
+        cls = globals()[raw["_type"]]
+        return cls.from_dict(raw)
+
+    raw["raw_dict"] = raw.copy()
+    raw = _translate_fields(raw)
+
+    packet_type = get_packet_type(raw)
+
+    raw["packet_type"] = packet_type
+    packet_class = TYPE_LOOKUP[packet_type]
+    if packet_type == PACKET_TYPE_WX:
+        # the weather information is in a dict
+        # this brings those values out to the outer dict
+        packet_class = WeatherPacket
+    elif packet_type == PACKET_TYPE_OBJECT and "weather" in raw:
+        packet_class = WeatherPacket
+    elif packet_type == PACKET_TYPE_UNKNOWN:
+        # Try and figure it out here
+        if "latitude" in raw:
+            packet_class = GPSPacket
+        else:
+            # LOG.warning(raw)
+            packet_class = UnknownPacket
+
+    raw.get("addresse", raw.get("to_call"))
+
+    # TODO: Find a global way to enable/disable this
+    # LOGU.opt(colors=True).info(
+    #     f"factory(<green>{packet_type: <8}</green>):"
+    #     f"(<red>{packet_class.__name__: <13}</red>): "
+    #     f"<light-blue>{raw.get('from_call'): <9}</light-blue> -> <cyan>{to: <9}</cyan>")
+    # LOG.info(raw.get('msgNo'))
+
+    return packet_class().from_dict(raw)  # type: ignore
```

### Comparing `aprsd-3.3.4/aprsd/packets/seen_list.py` & `aprsd-3.4.0/aprsd/packets/seen_list.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,54 @@
 import datetime
 import logging
-import threading
 
 from oslo_config import cfg
-import wrapt
 
+from aprsd.packets import collector, core
 from aprsd.utils import objectstore
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 
 
 class SeenList(objectstore.ObjectStoreMixin):
     """Global callsign seen list."""
 
     _instance = None
-    lock = threading.Lock()
     data: dict = {}
 
     def __new__(cls, *args, **kwargs):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
-            cls._instance._init_store()
             cls._instance.data = {}
         return cls._instance
 
-    @wrapt.synchronized(lock)
-    def update_seen(self, packet):
-        callsign = None
-        if packet.from_call:
-            callsign = packet.from_call
-        else:
-            LOG.warning(f"Can't find FROM in packet {packet}")
-            return
-        if callsign not in self.data:
-            self.data[callsign] = {
-                "last": None,
-                "count": 0,
-            }
-        self.data[callsign]["last"] = str(datetime.datetime.now())
-        self.data[callsign]["count"] += 1
+    def stats(self, serializable=False):
+        """Return the stats for the PacketTrack class."""
+        with self.lock:
+            return self.data
+
+    def rx(self, packet: type[core.Packet]):
+        """When we get a packet from the network, update the seen list."""
+        with self.lock:
+            callsign = None
+            if packet.from_call:
+                callsign = packet.from_call
+            else:
+                LOG.warning(f"Can't find FROM in packet {packet}")
+                return
+            if callsign not in self.data:
+                self.data[callsign] = {
+                    "last": None,
+                    "count": 0,
+                }
+            self.data[callsign]["last"] = datetime.datetime.now()
+            self.data[callsign]["count"] += 1
+
+    def tx(self, packet: type[core.Packet]):
+        """We don't care about TX packets."""
+
+
+# Register with the packet collector so we can process the packet
+# when we get it off the client (network)
+collector.PacketCollector().register(SeenList)
```

### Comparing `aprsd-3.3.4/aprsd/packets/watch_list.py` & `aprsd-3.4.0/aprsd/packets/watch_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,94 @@
 import datetime
 import logging
-import threading
 
 from oslo_config import cfg
-import wrapt
 
 from aprsd import utils
+from aprsd.packets import collector, core
 from aprsd.utils import objectstore
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 
 
 class WatchList(objectstore.ObjectStoreMixin):
     """Global watch list and info for callsigns."""
 
     _instance = None
-    lock = threading.Lock()
     data = {}
 
     def __new__(cls, *args, **kwargs):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
-            cls._instance._init_store()
-            cls._instance.data = {}
         return cls._instance
 
-    def __init__(self, config=None):
-        ring_size = CONF.watch_list.packet_keep_count
-
-        if CONF.watch_list.callsigns:
-            for callsign in CONF.watch_list.callsigns:
-                call = callsign.replace("*", "")
-                # FIXME(waboring) - we should fetch the last time we saw
-                # a beacon from a callsign or some other mechanism to find
-                # last time a message was seen by aprs-is.  For now this
-                # is all we can do.
-                self.data[call] = {
-                    "last": datetime.datetime.now(),
-                    "packets": utils.RingBuffer(
-                        ring_size,
-                    ),
+    def __init__(self):
+        super().__init__()
+        self._update_from_conf()
+
+    def _update_from_conf(self, config=None):
+        with self.lock:
+            if CONF.watch_list.enabled and CONF.watch_list.callsigns:
+                for callsign in CONF.watch_list.callsigns:
+                    call = callsign.replace("*", "")
+                    # FIXME(waboring) - we should fetch the last time we saw
+                    # a beacon from a callsign or some other mechanism to find
+                    # last time a message was seen by aprs-is.  For now this
+                    # is all we can do.
+                    if call not in self.data:
+                        self.data[call] = {
+                            "last": None,
+                            "packet": None,
+                        }
+
+    def stats(self, serializable=False) -> dict:
+        stats = {}
+        with self.lock:
+            for callsign in self.data:
+                stats[callsign] = {
+                    "last": self.data[callsign]["last"],
+                    "packet": self.data[callsign]["packet"],
+                    "age": self.age(callsign),
+                    "old": self.is_old(callsign),
                 }
+        return stats
 
     def is_enabled(self):
         return CONF.watch_list.enabled
 
     def callsign_in_watchlist(self, callsign):
-        return callsign in self.data
+        with self.lock:
+            return callsign in self.data
+
+    def rx(self, packet: type[core.Packet]) -> None:
+        """Track when we got a packet from the network."""
+        callsign = packet.from_call
 
-    @wrapt.synchronized(lock)
-    def update_seen(self, packet):
-        if packet.addresse:
-            callsign = packet.addresse
-        else:
-            callsign = packet.from_call
         if self.callsign_in_watchlist(callsign):
-            self.data[callsign]["last"] = datetime.datetime.now()
-            self.data[callsign]["packets"].append(packet)
+            with self.lock:
+                self.data[callsign]["last"] = datetime.datetime.now()
+                self.data[callsign]["packet"] = packet
+
+    def tx(self, packet: type[core.Packet]) -> None:
+        """We don't care about TX packets."""
 
     def last_seen(self, callsign):
-        if self.callsign_in_watchlist(callsign):
-            return self.data[callsign]["last"]
+        with self.lock:
+            if self.callsign_in_watchlist(callsign):
+                return self.data[callsign]["last"]
 
     def age(self, callsign):
         now = datetime.datetime.now()
-        return str(now - self.last_seen(callsign))
+        last_seen_time = self.last_seen(callsign)
+        if last_seen_time:
+            return str(now - last_seen_time)
+        else:
+            return None
 
     def max_delta(self, seconds=None):
         if not seconds:
             seconds = CONF.watch_list.alert_time_seconds
         max_timeout = {"seconds": seconds}
         return datetime.timedelta(**max_timeout)
 
@@ -79,18 +97,26 @@
 
         This tests to see if the last time we saw a callsign packet,
         if that is older than the allowed timeout in the config.
 
         We put this here so any notification plugin can use this
         same test.
         """
-        age = self.age(callsign)
-
-        delta = utils.parse_delta_str(age)
-        d = datetime.timedelta(**delta)
-
-        max_delta = self.max_delta(seconds=seconds)
+        if not self.callsign_in_watchlist(callsign):
+            return False
 
-        if d > max_delta:
-            return True
+        age = self.age(callsign)
+        if age:
+            delta = utils.parse_delta_str(age)
+            d = datetime.timedelta(**delta)
+
+            max_delta = self.max_delta(seconds=seconds)
+
+            if d > max_delta:
+                return True
+            else:
+                return False
         else:
             return False
+
+
+collector.PacketCollector().register(WatchList)
```

### Comparing `aprsd-3.3.4/aprsd/plugin.py` & `aprsd-3.4.0/aprsd/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# The base plugin class
+from __future__ import annotations
+
 import abc
 import importlib
 import inspect
 import logging
 import re
 import textwrap
 import threading
@@ -38,15 +39,15 @@
 hookimpl = pluggy.HookimplMarker("aprsd")
 
 
 class APRSDPluginSpec:
     """A hook specification namespace."""
 
     @hookspec
-    def filter(self, packet: packets.core.Packet):
+    def filter(self, packet: type[packets.Packet]):
         """My special little hook that you can customize."""
 
 
 class APRSDPluginBase(metaclass=abc.ABCMeta):
     """The base class for all APRSD Plugins."""
 
     config = None
@@ -61,15 +62,15 @@
 
     def __init__(self):
         self.message_counter = 0
         self.setup()
         self.threads = self.create_threads() or []
         self.start_threads()
 
-    def start_threads(self):
+    def start_threads(self) -> None:
         if self.enabled and self.threads:
             if not isinstance(self.threads, list):
                 self.threads = [self.threads]
 
             try:
                 for thread in self.threads:
                     if isinstance(thread, threads.APRSDThread):
@@ -86,18 +87,18 @@
                 LOG.error(
                     "Failed to start threads for plugin {}".format(
                         self,
                     ),
                 )
 
     @property
-    def message_count(self):
+    def message_count(self) -> int:
         return self.message_counter
 
-    def help(self):
+    def help(self) -> str:
         return "Help!"
 
     @abc.abstractmethod
     def setup(self):
         """Do any plugin setup here."""
         self.enabled = True
 
@@ -114,19 +115,19 @@
     def stop_threads(self):
         """Stop any threads this plugin might have created."""
         for thread in self.threads:
             if isinstance(thread, threads.APRSDThread):
                 thread.stop()
 
     @abc.abstractmethod
-    def filter(self, packet: packets.core.Packet):
+    def filter(self, packet: type[packets.Packet]) -> str | packets.MessagePacket:
         pass
 
     @abc.abstractmethod
-    def process(self, packet: packets.core.Packet):
+    def process(self, packet: type[packets.Packet]):
         """This is called when the filter passes."""
 
 
 class APRSDWatchListPluginBase(APRSDPluginBase, metaclass=abc.ABCMeta):
     """Base plugin class for all notification APRSD plugins.
 
     All these plugins will get every packet seen by APRSD's
@@ -150,15 +151,15 @@
                 aprs_client = client.factory.create().client
                 filter_str = "b/{}".format("/".join(watch_list))
                 aprs_client.set_filter(filter_str)
             else:
                 LOG.warning("Watch list enabled, but no callsigns set.")
 
     @hookimpl
-    def filter(self, packet: packets.core.Packet):
+    def filter(self, packet: type[packets.Packet]) -> str | packets.MessagePacket:
         result = packets.NULL_MESSAGE
         if self.enabled:
             wl = watch_list.WatchList()
             if wl.callsign_in_watchlist(packet.from_call):
                 # packet is from a callsign in the watch list
                 self.rx_inc()
                 try:
@@ -202,35 +203,35 @@
         )
 
     def setup(self):
         """Do any plugin setup here."""
         self.enabled = True
 
     @hookimpl
-    def filter(self, packet: packets.core.MessagePacket):
-        LOG.info(f"{self.__class__.__name__} called")
+    def filter(self, packet: packets.MessagePacket) -> str | packets.MessagePacket:
+        LOG.debug(f"{self.__class__.__name__} called")
         if not self.enabled:
             result = f"{self.__class__.__name__} isn't enabled"
             LOG.warning(result)
             return result
 
-        if not isinstance(packet, packets.core.MessagePacket):
+        if not isinstance(packet, packets.MessagePacket):
             LOG.warning(f"{self.__class__.__name__} Got a {packet.__class__.__name__} ignoring")
             return packets.NULL_MESSAGE
 
         result = None
 
         message = packet.message_text
         tocall = packet.to_call
 
         # Only process messages destined for us
         # and is an APRS message format and has a message.
         if (
             tocall == CONF.callsign
-            and isinstance(packet, packets.core.MessagePacket)
+            and isinstance(packet, packets.MessagePacket)
             and message
         ):
             if re.search(self.command_regex, message, re.IGNORECASE):
                 self.rx_inc()
                 try:
                     result = self.process(packet)
                 except Exception as ex:
@@ -265,15 +266,15 @@
 
     command_regex = "^[hH]"
     command_name = "help"
 
     def help(self):
         return "Help: send APRS help or help <plugin>"
 
-    def process(self, packet: packets.core.MessagePacket):
+    def process(self, packet: packets.MessagePacket):
         LOG.info("HelpPlugin")
         # fromcall = packet.get("from")
         message = packet.message_text
         # ack = packet.get("msgNo", "0")
         a = re.search(r"^.*\s+(.*)", message)
         command_name = None
         if a is not None:
@@ -339,14 +340,36 @@
     def _init(self):
         self._pluggy_pm = pluggy.PluginManager("aprsd")
         self._pluggy_pm.add_hookspecs(APRSDPluginSpec)
         # For the watchlist plugins
         self._watchlist_pm = pluggy.PluginManager("aprsd")
         self._watchlist_pm.add_hookspecs(APRSDPluginSpec)
 
+    def stats(self, serializable=False) -> dict:
+        """Collect and return stats for all plugins."""
+        def full_name_with_qualname(obj):
+            return "{}.{}".format(
+                obj.__class__.__module__,
+                obj.__class__.__qualname__,
+            )
+
+        plugin_stats = {}
+        plugins = self.get_plugins()
+        if plugins:
+
+            for p in plugins:
+                plugin_stats[full_name_with_qualname(p)] = {
+                    "enabled": p.enabled,
+                    "rx": p.rx_count,
+                    "tx": p.tx_count,
+                    "version": p.version,
+                }
+
+        return plugin_stats
+
     def is_plugin(self, obj):
         for c in inspect.getmro(obj):
             if issubclass(c, APRSDPluginBase):
                 return True
 
         return False
 
@@ -364,15 +387,17 @@
         :return:
         """
         module_name = None
         class_name = None
         try:
             module_name, class_name = module_class_string.rsplit(".", 1)
             module = importlib.import_module(module_name)
-            module = importlib.reload(module)
+            # Commented out because the email thread starts in a different context
+            # and hence gives a different singleton for the EmailStats
+            # module = importlib.reload(module)
         except Exception as ex:
             if not module_name:
                 LOG.error(f"Failed to load Plugin {module_class_string}")
             else:
                 LOG.error(f"Failed to load Plugin '{module_name}' : '{ex}'")
             return
 
@@ -465,20 +490,20 @@
             # Enabled plugins isn't set, so we default to loading all of
             # the core plugins.
             for p_name in CORE_MESSAGE_PLUGINS:
                 self._load_plugin(p_name)
 
         LOG.info("Completed Plugin Loading.")
 
-    def run(self, packet: packets.core.MessagePacket):
+    def run(self, packet: packets.MessagePacket):
         """Execute all the plugins run method."""
         with self.lock:
             return self._pluggy_pm.hook.filter(packet=packet)
 
-    def run_watchlist(self, packet: packets.core.Packet):
+    def run_watchlist(self, packet: packets.Packet):
         with self.lock:
             return self._watchlist_pm.hook.filter(packet=packet)
 
     def stop(self):
         """Stop all threads created by all plugins."""
         with self.lock:
             for p in self.get_plugins():
```

### Comparing `aprsd-3.3.4/aprsd/plugin_utils.py` & `aprsd-3.4.0/aprsd/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/plugins/email.py` & `aprsd-3.4.0/aprsd/plugins/email.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import smtplib
 import threading
 import time
 
 import imapclient
 from oslo_config import cfg
 
-from aprsd import packets, plugin, stats, threads
+from aprsd import packets, plugin, threads, utils
 from aprsd.threads import tx
 from aprsd.utils import trace
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 shortcuts_dict = None
@@ -56,14 +56,46 @@
 
     @delay.setter
     def delay(self, val):
         with self.lock:
             self._delay = val
 
 
+@utils.singleton
+class EmailStats:
+    """Singleton object to store stats related to email."""
+    _instance = None
+    tx = 0
+    rx = 0
+    email_thread_last_time = None
+
+    def stats(self, serializable=False):
+        if CONF.email_plugin.enabled:
+            last_check_time = self.email_thread_last_time
+            if serializable and last_check_time:
+                last_check_time = last_check_time.isoformat()
+            stats = {
+                "tx": self.tx,
+                "rx": self.rx,
+                "last_check_time": last_check_time,
+            }
+        else:
+            stats = {}
+        return stats
+
+    def tx_inc(self):
+        self.tx += 1
+
+    def rx_inc(self):
+        self.rx += 1
+
+    def email_thread_update(self):
+        self.email_thread_last_time = datetime.datetime.now()
+
+
 class EmailPlugin(plugin.APRSDRegexCommandPluginBase):
     """Email Plugin."""
 
     command_regex = "^-.*"
     command_name = "email"
     short_description = "Send and Receive email"
 
@@ -186,18 +218,14 @@
 
         return reply
 
 
 def _imap_connect():
     imap_port = CONF.email_plugin.imap_port
     use_ssl = CONF.email_plugin.imap_use_ssl
-    # host = CONFIG["aprsd"]["email"]["imap"]["host"]
-    # msg = "{}{}:{}".format("TLS " if use_ssl else "", host, imap_port)
-    #    LOG.debug("Connect to IMAP host {} with user '{}'".
-    #              format(msg, CONFIG['imap']['login']))
 
     try:
         server = imapclient.IMAPClient(
             CONF.email_plugin.imap_host,
             port=imap_port,
             use_uid=True,
             ssl=use_ssl,
@@ -436,15 +464,15 @@
     if server:
         try:
             server.sendmail(
                 CONF.email_plugin.smtp_login,
                 [to_addr],
                 msg.as_string(),
             )
-            stats.APRSDStats().email_tx_inc()
+            EmailStats().tx_inc()
         except Exception:
             LOG.exception("Sendmail Error!!!!")
             server.quit()
             return -1
         server.quit()
         return 0
 
@@ -541,15 +569,15 @@
 class APRSDEmailThread(threads.APRSDThread):
     def __init__(self):
         super().__init__("EmailThread")
         self.past = datetime.datetime.now()
 
     def loop(self):
         time.sleep(5)
-        stats.APRSDStats().email_thread_update()
+        EmailStats().email_thread_update()
         # always sleep for 5 seconds and see if we need to check email
         # This allows CTRL-C to stop the execution of this loop sooner
         # than check_email_delay time
         now = datetime.datetime.now()
         if now - self.past > datetime.timedelta(seconds=EmailInfo().delay):
             # It's time to check email
```

### Comparing `aprsd-3.3.4/aprsd/plugins/fortune.py` & `aprsd-3.4.0/aprsd/plugins/fortune.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/plugins/location.py` & `aprsd-3.4.0/aprsd/plugins/location.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/plugins/notify.py` & `aprsd-3.4.0/aprsd/plugins/notify.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/plugins/ping.py` & `aprsd-3.4.0/aprsd/plugins/ping.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/plugins/time.py` & `aprsd-3.4.0/aprsd/plugins/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import re
-import time
 
 from oslo_config import cfg
 import pytz
+from tzlocal import get_localzone
 
 from aprsd import packets, plugin, plugin_utils
 from aprsd.utils import fuzzy, trace
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
@@ -18,15 +18,16 @@
 
     # Look for t or t<space> or T<space> or time
     command_regex = r"^([t]|[t]\s|time)"
     command_name = "time"
     short_description = "What is the current local time."
 
     def _get_local_tz(self):
-        return pytz.timezone(time.strftime("%Z"))
+        lz = get_localzone()
+        return pytz.timezone(str(lz))
 
     def _get_utcnow(self):
         return pytz.datetime.datetime.utcnow()
 
     def build_date_str(self, localzone):
         utcnow = self._get_utcnow()
         gmt_t = pytz.utc.localize(utcnow)
```

### Comparing `aprsd-3.3.4/aprsd/plugins/weather.py` & `aprsd-3.4.0/aprsd/plugins/weather.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,14 @@
     short_description = "USA only METAR of GPS Beacon location"
 
     def setup(self):
         self.ensure_aprs_fi_key()
 
     @trace.trace
     def process(self, packet):
-        print("FISTY")
         fromcall = packet.get("from")
         message = packet.get("message_text", None)
         # ack = packet.get("msgNo", "0")
         LOG.info(f"WX Plugin '{message}'")
         a = re.search(r"^.*\s+(.*)", message)
         if a is not None:
             searchcall = a.group(1)
```

### Comparing `aprsd-3.3.4/aprsd/threads/keep_alive.py` & `aprsd-3.4.0/aprsd/threads/keep_alive.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import datetime
 import logging
 import time
 import tracemalloc
 
 from oslo_config import cfg
 
-from aprsd import client, packets, stats, utils
+from aprsd import client, packets, utils
+from aprsd.stats import collector
 from aprsd.threads import APRSDThread, APRSDThreadList
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 
 
@@ -20,96 +21,101 @@
     def __init__(self):
         tracemalloc.start()
         super().__init__("KeepAlive")
         max_timeout = {"hours": 0.0, "minutes": 2, "seconds": 0}
         self.max_delta = datetime.timedelta(**max_timeout)
 
     def loop(self):
-        if self.cntr % 60 == 0:
-            pkt_tracker = packets.PacketTrack()
-            stats_obj = stats.APRSDStats()
+        if self.loop_count % 60 == 0:
+            stats_json = collector.Collector().collect()
             pl = packets.PacketList()
             thread_list = APRSDThreadList()
             now = datetime.datetime.now()
-            last_email = stats_obj.email_thread_time
-            if last_email:
-                email_thread_time = utils.strfdelta(now - last_email)
+
+            if "EmailStats" in stats_json:
+                email_stats = stats_json["EmailStats"]
+                if email_stats.get("last_check_time"):
+                    email_thread_time = utils.strfdelta(now - email_stats["last_check_time"])
+                else:
+                    email_thread_time = "N/A"
             else:
                 email_thread_time = "N/A"
 
-            last_msg_time = utils.strfdelta(now - stats_obj.aprsis_keepalive)
-
-            current, peak = tracemalloc.get_traced_memory()
-            stats_obj.set_memory(current)
-            stats_obj.set_memory_peak(peak)
-
-            login = CONF.callsign
+            if "APRSClientStats" in stats_json and stats_json["APRSClientStats"].get("transport") == "aprsis":
+                if stats_json["APRSClientStats"].get("server_keepalive"):
+                    last_msg_time = utils.strfdelta(now - stats_json["APRSClientStats"]["server_keepalive"])
+                else:
+                    last_msg_time = "N/A"
+            else:
+                last_msg_time = "N/A"
 
-            tracked_packets = len(pkt_tracker)
+            tracked_packets = stats_json["PacketTrack"]["total_tracked"]
+            tx_msg = 0
+            rx_msg = 0
+            if "PacketList" in stats_json:
+                msg_packets = stats_json["PacketList"].get("MessagePacket")
+                if msg_packets:
+                    tx_msg = msg_packets.get("tx", 0)
+                    rx_msg = msg_packets.get("rx", 0)
 
             keepalive = (
                 "{} - Uptime {} RX:{} TX:{} Tracker:{} Msgs TX:{} RX:{} "
                 "Last:{} Email: {} - RAM Current:{} Peak:{} Threads:{}"
             ).format(
-                login,
-                utils.strfdelta(stats_obj.uptime),
+                stats_json["APRSDStats"]["callsign"],
+                stats_json["APRSDStats"]["uptime"],
                 pl.total_rx(),
                 pl.total_tx(),
                 tracked_packets,
-                stats_obj._pkt_cnt["MessagePacket"]["tx"],
-                stats_obj._pkt_cnt["MessagePacket"]["rx"],
+                tx_msg,
+                rx_msg,
                 last_msg_time,
                 email_thread_time,
-                utils.human_size(current),
-                utils.human_size(peak),
+                stats_json["APRSDStats"]["memory_current_str"],
+                stats_json["APRSDStats"]["memory_peak_str"],
                 len(thread_list),
             )
             LOG.info(keepalive)
-            thread_out = []
-            thread_info = {}
-            for thread in thread_list.threads_list:
-                alive = thread.is_alive()
-                age = thread.loop_age()
-                key = thread.__class__.__name__
-                thread_out.append(f"{key}:{alive}:{age}")
-                if key not in thread_info:
-                    thread_info[key] = {}
-                thread_info[key]["alive"] = alive
-                thread_info[key]["age"] = age
-                if not alive:
-                    LOG.error(f"Thread {thread}")
-            LOG.info(",".join(thread_out))
-            stats_obj.set_thread_info(thread_info)
+            if "APRSDThreadList" in stats_json:
+                thread_list = stats_json["APRSDThreadList"]
+                for thread_name in thread_list:
+                    thread = thread_list[thread_name]
+                    alive = thread["alive"]
+                    age = thread["age"]
+                    key = thread["name"]
+                    if not alive:
+                        LOG.error(f"Thread {thread}")
+                    LOG.info(f"{key: <15} Alive? {str(alive): <5} {str(age): <20}")
 
             # check the APRS connection
             cl = client.factory.create()
             # Reset the connection if it's dead and this isn't our
             # First time through the loop.
             # The first time through the loop can happen at startup where
             # The keepalive thread starts before the client has a chance
             # to make it's connection the first time.
             if not cl.is_alive() and self.cntr > 0:
                 LOG.error(f"{cl.__class__.__name__} is not alive!!! Resetting")
                 client.factory.create().reset()
-            else:
-                # See if we should reset the aprs-is client
-                # Due to losing a keepalive from them
-                delta_dict = utils.parse_delta_str(last_msg_time)
-                delta = datetime.timedelta(**delta_dict)
-
-                if delta > self.max_delta:
-                    #  We haven't gotten a keepalive from aprs-is in a while
-                    # reset the connection.a
-                    if not client.KISSClient.is_enabled():
-                        LOG.warning(f"Resetting connection to APRS-IS {delta}")
-                        client.factory.create().reset()
+            # else:
+            #     # See if we should reset the aprs-is client
+            #     # Due to losing a keepalive from them
+            #     delta_dict = utils.parse_delta_str(last_msg_time)
+            #     delta = datetime.timedelta(**delta_dict)
+            #
+            #     if delta > self.max_delta:
+            #         #  We haven't gotten a keepalive from aprs-is in a while
+            #         # reset the connection.a
+            #         if not client.KISSClient.is_enabled():
+            #             LOG.warning(f"Resetting connection to APRS-IS {delta}")
+            #             client.factory.create().reset()
 
             # Check version every day
             delta = now - self.checker_time
             if delta > datetime.timedelta(hours=24):
                 self.checker_time = now
                 level, msg = utils._check_version()
                 if level:
                     LOG.warning(msg)
-        self.cntr += 1
+            self.cntr += 1
         time.sleep(1)
         return True
```

### Comparing `aprsd-3.3.4/aprsd/threads/registry.py` & `aprsd-3.4.0/aprsd/threads/registry.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/threads/rx.py` & `aprsd-3.4.0/aprsd/threads/rx.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,60 +3,76 @@
 import queue
 import time
 
 import aprslib
 from oslo_config import cfg
 
 from aprsd import client, packets, plugin
+from aprsd.packets import collector
+from aprsd.packets import log as packet_log
 from aprsd.threads import APRSDThread, tx
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 
 
 class APRSDRXThread(APRSDThread):
     def __init__(self, packet_queue):
-        super().__init__("RX_MSG")
+        super().__init__("RX_PKT")
         self.packet_queue = packet_queue
         self._client = client.factory.create()
 
     def stop(self):
         self.thread_stop = True
-        client.factory.create().client.stop()
+        if self._client:
+            self._client.stop()
 
     def loop(self):
+        if not self._client:
+            self._client = client.factory.create()
+            time.sleep(1)
+            return True
         # setup the consumer of messages and block until a messages
         try:
             # This will register a packet consumer with aprslib
             # When new packets come in the consumer will process
             # the packet
 
             # Do a partial here because the consumer signature doesn't allow
             # For kwargs to be passed in to the consumer func we declare
             # and the aprslib developer didn't want to allow a PR to add
             # kwargs.  :(
             # https://github.com/rossengeorgiev/aprs-python/pull/56
-            self._client.client.consumer(
-                self.process_packet, raw=False, blocking=False,
+            self._client.consumer(
+                self._process_packet, raw=False, blocking=False,
             )
-
         except (
             aprslib.exceptions.ConnectionDrop,
             aprslib.exceptions.ConnectionError,
         ):
             LOG.error("Connection dropped, reconnecting")
-            time.sleep(5)
             # Force the deletion of the client object connected to aprs
             # This will cause a reconnect, next time client.get_client()
             # is called
             self._client.reset()
+            time.sleep(5)
+        except Exception:
+            # LOG.exception(ex)
+            LOG.error("Resetting connection and trying again.")
+            self._client.reset()
+            time.sleep(5)
         # Continue to loop
         return True
 
+    def _process_packet(self, *args, **kwargs):
+        """Intermediate callback so we can update the keepalive time."""
+        # Now call the 'real' packet processing for a RX'x packet
+        self.process_packet(*args, **kwargs)
+
     @abc.abstractmethod
     def process_packet(self, *args, **kwargs):
         pass
 
 
 class APRSDDupeRXThread(APRSDRXThread):
     """Process received packets.
@@ -76,50 +92,47 @@
         Ack Packets are sent to the PluginProcessPacketThread for processing.
         All other packets have to be checked as a dupe, and then only after
         we haven't seen this packet before, do we send it to the
         PluginProcessPacketThread for processing.
         """
         packet = self._client.decode_packet(*args, **kwargs)
         # LOG.debug(raw)
-        packet.log(header="RX")
+        packet_log.log(packet)
+        pkt_list = packets.PacketList()
 
         if isinstance(packet, packets.AckPacket):
             # We don't need to drop AckPackets, those should be
             # processed.
             self.packet_queue.put(packet)
         else:
             # Make sure we aren't re-processing the same packet
             # For RF based APRS Clients we can get duplicate packets
             # So we need to track them and not process the dupes.
             found = False
-            pkt_list = packets.PacketList()
             try:
                 # Find the packet in the list of already seen packets
                 # Based on the packet.key
                 found = pkt_list.find(packet)
             except KeyError:
                 found = False
 
             if not found:
-                # If we are in the process of already ack'ing
-                # a packet, we should drop the packet
-                # because it's a dupe within the time that
-                # we send the 3 acks for the packet.
-                pkt_list.rx(packet)
+                # We haven't seen this packet before, so we process it.
+                collector.PacketCollector().rx(packet)
                 self.packet_queue.put(packet)
             elif packet.timestamp - found.timestamp < CONF.packet_dupe_timeout:
-                # If the packet came in within 60 seconds of the
+                # If the packet came in within N seconds of the
                 # Last time seeing the packet, then we drop it as a dupe.
                 LOG.warning(f"Packet {packet.from_call}:{packet.msgNo} already tracked, dropping.")
             else:
                 LOG.warning(
                     f"Packet {packet.from_call}:{packet.msgNo} already tracked "
                     f"but older than {CONF.packet_dupe_timeout} seconds. processing.",
                 )
-                pkt_list.rx(packet)
+                collector.PacketCollector().rx(packet)
                 self.packet_queue.put(packet)
 
 
 class APRSDPluginRXThread(APRSDDupeRXThread):
     """"Process received packets.
 
     For backwards compatibility, we keep the APRSDPluginRXThread.
@@ -133,43 +146,45 @@
     the consumer.  This base class handles sending ack packets and
     will ack a message before sending the packet to the subclass
     for processing."""
 
     def __init__(self, packet_queue):
         self.packet_queue = packet_queue
         super().__init__("ProcessPKT")
-        self._loop_cnt = 1
 
     def process_ack_packet(self, packet):
         """We got an ack for a message, no need to resend it."""
         ack_num = packet.msgNo
-        LOG.info(f"Got ack for message {ack_num}")
-        pkt_tracker = packets.PacketTrack()
-        pkt_tracker.remove(ack_num)
+        LOG.debug(f"Got ack for message {ack_num}")
+        collector.PacketCollector().rx(packet)
+
+    def process_piggyback_ack(self, packet):
+        """We got an ack embedded in a packet."""
+        ack_num = packet.ackMsgNo
+        LOG.debug(f"Got PiggyBackAck for message {ack_num}")
+        collector.PacketCollector().rx(packet)
 
     def process_reject_packet(self, packet):
         """We got a reject message for a packet.  Stop sending the message."""
         ack_num = packet.msgNo
-        LOG.info(f"Got REJECT for message {ack_num}")
-        pkt_tracker = packets.PacketTrack()
-        pkt_tracker.remove(ack_num)
+        LOG.debug(f"Got REJECT for message {ack_num}")
+        collector.PacketCollector().rx(packet)
 
     def loop(self):
         try:
             packet = self.packet_queue.get(timeout=1)
             if packet:
                 self.process_packet(packet)
         except queue.Empty:
             pass
-        self._loop_cnt += 1
         return True
 
     def process_packet(self, packet):
         """Process a packet received from aprs-is server."""
-        LOG.debug(f"ProcessPKT-LOOP {self._loop_cnt}")
+        LOG.debug(f"ProcessPKT-LOOP {self.loop_count}")
         our_call = CONF.callsign.lower()
 
         from_call = packet.from_call
         if packet.addresse:
             to_call = packet.addresse
         else:
             to_call = packet.to_call
@@ -184,14 +199,18 @@
             self.process_ack_packet(packet)
         elif (
             isinstance(packet, packets.RejectPacket)
             and packet.addresse.lower() == our_call
         ):
             self.process_reject_packet(packet)
         else:
+            if hasattr(packet, "ackMsgNo") and packet.ackMsgNo:
+                # we got an ack embedded in this packet
+                # we need to handle the ack
+                self.process_piggyback_ack(packet)
             # Only ack messages that were sent directly to us
             if isinstance(packet, packets.MessagePacket):
                 if to_call and to_call.lower() == our_call:
                     # It's a MessagePacket and it's for us!
                     # let any threads do their thing, then ack
                     # send an ack last
                     tx.send(
```

### Comparing `aprsd-3.3.4/aprsd/threads/tx.py` & `aprsd-3.4.0/aprsd/threads/tx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import logging
+import threading
 import time
 
 from oslo_config import cfg
 from rush import quota, throttle
 from rush.contrib import decorator
 from rush.limiters import periodic
 from rush.stores import dictionary
+import wrapt
 
 from aprsd import client
 from aprsd import conf  # noqa
 from aprsd import threads as aprsd_threads
-from aprsd.packets import core, tracker
+from aprsd.packets import collector, core
+from aprsd.packets import log as packet_log
+from aprsd.packets import tracker
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 
 msg_t = throttle.Throttle(
     limiter=periodic.PeriodicLimiter(
@@ -31,22 +35,27 @@
     rate=quota.Quota.per_second(
         count=CONF.ack_rate_limit_period,
     ),
 )
 
 msg_throttle_decorator = decorator.ThrottleDecorator(throttle=msg_t)
 ack_throttle_decorator = decorator.ThrottleDecorator(throttle=ack_t)
+s_lock = threading.Lock()
 
 
+@wrapt.synchronized(s_lock)
 @msg_throttle_decorator.sleep_and_retry
 def send(packet: core.Packet, direct=False, aprs_client=None):
     """Send a packet either in a thread or directly to the client."""
     # prepare the packet for sending.
     # This constructs the packet.raw
     packet.prepare()
+    # Have to call the collector to track the packet
+    # After prepare, as prepare assigns the msgNo
+    collector.PacketCollector().tx(packet)
     if isinstance(packet, core.AckPacket):
         _send_ack(packet, direct=direct, aprs_client=aprs_client)
     else:
         _send_packet(packet, direct=direct, aprs_client=aprs_client)
 
 
 @msg_throttle_decorator.sleep_and_retry
@@ -70,27 +79,28 @@
 def _send_direct(packet, aprs_client=None):
     if aprs_client:
         cl = aprs_client
     else:
         cl = client.factory.create()
 
     packet.update_timestamp()
-    packet.log(header="TX")
-    cl.send(packet)
+    packet_log.log(packet, tx=True)
+    try:
+        cl.send(packet)
+    except Exception as e:
+        LOG.error(f"Failed to send packet: {packet}")
+        LOG.error(e)
 
 
 class SendPacketThread(aprsd_threads.APRSDThread):
     loop_count: int = 1
 
     def __init__(self, packet):
         self.packet = packet
-        name = self.packet.raw[:5]
-        super().__init__(f"TXPKT-{self.packet.msgNo}-{name}")
-        pkt_tracker = tracker.PacketTrack()
-        pkt_tracker.add(packet)
+        super().__init__(f"TX-{packet.to_call}-{self.packet.msgNo}")
 
     def loop(self):
         """Loop until a message is acked or it gets delayed.
 
         We only sleep for 5 seconds between each loop run, so
         that CTRL-C can exit the app in a short period.  Each sleep
         means the app quitting is blocked until sleep is done.
@@ -108,25 +118,24 @@
                 f"{self.packet.__class__.__name__}"
                 f"({self.packet.msgNo}) "
                 "Message Send Complete via Ack.",
             )
             return False
         else:
             send_now = False
-            if packet.send_count == packet.retry_count:
+            if packet.send_count >= packet.retry_count:
                 # we reached the send limit, don't send again
                 # TODO(hemna) - Need to put this in a delayed queue?
                 LOG.info(
                     f"{packet.__class__.__name__} "
                     f"({packet.msgNo}) "
                     "Message Send Complete. Max attempts reached"
                     f" {packet.retry_count}",
                 )
-                if not packet.allow_delay:
-                    pkt_tracker.remove(packet.msgNo)
+                pkt_tracker.remove(packet.msgNo)
                 return False
 
             # Message is still outstanding and needs to be acked.
             if packet.last_send_time:
                 # Message has a last send time tracking
                 now = int(round(time.time()))
                 sleeptime = (packet.send_count + 1) * 31
@@ -137,41 +146,43 @@
             else:
                 send_now = True
 
             if send_now:
                 # no attempt time, so lets send it, and start
                 # tracking the time.
                 packet.last_send_time = int(round(time.time()))
-                send(packet, direct=True)
+                _send_direct(packet)
                 packet.send_count += 1
 
             time.sleep(1)
             # Make sure we get called again.
             self.loop_count += 1
             return True
 
 
 class SendAckThread(aprsd_threads.APRSDThread):
     loop_count: int = 1
+    max_retries = 3
 
     def __init__(self, packet):
         self.packet = packet
-        super().__init__(f"SendAck-{self.packet.msgNo}")
+        super().__init__(f"TXAck-{packet.to_call}-{self.packet.msgNo}")
+        self.max_retries = CONF.default_ack_send_count
 
     def loop(self):
         """Separate thread to send acks with retries."""
         send_now = False
-        if self.packet.send_count == self.packet.retry_count:
+        if self.packet.send_count == self.max_retries:
             # we reached the send limit, don't send again
             # TODO(hemna) - Need to put this in a delayed queue?
-            LOG.info(
+            LOG.debug(
                 f"{self.packet.__class__.__name__}"
                 f"({self.packet.msgNo}) "
                 "Send Complete. Max attempts reached"
-                f" {self.packet.retry_count}",
+                f" {self.max_retries}",
             )
             return False
 
         if self.packet.last_send_time:
             # Message has a last send time tracking
             now = int(round(time.time()))
 
@@ -184,15 +195,15 @@
                 send_now = True
             elif self.loop_count % 10 == 0:
                 LOG.debug(f"Still wating. {delta}")
         else:
             send_now = True
 
         if send_now:
-            send(self.packet, direct=True)
+            _send_direct(self.packet)
             self.packet.send_count += 1
             self.packet.last_send_time = int(round(time.time()))
 
         time.sleep(1)
         self.loop_count += 1
         return True
 
@@ -226,11 +237,19 @@
                 from_call=CONF.callsign,
                 to_call="APRS",
                 latitude=float(CONF.latitude),
                 longitude=float(CONF.longitude),
                 comment="APRSD GPS Beacon",
                 symbol=CONF.beacon_symbol,
             )
-            send(pkt, direct=True)
+            try:
+                # Only send it once
+                pkt.retry_count = 1
+                send(pkt, direct=True)
+            except Exception as e:
+                LOG.error(f"Failed to send beacon: {e}")
+                client.factory.create().reset()
+                time.sleep(5)
+
         self._loop_cnt += 1
         time.sleep(1)
         return True
```

### Comparing `aprsd-3.3.4/aprsd/utils/__init__.py` & `aprsd-3.4.0/aprsd/utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Utilities and helper functions."""
 
 import errno
+import functools
 import os
 import re
 import sys
 import traceback
 
 import update_checker
 
@@ -18,14 +19,25 @@
 
 if sys.version_info.major == 3 and sys.version_info.minor >= 3:
     from collections.abc import MutableMapping
 else:
     from collections.abc import MutableMapping
 
 
+def singleton(cls):
+    """Make a class a Singleton class (only one instance)"""
+    @functools.wraps(cls)
+    def wrapper_singleton(*args, **kwargs):
+        if wrapper_singleton.instance is None:
+            wrapper_singleton.instance = cls(*args, **kwargs)
+        return wrapper_singleton.instance
+    wrapper_singleton.instance = None
+    return wrapper_singleton
+
+
 def env(*vars, **kwargs):
     """This returns the first environment variable set.
     if none are non-empty, defaults to '' or keyword arg default
     """
     for v in vars:
         value = os.environ.get(v, None)
         if value:
```

### Comparing `aprsd-3.3.4/aprsd/utils/counter.py` & `aprsd-3.4.0/aprsd/utils/counter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 from multiprocessing import RawValue
+import random
 import threading
 
 import wrapt
 
 
+MAX_PACKET_ID = 9999
+
+
 class PacketCounter:
     """
     Global Packet id counter class.
 
     This is a singleton based class that keeps
     an incrementing counter for all packets to
     be sent.  All new Packet objects gets a new
     message id, which is the next number available
     from the PacketCounter.
 
     """
 
     _instance = None
-    max_count = 9999
     lock = threading.Lock()
 
     def __new__(cls, *args, **kwargs):
         """Make this a singleton class."""
         if cls._instance is None:
             cls._instance = super().__new__(cls, *args, **kwargs)
-            cls._instance.val = RawValue("i", 1)
+            cls._instance.val = RawValue("i", random.randint(1, MAX_PACKET_ID))
         return cls._instance
 
     @wrapt.synchronized(lock)
     def increment(self):
-        if self.val.value == self.max_count:
+        if self.val.value == MAX_PACKET_ID:
             self.val.value = 1
         else:
             self.val.value += 1
 
     @property
     @wrapt.synchronized(lock)
     def value(self):
```

### Comparing `aprsd-3.3.4/aprsd/utils/fuzzyclock.py` & `aprsd-3.4.0/aprsd/utils/fuzzyclock.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/utils/json.py` & `aprsd-3.4.0/aprsd/utils/json.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import datetime
 import decimal
 import json
 import sys
 
+from aprsd.packets import core
+
 
 class EnhancedJSONEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, datetime.datetime):
             args = (
                 "year", "month", "day", "hour", "minute",
                 "second", "microsecond",
@@ -38,14 +40,32 @@
                 "__type__": "decimal.Decimal",
                 "args": [str(obj)],
             }
         else:
             return super().default(obj)
 
 
+class SimpleJSONEncoder(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, datetime.datetime):
+            return obj.isoformat()
+        elif isinstance(obj, datetime.date):
+            return str(obj)
+        elif isinstance(obj, datetime.time):
+            return str(obj)
+        elif isinstance(obj, datetime.timedelta):
+            return str(obj)
+        elif isinstance(obj, decimal.Decimal):
+            return str(obj)
+        elif isinstance(obj, core.Packet):
+            return obj.to_dict()
+        else:
+            return super().default(obj)
+
+
 class EnhancedJSONDecoder(json.JSONDecoder):
 
     def __init__(self, *args, **kwargs):
         super().__init__(
             *args, object_hook=self.object_hook,
             **kwargs,
         )
```

### Comparing `aprsd-3.3.4/aprsd/utils/objectstore.py` & `aprsd-3.4.0/aprsd/utils/objectstore.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 import pathlib
 import pickle
+import threading
 
 from oslo_config import cfg
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("APRSD")
 
@@ -21,27 +22,36 @@
 
 
     When APRSD quits, it calls save()
     When APRSD Starts, it calls load()
     aprsd server -f (flush) will wipe all saved objects.
     """
 
+    def __init__(self):
+        self.lock = threading.RLock()
+
     def __len__(self):
-        return len(self.data)
+        with self.lock:
+            return len(self.data)
 
     def __iter__(self):
-        return iter(self.data)
+        with self.lock:
+            return iter(self.data)
 
     def get_all(self):
         with self.lock:
             return self.data
 
-    def get(self, id):
+    def get(self, key):
+        with self.lock:
+            return self.data.get(key)
+
+    def copy(self):
         with self.lock:
-            return self.data[id]
+            return self.data.copy()
 
     def _init_store(self):
         if not CONF.enable_save:
             return
         sl = CONF.save_location
         if not os.path.exists(sl):
             LOG.warning(f"Save location {sl} doesn't exist")
@@ -54,39 +64,34 @@
         save_location = CONF.save_location
 
         return "{}/{}.p".format(
             save_location,
             self.__class__.__name__.lower(),
         )
 
-    def _dump(self):
-        dump = {}
-        with self.lock:
-            for key in self.data.keys():
-                dump[key] = self.data[key]
-
-        return dump
-
     def save(self):
         """Save any queued to disk?"""
         if not CONF.enable_save:
             return
+        self._init_store()
+        save_filename = self._save_filename()
         if len(self) > 0:
             LOG.info(
                 f"{self.__class__.__name__}::Saving"
-                f" {len(self)} entries to disk at"
-                f"{CONF.save_location}",
+                f" {len(self)} entries to disk at "
+                f"{save_filename}",
             )
-            with open(self._save_filename(), "wb+") as fp:
-                pickle.dump(self._dump(), fp)
+            with self.lock:
+                with open(save_filename, "wb+") as fp:
+                    pickle.dump(self.data, fp)
         else:
             LOG.debug(
                 "{} Nothing to save, flushing old save file '{}'".format(
                     self.__class__.__name__,
-                    self._save_filename(),
+                    save_filename,
                 ),
             )
             self.flush()
 
     def load(self):
         if not CONF.enable_save:
             return
```

### Comparing `aprsd-3.3.4/aprsd/utils/ring_buffer.py` & `aprsd-3.4.0/aprsd/utils/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/utils/trace.py` & `aprsd-3.4.0/aprsd/utils/trace.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/admin/static/css/index.css` & `aprsd-3.4.0/aprsd/web/admin/static/css/index.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/admin/static/css/tabs.css` & `aprsd-3.4.0/aprsd/web/admin/static/css/tabs.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/admin/static/images/Untitled.png` & `aprsd-3.4.0/aprsd/web/admin/static/images/Untitled.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-16-0.png` & `aprsd-3.4.0/aprsd/web/admin/static/images/aprs-symbols-16-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-16-1.png` & `aprsd-3.4.0/aprsd/web/admin/static/images/aprs-symbols-16-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-64-0.png` & `aprsd-3.4.0/aprsd/web/admin/static/images/aprs-symbols-64-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-64-1.png` & `aprsd-3.4.0/aprsd/web/admin/static/images/aprs-symbols-64-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/admin/static/images/aprs-symbols-64-2.png` & `aprsd-3.4.0/aprsd/web/admin/static/images/aprs-symbols-64-2.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/admin/static/js/charts.js` & `aprsd-3.4.0/aprsd/web/admin/static/js/charts.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -222,19 +222,21 @@
     chart.data.datasets[1].data.push(second);
     chart.data.datasets[2].data.push(third);
     chart.data.datasets[3].data.push(fourth);
     chart.update();
 }
 
 function update_stats(data) {
-    our_callsign = data["stats"]["aprsd"]["callsign"];
-    $("#version").text(data["stats"]["aprsd"]["version"]);
+    our_callsign = data["APRSDStats"]["callsign"];
+    $("#version").text(data["APRSDStats"]["version"]);
     $("#aprs_connection").html(data["aprs_connection"]);
-    $("#uptime").text("uptime: " + data["stats"]["aprsd"]["uptime"]);
+    $("#uptime").text("uptime: " + data["APRSDStats"]["uptime"]);
     const html_pretty = Prism.highlight(JSON.stringify(data, null, '\t'), Prism.languages.json, 'json');
     $("#jsonstats").html(html_pretty);
     short_time = data["time"].split(/\s(.+)/)[1];
-    updateDualData(packets_chart, short_time, data["stats"]["packets"]["sent"], data["stats"]["packets"]["received"]);
-    updateQuadData(message_chart, short_time, data["stats"]["messages"]["sent"], data["stats"]["messages"]["received"], data["stats"]["messages"]["ack_sent"], data["stats"]["messages"]["ack_recieved"]);
-    updateDualData(email_chart, short_time, data["stats"]["email"]["sent"], data["stats"]["email"]["recieved"]);
-    updateDualData(memory_chart, short_time, data["stats"]["aprsd"]["memory_peak"], data["stats"]["aprsd"]["memory_current"]);
+    packet_list = data["PacketList"]["packets"];
+    updateDualData(packets_chart, short_time, data["PacketList"]["sent"], data["PacketList"]["received"]);
+    updateQuadData(message_chart, short_time, packet_list["MessagePacket"]["tx"], packet_list["MessagePacket"]["rx"],
+        packet_list["AckPacket"]["tx"], packet_list["AckPacket"]["rx"]);
+    updateDualData(email_chart, short_time, data["EmailStats"]["sent"], data["EmailStats"]["recieved"]);
+    updateDualData(memory_chart, short_time, data["APRSDStats"]["memory_peak"], data["APRSDStats"]["memory_current"]);
 }
```

### Comparing `aprsd-3.3.4/aprsd/web/admin/static/js/echarts.js` & `aprsd-3.4.0/aprsd/web/admin/static/js/echarts.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -4,23 +4,26 @@
 var rx_data = [];
 
 var packet_types_data = {};
 
 var mem_current = []
 var mem_peak = []
 
+var thread_current = []
+
 
 function start_charts() {
     console.log("start_charts() called");
     // Initialize the echarts instance based on the prepared dom
     create_packets_chart();
     create_packets_types_chart();
     create_messages_chart();
     create_ack_chart();
     create_memory_chart();
+    create_thread_chart();
 }
 
 
 function create_packets_chart() {
     // The packets totals TX/RX chart.
     pkt_c_canvas = document.getElementById('packetsChart');
     packets_chart = echarts.init(pkt_c_canvas);
@@ -320,14 +323,69 @@
             }
         }]
     };
 
     memory_chart.setOption(option);
 }
 
+function create_thread_chart() {
+    thread_canvas = document.getElementById('threadChart');
+    thread_chart = echarts.init(thread_canvas);
+
+    // Specify the configuration items and data for the chart
+    var option = {
+        title: {
+            text: 'Active Threads'
+        },
+        legend: {},
+        tooltip: {
+            trigger: 'axis'
+        },
+        toolbox: {
+            show: true,
+            feature: {
+                mark: {
+                    show: true
+                },
+                dataView: {
+                    show: true,
+                    readOnly: false
+                },
+                magicType: {
+                    show: true,
+                    type: ['line', 'bar']
+                },
+                restore: {
+                    show: true
+                },
+                saveAsImage: {
+                    show: true
+                }
+            }
+        },
+        calculable: true,
+        xAxis: {
+            type: 'time'
+        },
+        yAxis: {},
+        series: [{
+            name: 'current',
+            type: 'line',
+            smooth: true,
+            color: 'red',
+            encode: {
+                x: 'timestamp',
+                y: 'current' // refer sensor 1 value
+            }
+        }]
+    };
+
+    thread_chart.setOption(option);
+}
+
 
 
 
 function updatePacketData(chart, time, first, second) {
     tx_data.push([time, first]);
     rx_data.push([time, second]);
     option = {
@@ -389,15 +447,14 @@
         }
         series.push(entry)
     }
 
     option = {
         series: series
     }
-    console.log(option)
     packet_types_chart.setOption(option);
 }
 
 function updateTypeChart(chart, key) {
     //Generic function to update a packet type chart
     if (!packet_types_data.hasOwnProperty(key)) {
         return;
@@ -430,36 +487,51 @@
             name: 'peak',
             data: mem_peak,
         }]
     }
     memory_chart.setOption(option);
 }
 
+function updateThreadChart(time, threads) {
+    keys = Object.keys(threads);
+    thread_count = keys.length;
+    thread_current.push([time, thread_count]);
+    option = {
+        series: [{
+            name: 'current',
+            data: thread_current,
+        }]
+    }
+    thread_chart.setOption(option);
+}
+
 function updateMessagesChart() {
     updateTypeChart(message_chart, "MessagePacket")
 }
 
 function updateAcksChart() {
     updateTypeChart(ack_chart, "AckPacket")
 }
 
 function update_stats(data) {
-    console.log(data);
-    our_callsign = data["stats"]["aprsd"]["callsign"];
-    $("#version").text(data["stats"]["aprsd"]["version"]);
-    $("#aprs_connection").html(data["aprs_connection"]);
-    $("#uptime").text("uptime: " + data["stats"]["aprsd"]["uptime"]);
+    console.log("update_stats() echarts.js called")
+    stats = data["stats"];
+    our_callsign = stats["APRSDStats"]["callsign"];
+    $("#version").text(stats["APRSDStats"]["version"]);
+    $("#aprs_connection").html(stats["aprs_connection"]);
+    $("#uptime").text("uptime: " + stats["APRSDStats"]["uptime"]);
     const html_pretty = Prism.highlight(JSON.stringify(data, null, '\t'), Prism.languages.json, 'json');
     $("#jsonstats").html(html_pretty);
 
     t = Date.parse(data["time"]);
     ts = new Date(t);
-    updatePacketData(packets_chart, ts, data["stats"]["packets"]["sent"], data["stats"]["packets"]["received"]);
-    updatePacketTypesData(ts, data["stats"]["packets"]["types"]);
+    updatePacketData(packets_chart, ts, stats["PacketList"]["tx"], stats["PacketList"]["rx"]);
+    updatePacketTypesData(ts, stats["PacketList"]["types"]);
     updatePacketTypesChart();
     updateMessagesChart();
     updateAcksChart();
-    updateMemChart(ts, data["stats"]["aprsd"]["memory_current"], data["stats"]["aprsd"]["memory_peak"]);
+    updateMemChart(ts, stats["APRSDStats"]["memory_current"], stats["APRSDStats"]["memory_peak"]);
+    updateThreadChart(ts, stats["APRSDThreadList"]);
     //updateQuadData(message_chart, short_time, data["stats"]["messages"]["sent"], data["stats"]["messages"]["received"], data["stats"]["messages"]["ack_sent"], data["stats"]["messages"]["ack_recieved"]);
     //updateDualData(email_chart, short_time, data["stats"]["email"]["sent"], data["stats"]["email"]["recieved"]);
     //updateDualData(memory_chart, short_time, data["stats"]["aprsd"]["memory_peak"], data["stats"]["aprsd"]["memory_current"]);
 }
```

### Comparing `aprsd-3.3.4/aprsd/web/admin/static/js/logs.js` & `aprsd-3.4.0/aprsd/web/admin/static/js/logs.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/admin/static/js/main.js` & `aprsd-3.4.0/aprsd/web/admin/static/js/main.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -23,18 +23,22 @@
 function ord(str) {
     return str.charCodeAt(0);
 }
 
 
 function update_watchlist(data) {
     // Update the watch list
+    stats = data["stats"];
+    if (stats.hasOwnProperty("WatchList") == false) {
+        return
+    }
     var watchdiv = $("#watchDiv");
     var html_str = '<table class="ui celled striped table"><thead><tr><th>HAM Callsign</th><th>Age since last seen by APRSD</th></tr></thead><tbody>'
     watchdiv.html('')
-    jQuery.each(data["stats"]["aprsd"]["watch_list"], function(i, val) {
+    jQuery.each(stats["WatchList"], function(i, val) {
         html_str += '<tr><td class="collapsing"><img id="callsign_' + i + '" class="aprsd_1"></img>' + i + '</td><td>' + val["last"] + '</td></tr>'
     });
     html_str += "</tbody></table>";
     watchdiv.append(html_str);
 
     jQuery.each(watchlist, function(i, val) {
         //update the symbol
@@ -58,63 +62,99 @@
     if (watchlist[callsign]["packets"].hasOwnProperty(val['ts']) == false) {
         watchlist[callsign]["packets"][val['ts']] = val;
     }
     //console.log(watchlist)
 }
 
 function update_seenlist(data) {
+    stats = data["stats"];
+    if (stats.hasOwnProperty("SeenList") == false) {
+        return
+    }
     var seendiv = $("#seenDiv");
     var html_str = '<table class="ui celled striped table">'
     html_str += '<thead><tr><th>HAM Callsign</th><th>Age since last seen by APRSD</th>'
     html_str += '<th>Number of packets RX</th></tr></thead><tbody>'
     seendiv.html('')
-    var seen_list = data["stats"]["aprsd"]["seen_list"]
+    var seen_list = stats["SeenList"]
     var len = Object.keys(seen_list).length
     $('#seen_count').html(len)
     jQuery.each(seen_list, function(i, val) {
         html_str += '<tr><td class="collapsing">'
         html_str += '<img id="callsign_' + i + '" class="aprsd_1"></img>' + i + '</td>'
         html_str += '<td>' + val["last"] + '</td>'
         html_str += '<td>' + val["count"] + '</td></tr>'
     });
     html_str += "</tbody></table>";
     seendiv.append(html_str);
 }
 
 function update_plugins(data) {
+    stats = data["stats"];
+    if (stats.hasOwnProperty("PluginManager") == false) {
+        return
+    }
     var plugindiv = $("#pluginDiv");
     var html_str = '<table class="ui celled striped table"><thead><tr>'
     html_str += '<th>Plugin Name</th><th>Plugin Enabled?</th>'
     html_str += '<th>Processed Packets</th><th>Sent Packets</th>'
     html_str += '<th>Version</th>'
     html_str += '</tr></thead><tbody>'
     plugindiv.html('')
 
-    var plugins = data["stats"]["plugins"];
+    var plugins = stats["PluginManager"];
     var keys = Object.keys(plugins);
     keys.sort();
     for (var i = 0; i < keys.length; i++) { // now lets iterate in sort order
         var key = keys[i];
         var val = plugins[key];
         html_str += '<tr><td class="collapsing">' + key + '</td>';
         html_str += '<td>' + val["enabled"] + '</td><td>' + val["rx"] + '</td>';
         html_str += '<td>' + val["tx"] + '</td><td>' + val["version"] + '</td></tr>';
     }
     html_str += "</tbody></table>";
     plugindiv.append(html_str);
 }
 
+function update_threads(data) {
+    stats = data["stats"];
+    if (stats.hasOwnProperty("APRSDThreadList") == false) {
+        return
+    }
+    var threadsdiv = $("#threadsDiv");
+    var countdiv = $("#thread_count");
+    var html_str = '<table class="ui celled striped table"><thead><tr>'
+    html_str += '<th>Thread Name</th><th>Alive?</th>'
+    html_str += '<th>Age</th><th>Loop Count</th>'
+    html_str += '</tr></thead><tbody>'
+    threadsdiv.html('')
+
+    var threads = stats["APRSDThreadList"];
+    var keys = Object.keys(threads);
+    countdiv.html(keys.length);
+    keys.sort();
+    for (var i = 0; i < keys.length; i++) { // now lets iterate in sort order
+        var key = keys[i];
+        var val = threads[key];
+        html_str += '<tr><td class="collapsing">' + key + '</td>';
+        html_str += '<td>' + val["alive"] + '</td><td>' + val["age"] + '</td>';
+        html_str += '<td>' + val["loop_count"] + '</td></tr>';
+    }
+    html_str += "</tbody></table>";
+    threadsdiv.append(html_str);
+}
+
 function update_packets(data) {
     var packetsdiv = $("#packetsDiv");
     //nuke the contents first, then add to it.
     if (size_dict(packet_list) == 0 && size_dict(data) > 0) {
         packetsdiv.html('')
     }
-    jQuery.each(data, function(i, val) {
-        pkt = JSON.parse(val);
+    jQuery.each(data.packets, function(i, val) {
+        pkt = val;
 
         update_watchlist_from_packet(pkt['from_call'], pkt);
         if (packet_list.hasOwnProperty(pkt['timestamp']) == false) {
             // Store the packet
             packet_list[pkt['timestamp']] = pkt;
             //ts_str = val["timestamp"].toString();
             //ts = ts_str.split(".")[0]*1000;
@@ -165,14 +205,15 @@
             type: 'GET',
             dataType: 'json',
             success: function(data) {
                 update_stats(data);
                 update_watchlist(data);
                 update_seenlist(data);
                 update_plugins(data);
+                update_threads(data);
             },
             complete: function() {
                 setTimeout(statsworker, 10000);
             }
         });
     })();
```

### Comparing `aprsd-3.3.4/aprsd/web/admin/static/js/send-message.js` & `aprsd-3.4.0/aprsd/web/admin/static/js/send-message.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/admin/static/js/tabs.js` & `aprsd-3.4.0/aprsd/web/admin/static/js/tabs.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/admin/templates/index.html` & `aprsd-3.4.0/aprsd/web/admin/templates/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,14 @@
             var initial_stats = {{ initial_stats|tojson|safe }};
 
             var memory_chart = null
             var message_chart = null
             var color = Chart.helpers.color;
 
             $(document).ready(function() {
-                console.log(initial_stats);
                 start_update();
                 start_charts();
                 init_messages();
                 init_logs();
 
                 $("#toggleStats").click(function() {
                     $("#jsonstats").fadeToggle(1000);
@@ -78,14 +77,15 @@
         <!-- Tab links -->
         <div class="ui top attached tabular menu">
             <div class="active item" data-tab="charts-tab">Charts</div>
             <div class="item" data-tab="msgs-tab">Messages</div>
             <div class="item" data-tab="seen-tab">Seen List</div>
             <div class="item" data-tab="watch-tab">Watch List</div>
             <div class="item" data-tab="plugin-tab">Plugins</div>
+            <div class="item" data-tab="threads-tab">Threads</div>
             <div class="item" data-tab="config-tab">Config</div>
             <div class="item" data-tab="log-tab">LogFile</div>
             <!-- <div class="item" data-tab="oslo-tab">OSLO CONFIG</div> //-->
             <div class="item" data-tab="raw-tab">Raw JSON</div>
         </div>
 
         <!-- Tab content -->
@@ -95,29 +95,33 @@
                 <div class="row">
                     <div class="column">
                         <div class="ui segment" style="height: 300px" id="packetsChart"></div>
                     </div>
                 </div>
                 <div class="row">
                     <div class="column">
-                        <div class="ui segment" style="height: 300px" id="packetTypesChart"></div>
+                        <div class="ui segment" style="height: 300px" id="messagesChart"></div>
+                    </div>
+                    <div class="column">
+                        <div class="ui segment" style="height: 300px" id="acksChart"></div>
                     </div>
                 </div>
                 <div class="row">
                     <div class="column">
-                        <div class="ui segment" style="height: 300px" id="messagesChart"></div>
+                        <div class="ui segment" style="height: 300px" id="packetTypesChart"></div>
                     </div>
+                </div>
+                <div class="row">
                     <div class="column">
-                        <div class="ui segment" style="height: 300px" id="acksChart"></div>
+                        <div class="ui segment" style="height: 300px" id="threadChart"></div>
                     </div>
                 </div>
                 <div class="row">
                     <div class="column">
-                        <div class="ui segment" style="height: 300px" id="memChart">
-                        </div>
+                        <div class="ui segment" style="height: 300px" id="memChart"></div>
                     </div>
                 </div>
           <!--      <div class="row">
                     <div id="stats" class="two column">
                         <button class="ui button" id="toggleStats">Toggle raw json</button>
                         <pre id="jsonstats" class="language-json">{{ stats }}</pre>
                     </div> //-->
@@ -152,14 +156,21 @@
         <div class="ui bottom attached tab segment" data-tab="plugin-tab">
             <h3 class="ui dividing header">
                 Plugins Loaded (<span id="plugin_count">{{ plugin_count }}</span>)
             </h3>
             <div id="pluginDiv" class="ui mini text">Loading</div>
         </div>
 
+        <div class="ui bottom attached tab segment" data-tab="threads-tab">
+            <h3 class="ui dividing header">
+                Threads Loaded (<span id="thread_count">{{ thread_count }}</span>)
+            </h3>
+            <div id="threadsDiv" class="ui mini text">Loading</div>
+        </div>
+
         <div class="ui bottom attached tab segment" data-tab="config-tab">
           <h3 class="ui dividing header">Config</h3>
           <pre id="configjson" class="language-json">{{ config_json|safe }}</pre>
         </div>
 
         <div class="ui bottom attached tab segment" data-tab="log-tab">
             <h3 class="ui dividing header">LOGFILE</h3>
@@ -170,15 +181,15 @@
         <div class="ui bottom attached tab segment" data-tab="oslo-tab">
             <h3 class="ui dividing header">OSLO</h3>
             <pre id="osloContainer" style="height:600px;overflow-y:auto;" class="language-json">{{ oslo_out|safe }}</pre>
         </div> //-->
 
         <div class="ui bottom attached tab segment" data-tab="raw-tab">
           <h3 class="ui dividing header">Raw JSON</h3>
-          <pre id="jsonstats" class="language-yaml" style="height:600px;overflow-y:auto;">{{ stats|safe }}</pre>
+          <pre id="jsonstats" class="language-yaml" style="height:600px;overflow-y:auto;">{{ initial_stats|safe }}</pre>
         </div>
 
         <div class="ui text container">
             <a href="https://badge.fury.io/py/aprsd"><img src="https://badge.fury.io/py/aprsd.svg" alt="PyPI version" height="18"></a>
             <a href="https://github.com/craigerl/aprsd"><img src="https://img.shields.io/badge/Made%20with-Python-1f425f.svg" height="18"></a>
         </div>
     </body>
```

#### html2text {}

```diff
@@ -2,26 +2,29 @@
 {{ callsign }} connected to {{ aprs_connection|safe }}
 NONE
 Charts
 Messages
 Seen List
 Watch List
 Plugins
+Threads
 Config
 LogFile
 Raw JSON
 ******** CChhaarrttss ********
 ******** MMeessssaaggeess ((00)) ********
 Loading
 ******** CCaallllssiiggnn SSeeeenn LLiisstt (({{{{ sseeeenn__ccoouunntt }}}})) ********
 Loading
 ******** CCaallllssiiggnn WWaattcchh LLiisstt (({{{{ wwaattcchh__ccoouunntt }}}})) ? ? ?  NNoottiiffiiccaattiioonn aaggee -- {{
 {{ wwaattcchh__aaggee }}}} ********
 Loading
 ******** PPlluuggiinnss LLooaaddeedd (({{{{ pplluuggiinn__ccoouunntt }}}})) ********
 Loading
+******** TThhrreeaaddss LLooaaddeedd (({{{{ tthhrreeaadd__ccoouunntt }}}})) ********
+Loading
 ******** CCoonnffiigg ********
 {{ config_json|safe }}
 ******** LLOOGGFFIILLEE ********
 ******** RRaaww JJSSOONN ********
-{{ stats|safe }}
+{{ initial_stats|safe }}
 _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_M_a_d_e_%_2_0_w_i_t_h_-_P_y_t_h_o_n_-_1_f_4_2_5_f_._s_v_g_]
```

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/chat.css` & `aprsd-3.4.0/aprsd/web/chat/static/css/chat.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/index.css` & `aprsd-3.4.0/aprsd/web/chat/static/css/index.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/style.css.map` & `aprsd-3.4.0/aprsd/web/chat/static/css/style.css.map`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/tabs.css` & `aprsd-3.4.0/aprsd/web/chat/static/css/tabs.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/bootstrap.min.css` & `aprsd-3.4.0/aprsd/web/chat/static/css/upstream/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/font.woff2` & `aprsd-3.4.0/aprsd/web/chat/static/css/upstream/font.woff2`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/google-fonts.css` & `aprsd-3.4.0/aprsd/web/chat/static/css/upstream/google-fonts.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/jquery-ui.css` & `aprsd-3.4.0/aprsd/web/chat/static/css/upstream/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/jquery.toast.css` & `aprsd-3.4.0/aprsd/web/chat/static/css/upstream/jquery.toast.css`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff` & `aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff2` & `aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Bold.woff2`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff` & `aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff2` & `aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/LatoLatin-Regular.woff2`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff` & `aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff2` & `aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/icons.woff2`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff` & `aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff2` & `aprsd-3.4.0/aprsd/web/chat/static/css/upstream/themes/default/assets/fonts/outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/images/Untitled.png` & `aprsd-3.4.0/aprsd/web/chat/static/images/Untitled.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-16-0.png` & `aprsd-3.4.0/aprsd/web/chat/static/images/aprs-symbols-16-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-16-1.png` & `aprsd-3.4.0/aprsd/web/chat/static/images/aprs-symbols-16-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-64-0.png` & `aprsd-3.4.0/aprsd/web/chat/static/images/aprs-symbols-64-0.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-64-1.png` & `aprsd-3.4.0/aprsd/web/chat/static/images/aprs-symbols-64-1.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/images/aprs-symbols-64-2.png` & `aprsd-3.4.0/aprsd/web/chat/static/images/aprs-symbols-64-2.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/images/globe.svg` & `aprsd-3.4.0/aprsd/web/chat/static/images/globe.svg`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/js/gps.js` & `aprsd-3.4.0/aprsd/web/chat/static/js/gps.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -65,17 +65,19 @@
         showProgress: 'top',
         classProgress: 'blue',
     });
 }
 
 function showPosition(position) {
     console.log("showPosition Called");
+    path = $('#pkt_path option:selected').val();
     msg = {
         'latitude': position.coords.latitude,
-        'longitude': position.coords.longitude
+        'longitude': position.coords.longitude,
+        'path': path,
     }
     console.log(msg);
     $.toast({
         heading: 'Sending GPS Beacon',
         text: "Latitude: " + position.coords.latitude + "<br>Longitude: " + position.coords.longitude,
         loader: true,
         loaderBg: '#9EC600',
```

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/js/main.js` & `aprsd-3.4.0/aprsd/web/chat/static/js/main.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -17,17 +17,18 @@
 }
 
 function ord(str) {
     return str.charCodeAt(0);
 }
 
 function update_stats(data) {
-    $("#version").text(data["stats"]["aprsd"]["version"]);
+    console.log(data);
+    $("#version").text(data["stats"]["APRSDStats"]["version"]);
     $("#aprs_connection").html(data["aprs_connection"]);
-    $("#uptime").text("uptime: " + data["stats"]["aprsd"]["uptime"]);
+    $("#uptime").text("uptime: " + data["stats"]["APRSDStats"]["uptime"]);
     short_time = data["time"].split(/\s(.+)/)[1];
 }
 
 
 function start_update() {
 
     (function statsworker() {
@@ -35,12 +36,12 @@
             url: "/stats",
             type: 'GET',
             dataType: 'json',
             success: function(data) {
                 update_stats(data);
             },
             complete: function() {
-                setTimeout(statsworker, 10000);
+                setTimeout(statsworker, 60000);
             }
         });
     })();
 }
```

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/js/send-message.js` & `aprsd-3.4.0/aprsd/web/chat/static/js/send-message.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -333,14 +333,15 @@
         active_str = "";
     }
 
     item_html = '<li class="nav-item" role="presentation" callsign="' + callsign + '" id="' + tab_id_li + '">';
     //item_html += '<button onClick="callsign_select(\''+callsign+'\');" callsign="'+callsign+'" class="nav-link '+active_str+'" id="'+tab_id+'" data-bs-toggle="tab" data-bs-target="#'+tab_content+'" type="button" role="tab" aria-controls="'+callsign+'" aria-selected="true">';
     item_html += '<button onClick="callsign_select(\'' + callsign + '\');" callsign="' + callsign + '" class="nav-link position-relative ' + active_str + '" id="' + tab_id + '" data-bs-toggle="tab" data-bs-target="#' + tab_content + '" type="button" role="tab" aria-controls="' + callsign + '" aria-selected="true">';
     item_html += callsign + '&nbsp;&nbsp;';
+    item_html += '<span id="' + tab_notify_id + '" class="position-absolute top-0 start-80 translate-middle badge bg-danger border border-light rounded-pill visually-hidden">0</span>';
     item_html += '<span onclick="delete_tab(\'' + callsign + '\');">×</span>';
     item_html += '</button></li>'
 
     callsignTabs.append(item_html);
     create_callsign_tab_content(callsign, active);
 }
 
@@ -427,21 +428,23 @@
     id = ts_id['id']
     message_list[callsign][id] = msg;
     if (selected_tab_callsign != callsign) {
         // We need to update the notification for the tab
         tab_notify_id = tab_notification_id(callsign, true);
         // get the current count of notifications
         count = parseInt($(tab_notify_id).text());
+        if (isNaN(count)) {
+            count = 0;
+        }
         count += 1;
         $(tab_notify_id).text(count);
         $(tab_notify_id).removeClass('visually-hidden');
     }
 
     // Find the right div to place the html
-
     new_callsign = add_callsign(callsign, msg);
     update_callsign_path(callsign, msg);
     append_message_html(callsign, msg_html, new_callsign);
     len = Object.keys(callsign_list).length;
     if (new_callsign && len == 1) {
         //Now click the tab if and only if there is only one tab
         callsign_tab_id = callsign_tab(callsign);
@@ -524,15 +527,15 @@
     t = info['time'];
     d = info['date'];
     ack_id = info['ack_id'];
 
     msg_html = create_message_html(d, t, msg['from_call'], msg['to_call'], msg['message_text'], ack_id, msg, false);
     append_message(msg['to_call'], msg, msg_html);
     save_data();
-    scroll_main_content(msg['from_call']);
+    scroll_main_content(msg['to_call']);
 }
 
 function from_msg(msg) {
     if (!from_msg_list.hasOwnProperty(msg["from_call"])) {
         from_msg_list[msg["from_call"]] = new Array();
     }
```

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/js/tabs.js` & `aprsd-3.4.0/aprsd/web/chat/static/js/tabs.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/js/upstream/bootstrap.bundle.min.js` & `aprsd-3.4.0/aprsd/web/chat/static/js/upstream/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/js/upstream/jquery-3.7.1.min.js` & `aprsd-3.4.0/aprsd/web/chat/static/js/upstream/jquery-3.7.1.min.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/js/upstream/jquery-ui.min.js` & `aprsd-3.4.0/aprsd/web/chat/static/js/upstream/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/js/upstream/jquery.toast.js` & `aprsd-3.4.0/aprsd/web/chat/static/js/upstream/jquery.toast.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/js/upstream/semantic.min.js` & `aprsd-3.4.0/aprsd/web/chat/static/js/upstream/semantic.min.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/static/js/upstream/socket.io.min.js` & `aprsd-3.4.0/aprsd/web/chat/static/js/upstream/socket.io.min.js`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd/web/chat/templates/index.html` & `aprsd-3.4.0/aprsd/web/chat/templates/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
                         <div class="col-auto">
                             <label for="pkt_path" class="visually-hidden">PATH</label>
                             <select class="form-control mb-2 mr-sm-2" name="pkt_path" id="pkt_path" style="width:auto;">
                                 <option value="" disabled selected>Default Path</option>
                                 <option value="WIDE1-1">WIDE1-1</option>
                                 <option value="WIDE1-1,WIDE2-1">WIDE1-1,WIDE2-1</option>
                                 <option value="ARISS">ARISS</option>
+                                <option value="GATE">GATE</option>
                             </select>
                         </div>
                         <div class="col-sm-3">
                             <label for="message" class="visually-hidden">Message</label>
                             <input type="search" class="form-control mb-2 mr-sm-2" name="message" id="message" size="40" maxlength="67" placeholder="Message">
                         </div>
                         <div class="col-auto">
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 ************ AAPPRRSSDD WWeebbCChhaatt {{{{ vveerrssiioonn }}}} ************
 {{ callsign }} connected to {{ aprs_connection|safe }} NONE
 Callsign[Unknown INPUT type]
-PATH[One of: Default Path/WIDE1-1/WIDE1-1,WIDE2-1/ARISS]
+PATH[One of: Default Path/WIDE1-1/WIDE1-1,WIDE2-1/ARISS/GATE]
 Message[Unknown INPUT type]
 [Send]Send Position
 _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_M_a_d_e_%_2_0_w_i_t_h_-_P_y_t_h_o_n_-_1_f_4_2_5_f_._s_v_g_]
```

### Comparing `aprsd-3.3.4/aprsd/wsgi.py` & `aprsd-3.4.0/aprsd/wsgi.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import datetime
 import importlib.metadata as imp
 import io
 import json
 import logging
-import time
+import queue
 
 import flask
-from flask import Flask
+from flask import Flask, request
 from flask_httpauth import HTTPBasicAuth
 from oslo_config import cfg, generator
 import socketio
 from werkzeug.security import check_password_hash
 
 import aprsd
 from aprsd import cli_helper, client, conf, packets, plugin, threads
 from aprsd.log import log
-from aprsd.rpc import client as aprsd_rpc_client
+from aprsd.threads import stats as stats_threads
+from aprsd.utils import json as aprsd_json
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger("gunicorn.access")
+logging_queue = queue.Queue()
 
 auth = HTTPBasicAuth()
-users = {}
+users: dict[str, str] = {}
 app = Flask(
     "aprsd",
     static_url_path="/static",
     static_folder="web/admin/static",
     template_folder="web/admin/templates",
 )
 bg_thread = None
@@ -41,122 +43,48 @@
     global users
 
     if username in users and check_password_hash(users.get(username), password):
         return username
 
 
 def _stats():
-    track = aprsd_rpc_client.RPCClient().get_packet_track()
+    stats_obj = stats_threads.StatsStore()
+    stats_obj.load()
     now = datetime.datetime.now()
-
     time_format = "%m-%d-%Y %H:%M:%S"
-
-    stats_dict = aprsd_rpc_client.RPCClient().get_stats_dict()
-    if not stats_dict:
-        stats_dict = {
-            "aprsd": {},
-            "aprs-is": {"server": ""},
-            "messages": {
-                "sent": 0,
-                "received": 0,
-            },
-            "email": {
-                "sent": 0,
-                "received": 0,
-            },
-            "seen_list": {
-                "sent": 0,
-                "received": 0,
-            },
-        }
-
-    # Convert the watch_list entries to age
-    wl = aprsd_rpc_client.RPCClient().get_watch_list()
-    new_list = {}
-    if wl:
-        for call in wl.get_all():
-            # call_date = datetime.datetime.strptime(
-            #    str(wl.last_seen(call)),
-            #    "%Y-%m-%d %H:%M:%S.%f",
-            # )
-
-            # We have to convert the RingBuffer to a real list
-            # so that json.dumps works.
-            # pkts = []
-            # for pkt in wl.get(call)["packets"].get():
-            #     pkts.append(pkt)
-
-            new_list[call] = {
-                "last": wl.age(call),
-                # "packets": pkts
-            }
-
-    stats_dict["aprsd"]["watch_list"] = new_list
-    packet_list = aprsd_rpc_client.RPCClient().get_packet_list()
-    rx = tx = 0
-    types = {}
-    if packet_list:
-        rx = packet_list.total_rx()
-        tx = packet_list.total_tx()
-        types_copy = packet_list.types.copy()
-
-        for key in types_copy:
-            types[str(key)] = dict(types_copy[key])
-
-    stats_dict["packets"] = {
-        "sent": tx,
-        "received": rx,
-        "types": types,
-    }
-    if track:
-        size_tracker = len(track)
-    else:
-        size_tracker = 0
-
-    result = {
+    stats = {
         "time": now.strftime(time_format),
-        "size_tracker": size_tracker,
-        "stats": stats_dict,
+        "stats": stats_obj.data,
     }
-
-    return result
+    return stats
 
 
 @app.route("/stats")
 def stats():
     LOG.debug("/stats called")
-    return json.dumps(_stats())
+    return json.dumps(_stats(), cls=aprsd_json.SimpleJSONEncoder)
 
 
 @app.route("/")
 def index():
     stats = _stats()
-    wl = aprsd_rpc_client.RPCClient().get_watch_list()
-    if wl and wl.is_enabled():
-        watch_count = len(wl)
-        watch_age = wl.max_delta()
-    else:
-        watch_count = 0
-        watch_age = 0
-
-    sl = aprsd_rpc_client.RPCClient().get_seen_list()
-    if sl:
-        seen_count = len(sl)
-    else:
-        seen_count = 0
-
     pm = plugin.PluginManager()
     plugins = pm.get_plugins()
     plugin_count = len(plugins)
+    client_stats = stats["stats"].get("APRSClientStats", {})
 
     if CONF.aprs_network.enabled:
         transport = "aprs-is"
+        if client_stats:
+            aprs_connection = client_stats.get("server_string", "")
+        else:
+            aprs_connection = "APRS-IS"
         aprs_connection = (
             "APRS-IS Server: <a href='http://status.aprs2.net' >"
-            "{}</a>".format(stats["stats"]["aprs-is"]["server"])
+            "{}</a>".format(aprs_connection)
         )
     else:
         # We might be connected to a KISS socket?
         if client.KISSClient.kiss_enabled():
             transport = client.KISSClient.transport()
             if transport == client.TRANSPORT_TCPKISS:
                 aprs_connection = (
@@ -169,32 +97,37 @@
                 aprs_connection = (
                     "SerialKISS://{}@{} baud".format(
                         CONF.kiss_serial.device,
                         CONF.kiss_serial.baudrate,
                     )
                 )
 
-    stats["transport"] = transport
-    stats["aprs_connection"] = aprs_connection
+    if client_stats:
+        stats["stats"]["APRSClientStats"]["transport"] = transport
+        stats["stats"]["APRSClientStats"]["aprs_connection"] = aprs_connection
     entries = conf.conf_to_dict()
 
+    thread_info = stats["stats"].get("APRSDThreadList", {})
+    if thread_info:
+        thread_count = len(thread_info)
+    else:
+        thread_count = "unknown"
+
     return flask.render_template(
         "index.html",
-        initial_stats=stats,
+        initial_stats=json.dumps(stats, cls=aprsd_json.SimpleJSONEncoder),
         aprs_connection=aprs_connection,
         callsign=CONF.callsign,
         version=aprsd.__version__,
         config_json=json.dumps(
             entries, indent=4,
             sort_keys=True, default=str,
         ),
-        watch_count=watch_count,
-        watch_age=watch_age,
-        seen_count=seen_count,
         plugin_count=plugin_count,
+        thread_count=thread_count,
         # oslo_out=generate_oslo()
     )
 
 
 @auth.login_required
 def messages():
     track = packets.PacketTrack()
@@ -205,27 +138,18 @@
 
     return flask.render_template("messages.html", messages=json.dumps(msgs))
 
 
 @auth.login_required
 @app.route("/packets")
 def get_packets():
-    LOG.debug("/packets called")
-    packet_list = aprsd_rpc_client.RPCClient().get_packet_list()
-    if packet_list:
-        tmp_list = []
-        pkts = packet_list.copy()
-        for key in pkts:
-            pkt = packet_list.get(key)
-            if pkt:
-                tmp_list.append(pkt.json)
-
-        return json.dumps(tmp_list)
-    else:
-        return json.dumps([])
+    stats = _stats()
+    stats_dict = stats["stats"]
+    packets = stats_dict.get("PacketList", {})
+    return json.dumps(packets, cls=aprsd_json.SimpleJSONEncoder)
 
 
 @auth.login_required
 @app.route("/plugins")
 def plugins():
     LOG.debug("/plugins called")
     pm = plugin.PluginManager()
@@ -269,49 +193,60 @@
 def save():
     """Save the existing queue to disk."""
     track = packets.PacketTrack()
     track.save()
     return json.dumps({"messages": "saved"})
 
 
+@app.route("/log_entries", methods=["POST"])
+def log_entries():
+    """The url that the server can call to update the logs."""
+    entries = request.json
+    LOG.info(f"Log entries called {len(entries)}")
+    for entry in entries:
+        logging_queue.put(entry)
+    return json.dumps({"messages": "saved"})
+
+
 class LogUpdateThread(threads.APRSDThread):
 
-    def __init__(self):
+    def __init__(self, logging_queue=None):
         super().__init__("LogUpdate")
+        self.logging_queue = logging_queue
 
     def loop(self):
         if sio:
-            log_entries = aprsd_rpc_client.RPCClient().get_log_entries()
-
-            if log_entries:
-                LOG.info(f"Sending log entries! {len(log_entries)}")
-                for entry in log_entries:
+            try:
+                log_entry = self.logging_queue.get(block=True, timeout=1)
+                if log_entry:
                     sio.emit(
-                        "log_entry", entry,
+                        "log_entry",
+                        log_entry,
                         namespace="/logs",
                     )
-        time.sleep(5)
+            except queue.Empty:
+                pass
         return True
 
 
 class LoggingNamespace(socketio.Namespace):
     log_thread = None
 
     def on_connect(self, sid, environ):
-        global sio
-        LOG.debug(f"LOG on_connect {sid}")
+        global sio, logging_queue
+        LOG.info(f"LOG on_connect {sid}")
         sio.emit(
             "connected", {"data": "/logs Connected"},
             namespace="/logs",
         )
-        self.log_thread = LogUpdateThread()
+        self.log_thread = LogUpdateThread(logging_queue=logging_queue)
         self.log_thread.start()
 
     def on_disconnect(self, sid):
-        LOG.debug(f"LOG Disconnected {sid}")
+        LOG.info(f"LOG Disconnected {sid}")
         if self.log_thread:
             self.log_thread.stop()
 
 
 def init_app(config_file=None, log_level=None):
     default_config_file = cli_helper.DEFAULT_CONFIG_FILE
     if not config_file:
@@ -328,16 +263,16 @@
     return log_level
 
 
 if __name__ == "__main__":
     async_mode = "threading"
     sio = socketio.Server(logger=True, async_mode=async_mode)
     app.wsgi_app = socketio.WSGIApp(sio, app.wsgi_app)
-    log_level = init_app(log_level="DEBUG")
-    log.setup_logging(app, log_level)
+    log_level = init_app()
+    log.setup_logging(log_level)
     sio.register_namespace(LoggingNamespace("/logs"))
     CONF.log_opt_values(LOG, logging.DEBUG)
     app.run(
         threaded=True,
         debug=False,
         port=CONF.admin.web_port,
         host=CONF.admin.web_ip,
@@ -348,33 +283,33 @@
     # Start with
     # uwsgi --http :8000 --gevent 1000 --http-websockets --master -w aprsd.wsgi --callable app
 
     async_mode = "gevent_uwsgi"
     sio = socketio.Server(logger=True, async_mode=async_mode)
     app.wsgi_app = socketio.WSGIApp(sio, app.wsgi_app)
     log_level = init_app(
-        log_level="DEBUG",
+        # log_level="DEBUG",
         config_file="/config/aprsd.conf",
         # Commented out for local development.
         # config_file=cli_helper.DEFAULT_CONFIG_FILE
     )
-    log.setup_logging(app, log_level)
+    log.setup_logging(log_level)
     sio.register_namespace(LoggingNamespace("/logs"))
     CONF.log_opt_values(LOG, logging.DEBUG)
 
 
 if __name__ == "aprsd.wsgi":
     # set async_mode to 'threading', 'eventlet', 'gevent' or 'gevent_uwsgi' to
     # force a mode else, the best mode is selected automatically from what's
     # installed
     async_mode = "gevent_uwsgi"
     sio = socketio.Server(logger=True, async_mode=async_mode)
     app.wsgi_app = socketio.WSGIApp(sio, app.wsgi_app)
 
     log_level = init_app(
-        log_level="DEBUG",
+        # log_level="DEBUG",
         config_file="/config/aprsd.conf",
         # config_file=cli_helper.DEFAULT_CONFIG_FILE,
     )
-    log.setup_logging(app, log_level)
+    log.setup_logging(log_level)
     sio.register_namespace(LoggingNamespace("/logs"))
     CONF.log_opt_values(LOG, logging.DEBUG)
```

### Comparing `aprsd-3.3.4/aprsd-lnav.json` & `aprsd-3.4.0/aprsd-lnav.json`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/aprsd.egg-info/PKG-INFO` & `aprsd-3.4.0/aprsd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aprsd
-Version: 3.3.4
+Version: 3.4.0
 Summary: Amateur radio APRS daemon which listens for messages and responds
 Home-page: http://aprsd.readthedocs.org
 Author: Craig Lamparter
 Author-email: something@somewhere.com
 License: Apache
 Project-URL: Source, https://github.com/craigerl/aprsd
 Project-URL: Tracker, https://github.com/craigerl/aprsd/issues
@@ -27,76 +27,74 @@
 Requires-Dist: blinker==1.7.0
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: click==8.1.7
 Requires-Dist: click-completion==0.5.2
 Requires-Dist: click-params==0.5.0
 Requires-Dist: commonmark==0.9.1
-Requires-Dist: dacite2==2.0.0
 Requires-Dist: dataclasses==0.6
 Requires-Dist: dataclasses-json==0.6.4
 Requires-Dist: debtcollector==3.0.0
 Requires-Dist: deprecated==1.2.14
 Requires-Dist: dnspython==2.6.1
-Requires-Dist: eventlet==0.35.2
-Requires-Dist: flask==3.0.2
+Requires-Dist: eventlet==0.36.1
+Requires-Dist: flask==3.0.3
 Requires-Dist: flask-httpauth==4.8.0
 Requires-Dist: flask-socketio==5.3.6
 Requires-Dist: geographiclib==2.0
 Requires-Dist: geopy==2.4.1
 Requires-Dist: gevent==24.2.1
 Requires-Dist: greenlet==3.0.3
 Requires-Dist: h11==0.14.0
-Requires-Dist: idna==3.6
+Requires-Dist: idna==3.7
 Requires-Dist: imapclient==3.0.1
-Requires-Dist: importlib-metadata==7.0.1
-Requires-Dist: itsdangerous==2.1.2
+Requires-Dist: importlib-metadata==7.1.0
+Requires-Dist: itsdangerous==2.2.0
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: kiss3==8.0.0
 Requires-Dist: loguru==0.7.2
 Requires-Dist: markupsafe==2.1.5
 Requires-Dist: marshmallow==3.21.1
 Requires-Dist: mypy-extensions==1.0.0
 Requires-Dist: netaddr==1.2.1
 Requires-Dist: oslo-config==9.4.0
 Requires-Dist: oslo-i18n==6.3.0
-Requires-Dist: packaging==23.2
+Requires-Dist: packaging==24.0
 Requires-Dist: pbr==6.0.0
-Requires-Dist: pluggy==1.4.0
-Requires-Dist: plumbum==1.8.2
+Requires-Dist: pluggy==1.5.0
 Requires-Dist: pygments==2.17.2
 Requires-Dist: pyserial==3.5
 Requires-Dist: pyserial-asyncio==0.6
 Requires-Dist: python-engineio==4.9.0
-Requires-Dist: python-socketio==5.11.1
+Requires-Dist: python-socketio==5.11.2
 Requires-Dist: pytz==2024.1
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: rfc3986==2.0.0
 Requires-Dist: rich==12.6.0
-Requires-Dist: rpyc==6.0.0
 Requires-Dist: rush==2021.4.0
 Requires-Dist: shellingham==1.5.4
 Requires-Dist: simple-websocket==1.0.0
 Requires-Dist: six==1.16.0
 Requires-Dist: soupsieve==2.5
 Requires-Dist: stevedore==5.2.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: thesmuggler==1.0.1
-Requires-Dist: typing-extensions==4.10.0
+Requires-Dist: typing-extensions==4.11.0
 Requires-Dist: typing-inspect==0.9.0
+Requires-Dist: tzlocal==5.2
 Requires-Dist: update-checker==0.18.0
 Requires-Dist: urllib3==2.2.1
 Requires-Dist: validators==0.22.0
-Requires-Dist: werkzeug==3.0.1
+Requires-Dist: werkzeug==3.0.2
 Requires-Dist: wrapt==1.16.0
 Requires-Dist: wsproto==1.2.0
-Requires-Dist: zipp==3.17.0
+Requires-Dist: zipp==3.18.1
 Requires-Dist: zope-event==5.0
-Requires-Dist: zope-interface==6.2
+Requires-Dist: zope-interface==6.3
 
 ===============================================
 APRSD - Ham radio APRS-IS Message plugin server
 ===============================================
 
 KM6LYW and WB4BOR
 ____________________
```

### Comparing `aprsd-3.3.4/aprsd.egg-info/SOURCES.txt` & `aprsd-3.4.0/aprsd.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 aprsd/cli_helper.py
 aprsd/client.py
 aprsd/exception.py
 aprsd/main.py
 aprsd/messaging.py
 aprsd/plugin.py
 aprsd/plugin_utils.py
-aprsd/stats.py
 aprsd/wsgi.py
 aprsd.egg-info/PKG-INFO
 aprsd.egg-info/SOURCES.txt
 aprsd.egg-info/dependency_links.txt
 aprsd.egg-info/entry_points.txt
 aprsd.egg-info/not-zip-safe
 aprsd.egg-info/pbr.json
@@ -61,38 +60,40 @@
 aprsd/conf/log.py
 aprsd/conf/opts.py
 aprsd/conf/plugin_common.py
 aprsd/conf/plugin_email.py
 aprsd/log/__init__.py
 aprsd/log/log.py
 aprsd/packets/__init__.py
+aprsd/packets/collector.py
 aprsd/packets/core.py
+aprsd/packets/log.py
 aprsd/packets/packet_list.py
 aprsd/packets/seen_list.py
 aprsd/packets/tracker.py
 aprsd/packets/watch_list.py
 aprsd/plugins/__init__.py
 aprsd/plugins/email.py
 aprsd/plugins/fortune.py
 aprsd/plugins/location.py
 aprsd/plugins/notify.py
 aprsd/plugins/ping.py
-aprsd/plugins/query.py
 aprsd/plugins/time.py
 aprsd/plugins/version.py
 aprsd/plugins/weather.py
-aprsd/rpc/__init__.py
-aprsd/rpc/client.py
-aprsd/rpc/server.py
+aprsd/stats/__init__.py
+aprsd/stats/app.py
+aprsd/stats/collector.py
 aprsd/threads/__init__.py
 aprsd/threads/aprsd.py
 aprsd/threads/keep_alive.py
 aprsd/threads/log_monitor.py
 aprsd/threads/registry.py
 aprsd/threads/rx.py
+aprsd/threads/stats.py
 aprsd/threads/tx.py
 aprsd/utils/__init__.py
 aprsd/utils/counter.py
 aprsd/utils/fuzzyclock.py
 aprsd/utils/json.py
 aprsd/utils/objectstore.py
 aprsd/utils/ring_buffer.py
@@ -111,16 +112,14 @@
 aprsd/web/admin/static/js/charts.js
 aprsd/web/admin/static/js/echarts.js
 aprsd/web/admin/static/js/logs.js
 aprsd/web/admin/static/js/main.js
 aprsd/web/admin/static/js/prism.js
 aprsd/web/admin/static/js/send-message.js
 aprsd/web/admin/static/js/tabs.js
-aprsd/web/admin/static/json-viewer/jquery.json-viewer.css
-aprsd/web/admin/static/json-viewer/jquery.json-viewer.js
 aprsd/web/admin/templates/index.html
 aprsd/web/chat/static/css/chat.css
 aprsd/web/chat/static/css/index.css
 aprsd/web/chat/static/css/style.css.map
 aprsd/web/chat/static/css/tabs.css
 aprsd/web/chat/static/css/upstream/bootstrap.min.css
 aprsd/web/chat/static/css/upstream/font.woff2
@@ -148,24 +147,23 @@
 aprsd/web/chat/static/js/tabs.js
 aprsd/web/chat/static/js/upstream/bootstrap.bundle.min.js
 aprsd/web/chat/static/js/upstream/jquery-3.7.1.min.js
 aprsd/web/chat/static/js/upstream/jquery-ui.min.js
 aprsd/web/chat/static/js/upstream/jquery.toast.js
 aprsd/web/chat/static/js/upstream/semantic.min.js
 aprsd/web/chat/static/js/upstream/socket.io.min.js
-aprsd/web/chat/static/json-viewer/jquery.json-viewer.css
-aprsd/web/chat/static/json-viewer/jquery.json-viewer.js
 aprsd/web/chat/templates/index.html
 docker/Dockerfile
 docker/Dockerfile-dev
 docker/build.sh
 docker/docker-compose.yml
 docker/bin/admin.sh
 docker/bin/listen.sh
 docker/bin/run.sh
+docker/bin/setup.sh
 docs/aprsd.drawio
 docs/changelog.rst
 docs/clean_docs.py
 docs/conf.py
 docs/configure.rst
 docs/index.rst
 docs/install.rst
@@ -201,12 +199,11 @@
 tests/cmds/test_send_message.py
 tests/cmds/test_webchat.py
 tests/plugins/__init__.py
 tests/plugins/test_fortune.py
 tests/plugins/test_location.py
 tests/plugins/test_notify.py
 tests/plugins/test_ping.py
-tests/plugins/test_query.py
 tests/plugins/test_time.py
 tests/plugins/test_version.py
 tests/plugins/test_weather.py
 tools/fast8.sh
```

### Comparing `aprsd-3.3.4/aprsd.egg-info/requires.txt` & `aprsd-3.4.0/aprsd.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,69 +7,67 @@
 blinker==1.7.0
 certifi==2024.2.2
 charset-normalizer==3.3.2
 click==8.1.7
 click-completion==0.5.2
 click-params==0.5.0
 commonmark==0.9.1
-dacite2==2.0.0
 dataclasses==0.6
 dataclasses-json==0.6.4
 debtcollector==3.0.0
 deprecated==1.2.14
 dnspython==2.6.1
-eventlet==0.35.2
-flask==3.0.2
+eventlet==0.36.1
+flask==3.0.3
 flask-httpauth==4.8.0
 flask-socketio==5.3.6
 geographiclib==2.0
 geopy==2.4.1
 gevent==24.2.1
 greenlet==3.0.3
 h11==0.14.0
-idna==3.6
+idna==3.7
 imapclient==3.0.1
-importlib-metadata==7.0.1
-itsdangerous==2.1.2
+importlib-metadata==7.1.0
+itsdangerous==2.2.0
 jinja2==3.1.3
 kiss3==8.0.0
 loguru==0.7.2
 markupsafe==2.1.5
 marshmallow==3.21.1
 mypy-extensions==1.0.0
 netaddr==1.2.1
 oslo-config==9.4.0
 oslo-i18n==6.3.0
-packaging==23.2
+packaging==24.0
 pbr==6.0.0
-pluggy==1.4.0
-plumbum==1.8.2
+pluggy==1.5.0
 pygments==2.17.2
 pyserial==3.5
 pyserial-asyncio==0.6
 python-engineio==4.9.0
-python-socketio==5.11.1
+python-socketio==5.11.2
 pytz==2024.1
 pyyaml==6.0.1
 requests==2.31.0
 rfc3986==2.0.0
 rich==12.6.0
-rpyc==6.0.0
 rush==2021.4.0
 shellingham==1.5.4
 simple-websocket==1.0.0
 six==1.16.0
 soupsieve==2.5
 stevedore==5.2.0
 tabulate==0.9.0
 thesmuggler==1.0.1
-typing-extensions==4.10.0
+typing-extensions==4.11.0
 typing-inspect==0.9.0
+tzlocal==5.2
 update-checker==0.18.0
 urllib3==2.2.1
 validators==0.22.0
-werkzeug==3.0.1
+werkzeug==3.0.2
 wrapt==1.16.0
 wsproto==1.2.0
-zipp==3.17.0
+zipp==3.18.1
 zope-event==5.0
-zope-interface==6.2
+zope-interface==6.3
```

### Comparing `aprsd-3.3.4/dev-requirements.txt` & `aprsd-3.4.0/dev-requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,81 +4,80 @@
 #
 #    pip-compile --annotation-style=line dev-requirements.in
 #
 add-trailing-comma==3.1.0  # via gray
 alabaster==0.7.16         # via sphinx
 autoflake==1.5.3          # via gray
 babel==2.14.0             # via sphinx
-black==24.2.0             # via gray
-build==1.1.1              # via pip-tools
+black==24.4.0             # via gray
+build==1.2.1              # via pip-tools
 cachetools==5.3.3         # via tox
 certifi==2024.2.2         # via requests
 cfgv==3.4.0               # via pre-commit
 chardet==5.2.0            # via tox
 charset-normalizer==3.3.2  # via requests
 click==8.1.7              # via black, fixit, moreorless, pip-tools
 colorama==0.4.6           # via tox
 commonmark==0.9.1         # via rich
 configargparse==1.7       # via gray
-coverage[toml]==7.4.3     # via pytest-cov
+coverage[toml]==7.5.0     # via pytest-cov
 distlib==0.3.8            # via virtualenv
-docutils==0.20.1          # via sphinx
-exceptiongroup==1.2.0     # via pytest
-filelock==3.13.1          # via tox, virtualenv
+docutils==0.21.2          # via sphinx
+exceptiongroup==1.2.1     # via pytest
+filelock==3.13.4          # via tox, virtualenv
 fixit==2.1.0              # via gray
 flake8==7.0.0             # via -r dev-requirements.in, pep8-naming
 gray==0.14.0              # via -r dev-requirements.in
-identify==2.5.35          # via pre-commit
-idna==3.6                 # via requests
+identify==2.5.36          # via pre-commit
+idna==3.7                 # via requests
 imagesize==1.4.1          # via sphinx
 iniconfig==2.0.0          # via pytest
 isort==5.13.2             # via -r dev-requirements.in, gray
 jinja2==3.1.3             # via sphinx
-libcst==1.2.0             # via fixit
+libcst==1.3.1             # via fixit
 markupsafe==2.1.5         # via jinja2
 mccabe==0.7.0             # via flake8
 moreorless==0.4.0         # via fixit
-mypy==1.8.0               # via -r dev-requirements.in
-mypy-extensions==1.0.0    # via black, mypy, typing-inspect
+mypy==1.9.0               # via -r dev-requirements.in
+mypy-extensions==1.0.0    # via black, mypy
 nodeenv==1.8.0            # via pre-commit
-packaging==23.2           # via black, build, fixit, pyproject-api, pytest, sphinx, tox
+packaging==24.0           # via black, build, fixit, pyproject-api, pytest, sphinx, tox
 pathspec==0.12.1          # via black, trailrunner
 pep8-naming==0.13.3       # via -r dev-requirements.in
 pip-tools==7.4.1          # via -r dev-requirements.in
-platformdirs==4.2.0       # via black, tox, virtualenv
-pluggy==1.4.0             # via pytest, tox
-pre-commit==3.6.2         # via -r dev-requirements.in
+platformdirs==4.2.1       # via black, tox, virtualenv
+pluggy==1.5.0             # via pytest, tox
+pre-commit==3.7.0         # via -r dev-requirements.in
 pycodestyle==2.11.1       # via flake8
 pyflakes==3.2.0           # via autoflake, flake8
 pygments==2.17.2          # via rich, sphinx
 pyproject-api==1.6.1      # via tox
 pyproject-hooks==1.0.0    # via build, pip-tools
-pytest==8.0.2             # via -r dev-requirements.in, pytest-cov
-pytest-cov==4.1.0         # via -r dev-requirements.in
-pyupgrade==3.15.1         # via gray
+pytest==8.1.1             # via -r dev-requirements.in, pytest-cov
+pytest-cov==5.0.0         # via -r dev-requirements.in
+pyupgrade==3.15.2         # via gray
 pyyaml==6.0.1             # via libcst, pre-commit
 requests==2.31.0          # via sphinx
 rich==12.6.0              # via gray
 snowballstemmer==2.2.0    # via sphinx
-sphinx==7.2.6             # via -r dev-requirements.in
+sphinx==7.3.7             # via -r dev-requirements.in
 sphinxcontrib-applehelp==1.0.8  # via sphinx
 sphinxcontrib-devhelp==1.0.6  # via sphinx
 sphinxcontrib-htmlhelp==2.0.5  # via sphinx
 sphinxcontrib-jsmath==1.0.1  # via sphinx
 sphinxcontrib-qthelp==1.0.7  # via sphinx
 sphinxcontrib-serializinghtml==1.1.10  # via sphinx
 tokenize-rt==5.2.0        # via add-trailing-comma, pyupgrade
 toml==0.10.2              # via autoflake
-tomli==2.0.1              # via black, build, coverage, fixit, mypy, pip-tools, pyproject-api, pyproject-hooks, pytest, tox
-tox==4.14.0               # via -r dev-requirements.in
+tomli==2.0.1              # via black, build, coverage, fixit, mypy, pip-tools, pyproject-api, pyproject-hooks, pytest, sphinx, tox
+tox==4.14.2               # via -r dev-requirements.in
 trailrunner==1.4.0        # via fixit
-typing-extensions==4.10.0  # via black, libcst, mypy, typing-inspect
-typing-inspect==0.9.0     # via libcst
+typing-extensions==4.11.0  # via black, mypy
 unify==0.5                # via gray
 untokenize==0.1.1         # via unify
 urllib3==2.2.1            # via requests
-virtualenv==20.25.1       # via pre-commit, tox
-wheel==0.42.0             # via pip-tools
+virtualenv==20.26.0       # via pre-commit, tox
+wheel==0.43.0             # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `aprsd-3.3.4/docker/Dockerfile` & `aprsd-3.4.0/docker/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 FROM python:3.11-slim as build
 
-ARG VERSION=3.1.0
+ARG VERSION=3.4.0
 ENV TZ=${TZ:-US/Eastern}
 ENV LC_ALL=C.UTF-8
 ENV LANG=C.UTF-8
 ENV APRSD_PIP_VERSION=${VERSION}
 
 ENV PIP_DEFAULT_TIMEOUT=100 \
     # Allow statements and log messages to immediately appear
@@ -30,33 +30,34 @@
     && apt-get clean -y
 
 
 ### Final stage
 FROM build as final
 WORKDIR /app
 
+RUN pip3 install -U pip
 RUN pip3 install aprsd==$APRSD_PIP_VERSION
 RUN pip install gevent uwsgi
 RUN which aprsd
 RUN mkdir /config
 RUN chown -R appuser:appgroup /app
 RUN chown -R appuser:appgroup /config
 USER appuser
 RUN echo "PATH=\$PATH:/usr/games" >> /app/.bashrc
 RUN which aprsd
 RUN aprsd sample-config > /config/aprsd.conf
 
-ADD bin/run.sh /app
-ADD bin/listen.sh /app
+ADD bin/setup.sh /app
 ADD bin/admin.sh /app
 
 # For the web admin interface
 EXPOSE 8001
 
-ENTRYPOINT ["/app/run.sh"]
 VOLUME ["/config"]
+ENTRYPOINT ["/app/setup.sh"]
+CMD ["server"]
 
 # Set the user to run the application
 USER appuser
 
 HEALTHCHECK --interval=1m --timeout=12s --start-period=30s \
     CMD aprsd healthcheck --config /config/aprsd.conf --loglevel DEBUG
```

### Comparing `aprsd-3.3.4/docker/Dockerfile-dev` & `aprsd-3.4.0/docker/Dockerfile-dev`

 * *Files 10% similar despite different names*

```diff
@@ -29,30 +29,32 @@
 
 
 ### Final stage
 FROM build as final
 WORKDIR /app
 
 RUN git clone -b $APRSD_BRANCH https://github.com/craigerl/aprsd
+RUN pip install -U pip
 RUN cd aprsd && pip install --no-cache-dir .
-RUN pip install gevent uwsgi
+RUN pip install gevent uwsgi==2.0.24
 RUN which aprsd
 RUN mkdir /config
 RUN chown -R appuser:appgroup /app
 RUN chown -R appuser:appgroup /config
 USER appuser
 RUN echo "PATH=\$PATH:/usr/games" >> /app/.bashrc
 RUN which aprsd
 RUN aprsd sample-config > /config/aprsd.conf
 
-ADD bin/run.sh /app
-ADD bin/listen.sh /app
+ADD bin/setup.sh /app
 ADD bin/admin.sh /app
 
 EXPOSE 8000
+EXPOSE 8001
 
-# CMD ["gunicorn", "aprsd.wsgi:app", "--host", "0.0.0.0", "--port", "8000"]
-ENTRYPOINT ["/app/run.sh"]
 VOLUME ["/config"]
+# CMD ["gunicorn", "aprsd.wsgi:app", "--host", "0.0.0.0", "--port", "8000"]
+ENTRYPOINT ["/app/setup.sh"]
+CMD ["server"]
 
 # Set the user to run the application
 USER appuser
```

### Comparing `aprsd-3.3.4/docker/bin/admin.sh` & `aprsd-3.4.0/docker/bin/admin.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docker/bin/listen.sh` & `aprsd-3.4.0/docker/bin/listen.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docker/bin/run.sh` & `aprsd-3.4.0/docker/bin/run.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docker/build.sh` & `aprsd-3.4.0/docker/build.sh`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 ALL_PLATFORMS=0
 DEV=0
 REBUILD_BUILDX=0
 TAG="latest"
 BRANCH=${BRANCH:-master}
-VERSION="3.0.0"
+VERSION="3.3.4"
 
 while getopts “hdart:b:v:” OPTION
 do
     case $OPTION in
         t)
            TAG=$OPTARG
            ;;
```

### Comparing `aprsd-3.3.4/docs/_static/aprsd_overview.png` & `aprsd-3.4.0/docs/_static/aprsd_overview.png`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/_static/aprsd_overview.svg` & `aprsd-3.4.0/docs/_static/aprsd_overview.svg`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/apidoc/aprsd.cmds.rst` & `aprsd-3.4.0/docs/apidoc/aprsd.cmds.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/apidoc/aprsd.conf.rst` & `aprsd-3.4.0/docs/apidoc/aprsd.conf.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/apidoc/aprsd.packets.rst` & `aprsd-3.4.0/docs/apidoc/aprsd.packets.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/apidoc/aprsd.plugins.rst` & `aprsd-3.4.0/docs/apidoc/aprsd.plugins.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/apidoc/aprsd.rst` & `aprsd-3.4.0/docs/apidoc/aprsd.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/apidoc/aprsd.threads.rst` & `aprsd-3.4.0/docs/apidoc/aprsd.threads.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/apidoc/aprsd.utils.rst` & `aprsd-3.4.0/docs/apidoc/aprsd.utils.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/aprsd.drawio` & `aprsd-3.4.0/docs/aprsd.drawio`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/changelog.rst` & `aprsd-3.4.0/ChangeLog`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,408 @@
 CHANGES
 =======
 
+v3.4.0
+------
+
+* Change setup.h
+* Fixed docker setup.sh comparison
+* Fixed unit tests failing with WatchList
+* Added config enable\_packet\_logging
+* Make all the Objectstore children use the same lock
+* Fixed PacketTrack with UnknownPacket
+* Removed the requirement on click-completion
+* Update Dockerfiles
+* Added fox for entry\_points with old python
+* Added config for enable\_seen\_list
+* Fix APRSDStats start\_time
+* Added default\_packet\_send\_count config
+* Call packet collecter after prepare during tx
+* Added PacketTrack to packet collector
+* Webchat Send Beacon uses Path selected in UI
+* Added try except blocks in collectors
+* Remove error logs from watch list
+* Fixed issue with PacketList being empty
+* Added new PacketCollector
+* Fixed Keepalive access to email stats
+* Added support for RX replyacks
+* Changed Stats Collector registration
+* Added PacketList.set\_maxlen()
+* another fix for tx send
+* removed Packet.last\_send\_attempt and just use send\_count
+* Fix access to PacketList.\_maxlen
+* added packet\_count in packet\_list stats
+* force uwsgi to 2.0.24
+* ismall update
+* Added new config optons for PacketList
+* Update requirements
+* Added threads chart to admin ui graphs
+* set packetlist max back to 100
+* ensure thread count is updated
+* Added threads table in the admin web ui
+* Fixed issue with APRSDThreadList stats()
+* Added new default\_ack\_send\_count config option
+* Remove packet from tracker after max attempts
+* Limit packets to 50 in PacketList
+* syncronize the add for StatsStore
+* Lock on stats for PacketList
+* Fixed PacketList maxlen
+* Fixed a problem with the webchat tab notification
+* Another fix for ACK packets
+* Fix issue not tracking RX Ack packets for stats
+* Fix time plugin
+* add GATE route to webchat along with WIDE1, etc
+* Update webchat, include GATE route along with WIDE, ARISS, etc
+* Get rid of some useless warning logs
+* Added human\_info property to MessagePackets
+* Fixed scrolling problem with new webchat sent msg
+* Fix some issues with listen command
+* Admin interface catch empty stats
+* Ensure StatsStore has empty data
+* Ensure latest pip is in docker image
+* LOG failed requests post to admin ui
+* changed admin web\_ip to StrOpt
+* Updated prism to 1.29
+* Removed json-viewer
+* Remove rpyc as a requirement
+* Delete more stats from webchat
+* Admin UI working again
+* Removed RPC Server and client
+* Remove the logging of the conf password if not set
+* Lock around client reset
+* Allow stats collector to serialize upon creation
+* Fixed issues with watch list at startup
+* Fixed access to log\_monitor
+* Got unit tests working again
+* Fixed pep8 errors and missing files
+* Reworked the stats making the rpc server obsolete
+* Update client.py to add consumer in the API
+* Fix for sample-config warning
+* update requirements
+* Put packet.json back in
+* Change debug log color
+* Fix for filtering curse words
+* added packet counter random int
+* More packet cleanup and tests
+* Show comment in multiline packet output
+* Added new config option log\_packet\_format
+* Some packet cleanup
+* Added new webchat config option for logging
+* Fix some pep8 issues
+* Completely redo logging of packets!!
+* Fixed some logging in webchat
+* Added missing packet types in listen command
+* Don't call stats so often in webchat
+* Eliminated need for from\_aprslib\_dict
+* Fix for micE packet decoding with mbits
+* updated dev-requirements
+* Fixed some tox errors related to mypy
+* Refactored packets
+* removed print
+* small refactor of stats usage in version plugin
+* Added type setting on pluging.py for mypy
+* Moved Threads list for mypy
+* No need to synchronize on stats
+* Start to add types
+* Update tox for mypy runs
+* Bump black from 24.2.0 to 24.3.0
+* replaced access to conf from uwsgi
+* Fixed call to setup\_logging in uwsgi
+* Fixed access to conf.log in logging\_setup
+
+v3.3.2
+------
+
+* Changelog for 3.3.2
+* Remove warning during sample-config
+* Removed print in utils
+
+v3.3.1
+------
+
+* Updates for 3.3.1
+* Fixed failure with fetch-stats
+* Fixed problem with list-plugins
+
+v3.3.0
+------
+
+* Changelog for 3.3.0
+* sample-config fix
+* Fixed registry url post
+* Changed processpkt message
+* Fixed RegistryThread not sending requests
+* use log.setup\_logging
+* Disable debug logs for aprslib
+* Make registry thread sleep
+* Put threads first after date/time
+* Replace slow rich logging with loguru
+* Updated requirements
+* Fixed pep8
+* Added list-extensions and updated README.rst
+* Change defaults for beacon and registry
+* Add log info for Beacon and Registry threads
+* fixed frequency\_seconds to IntOpt
+* fixed references to conf
+* changed the default packet timeout to 5 minutes
+* Fixed default service registry url
+* fix pep8 failures
+* py311 fails in github
+* Don't send uptime to registry
+* Added sending software string to registry
+* add py310 gh actions
+* Added the new APRS Registry thread
+* Added installing extensions to Docker run
+* Cleanup some logs
+* Added BeaconPacket
+* updated requirements files
+* removed some unneeded code
+* Added iterator to objectstore
+* Added some missing classes to threads
+* Added support for loading extensions
+* Added location for callsign tabs in webchat
+* updated gitignore
+* Create codeql.yml
+* update github action branchs to v8
+* Added Location info on webchat interface
+* Updated dev test-plugin command
+* Update requirements.txt
+* Update for v3.2.3
+
+v3.2.3
+------
+
+* Force fortune path during setup test
+* added /usr/games to path
+* Added fortune to Dockerfile-dev
+* Added missing fortune app
+* aprsd: main.py: Fix premature return in sample\_config
+* Update weather.py  because you can't sort icons by penis
+* Update weather.py  both weather plugins have new Ww regex
+* Update weather.py
+* Fixed a bug with OWMWeatherPlugin
+* Rework Location Plugin
+
+v3.2.2
+------
+
+* Update for v3.2.2 release
+* Fix for types
+* Fix wsgi for prod
+* pep8 fixes
+* remove python 3.12 from github builds
+* Fixed datetime access in core.py
+* removed invalid reference to config.py
+* Updated requirements
+* Reworked the admin graphs
+* Test new packet serialization
+* Try to localize js libs and css for no internet
+* Normalize listen --aprs-login
+* Bump werkzeug from 2.3.7 to 3.0.1
+* Update INSTALL with new conf files
+* Bump urllib3 from 2.0.6 to 2.0.7
+
+v3.2.1
+------
+
+* Changelog for 3.2.1
+* Update index.html disable form autocomplete
+* Update the packet\_dupe\_timeout warning
+* Update the webchat paths
+* Changed the path option to a ListOpt
+* Fixed default path for tcp\_kiss client
+* Set a default password for admin
+* Fix path for KISS clients
+* Added packet\_dupe\_timeout conf
+* Add ability to change path on every TX packet
+* Make Packet objects hashable
+* Bump urllib3 from 2.0.4 to 2.0.6
+* Don't process AckPackets as dupes
+* Fixed another msgNo int issue
+* Fixed issue with packet tracker and msgNO Counter
+* Fixed import of Mutablemapping
+* pep8 fixes
+* rewrote packet\_list and drop dupe packets
+* Log a warning on dupe
+* Fix for dupe packets
+
+v3.2.0
+------
+
+* Update Changelog for 3.2.0
+* minor cleanup prior to release
+* Webchat: fix input maxlength
+* WebChat: cleanup some console.logs
+* WebChat: flash a dupe message
+* Webchat: Fix issue accessing msg.id
+* Webchat: Fix chat css on older browsers
+* WebChat: new tab should get focus
+* Bump gevent from 23.9.0.post1 to 23.9.1
+* Webchat: Fix pep8 errors
+* Webchat: Added tab notifications and raw packet
+* WebChat: Prevent sending message without callsign
+* WebChat: fixed content area scrolling
+* Webchat: tweaks to UI for expanding chat
+* Webchat: Fixed bug deleteing first tab
+* Ensure Keepalive doesn't reset client at startup
+* Ensure parse\_delta\_str doesn't puke
+* WebChat: Send GPS Beacon working
+* webchat: got active tab onclick working
+* webchat: set to\_call to value of tab when selected
+* Center the webchat input form
+* Update index.html to use chat.css
+* Deleted webchat mobile pages
+* Added close X on webchat tabs
+* Reworked webchat with new UI
+* Updated the webchat UI to look like iMessage
+* Restore previous conversations in webchat
+* Remove VIM from Dockerfile
+* recreate client during reset()
+* updated github workflows
+* Updated documentation build
+* Removed admin\_web.py
+* Removed some RPC server log noise
+* Fixed admin page packet date
+* RPC Server logs the client IP on failed auth
+* Start keepalive thread first
+* fixed an issue in the mobile webchat
+* Added dupe checkig code to webchat mobile
+* click on the div after added
+* Webchat suppress to display of dupe messages
+* Convert webchat internet urls to local static urls
+* Make use of webchat gps config options
+* Added new webchat config section
+* fixed webchat logging.logformat typeoh
+
+v3.1.3
+------
+
+* prep for 3.1.3
+* Forcefully allow development webchat flask
+
+v3.1.2
+------
+
+* Updated Changelog for 3.1.2
+* Added support for ThirdParty packet types
+* Disable the Send GPS Beacon button
+* Removed adhoc ssl support in webchat
+
+v3.1.1
+------
+
+* Updated Changelog for v3.1.1
+* Fixed pep8 failures
+* re-enable USWeatherPlugin to use mapClick
+* Fix sending packets over KISS interface
+* Use config web\_ip for running admin ui from module
+* remove loop log
+* Max out the client reconnect backoff to 5
+* Update the Dockerfile
+
+v3.1.0
+------
+
+* Changelog updates for v3.1.0
+* Use CONF.admin.web\_port for single launch web admin
+* Fixed sio namespace registration
+* Update Dockerfile-dev to include uwsgi
+* Fixed pep8
+* change port to 8000
+* replacement of flask-socketio with python-socketio
+* Change how fetch-stats gets it's defaults
+* Ensure fetch-stats ip is a string
+* Add info logging for rpc server calls
+* updated wsgi config default /config/aprsd.conf
+* Added timing after each thread loop
+* Update docker bin/admin.sh
+* Removed flask-classful from webchat
+* Remove flask pinning
+* removed linux/arm/v8
+* Update master build to include linux/arm/v8
+* Update Dockerfile-dev to fix plugin permissions
+* update manual build github
+* Update requirements for upgraded cryptography
+* Added more libs for Dockerfile-dev
+* Replace Dockerfile-dev with python3 slim
+* Moved logging to log for wsgi.py
+* Changed weather plugin regex pattern
+* Limit the float values to 3 decimal places
+* Fixed rain numbers from aprslib
+* Fixed rpc client initialization
+* Fix in for aprslib issue #80
+* Try and fix Dockerfile-dev
+* Fixed pep8 errors
+* Populate stats object with threads info
+* added counts to the fetch-stats table
+* Added the fetch-stats command
+* Replace ratelimiter with rush
+* Added some utilities to Dockerfile-dev
+* add arm64 for manual github build
+* Added manual master build
+* Update master-build.yml
+* Add github manual trigger for master build
+* Fixed unit tests for Location plugin
+* USe new tox and update githubworkflows
+* Updated requirements
+* force tox to 4.3.5
+* Update github workflows
+* Fixed pep8 violation
+* Added rpc server for listen
+* Update location plugin and reworked requirements
+* Fixed .readthedocs.yaml format
+* Add .readthedocs.yaml
+* Example plugin wrong function
+* Ensure conf is imported for threads/tx
+* Update Dockerfile to help build cryptography
+
+v3.0.3
+------
+
+* Update Changelog to 3.0.3
+* cleanup some debug messages
+* Fixed loading of plugins for server
+* Don't load help plugin for listen command
+* Added listen args
+* Change listen command plugins
+* Added listen.sh for docker
+* Update Listen command
+* Update Dockerfile
+* Add ratelimiting for acks and other packets
+
+v3.0.2
+------
+
+* Update Changelog for 3.0.2
+* Import RejectPacket
+
+v3.0.1
+------
+
+* 3.0.1
+* Add support to Reject messages
+* Update Docker builds for 3.0.0
+
+v3.0.0
+------
+
+* Update Changelog for 3.0.0
+* Ensure server command main thread doesn't exit
+* Fixed save directory default
+* Fixed pep8 failure
+* Cleaned up KISS interfaces use of old config
+* reworked usage of importlib.metadata
+* Added new docs files for 3.0.0
+* Removed url option from healthcheck in dev
+* Updated Healthcheck to use rpc to call aprsd
+* Updated docker/bin/run.sh to use new conf
+* Added ObjectPacket
+* Update regex processing and regex for plugins
+* Change ordering of starting up of server command
+* Update documentation and README
 * Decouple admin web interface from server command
 * Dockerfile now produces aprsd.conf
 * Fix some unit tests and loading of CONF w/o file
 * Added missing conf
 * Removed references to old custom config
 * Convert config to oslo\_config
 * Added rain formatting unit tests to WeatherPacket
```

### Comparing `aprsd-3.3.4/docs/clean_docs.py` & `aprsd-3.4.0/docs/clean_docs.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/conf.py` & `aprsd-3.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/configure.rst` & `aprsd-3.4.0/docs/configure.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/index.rst` & `aprsd-3.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/install.rst` & `aprsd-3.4.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/links.rst` & `aprsd-3.4.0/docs/links.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/plugin.rst` & `aprsd-3.4.0/docs/plugin.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/readme.rst` & `aprsd-3.4.0/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/docs/server.rst` & `aprsd-3.4.0/docs/server.rst`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/pyproject.toml` & `aprsd-3.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/requirements.txt` & `aprsd-3.4.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,72 +13,70 @@
 blinker==1.7.0            # via flask
 certifi==2024.2.2         # via requests
 charset-normalizer==3.3.2  # via requests
 click==8.1.7              # via -r requirements.in, click-completion, click-params, flask
 click-completion==0.5.2   # via -r requirements.in
 click-params==0.5.0       # via -r requirements.in
 commonmark==0.9.1         # via rich
-dacite2==2.0.0            # via -r requirements.in
 dataclasses==0.6          # via -r requirements.in
 dataclasses-json==0.6.4   # via -r requirements.in
 debtcollector==3.0.0      # via oslo-config
 deprecated==1.2.14        # via click-params
 dnspython==2.6.1          # via eventlet
-eventlet==0.35.2          # via -r requirements.in
-flask==3.0.2              # via -r requirements.in, flask-httpauth, flask-socketio
+eventlet==0.36.1          # via -r requirements.in
+flask==3.0.3              # via -r requirements.in, flask-httpauth, flask-socketio
 flask-httpauth==4.8.0     # via -r requirements.in
 flask-socketio==5.3.6     # via -r requirements.in
 geographiclib==2.0        # via geopy
 geopy==2.4.1              # via -r requirements.in
 gevent==24.2.1            # via -r requirements.in
 greenlet==3.0.3           # via eventlet, gevent
 h11==0.14.0               # via wsproto
-idna==3.6                 # via requests
+idna==3.7                 # via requests
 imapclient==3.0.1         # via -r requirements.in
-importlib-metadata==7.0.1  # via ax253, kiss3
-itsdangerous==2.1.2       # via flask
+importlib-metadata==7.1.0  # via ax253, kiss3
+itsdangerous==2.2.0       # via flask
 jinja2==3.1.3             # via click-completion, flask
 kiss3==8.0.0              # via -r requirements.in
 loguru==0.7.2             # via -r requirements.in
 markupsafe==2.1.5         # via jinja2, werkzeug
 marshmallow==3.21.1       # via dataclasses-json
 mypy-extensions==1.0.0    # via typing-inspect
 netaddr==1.2.1            # via oslo-config
 oslo-config==9.4.0        # via -r requirements.in
 oslo-i18n==6.3.0          # via oslo-config
-packaging==23.2           # via marshmallow
+packaging==24.0           # via marshmallow
 pbr==6.0.0                # via -r requirements.in, oslo-i18n, stevedore
-pluggy==1.4.0             # via -r requirements.in
-plumbum==1.8.2            # via rpyc
+pluggy==1.5.0             # via -r requirements.in
 pygments==2.17.2          # via rich
 pyserial==3.5             # via pyserial-asyncio
 pyserial-asyncio==0.6     # via kiss3
 python-engineio==4.9.0    # via python-socketio
-python-socketio==5.11.1   # via -r requirements.in, flask-socketio
+python-socketio==5.11.2   # via -r requirements.in, flask-socketio
 pytz==2024.1              # via -r requirements.in
 pyyaml==6.0.1             # via -r requirements.in, oslo-config
 requests==2.31.0          # via -r requirements.in, oslo-config, update-checker
 rfc3986==2.0.0            # via oslo-config
 rich==12.6.0              # via -r requirements.in
-rpyc==6.0.0               # via -r requirements.in
 rush==2021.4.0            # via -r requirements.in
 shellingham==1.5.4        # via -r requirements.in, click-completion
 simple-websocket==1.0.0   # via python-engineio
 six==1.16.0               # via -r requirements.in, click-completion
 soupsieve==2.5            # via beautifulsoup4
 stevedore==5.2.0          # via oslo-config
 tabulate==0.9.0           # via -r requirements.in
 thesmuggler==1.0.1        # via -r requirements.in
-typing-extensions==4.10.0  # via typing-inspect
+typing-extensions==4.11.0  # via typing-inspect
 typing-inspect==0.9.0     # via dataclasses-json
+tzlocal==5.2              # via -r requirements.in
 update-checker==0.18.0    # via -r requirements.in
 urllib3==2.2.1            # via requests
 validators==0.22.0        # via click-params
-werkzeug==3.0.1           # via -r requirements.in, flask
+werkzeug==3.0.2           # via -r requirements.in, flask
 wrapt==1.16.0             # via -r requirements.in, debtcollector, deprecated
 wsproto==1.2.0            # via simple-websocket
-zipp==3.17.0              # via importlib-metadata
+zipp==3.18.1              # via importlib-metadata
 zope-event==5.0           # via gevent
-zope-interface==6.2       # via gevent
+zope-interface==6.3       # via gevent
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `aprsd-3.3.4/setup.cfg` & `aprsd-3.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/setup.py` & `aprsd-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/tests/cmds/test_send_message.py` & `aprsd-3.4.0/tests/cmds/test_send_message.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/tests/cmds/test_webchat.py` & `aprsd-3.4.0/tests/cmds/test_webchat.py`

 * *Files 15% similar despite different names*

```diff
@@ -47,19 +47,16 @@
     @mock.patch("aprsd.cmds.webchat.socketio")
     def test_process_ack_packet(
         self,
         mock_remove, mock_socketio,
     ):
         self.config_and_init()
         mock_socketio.emit = mock.MagicMock()
-        packet = fake.fake_packet(
-            message="blah",
-            msg_number=1,
-            message_format=core.PACKET_TYPE_ACK,
-        )
+        # Create an ACK packet
+        packet = fake.fake_ack_packet()
         mock_queue = mock.MagicMock()
         socketio = mock.MagicMock()
         wcp = webchat.WebChatProcessPacketThread(mock_queue, socketio)
 
         wcp.process_ack_packet(packet)
         mock_remove.called_once()
         mock_socketio.called_once()
```

### Comparing `aprsd-3.3.4/tests/fake.py` & `aprsd-3.4.0/tests/fake.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,48 @@
-from aprsd import packets, plugin, threads
+from aprsd import plugin, threads
 from aprsd.packets import core
 
 
 FAKE_MESSAGE_TEXT = "fake MeSSage"
 FAKE_FROM_CALLSIGN = "KFAKE"
 FAKE_TO_CALLSIGN = "KMINE"
 
 
 def fake_packet(
     fromcall=FAKE_FROM_CALLSIGN,
     tocall=FAKE_TO_CALLSIGN,
     message=None,
     msg_number=None,
     message_format=core.PACKET_TYPE_MESSAGE,
+    response=None,
 ):
     packet_dict = {
         "from": fromcall,
         "addresse": tocall,
         "to": tocall,
         "format": message_format,
         "raw": "",
     }
     if message:
         packet_dict["message_text"] = message
 
     if msg_number:
         packet_dict["msgNo"] = str(msg_number)
 
-    return packets.Packet.factory(packet_dict)
+    if response:
+        packet_dict["response"] = response
+
+    return core.factory(packet_dict)
+
+
+def fake_ack_packet():
+    return fake_packet(
+        msg_number=12,
+        response=core.PACKET_TYPE_ACK,
+    )
 
 
 class FakeBaseNoThreadsPlugin(plugin.APRSDPluginBase):
     version = "1.0"
 
     def setup(self):
         self.enabled = True
```

### Comparing `aprsd-3.3.4/tests/plugins/test_fortune.py` & `aprsd-3.4.0/tests/plugins/test_fortune.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/tests/plugins/test_location.py` & `aprsd-3.4.0/tests/plugins/test_location.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/tests/plugins/test_notify.py` & `aprsd-3.4.0/tests/plugins/test_notify.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/tests/plugins/test_ping.py` & `aprsd-3.4.0/tests/plugins/test_ping.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/tests/plugins/test_time.py` & `aprsd-3.4.0/tests/plugins/test_time.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/tests/plugins/test_weather.py` & `aprsd-3.4.0/tests/plugins/test_weather.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from .. import fake, test_plugin
 
 
 CONF = cfg.CONF
 
 
-class TestUSWeatherPluginPlugin(test_plugin.TestPlugin):
+class TestUSWeatherPlugin(test_plugin.TestPlugin):
 
     def test_not_enabled_missing_aprs_fi_key(self):
         # When the aprs.fi api key isn't set, then
         # the LocationPlugin will be disabled.
         CONF.aprs_fi.apiKey = None
         CONF.callsign = fake.FAKE_TO_CALLSIGN
         wx = weather_plugin.USWeatherPlugin()
```

### Comparing `aprsd-3.3.4/tests/test_email.py` & `aprsd-3.4.0/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/tests/test_main.py` & `aprsd-3.4.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/tests/test_plugin.py` & `aprsd-3.4.0/tests/test_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from unittest import mock
 
 from oslo_config import cfg
 
 from aprsd import conf  # noqa: F401
 from aprsd import packets
 from aprsd import plugin as aprsd_plugin
-from aprsd import plugins, stats
+from aprsd import plugins
 from aprsd.packets import core
 
 from . import fake
 
 
 CONF = cfg.CONF
 
@@ -41,15 +41,14 @@
     def test_get_plugins_with_plugins(self):
         CONF.enabled_plugins = ["aprsd.plugins.ping.PingPlugin"]
         pm = aprsd_plugin.PluginManager()
         plugin_list = pm.get_plugins()
         self.assertEqual([], plugin_list)
         pm.setup_plugins()
         plugin_list = pm.get_plugins()
-        print(plugin_list)
         self.assertIsInstance(plugin_list, list)
         self.assertIsInstance(
             plugin_list[0],
             (
                 aprsd_plugin.HelpPlugin,
                 plugins.ping.PingPlugin,
             ),
@@ -86,15 +85,14 @@
 
     def setUp(self) -> None:
         self.fromcall = fake.FAKE_FROM_CALLSIGN
         self.ack = 1
         self.config_and_init()
 
     def tearDown(self) -> None:
-        stats.APRSDStats._instance = None
         packets.WatchList._instance = None
         packets.SeenList._instance = None
         packets.PacketTrack._instance = None
         self.config = None
 
     def config_and_init(self):
         CONF.callsign = self.fromcall
@@ -159,17 +157,15 @@
             message_format=core.PACKET_TYPE_MICE,
         )
         expected = packets.NULL_MESSAGE
         actual = p.filter(packet)
         self.assertEqual(expected, actual)
         mock_process.assert_not_called()
 
-        packet = fake.fake_packet(
-            message_format=core.PACKET_TYPE_ACK,
-        )
+        packet = fake.fake_ack_packet()
         expected = packets.NULL_MESSAGE
         actual = p.filter(packet)
         self.assertEqual(expected, actual)
         mock_process.assert_not_called()
 
     @mock.patch.object(fake.FakeRegexCommandPlugin, "process")
     def test_regex_base_assert_called(self, mock_process):
```

### Comparing `aprsd-3.3.4/tools/fast8.sh` & `aprsd-3.4.0/tools/fast8.sh`

 * *Files identical despite different names*

### Comparing `aprsd-3.3.4/tox.ini` & `aprsd-3.4.0/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -90,14 +90,14 @@
     gray aprsd tests
 
 [testenv:type-check]
 skip_install = true
 deps = -r{toxinidir}/requirements.txt
     -r{toxinidir}/dev-requirements.txt
 commands =
-    mypy aprsd
+    mypy --ignore-missing-imports --install-types aprsd
 
 [testenv:pre-commit]
 skip_install = true
 basepython = python3
 deps = pre-commit
 commands = pre-commit run --all-files --show-diff-on-failure
```

