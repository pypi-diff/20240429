# Comparing `tmp/tradedangerous-11.1.1.tar.gz` & `tmp/tradedangerous-11.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradedangerous-11.1.1.tar", last modified: Sun Apr 28 21:44:13 2024, max compression
+gzip compressed data, was "tradedangerous-11.1.2.tar", last modified: Mon Apr 29 19:11:58 2024, max compression
```

## Comparing `tradedangerous-11.1.1.tar` & `tradedangerous-11.1.2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:44:13.608173 tradedangerous-11.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-28 21:44:13.608173 tradedangerous-11.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-28 21:44:13.608173 tradedangerous-11.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:44:13.592173 tradedangerous-11.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tests/test_bootstrap_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tests/test_bootstrap_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tests/test_peek.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tests/test_trade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tests/test_trade_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/trade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:44:13.596174 tradedangerous-11.1.1/tradedangerous/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36080 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:44:13.600174 tradedangerous-11.1.1/tradedangerous/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/TEMPLATE.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/buildcache_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/buy_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/commandenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/export_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/import_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/local_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/market_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/nav_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/olddata_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/rares_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/sell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/shipvendor_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/station_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/trade_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/update_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/commands/update_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/csvexport.py
--rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/edscupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/edsmupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/jsonprices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:44:13.600174 tradedangerous-11.1.1/tradedangerous/mfd/
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/mfd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:44:13.604174 tradedangerous-11.1.1/tradedangerous/mfd/saitek/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/mfd/saitek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/mfd/saitek/directoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/mfd/saitek/x52pro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:44:13.604174 tradedangerous-11.1.1/tradedangerous/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/misc/checkpricebounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/misc/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/misc/coord64.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/misc/derp-sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/misc/diff-system-csvs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/misc/eddb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/misc/eddn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/misc/edsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/misc/edsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/misc/importeddbstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/misc/prices-json-exp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/misc/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:44:13.604174 tradedangerous-11.1.1/tradedangerous/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/plugins/edapi_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/plugins/edcd_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    21525 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/plugins/eddblink_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/plugins/edmc_batch_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/plugins/journal_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/plugins/netlog_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    27048 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/plugins/spansh_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/prices.py
--rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/submit-distances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:44:13.608173 tradedangerous-11.1.1/tradedangerous/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/templates/Added.csv
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/templates/Category.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/templates/RareItem.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/templates/TradeDangerous.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/tradecalc.py
--rw-r--r--   0 runner    (1001) docker     (127)    72220 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/tradedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/tradeenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/tradeexcept.py
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradedangerous/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-28 21:43:24.000000 tradedangerous-11.1.1/tradedangerous/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:44:13.608173 tradedangerous-11.1.1/tradedangerous.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-28 21:44:13.000000 tradedangerous-11.1.1/tradedangerous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-28 21:44:13.000000 tradedangerous-11.1.1/tradedangerous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 21:44:13.000000 tradedangerous-11.1.1/tradedangerous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-28 21:44:13.000000 tradedangerous-11.1.1/tradedangerous.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 21:44:13.000000 tradedangerous-11.1.1/tradedangerous.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-28 21:44:13.000000 tradedangerous-11.1.1/tradedangerous.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-28 21:44:13.000000 tradedangerous-11.1.1/tradedangerous.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-28 21:43:05.000000 tradedangerous-11.1.1/tradegui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.520146 tradedangerous-11.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-29 19:11:58.520146 tradedangerous-11.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-29 19:11:58.520146 tradedangerous-11.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.508146 tradedangerous-11.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_bootstrap_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_bootstrap_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_peek.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_trade_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/trade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.512146 tradedangerous-11.1.2/tradedangerous/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36080 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.516146 tradedangerous-11.1.2/tradedangerous/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/TEMPLATE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/buildcache_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/buy_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/commandenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/export_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/import_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/local_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/market_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/nav_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/olddata_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/rares_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/sell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/shipvendor_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/station_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/trade_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/update_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/commands/update_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/csvexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/edscupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/edsmupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/jsonprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.516146 tradedangerous-11.1.2/tradedangerous/mfd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/mfd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.516146 tradedangerous-11.1.2/tradedangerous/mfd/saitek/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/mfd/saitek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/mfd/saitek/directoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/mfd/saitek/x52pro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.520146 tradedangerous-11.1.2/tradedangerous/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/checkpricebounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/coord64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/derp-sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/diff-system-csvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/eddb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/eddn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/edsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/edsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/importeddbstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/prices-json-exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/misc/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.520146 tradedangerous-11.1.2/tradedangerous/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/edapi_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/edcd_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22484 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/eddblink_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/edmc_batch_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/journal_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/netlog_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27048 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/plugins/spansh_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/submit-distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.520146 tradedangerous-11.1.2/tradedangerous/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/templates/Added.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/templates/Category.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/templates/RareItem.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/templates/TradeDangerous.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/tradecalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72220 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/tradedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/tradeenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/tradeexcept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradedangerous/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-29 19:11:08.000000 tradedangerous-11.1.2/tradedangerous/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:11:58.520146 tradedangerous-11.1.2/tradedangerous.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-29 19:11:58.000000 tradedangerous-11.1.2/tradedangerous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-29 19:11:58.000000 tradedangerous-11.1.2/tradedangerous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:11:58.000000 tradedangerous-11.1.2/tradedangerous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 19:11:58.000000 tradedangerous-11.1.2/tradedangerous.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:11:58.000000 tradedangerous-11.1.2/tradedangerous.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 19:11:58.000000 tradedangerous-11.1.2/tradedangerous.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 19:11:58.000000 tradedangerous-11.1.2/tradedangerous.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-29 19:10:49.000000 tradedangerous-11.1.2/tradegui.py
```

### Comparing `tradedangerous-11.1.1/LICENSE` & `tradedangerous-11.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/PKG-INFO` & `tradedangerous-11.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.1.1
+Version: 11.1.2
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.1.1/README.md` & `tradedangerous-11.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/setup.py` & `tradedangerous-11.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tests/test_bootstrap_commands.py` & `tradedangerous-11.1.2/tests/test_bootstrap_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tests/test_bootstrap_plugins.py` & `tradedangerous-11.1.2/tests/test_bootstrap_plugins.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tests/test_cache.py` & `tradedangerous-11.1.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tests/test_commands.py` & `tradedangerous-11.1.2/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tests/test_fs.py` & `tradedangerous-11.1.2/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tests/test_peek.py` & `tradedangerous-11.1.2/tests/test_peek.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tests/test_trade.py` & `tradedangerous-11.1.2/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tests/test_trade_run.py` & `tradedangerous-11.1.2/tests/test_trade_run.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tests/test_utils.py` & `tradedangerous-11.1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/trade.py` & `tradedangerous-11.1.2/trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/__init__.py` & `tradedangerous-11.1.2/tradedangerous/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/cache.py` & `tradedangerous-11.1.2/tradedangerous/cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/cli.py` & `tradedangerous-11.1.2/tradedangerous/cli.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/TEMPLATE.py` & `tradedangerous-11.1.2/tradedangerous/commands/TEMPLATE.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/__init__.py` & `tradedangerous-11.1.2/tradedangerous/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/buildcache_cmd.py` & `tradedangerous-11.1.2/tradedangerous/commands/buildcache_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/buy_cmd.py` & `tradedangerous-11.1.2/tradedangerous/commands/buy_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/commandenv.py` & `tradedangerous-11.1.2/tradedangerous/commands/commandenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/exceptions.py` & `tradedangerous-11.1.2/tradedangerous/commands/exceptions.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/export_cmd.py` & `tradedangerous-11.1.2/tradedangerous/commands/export_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/import_cmd.py` & `tradedangerous-11.1.2/tradedangerous/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/local_cmd.py` & `tradedangerous-11.1.2/tradedangerous/commands/local_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/market_cmd.py` & `tradedangerous-11.1.2/tradedangerous/commands/market_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/nav_cmd.py` & `tradedangerous-11.1.2/tradedangerous/commands/nav_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/olddata_cmd.py` & `tradedangerous-11.1.2/tradedangerous/commands/olddata_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/parsing.py` & `tradedangerous-11.1.2/tradedangerous/commands/parsing.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/rares_cmd.py` & `tradedangerous-11.1.2/tradedangerous/commands/rares_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/run_cmd.py` & `tradedangerous-11.1.2/tradedangerous/commands/run_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/sell_cmd.py` & `tradedangerous-11.1.2/tradedangerous/commands/sell_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/shipvendor_cmd.py` & `tradedangerous-11.1.2/tradedangerous/commands/shipvendor_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/station_cmd.py` & `tradedangerous-11.1.2/tradedangerous/commands/station_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/trade_cmd.py` & `tradedangerous-11.1.2/tradedangerous/commands/trade_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/update_cmd.py` & `tradedangerous-11.1.2/tradedangerous/commands/update_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/commands/update_gui.py` & `tradedangerous-11.1.2/tradedangerous/commands/update_gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/corrections.py` & `tradedangerous-11.1.2/tradedangerous/corrections.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/csvexport.py` & `tradedangerous-11.1.2/tradedangerous/csvexport.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/edscupdate.py` & `tradedangerous-11.1.2/tradedangerous/edscupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/edsmupdate.py` & `tradedangerous-11.1.2/tradedangerous/edsmupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/formatting.py` & `tradedangerous-11.1.2/tradedangerous/formatting.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/fs.py` & `tradedangerous-11.1.2/tradedangerous/fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/gui.py` & `tradedangerous-11.1.2/tradedangerous/gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/jsonprices.py` & `tradedangerous-11.1.2/tradedangerous/jsonprices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/mapping.py` & `tradedangerous-11.1.2/tradedangerous/mapping.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/mfd/__init__.py` & `tradedangerous-11.1.2/tradedangerous/mfd/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/mfd/saitek/directoutput.py` & `tradedangerous-11.1.2/tradedangerous/mfd/saitek/directoutput.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/mfd/saitek/x52pro.py` & `tradedangerous-11.1.2/tradedangerous/mfd/saitek/x52pro.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/misc/checkpricebounds.py` & `tradedangerous-11.1.2/tradedangerous/misc/checkpricebounds.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/misc/clipboard.py` & `tradedangerous-11.1.2/tradedangerous/misc/clipboard.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/misc/coord64.py` & `tradedangerous-11.1.2/tradedangerous/misc/coord64.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/misc/derp-sentinel.py` & `tradedangerous-11.1.2/tradedangerous/misc/derp-sentinel.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/misc/diff-system-csvs.py` & `tradedangerous-11.1.2/tradedangerous/misc/diff-system-csvs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/misc/eddb.py` & `tradedangerous-11.1.2/tradedangerous/misc/eddb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/misc/eddn.py` & `tradedangerous-11.1.2/tradedangerous/misc/eddn.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/misc/edsc.py` & `tradedangerous-11.1.2/tradedangerous/misc/edsc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/misc/edsm.py` & `tradedangerous-11.1.2/tradedangerous/misc/edsm.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/misc/importeddbstats.py` & `tradedangerous-11.1.2/tradedangerous/misc/importeddbstats.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/misc/prices-json-exp.py` & `tradedangerous-11.1.2/tradedangerous/misc/prices-json-exp.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/misc/progress.py` & `tradedangerous-11.1.2/tradedangerous/misc/progress.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/plugins/__init__.py` & `tradedangerous-11.1.2/tradedangerous/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/plugins/edapi_plug.py` & `tradedangerous-11.1.2/tradedangerous/plugins/edapi_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/plugins/edcd_plug.py` & `tradedangerous-11.1.2/tradedangerous/plugins/edcd_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/plugins/eddblink_plug.py` & `tradedangerous-11.1.2/tradedangerous/plugins/eddblink_plug.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,49 @@
 import datetime
 import json
 import os
 import sqlite3
 import ssl
 import time
 import typing
+import locale
 
 from urllib import request
 from pathlib import Path
 
 from .. import plugins, cache, transfers
 from ..misc import progress as pbar
 from ..plugins import PluginException
 
 
 if typing.TYPE_CHECKING:
     from typing import Optional
     from .. tradeenv import TradeEnv
 
-
+# Find the first English UTF-8 locale for use in parsing timestamps.
+LOCALE = None
+import platform
+if platform.system() == 'Windows':
+    for lang in locale.windows_locale.values():
+        if "en" in lang:
+            LOCALE = lang
+            break
+else:
+    # for other operating systems
+    for lang in locale.locale_alias.values():
+        if "en" in lang and "UTF-8" in lang:
+            LOCALE = lang
+            break
+if not LOCALE:
+    raise PluginException(
+        "Unable to find compatible locale.\n" +
+        "This plugin needs an English, UTF-8 compatible " +
+        "locale installed in order to function correctly.\n" + 
+        "Please refer to your OS for instructions installing one."
+    )
 # Constants
 BASE_URL = os.environ.get('TD_SERVER') or "https://elite.tromador.com/files/"
 CONTEXT=ssl.create_default_context(cafile=certifi.where())
 
 
 def _request_url(url, headers=None):
     data = None
@@ -155,15 +176,14 @@
     def now(self):
         return datetime.datetime.now()
     
     def downloadFile(self, path):
         """
         Fetch the latest dumpfile from the website if newer than local copy.
         """
-        
         def openURL(url):
             return _request_url(url, headers = {'User-Agent': 'Trade-Dangerous'})
         
         if path not in (self.liveListingsPath, self.listingsPath):
             localPath = Path(self.tdb.dataPath, path)
         else:
             localPath = Path(self.dataPath, path)
@@ -174,15 +194,17 @@
         try:
             response = openURL(url)
         except Exception as e:  # pylint: disable=broad-exception-caught
             self.tdenv.WARN("Problem with download:\n    URL: {}\n    Error: {}", BASE_URL + str(path), str(e))
             return False
         
         url_time = response.getheader("Last-Modified")
+        locale.setlocale(locale.LC_ALL, LOCALE)
         dumpModded = datetime.datetime.strptime(url_time, "%a, %d %b %Y %H:%M:%S %Z").timestamp()
+        locale.setlocale(locale.LC_ALL, '')
         
         if Path.exists(localPath):
             localModded = localPath.stat().st_mtime
             if localModded >= dumpModded:
                 self.tdenv.DEBUG0("'{}': Dump is not more recent than Local.", path)
                 return False
         
@@ -327,14 +349,16 @@
         self.tdenv.NOTE("Optimizing database...")
         db.execute("VACUUM")
         self.tdb.close()
         
         self.tdenv.NOTE("Finished processing market data. End time = {}", self.now())
     
     def run(self):
+        self.tdenv.DEBUG2(f'Using "{LOCALE}" locale for parsing modified timestamps. Please include this information in any error reports.')
+        
         # Create the /eddb folder for downloading the source files if it doesn't exist.
         try:
             Path(str(self.dataPath)).mkdir()
         except FileExistsError:
             pass
         
         # Run 'listings' by default:
```

### Comparing `tradedangerous-11.1.1/tradedangerous/plugins/edmc_batch_plug.py` & `tradedangerous-11.1.2/tradedangerous/plugins/edmc_batch_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/plugins/journal_plug.py` & `tradedangerous-11.1.2/tradedangerous/plugins/journal_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/plugins/netlog_plug.py` & `tradedangerous-11.1.2/tradedangerous/plugins/netlog_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/plugins/spansh_plug.py` & `tradedangerous-11.1.2/tradedangerous/plugins/spansh_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/prices.py` & `tradedangerous-11.1.2/tradedangerous/prices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/submit-distances.py` & `tradedangerous-11.1.2/tradedangerous/submit-distances.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/templates/Added.csv` & `tradedangerous-11.1.2/tradedangerous/templates/Added.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/templates/RareItem.csv` & `tradedangerous-11.1.2/tradedangerous/templates/RareItem.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/templates/TradeDangerous.sql` & `tradedangerous-11.1.2/tradedangerous/templates/TradeDangerous.sql`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/tools.py` & `tradedangerous-11.1.2/tradedangerous/tools.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/tradecalc.py` & `tradedangerous-11.1.2/tradedangerous/tradecalc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/tradedb.py` & `tradedangerous-11.1.2/tradedangerous/tradedb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/tradeenv.py` & `tradedangerous-11.1.2/tradedangerous/tradeenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/transfers.py` & `tradedangerous-11.1.2/tradedangerous/transfers.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/utils.py` & `tradedangerous-11.1.2/tradedangerous/utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradedangerous/version.py` & `tradedangerous-11.1.2/tradedangerous/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 # this software so long as you include this copyright notice.
 # I guarantee there is at least one bug neither of us knew about.
 # --------------------------------------------------------------------
 
 """just keeper of current version"""
 
 # TODO: remember to update tests when version changes
-__version__ = '11.1.1'
+__version__ = '11.1.2'
```

### Comparing `tradedangerous-11.1.1/tradedangerous.egg-info/PKG-INFO` & `tradedangerous-11.1.2/tradedangerous.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.1.1
+Version: 11.1.2
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.1.1/tradedangerous.egg-info/SOURCES.txt` & `tradedangerous-11.1.2/tradedangerous.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.1.1/tradegui.py` & `tradedangerous-11.1.2/tradegui.py`

 * *Files identical despite different names*

