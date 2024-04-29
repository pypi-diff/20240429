# Comparing `tmp/syncgrid-3.8.tar.gz` & `tmp/syncgrid-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncgrid-3.8.tar", last modified: Mon Apr 29 20:29:46 2024, max compression
+gzip compressed data, was "syncgrid-3.9.tar", last modified: Mon Apr 29 20:36:24 2024, max compression
```

## Comparing `syncgrid-3.8.tar` & `syncgrid-3.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 20:29:46.292021 syncgrid-3.8/
--rw-rw-rw-   0        0        0      139 2024-04-29 20:29:46.291020 syncgrid-3.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-29 20:29:46.293352 syncgrid-3.8/setup.cfg
--rw-rw-rw-   0        0        0      246 2024-04-29 15:40:15.000000 syncgrid-3.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 20:29:46.271546 syncgrid-3.8/syncgrid/
--rw-rw-rw-   0        0        0      607 2024-04-29 20:28:04.000000 syncgrid-3.8/syncgrid/__init__.py
--rw-rw-rw-   0        0        0    14747 2024-04-29 20:27:55.000000 syncgrid-3.8/syncgrid/main.py
-drwxrwxrwx   0        0        0        0 2024-04-29 20:29:46.288959 syncgrid-3.8/syncgrid.egg-info/
--rw-rw-rw-   0        0        0      139 2024-04-29 20:29:46.000000 syncgrid-3.8/syncgrid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-04-29 20:29:46.000000 syncgrid-3.8/syncgrid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 20:29:46.000000 syncgrid-3.8/syncgrid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-29 20:29:46.000000 syncgrid-3.8/syncgrid.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2024-04-29 20:29:46.000000 syncgrid-3.8/syncgrid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 20:36:24.268021 syncgrid-3.9/
+-rw-rw-rw-   0        0        0      139 2024-04-29 20:36:24.266010 syncgrid-3.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-29 20:36:24.268021 syncgrid-3.9/setup.cfg
+-rw-rw-rw-   0        0        0      465 2024-04-29 20:36:11.000000 syncgrid-3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 20:36:24.249815 syncgrid-3.9/syncgrid/
+-rw-rw-rw-   0        0        0    15168 2024-04-29 20:35:49.000000 syncgrid-3.9/syncgrid/__init__.py
+-rw-rw-rw-   0        0        0    14747 2024-04-29 20:36:21.000000 syncgrid-3.9/syncgrid/main.py
+drwxrwxrwx   0        0        0        0 2024-04-29 20:36:24.264736 syncgrid-3.9/syncgrid.egg-info/
+-rw-rw-rw-   0        0        0      139 2024-04-29 20:36:24.000000 syncgrid-3.9/syncgrid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-04-29 20:36:24.000000 syncgrid-3.9/syncgrid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 20:36:24.000000 syncgrid-3.9/syncgrid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-29 20:36:24.000000 syncgrid-3.9/syncgrid.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2024-04-29 20:36:24.000000 syncgrid-3.9/syncgrid.egg-info/top_level.txt
```

### Comparing `syncgrid-3.8/syncgrid/main.py` & `syncgrid-3.9/syncgrid/main.py`

 * *Files identical despite different names*

