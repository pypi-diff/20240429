# Comparing `tmp/volstreet-8.0.1.tar.gz` & `tmp/volstreet-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-8.0.1.tar", last modified: Fri Apr 26 03:29:16 2024, max compression
+gzip compressed data, was "volstreet-8.1.0.tar", last modified: Mon Apr 29 03:39:25 2024, max compression
```

## Comparing `volstreet-8.0.1.tar` & `volstreet-8.1.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.495072 volstreet-8.0.1/
--rw-rw-rw-   0        0        0     1293 2024-04-26 03:29:16.494549 volstreet-8.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-8.0.1/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-8.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1155 2024-04-26 03:29:16.496603 volstreet-8.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.376282 volstreet-8.0.1/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-8.0.1/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.396590 volstreet-8.0.1/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-26 02:47:59.000000 volstreet-8.0.1/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     3726 2024-04-26 02:48:50.000000 volstreet-8.0.1/volstreet/angel_interface/access_rate_handler.py
--rw-rw-rw-   0        0        0      274 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     2713 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    18658 2024-04-26 03:17:20.000000 volstreet-8.0.1/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-8.0.1/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    30663 2024-04-22 06:48:57.000000 volstreet-8.0.1/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6687 2024-04-26 02:56:08.000000 volstreet-8.0.1/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.421529 volstreet-8.0.1/volstreet/backtests/
--rw-rw-rw-   0        0        0      267 2024-04-24 06:53:53.000000 volstreet-8.0.1/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0     4064 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/backtests/analysis.py
--rw-rw-rw-   0        0        0     3296 2024-04-25 15:14:45.000000 volstreet-8.0.1/volstreet/backtests/data_updation.py
--rw-rw-rw-   0        0        0    11857 2024-04-25 10:13:39.000000 volstreet-8.0.1/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-8.0.1/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    48672 2024-04-24 06:53:53.000000 volstreet-8.0.1/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-8.0.1/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0     6059 2024-04-25 10:23:36.000000 volstreet-8.0.1/volstreet/backtests/proxy_functions.py
--rw-rw-rw-   0        0        0     2707 2024-04-24 14:17:18.000000 volstreet-8.0.1/volstreet/backtests/result_processing.py
--rw-rw-rw-   0        0        0     6075 2024-04-25 10:19:27.000000 volstreet-8.0.1/volstreet/backtests/runner.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-8.0.1/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-8.0.1/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     1689 2024-04-25 14:52:32.000000 volstreet-8.0.1/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    20854 2024-04-24 06:53:53.000000 volstreet-8.0.1/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     5574 2024-04-24 06:53:53.000000 volstreet-8.0.1/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.437362 volstreet-8.0.1/volstreet/datamodule/
--rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-8.0.1/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     8882 2024-04-13 05:28:03.000000 volstreet-8.0.1/volstreet/datamodule/data_handling.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-8.0.1/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-8.0.1/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-8.0.1/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.437362 volstreet-8.0.1/volstreet/historical_info/
--rw-rw-rw-   0        0        0      975 2024-04-24 06:53:53.000000 volstreet-8.0.1/volstreet/historical_info/__init__.py
--rw-rw-rw-   0        0        0    18590 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0    16832 2024-04-25 14:56:47.000000 volstreet-8.0.1/volstreet/historical_info/market_days.pkl
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.437362 volstreet-8.0.1/volstreet/models/
--rw-rw-rw-   0        0        0      565 2024-04-24 06:53:53.000000 volstreet-8.0.1/volstreet/models/__init__.py
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-8.0.1/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.446448 volstreet-8.0.1/volstreet/position_dashboard/
--rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/position_dashboard/__init__.py
--rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/position_dashboard/app.py
--rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/position_dashboard/formatting.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.457555 volstreet-8.0.1/volstreet/strategies/
--rw-rw-rw-   0        0        0      156 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0    28950 2024-04-26 03:19:34.000000 volstreet-8.0.1/volstreet/strategies/deployment.py
--rw-rw-rw-   0        0        0     5194 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    56703 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0     2949 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/strategies/monitoring.py
--rw-rw-rw-   0        0        0    17179 2024-04-10 07:52:35.000000 volstreet-8.0.1/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0    91543 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/strategies/strats.py
--rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-8.0.1/volstreet/strategies/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.457555 volstreet-8.0.1/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26799 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0    19327 2024-04-26 03:27:47.000000 volstreet-8.0.1/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    20198 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.476149 volstreet-8.0.1/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-8.0.1/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    13115 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-8.0.1/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6488 2024-04-23 04:22:25.000000 volstreet-8.0.1/volstreet/vectorized_blackscholes.py
--rw-rw-rw-   0        0        0       16 2024-04-26 02:35:35.000000 volstreet-8.0.1/volstreet/volstreet_mode.json
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.488903 volstreet-8.0.1/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-8.0.1/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-8.0.1/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-8.0.1/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-8.0.1/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-8.0.1/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:29:16.488903 volstreet-8.0.1/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1293 2024-04-26 03:29:16.000000 volstreet-8.0.1/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2833 2024-04-26 03:29:16.000000 volstreet-8.0.1/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 03:29:16.000000 volstreet-8.0.1/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      460 2024-04-26 03:29:16.000000 volstreet-8.0.1/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-26 03:29:16.000000 volstreet-8.0.1/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 03:39:25.927824 volstreet-8.1.0/
+-rw-rw-rw-   0        0        0     1293 2024-04-29 03:39:25.927824 volstreet-8.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-8.1.0/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-8.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1155 2024-04-29 03:39:25.929932 volstreet-8.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 03:39:25.766726 volstreet-8.1.0/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-8.1.0/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:39:25.793294 volstreet-8.1.0/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-26 02:47:59.000000 volstreet-8.1.0/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     3726 2024-04-26 02:48:50.000000 volstreet-8.1.0/volstreet/angel_interface/access_rate_handler.py
+-rw-rw-rw-   0        0        0      274 2024-04-23 04:22:25.000000 volstreet-8.1.0/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     2843 2024-04-28 03:29:15.000000 volstreet-8.1.0/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    18658 2024-04-26 03:17:20.000000 volstreet-8.1.0/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-8.1.0/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    30663 2024-04-22 06:48:57.000000 volstreet-8.1.0/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6687 2024-04-26 02:56:08.000000 volstreet-8.1.0/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:39:25.829102 volstreet-8.1.0/volstreet/backtests/
+-rw-rw-rw-   0        0        0      290 2024-04-28 14:01:14.000000 volstreet-8.1.0/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0     4064 2024-04-23 04:22:25.000000 volstreet-8.1.0/volstreet/backtests/analysis.py
+-rw-rw-rw-   0        0        0     4101 2024-04-28 03:48:57.000000 volstreet-8.1.0/volstreet/backtests/data_updation.py
+-rw-rw-rw-   0        0        0    11857 2024-04-25 10:13:39.000000 volstreet-8.1.0/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-8.1.0/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    48672 2024-04-24 06:53:53.000000 volstreet-8.1.0/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-8.1.0/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0     5926 2024-04-26 13:19:27.000000 volstreet-8.1.0/volstreet/backtests/proxy_functions.py
+-rw-rw-rw-   0        0        0     2707 2024-04-24 14:17:18.000000 volstreet-8.1.0/volstreet/backtests/result_processing.py
+-rw-rw-rw-   0        0        0     6051 2024-04-26 10:25:05.000000 volstreet-8.1.0/volstreet/backtests/runner.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-8.1.0/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-8.1.0/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     1689 2024-04-25 14:52:32.000000 volstreet-8.1.0/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    20854 2024-04-24 06:53:53.000000 volstreet-8.1.0/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     5574 2024-04-24 06:53:53.000000 volstreet-8.1.0/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:39:25.846356 volstreet-8.1.0/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-8.1.0/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     9035 2024-04-26 13:37:15.000000 volstreet-8.1.0/volstreet/datamodule/data_handling.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-8.1.0/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-8.1.0/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-8.1.0/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:39:25.855171 volstreet-8.1.0/volstreet/historical_info/
+-rw-rw-rw-   0        0        0      975 2024-04-24 06:53:53.000000 volstreet-8.1.0/volstreet/historical_info/__init__.py
+-rw-rw-rw-   0        0        0    18590 2024-04-29 02:56:24.000000 volstreet-8.1.0/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0    16858 2024-04-26 13:32:31.000000 volstreet-8.1.0/volstreet/historical_info/market_days.pkl
+drwxrwxrwx   0        0        0        0 2024-04-29 03:39:25.858489 volstreet-8.1.0/volstreet/models/
+-rw-rw-rw-   0        0        0      565 2024-04-24 06:53:53.000000 volstreet-8.1.0/volstreet/models/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-8.1.0/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:39:25.865641 volstreet-8.1.0/volstreet/position_dashboard/
+-rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-8.1.0/volstreet/position_dashboard/__init__.py
+-rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-8.1.0/volstreet/position_dashboard/app.py
+-rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-8.1.0/volstreet/position_dashboard/formatting.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:39:25.888081 volstreet-8.1.0/volstreet/strategies/
+-rw-rw-rw-   0        0        0      156 2024-04-17 11:41:53.000000 volstreet-8.1.0/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0    28950 2024-04-26 03:19:34.000000 volstreet-8.1.0/volstreet/strategies/deployment.py
+-rw-rw-rw-   0        0        0     5194 2024-04-17 11:41:53.000000 volstreet-8.1.0/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    51697 2024-04-29 03:38:31.000000 volstreet-8.1.0/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0     2949 2024-04-17 11:41:53.000000 volstreet-8.1.0/volstreet/strategies/monitoring.py
+-rw-rw-rw-   0        0        0    17179 2024-04-10 07:52:35.000000 volstreet-8.1.0/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0    97535 2024-04-29 03:27:51.000000 volstreet-8.1.0/volstreet/strategies/strats.py
+-rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-8.1.0/volstreet/strategies/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:39:25.896773 volstreet-8.1.0/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-8.1.0/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26799 2024-04-23 04:22:25.000000 volstreet-8.1.0/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0    19381 2024-04-28 03:28:24.000000 volstreet-8.1.0/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    20598 2024-04-28 16:45:33.000000 volstreet-8.1.0/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:39:25.910495 volstreet-8.1.0/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-8.1.0/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    13115 2024-04-23 04:22:25.000000 volstreet-8.1.0/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-8.1.0/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9915 2024-04-26 13:19:30.000000 volstreet-8.1.0/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6488 2024-04-23 04:22:25.000000 volstreet-8.1.0/volstreet/vectorized_blackscholes.py
+-rw-rw-rw-   0        0        0       16 2024-04-29 03:37:37.000000 volstreet-8.1.0/volstreet/volstreet_mode.json
+drwxrwxrwx   0        0        0        0 2024-04-29 03:39:25.923216 volstreet-8.1.0/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-8.1.0/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-8.1.0/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-8.1.0/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-8.1.0/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-8.1.0/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:39:25.926787 volstreet-8.1.0/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1293 2024-04-29 03:39:25.000000 volstreet-8.1.0/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2833 2024-04-29 03:39:25.000000 volstreet-8.1.0/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 03:39:25.000000 volstreet-8.1.0/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      460 2024-04-29 03:39:25.000000 volstreet-8.1.0/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-29 03:39:25.000000 volstreet-8.1.0/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-8.0.1/PKG-INFO` & `volstreet-8.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 8.0.1
+Version: 8.1.0
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-8.0.1/setup.cfg` & `volstreet-8.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 382e 302e 310d 0a61  rsion = 8.0.1..a
+00000020: 7273 696f 6e20 3d20 382e 312e 300d 0a61  rsion = 8.1.0..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-8.0.1/volstreet/angel_interface/access_rate_handler.py` & `volstreet-8.1.0/volstreet/angel_interface/access_rate_handler.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/angel_interface/async_interface.py` & `volstreet-8.1.0/volstreet/angel_interface/async_interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,15 +28,20 @@
                     logger.error(f"Max attempts reached. {message}")
                     raise e
 
     return async_wrapped
 
 
 @retry_on_error
-async def get_ltp_async(params: dict, session=None):
+async def get_ltp_async(token, session=None):
+    params = {
+        "exchange": token_exchange_dict.get(token),
+        "symboltoken": token,
+        "tradingsymbol": "",
+    }
     response = await ActiveSession.obj.async_get_ltp(params, session)
     return response["data"]["ltp"]
 
 
 @retry_on_error
 async def get_quotes_async(
     tokens: list, mode: str = "FULL", return_type="dict", session=None
```

### Comparing `volstreet-8.0.1/volstreet/angel_interface/base_websocket.py` & `volstreet-8.1.0/volstreet/angel_interface/base_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/angel_interface/interface.py` & `volstreet-8.1.0/volstreet/angel_interface/interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/angel_interface/login.py` & `volstreet-8.1.0/volstreet/angel_interface/login.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/angel_interface/order_websocket.py` & `volstreet-8.1.0/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/angel_interface/price_websocket.py` & `volstreet-8.1.0/volstreet/angel_interface/price_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/angel_interface/smart_connect.py` & `volstreet-8.1.0/volstreet/angel_interface/smart_connect.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/backtests/analysis.py` & `volstreet-8.1.0/volstreet/backtests/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/backtests/data_updation.py` & `volstreet-8.1.0/volstreet/backtests/data_updation.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,36 +51,53 @@
     with open(file_path, "wb") as file:
         pickle.dump(new_market_days, file)
         logger.info(
             f"Updated market days. New number of market days: {len(new_market_days)}"
         )
 
 
-def update_price_stream_for_index(index: str) -> None:
+def update_price_stream_for_index(
+    index: str, earliest_allowed_date: datetime = None, days_to_expiry: int = 2
+) -> None:
     backtester = BackTester()
     index = UnderlyingInfo(index)
     engine = create_engine(backtester._alchemy_engine_url)
     market_dts = [datetime.combine(day, datetime.min.time()) for day in market_days]
     target_days = [
         day.date()
         for day in market_dts
-        if backtester.historic_time_to_expiry(index.name, day, in_days=True) <= 2
+        if backtester.historic_time_to_expiry(index.name, day, in_days=True)
+        <= days_to_expiry
     ]  # For now only two nearest expiry dates
     latest_date = backtester.execute_query(
         f"""
         SELECT MAX(DATE(timestamp)) FROM price_stream WHERE symboltoken LIKE '{index.name}%'
         """
     )[0][0]
+    filter_date = latest_date or earliest_allowed_date
+    assert (
+        filter_date
+    ), "Atleast one of latest_date or earliest_allowed_date must be provided"
     dates_to_update = [
-        day for day in target_days if day > latest_date
+        day for day in target_days if day > earliest_allowed_date.date()
     ]  # Only update the days which are not already present in the database
+    if not dates_to_update:
+        logger.info(f"No days to update for {index.name}")
+        return
+    logger.info(f"Updating price stream for {index.name} for days: {dates_to_update}")
     for day in dates_to_update:
+        logger.info(f"Updating price stream for {index.name} on {day}")
         df = backtester.get_prices_for_day(
             underlying_info=index,
             day=day,
             num_strikes=50,
         )
         df["timestamp"] = pd.to_datetime(df["timestamp"])
         df = df[["timestamp", "symboltoken", "price"]]
         df["price"] = df["price"].round(3)
         df = df.sort_values(["timestamp", "symboltoken"])
+        logger.info(
+            f"Updating price stream for {index.name} on {day} with len {len(df)}"
+        )
         df.to_sql("price_stream", con=engine, if_exists="append", index=False)
+        logger.info(f"Updated price stream for {index.name} on {day}")
+    logger.info(f"Finished updating price stream for {index.name}")
```

### Comparing `volstreet-8.0.1/volstreet/backtests/database.py` & `volstreet-8.1.0/volstreet/backtests/database.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/backtests/delta_hedging.py` & `volstreet-8.1.0/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/backtests/delta_optimizer.py` & `volstreet-8.1.0/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/backtests/framework.py` & `volstreet-8.1.0/volstreet/backtests/framework.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-8.1.0/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/backtests/proxy_functions.py` & `volstreet-8.1.0/volstreet/backtests/proxy_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,17 +64,15 @@
     if expiry is None and strike is None and option_type is None:
         return name.upper(), name.upper()
     else:
         symbol = f"{name.upper()}{expiry.upper()}{int(strike)}{option_type.upper()}"
         return symbol, symbol
 
 
-def get_expiry_dates(expiry_frequency: int):
-    expiry_frequencies = {v: k for k, v in EXPIRY_FREQUENCIES.items()}
-    underlying = expiry_frequencies[expiry_frequency]
+def get_expiry_dates(underlying: str):
     expiries = fetch_historical_expiry(
         underlying, current_time(), threshold_days=0, n_exp=4
     )
     return expiries
 
 
 def get_base(name, expiry):
```

### Comparing `volstreet-8.0.1/volstreet/backtests/result_processing.py` & `volstreet-8.1.0/volstreet/backtests/result_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/backtests/runner.py` & `volstreet-8.1.0/volstreet/backtests/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,35 +16,34 @@
     def __init__(
         self,
         underlying: UnderlyingInfo,
         start_date: "datetime.date",
         end_date: "datetime.date",
         strategy: Callable,
         parameters: dict,
-        start_time: "datetime.time" = time(9, 16),
         end_directory: str = None,
     ):
         self.underlying = underlying
         self.start_date = start_date
         self.end_date = end_date
         self.strategy = strategy
         self.parameters = parameters
-        self.start_time = start_time
         self.end_directory = end_directory
 
         # Post initialization
         self.price_feed = ProxyPriceFeed
         self.Index = __import__("volstreet.trade_interface").Index
         self.end_directory = self.make_result_directory(end_directory)
 
     def make_result_directory(self, end_directory):
         # Making a directory to store the results
         strategy = self.strategy.__name__
         index_strategy_directory = f"backtester\\{self.underlying.name}_{strategy}\\"
         if end_directory is None:
+            make_directory_if_needed(index_strategy_directory)
             folder_number = len(os.listdir(index_strategy_directory)) + 1
             end_directory = f"test_{folder_number}\\"
 
         end_directory = os.path.join(index_strategy_directory, f"{end_directory}\\")
         make_directory_if_needed(end_directory)
         return end_directory
 
@@ -87,15 +86,15 @@
             for daily_prices in as_completed(daily_prices):
                 try:
                     date = daily_prices.result().timestamp.first().iloc[0].date()
                     self.price_feed._current_group = (
                         daily_prices.result()
                     )  # Updating prices
                     config.backtest_state = datetime.combine(
-                        date, self.start_time
+                        date, time(*start_time)
                     )  # State changes to the next day
                     self.price_feed.update_prices()  # data_bank gets updated
                     updated_index_instance = self.Index(
                         self.underlying.name
                     )  # Index instance gets updated
                     ProxyFeeds.order_feed = []  # Order feed gets reset
                     self.strategy(
```

### Comparing `volstreet-8.0.1/volstreet/backtests/tools.py` & `volstreet-8.1.0/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/backtests/trend.py` & `volstreet-8.1.0/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/backtests/underlying_info.py` & `volstreet-8.1.0/volstreet/backtests/underlying_info.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/blackscholes.py` & `volstreet-8.1.0/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/config.py` & `volstreet-8.1.0/volstreet/config.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/database_connection.py` & `volstreet-8.1.0/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/datamodule/analysis.py` & `volstreet-8.1.0/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/datamodule/archive.py` & `volstreet-8.1.0/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/datamodule/data_handling.py` & `volstreet-8.1.0/volstreet/datamodule/data_handling.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,17 @@
     dates_present = [date[0] for date in dates_present]
 
     new_files = []  # List to keep track of new files
     for attempt in range(3):
         try:
             with FTPConnection(host, username, password) as ftp:
                 zip_files = find_zip_files(ftp, remote_base_directory)
+                zip_files = [
+                    file for file in zip_files if "CONTRACT" not in file
+                ]  # Filter out CONTRACT files
                 dates_of_files = [
                     file.split("_")[4].rstrip(".zip") for file in zip_files
                 ]
                 dates_of_files = [
                     datetime.strptime(date, "%d%m%Y").date() for date in dates_of_files
                 ]
                 for file, date in zip(zip_files, dates_of_files):
```

### Comparing `volstreet-8.0.1/volstreet/datamodule/eod_client.py` & `volstreet-8.1.0/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/datamodule/gambling.py` & `volstreet-8.1.0/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/datamodule/intraday_data.py` & `volstreet-8.1.0/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/datamodule/stockmock.py` & `volstreet-8.1.0/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/datamodule/trading_assistance.py` & `volstreet-8.1.0/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/dealingroom.py` & `volstreet-8.1.0/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/decorators.py` & `volstreet-8.1.0/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/discord_bot.py` & `volstreet-8.1.0/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/exceptions.py` & `volstreet-8.1.0/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/historical_info/__init__.py` & `volstreet-8.1.0/volstreet/historical_info/__init__.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/historical_info/index_expiries.pkl` & `volstreet-8.1.0/volstreet/historical_info/index_expiries.pkl`

 * *Files 1% similar despite different names*

```diff
@@ -730,28 +730,28 @@
 00002d90: 9452 9468 0528 8a08 00b0 c771 145f b817  .R.h.(.....q._..
 00002da0: 4e4e 4b0a 7494 5294 6805 288a 0800 b0a1  NNK.t.R.h.(.....
 00002db0: d98f 36ba 174e 4e4b 0a74 9452 9468 0528  ..6..NNK.t.R.h.(
 00002dc0: 8a08 00b0 cad2 9f5c bc17 4e4e 4b0a 7494  .......\..NNK.t.
 00002dd0: 5294 6805 288a 0800 b0f3 cbaf 82be 174e  R.h.(..........N
 00002de0: 4e4b 0a74 9452 9468 0528 8a08 00b0 1cc5  NK.t.R.h.(......
 00002df0: bfa8 c017 4e4e 4b0a 7494 5294 6805 288a  ....NNK.t.R.h.(.
-00002e00: 0800 b06b 5654 f7c0 174e 4e4b 0a74 9452  ...kVT...NNK.t.R
-00002e10: 9468 0528 8a08 00b0 45be cfce c217 4e4e  .h.(....E.....NN
-00002e20: 4b0a 7494 5294 6805 288a 0800 b06e b7df  K.t.R.h.(....n..
-00002e30: f4c4 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
-00002e40: 00b0 481f 5bcc c617 4e4e 4b0a 7494 5294  ..H.[...NNK.t.R.
-00002e50: 6805 288a 0800 b0c0 a9ff 40c9 174e 4e4b  h.(.......@..NNK
-00002e60: 0a74 9452 9468 0528 8a08 00b0 9a11 7b18  .t.R.h.(......{.
-00002e70: cb17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
-00002e80: b012 9c1f 8dcd 174e 4e4b 0a74 9452 9468  .......NNK.t.R.h
-00002e90: 0528 8a08 00b0 3b95 2fb3 cf17 4e4e 4b0a  .(....;./...NNK.
-00002ea0: 7494 5294 6805 288a 0800 b064 8e3f d9d1  t.R.h.(....d.?..
+00002e00: 0800 b045 becf cec2 174e 4e4b 0a74 9452  ...E.....NNK.t.R
+00002e10: 9468 0528 8a08 00b0 6eb7 dff4 c417 4e4e  .h.(....n.....NN
+00002e20: 4b0a 7494 5294 6805 288a 0800 b048 1f5b  K.t.R.h.(....H.[
+00002e30: ccc6 174e 4e4b 0a74 9452 9468 0528 8a08  ...NNK.t.R.h.(..
+00002e40: 00b0 c0a9 ff40 c917 4e4e 4b0a 7494 5294  .....@..NNK.t.R.
+00002e50: 6805 288a 0800 b09a 117b 18cb 174e 4e4b  h.(......{...NNK
+00002e60: 0a74 9452 9468 0528 8a08 00b0 129c 1f8d  .t.R.h.(........
+00002e70: cd17 4e4e 4b0a 7494 5294 6805 288a 0800  ..NNK.t.R.h.(...
+00002e80: b03b 952f b3cf 174e 4e4b 0a74 9452 9468  .;./...NNK.t.R.h
+00002e90: 0528 8a08 00b0 648e 3fd9 d117 4e4e 4b0a  .(....d.?...NNK.
+00002ea0: 7494 5294 6805 288a 0800 b08d 874f ffd3  t.R.h.(......O..
 00002eb0: 174e 4e4b 0a74 9452 9468 0528 8a08 00b0  .NNK.t.R.h.(....
-00002ec0: 8d87 4fff d317 4e4e 4b0a 7494 5294 6805  ..O...NNK.t.R.h.
-00002ed0: 288a 0800 b031 6c8f 97dc 174e 4e4b 0a74  (....1l....NNK.t
+00002ec0: 316c 8f97 dc17 4e4e 4b0a 7494 5294 6805  1l....NNK.t.R.h.
+00002ed0: 288a 0800 b0fe 49df 55e7 174e 4e4b 0a74  (.....I.U..NNK.t
 00002ee0: 9452 9468 0528 8a08 00b0 4613 5f86 f817  .R.h.(....F._...
 00002ef0: 4e4e 4b0a 7494 5294 6805 288a 0800 b00c  NNK.t.R.h.(.....
 00002f00: 299a 2614 184e 4e4b 0a74 9452 9468 0528  ).&..NNK.t.R.h.(
 00002f10: 8a08 00b0 7061 fe63 3018 4e4e 4b0a 7494  ....pa.c0.NNK.t.
 00002f20: 5294 658c 0846 494e 4e49 4654 5994 5d94  R.e..FINNIFTY.].
 00002f30: 2868 0528 8a08 00b0 accc e822 5a16 4e4e  (h.(......."Z.NN
 00002f40: 4b0a 7494 5294 6805 288a 0800 b0d5 c5f8  K.t.R.h.(.......
```

### Comparing `volstreet-8.0.1/volstreet/historical_info/market_days.pkl` & `volstreet-8.1.0/volstreet/historical_info/market_days.pkl`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 95b5 4100 0000 0000 005d 9428 8c08  ....A......].(..
+00000000: 8004 95cf 4100 0000 0000 005d 9428 8c08  ....A......].(..
 00000010: 6461 7465 7469 6d65 948c 0464 6174 6594  datetime...date.
 00000020: 9394 4304 07e3 0201 9485 9452 9468 0343  ..C........R.h.C
 00000030: 0407 e302 0494 8594 5294 6803 4304 07e3  ........R.h.C...
 00000040: 0205 9485 9452 9468 0343 0407 e302 0694  .....R.h.C......
 00000050: 8594 5294 6803 4304 07e3 0207 9485 9452  ..R.h.C........R
 00000060: 9468 0343 0407 e302 0894 8594 5294 6803  .h.C........R.h.
 00000070: 4304 07e3 020b 9485 9452 9468 0343 0407  C........R.h.C..
@@ -1045,8 +1045,10 @@
 00004140: 07e8 0409 9485 9452 9468 0343 0407 e804  .......R.h.C....
 00004150: 0a94 8594 5294 6803 4304 07e8 040c 9485  ....R.h.C.......
 00004160: 9452 9468 0343 0407 e804 0f94 8594 5294  .R.h.C........R.
 00004170: 6803 4304 07e8 0410 9485 9452 9468 0343  h.C........R.h.C
 00004180: 0407 e804 1294 8594 5294 6803 4304 07e8  ........R.h.C...
 00004190: 0413 9485 9452 9468 0343 0407 e804 1694  .....R.h.C......
 000041a0: 8594 5294 6803 4304 07e8 0417 9485 9452  ..R.h.C........R
-000041b0: 9468 0343 0407 e804 1894 8594 5294 652e  .h.C........R.e.
+000041b0: 9468 0343 0407 e804 1894 8594 5294 6803  .h.C........R.h.
+000041c0: 4304 07e8 0419 9485 9452 9468 0343 0407  C........R.h.C..
+000041d0: e804 1a94 8594 5294 652e                 ......R.e.
```

### Comparing `volstreet-8.0.1/volstreet/models/__init__.py` & `volstreet-8.1.0/volstreet/models/__init__.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/parallelization.py` & `volstreet-8.1.0/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/performance_tracking.py` & `volstreet-8.1.0/volstreet/performance_tracking.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/position_dashboard/app.py` & `volstreet-8.1.0/volstreet/position_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/position_dashboard/formatting.py` & `volstreet-8.1.0/volstreet/position_dashboard/formatting.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/strategies/deployment.py` & `volstreet-8.1.0/volstreet/strategies/deployment.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/strategies/error_handling.py` & `volstreet-8.1.0/volstreet/strategies/error_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/strategies/helpers.py` & `volstreet-8.1.0/volstreet/strategies/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -299,16 +299,16 @@
 
         :param options: List of options to filter.
         :param option_type: Type of the options (CALL or PUT).
         :return: Filtered list of options.
         """
         try:
             otm_strikes = self.underlying.get_otm_strikes(
-                [opt.strike for opt in options], option_type
-            )
+                [opt.strike for opt in options], option_type, cut_off_pct=3
+            )  # Very important to filter out absurd strikes to avoid expensive API calls
             filtered_options = filter_out_illiquid_options(
                 [opt for opt in options if opt.strike in otm_strikes],
                 timedelta_minutes=3,
             )
         except Exception as e:
             logger.error(
                 f"Error while filtering out illiquid options for {self.underlying.name} "
@@ -462,15 +462,18 @@
         if filter_func:
             return np.array([*filter(filter_func, gammas)])
         else:
             return np.array(gammas)
 
     def potential_greeks(self) -> Greeks:
         greeks = np.sum(
-            [(opt.recommended_qty * opt.current_greeks) for opt in self.all_options]
+            [
+                (opt.recommended_qty * opt.current_greeks)
+                for opt in self.recommended_options
+            ]
         )
         return greeks
 
     def aggregate_greeks(self) -> Greeks:
         return np.sum([opt.position_greeks for opt in self.active_options])
 
     def reset_options(self):
@@ -628,137 +631,14 @@
             greeks,
             0.65,
             self.underlying.get_synthetic_future_price(self.expiry),
             is_call,
         )
         return greeks
 
-    # def set_recommendation_for_first_side(
-    #     self,
-    #     options: list[Option],
-    #     is_call: bool,
-    # ) -> tuple[tuple[float, float], tuple[float, float]]:
-    #     greeks = self.prepare_greek_frame_with_options(options, is_call)
-    #
-    #     # Finding the gamma of the option whose delta is closest to 0.1
-    #     idx = np.abs(greeks[:, 2] - 0.1).argmin()
-    #     target_gamma = greeks[idx, 3]
-    #     gamma_floor = dynamic_floor(target_gamma)
-    #     gamma_ceil = dynamic_ceil(target_gamma)
-    #
-    #     for attempt in range(3):
-    #         try:
-    #             weights = optimize_option_weights(
-    #                 greeks[:, 2],
-    #                 greeks[:, 3],
-    #                 0.09,
-    #                 0.6,
-    #                 gamma_floor,
-    #                 gamma_ceil,
-    #             )
-    #             break
-    #         except OptimizationError as e:
-    #             if attempt == 2:
-    #                 raise e
-    #             gamma_floor *= 0.95
-    #             gamma_ceil *= 1.05
-    #         except Exception as e:
-    #             logger.error(
-    #                 f"Error in optimization: {e}, Traceback: {traceback.format_exc()}"
-    #             )
-    #             raise e
-    #
-    #     # noinspection PyUnboundLocalVariable
-    #     for option, weight in zip(greeks[:, -1], weights):
-    #         option.recommended_qty = round_shares_to_lot_size(
-    #             weight * self.base_exposure_qty, option.lot_size
-    #         )
-    #
-    #     # Return the weighted delta which will be used to configure the other side
-    #     calibrated_delta = np.dot(weights, greeks[:, 2])
-    #     target_deltas = (abs(calibrated_delta) - 0.01, abs(calibrated_delta) + 0.01)
-    #     target_gammas = (gamma_floor, gamma_ceil)
-    #     return target_deltas, target_gammas
-    #
-    # def set_recommendation_for_second_side(
-    #     self,
-    #     options: list[Option],
-    #     is_call: bool,
-    #     target_deltas: tuple[float, float],
-    #     target_gammas: tuple[float, float],
-    # ) -> None:
-    #     greeks = self.prepare_greek_frame_with_options(options, is_call)
-    #
-    #     for attempt in range(3):
-    #         try:
-    #             # This will try with multiple gamma scalers within itself,
-    #             # if all fails, it will raise an OptimizationError
-    #             weights = optimize_option_weights(
-    #                 greeks[:, 2], greeks[:, 3], *target_deltas, *target_gammas
-    #             )
-    #             break
-    #         except OptimizationError:
-    #             if attempt == 2:
-    #                 raise OptimizationError("Second side optimization failed")
-    #             elif attempt == 1:
-    #                 target_gammas = (-10000, 10000)  # Use the entire range
-    #             else:
-    #                 target_gammas = (target_gammas[0] * 0.75, target_gammas[1] * 1.25)
-    #         except Exception as e:
-    #             logger.error(
-    #                 f"Error in optimization: {e}, Traceback: {traceback.format_exc()}"
-    #             )
-    #             raise OptimizationError("Second side optimization failed")
-    #
-    #     # noinspection PyUnboundLocalVariable
-    #     for option, weight in zip(greeks[:, -1], weights):
-    #         option.recommended_qty = round_shares_to_lot_size(
-    #             weight * self.base_exposure_qty, option.lot_size
-    #         )
-    #
-    # def set_optimized_recommended_qty(self) -> None:
-    #     self.reset_options()
-    #     try:
-    #         target_deltas, target_gammas = self.set_recommendation_for_first_side(
-    #             self.prospective_calls, is_call=True
-    #         )
-    #         self.set_recommendation_for_second_side(
-    #             self.prospective_puts,
-    #             is_call=False,
-    #             target_deltas=target_deltas,
-    #             target_gammas=target_gammas,
-    #         )
-    #     except Exception as e:
-    #         if "Second side optimization failed" in str(e):
-    #             notifier(
-    #                 f"Second side optimization failed for {self.underlying.name}. "
-    #                 f"Trying to calibrate again in reverse order.",
-    #                 self.notifier_url,
-    #                 "ERROR",
-    #             )
-    #             self.reset_options()  # CRUCIAL TO RESET THE OPTIONS
-    #
-    #             # Reverse the order of calibration
-    #             target_deltas, target_gammas = self.set_recommendation_for_first_side(
-    #                 self.prospective_puts, is_call=False
-    #             )
-    #             self.set_recommendation_for_second_side(
-    #                 self.prospective_calls,
-    #                 is_call=True,
-    #                 target_deltas=target_deltas,
-    #                 target_gammas=target_gammas,
-    #             )
-    #         else:
-    #             notifier(
-    #                 f"Optimization failed for {self.underlying.name}.",
-    #                 self.notifier_url,
-    #                 "ERROR",
-    #             )
-    #             raise e
-
     def set_recommended_qty_backup(
         self, target_delta: float = None, attempt_no: int = 0
     ):
         self.reset_options()
 
         if target_delta > 0.7 or attempt_no > 5:
             raise ValueError(
@@ -935,14 +815,21 @@
 
         date = current_time().strftime("%Y-%m-%d")
         if directory is None:
             file_path = f"{ActiveSession.obj.userId}\\{self.underlying.name}_delta_data\\{date}.json"
         else:
             file_path = os.path.join(directory, f"{date}.json")
 
+        total_premium_outstanding = sum(
+            [option.premium_outstanding for option in self.active_options]
+        )
+        total_premium_received = sum(
+            [option.premium_received for option in self.all_options]
+        )
+
         position_status = {
             "timestamp": current_time(),
             "underlying": self.underlying.name,
             "underlying_price": self.underlying.fetch_ltp(),
             "expiry": self.expiry,
             "base_exposure_qty": self.base_exposure_qty,
             "active_call_options": [
@@ -964,21 +851,17 @@
                     "premium_received": option.premium_received,
                     "current_ltp": option.current_ltp,
                     "current_greeks": option.current_greeks.as_dict(),
                 }
                 for option in self.active_put_options
             ],
             "aggregate_greeks": self.aggregate_greeks().as_dict(),
-            "total_premium_received": sum(
-                [option.premium_received for option in self.all_options]
-            ),
-            "total_premium_outstanding": sum(
-                [option.premium_outstanding for option in self.active_options]
-            ),
-            "mtm": sum([option.mtm for option in self.all_options]),
+            "total_premium_received": total_premium_received,
+            "total_premium_outstanding": total_premium_outstanding,
+            "mtm": total_premium_outstanding - total_premium_received,
             "exit_triggers": self.exit_triggers,
         }
 
         load_combine_save_json_data(position_status, file_path, default_structure=list)
 
 
 def generate_optimized_result(
```

### Comparing `volstreet-8.0.1/volstreet/strategies/monitoring.py` & `volstreet-8.1.0/volstreet/strategies/monitoring.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/strategies/optimization.py` & `volstreet-8.1.0/volstreet/strategies/optimization.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/strategies/strats.py` & `volstreet-8.1.0/volstreet/strategies/strats.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from volstreet.config import logger
 from volstreet.utils.core import (
     current_time,
     find_strike,
     time_to_expiry,
     check_for_weekend,
     calculate_ema,
-    strike_range_different,
     convert_exposure_to_lots,
 )
 from volstreet.utils.communication import notifier, log_error
 from volstreet.utils.data_io import save_json_data
 from volstreet.exceptions import IntrinsicValueError
 from volstreet.blackscholes import simulate_price, calculate_strangle_iv
 from volstreet.angel_interface.interface import (
@@ -293,21 +292,20 @@
 
 
 @exit_on_error
 @increase_robustness
 def delta_hedged_strangle(
     underlying: Index | Stock,
     exposure: int | float,
-    tracking_strikes: int,
+    delta_threshold_pct: float = 0.04,
     target_delta: float = 0.1,
-    optimized: bool = False,
+    optimized: bool = True,
     optimize_gamma: bool = False,
     theta_time_jump_hours: float = 1,  # In hours
     delta_interval_minutes: int | float = 1,
-    delta_threshold_pct: float = 0.04,
     hedge_margin: float | None = None,  # eg 0.2
     exit_time: Optional[tuple] = (15, 29),
     use_cache: Optional[bool] = True,
     at_market: bool = False,
     notification_url: Optional[str] = None,
     strategy_tag: Optional[str] = "Delta hedged strangle",
     data_directory: Optional[str] = None,
@@ -365,24 +363,16 @@
     delta_position: DeltaPosition = DeltaPosition(
         underlying=underlying,
         base_exposure_qty=base_qty_shares,
         greek_settings={"theta_time_jump": theta_time_jump_hours / (365 * 24)},
         order_tag=strategy_tag,
         notifier_url=notification_url,
     )
+    delta_position.update_prospective_options(25, use_cache)
     while current_time().time() < time(*exit_time):
-        if delta_position.cached_strikes is None or strike_range_different(
-            underlying.get_active_strikes(tracking_strikes),
-            delta_position.cached_strikes,
-        ):
-            delta_position.update_prospective_options(tracking_strikes, use_cache)
-            logger.info(
-                f"{current_time()} {underlying.name} set active options and set "
-                f"{len(delta_position.all_options)} prospective options"
-            )
         delta_position.update_underlying()
         delta_position.set_recommended_qty(target_delta, optimized, optimize_gamma)
         delta_position.adjust_recommended_qty()
         delta_position.enter_positions(at_market=at_market)
         delta_position.reset_trigger_flags()
 
         def interruption_condition():
@@ -1868,36 +1858,65 @@
     notification_url: Optional[str] = None,
     strategy_tag: Optional[str] = "Quick Strangle",
 ):
 
     if not exposure and not investment:
         raise ValueError("Exposure or investment must be provided")
 
+    DISPARITY_THRESHOLD = 0.2
+
     # Entering the main function
     if time(*scan_exit_time) < current_time().time():
         notifier(
             f"{underlying.name} {strategy_tag} not being deployed after exit time",
             notification_url,
             "INFO",
         )
         return
 
+    def fetch_spot_and_basis(underlying: Index, expiry: str) -> tuple[float, float]:
+        spot_price = underlying.fetch_ltp()
+        current_basis = underlying.get_basis_for_expiry(
+            expiry=expiry, underlying_price=spot
+        )
+        return spot_price, current_basis
+
+    def get_strangle_with_prices(
+        underlying: Index, offset: float, expiry: str
+    ) -> Strangle:
+        strike = find_strike(spot + offset, underlying.base)
+        strangle: Strangle = Strangle(strike, strike, underlying.name, expiry)
+        prices = strangle.fetch_ltp(for_type=action.value)
+        return strangle
+
+    def calculate_ivs(strangle, spot_price, r, prices):
+        ivs = strangle.fetch_ivs(spot=spot_price, r=r, prices=prices)
+        return np.mean(ivs)
+
+    def disparity_check(call_ltp, put_ltp):
+        disparity = abs(call_ltp - put_ltp) / min(call_ltp, put_ltp)
+        return disparity < DISPARITY_THRESHOLD
+
+    last_log_time = current_time()
+
+    def log_iv_status():
+        nonlocal ivs, last_log_time
+        if current_time() - last_log_time > timedelta(seconds=0.1):
+            logger.info(f"{underlying.name} {strategy_tag} IVs: {ivs}")
+            last_log_time = current_time()
+
     def condition_triggered() -> bool | tuple[Strangle, float, float]:
         nonlocal ivs, action, iv_threshold, strategy_tag, position
         if action == Action.BUY:
             strangle = min(ivs, key=ivs.get)
         else:
             strangle = max(ivs, key=ivs.get)
         iv = ivs[strangle]
         # noinspection PyTypeChecker
         total_price = np.sum(strangle.fetch_ltp(for_type=action.value))
-        logger.info(
-            f"{underlying.name} {strategy_tag} IV is {iv} for {strangle} "
-            f"with total price {total_price}"
-        )
         condition = iv <= iv_threshold if action == Action.BUY else iv >= iv_threshold
 
         if condition:
             position.position_active = True
             position.instrument = strangle
             position.initiating_price = total_price
             return True
@@ -1925,35 +1944,36 @@
 
     if stop_loss is None:
         stop_loss = np.nan
 
     position = PositionMonitor(underlying)
 
     while current_time().time() < time(*scan_exit_time):
-        spot = underlying.fetch_ltp()
-        basis = underlying.get_basis_for_expiry(expiry=expiry, underlying_price=spot)
-        above_strike = find_strike(spot + underlying.base, underlying.base)
-        below_strike = find_strike(spot - underlying.base, underlying.base)
-        above_strangle = Strangle(above_strike, above_strike, underlying.name, expiry)
-        below_strangle = Strangle(below_strike, below_strike, underlying.name, expiry)
-        above_strangle_prices = above_strangle.fetch_ltp(for_type=action.value)
-        below_strangle_price = below_strangle.fetch_ltp(for_type=action.value)
-
-        ivs = {
-            above_strangle: np.mean(
-                above_strangle.fetch_ivs(
-                    spot=spot, r=basis, prices=above_strangle_prices
-                )
-            ),
-            below_strangle: np.mean(
-                below_strangle.fetch_ivs(
-                    spot=spot, r=basis, prices=below_strangle_price
-                )
-            ),
-        }
+        spot, basis = fetch_spot_and_basis(underlying, expiry)
+        above_strangle, above_prices = get_strangle_with_prices(
+            underlying, underlying.base, expiry
+        )
+        below_strangle, below_prices = get_strangle_with_prices(
+            underlying, -underlying.base, expiry
+        )
+        ivs = {}
+        if disparity_check(*above_prices):
+            ivs[above_strangle] = calculate_ivs(
+                above_strangle, spot, basis, above_prices
+            )
+        if disparity_check(*below_prices):
+            ivs[below_strangle] = calculate_ivs(
+                below_strangle, spot, basis, below_prices
+            )
+
+        if not ivs:
+            sleep(0.1)
+            continue
+
+        log_iv_status()
 
         if condition_triggered():
             if exposure != 0:
                 quantity_in_lots = convert_exposure_to_lots(
                     exposure, underlying.fetch_ltp(), underlying.lot_size
                 )
             elif investment != 0:
@@ -2345,7 +2365,155 @@
         "trend",
         start_time=start_time,
         underlying=underlying,
         notification_url=notification_url,
         additional_info=f"Profit pct: {combined_pnl_pct:0.2f}",
     )
     underlying.strategy_log[strategy_tag].extend(entries_log)
+
+
+def reentry_straddle(
+    underlying: Index | Stock,
+    exposure: int | float,
+    exit_time: tuple[int, int] = (15, 29),
+    stop_loss: Optional[float] = 0.5,
+    at_market: bool = False,
+    notification_url: Optional[str] = None,
+    strategy_tag: Optional[str] = "Reentry_straddle",
+    data_directory: Optional[str] = None,
+):
+
+    def exit_option(option: Option, quantity_in_lots: int):
+        instructions = {
+            option: {
+                "action": Action.BUY,
+                "quantity_in_lots": quantity_in_lots,
+                "order_tag": strategy_tag,
+            }
+        }
+        execution_details = execute_instructions(instructions, at_market=at_market)
+        option_exit_price = execution_details[option]
+        return option_exit_price
+
+    def reenter_option(option: Option, quantity_in_lots: int):
+        instructions = {
+            option: {
+                "action": Action.SELL,
+                "quantity_in_lots": quantity_in_lots,
+                "order_tag": strategy_tag,
+            }
+        }
+        execution_details = execute_instructions(instructions, at_market=at_market)
+        option_entry_price = execution_details[option]
+        return option_entry_price
+
+    if time(*exit_time) < current_time().time():
+        notifier(
+            f"{underlying.name} {strategy_tag} not being deployed after exit time",
+            notification_url,
+            "INFO",
+        )
+        return
+
+    spot_price = underlying.fetch_ltp()
+    atm_strike = find_strike(spot_price, underlying.base)
+    expiry = underlying.current_expiry
+    quantity_in_lots = convert_exposure_to_lots(
+        exposure, spot_price, underlying.lot_size
+    )
+
+    straddle = Straddle(atm_strike, underlying.name, expiry)
+
+    # Placing the main order
+    execution_details = execute_instructions(
+        {
+            straddle: {
+                "action": Action.SELL,
+                "quantity_in_lots": quantity_in_lots,
+                "order_tag": strategy_tag,
+            }
+        }
+    )
+    call_avg_price, put_avg_price = execution_details[straddle]
+    total_avg_price = call_avg_price + put_avg_price
+    call_sl_price = call_avg_price * (1 + stop_loss)
+    put_sl_price = put_avg_price * (1 + stop_loss)
+
+    neutral = True
+    call_sl_hit = False
+    put_sl_hit = False
+    trend_sl_hit = False
+
+    reattempt_bank = {straddle.call_option: 1, straddle.put_option: 1}
+
+    while current_time().time() < time(*exit_time):
+        sleep_until_next_action(1, exit_time)
+        if neutral:
+            call_ltp, put_ltp = straddle.fetch_ltp()
+            call_sl_hit = call_ltp > call_sl_price
+            put_sl_hit = put_ltp > put_sl_price
+            if call_sl_hit and put_sl_hit:
+                raise ValueError("Both stop losses hit for some reason")
+            elif call_sl_hit or put_sl_hit:
+                option_to_exit = (
+                    straddle.call_option if call_sl_hit else straddle.put_option
+                )
+                option_exit_price = exit_option(option_to_exit, quantity_in_lots)
+                neutral = False
+
+        else:
+            # Re-entry is the first type of condition that can change the position now
+            reentry_option, reentry_check_price = (
+                (straddle.call_option, call_avg_price)
+                if call_sl_hit
+                else (straddle.put_option, put_avg_price)
+            )
+            reentry_condition = (
+                reentry_option.fetch_ltp() < reentry_check_price
+            ) and reattempt_bank[reentry_option] > 0
+
+            if reentry_condition:
+                option_entry_price = reenter_option(reentry_option, quantity_in_lots)
+                reattempt_bank[reentry_option] -= 1
+                neutral = True
+
+            # Second type of condition is trend condition
+            trend_option, trend_sl_price = (
+                (straddle.put_option, put_sl_price)
+                if call_sl_hit
+                else (straddle.call_option, call_sl_price)
+            )
+            trend_sl_hit = trend_option.fetch_ltp() > trend_sl_price
+
+            if trend_sl_hit:
+                exit_option(trend_option, quantity_in_lots)
+                # The below condition basically means that the trend option has switched
+                # Happens in the rare case that there is a significant movement
+                # in the opposite direction of the trend
+                if reentry_condition:
+                    # We have already reentered the reentry option
+                    # And exited the trend option
+                    # We just need to change the flags
+                    call_sl_hit, put_sl_hit = put_sl_hit, call_sl_hit
+                    neutral = False
+                    continue
+                break
+
+    # Exit open positions if any
+    if neutral:
+        # Exit the strangle
+        execution_details = execute_instructions(
+            {
+                straddle: {
+                    "action": Action.BUY,
+                    "quantity_in_lots": quantity_in_lots,
+                    "order_tag": strategy_tag,
+                }
+            }
+        )
+        call_exit_price, put_exit_price = execution_details[straddle]
+        total_exit_price = call_exit_price + put_exit_price
+        pnl = total_avg_price - total_exit_price
+    elif not neutral and not trend_sl_hit:
+        option_exit_price = exit_option(trend_option, quantity_in_lots)
+    else:
+        pass
```

### Comparing `volstreet-8.0.1/volstreet/trade_interface/instruments.py` & `volstreet-8.1.0/volstreet/trade_interface/instruments.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/trade_interface/order_execution.py` & `volstreet-8.1.0/volstreet/trade_interface/order_execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     update_order_params,
     lookup_and_return,
     fetch_quotes,
     fetch_book,
 )
 from volstreet.angel_interface.async_interface import (
     get_quotes_async,
+    get_ltp_async,
     place_order_async,
     modify_order_async,
     unique_order_status_async,
 )
 from volstreet.trade_interface.instruments import (
     Option,
     Strangle,
@@ -127,15 +128,16 @@
     while open_orders:
         if iteration == 3:
             notifier(
                 f"Max modification iterations reached for symbol {symbol}.",
                 config.ERROR_NOTIFICATION_SETTINGS["url"],
                 "ERROR",
             )
-            break  # todo: Can we add get_ltp_async here to return the ltp as the avg price? think about it
+            token = orders[0]["symboltoken"]  # All orders have the same symbol token
+            return await get_ltp_async(token, session)
         additional_buffer = iteration / 100
         quotes = await get_quotes_async(
             [order["symboltoken"] for order in open_orders], session=session
         )
         await modify_open_orders(open_orders, quotes, additional_buffer, session)
         await asyncio.sleep(0.25)
         statuses = await fetch_statuses(order_ids, session)
```

### Comparing `volstreet-8.0.1/volstreet/trade_interface/underlyings.py` & `volstreet-8.1.0/volstreet/trade_interface/underlyings.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             logger.error(
                 f"Symbol dataframe is empty. Using hardcoded freeze qty for {self.name}"
             )
             freeze_qty_in_lots = 100 if self.name == "SENSEX" else 30  # Hardcoded
             return int(freeze_qty_in_lots)
 
     def fetch_exps(self):
-        exps = get_expiry_dates(config.EXPIRY_FREQUENCIES.get(self.name, "monthly"))
+        exps = get_expiry_dates(self.name)
         exps = pd.DatetimeIndex(exps).strftime("%d%b%y").str.upper().tolist()
 
         self.current_expiry = exps[0]
         self.next_expiry = exps[1]
         self.far_expiry = exps[2]
 
         if self.name in config.EXPIRY_FREQUENCIES:
@@ -325,27 +325,38 @@
             current_strike + (self.base * range_of_strikes),
             self.base,
         )
         strike_range = [*map(int, strike_range)]
         return strike_range
 
     def get_otm_strikes(
-        self, strike_range: Iterable[int], option_type: OptionType
+        self,
+        strike_range: Iterable[int],
+        option_type: OptionType,
+        cut_off_pct: float = 3,
     ) -> list[int]:
         """Filters out itm strikes and returns tradeable strikes. Itm is defined as strike which is
         more than 4 bases away from the ltp. Direction of itm is determined by option_type
-        HARDCODED 4 BASES"""
+        HARDCODED 4 BASES
+        Cut off percentage is the percentage of strikes to be considered from the ATM strike.
+        Default is 3%. Strikes beyond this percentage are filtered out.
+        """
         ltp = self.fetch_ltp()
+        cut_off_price = (
+            ltp * (1 + cut_off_pct / 100)
+            if option_type == OptionType.CALL
+            else ltp * (1 - cut_off_pct / 100)
+        )
         return [
             strike
             for strike in strike_range
             if option_type == OptionType.CALL
-            and strike > (ltp - 4 * self.base)
+            and ((ltp - 4 * self.base) < strike < cut_off_price)
             or option_type == OptionType.PUT
-            and strike < (ltp + 4 * self.base)
+            and ((ltp + 4 * self.base) > strike > cut_off_price)
         ]
 
     def get_range_of_strangles(
         self, c_strike, p_strike, strike_range, exp=None
     ) -> list[Strangle | Straddle]:
         """Gets a range of strangles around the given strikes. If c_strike == p_strike, returns a range of straddles"""
```

### Comparing `volstreet-8.0.1/volstreet/utils/change_config.py` & `volstreet-8.1.0/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/utils/communication.py` & `volstreet-8.1.0/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/utils/core.py` & `volstreet-8.1.0/volstreet/utils/core.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/utils/data_io.py` & `volstreet-8.1.0/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/utils/scrip_processing.py` & `volstreet-8.1.0/volstreet/utils/scrip_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dateutil import rrule
 from datetime import datetime, timedelta
 from itertools import groupby
 import numpy as np
 import pandas as pd
 from functools import lru_cache
+from volstreet import config
 from volstreet.config import holidays, scrips, logger, implemented_indices
 from volstreet.utils.core import current_time
 from volstreet.exceptions import ScripsLocationError
 
 
 @lru_cache(maxsize=1280)
 def get_symbol_token(
@@ -96,15 +97,18 @@
         symbol, token = filtered_scrips[["symbol", "token"]].values[0]
     else:
         raise ValueError("Invalid arguments")
 
     return symbol, token
 
 
-def get_expiry_dates(expiry_frequency: int):
+def get_expiry_dates(underlying: str):
+    expiry_frequency = config.EXPIRY_FREQUENCIES.get(
+        underlying, "monthly"
+    )  # Get the weekday
     if expiry_frequency == "monthly":
         monthly_expiry_dates = generate_potential_expiry_dates(
             rule=rrule.MONTHLY, weekday=rrule.TH(-1)
         )
         monthly_expiry_dates = [
             shift_for_holidays_and_weekends(date) for date in monthly_expiry_dates
         ]
```

### Comparing `volstreet-8.0.1/volstreet/vectorized_blackscholes.py` & `volstreet-8.1.0/volstreet/vectorized_blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/vslogging/formatters.py` & `volstreet-8.1.0/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/vslogging/logging_config.json` & `volstreet-8.1.0/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/vslogging/logging_setup.py` & `volstreet-8.1.0/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet/vslogging/parsing.py` & `volstreet-8.1.0/volstreet/vslogging/parsing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.0.1/volstreet.egg-info/PKG-INFO` & `volstreet-8.1.0/volstreet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 8.0.1
+Version: 8.1.0
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-8.0.1/volstreet.egg-info/SOURCES.txt` & `volstreet-8.1.0/volstreet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

