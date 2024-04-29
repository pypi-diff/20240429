# Comparing `tmp/asyncio_payok-0.0.4.tar.gz` & `tmp/asyncio_payok-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncio_payok-0.0.4.tar", last modified: Tue Apr 16 12:13:08 2024, max compression
+gzip compressed data, was "asyncio_payok-1.0.0.tar", last modified: Mon Apr 29 15:43:11 2024, max compression
```

## Comparing `asyncio_payok-0.0.4.tar` & `asyncio_payok-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 12:13:08.813252 asyncio_payok-0.0.4/
--rw-rw-rw-   0        0        0     2250 2024-04-16 12:13:08.811254 asyncio_payok-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1920 2024-04-16 10:22:24.000000 asyncio_payok-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 12:13:08.754908 asyncio_payok-0.0.4/asyncio_payok/
--rw-rw-rw-   0        0        0       24 2024-04-09 06:26:31.000000 asyncio_payok-0.0.4/asyncio_payok/__init__.py
--rw-rw-rw-   0        0        0     5821 2024-04-16 12:11:56.000000 asyncio_payok-0.0.4/asyncio_payok/api.py
-drwxrwxrwx   0        0        0        0 2024-04-16 12:13:08.808251 asyncio_payok-0.0.4/asyncio_payok/const/
--rw-rw-rw-   0        0        0       40 2024-04-09 06:25:25.000000 asyncio_payok-0.0.4/asyncio_payok/const/__init__.py
--rw-rw-rw-   0        0        0      356 2024-04-08 11:04:10.000000 asyncio_payok-0.0.4/asyncio_payok/const/en.py
--rw-rw-rw-   0        0        0     1228 2024-04-09 06:25:25.000000 asyncio_payok-0.0.4/asyncio_payok/const/models.py
--rw-rw-rw-   0        0        0     1550 2024-04-15 12:48:38.000000 asyncio_payok-0.0.4/asyncio_payok/payok_base.py
-drwxrwxrwx   0        0        0        0 2024-04-16 12:13:08.810255 asyncio_payok-0.0.4/asyncio_payok.egg-info/
--rw-rw-rw-   0        0        0     2250 2024-04-16 12:13:08.000000 asyncio_payok-0.0.4/asyncio_payok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2024-04-16 12:13:08.000000 asyncio_payok-0.0.4/asyncio_payok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 12:13:08.000000 asyncio_payok-0.0.4/asyncio_payok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-16 12:13:08.000000 asyncio_payok-0.0.4/asyncio_payok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-16 12:13:08.000000 asyncio_payok-0.0.4/asyncio_payok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 12:13:08.813252 asyncio_payok-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      469 2024-04-16 12:13:06.000000 asyncio_payok-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:43:11.890672 asyncio_payok-1.0.0/
+-rw-rw-rw-   0        0        0     2250 2024-04-29 15:43:11.889673 asyncio_payok-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1920 2024-04-16 10:22:24.000000 asyncio_payok-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 15:43:11.829676 asyncio_payok-1.0.0/any_utils/
+-rw-rw-rw-   0        0        0       28 2024-04-27 15:09:09.000000 asyncio_payok-1.0.0/any_utils/__init__.py
+-rw-rw-rw-   0        0        0      335 2024-04-27 15:10:13.000000 asyncio_payok-1.0.0/any_utils/metrics.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:43:11.836670 asyncio_payok-1.0.0/asyncio_payok/
+-rw-rw-rw-   0        0        0       45 2024-04-29 15:01:28.000000 asyncio_payok-1.0.0/asyncio_payok/__init__.py
+-rw-rw-rw-   0        0        0     3916 2024-04-29 15:01:28.000000 asyncio_payok-1.0.0/asyncio_payok/api.py
+-rw-rw-rw-   0        0        0     1907 2024-04-27 15:32:01.000000 asyncio_payok-1.0.0/asyncio_payok/base.py
+-rw-rw-rw-   0        0        0     3353 2024-04-29 12:26:29.000000 asyncio_payok-1.0.0/asyncio_payok/concrete.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:43:11.886673 asyncio_payok-1.0.0/asyncio_payok/const/
+-rw-rw-rw-   0        0        0       99 2024-04-29 12:25:05.000000 asyncio_payok-1.0.0/asyncio_payok/const/__init__.py
+-rw-rw-rw-   0        0        0      357 2024-04-24 18:49:44.000000 asyncio_payok-1.0.0/asyncio_payok/const/enums.py
+-rw-rw-rw-   0        0        0      126 2024-04-26 14:46:04.000000 asyncio_payok-1.0.0/asyncio_payok/const/ex.py
+-rw-rw-rw-   0        0        0     1506 2024-04-27 15:30:38.000000 asyncio_payok-1.0.0/asyncio_payok/const/models.py
+-rw-rw-rw-   0        0        0     3781 2024-04-29 12:27:25.000000 asyncio_payok-1.0.0/asyncio_payok/operations.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:43:11.887671 asyncio_payok-1.0.0/asyncio_payok.egg-info/
+-rw-rw-rw-   0        0        0     2250 2024-04-29 15:43:11.000000 asyncio_payok-1.0.0/asyncio_payok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2024-04-29 15:43:11.000000 asyncio_payok-1.0.0/asyncio_payok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 15:43:11.000000 asyncio_payok-1.0.0/asyncio_payok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-29 15:43:11.000000 asyncio_payok-1.0.0/asyncio_payok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-29 15:43:11.000000 asyncio_payok-1.0.0/asyncio_payok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 15:43:11.891673 asyncio_payok-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      469 2024-04-29 15:01:28.000000 asyncio_payok-1.0.0/setup.py
```

### Comparing `asyncio_payok-0.0.4/PKG-INFO` & `asyncio_payok-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncio_payok
-Version: 0.0.4
+Version: 1.0.0
 Summary: Asyncio client for PayOk API
 Home-page: https://github.com/slimeless/asycncio-payok
 Author: Abracadabra
 Author-email: stopcrybby@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
```

### Comparing `asyncio_payok-0.0.4/README.md` & `asyncio_payok-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `asyncio_payok-0.0.4/asyncio_payok.egg-info/PKG-INFO` & `asyncio_payok-1.0.0/asyncio_payok.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncio_payok
-Version: 0.0.4
+Version: 1.0.0
 Summary: Asyncio client for PayOk API
 Home-page: https://github.com/slimeless/asycncio-payok
 Author: Abracadabra
 Author-email: stopcrybby@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
```

