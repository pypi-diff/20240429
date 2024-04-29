# Comparing `tmp/pkscreener-0.44.20240428.303.tar.gz` & `tmp/pkscreener-0.44.20240428.304.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240428.303.tar", last modified: Sun Apr 28 20:21:34 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240428.304.tar", last modified: Sun Apr 28 23:39:43 2024, max compression
```

## Comparing `pkscreener-0.44.20240428.303.tar` & `pkscreener-0.44.20240428.304.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 20:21:34.245054 pkscreener-0.44.20240428.303/
--rw-rw-rw-   0        0        0     1086 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-28 20:21:34.245054 pkscreener-0.44.20240428.303/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 20:21:34.229432 pkscreener-0.44.20240428.303/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:21:34.245054 pkscreener-0.44.20240428.303/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25815 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7288 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29409 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    20421 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8124 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   116109 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    51424 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    81788 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-28 20:21:25.000000 pkscreener-0.44.20240428.303/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   123016 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47924 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    25522 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:21:34.229432 pkscreener-0.44.20240428.303/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-28 20:21:34.000000 pkscreener-0.44.20240428.303/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-28 20:21:34.000000 pkscreener-0.44.20240428.303/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 20:21:34.000000 pkscreener-0.44.20240428.303/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-04-28 20:21:34.000000 pkscreener-0.44.20240428.303/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-28 20:21:34.000000 pkscreener-0.44.20240428.303/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-28 20:21:34.000000 pkscreener-0.44.20240428.303/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-28 20:21:34.245054 pkscreener-0.44.20240428.303/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-04-28 20:15:37.000000 pkscreener-0.44.20240428.303/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 23:39:43.446266 pkscreener-0.44.20240428.304/
+-rw-rw-rw-   0        0        0     1086 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-28 23:39:43.446266 pkscreener-0.44.20240428.304/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 23:39:43.430648 pkscreener-0.44.20240428.304/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 23:39:43.446266 pkscreener-0.44.20240428.304/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25815 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7288 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29455 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    20421 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8124 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   116796 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    51535 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    81792 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-28 23:39:35.000000 pkscreener-0.44.20240428.304/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   123016 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    41457 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    25522 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-28 23:39:43.430648 pkscreener-0.44.20240428.304/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-28 23:39:43.000000 pkscreener-0.44.20240428.304/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-28 23:39:43.000000 pkscreener-0.44.20240428.304/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 23:39:43.000000 pkscreener-0.44.20240428.304/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-04-28 23:39:43.000000 pkscreener-0.44.20240428.304/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-28 23:39:43.000000 pkscreener-0.44.20240428.304/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-28 23:39:43.000000 pkscreener-0.44.20240428.304/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-28 23:39:43.446266 pkscreener-0.44.20240428.304/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-04-28 23:36:13.000000 pkscreener-0.44.20240428.304/setup.py
```

### Comparing `pkscreener-0.44.20240428.303/LICENSE` & `pkscreener-0.44.20240428.304/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/LICENSE-Others` & `pkscreener-0.44.20240428.304/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/PKG-INFO` & `pkscreener-0.44.20240428.304/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240428.303
+Version: 0.44.20240428.304
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240428.303.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240428.304.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240425.293/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.303/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240425.293/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.303/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240425.293/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.303/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240428.303/README.md` & `pkscreener-0.44.20240428.304/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240425.293/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.303/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240425.293/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.303/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240425.293/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.303/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240428.303/pkscreener/__init__.py` & `pkscreener-0.44.20240428.304/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/MenuOptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     "21": "MF/FIIs Popular Stocks         ",
     "22": "View Stock Performance         ",
     "23": "Breaking out now               ",
     "24": "Higher Highs,Lows & Close (SuperTrend)",
     "25": "Lower Highs,Lows (Sell/Watch for Rev.)",
     "26": "Stocks with stock-split/bonus/dividends",
     "27": "ATR Cross                      ",
+    "28": "Higher Opens                   ",
     # "27": "Intraday Momentum Build-up      ",
     # "28": "Extremely bullish daily close      ",
     # "29": "Rising RSI                      ",
     # "30": "RSI entering bullish territory",
     "42": "Show Last Screened Results",
     "M": "Back to the Top/Main menu",
     "Z": "Exit (Ctrl + C)",
```

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/ScreeningStatistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,14 +477,33 @@
         recent = data.tail(1)
         cond1 = recent["RSI12"].iloc[0] > 55
         cond2 = cond1 and (macd.iloc[:1][0] > 0)
         cond3 = cond2 and (recent["Close"].iloc[0] > recent["EMA10"].iloc[0])
         cond4 = cond3 and (recent["Close"].iloc[0] > recent["EMA200"].iloc[0])
         return cond4
     
+    # Find stocks that opened higher than the previous high
+    def findHigherOpens(self, df):
+        if df is None or len(df) == 0:
+            return False
+        data = df.copy()
+        data = data.fillna(0)
+        data = data.replace([np.inf, -np.inf], 0)
+        recent = data.head(2)
+        return recent["Open"].iloc[0] > recent["Close"].iloc[1]
+
+    def findHigherBullishOpens(self, df):
+        if df is None or len(df) == 0:
+            return False
+        data = df.copy()
+        data = data.fillna(0)
+        data = data.replace([np.inf, -np.inf], 0)
+        recent = data.head(2)
+        return recent["Open"].iloc[0] > recent["High"].iloc[1]
+    
     def findNR4Day(self, df):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         # https://chartink.com/screener/nr4-daily-today
         if data.tail(1)["Volume"].iloc[0] <= 50000:
             return False
```

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/StockScreener.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,15 +471,15 @@
                                                                   or (isBuyingTrendline))
                                                                   or (respChartPattern == 6 and hasBbandsSqz)
                                                                   or (respChartPattern == 7 and isCandlePattern))
                         or (executeOption == 8 and isValidCci)
                         or (executeOption == 9 and hasMinVolumeRatio)
                         or (executeOption == 10 and isPriceRisingByAtLeast2Percent)
                         or (executeOption == 11 and isShortTermBullish)
-                        or (executeOption in [12,13,14,15,16,17,18,19,20,23,24,25,27] and isValidityCheckMet)
+                        or (executeOption in [12,13,14,15,16,17,18,19,20,23,24,25,27,28] and isValidityCheckMet)
                         or (executeOption == 21 and (mfiStake > 0 and reversalOption in [3,5]))
                         or (executeOption == 21 and (mfiStake < 0 and reversalOption in [6,7]))
                         or (executeOption == 21 and (fairValueDiff > 0 and reversalOption in [8]))
                         or (executeOption == 21 and (fairValueDiff < 0 and reversalOption in [9]))
                         or (executeOption == 26)
                     ):
                         isNotMonitoringDashboard = userArgs.monitor is None
@@ -605,15 +605,15 @@
                     )
                     + colorText.END
                 )
         return None
 
     def performValidityCheckForExecuteOptions(self,executeOption,screener,fullData,screeningDictionary,saveDictionary,processedData):
         isValid = True
-        if executeOption not in [11,12,13,14,15,16,17,18,19,20,23,24,25,27]:
+        if executeOption not in [11,12,13,14,15,16,17,18,19,20,23,24,25,27,28]:
             return True
         if executeOption == 11:
             isValid = screener.validateShortTermBullish(
                 fullData, screeningDictionary, saveDictionary
             )
         elif executeOption == 12:
             isValid = (
@@ -643,14 +643,16 @@
             isValid = (
                 screener.validateHigherHighsHigherLowsHigherClose(fullData)
             )
         elif executeOption == 25:
             isValid = screener.validateLowerHighsLowerLows(processedData)
         elif executeOption == 27:
             isValid = screener.findATRCross(processedData)
+        elif executeOption == 28:
+            isValid = screener.findHigherBullishOpens(processedData)
         
         return isValid        
                     
     def performBasicVolumeChecks(self, executeOption, volumeRatio, screeningDictionary, saveDictionary, processedData, configManager, screener):
         minVolume = configManager.minVolume / (
                     100 if configManager.isIntradayConfig() else 1
                 )
```

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
         prefix = ""
         for style in otherStyles:
             cleanedUpStyledValue = cleanedUpStyledValue.replace(style, "")
         # Find how many different colors are used for the cell value
         coloredStyledValues = cleanedUpStyledValue.split(colorText.END)
         for cleanedUpStyledValue in coloredStyledValues:
             cleanedUpStyledValue = cleanedUpStyledValue.replace(colorText.END,"")
-            if cleanedUpStyledValue.strip() in ["", ","]:
+            if cleanedUpStyledValue.strip() in ["", ",","/"]:
                 if len(cleanedUpStyledValues) > 0:
                     cleanedUpStyledValues[len(cleanedUpStyledValues)-1] = f"{cleanedUpStyledValues[len(cleanedUpStyledValues)-1]}{cleanedUpStyledValue}"
                 else:
                     prefix = cleanedUpStyledValue
             else:
                 for style in mainStyles:
                     if style in cleanedUpStyledValue:
```

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/classes/keys.py` & `pkscreener-0.44.20240428.304/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/courbd.ttf` & `pkscreener-0.44.20240428.304/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/globals.py` & `pkscreener-0.44.20240428.304/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1039,19 +1039,19 @@
             df = df[
                 df["Stock"].astype(str).str.contains("BSE:") == False
             ]
             listStockCodes.extend(list(df["Stock"]))
     if executeOption == 42:
         Utility.tools.getLastScreenedResults(defaultAnswer)
         return None, None
-    if executeOption >= 28 and executeOption <= 41:
+    if executeOption >= 29 and executeOption <= 41:
         OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
-            + "\n[+] Error: Option 28 to 41 Not implemented yet! Press <Enter> to continue."
+            + "\n[+] Error: Option 29 to 41 Not implemented yet! Press <Enter> to continue."
             + colorText.END
         )
         input("Press <Enter> to continue...")
         return None, None
     if (
         not str(indexOption).isnumeric() and indexOption in ["W", "E", "M", "N", "Z"]
     ) or (
@@ -2541,16 +2541,16 @@
         skip=["N", "E"],
     )
     indexOption, executeOption = initPostLevel1Execution(
         indexOption=indexOption,
         executeOption=executeOption,
         skip=[
             "0",
-            "28",
             "29",
+            "30",
             "42",
         ],
     )
     return indexOption, executeOption, backtestPeriod
 
 def toggleUserConfig():
     configManager.toggleConfig(
```

### Comparing `pkscreener-0.44.20240428.303/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240428.304/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240428.304/pkscreener/pkscreenerbot.py`

 * *Files 13% similar despite different names*

```diff
@@ -95,14 +95,28 @@
 ONE, TWO, THREE, FOUR = range(4)
 
 m0 = menus()
 m1 = menus()
 m2 = menus()
 m3 = menus()
 
+TOP_LEVEL_SCANNER_MENUS = ["X", "B"]
+TOP_LEVEL_SCANNER_SKIP_MENUS = ["S", "T", "E", "U", "Z", "C", "G"]
+INDEX_SKIP_MENUS = ["W","E","M","Z","0","2","3","4","6","7","9","10","13"]
+SCANNER_SKIP_MENUS_1_TO_7 = ["0","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
+SCANNER_SKIP_MENUS_8_TO_13 = ["0","1","2","3","4","5","6","7","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
+SCANNER_SKIP_MENUS_14_TO_19 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
+SCANNER_SKIP_MENUS_20_TO_27 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","22","28","29","30","42","M","Z"]
+SCANNER_MENUS_WITH_NO_SUBMENUS = ["1","2","3","10","11","12","13","14","15","16","17","18","19","20","21","23","24","25","26","27"]
+SCANNER_MENUS_WITH_SUBMENU_SUPPORT = ["6", "7", "21"]
+
+INDEX_COMMANDS_SKIP_MENUS_SCANNER = ["W", "E", "M", "Z"]
+INDEX_COMMANDS_SKIP_MENUS_BACKTEST = ["W", "E", "M", "Z", "N", "0", "15"]
+UNSUPPORTED_COMMAND_MENUS =["22","28","29","30","42","M","Z"]
+SUPPORTED_COMMAND_MENUS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27"]
 
 async def start(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Send message on `/start`."""
     if update is None or update.message is None:
         return
     # Get user that sent /start and log his name
     user = update.message.from_user
@@ -110,26 +124,26 @@
     # Build InlineKeyboard where each button has a displayed text
     # and a string as callback_data
     # The keyboard is a list of button rows, where each row is in turn
     # a list (hence `[[...]]`).
     mns = m0.renderForMenu(asList=True)
     inlineMenus = []
     for mnu in mns:
-        if mnu.menuKey in ["X", "B", "G"]:
+        if mnu.menuKey in TOP_LEVEL_SCANNER_MENUS:
             inlineMenus.append(
                 InlineKeyboardButton(
                     mnu.menuText.split("(")[0],
                     callback_data="C" + str(mnu.menuKey),
                 )
             )
     keyboard = [inlineMenus]
     reply_markup = InlineKeyboardMarkup(keyboard)
     cmds = m0.renderForMenu(
         selectedMenu=None,
-        skip=["S", "T", "E", "U", "Z", "C", "G"],
+        skip=TOP_LEVEL_SCANNER_SKIP_MENUS,
         asList=True,
         renderStyle=MenuRenderStyle.STANDALONE,
     )
     cmdText = ""
     for cmd in cmds:
         cmdText = f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
     # Send message with text and appended InlineKeyboard
@@ -146,61 +160,32 @@
     return START_ROUTES
 
 
 async def XScanners(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Show new choice of buttons"""
     query = update.callback_query
     data = query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G")
-    if data not in ["X", "B", "G"]:
+    if data not in TOP_LEVEL_SCANNER_MENUS:
         return start(update, context)
     midSkip = "1" if data == "X" else "N"
+    skipMenus = INDEX_SKIP_MENUS.append(midSkip)
     menuText = (
         m1.renderForMenu(
             m0.find(data),
-            skip=[
-                "W",
-                "E",
-                "M",
-                "Z",
-                "0",
-                "2",
-                midSkip,
-                "3",
-                "4",
-                "6",
-                "7",
-                "9",
-                "10",
-                "13",
-            ],
+            skip=skipMenus,
             renderStyle=MenuRenderStyle.STANDALONE,
         )
         .replace("     ", "")
         .replace("    ", "")
         .replace("\t", "")
         .replace(colorText.FAIL,"").replace(colorText.END,"")
     )
     mns = m1.renderForMenu(
         m0.find(data),
-        skip=[
-            "W",
-            "E",
-            "M",
-            "Z",
-            "0",
-            "2",
-            midSkip,
-            "3",
-            "4",
-            "6",
-            "7",
-            "9",
-            "10",
-            "13",
-        ],
+        skip=skipMenus,
         asList=True,
     )
     inlineMenus = []
     await query.answer()
     for mnu in mns:
         inlineMenus.append(
             InlineKeyboardButton(
@@ -221,312 +206,84 @@
     query = update.callback_query
     await query.answer()
     preSelection = (
         query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G")
     )
     selection = preSelection.split("_")
     preSelection = f"{selection[0]}_{selection[1]}"
-    if selection[0].upper() not in ["X", "B", "G"]:
+    if selection[0].upper() not in TOP_LEVEL_SCANNER_MENUS:
         return start(update, context)
     if len(selection) == 2 or (len(selection) == 3 and selection[2] == "P"):
         if str(selection[1]).isnumeric():
             # It's only level 2
             menuText = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=[
-                    "0",
-                    "8",
-                    "9",
-                    "10",
-                    "11",
-                    "12",
-                    "13",
-                    "14",
-                    "15",
-                    "16",
-                    "17",
-                    "18",
-                    "19",
-                    "20",
-                    "21",
-                    "22",
-                    "23",
-                    "24",
-                    "25",
-                    "26",
-                    "27",
-                    "28",
-                    "29",
-                    "30",
-                    "42",
-                    "M",
-                    "Z",
-                ],
+                skip=SCANNER_SKIP_MENUS_1_TO_7,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             menuText = menuText + "\nN > More options"
             mns = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=[
-                    "0",
-                    "8",
-                    "9",
-                    "10",
-                    "11",
-                    "12",
-                    "13",
-                    "14",
-                    "15",
-                    "16",
-                    "17",
-                    "18",
-                    "19",
-                    "20",
-                    "21",
-                    "22",
-                    "23",
-                    "24",
-                    "25",
-                    "26",
-                    "27",
-                    "28",
-                    "29",
-                    "30",
-                    "42",
-                    "M",
-                    "Z",
-                ],
+                skip=SCANNER_SKIP_MENUS_1_TO_7,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             mns.append(menu().create("N", "More Options", 2))
         elif selection[1] == "N":
             selection.extend(["", ""])
     elif len(selection) == 3:
         if selection[2] == "N":
             menuText = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=[
-                    "0",
-                    "1",
-                    "2",
-                    "3",
-                    "4",
-                    "5",
-                    "6",
-                    "7",
-                    "14",
-                    "15",
-                    "16",
-                    "17",
-                    "18",
-                    "19",
-                    "20",
-                    "21",
-                    "22",
-                    "23",
-                    "24",
-                    "25",
-                    "26",
-                    "27",
-                    "28",
-                    "29",
-                    "30",
-                    "42",
-                    "M",
-                    "Z",
-                ],
+                skip=SCANNER_SKIP_MENUS_8_TO_13,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             menuText = menuText + "\nP > Previous Options"
             menuText = menuText + "\nM > More Options"
             mns = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=[
-                    "0",
-                    "1",
-                    "2",
-                    "3",
-                    "4",
-                    "5",
-                    "6",
-                    "7",
-                    "14",
-                    "15",
-                    "16",
-                    "17",
-                    "18",
-                    "19",
-                    "20",
-                    "21",
-                    "22",
-                    "23",
-                    "24",
-                    "25",
-                    "26",
-                    "27",
-                    "28",
-                    "29",
-                    "30",
-                    "42",
-                    "M",
-                    "Z",
-                ],
+                skip=SCANNER_SKIP_MENUS_8_TO_13,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             mns.append(menu().create("P", "Previous Options", 2))
             mns.append(menu().create("M", "More Options", 2))
         elif selection[2] == "M":
             menuText = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=[
-                    "0",
-                    "1",
-                    "2",
-                    "3",
-                    "4",
-                    "5",
-                    "6",
-                    "7",
-                    "8",
-                    "9",
-                    "10",
-                    "11",
-                    "12",
-                    "13",
-                    "20",
-                    "21",
-                    "22",
-                    "23",
-                    "24",
-                    "25",
-                    "26",
-                    "27",
-                    "28",
-                    "29",
-                    "30",
-                    "42",
-                    "M",
-                    "Z",
-                ],
+                skip=SCANNER_SKIP_MENUS_14_TO_19,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             menuText = menuText + "\nP > Previous Options"
             menuText = menuText + "\n>> More Options"
             mns = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=[
-                    "0",
-                    "1",
-                    "2",
-                    "3",
-                    "4",
-                    "5",
-                    "6",
-                    "7",
-                    "8",
-                    "9",
-                    "10",
-                    "11",
-                    "12",
-                    "13",
-                    "20",
-                    "21",
-                    "22",
-                    "23",
-                    "24",
-                    "25",
-                    "26",
-                    "27",
-                    "28",
-                    "29",
-                    "30",
-                    "42",
-                    "M",
-                    "Z",
-                ],
+                skip=SCANNER_SKIP_MENUS_14_TO_19,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             mns.append(menu().create("P", "Previous Options", 2))
             mns.append(menu().create(">>", "More Options", 2))
         elif selection[2] == ">>":
             menuText = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=[
-                    "0",
-                    "1",
-                    "2",
-                    "3",
-                    "4",
-                    "5",
-                    "6",
-                    "7",
-                    "8",
-                    "9",
-                    "10",
-                    "11",
-                    "12",
-                    "13",
-                    "14",
-                    "15",
-                    "16",
-                    "17",
-                    "18",
-                    "19",
-                    "22",
-                    "28",
-                    "29",
-                    "30",
-                    "42",
-                    "M",
-                    "Z",
-                ],
+                skip=SCANNER_SKIP_MENUS_20_TO_27,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             menuText = menuText + "\nP > Previous Options"
             mns = m2.renderForMenu(
                 m1.find(selection[1]),
-                skip=[
-                    "0",
-                    "1",
-                    "2",
-                    "3",
-                    "4",
-                    "5",
-                    "6",
-                    "7",
-                    "8",
-                    "9",
-                    "10",
-                    "11",
-                    "12",
-                    "13",
-                    "14",
-                    "15",
-                    "16",
-                    "17",
-                    "18",
-                    "19",
-                    "22",
-                    "28",
-                    "29",
-                    "30",
-                    "42",
-                    "M",
-                    "Z",
-                ],
+                skip=SCANNER_SKIP_MENUS_20_TO_27,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             mns.append(menu().create("P", "Previous Options", 2))
         elif str(selection[2]).isnumeric():
             preSelection = f"{selection[0]}_{selection[1]}_{selection[2]}"
-            if selection[2] in ["6", "7", "21"]:
+            if selection[2] in SCANNER_MENUS_WITH_SUBMENU_SUPPORT:
                 menuText = m3.renderForMenu(
                     m2.find(selection[2]),
                     renderStyle=MenuRenderStyle.STANDALONE,
                     skip=["0"],
                 )
                 mns = m3.renderForMenu(
                     m2.find(selection[2]),
@@ -539,35 +296,15 @@
                     selection.extend(["D", ""])
                 elif selection[2] == "5":  # RSI range
                     selection.extend(["D", "D"])
                 elif selection[2] == "8":  # CCI range
                     selection.extend(["D", "D"])
                 elif selection[2] == "9":  # Vol gainer ratio
                     selection.extend(["D", ""])
-                elif selection[2] in [
-                    "1",
-                    "2",
-                    "3",
-                    "10",
-                    "11",
-                    "12",
-                    "13",
-                    "14",
-                    "15",
-                    "16",
-                    "17",
-                    "18",
-                    "19",
-                    "20",
-                    "21",
-                    "23",
-                    "24",
-                    "25",
-                    "26","27"
-                ]:  # Vol gainer ratio
+                elif selection[2] in SCANNER_MENUS_WITH_NO_SUBMENUS:  # Vol gainer ratio
                     selection.extend(["", ""])
     elif len(selection) == 4:
         preSelection = (
             query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G")
         )
     optionChoices = ""
     if len(selection) <= 3:
@@ -610,15 +347,15 @@
             menuText=menuText, update=update, context=context, reply_markup=reply_markup
         )
     return START_ROUTES
 
 def default_markup(inlineMenus):
     mns = m0.renderForMenu(asList=True)
     for mnu in mns:
-        if mnu.menuKey in ["X", "B", "G"]:
+        if mnu.menuKey in TOP_LEVEL_SCANNER_MENUS:
             inlineMenus.append(
                     InlineKeyboardButton(
                         mnu.menuText.split("(")[0],
                         callback_data="C" + str(mnu.menuKey),
                     )
                 )
     keyboard = [inlineMenus]
@@ -811,28 +548,26 @@
 
     if cmd == "start":
         await start(update=update, context=context)
         return START_ROUTES
     if cmd == "help":
         await help_command(update=update, context=context)
         return START_ROUTES
-    if cmd in ["x", "b", "g"]:
+    if cmd.upper() in TOP_LEVEL_SCANNER_MENUS:
         await shareUpdateWithChannel(update=update, context=context)
         m0.renderForMenu(
             selectedMenu=None,
-            skip=["S", "T", "E", "U", "Z", "C", "G"],
+            skip=TOP_LEVEL_SCANNER_SKIP_MENUS,
             renderStyle=MenuRenderStyle.STANDALONE,
         )
         selectedMenu = m0.find(cmd.upper())
         cmdText = ""
         cmds = m1.renderForMenu(
             selectedMenu=selectedMenu,
-            skip=(
-                ["W", "E", "M", "Z"] if cmd in ["x"] else ["W", "E", "M", "Z", "N", "0", "15"]
-            ),
+            skip=(INDEX_COMMANDS_SKIP_MENUS_SCANNER  if cmd in ["x"] else INDEX_COMMANDS_SKIP_MENUS_BACKTEST),
             asList=True,
             renderStyle=MenuRenderStyle.STANDALONE,
         )
         for cmd in cmds:
             if cmd in ["N", "0"]:
                 continue
             cmdText = (
@@ -878,24 +613,24 @@
 
     if "x_" in cmd or "b_" in cmd or "g_" in cmd:
         await shareUpdateWithChannel(update=update, context=context)
         selection = cmd.split("_")
         if len(selection) == 2:
             m0.renderForMenu(
                 selectedMenu=None,
-                skip=["S", "T", "E", "U", "Z", "C", "G"],
+                skip=TOP_LEVEL_SCANNER_SKIP_MENUS,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             selectedMenu = m0.find(selection[0].upper())
             m1.renderForMenu(
                 selectedMenu=selectedMenu,
                 skip=(
-                    ["W", "E", "M", "Z"]
+                    INDEX_COMMANDS_SKIP_MENUS_SCANNER
                     if "x_" in cmd
-                    else ["W", "E", "M", "Z", "N", "0"]
+                    else INDEX_COMMANDS_SKIP_MENUS_BACKTEST
                 ),
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             selectedMenu = m1.find(selection[1].upper())
             if "x_" in cmd and selectedMenu.menuKey == "N":  # Nifty prediction
                 options = ":".join(selection)
@@ -913,67 +648,50 @@
             ):  # a specific stock by name
                 cmdText = "For option 0 <Screen stocks by the stock name>, please type in the command in the following format\n/X_0 SBIN or /X_0_0 SBIN and hit send where SBIN is the NSE stock code.For multiple stocks, you can type in /X_0 SBIN,ICICIBANK,OtherStocks. You can put in any number of stocks separated by space or comma(,)."
                 """Send a message when the command /help is issued."""
                 await update.message.reply_text(f"Choose an option:\n{cmdText}")
                 return START_ROUTES
             cmds = m2.renderForMenu(
                 selectedMenu=selectedMenu,
-                skip=[
-                    "22",
-                    "27",
-                    "28",
-                    "29",
-                    "30",
-                    "42",
-                    "M",
-                    "Z",
-                ],
+                skip=UNSUPPORTED_COMMAND_MENUS,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             cmdText = ""
             for cmd in cmds:
                 cmdText = (
                     f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
                 )
             await update.message.reply_text(f"Choose an option:\n{cmdText}")
             return START_ROUTES
         elif len(selection) == 3:
             m0.renderForMenu(
                 selectedMenu=None,
-                skip=["S", "T", "E", "U", "Z", "C", "G"],
+                skip=TOP_LEVEL_SCANNER_SKIP_MENUS,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             selectedMenu = m0.find(selection[0].upper())
             m1.renderForMenu(
                 selectedMenu=selectedMenu,
                 skip=(
-                    ["W", "E", "M", "Z"]
+                    INDEX_COMMANDS_SKIP_MENUS_SCANNER
                     if "x_" in cmd
-                    else ["W", "E", "M", "Z", "N", "0"]
+                    else INDEX_COMMANDS_SKIP_MENUS_BACKTEST
                 ),
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             selectedMenu = m1.find(selection[1].upper())
             m2.renderForMenu(
                 selectedMenu=selectedMenu,
-                skip=[
-                    "22",
-                    "28",
-                    "29",
-                    "30",
-                    "42",
-                    "M",
-                    "Z",
-                ],
+                skip=UNSUPPORTED_COMMAND_MENUS,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
-            if selection[2] in ["6", "7", "21"]:
+            if selection[2] in SCANNER_MENUS_WITH_SUBMENU_SUPPORT:
                 selectedMenu = m2.find(selection[2].upper())
                 cmds = m3.renderForMenu(
                     selectedMenu=selectedMenu,
                     asList=True,
                     renderStyle=MenuRenderStyle.STANDALONE,
                     skip=["0"],
                 )
@@ -987,34 +705,15 @@
                     selection.extend(["D", ""])
                 elif selection[2] == "5":  # RSI range
                     selection.extend(["D", "D"])
                 elif selection[2] == "8":  # CCI range
                     selection.extend(["D", "D"])
                 elif selection[2] == "9":  # Vol gainer ratio
                     selection.extend(["D", ""])
-                elif selection[2] in [
-                    "1",
-                    "2",
-                    "3",
-                    "10",
-                    "11",
-                    "12",
-                    "13",
-                    "14",
-                    "15",
-                    "16",
-                    "17",
-                    "18",
-                    "19",
-                    "20",
-                    "21",
-                    "22",
-                    "23",
-                    "24",
-                ]:  # Vol gainer ratio
+                elif selection[2] in SUPPORTED_COMMAND_MENUS:
                     selection.extend(["", ""])
         if len(selection) >= 4:
             options = ":".join(selection)
             await launchScreener(
                 options=options,
                 user=update.message.from_user,
                 context=context,
@@ -1061,15 +760,15 @@
 
 async def help_command(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
     if _shouldAvoidResponse(update):
         return
 
     cmds = m0.renderForMenu(
         selectedMenu=None,
-        skip=["S", "T", "E", "U", "Z", "C", "G"],
+        skip=TOP_LEVEL_SCANNER_SKIP_MENUS,
         asList=True,
         renderStyle=MenuRenderStyle.STANDALONE,
     )
     cmdText = ""
     for cmd in cmds:
         cmdText = f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
     """Send a message when the command /help is issued."""
@@ -1115,26 +814,26 @@
         return True
     return False
 
 
 def addCommandsForMenuItems(application):
     cmds0 = m0.renderForMenu(
         selectedMenu=None,
-        skip=["S", "T", "E", "U", "Z", "C", "G"],
+        skip=TOP_LEVEL_SCANNER_SKIP_MENUS,
         asList=True,
         renderStyle=MenuRenderStyle.STANDALONE,
     )
     for mnu0 in cmds0:
         p0 = mnu0.menuKey.upper()
         application.add_handler(CommandHandler(p0, command_handler))
         selectedMenu = m0.find(p0)
         cmds1 = m1.renderForMenu(
             selectedMenu=selectedMenu,
             skip=(
-                ["W", "E", "M", "Z"] if p0 == "X" else ["W", "E", "M", "Z", "N", "0"]
+                INDEX_COMMANDS_SKIP_MENUS_SCANNER if p0 == "X" else INDEX_COMMANDS_SKIP_MENUS_BACKTEST
             ),
             asList=True,
             renderStyle=MenuRenderStyle.STANDALONE,
         )
         for mnu1 in cmds1:
             p1 = mnu1.menuKey.upper()
             if p1 in ["N", "0"]:
@@ -1143,32 +842,24 @@
                         CommandHandler(f"{p0}_{p1}", command_handler)
                     )
                 continue
             application.add_handler(CommandHandler(f"{p0}_{p1}", command_handler))
             selectedMenu = m1.find(p1)
             cmds2 = m2.renderForMenu(
                 selectedMenu=selectedMenu,
-                skip=[
-                    "22",
-                    "28",
-                    "29",
-                    "30",
-                    "42",
-                    "M",
-                    "Z",
-                ],
+                skip=UNSUPPORTED_COMMAND_MENUS,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             for mnu2 in cmds2:
                 p2 = mnu2.menuKey.upper()
                 application.add_handler(
                     CommandHandler(f"{p0}_{p1}_{p2}", command_handler)
                 )
-                if p2 in ["6", "7", "21"]:
+                if p2 in SCANNER_MENUS_WITH_SUBMENU_SUPPORT:
                     selectedMenu = m2.find(p2)
                     cmds3 = m3.renderForMenu(
                         selectedMenu=selectedMenu,
                         asList=True,
                         renderStyle=MenuRenderStyle.STANDALONE,
                         skip=["0"],
                     )
```

### Comparing `pkscreener-0.44.20240428.303/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240428.304/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240428.304/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240428.303
+Version: 0.44.20240428.304
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240428.303.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240428.304.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240425.293/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.303/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240425.293/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.303/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240425.293/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240428.303/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240428.303/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240428.304/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240428.303/setup.py` & `pkscreener-0.44.20240428.304/setup.py`

 * *Files identical despite different names*

