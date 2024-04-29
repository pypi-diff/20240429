# Comparing `tmp/g3elements-0.1.0.tar.gz` & `tmp/g3elements-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g3elements-0.1.0.tar", last modified: Tue Feb  6 17:17:46 2024, max compression
+gzip compressed data, was "g3elements-0.2.0.tar", last modified: Mon Apr 29 12:51:52 2024, max compression
```

## Comparing `g3elements-0.1.0.tar` & `g3elements-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-02-06 17:17:46.580079 g3elements-0.1.0/
--rw-rw-rw-   0        0        0     1091 2023-06-02 14:34:32.000000 g3elements-0.1.0/LICENCE
--rw-rw-rw-   0        0        0      640 2024-02-06 17:17:46.580079 g3elements-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       57 2023-07-26 10:08:43.000000 g3elements-0.1.0/README.md
--rw-rw-rw-   0        0        0      979 2024-02-06 16:57:36.000000 g3elements-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-06 17:17:46.580079 g3elements-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-06 17:17:46.434051 g3elements-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-02-06 17:17:46.517658 g3elements-0.1.0/src/g3elements/
--rw-rw-rw-   0        0        0     3577 2024-02-06 12:09:11.000000 g3elements-0.1.0/src/g3elements/__init__.py
--rw-rw-rw-   0        0        0     3940 2024-02-06 12:06:52.000000 g3elements-0.1.0/src/g3elements/_cabinet.py
--rw-rw-rw-   0        0        0      297 2024-01-24 23:10:05.000000 g3elements-0.1.0/src/g3elements/_crossing.py
--rw-rw-rw-   0        0        0      576 2024-01-24 23:11:04.000000 g3elements-0.1.0/src/g3elements/_detector.py
--rw-rw-rw-   0        0        0     4770 2024-01-25 21:17:21.000000 g3elements-0.1.0/src/g3elements/_element.py
--rw-rw-rw-   0        0        0      579 2024-02-06 12:07:06.000000 g3elements-0.1.0/src/g3elements/_gate.py
--rw-rw-rw-   0        0        0      300 2024-01-24 23:18:34.000000 g3elements-0.1.0/src/g3elements/_gpio.py
--rw-rw-rw-   0        0        0     3423 2024-02-06 12:07:13.000000 g3elements-0.1.0/src/g3elements/_heating.py
--rw-rw-rw-   0        0        0      310 2024-01-24 23:28:44.000000 g3elements-0.1.0/src/g3elements/_matrix.py
--rw-rw-rw-   0        0        0     1622 2024-02-06 12:06:33.000000 g3elements-0.1.0/src/g3elements/_pointmachine.py
--rw-rw-rw-   0        0        0     5974 2024-02-06 12:07:18.000000 g3elements-0.1.0/src/g3elements/_requestor.py
--rw-rw-rw-   0        0        0     9053 2024-01-25 22:49:09.000000 g3elements-0.1.0/src/g3elements/_route.py
--rw-rw-rw-   0        0        0     3043 2024-02-06 12:07:27.000000 g3elements-0.1.0/src/g3elements/_signal_symbol.py
--rw-rw-rw-   0        0        0      626 2024-01-25 16:28:38.000000 g3elements-0.1.0/src/g3elements/_system.py
--rw-rw-rw-   0        0        0    14221 2024-02-06 12:09:11.000000 g3elements-0.1.0/src/g3elements/_zone.py
-drwxrwxrwx   0        0        0        0 2024-02-06 17:17:46.575602 g3elements-0.1.0/src/g3elements/config/
--rw-rw-rw-   0        0        0      225 2024-02-06 12:11:24.000000 g3elements-0.1.0/src/g3elements/config/__init__.py
--rw-rw-rw-   0        0        0    13144 2024-02-06 17:10:07.000000 g3elements-0.1.0/src/g3elements/config/_cli.py
--rw-rw-rw-   0        0        0    20248 2024-02-06 14:55:41.000000 g3elements-0.1.0/src/g3elements/config/_g3core_updater.py
--rw-rw-rw-   0        0        0      876 2024-01-17 13:58:11.000000 g3elements-0.1.0/src/g3elements/config/_hw_connections.py
--rw-rw-rw-   0        0        0     8387 2024-02-06 17:09:49.000000 g3elements-0.1.0/src/g3elements/config/_iomap_updater.py
--rw-rw-rw-   0        0        0     7183 2024-01-31 09:16:36.000000 g3elements-0.1.0/src/g3elements/config/_sw_system_dict_wrapper.py
--rw-rw-rw-   0        0        0     3724 2024-02-06 17:10:21.000000 g3elements-0.1.0/src/g3elements/config/_system_config_processor.py
--rw-rw-rw-   0        0        0     1167 2024-01-23 19:33:50.000000 g3elements-0.1.0/src/g3elements/config/type_hinting.py
--rw-rw-rw-   0        0        0        0 2023-07-31 11:06:46.000000 g3elements-0.1.0/src/g3elements/py.typed
-drwxrwxrwx   0        0        0        0 2024-02-06 17:17:46.580079 g3elements-0.1.0/src/g3elements.egg-info/
--rw-rw-rw-   0        0        0      640 2024-02-06 17:17:46.000000 g3elements-0.1.0/src/g3elements.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1016 2024-02-06 17:17:46.000000 g3elements-0.1.0/src/g3elements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-06 17:17:46.000000 g3elements-0.1.0/src/g3elements.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-02-06 17:17:46.000000 g3elements-0.1.0/src/g3elements.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-02-06 17:17:46.000000 g3elements-0.1.0/src/g3elements.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-06 17:17:46.000000 g3elements-0.1.0/src/g3elements.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 12:51:52.226670 g3elements-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-02 14:34:32.000000 g3elements-0.2.0/LICENCE
+-rw-rw-rw-   0        0        0     1124 2024-04-29 12:51:52.224668 g3elements-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2023-07-26 10:08:43.000000 g3elements-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1331 2024-04-25 12:01:00.000000 g3elements-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 12:51:52.227667 g3elements-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 12:51:52.043685 g3elements-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 12:51:52.090665 g3elements-0.2.0/src/g3elements/
+-rw-rw-rw-   0        0        0     3452 2024-04-24 19:57:47.000000 g3elements-0.2.0/src/g3elements/__init__.py
+-rw-rw-rw-   0        0        0    56627 2024-04-24 19:55:40.000000 g3elements-0.2.0/src/g3elements/_elements.py
+-rw-rw-rw-   0        0        0        0 2023-07-31 11:06:46.000000 g3elements-0.2.0/src/g3elements/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-29 12:51:52.193668 g3elements-0.2.0/src/g3elements/route_utils/
+-rw-rw-rw-   0        0        0      424 2024-03-24 09:01:33.000000 g3elements-0.2.0/src/g3elements/route_utils/__init__.py
+-rw-rw-rw-   0        0        0    47295 2024-04-02 13:14:25.000000 g3elements-0.2.0/src/g3elements/route_utils/_analyzer.py
+-rw-rw-rw-   0        0        0    18088 2024-03-24 18:15:19.000000 g3elements-0.2.0/src/g3elements/route_utils/_manager.py
+-rw-rw-rw-   0        0        0     3495 2024-03-23 17:23:25.000000 g3elements-0.2.0/src/g3elements/route_utils/_tram.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:51:52.221666 g3elements-0.2.0/src/g3elements.egg-info/
+-rw-rw-rw-   0        0        0     1124 2024-04-29 12:51:51.000000 g3elements-0.2.0/src/g3elements.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2024-04-29 12:51:52.000000 g3elements-0.2.0/src/g3elements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 12:51:51.000000 g3elements-0.2.0/src/g3elements.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-29 12:51:51.000000 g3elements-0.2.0/src/g3elements.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-29 12:51:51.000000 g3elements-0.2.0/src/g3elements.egg-info/top_level.txt
```

### Comparing `g3elements-0.1.0/LICENCE` & `g3elements-0.2.0/LICENCE`

 * *Files identical despite different names*

