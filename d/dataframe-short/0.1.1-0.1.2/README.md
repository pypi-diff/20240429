# Comparing `tmp/dataframe_short-0.1.1.tar.gz` & `tmp/dataframe_short-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataframe_short-0.1.1.tar", last modified: Mon Apr 29 02:47:22 2024, max compression
+gzip compressed data, was "dataframe_short-0.1.2.tar", last modified: Mon Apr 29 03:37:57 2024, max compression
```

## Comparing `dataframe_short-0.1.1.tar` & `dataframe_short-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 02:47:22.191701 dataframe_short-0.1.1/
--rw-rw-rw-   0        0        0      304 2024-04-29 02:47:22.191701 dataframe_short-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 02:47:22.191701 dataframe_short-0.1.1/dataframe_short/
--rw-rw-rw-   0        0        0      119 2024-04-18 01:36:13.000000 dataframe_short-0.1.1/dataframe_short/__init__.py
--rw-rw-rw-   0        0        0     7711 2024-03-17 03:24:34.000000 dataframe_short-0.1.1/dataframe_short/dataframe_test.py
--rw-rw-rw-   0        0        0     2803 2024-03-11 03:40:50.000000 dataframe_short-0.1.1/dataframe_short/func_24_Feb.py
--rw-rw-rw-   0        0        0    49641 2024-04-29 01:56:48.000000 dataframe_short-0.1.1/dataframe_short/lib02_dataframe.py
-drwxrwxrwx   0        0        0        0 2024-04-29 02:47:22.191701 dataframe_short-0.1.1/dataframe_short.egg-info/
--rw-rw-rw-   0        0        0      304 2024-04-29 02:47:22.000000 dataframe_short-0.1.1/dataframe_short.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-29 02:47:22.000000 dataframe_short-0.1.1/dataframe_short.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 02:47:22.000000 dataframe_short-0.1.1/dataframe_short.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-29 02:47:22.000000 dataframe_short-0.1.1/dataframe_short.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 02:47:22.191701 dataframe_short-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      359 2024-04-29 02:43:11.000000 dataframe_short-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:37:57.877388 dataframe_short-0.1.2/
+-rw-rw-rw-   0        0        0      255 2024-04-29 03:37:57.876391 dataframe_short-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 03:37:57.863426 dataframe_short-0.1.2/dataframe_short/
+-rw-rw-rw-   0        0        0      119 2024-04-29 03:35:00.000000 dataframe_short-0.1.2/dataframe_short/__init__.py
+-rw-rw-rw-   0        0        0     7711 2024-03-17 03:24:34.000000 dataframe_short-0.1.2/dataframe_short/dataframe_test.py
+-rw-rw-rw-   0        0        0     2803 2024-03-11 03:40:50.000000 dataframe_short-0.1.2/dataframe_short/func_24_Feb.py
+-rw-rw-rw-   0        0        0    49641 2024-04-29 01:56:48.000000 dataframe_short-0.1.2/dataframe_short/lib02_dataframe.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:37:57.874396 dataframe_short-0.1.2/dataframe_short.egg-info/
+-rw-rw-rw-   0        0        0      255 2024-04-29 03:37:57.000000 dataframe_short-0.1.2/dataframe_short.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-29 03:37:57.000000 dataframe_short-0.1.2/dataframe_short.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 03:37:57.000000 dataframe_short-0.1.2/dataframe_short.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-29 03:37:57.000000 dataframe_short-0.1.2/dataframe_short.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 03:37:57.877388 dataframe_short-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      362 2024-04-29 03:34:55.000000 dataframe_short-0.1.2/setup.py
```

### Comparing `dataframe_short-0.1.1/dataframe_short/dataframe_test.py` & `dataframe_short-0.1.2/dataframe_short/dataframe_test.py`

 * *Files identical despite different names*

### Comparing `dataframe_short-0.1.1/dataframe_short/func_24_Feb.py` & `dataframe_short-0.1.2/dataframe_short/func_24_Feb.py`

 * *Files identical despite different names*

### Comparing `dataframe_short-0.1.1/dataframe_short/lib02_dataframe.py` & `dataframe_short-0.1.2/dataframe_short/lib02_dataframe.py`

 * *Files identical despite different names*

