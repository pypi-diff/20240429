# Comparing `tmp/tqsdk-3.5.7.tar.gz` & `tmp/tqsdk-3.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tqsdk-3.5.7.tar", last modified: Tue Apr 23 02:18:44 2024, max compression
+gzip compressed data, was "dist/tqsdk-3.5.8.tar", last modified: Mon Apr 29 10:12:41 2024, max compression
```

## Comparing `tqsdk-3.5.7.tar` & `tqsdk-3.5.8.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/
--rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/rangeset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/baseModule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/stockprofit.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/datetime_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)    19888 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tqwebhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/data_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/sm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/demo/example/
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/aberration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/rbreaker2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/doublema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/turtle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/gridtrading.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/vwap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/dualthrust.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/gridtrading_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/rbreaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/momentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/escalator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/fairy_four_price.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/random_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t70.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t20.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t30.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t91.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t93.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/replay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t80.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/replay2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t71.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t92.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t60.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t90.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t96.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t40.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t41.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/underlying_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/backtest.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t94.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t95.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t72.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/multiaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/download_orders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/ta_option.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o41.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o72.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o30.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o71.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o40.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o20.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o70.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o74.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o73.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o60.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/ta.py
--rw-r--r--   0 runner    (1001) docker     (127)    21994 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)    20999 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/objs_not_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/trading_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/backtest/
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/backtest/replay.py
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/backtest/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/backtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43337 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/backtest/backtest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/__pyinstaller/hook-tqsdk.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/risk_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)    15912 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/algorithm/time_table_generater.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/algorithm/twap.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/multiaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/baseApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/risk_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/utils_symbols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/lib/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/lib/time_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/lib/target_pos_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37335 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/lib/target_pos_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    52750 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/tafunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    37797 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/objs.py
--rw-r--r--   0 runner    (1001) docker     (127)   210161 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/trade_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)   132245 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/expired_quotes.json.lzma
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/tradeable/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/
--rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/tqsim.py
--rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/trade_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    36480 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/trade_future.py
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27585 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/trade_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/tqsim_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)    18113 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/basesim.py
--rw-r--r--   0 runner    (1001) docker     (127)    15130 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/tradeable/otg/
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/otg/tqkq.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/otg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/otg/tqaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/otg/tqzq.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/otg/base_otg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/tradeable.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/web/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/web/js/
--rw-r--r--   0 runner    (1001) docker     (127)  1787845 2024-04-23 02:18:10.000000 tqsdk-3.5.7/tqsdk/web/js/chunk-vendors.d7fceff6.js
--rw-r--r--   0 runner    (1001) docker     (127)    62759 2024-04-23 02:18:10.000000 tqsdk-3.5.7/tqsdk/web/js/app.2c843c86.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/web/img/
--rw-r--r--   0 runner    (1001) docker     (127)   555353 2024-04-23 02:18:05.000000 tqsdk-3.5.7/tqsdk/web/img/ionicons.a2c4a261.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/web/img/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-23 02:18:09.000000 tqsdk-3.5.7/tqsdk/web/img/icons/ms-icon-70x70.png
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-23 02:18:05.000000 tqsdk-3.5.7/tqsdk/web/img/icons/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-23 02:18:07.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-23 02:18:09.000000 tqsdk-3.5.7/tqsdk/web/img/icons/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-23 02:18:07.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-76x76.png
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-23 02:18:06.000000 tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-48x48.png
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/favicon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-23 02:18:05.000000 tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-23 02:18:06.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-23 02:18:07.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-23 02:18:06.000000 tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-36x36.png
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-23 02:18:07.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-23 02:18:09.000000 tqsdk-3.5.7/tqsdk/web/img/icons/msapplication-icon-144x144.png.png
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-23 02:18:05.000000 tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-23 02:18:06.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-114x114.png
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-04-23 02:18:09.000000 tqsdk-3.5.7/tqsdk/web/img/icons/ms-icon-310x310.png
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-23 02:18:06.000000 tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-23 02:18:07.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-57x57.png
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-23 02:18:09.000000 tqsdk-3.5.7/tqsdk/web/img/icons/notes
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-23 02:18:06.000000 tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-23 02:18:06.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-23 02:18:09.000000 tqsdk-3.5.7/tqsdk/web/img/icons/ms-icon-150x150.png
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-23 02:18:07.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-180x180.png
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-23 02:18:03.000000 tqsdk-3.5.7/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/web/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   197740 2024-04-23 02:18:04.000000 tqsdk-3.5.7/tqsdk/web/fonts/ionicons.99ac3308.woff
--rw-r--r--   0 runner    (1001) docker     (127)   197664 2024-04-23 02:18:05.000000 tqsdk-3.5.7/tqsdk/web/fonts/ionicons.d535a25a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    82216 2024-04-23 02:18:04.000000 tqsdk-3.5.7/tqsdk/web/fonts/ionicons.143146fa.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-23 02:18:03.000000 tqsdk-3.5.7/tqsdk/web/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   246120 2024-04-23 02:18:03.000000 tqsdk-3.5.7/tqsdk/web/d3.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-23 02:18:04.000000 tqsdk-3.5.7/tqsdk/web/service-worker.js
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 02:18:03.000000 tqsdk-3.5.7/tqsdk/web/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-23 02:18:03.000000 tqsdk-3.5.7/tqsdk/web/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/web/css/
--rw-r--r--   0 runner    (1001) docker     (127)   279508 2024-04-23 02:18:04.000000 tqsdk-3.5.7/tqsdk/web/css/chunk-vendors.c93e9127.css
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-23 02:18:04.000000 tqsdk-3.5.7/tqsdk/web/css/app.d72d8978.css
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-23 02:18:03.000000 tqsdk-3.5.7/tqsdk/web/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tools/dead_ins.lzma
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21845 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tools/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    20440 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    91538 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/ta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)    21813 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/ins_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    23562 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/data_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-23 02:18:01.000000 tqsdk-3.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-23 02:18:01.000000 tqsdk-3.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-23 02:18:44.000000 tqsdk-3.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-23 02:18:01.000000 tqsdk-3.5.7/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 02:18:44.000000 tqsdk-3.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-23 02:18:01.000000 tqsdk-3.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/rangeset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/baseModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/stockprofit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/datetime_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19888 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tqwebhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/data_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/sm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/demo/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/aberration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/rbreaker2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/doublema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/gridtrading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/vwap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/dualthrust.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/gridtrading_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/rbreaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/momentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/escalator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/fairy_four_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/random_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t70.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t30.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t91.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t93.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t80.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/replay2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t71.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t92.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t60.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t90.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t96.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t40.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t41.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/underlying_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t94.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t95.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t72.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/multiaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/download_orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/ta_option.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o41.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o72.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o30.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o71.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o20.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o70.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o74.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o73.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o60.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/ta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21994 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20999 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/objs_not_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/trading_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/backtest/
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/backtest/replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/backtest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/backtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44023 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/backtest/backtest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/__pyinstaller/hook-tqsdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/risk_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)    15912 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/algorithm/time_table_generater.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/algorithm/twap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/multiaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/baseApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/risk_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/utils_symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/lib/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/lib/time_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/lib/target_pos_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40355 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/lib/target_pos_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52750 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tafunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37797 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/objs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   210312 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/trade_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)   132245 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/expired_quotes.json.lzma
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/tradeable/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/tqsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/trade_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36480 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/trade_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27585 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/trade_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/tqsim_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18113 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/basesim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15130 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/tradeable/otg/
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/otg/tqkq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/otg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/otg/tqaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/otg/tqzq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/otg/base_otg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/tradeable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/web/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/web/js/
+-rw-r--r--   0 runner    (1001) docker     (127)  1787845 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/js/chunk-vendors.d7fceff6.js
+-rw-r--r--   0 runner    (1001) docker     (127)    62759 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/js/app.2c843c86.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/web/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   555353 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/img/ionicons.a2c4a261.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/web/img/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/ms-icon-70x70.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/img/icons/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/favicon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-36x36.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/msapplication-icon-144x144.png.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-114x114.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/ms-icon-310x310.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-57x57.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/notes
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/ms-icon-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-180x180.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/web/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   197740 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/fonts/ionicons.99ac3308.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   197664 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/fonts/ionicons.d535a25a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    82216 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/fonts/ionicons.143146fa.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   246120 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/d3.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/service-worker.js
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/web/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   279508 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/css/chunk-vendors.c93e9127.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/css/app.d72d8978.css
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tools/dead_ins.lzma
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21566 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tools/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20440 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91538 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/ta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22562 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/ins_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23562 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/data_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-29 10:12:08.000000 tqsdk-3.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-29 10:12:08.000000 tqsdk-3.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-29 10:12:41.000000 tqsdk-3.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-29 10:12:08.000000 tqsdk-3.5.8/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-29 10:12:41.000000 tqsdk-3.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-29 10:12:08.000000 tqsdk-3.5.8/setup.py
```

### Comparing `tqsdk-3.5.7/tqsdk/rangeset.py` & `tqsdk-3.5.8/tqsdk/rangeset.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/baseModule.py` & `tqsdk-3.5.8/tqsdk/baseModule.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/stockprofit.py` & `tqsdk-3.5.8/tqsdk/stockprofit.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/datetime_state.py` & `tqsdk-3.5.8/tqsdk/datetime_state.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/datetime.py` & `tqsdk-3.5.8/tqsdk/datetime.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tqwebhelper.py` & `tqsdk-3.5.8/tqsdk/tqwebhelper.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/symbols.py` & `tqsdk-3.5.8/tqsdk/symbols.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/data_extension.py` & `tqsdk-3.5.8/tqsdk/data_extension.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/sm.py` & `tqsdk-3.5.8/tqsdk/sm.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/example/aberration.py` & `tqsdk-3.5.8/tqsdk/demo/example/aberration.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/example/rbreaker2.py` & `tqsdk-3.5.8/tqsdk/demo/example/rbreaker2.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/example/doublema.py` & `tqsdk-3.5.8/tqsdk/demo/example/doublema.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/example/turtle.py` & `tqsdk-3.5.8/tqsdk/demo/example/turtle.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/example/gridtrading.py` & `tqsdk-3.5.8/tqsdk/demo/example/gridtrading.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/example/vwap.py` & `tqsdk-3.5.8/tqsdk/demo/example/vwap.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/example/dualthrust.py` & `tqsdk-3.5.8/tqsdk/demo/example/dualthrust.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/example/gridtrading_async.py` & `tqsdk-3.5.8/tqsdk/demo/example/gridtrading_async.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/example/rbreaker.py` & `tqsdk-3.5.8/tqsdk/demo/example/rbreaker.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/example/momentum.py` & `tqsdk-3.5.8/tqsdk/demo/example/momentum.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/example/escalator.py` & `tqsdk-3.5.8/tqsdk/demo/example/escalator.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/example/fairy_four_price.py` & `tqsdk-3.5.8/tqsdk/demo/example/fairy_four_price.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/example/random_forest.py` & `tqsdk-3.5.8/tqsdk/demo/example/random_forest.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t70.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t70.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t20.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t20.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t30.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t30.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t91.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t91.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t93.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t93.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/replay.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/replay.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t80.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t80.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/replay2.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/replay2.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t71.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t71.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t92.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t92.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/downloader.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/downloader.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t60.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t60.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t90.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t90.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t96.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t96.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t40.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t40.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t41.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t41.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/backtest.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/backtest.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t94.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t94.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t95.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t95.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/tutorial/t72.py` & `tqsdk-3.5.8/tqsdk/demo/tutorial/t72.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/multiaccount.py` & `tqsdk-3.5.8/tqsdk/demo/multiaccount.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/download_orders.py` & `tqsdk-3.5.8/tqsdk/demo/download_orders.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/ta_option.py` & `tqsdk-3.5.8/tqsdk/demo/ta_option.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o41.py` & `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o41.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o72.py` & `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o72.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o30.py` & `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o30.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o71.py` & `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o71.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o40.py` & `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o40.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o20.py` & `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o20.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o70.py` & `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o70.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o74.py` & `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o74.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o73.py` & `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o73.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o60.py` & `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o60.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/demo/ta.py` & `tqsdk-3.5.8/tqsdk/demo/ta.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/connect.py` & `tqsdk-3.5.8/tqsdk/connect.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/objs_not_entity.py` & `tqsdk-3.5.8/tqsdk/objs_not_entity.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/auth.py` & `tqsdk-3.5.8/tqsdk/auth.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/trading_status.py` & `tqsdk-3.5.8/tqsdk/trading_status.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/utils.py` & `tqsdk-3.5.8/tqsdk/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/backtest/replay.py` & `tqsdk-3.5.8/tqsdk/backtest/replay.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/backtest/utils.py` & `tqsdk-3.5.8/tqsdk/backtest/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/backtest/backtest.py` & `tqsdk-3.5.8/tqsdk/backtest/backtest.py`

 * *Files 4% similar despite different names*

```diff
@@ -346,15 +346,15 @@
                 else:
                     self._current_dt = timestamp  # 否则将回测时间更新至最新行情时间
             diff = self._serials[min_request_key]["diff"]
             self._diffs.append(diff)
             # klines 请求，需要记录已经发送 api 的数据
             for symbol in diff.get("klines", {}):
                 for dur in diff["klines"][symbol]:
-                    for kid in diff["klines"][symbol][dur]["data"]:
+                    for kid in diff["klines"][symbol][dur].get('data', {}):
                         rs = self._sended_to_api.setdefault((symbol, int(dur)), [])
                         kid = int(kid)
                         self._sended_to_api[(symbol, int(dur))] = _rangeset_range_union(rs, (kid, kid + 1))
             # 记录用于生成 quote 的信息
             quotes_helper[min_request_key] = {
                 "timestamp": timestamp,
                 "kline_or_tick": self._serials[min_request_key]["kline_or_tick"],
@@ -386,30 +386,32 @@
             symbol = ins.split(",")[0]
             if quotes_helper[key]["is_before_current_dt"] and self._quotes.get(symbol, {}).get("sended_init_quote"):
                 # 先订阅 A 合约，再订阅 A 合约日线，那么 A 合约的行情时间会回退: 2021-01-04 09:31:59.999999 -> 2021-01-01 18:00:00.000000
                 # 如果当前 timestamp 小于 _current_dt，那么这个 quote_diff 不需要发到下游
                 # 如果先订阅 A 合约（有夜盘），时间停留在夜盘开始时间， 再订阅 B 合约（没有夜盘），那么 B 合约的行情（前一天收盘时间）应该发下去，
                 # 否则 get_quote(B) 等到收到行情才返回，会直接把时间推进到第二天白盘。
                 continue
+            item = quotes_helper[key]["kline_or_tick"]
+            if item is None:
+                # item 如果是 None 的话，没有可以生成行情的信息的数据，那么不生成 quote_diff
+                continue
             diffs = None
             if self._quotes[symbol]['min_duration'] == 0 and dur == 0:
                 # tick 生成行情
-                tick = quotes_helper[key]["kline_or_tick"]
-                diffs = TqBacktest._get_quote_diffs_from_tick(symbol, tick)
+                diffs = TqBacktest._get_quote_diffs_from_tick(symbol, item)
             if self._quotes[symbol]['min_duration'] != 0:
                 # kline 生成行情
                 when = quotes_helper[key]["when"]
                 timestamp = quotes_helper[key]["timestamp"]  # quote 行情时间
-                kline = quotes_helper[key]["kline_or_tick"]
                 quote_info = self._data["quotes"][symbol]
                 froms = ["open"] if when == "OPEN" else ["close"]
                 if when == "CLOSE" and self._quotes[symbol]['min_duration'] == dur:
                     # kline 生成 quote 数据，只有该合约订阅的最小周期会生成 high low 对应的行情
                     froms = ["high", "low", "close"]
-                diffs = TqBacktest._get_quote_diffs_from_kline(symbol, quote_info['price_tick'], timestamp, kline, froms)
+                diffs = TqBacktest._get_quote_diffs_from_kline(symbol, quote_info['price_tick'], timestamp, item, froms)
             if diffs:
                 self._quotes[symbol]["sended_init_quote"] = True
                 self._diffs.extend(diffs)
 
     def _get_backtest_time(self) -> dict:
         if self._is_first_send:
             self._is_first_send = False
@@ -501,26 +503,39 @@
             await self._md_send_chan.send(chart_info.copy())
             try:
                 async for _ in update_chan:
                     chart = _get_obj(self._data, ["charts", chart_info["chart_id"]])
                     if not (chart_info.items() <= _get_obj(chart, ["state"]).items()):
                         # 当前请求还没收齐回应, 不应继续处理
                         continue
-                    left_id = chart.get("left_id", -1)
-                    right_id = chart.get("right_id", -1)
-                    if (left_id == -1 and right_id == -1) or chart.get("more_data", True):
-                        continue  # 定位信息还没收到, 数据没有完全收到
+                    if not chart.get("ready", False):
+                        continue  # chart 数据还没准备好
                     last_id = serials[0].get("last_id", -1)
                     if last_id == -1:
-                        continue  # 数据序列还没收到
+                        # 所有合约的 tick 数据一定有，开盘一定会收到一笔 tick
+                        # kline 是由有价格的 tick 生成的，所以 kline 可能没有数据的
+                        assert dur > 0
+                        diff = {
+                            "klines": {
+                                symbol_list[0]: {
+                                    str(dur): {
+                                        "last_id": -1
+                                    }
+                                }
+                            }
+                        }
+                        yield self._current_dt, diff, None, "OPEN"
+                        return
                     if self._data.get("mdhis_more_data", True):
                         self._data["_listener"].add(update_chan)
                         continue
                     else:
                         self._data["_listener"].discard(update_chan)
+                    left_id = chart.get("left_id", -1)
+                    right_id = chart.get("right_id", -1)
                     if current_id is None:
                         current_id = max(left_id, 0)
                     # 发送下一段 chart 8964 根 kline
                     chart_info["chart_id"] = chart_id_b if chart_info["chart_id"] == chart_id_a else chart_id_a
                     chart_info["left_kline_id"] = right_id
                     chart_info.pop("focus_datetime", None)
                     chart_info.pop("focus_position", None)
```

### Comparing `tqsdk-3.5.7/tqsdk/risk_rule.py` & `tqsdk-3.5.8/tqsdk/risk_rule.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/algorithm/time_table_generater.py` & `tqsdk-3.5.8/tqsdk/algorithm/time_table_generater.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/algorithm/twap.py` & `tqsdk-3.5.8/tqsdk/algorithm/twap.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/__init__.py` & `tqsdk-3.5.8/tqsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/multiaccount.py` & `tqsdk-3.5.8/tqsdk/multiaccount.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/baseApi.py` & `tqsdk-3.5.8/tqsdk/baseApi.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/calendar.py` & `tqsdk-3.5.8/tqsdk/calendar.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/risk_manager.py` & `tqsdk-3.5.8/tqsdk/risk_manager.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/utils_symbols.py` & `tqsdk-3.5.8/tqsdk/utils_symbols.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/lib/notify.py` & `tqsdk-3.5.8/tqsdk/lib/notify.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/lib/target_pos_scheduler.py` & `tqsdk-3.5.8/tqsdk/lib/target_pos_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,28 +131,28 @@
                                                     trade_objs_chan=self._trade_objs_chan,
                                                     account=self._account)
                     target_pos_task.set_target_volume(row['target_pos'])
                 if _index < self._time_table.shape[0] - 1:  # 非最后一项
                     async for _ in self._api.register_update_notify(quote):
                         if _get_trade_timestamp(quote.datetime, float('nan')) > row['deadline']:
                             if target_pos_task:
-                                target_pos_task._task.cancel()
-                                await asyncio.gather(target_pos_task._task, return_exceptions=True)
+                                target_pos_task.cancel()
+                                await asyncio.gather(target_pos_task, return_exceptions=True)
                             break
                 elif target_pos_task:  # 最后一项，如果有 target_pos_task 等待持仓调整完成，否则直接退出
                     position = self._account.get_position(self._symbol)
                     if position.pos != row['target_pos']:
                         async for _ in self._api.register_update_notify(position):
                             if position.pos == row['target_pos']:
                                 break
                 _index = _index + 1
         finally:
             if target_pos_task:
-                target_pos_task._task.cancel()
-                await asyncio.gather(target_pos_task._task, return_exceptions=True)
+                target_pos_task.cancel()
+                await asyncio.gather(target_pos_task, return_exceptions=True)
             await self._trade_objs_chan.close()
             await self._trade_recv_task
 
     async def _trade_recv(self):
         async for trade in self._trade_objs_chan:
             self.trades_df.loc[self.trades_df.shape[0]] = [trade[k] for k in self._trade_keys]
```

### Comparing `tqsdk-3.5.7/tqsdk/lib/utils.py` & `tqsdk-3.5.8/tqsdk/lib/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/lib/target_pos_task.py` & `tqsdk-3.5.8/tqsdk/lib/target_pos_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -210,14 +210,41 @@
         self._pos_chan = TqChan(self._api, last_only=True)
         self._trade_chan = trade_chan
         self._trade_objs_chan = trade_objs_chan
         self._task = self._api.create_task(self._target_pos_task())
         self._time_update_task = self._api.create_task(self._update_time_from_md())  # 监听行情更新并记录当时本地时间的task
         self._local_time_record = time.time() - 0.005  # 更新最新行情时间时的本地时间
         self._local_time_record_update_chan = TqChan(self._api, last_only=True)  # 监听 self._local_time_record 更新
+        self._wait_task_finished = self._api._loop.create_future()
+        self._task.add_done_callback(lambda _: self._api.create_task(self._exit_task()))
+
+    async def _exit_task(self):
+        """
+        执行 task.cancel() 时, 删除掉该 symbol 对应的 TargetPosTask 实例，以释放占有的资源。
+
+        当用户代码为：
+        t = TargetPosTask(api, 'SHFE.rb2106', min_volume=2, max_volume=10)
+        t.cancel()
+        await asyncio.gather(t._task, return_exceptions=True)
+
+        以上代码执行后，t._task 中的 finally 部分没有被执行过，因为 t._task 本身从来没有被执行过。
+
+        所以这里用 add_done_callback 的方式，处理 __init__ 方法中创建的资源。
+        self._task、self._pos_chan、self._time_update_task 都是在 __init__ 方法里创建的资源，所以在这里释放资源，
+        self._task 中的 finally 部分只处理在 self._task 函数里创建的资源。
+        """
+        # self._account 类型为 TqSim/TqKq/TqAccount，都包括 _account_key 变量
+        TargetPosTaskSingleton._instances.pop(self._account._account_key + "#" + self._symbol, None)
+        await self._pos_chan.close()
+        self._time_update_task.cancel()
+        await asyncio.gather(self._time_update_task, return_exceptions=True)
+        self._wait_task_finished.set_result(True)
+
+    def __await__(self):
+        return self._wait_task_finished.__await__()
 
     def set_target_volume(self, volume: int) -> None:
         """
         设置目标持仓手数
 
         Args:
             volume (int): 目标持仓手数，正数表示多头，负数表示空头，0表示空仓
@@ -375,20 +402,15 @@
                                                                max_volume=self._max_volume, price=self._price,
                                                                trade_chan=self._trade_chan,
                                                                trade_objs_chan=self._trade_objs_chan,
                                                                account=self._account)
                     all_tasks.append(order_task)
                     delta_volume -= order_volume if order_dir == "BUY" else -order_volume
         finally:
-            # 执行 task.cancel() 时, 删除掉该 symbol 对应的 TargetPosTask 实例
-            # self._account 类型为 TqSim/TqKq/TqAccount，都包括 _account_key 变量
-            TargetPosTaskSingleton._instances.pop(self._account._account_key + "#" + self._symbol, None)
-            await self._pos_chan.close()
-            self._time_update_task.cancel()
-            await asyncio.gather(*([t._task for t in all_tasks] + [self._time_update_task]), return_exceptions=True)
+            await asyncio.gather(*[t._task for t in all_tasks], return_exceptions=True)
 
     def cancel(self):
         """
         取消当前 TargetPosTask 实例，会将该实例已经发出但还是未成交的委托单撤单，并且如果后续调用此实例的 set_target_volume 函数会报错。
 
         任何时刻，每个账户下一个合约只能有一个 TargetPosTask 实例，并且其构造参数不能修改。
 
@@ -419,25 +441,68 @@
 
             while True:
                 api.wait_update()
                 # ... 策略代码 ...
 
             api.close()
 
+
+        Example2::
+
+            # 在异步代码中使用
+            from datetime import datetime, time
+            from tqsdk import TqApi, TargetPosTask
+
+            api = TqApi(auth=TqAuth("快期账户", "账户密码"))
+            quote = api.get_quote("SHFE.rb2110")
+
+            async def demo(SYMBOL):
+                quote = await api.get_quote(SYMBOL)
+                target_pos_passive = TargetPosTask(api, SYMBOL, price="PASSIVE")
+                async with api.register_update_notify() as update_chan:
+                    async for _ in update_chan:
+                        if datetime.strptime(quote.datetime, "%Y-%m-%d %H:%M:%S.%f").time() < time(14, 50):
+                            # ... 策略代码 ...
+                        else:
+                            target_pos_passive.cancel()  # 取消 TargetPosTask 实例
+                            await target_pos_passive  # 等待 target_pos_passive 处理 cancel 结束
+                            break
+
+                target_pos_active = TargetPosTask(api, "SHFE.rb2110", price="ACTIVE")
+                target_pos_active.set_target_volume(0)  # 平所有仓位
+                pos = await api.get_position(SYMBOL)
+                async with api.register_update_notify() as update_chan:
+                    async for _ in update_chan:
+                        if pos.pos == 0:
+                            target_pos_active.cancel()  # 取消 TargetPosTask 实例
+                            await target_pos_active  # 等待 target_pos_active 处理 cancel 结束
+                            break
+
+
+            symbol_list = ["SHFE.rb2107", "DCE.m2109"]  # 设置合约代码
+            for symbol in symbol_list:
+                api.create_task(demo("SHFE.rb2107"))  # 为每个合约创建异步任务
+
+            while True:
+                api.wait_update()
+
         """
         self._task.cancel()
 
     def is_finished(self) -> bool:
         """
         返回当前 TargetPosTask 实例是否已经结束。即如果后续调用此实例的 set_target_volume 函数会报错，此实例不会再下单或者撤单。
 
         Returns:
             bool: 当前 TargetPosTask 实例是否已经结束
         """
-        return self._task.done()
+        if self._wait_task_finished.done():
+            assert self._task.done() is True
+            return self._wait_task_finished.result()
+        return False
 
 
 class InsertOrderUntilAllTradedTask(object):
     """追价下单task, 该task会在行情变化后自动撤单重下，直到全部成交
      （注：此类主要在tqsdk内部使用，并非简单用法，不建议用户使用）"""
 
     def __init__(self, api, symbol, direction, offset, volume, min_volume: Optional[int] = None,
```

### Comparing `tqsdk-3.5.7/tqsdk/tafunc.py` & `tqsdk-3.5.8/tqsdk/tafunc.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/exceptions.py` & `tqsdk-3.5.8/tqsdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/log.py` & `tqsdk-3.5.8/tqsdk/log.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/objs.py` & `tqsdk-3.5.8/tqsdk/objs.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/api.py` & `tqsdk-3.5.8/tqsdk/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2819,15 +2819,20 @@
                 api.wait_update()
 
             api.close()
 
         """
         if self._stock is False:
             raise Exception("期货行情系统(_stock = False)不支持当前接口调用")
-        symbol_list = [symbol] if isinstance(symbol, str) else symbol
+        if isinstance(symbol, str):
+            symbol_list = [symbol]
+        else:
+            if len(symbol) == 0:
+                raise Exception("symbol 参数不能为空列表。")
+            symbol_list = symbol
         if any([s == "" for s in symbol_list]):
             raise Exception(f"symbol 参数 {symbol} 中不能有空字符串。")
         backtest_timestamp = _datetime_to_timestamp_nano(self._get_current_datetime()) if isinstance(self._backtest,
                                                                                                TqBacktest) else None
         df = TqSymbolDataFrame(self, symbol_list, backtest_timestamp=backtest_timestamp)
         deadline = time.time() + 30
         while not self._loop.is_running() and not df.__dict__["_task"].done():
```

### Comparing `tqsdk-3.5.7/tqsdk/entity.py` & `tqsdk-3.5.8/tqsdk/entity.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/trade_extension.py` & `tqsdk-3.5.8/tqsdk/trade_extension.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/expired_quotes.json.lzma` & `tqsdk-3.5.8/tqsdk/expired_quotes.json.lzma`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/channel.py` & `tqsdk-3.5.8/tqsdk/channel.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tradeable/sim/tqsim.py` & `tqsdk-3.5.8/tqsdk/tradeable/sim/tqsim.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tradeable/sim/trade_base.py` & `tqsdk-3.5.8/tqsdk/tradeable/sim/trade_base.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tradeable/sim/trade_future.py` & `tqsdk-3.5.8/tqsdk/tradeable/sim/trade_future.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tradeable/sim/utils.py` & `tqsdk-3.5.8/tqsdk/tradeable/sim/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tradeable/sim/trade_stock.py` & `tqsdk-3.5.8/tqsdk/tradeable/sim/trade_stock.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tradeable/sim/tqsim_stock.py` & `tqsdk-3.5.8/tqsdk/tradeable/sim/tqsim_stock.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tradeable/sim/basesim.py` & `tqsdk-3.5.8/tqsdk/tradeable/sim/basesim.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tradeable/mixin.py` & `tqsdk-3.5.8/tqsdk/tradeable/mixin.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tradeable/otg/tqkq.py` & `tqsdk-3.5.8/tqsdk/tradeable/otg/tqkq.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tradeable/otg/tqaccount.py` & `tqsdk-3.5.8/tqsdk/tradeable/otg/tqaccount.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tradeable/otg/tqzq.py` & `tqsdk-3.5.8/tqsdk/tradeable/otg/tqzq.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tradeable/otg/base_otg.py` & `tqsdk-3.5.8/tqsdk/tradeable/otg/base_otg.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tradeable/tradeable.py` & `tqsdk-3.5.8/tqsdk/tradeable/tradeable.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/js/chunk-vendors.d7fceff6.js` & `tqsdk-3.5.8/tqsdk/web/js/chunk-vendors.d7fceff6.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/js/app.2c843c86.js` & `tqsdk-3.5.8/tqsdk/web/js/app.2c843c86.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/ionicons.a2c4a261.svg` & `tqsdk-3.5.8/tqsdk/web/img/ionicons.a2c4a261.svg`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/ms-icon-70x70.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/ms-icon-70x70.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/android-chrome-192x192.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-60x60.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/mstile-150x150.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-76x76.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-48x48.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-48x48.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/favicon-96x96.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-144x144.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-144x144.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-72x72.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-36x36.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-36x36.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-152x152.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/favicon.ico` & `tqsdk-3.5.8/tqsdk/web/img/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/msapplication-icon-144x144.png.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/msapplication-icon-144x144.png.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-192x192.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-192x192.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-114x114.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/ms-icon-310x310.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/ms-icon-310x310.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-72x72.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/favicon-32x32.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-57x57.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/notes` & `tqsdk-3.5.8/tqsdk/web/img/icons/notes`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-96x96.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-96x96.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/favicon-16x16.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-120x120.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/ms-icon-150x150.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/ms-icon-150x150.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-precomposed.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/manifest.json` & `tqsdk-3.5.8/tqsdk/web/img/icons/manifest.json`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-180x180.png` & `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js` & `tqsdk-3.5.8/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/fonts/ionicons.99ac3308.woff` & `tqsdk-3.5.8/tqsdk/web/fonts/ionicons.99ac3308.woff`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/fonts/ionicons.d535a25a.ttf` & `tqsdk-3.5.8/tqsdk/web/fonts/ionicons.d535a25a.ttf`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/fonts/ionicons.143146fa.woff2` & `tqsdk-3.5.8/tqsdk/web/fonts/ionicons.143146fa.woff2`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/favicon.ico` & `tqsdk-3.5.8/tqsdk/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/d3.min.js` & `tqsdk-3.5.8/tqsdk/web/d3.min.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/service-worker.js` & `tqsdk-3.5.8/tqsdk/web/service-worker.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/index.html` & `tqsdk-3.5.8/tqsdk/web/index.html`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/css/chunk-vendors.c93e9127.css` & `tqsdk-3.5.8/tqsdk/web/css/chunk-vendors.c93e9127.css`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/css/app.d72d8978.css` & `tqsdk-3.5.8/tqsdk/web/css/app.d72d8978.css`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/web/manifest.json` & `tqsdk-3.5.8/tqsdk/web/manifest.json`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tools/dead_ins.lzma` & `tqsdk-3.5.8/tqsdk/tools/dead_ins.lzma`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/tools/downloader.py` & `tqsdk-3.5.8/tqsdk/tools/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     历史数据下载器, 输出到csv文件
 
     多合约按时间横向对齐
     """
 
     def __init__(self, api: TqApi, symbol_list: Union[str, List[str]], dur_sec: int, start_dt: Union[date, datetime],
-                 end_dt: Union[date, datetime], csv_file_name: Union[str, asyncio.StreamWriter],
+                 end_dt: Union[date, datetime], csv_file_name: Union[str, asyncio.StreamWriter], write_mode: str = "w",
                  adj_type: Union[str, None] = None) -> None:
         """
         创建历史数据下载器实例
 
         Args:
             api (TqApi): TqApi实例，该下载器将使用指定的api下载数据
 
@@ -65,14 +65,16 @@
                 * datetime: 指的是具体时间点，如果没有指定时区信息，则默认为北京时间
 
             csv_file_name (str/StreamWriter): [必填]输出方式:
                 * str : 输出 csv 的文件名
 
                 * StreamWriter: 直接将内容输出到 StreamWriter
 
+            write_mode (str): 写入模式，默认值为 "w"。"w" 表示覆盖写入，会写入标题行，再写入数据；"a" 表示追加写入，不写标题行，直接写入数据。
+
             adj_type (str/None): 复权计算方式，默认值为 None。"F" 为前复权；"B" 为后复权；None 表示不复权。只对股票、基金合约有效。
 
         Example::
 
             from datetime import datetime, date
             from contextlib import closing
             from tqsdk import TqApi, TqAuth, TqSim
@@ -114,14 +116,17 @@
         if adj_type not in [None, "F", "B", "FORWARD", "BACK"]:
             raise Exception("adj_type 参数只支持 None (不复权) ｜ 'F' (前复权) ｜ 'B' (后复权)")
         self._adj_type = adj_type[0] if adj_type else adj_type
         if isinstance(csv_file_name, str) or isinstance(csv_file_name, asyncio.StreamWriter):
             self._csv_file_name = csv_file_name
         else:
             raise Exception("csv_file_name 参数只支持 str ｜ StreamWriter 类型")
+        if write_mode not in ["w", "a"]:
+            raise Exception("write_mode 参数只支持 'w' ｜ 'a'")
+        self._write_mode = write_mode
         self._csv_header = self._get_headers()
         # 缓存合约对应的复权系数矩阵，每个合约只计算一次
         # 含义为截止 datetime 之前(不包含) 应使用 factor 复权
         self._dividend_cache = {}
         self._data_series = None
         self._task = self._api.create_task(self._run())
 
@@ -201,18 +206,18 @@
                 chart = _get_obj(self._api._data, ["charts", chart_info["chart_id"]])
                 serial = _get_obj(self._api._data, ["klines", quote.instrument_id, str(86400000000000)])
                 try:
                     async with self._api.register_update_notify() as update_chan:
                         async for _ in update_chan:
                             if not (chart_info.items() <= _get_obj(chart, ["state"]).items()):
                                 continue  # 当前请求还没收齐回应, 不应继续处理
+                            if chart.get("ready", False) is False:
+                                continue  # 合约的数据是否收到
                             left_id = chart.get("left_id", -1)
-                            right_id = chart.get("right_id", -1)
-                            if (left_id == -1 and right_id == -1) or self._api._data.get("mdhis_more_data", True) or serial.get("last_id", -1) == -1:
-                                continue  # 定位信息还没收到, 或数据序列还没收到, 合约的数据是否收到
+                            assert left_id != -1  # 需要下载除权除息日的前一天行情，即这一天一定是有行情的，left_id 一定不是 -1
                             last_item = serial["data"].get(str(left_id), {})
                             # 复权时间点的昨收盘
                             df.loc[i, 'pre_close'] = last_item['close'] if last_item.get('close') else float('nan')
                             break
                 finally:
                     await self._api._send_chan.send({
                         "aid": "set_chart",
@@ -252,17 +257,18 @@
         else:
             cols = ["last_price", "highest", "lowest"]
             cols.extend(f"{x}{i}" for x in ["bid_price", "ask_price"] for i in range(1, 6))
         try:
             if isinstance(self._csv_file_name, asyncio.StreamWriter):
                 writer = StreamWriter(self._csv_file_name)
             else:
-                writer = open(self._csv_file_name, 'w', newline='')
+                writer = open(self._csv_file_name, self._write_mode, newline='')
             csv_writer = csv.writer(writer, dialect='excel')
-            csv_writer.writerow(self._csv_header)
+            if self._write_mode == "w":
+                csv_writer.writerow(self._csv_header)
             async for item in gen:
                 for quote in self._quote_list:
                     symbol = quote.instrument_id
                     if self._adj_type and quote.ins_class in ["STOCK", "FUND"]:
                         # 如果存在 STOCK / FUND 并且 adj_type is not None, 这里需要提前准备下载时间段内的复权因子
                         # 前复权需要提前计算除权因子
                         await self._ensure_dividend_factor(quote, item[index_datetime_nano])
@@ -287,56 +293,47 @@
                 self._csv_file_name.write_eof()
             else:
                 writer.close()
             # 这里 `await gen.aclose()` 实际测试代码与文档描述不符，无论文件全部下载完正常退出还是写文件过程中抛出例外退出，都没有再抛出任何例外
             # https://docs.python.org/3/reference/expressions.html#agen.aclose
             await gen.aclose()
 
-    async def _timeout_handle(self, timeout, chart):
-        await asyncio.sleep(timeout)
-        if chart.get("left_id", -1) == -1 and chart.get("right_id", -1) == -1:
-            self._task.cancel()
-
     async def _download_data(self):
         """下载数据, 多合约横向按时间对齐"""
         chart_info = {
             "aid": "set_chart",
             "chart_id": _generate_uuid("PYSDK_downloader"),
             "ins_list": ",".join(self._symbol_list),
             "duration": self._dur_nano,
             "view_width": 2000,
             "focus_datetime": self._start_dt_nano,
             "focus_position": 0,
         }
         # 还没有发送过任何请求, 先请求定位左端点
         await self._api._send_chan.send(chart_info)
         chart = _get_obj(self._api._data, ["charts", chart_info["chart_id"]])
-        # 增加一个 task，在 30s 后检查 chart 是否返回了左右 id 范围，如果没有就 cancel self._task，防止程序一直卡在那里
-        timeout_task = self._api.create_task(self._timeout_handle(self._timeout_seconds, chart))
         current_id = None  # 当前数据指针
         data_cols = self._get_data_cols()
         serials = []
         for symbol in self._symbol_list:
             path = ["klines", symbol, str(self._dur_nano)] if self._dur_nano != 0 else ["ticks", symbol]
             serial = _get_obj(self._api._data, path)
             serials.append(serial)
         try:
             async with self._api.register_update_notify() as update_chan:
                 async for _ in update_chan:
                     if not (chart_info.items() <= _get_obj(chart, ["state"]).items()):
                         # 当前请求还没收齐回应, 不应继续处理
                         continue
+                    if chart.get("ready", False) is False:
+                        continue  # 数据序列还没收到，包含主合约和所有副合约
+                    if serials[0].get("last_id", -1) == -1:
+                        return  # 没有数据，直接退出
                     left_id = chart.get("left_id", -1)
                     right_id = chart.get("right_id", -1)
-                    if (left_id == -1 and right_id == -1) or chart.get("more_data", True):
-                        # 定位信息还没收到, 或数据序列还没收到
-                        continue
-                    # 检查合约的数据是否收到
-                    if any([serial.get("last_id", -1) == -1 for serial in serials]):
-                        continue
                     if current_id is None:
                         current_id = max(left_id, 0)
                     while current_id <= right_id:
                         item = serials[0]["data"].get(str(current_id), {})
                         if item.get("datetime", 0) == 0 or item["datetime"] > self._end_dt_nano:
                             # 当前 id 已超出 last_id 或k线数据的时间已经超过用户限定的右端
                             return
@@ -362,16 +359,14 @@
             await self._api._send_chan.send({
                 "aid": "set_chart",
                 "chart_id": chart_info["chart_id"],
                 "ins_list": "",
                 "duration": self._dur_nano,
                 "view_width": 2000,
             })
-            timeout_task.cancel()
-            await asyncio.gather(timeout_task, return_exceptions=True)
 
     def _get_headers(self):
         data_cols = self._get_data_cols()
         return ["datetime", "datetime_nano"] + [f"{symbol}.{col}" for symbol in self._symbol_list for col in data_cols]
 
     def _get_data_cols(self):
         if self._dur_nano != 0:
```

### Comparing `tqsdk-3.5.7/tqsdk/report.py` & `tqsdk-3.5.8/tqsdk/report.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/ta.py` & `tqsdk-3.5.8/tqsdk/ta.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/diff.py` & `tqsdk-3.5.8/tqsdk/diff.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/tqsdk/ins_schema.py` & `tqsdk-3.5.8/tqsdk/ins_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,30 @@
 # -*- coding:utf-8 -*-
 __author__ = 'yanqiong'
 
 
 import sgqlc.types
 from sgqlc.operation import Fragment
 
+
+########################################################################
+# Monkey patching 检查请求的参数是否合法，与 api.query_graphql 函数的校验规则保持一致
+########################################################################
+_origin__to_graphql_input__ = sgqlc.types.Arg.__to_graphql_input__
+
+
+def _tqsdk__to_graphql_input__(self, value, *args, **kwargs):
+    if value == "" or isinstance(value, list) and (any([s == "" for s in value]) or len(value) == 0):
+        raise Exception(f"variables 中变量值不支持空字符串、空列表或者列表中包括空字符串。")
+    return _origin__to_graphql_input__(self, value, *args, **kwargs)
+
+
+sgqlc.types.Arg.__to_graphql_input__ = _tqsdk__to_graphql_input__
+
+
 ins_schema = sgqlc.types.Schema()
 
 
 ########################################################################
 # Scalars and Enumerations
 ########################################################################
 Boolean = sgqlc.types.Boolean
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tqsdk-3.5.7/tqsdk/data_series.py` & `tqsdk-3.5.8/tqsdk/data_series.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/README.md` & `tqsdk-3.5.8/README.md`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/LICENSE` & `tqsdk-3.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/PKG-INFO` & `tqsdk-3.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tqsdk
-Version: 3.5.7
+Version: 3.5.8
 Summary: TianQin SDK
 Home-page: https://www.shinnytech.com/tqsdk
 Author: TianQin
 Author-email: tianqincn@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tqsdk-3.5.7/tqsdk.egg-info/PKG-INFO` & `tqsdk-3.5.8/tqsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tqsdk
-Version: 3.5.7
+Version: 3.5.8
 Summary: TianQin SDK
 Home-page: https://www.shinnytech.com/tqsdk
 Author: TianQin
 Author-email: tianqincn@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tqsdk-3.5.7/tqsdk.egg-info/SOURCES.txt` & `tqsdk-3.5.8/tqsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.7/setup.py` & `tqsdk-3.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", mode="r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tqsdk',
-    version="3.5.7",
+    version="3.5.8",
     description='TianQin SDK',
     author='TianQin',
     author_email='tianqincn@gmail.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://www.shinnytech.com/tqsdk',
     packages=setuptools.find_packages(exclude=["tqsdk.test", "tqsdk.test.*"]),
```

