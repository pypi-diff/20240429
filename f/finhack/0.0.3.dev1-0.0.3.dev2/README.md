# Comparing `tmp/finhack-0.0.3.dev1.tar.gz` & `tmp/finhack-0.0.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finhack-0.0.3.dev1.tar", last modified: Tue Apr  9 06:04:22 2024, max compression
+gzip compressed data, was "finhack-0.0.3.dev2.tar", last modified: Mon Apr 29 01:42:27 2024, max compression
```

## Comparing `finhack-0.0.3.dev1.tar` & `finhack-0.0.3.dev2.tar`

### file list

```diff
@@ -1,359 +1,359 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/
--rw-r--r--   0 root         (0) root         (0)    73748 2023-12-27 02:20:47.000000 finhack-0.0.3.dev1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      138 2024-01-18 10:18:24.000000 finhack-0.0.3.dev1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      159 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3648 2024-04-07 06:51:23.000000 finhack-0.0.3.dev1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/examples/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-13 11:17:21.000000 finhack-0.0.3.dev1/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/finhack/
--rw-r--r--   0 root         (0) root         (0)       27 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/finhack/collector/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/collector/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 17:17:00.000000 finhack-0.0.3.dev1/finhack/collector/baseCollector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/finhack/collector/tushare/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/collector/tushare/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/finhack/collector/tushare/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/collector/tushare/__pycache__/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5475 2023-07-18 11:03:58.000000 finhack-0.0.3.dev1/finhack/collector/tushare/astockbasic.py
--rwxr-xr-x   0 root         (0) root         (0)    19378 2023-07-18 11:06:31.000000 finhack-0.0.3.dev1/finhack/collector/tushare/astockfinance.py
--rwxr-xr-x   0 root         (0) root         (0)    16164 2023-07-18 11:08:47.000000 finhack-0.0.3.dev1/finhack/collector/tushare/astockindex.py
--rwxr-xr-x   0 root         (0) root         (0)     2437 2023-07-18 10:59:04.000000 finhack-0.0.3.dev1/finhack/collector/tushare/astockmarket.py
--rwxr-xr-x   0 root         (0) root         (0)     7588 2023-07-18 11:15:02.000000 finhack-0.0.3.dev1/finhack/collector/tushare/astockother.py
--rwxr-xr-x   0 root         (0) root         (0)     4228 2023-07-18 11:10:21.000000 finhack-0.0.3.dev1/finhack/collector/tushare/astockprice.py
--rwxr-xr-x   0 root         (0) root         (0)     4534 2023-07-18 11:14:49.000000 finhack-0.0.3.dev1/finhack/collector/tushare/cb.py
--rwxr-xr-x   0 root         (0) root         (0)     2373 2023-07-18 10:59:25.000000 finhack-0.0.3.dev1/finhack/collector/tushare/econo.py
--rwxr-xr-x   0 root         (0) root         (0)     6335 2023-07-18 11:13:49.000000 finhack-0.0.3.dev1/finhack/collector/tushare/fund.py
--rwxr-xr-x   0 root         (0) root         (0)     1987 2023-07-18 10:59:31.000000 finhack-0.0.3.dev1/finhack/collector/tushare/futures.py
--rwxr-xr-x   0 root         (0) root         (0)      520 2023-07-18 11:12:40.000000 finhack-0.0.3.dev1/finhack/collector/tushare/fx.py
--rwxr-xr-x   0 root         (0) root         (0)    10537 2023-07-18 11:12:33.000000 finhack-0.0.3.dev1/finhack/collector/tushare/helper.py
--rwxr-xr-x   0 root         (0) root         (0)      677 2023-07-18 10:59:39.000000 finhack-0.0.3.dev1/finhack/collector/tushare/hstock.py
--rwxr-xr-x   0 root         (0) root         (0)     1271 2023-07-18 10:59:42.000000 finhack-0.0.3.dev1/finhack/collector/tushare/other.py
--rwxr-xr-x   0 root         (0) root         (0)     7980 2024-01-03 17:45:57.000000 finhack-0.0.3.dev1/finhack/collector/tushare/tushare_collector.py
--rwxr-xr-x   0 root         (0) root         (0)      669 2023-07-18 10:59:45.000000 finhack-0.0.3.dev1/finhack/collector/tushare/ustock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/finhack/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:06:37.000000 finhack-0.0.3.dev1/finhack/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/finhack/core/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/core/__pycache__/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/core/classes/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:05:35.000000 finhack-0.0.3.dev1/finhack/core/classes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/core/classes/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/core/classes/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2952 2024-04-07 06:44:16.000000 finhack-0.0.3.dev1/finhack/core/classes/dictobj.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/core/command/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/core/command/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1236 2024-01-30 03:58:55.000000 finhack-0.0.3.dev1/finhack/core/command/finhack
--rw-r--r--   0 root         (0) root         (0)     9001 2024-04-01 11:27:46.000000 finhack-0.0.3.dev1/finhack/core/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/core/data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/core/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/core/data/logs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/core/data/logs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/core/loader/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:10:41.000000 finhack-0.0.3.dev1/finhack/core/loader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/core/loader/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/core/loader/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3966 2024-01-31 04:25:19.000000 finhack-0.0.3.dev1/finhack/core/loader/base_loader.py
--rw-r--r--   0 root         (0) root         (0)      294 2024-01-04 11:30:36.000000 finhack-0.0.3.dev1/finhack/core/loader/collector_loader.py
--rw-r--r--   0 root         (0) root         (0)      277 2024-01-04 11:30:49.000000 finhack-0.0.3.dev1/finhack/core/loader/factor_loader.py
--rw-r--r--   0 root         (0) root         (0)      285 2024-01-04 11:32:05.000000 finhack-0.0.3.dev1/finhack/core/loader/helper_loader.py
--rw-r--r--   0 root         (0) root         (0)      315 2024-01-04 11:32:07.000000 finhack-0.0.3.dev1/finhack/core/loader/trader_loader.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 07:25:21.000000 finhack-0.0.3.dev1/finhack/core/notify.py
--rw-r--r--   0 root         (0) root         (0)      121 2024-01-23 07:25:27.000000 finhack-0.0.3.dev1/finhack/core/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/factor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/factor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/factor/default/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-04 10:31:48.000000 finhack-0.0.3.dev1/finhack/factor/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/factor/default/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/factor/default/__pycache__/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    24778 2024-03-19 03:48:09.000000 finhack-0.0.3.dev1/finhack/factor/default/alphaEngine.py
--rw-r--r--   0 root         (0) root         (0)     4955 2024-04-03 01:54:17.000000 finhack-0.0.3.dev1/finhack/factor/default/default_factor.py
--rwxrwxrwx   0 root         (0) root         (0)    18152 2024-03-04 11:36:16.000000 finhack-0.0.3.dev1/finhack/factor/default/factorAnalyzer.py
--rwxrwxrwx   0 root         (0) root         (0)     7888 2024-03-04 10:37:04.000000 finhack-0.0.3.dev1/finhack/factor/default/factorManager.py
--rwxrwxrwx   0 root         (0) root         (0)    13617 2024-04-03 01:56:59.000000 finhack-0.0.3.dev1/finhack/factor/default/factorMining.py
--rwxrwxrwx   0 root         (0) root         (0)     3034 2024-03-04 10:32:09.000000 finhack-0.0.3.dev1/finhack/factor/default/factorPkl.py
--rw-r--r--   0 root         (0) root         (0)     3529 2023-07-18 16:57:34.000000 finhack-0.0.3.dev1/finhack/factor/default/factorRepair.py
--rwxrwxrwx   0 root         (0) root         (0)    20166 2024-03-18 10:50:36.000000 finhack-0.0.3.dev1/finhack/factor/default/indicatorCompute.py
--rwxrwxrwx   0 root         (0) root         (0)    18873 2024-03-19 04:08:04.000000 finhack-0.0.3.dev1/finhack/factor/default/preCheck.py
--rwxrwxrwx   0 root         (0) root         (0)     2675 2024-03-19 01:59:28.000000 finhack-0.0.3.dev1/finhack/factor/default/taskRunner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/helper/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/helper/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/helper/struct/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/helper/struct/__init__.py
--rw-r--r--   0 root         (0) root         (0)      192 2023-10-30 10:01:09.000000 finhack-0.0.3.dev1/finhack/helper/struct/struct_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/library/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/library/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/library/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/library/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1606 2024-04-03 02:00:10.000000 finhack-0.0.3.dev1/finhack/library/ai.py
--rwxrwxrwx   0 root         (0) root         (0)     1437 2024-02-28 08:52:26.000000 finhack-0.0.3.dev1/finhack/library/alert.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-12-28 02:00:35.000000 finhack-0.0.3.dev1/finhack/library/class_loader.py
--rw-r--r--   0 root         (0) root         (0)      771 2024-03-18 12:40:27.000000 finhack-0.0.3.dev1/finhack/library/config.py
--rw-r--r--   0 root         (0) root         (0)     1159 2024-03-27 04:56:20.000000 finhack-0.0.3.dev1/finhack/library/log.py
--rwxrwxrwx   0 root         (0) root         (0)     3254 2023-07-18 11:03:32.000000 finhack-0.0.3.dev1/finhack/library/monitor.py
--rw-r--r--   0 root         (0) root         (0)     2254 2024-02-28 10:19:22.000000 finhack-0.0.3.dev1/finhack/library/mycache.py
--rwxrwxrwx   0 root         (0) root         (0)     3088 2023-07-18 03:02:15.000000 finhack-0.0.3.dev1/finhack/library/mydb.py
--rwxrwxrwx   0 root         (0) root         (0)      830 2023-09-18 06:59:38.000000 finhack-0.0.3.dev1/finhack/library/thread.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-12-26 11:12:16.000000 finhack-0.0.3.dev1/finhack/library/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/market/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:22:54.000000 finhack-0.0.3.dev1/finhack/market/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.586925 finhack-0.0.3.dev1/finhack/market/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/market/__pycache__/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/market/astock/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-20 07:33:55.000000 finhack-0.0.3.dev1/finhack/market/astock/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/market/astock/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/market/astock/__pycache__/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1690 2024-01-04 15:33:35.000000 finhack-0.0.3.dev1/finhack/market/astock/astock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/market/astock/tushare/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-04 06:44:17.000000 finhack-0.0.3.dev1/finhack/market/astock/tushare/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    17309 2024-04-08 09:49:34.000000 finhack-0.0.3.dev1/finhack/market/astock/tushare/astock.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-04-01 02:44:49.000000 finhack-0.0.3.dev1/finhack/market/astock/tushare/indexHelper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/plugin/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/plugin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/plugin/default/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/plugin/default/__init__.py
--rw-r--r--   0 root         (0) root         (0)      126 2023-11-02 17:26:48.000000 finhack-0.0.3.dev1/finhack/plugin/default/default_plugin.py
--rw-r--r--   0 root         (0) root         (0)      508 2024-04-09 06:04:21.000000 finhack-0.0.3.dev1/finhack/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/server/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 09:57:12.000000 finhack-0.0.3.dev1/finhack/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/server/default/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 09:57:12.000000 finhack-0.0.3.dev1/finhack/server/default/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5545 2024-04-07 17:24:34.000000 finhack-0.0.3.dev1/finhack/server/default/default_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trader/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trader/default/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trader/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trader/default/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trader/default/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)      759 2023-12-08 09:41:42.000000 finhack-0.0.3.dev1/finhack/trader/default/calendar.py
--rw-r--r--   0 root         (0) root         (0)     4356 2024-04-03 00:02:23.000000 finhack-0.0.3.dev1/finhack/trader/default/context.py
--rw-r--r--   0 root         (0) root         (0)    17061 2024-03-05 05:58:00.000000 finhack-0.0.3.dev1/finhack/trader/default/data.py
--rw-r--r--   0 root         (0) root         (0)    11700 2024-04-07 08:17:55.000000 finhack-0.0.3.dev1/finhack/trader/default/default_trader.py
--rw-r--r--   0 root         (0) root         (0)     9720 2023-12-23 18:52:29.000000 finhack-0.0.3.dev1/finhack/trader/default/event.py
--rw-r--r--   0 root         (0) root         (0)    19045 2024-04-07 06:35:50.000000 finhack-0.0.3.dev1/finhack/trader/default/function.py
--rw-r--r--   0 root         (0) root         (0)     4930 2024-03-05 06:26:36.000000 finhack-0.0.3.dev1/finhack/trader/default/object.py
--rw-r--r--   0 root         (0) root         (0)     9397 2024-04-04 16:15:25.000000 finhack-0.0.3.dev1/finhack/trader/default/performance.py
--rw-r--r--   0 root         (0) root         (0)     8597 2024-03-26 02:45:51.000000 finhack-0.0.3.dev1/finhack/trader/default/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trainer/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trainer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trainer/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trainer/__pycache__/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trainer/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trainer/auto/__init__.py
--rw-r--r--   0 root         (0) root         (0)       32 2024-01-23 10:56:05.000000 finhack-0.0.3.dev1/finhack/trainer/auto/auto_trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trainer/lightgbm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trainer/lightgbm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/trainer/lightgbm/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/trainer/lightgbm/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13418 2024-03-22 09:36:36.000000 finhack-0.0.3.dev1/finhack/trainer/lightgbm/lightgbm_trainer.py
--rw-r--r--   0 root         (0) root         (0)     4386 2024-03-26 06:58:49.000000 finhack-0.0.3.dev1/finhack/trainer/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/widgets/templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 03:52:10.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/.proj
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/auto/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-03 03:37:25.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/auto/default/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 03:44:51.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/auto/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-26 08:46:08.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/default/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-26 08:46:08.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/default/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 02:17:07.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/default/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8421 2024-04-07 14:16:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/default/default_backtest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/choice/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/choice/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/factors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.590924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/index/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/index/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/kv/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/kv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/market/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/market/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/notice/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 07:28:17.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/notice/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/price/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/price/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 09:02:59.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)      914 2024-04-09 01:00:01.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime/constant.py
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-09 01:00:01.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime/global_var.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 08:25:47.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      183 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/ai.conf
--rwxrwxrwx   0 root         (0) root         (0)      398 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/alert.conf
--rw-r--r--   0 root         (0) root         (0)     4433 2024-04-04 09:56:10.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/args.conf
--rw-rw-r--   0 root         (0) root         (0)      283 2024-04-04 09:53:25.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/backtest.conf
--rw-r--r--   0 root         (0) root         (0)      847 2024-03-15 02:02:17.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/constant.conf
--rw-r--r--   0 root         (0) root         (0)       18 2023-12-28 01:09:57.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/core.conf
--rwxrwxrwx   0 root         (0) root         (0)      336 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/db.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    13827 2024-03-04 08:10:44.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha101
--rwxrwxrwx   0 root         (0) root         (0)    22039 2022-12-04 10:31:48.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha191
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3010 2024-04-08 10:00:03.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/all
--rw-r--r--   0 root         (0) root         (0)     3443 2023-05-03 18:51:57.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/woldy
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-04-17 10:39:56.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/autotrain
--rw-r--r--   0 root         (0) root         (0)       67 2024-02-28 07:23:35.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/global_var.conf
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-05-09 07:57:06.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/task.conf
--rw-rw-r--   0 root         (0) root         (0)      106 2024-04-03 03:14:00.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/trader.conf
--rw-r--r--   0 root         (0) root         (0)       21 2023-12-24 17:51:59.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/train.conf
--rwxrwxrwx   0 root         (0) root         (0)      148 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/ts.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.594924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/code_factors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/code_factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/date_factors/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/date_factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 04:41:32.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/all_factors.parquet/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 06:44:04.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/all_factors.parquet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 10:44:16.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/_tmp/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:11:07.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/_tmp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:28:19.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/_tmp/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:28:19.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/_tmp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/logs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/logs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/logs/trader/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/logs/trader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/preds/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/preds/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 08:48:12.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2253 2024-04-07 08:36:40.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/css/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/css/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/images/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/images/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/js/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/js/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/rqalpha/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 05:53:37.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/rqalpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/trader/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/static/trader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/running/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 04:10:28.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/running/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/
--rw-r--r--   0 root         (0) root         (0)     1195 2022-12-07 19:27:24.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/QIML365.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-04 10:31:48.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/__pycache__/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8109 2024-01-07 01:31:52.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/extend.py
--rwxrwxrwx   0 root         (0) root         (0)     5827 2024-01-07 01:43:56.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/financial.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-03-20 07:07:21.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/member.py
--rwxrwxrwx   0 root         (0) root         (0)     1948 2024-01-07 01:32:06.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/myfactors.py
--rwxrwxrwx   0 root         (0) root         (0)    21290 2024-01-07 01:32:35.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/ta_lib.py
--rwxrwxrwx   0 root         (0) root         (0)     1954 2024-01-07 01:33:13.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/volumeprice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/
--rw-r--r--   0 root         (0) root         (0)      523 2023-12-28 01:38:27.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/1testmodule_loader.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 01:51:08.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)      521 2024-01-04 11:32:51.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/testmodule_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/prompt/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 09:34:57.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/prompt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/prompts/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 09:03:25.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/prompts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/script/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 11:25:50.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/script/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/
--rw-r--r--   0 root         (0) root         (0)     3047 2024-04-01 11:33:59.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/AITopNStrategy.py
--rw-r--r--   0 root         (0) root         (0)     3348 2024-01-30 07:19:08.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy.py
--rw-r--r--   0 root         (0) root         (0)     2280 2024-04-07 04:58:56.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/DemoStrategy.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/__pycache__/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/default/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/default/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 01:51:08.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/default/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10912 2024-03-25 02:37:56.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/default/default_testmodule.py
--rw-r--r--   0 root         (0) root         (0)      400 2023-07-24 08:45:41.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/default/testmodule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 10:57:17.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.598924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-13 11:19:29.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/__pycache__/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 10:57:28.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-07 11:04:36.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)      759 2024-03-07 11:04:36.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/calendar.py
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-12 08:46:32.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/client.py
--rw-r--r--   0 root         (0) root         (0)     3704 2024-04-02 23:44:21.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/context.py
--rw-r--r--   0 root         (0) root         (0)      587 2024-04-02 08:04:02.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/data.py
--rw-r--r--   0 root         (0) root         (0)     2958 2024-04-07 06:43:50.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/dictobj.py
--rw-r--r--   0 root         (0) root         (0)     6080 2024-04-08 02:08:50.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/event.py
--rw-r--r--   0 root         (0) root         (0)    11500 2024-04-08 07:23:29.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/function.py
--rw-r--r--   0 root         (0) root         (0)     4940 2024-03-28 17:49:09.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/object.py
--rw-rw-r--   0 root         (0) root         (0)     7813 2024-04-07 15:23:44.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmtClient.py
--rwxrwxrwx   0 root         (0) root         (0)     5367 2024-03-27 12:07:44.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2.py
--rwxrwxrwx   0 root         (0) root         (0)    14005 2024-03-27 12:12:48.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2_grpc.py
--rwxrwxrwx   0 root         (0) root         (0)     5060 2024-04-08 01:58:40.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmt_trader.py
--rw-r--r--   0 root         (0) root         (0)     8691 2024-04-08 07:15:00.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/rqalpha/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 05:53:37.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/rqalpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/rqalpha/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 05:53:37.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/rqalpha/__pycache__/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1544 2024-04-07 14:18:21.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/rqalpha/append_code.py
--rw-rw-r--   0 root         (0) root         (0)    10542 2024-04-07 14:12:58.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/rqalpha/rqalpha_trader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 10:57:28.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-07 11:04:36.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)      759 2024-03-07 11:04:36.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/calendar.py
--rw-r--r--   0 root         (0) root         (0)     3704 2024-04-02 23:44:21.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/context.py
--rw-r--r--   0 root         (0) root         (0)      587 2024-04-02 08:04:02.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/data.py
--rw-r--r--   0 root         (0) root         (0)     2802 2024-03-28 07:35:08.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/dictobj.py
--rw-r--r--   0 root         (0) root         (0)     6079 2024-04-03 00:53:34.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/event.py
--rw-r--r--   0 root         (0) root         (0)    11401 2024-04-02 12:03:48.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/function.py
--rw-r--r--   0 root         (0) root         (0)     4940 2024-03-28 17:49:09.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/object.py
--rw-rw-r--   0 root         (0) root         (0)     7813 2024-03-28 01:56:33.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/qmtClient.py
--rwxrwxrwx   0 root         (0) root         (0)     5367 2024-03-27 12:07:44.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/qmt_pb2.py
--rwxrwxrwx   0 root         (0) root         (0)    14005 2024-03-27 12:12:48.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/qmt_pb2_grpc.py
--rwxrwxrwx   0 root         (0) root         (0)     5060 2024-04-02 23:49:54.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/qmt_trader.py
--rw-r--r--   0 root         (0) root         (0)     8747 2024-03-26 02:45:53.000000 finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/finhack/widgets/templates/runtime/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev1/finhack/widgets/templates/runtime/__init__.py
--rw-r--r--   0 root         (0) root         (0)      540 2023-07-17 12:29:42.000000 finhack-0.0.3.dev1/finhack/widgets/templates/runtime/constant.py
--rw-r--r--   0 root         (0) root         (0)       67 2024-02-28 07:21:31.000000 finhack-0.0.3.dev1/finhack/widgets/templates/runtime/global_var.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 06:04:22.582925 finhack-0.0.3.dev1/finhack.egg-info/
--rw-r--r--   0 root         (0) root         (0)      159 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12956 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      509 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-09 06:04:22.000000 finhack-0.0.3.dev1/finhack.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 06:04:22.602924 finhack-0.0.3.dev1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      876 2024-04-09 06:04:19.000000 finhack-0.0.3.dev1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.011615 finhack-0.0.3.dev2/
+-rw-r--r--   0 root         (0) root         (0)    73748 2023-12-27 02:20:47.000000 finhack-0.0.3.dev2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      138 2024-01-18 10:18:24.000000 finhack-0.0.3.dev2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-04-29 01:42:27.011615 finhack-0.0.3.dev2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3993 2024-04-24 06:08:42.000000 finhack-0.0.3.dev2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.975614 finhack-0.0.3.dev2/examples/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-13 11:17:21.000000 finhack-0.0.3.dev2/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.975614 finhack-0.0.3.dev2/finhack/
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-29 01:42:26.000000 finhack-0.0.3.dev2/finhack/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.979614 finhack-0.0.3.dev2/finhack/collector/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/collector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 17:17:00.000000 finhack-0.0.3.dev2/finhack/collector/baseCollector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.979614 finhack-0.0.3.dev2/finhack/collector/tushare/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/collector/tushare/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.979614 finhack-0.0.3.dev2/finhack/collector/tushare/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/collector/tushare/__pycache__/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5475 2023-07-18 11:03:58.000000 finhack-0.0.3.dev2/finhack/collector/tushare/astockbasic.py
+-rwxr-xr-x   0 root         (0) root         (0)    19378 2023-07-18 11:06:31.000000 finhack-0.0.3.dev2/finhack/collector/tushare/astockfinance.py
+-rwxr-xr-x   0 root         (0) root         (0)    16164 2023-07-18 11:08:47.000000 finhack-0.0.3.dev2/finhack/collector/tushare/astockindex.py
+-rwxr-xr-x   0 root         (0) root         (0)     2437 2023-07-18 10:59:04.000000 finhack-0.0.3.dev2/finhack/collector/tushare/astockmarket.py
+-rwxr-xr-x   0 root         (0) root         (0)     7588 2023-07-18 11:15:02.000000 finhack-0.0.3.dev2/finhack/collector/tushare/astockother.py
+-rwxr-xr-x   0 root         (0) root         (0)     4228 2023-07-18 11:10:21.000000 finhack-0.0.3.dev2/finhack/collector/tushare/astockprice.py
+-rwxr-xr-x   0 root         (0) root         (0)     4534 2023-07-18 11:14:49.000000 finhack-0.0.3.dev2/finhack/collector/tushare/cb.py
+-rwxr-xr-x   0 root         (0) root         (0)     2373 2023-07-18 10:59:25.000000 finhack-0.0.3.dev2/finhack/collector/tushare/econo.py
+-rwxr-xr-x   0 root         (0) root         (0)     6335 2023-07-18 11:13:49.000000 finhack-0.0.3.dev2/finhack/collector/tushare/fund.py
+-rwxr-xr-x   0 root         (0) root         (0)     1987 2023-07-18 10:59:31.000000 finhack-0.0.3.dev2/finhack/collector/tushare/futures.py
+-rwxr-xr-x   0 root         (0) root         (0)      520 2023-07-18 11:12:40.000000 finhack-0.0.3.dev2/finhack/collector/tushare/fx.py
+-rwxr-xr-x   0 root         (0) root         (0)    10537 2023-07-18 11:12:33.000000 finhack-0.0.3.dev2/finhack/collector/tushare/helper.py
+-rwxr-xr-x   0 root         (0) root         (0)      677 2023-07-18 10:59:39.000000 finhack-0.0.3.dev2/finhack/collector/tushare/hstock.py
+-rwxr-xr-x   0 root         (0) root         (0)     1271 2023-07-18 10:59:42.000000 finhack-0.0.3.dev2/finhack/collector/tushare/other.py
+-rwxr-xr-x   0 root         (0) root         (0)     7980 2024-01-03 17:45:57.000000 finhack-0.0.3.dev2/finhack/collector/tushare/tushare_collector.py
+-rwxr-xr-x   0 root         (0) root         (0)      669 2023-07-18 10:59:45.000000 finhack-0.0.3.dev2/finhack/collector/tushare/ustock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.979614 finhack-0.0.3.dev2/finhack/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:06:37.000000 finhack-0.0.3.dev2/finhack/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.979614 finhack-0.0.3.dev2/finhack/core/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/core/__pycache__/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.979614 finhack-0.0.3.dev2/finhack/core/classes/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:05:35.000000 finhack-0.0.3.dev2/finhack/core/classes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.983614 finhack-0.0.3.dev2/finhack/core/classes/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/core/classes/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2024-04-07 06:44:16.000000 finhack-0.0.3.dev2/finhack/core/classes/dictobj.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.983614 finhack-0.0.3.dev2/finhack/core/command/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/core/command/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1236 2024-01-30 03:58:55.000000 finhack-0.0.3.dev2/finhack/core/command/finhack
+-rw-r--r--   0 root         (0) root         (0)     9001 2024-04-15 06:01:04.000000 finhack-0.0.3.dev2/finhack/core/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.983614 finhack-0.0.3.dev2/finhack/core/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/core/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.983614 finhack-0.0.3.dev2/finhack/core/data/logs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/core/data/logs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.983614 finhack-0.0.3.dev2/finhack/core/loader/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:10:41.000000 finhack-0.0.3.dev2/finhack/core/loader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.983614 finhack-0.0.3.dev2/finhack/core/loader/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/core/loader/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2024-01-31 04:25:19.000000 finhack-0.0.3.dev2/finhack/core/loader/base_loader.py
+-rw-r--r--   0 root         (0) root         (0)      294 2024-01-04 11:30:36.000000 finhack-0.0.3.dev2/finhack/core/loader/collector_loader.py
+-rw-r--r--   0 root         (0) root         (0)      277 2024-01-04 11:30:49.000000 finhack-0.0.3.dev2/finhack/core/loader/factor_loader.py
+-rw-r--r--   0 root         (0) root         (0)      285 2024-01-04 11:32:05.000000 finhack-0.0.3.dev2/finhack/core/loader/helper_loader.py
+-rw-r--r--   0 root         (0) root         (0)      315 2024-01-04 11:32:07.000000 finhack-0.0.3.dev2/finhack/core/loader/trader_loader.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 07:25:21.000000 finhack-0.0.3.dev2/finhack/core/notify.py
+-rw-r--r--   0 root         (0) root         (0)      121 2024-01-23 07:25:27.000000 finhack-0.0.3.dev2/finhack/core/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.983614 finhack-0.0.3.dev2/finhack/factor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/factor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.983614 finhack-0.0.3.dev2/finhack/factor/default/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-04 10:31:48.000000 finhack-0.0.3.dev2/finhack/factor/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.987614 finhack-0.0.3.dev2/finhack/factor/default/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/factor/default/__pycache__/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    24778 2024-03-19 03:48:09.000000 finhack-0.0.3.dev2/finhack/factor/default/alphaEngine.py
+-rw-r--r--   0 root         (0) root         (0)     4955 2024-04-03 01:54:17.000000 finhack-0.0.3.dev2/finhack/factor/default/default_factor.py
+-rwxrwxrwx   0 root         (0) root         (0)    18152 2024-03-04 11:36:16.000000 finhack-0.0.3.dev2/finhack/factor/default/factorAnalyzer.py
+-rwxrwxrwx   0 root         (0) root         (0)     7888 2024-03-04 10:37:04.000000 finhack-0.0.3.dev2/finhack/factor/default/factorManager.py
+-rwxrwxrwx   0 root         (0) root         (0)    13617 2024-04-03 01:56:59.000000 finhack-0.0.3.dev2/finhack/factor/default/factorMining.py
+-rwxrwxrwx   0 root         (0) root         (0)     3034 2024-03-04 10:32:09.000000 finhack-0.0.3.dev2/finhack/factor/default/factorPkl.py
+-rw-r--r--   0 root         (0) root         (0)     3529 2023-07-18 16:57:34.000000 finhack-0.0.3.dev2/finhack/factor/default/factorRepair.py
+-rwxrwxrwx   0 root         (0) root         (0)    20166 2024-03-18 10:50:36.000000 finhack-0.0.3.dev2/finhack/factor/default/indicatorCompute.py
+-rwxrwxrwx   0 root         (0) root         (0)    18873 2024-03-19 04:08:04.000000 finhack-0.0.3.dev2/finhack/factor/default/preCheck.py
+-rwxrwxrwx   0 root         (0) root         (0)     2675 2024-03-19 01:59:28.000000 finhack-0.0.3.dev2/finhack/factor/default/taskRunner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.987614 finhack-0.0.3.dev2/finhack/helper/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/helper/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.987614 finhack-0.0.3.dev2/finhack/helper/struct/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/helper/struct/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      192 2023-10-30 10:01:09.000000 finhack-0.0.3.dev2/finhack/helper/struct/struct_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.987614 finhack-0.0.3.dev2/finhack/library/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/library/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.987614 finhack-0.0.3.dev2/finhack/library/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/library/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2024-04-03 02:00:10.000000 finhack-0.0.3.dev2/finhack/library/ai.py
+-rwxrwxrwx   0 root         (0) root         (0)     1437 2024-02-28 08:52:26.000000 finhack-0.0.3.dev2/finhack/library/alert.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-12-28 02:00:35.000000 finhack-0.0.3.dev2/finhack/library/class_loader.py
+-rw-r--r--   0 root         (0) root         (0)      771 2024-03-18 12:40:27.000000 finhack-0.0.3.dev2/finhack/library/config.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2024-03-27 04:56:20.000000 finhack-0.0.3.dev2/finhack/library/log.py
+-rwxrwxrwx   0 root         (0) root         (0)     3254 2023-07-18 11:03:32.000000 finhack-0.0.3.dev2/finhack/library/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2024-02-28 10:19:22.000000 finhack-0.0.3.dev2/finhack/library/mycache.py
+-rwxrwxrwx   0 root         (0) root         (0)     3088 2023-07-18 03:02:15.000000 finhack-0.0.3.dev2/finhack/library/mydb.py
+-rwxrwxrwx   0 root         (0) root         (0)      830 2023-09-18 06:59:38.000000 finhack-0.0.3.dev2/finhack/library/thread.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-12-26 11:12:16.000000 finhack-0.0.3.dev2/finhack/library/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.987614 finhack-0.0.3.dev2/finhack/market/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:22:54.000000 finhack-0.0.3.dev2/finhack/market/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.987614 finhack-0.0.3.dev2/finhack/market/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/market/__pycache__/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.987614 finhack-0.0.3.dev2/finhack/market/astock/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-20 07:33:55.000000 finhack-0.0.3.dev2/finhack/market/astock/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.987614 finhack-0.0.3.dev2/finhack/market/astock/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/market/astock/__pycache__/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1690 2024-01-04 15:33:35.000000 finhack-0.0.3.dev2/finhack/market/astock/astock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.987614 finhack-0.0.3.dev2/finhack/market/astock/tushare/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-04 06:44:17.000000 finhack-0.0.3.dev2/finhack/market/astock/tushare/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17309 2024-04-08 09:49:34.000000 finhack-0.0.3.dev2/finhack/market/astock/tushare/astock.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-04-01 02:44:49.000000 finhack-0.0.3.dev2/finhack/market/astock/tushare/indexHelper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.987614 finhack-0.0.3.dev2/finhack/plugin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/plugin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.987614 finhack-0.0.3.dev2/finhack/plugin/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/plugin/default/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      126 2023-11-02 17:26:48.000000 finhack-0.0.3.dev2/finhack/plugin/default/default_plugin.py
+-rw-r--r--   0 root         (0) root         (0)      508 2024-04-29 01:42:26.000000 finhack-0.0.3.dev2/finhack/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.987614 finhack-0.0.3.dev2/finhack/server/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 09:57:12.000000 finhack-0.0.3.dev2/finhack/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.987614 finhack-0.0.3.dev2/finhack/server/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 09:57:12.000000 finhack-0.0.3.dev2/finhack/server/default/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5545 2024-04-07 17:24:34.000000 finhack-0.0.3.dev2/finhack/server/default/default_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.991614 finhack-0.0.3.dev2/finhack/trader/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/trader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.991614 finhack-0.0.3.dev2/finhack/trader/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/trader/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.991614 finhack-0.0.3.dev2/finhack/trader/default/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/trader/default/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      759 2023-12-08 09:41:42.000000 finhack-0.0.3.dev2/finhack/trader/default/calendar.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2024-04-03 00:02:23.000000 finhack-0.0.3.dev2/finhack/trader/default/context.py
+-rw-r--r--   0 root         (0) root         (0)    17061 2024-03-05 05:58:00.000000 finhack-0.0.3.dev2/finhack/trader/default/data.py
+-rw-r--r--   0 root         (0) root         (0)    11700 2024-04-07 08:17:55.000000 finhack-0.0.3.dev2/finhack/trader/default/default_trader.py
+-rw-r--r--   0 root         (0) root         (0)     9720 2023-12-23 18:52:29.000000 finhack-0.0.3.dev2/finhack/trader/default/event.py
+-rw-r--r--   0 root         (0) root         (0)    19045 2024-04-07 06:35:50.000000 finhack-0.0.3.dev2/finhack/trader/default/function.py
+-rw-r--r--   0 root         (0) root         (0)     4930 2024-03-05 06:26:36.000000 finhack-0.0.3.dev2/finhack/trader/default/object.py
+-rw-r--r--   0 root         (0) root         (0)     9397 2024-04-04 16:15:25.000000 finhack-0.0.3.dev2/finhack/trader/default/performance.py
+-rw-r--r--   0 root         (0) root         (0)     8597 2024-03-26 02:45:51.000000 finhack-0.0.3.dev2/finhack/trader/default/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.991614 finhack-0.0.3.dev2/finhack/trainer/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/trainer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.991614 finhack-0.0.3.dev2/finhack/trainer/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/trainer/__pycache__/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.991614 finhack-0.0.3.dev2/finhack/trainer/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/trainer/auto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       32 2024-01-23 10:56:05.000000 finhack-0.0.3.dev2/finhack/trainer/auto/auto_trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.991614 finhack-0.0.3.dev2/finhack/trainer/lightgbm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/trainer/lightgbm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.991614 finhack-0.0.3.dev2/finhack/trainer/lightgbm/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/trainer/lightgbm/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13418 2024-03-22 09:36:36.000000 finhack-0.0.3.dev2/finhack/trainer/lightgbm/lightgbm_trainer.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2024-03-26 06:58:49.000000 finhack-0.0.3.dev2/finhack/trainer/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.991614 finhack-0.0.3.dev2/finhack/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.991614 finhack-0.0.3.dev2/finhack/widgets/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/widgets/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.991614 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 03:52:10.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/.proj
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.991614 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/auto/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-03 03:37:25.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.991614 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/auto/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 03:44:51.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/auto/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.991614 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/backtest/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-26 08:46:08.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/backtest/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/backtest/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-26 08:46:08.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/backtest/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/backtest/default/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 02:17:07.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/backtest/default/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8421 2024-04-07 14:16:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/backtest/default/default_backtest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/choice/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/choice/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/factors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/index/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/index/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/kv/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/kv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/market/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/market/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/notice/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 07:28:17.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/notice/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/price/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/price/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/runtime/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 09:02:59.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/runtime/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/runtime/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/runtime/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      914 2024-04-27 10:21:01.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/runtime/constant.py
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-27 10:21:01.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/runtime/global_var.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 08:25:47.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/runtime.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-29 01:42:26.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/ai.conf
+-rwxrwxrwx   0 root         (0) root         (0)      398 2024-04-29 01:42:26.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/alert.conf
+-rw-r--r--   0 root         (0) root         (0)     4433 2024-04-04 09:56:10.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/args.conf
+-rw-rw-r--   0 root         (0) root         (0)      283 2024-04-04 09:53:25.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/backtest.conf
+-rw-r--r--   0 root         (0) root         (0)      847 2024-03-15 02:02:17.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/constant.conf
+-rw-r--r--   0 root         (0) root         (0)       18 2023-12-28 01:09:57.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/core.conf
+-rwxrwxrwx   0 root         (0) root         (0)      336 2024-04-29 01:42:26.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/db.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.995615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    13827 2024-03-04 08:10:44.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha101
+-rwxrwxrwx   0 root         (0) root         (0)    22039 2022-12-04 10:31:48.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha191
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3010 2024-04-27 10:21:03.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/all
+-rw-r--r--   0 root         (0) root         (0)     3443 2023-05-03 18:51:57.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/woldy
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-04-17 10:39:56.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/autotrain
+-rw-r--r--   0 root         (0) root         (0)       67 2024-02-28 07:23:35.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/global_var.conf
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-05-09 07:57:06.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/task.conf
+-rw-rw-r--   0 root         (0) root         (0)      106 2024-04-03 03:14:00.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/trader.conf
+-rw-r--r--   0 root         (0) root         (0)       21 2023-12-24 17:51:59.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/train.conf
+-rwxrwxrwx   0 root         (0) root         (0)      148 2024-04-29 01:42:26.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/ts.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/code_factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/code_factors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/date_factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 01:42:26.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/date_factors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/single_factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/single_factors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 04:41:32.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/all_factors.parquet/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 06:44:04.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/all_factors.parquet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 10:44:16.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/_tmp/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:11:07.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/_tmp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:28:19.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/_tmp/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:28:19.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/_tmp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/logs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/logs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/logs/trader/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/logs/trader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/preds/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/preds/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 08:48:12.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2253 2024-04-07 08:36:40.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/static/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/static/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/static/css/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/static/css/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/static/images/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/static/images/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/static/js/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/static/js/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/static/rqalpha/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 05:53:37.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/static/rqalpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/static/trader/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/static/trader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.999615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/running/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 04:10:28.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/running/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.003615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/
+-rw-r--r--   0 root         (0) root         (0)     1195 2022-12-07 19:27:24.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/QIML365.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-04 10:31:48.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.003615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/__pycache__/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8109 2024-01-07 01:31:52.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/extend.py
+-rwxrwxrwx   0 root         (0) root         (0)     5827 2024-01-07 01:43:56.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/financial.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-03-20 07:07:21.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/member.py
+-rwxrwxrwx   0 root         (0) root         (0)     1948 2024-01-07 01:32:06.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/myfactors.py
+-rwxrwxrwx   0 root         (0) root         (0)    21290 2024-01-07 01:32:35.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/ta_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)     1954 2024-01-07 01:33:13.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/volumeprice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.003615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/loader/
+-rw-r--r--   0 root         (0) root         (0)      523 2023-12-28 01:38:27.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/loader/1testmodule_loader.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/loader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.003615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/loader/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 01:51:08.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/loader/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      521 2024-01-04 11:32:51.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/loader/testmodule_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.003615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/prompt/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 09:34:57.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/prompt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.003615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/prompts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 09:03:25.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/prompts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.003615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/script/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 11:25:50.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/script/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.003615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/strategy/
+-rw-r--r--   0 root         (0) root         (0)     3047 2024-04-01 11:33:59.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/strategy/AITopNStrategy.py
+-rw-r--r--   0 root         (0) root         (0)     3348 2024-01-30 07:19:08.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2024-04-07 04:58:56.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/strategy/DemoStrategy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/strategy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.003615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/strategy/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/strategy/__pycache__/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.003615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/testmodule/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/testmodule/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.003615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/testmodule/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/testmodule/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.003615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/testmodule/default/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 01:51:08.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/testmodule/default/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2024-03-25 02:37:56.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/testmodule/default/default_testmodule.py
+-rw-r--r--   0 root         (0) root         (0)      400 2023-07-24 08:45:41.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/testmodule/default/testmodule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.003615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 10:57:17.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.003615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-13 11:19:29.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/__pycache__/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.007615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 10:57:28.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.007615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-07 11:04:36.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      759 2024-03-07 11:04:36.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/calendar.py
+-rw-r--r--   0 root         (0) root         (0)       66 2024-03-12 08:46:32.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/client.py
+-rw-r--r--   0 root         (0) root         (0)     3704 2024-04-02 23:44:21.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/context.py
+-rw-r--r--   0 root         (0) root         (0)      587 2024-04-02 08:04:02.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/data.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2024-04-07 06:43:50.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/dictobj.py
+-rw-r--r--   0 root         (0) root         (0)     6065 2024-04-26 01:39:48.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/event.py
+-rw-r--r--   0 root         (0) root         (0)    11669 2024-04-26 01:40:00.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/function.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2024-04-10 01:57:16.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/object.py
+-rw-rw-r--   0 root         (0) root         (0)     7813 2024-04-07 15:23:44.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/qmtClient.py
+-rwxrwxrwx   0 root         (0) root         (0)     5367 2024-03-27 12:07:44.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2.py
+-rwxrwxrwx   0 root         (0) root         (0)    14005 2024-03-27 12:12:48.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2_grpc.py
+-rwxrwxrwx   0 root         (0) root         (0)     5464 2024-04-22 11:53:46.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/qmt_trader.py
+-rw-r--r--   0 root         (0) root         (0)     8691 2024-04-25 08:07:36.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.007615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/rqalpha/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 05:53:37.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/rqalpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.007615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/rqalpha/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 05:53:37.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/rqalpha/__pycache__/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1544 2024-04-07 14:18:21.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/rqalpha/append_code.py
+-rw-rw-r--   0 root         (0) root         (0)    10542 2024-04-07 14:12:58.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/rqalpha/rqalpha_trader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.011615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 10:57:28.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.011615 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-07 11:04:36.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      759 2024-03-07 11:04:36.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/calendar.py
+-rw-r--r--   0 root         (0) root         (0)     3704 2024-04-02 23:44:21.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/context.py
+-rw-r--r--   0 root         (0) root         (0)      587 2024-04-02 08:04:02.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/data.py
+-rw-r--r--   0 root         (0) root         (0)     2802 2024-03-28 07:35:08.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/dictobj.py
+-rw-r--r--   0 root         (0) root         (0)     6079 2024-04-03 00:53:34.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/event.py
+-rw-r--r--   0 root         (0) root         (0)    11401 2024-04-02 12:03:48.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/function.py
+-rw-r--r--   0 root         (0) root         (0)     4940 2024-03-28 17:49:09.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/object.py
+-rw-rw-r--   0 root         (0) root         (0)     7813 2024-03-28 01:56:33.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/qmtClient.py
+-rwxrwxrwx   0 root         (0) root         (0)     5367 2024-03-27 12:07:44.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/qmt_pb2.py
+-rwxrwxrwx   0 root         (0) root         (0)    14005 2024-03-27 12:12:48.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/qmt_pb2_grpc.py
+-rwxrwxrwx   0 root         (0) root         (0)     5060 2024-04-02 23:49:54.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/qmt_trader.py
+-rw-r--r--   0 root         (0) root         (0)     8626 2024-04-10 02:49:27.000000 finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:27.011615 finhack-0.0.3.dev2/finhack/widgets/templates/runtime/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.3.dev2/finhack/widgets/templates/runtime/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      540 2023-07-17 12:29:42.000000 finhack-0.0.3.dev2/finhack/widgets/templates/runtime/constant.py
+-rw-r--r--   0 root         (0) root         (0)       67 2024-02-28 07:21:31.000000 finhack-0.0.3.dev2/finhack/widgets/templates/runtime/global_var.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 01:42:26.975614 finhack-0.0.3.dev2/finhack.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-04-29 01:42:26.000000 finhack-0.0.3.dev2/finhack.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12956 2024-04-29 01:42:26.000000 finhack-0.0.3.dev2/finhack.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 01:42:26.000000 finhack-0.0.3.dev2/finhack.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      509 2024-04-29 01:42:26.000000 finhack-0.0.3.dev2/finhack.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-29 01:42:26.000000 finhack-0.0.3.dev2/finhack.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 01:42:27.011615 finhack-0.0.3.dev2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      876 2024-04-24 06:07:08.000000 finhack-0.0.3.dev2/setup.py
```

### Comparing `finhack-0.0.3.dev1/LICENSE.txt` & `finhack-0.0.3.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/README.md` & `finhack-0.0.3.dev2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,18 @@
 # FinHack® 炼金术(自测中，5月份开放内测)
+- 如果有更新，那就是亏钱了
+- 如果更新的很频繁，那就是亏了很多钱
+- 啥时候不更新了，就是赚到钱了
+- 啥时候删库了，就是赚到大钱了
+
+--
+
+最近不更新了，理由是我发现日频回测太不靠谱了，目前正在思考分钟级回测以及多品种回测的解决方案（2024.04.19）
+
+
 ## 项目介绍
 <div>FinHack®, an easily extensible quantitative finance framework, integrates a complete workflow for quantitative investment research in its current version, including data collection, factor computation, factor mining, factor analysis, machine learning, strategy development, and quantitative backtesting. In later stages, it will expand to include more data sources, trading instruments, analytical tools, and practical plugins, aiming to create an open, customizable, and high-level quantitative finance framework to aid Quants and researchers in related fields with their financial research work.</div>
 <br/>
 FinHack®，一个易于拓展的量化金融框架，它在当前版本中集成了<B>数据采集、因子计算、因子挖掘、因子分析、机器学习、策略编写、量化回测、实盘接入</B>等全流程的量化投研工作，后期它将拓展出更多的数据源、交易品种与分析工具与实用插件，力求打造一个开放的、可定制的、高水平的量化金融框架，助力广大Quant与相关学科工作者的金融研究工作。
 
 ## 项目特点
 - 良好的拓展性，包括但不限于拓展自己的数据源、因子、AI模型、量化策略以及回测规则
```

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/astockbasic.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/astockbasic.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/astockfinance.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/astockfinance.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/astockindex.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/astockindex.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/astockmarket.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/astockmarket.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/astockother.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/astockother.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/astockprice.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/astockprice.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/cb.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/cb.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/econo.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/econo.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/fund.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/fund.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/futures.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/futures.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/fx.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/fx.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/helper.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/helper.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/hstock.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/hstock.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/other.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/other.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/tushare_collector.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/tushare_collector.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/collector/tushare/ustock.py` & `finhack-0.0.3.dev2/finhack/collector/tushare/ustock.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/core/classes/dictobj.py` & `finhack-0.0.3.dev2/finhack/core/classes/dictobj.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/core/command/finhack` & `finhack-0.0.3.dev2/finhack/core/command/finhack`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/core/core.py` & `finhack-0.0.3.dev2/finhack/core/core.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/core/loader/base_loader.py` & `finhack-0.0.3.dev2/finhack/core/loader/base_loader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/factor/default/alphaEngine.py` & `finhack-0.0.3.dev2/finhack/factor/default/alphaEngine.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/factor/default/default_factor.py` & `finhack-0.0.3.dev2/finhack/factor/default/default_factor.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/factor/default/factorAnalyzer.py` & `finhack-0.0.3.dev2/finhack/factor/default/factorAnalyzer.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/factor/default/factorManager.py` & `finhack-0.0.3.dev2/finhack/factor/default/factorManager.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/factor/default/factorMining.py` & `finhack-0.0.3.dev2/finhack/factor/default/factorMining.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/factor/default/factorPkl.py` & `finhack-0.0.3.dev2/finhack/factor/default/factorPkl.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/factor/default/factorRepair.py` & `finhack-0.0.3.dev2/finhack/factor/default/factorRepair.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/factor/default/indicatorCompute.py` & `finhack-0.0.3.dev2/finhack/factor/default/indicatorCompute.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/factor/default/preCheck.py` & `finhack-0.0.3.dev2/finhack/factor/default/preCheck.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/factor/default/taskRunner.py` & `finhack-0.0.3.dev2/finhack/factor/default/taskRunner.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/library/ai.py` & `finhack-0.0.3.dev2/finhack/library/ai.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/library/alert.py` & `finhack-0.0.3.dev2/finhack/library/alert.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/library/class_loader.py` & `finhack-0.0.3.dev2/finhack/library/class_loader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/library/config.py` & `finhack-0.0.3.dev2/finhack/library/config.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/library/log.py` & `finhack-0.0.3.dev2/finhack/library/log.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/library/monitor.py` & `finhack-0.0.3.dev2/finhack/library/monitor.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/library/mycache.py` & `finhack-0.0.3.dev2/finhack/library/mycache.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/library/mydb.py` & `finhack-0.0.3.dev2/finhack/library/mydb.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/library/thread.py` & `finhack-0.0.3.dev2/finhack/library/thread.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/library/utils.py` & `finhack-0.0.3.dev2/finhack/library/utils.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/market/astock/astock.py` & `finhack-0.0.3.dev2/finhack/market/astock/astock.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/market/astock/tushare/astock.py` & `finhack-0.0.3.dev2/finhack/market/astock/tushare/astock.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/market/astock/tushare/indexHelper.py` & `finhack-0.0.3.dev2/finhack/market/astock/tushare/indexHelper.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/server/default/default_server.py` & `finhack-0.0.3.dev2/finhack/server/default/default_server.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/trader/default/calendar.py` & `finhack-0.0.3.dev2/finhack/trader/default/calendar.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/trader/default/context.py` & `finhack-0.0.3.dev2/finhack/trader/default/context.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/trader/default/data.py` & `finhack-0.0.3.dev2/finhack/trader/default/data.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/trader/default/default_trader.py` & `finhack-0.0.3.dev2/finhack/trader/default/default_trader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/trader/default/event.py` & `finhack-0.0.3.dev2/finhack/trader/default/event.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/trader/default/function.py` & `finhack-0.0.3.dev2/finhack/trader/default/function.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/trader/default/object.py` & `finhack-0.0.3.dev2/finhack/trader/default/object.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/trader/default/performance.py` & `finhack-0.0.3.dev2/finhack/trader/default/performance.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/trader/default/rules.py` & `finhack-0.0.3.dev2/finhack/trader/default/rules.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/trainer/lightgbm/lightgbm_trainer.py` & `finhack-0.0.3.dev2/finhack/trainer/lightgbm/lightgbm_trainer.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/trainer/trainer.py` & `finhack-0.0.3.dev2/finhack/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/backtest/default/default_backtest.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/backtest/default/default_backtest.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime/constant.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/runtime/constant.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/cache/runtime.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/cache/runtime.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/args.conf` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/args.conf`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/constant.conf` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/constant.conf`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha101` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha101`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha191` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha191`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/all` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/all`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/woldy` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/woldy`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/autotrain` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/autotrain`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/data/reports/index.html` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/data/reports/index.html`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/QIML365.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/QIML365.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/extend.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/extend.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/financial.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/financial.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/myfactors.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/myfactors.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/ta_lib.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/ta_lib.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/indicators/volumeprice.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/indicators/volumeprice.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/1testmodule_loader.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/loader/1testmodule_loader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/loader/testmodule_loader.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/loader/testmodule_loader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/AITopNStrategy.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/strategy/AITopNStrategy.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/strategy/DemoStrategy.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/strategy/DemoStrategy.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/testmodule/default/default_testmodule.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/testmodule/default/default_testmodule.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/calendar.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/calendar.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/context.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/context.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/data.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/data.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/dictobj.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/dictobj.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/event.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         
         
 
     def before_market(context):
         # 获取今天的日期
         today = datetime.today().strftime('%Y%m%d')
         # 获取今天前三天的日期
-        thirty_days_ago = (datetime.today() - timedelta(days=15)).strftime('%Y%m%d')
+        thirty_days_ago = (datetime.today() - timedelta(days=3)).strftime('%Y%m%d')
         model_id=context.trade.model_id
         preds=load_preds_data(model_id=model_id,start_time=thirty_days_ago,end_time=today)
         context.g.preds=preds
         return True
```

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/function.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     else:
         context.id=hash_value
     qclient.assetSync(context)
     qclient.positionSync(context)
 
 
 
+
 def set_benchmark(code):
     context['trade']['benchmark']=code
     
 def set_option(key,value):
     if key in context['trade']:
         context['trade'][key]=value
     elif key in context['account']:
@@ -110,20 +111,21 @@
     if match and time.count(':')==1:
         hours, minutes = time.split(":")
         time = f"{hours.zfill(2)}:{minutes.zfill(2)}:00"
      
     for date in date_list:
         new_event={
             'event_name':func.__name__,
-            'event_func':func,
+            #'event_func':func,
             'event_time':date+' '+time,
             'event_type':'user_event'
         }
         context['data']['event_list'].append(new_event)
-        context['data']['event_list'].sort(key=lambda x: x['event_time'])
+    context['data']['event_list'].sort(key=lambda x: x['event_time'])
+       
     
 def run_daily(func,time,reference_security=None):
     return run_interval(func,time,'daily',date_list=context['data']['calendar'])
 
 
 # #这个函数是按交易日，预留，懒得写逻辑
 # def run_tmonthly(func, monthday, time='9:30', reference_security=None, force=False):
@@ -246,14 +248,15 @@
 #         self.amount=amount
 #         self.enable_amount=enable_amount
 #         self.last_sale_price=last_sale_price
 #         self.cost_basis=last_sale_price
 #         self.total_value=amount*last_sale_price
 
 def order_buy(security,amount,price=None):  
+    log(f"调用order_buy买入{security}共{amount}股,价格为{str(None)}")  
     o=Order(code=security,amount=amount,is_buy=True,context=context)
     rules=Rules(order=o,context=context,log=log)
     o=rules.apply()
 
     if o.status!=1:
         return False
     if o.amount==0:
@@ -263,14 +266,15 @@
         o.price=price
     qclient.OrderBuy(o.code,o.amount,o.price)
     log(f"下单买入{o.code}共计{o.amount}股，单价{o.price}")   
     return True
       
 
 def order_sell(security,amount,price=None):
+    log(f"调用order_sell卖出{security}共{amount}股,价格为{str(None)}")  
     o=Order(code=security,amount=amount,is_buy=False,context=context)
     rules=Rules(order=o,context=context,log=log)
     o=rules.apply()
     if o.status!=1:
         return False
     if o.amount==0:
         log(f"{o.code}--{o.amount}，卖单数为0，自动取消订单")
```

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/object.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/object.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmtClient.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/qmtClient.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2_grpc.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/qmt_trader.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/qmt_trader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/qmt/rules.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/rules.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/rqalpha/append_code.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/rqalpha/append_code.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/rqalpha/rqalpha_trader.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/rqalpha/rqalpha_trader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/calendar.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/calendar.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/context.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/context.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/data.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/data.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/dictobj.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/dictobj.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/event.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,20 +45,20 @@
         calendar=context['data']['calendar']
         for date in calendar:
             for event_name,event_time in daily_event_list['astock']:
                 if hasattr(Event, event_name):
                     func = getattr(Event, event_name)
                     new_event={
                         'event_name':event_name,
-                        'event_func':func,
+                        #'event_func':func,
                         'event_time':date+' '+event_time,
                         'event_type':'market_event'
                     }
                     context['data']['event_list'].append(new_event)
-                    context['data']['event_list'].sort(key=lambda x: x['event_time'])                
+        context['data']['event_list'].sort(key=lambda x: x['event_time'])            
                     
         return True
         
         
     def start_interval(context):
         now_date=context.current_dt.strftime('%Y%m%d')
         start_date=context.trade.start_time[0:10].replace('-','')
@@ -69,15 +69,15 @@
         
         
 
     def before_market(context):
         # 获取今天的日期
         today = datetime.today().strftime('%Y%m%d')
         # 获取今天前三天的日期
-        thirty_days_ago = (datetime.today() - timedelta(days=3)).strftime('%Y%m%d')
+        thirty_days_ago = (datetime.today() - timedelta(days=15)).strftime('%Y%m%d')
         model_id=context.trade.model_id
         preds=load_preds_data(model_id=model_id,start_time=thirty_days_ago,end_time=today)
         context.g.preds=preds
         return True
```

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/function.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/function.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/object.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/object.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 class Order():
     def __init__(self,code='',amount='',is_buy=True,side='long',action='',context=None):
         self.code=code
         self.amount=amount
         self.enable_amount=amount
         self.filled=0
         self.info=Data.get_daily_info(code=code,context=context)
+        print(self.info)
         self.price=Data.get_price(code=code,context=context)
         self.order_id = self.generate_order_id()
         self.is_buy=is_buy
         self.cost=0
         self.slip_value=0 #滑点滑掉了多少
         self.last_sale_price=None
         #正常
```

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/qmtClient.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/qmtClient.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/qmt_pb2.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/qmt_pb2.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/qmt_pb2_grpc.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/qmt_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/qmt_trader.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/qmt/qmt_trader.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,16 @@
         starttime=datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         init_context(self.args)
         loaded_context = self.load_context(context)
         if loaded_context is not None:
             context = loaded_context
         else:
             pass
+        
+
 
         start_time=context['trade']['start_time']
         end_time=context['trade']['end_time']
         market=context['trade']['market']
         
         Log.tlogger=Log.tLog(context.id,logs_dir=LOGS_DIR,background=self.args.background,level=self.args.log_level).logger
         log("正在初始化交易上下文")
@@ -109,18 +111,26 @@
                 time_to_wait = (event_time - current_time).total_seconds()
                 log(f"下次事件时间{event_time}，将在{time_to_wait}秒后执行，正在sleep等待…")
                 time.sleep(time_to_wait)  # 等待直到事件时间到达
             else:
                 # 如果 event_time 在当前时间的10秒钟以内
                 if 0 <= (current_time - event_time).total_seconds() < 10:
                     log(f"执行{event['event_name']}")
-                    event['event_func'](context)
+
+                    if event['event_type']=="market_event":
+                        event_func = getattr(Event, event['event_name'])
+                    elif event['event_type']=="user_event":
+                        event_func = getattr(strategy, event['event_name'])
+                    else:
+                        log(f"未知时间{event['event_name']}")
+                    event_func(context)
                 else:
                     continue  # 如果时间早于当前时间超过10秒，则跳过此事件
 
             # 更新context的日期信息
             if context.previous_date is None or context.current_dt is None:
                 pass
             elif context.current_dt.date() != event_time.date():
                 context.previous_date = context.current_dt.date()
-            context.current_dt = event_time
-            self.save_context(context)
+            #context.current_dt = event_time
+            self.save_context(context)
+        log("全部事件执行完毕")
```

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/empty_project/trader/sim/rules.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/empty_project/trader/sim/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,18 +102,14 @@
             if self.order.price<=self.order.info.downLimit and self.order.price==self.order.info.low:
                 self.order.filled=0
                 self.log(f"{self.order.code}跌停，无法卖出！",'warning')  
                 return False
         return True
 
     def rule_100(self):
-        print('---')
-        print(self.order.amount)
-        print(int(self.order.amount/100)*100)
-        print('---')
         if self.order.amount!=int(self.order.amount/100)*100:
             self.order.amount=int(self.order.amount/100)*100
             self.log(f"{self.order.code}自动调整交易数量为{self.order.amount}！",'warning')  
         return True
```

### Comparing `finhack-0.0.3.dev1/finhack/widgets/templates/runtime/constant.py` & `finhack-0.0.3.dev2/finhack/widgets/templates/runtime/constant.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/finhack.egg-info/SOURCES.txt` & `finhack-0.0.3.dev2/finhack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finhack-0.0.3.dev1/setup.py` & `finhack-0.0.3.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import os 
 
 root_dir = 'finhack'
-version='0.0.3.dev1'
+version='0.0.3.dev2'
 
 for subdir, dirs, files in os.walk(root_dir):
     if not '__init__.py' in files:
         init_file_path = os.path.join(subdir, '__init__.py')
         open(init_file_path, 'a').close()
         print(f'Created __init__.py in {subdir}')
```

