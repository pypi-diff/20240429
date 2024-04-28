# Comparing `tmp/IslandSheds-0.0.15.tar.gz` & `tmp/islandsheds-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IslandSheds-0.0.15.tar", last modified: Sun Apr 28 04:09:17 2024, max compression
+gzip compressed data, was "islandsheds-0.0.16.tar", last modified: Sun Apr 28 22:50:55 2024, max compression
```

## Comparing `IslandSheds-0.0.15.tar` & `islandsheds-0.0.16.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 04:09:17.789608 IslandSheds-0.0.15/
-drwxrwxrwx   0        0        0        0 2024-04-28 04:09:17.756980 IslandSheds-0.0.15/IslandSheds/
--rw-rw-rw-   0        0        0      164 2024-04-28 03:58:11.000000 IslandSheds-0.0.15/IslandSheds/__init__.py
--rw-rw-rw-   0        0        0     3475 2024-04-28 02:28:07.000000 IslandSheds-0.0.15/IslandSheds/downloader.py
-drwxrwxrwx   0        0        0        0 2024-04-28 04:09:17.787443 IslandSheds-0.0.15/IslandSheds.egg-info/
--rw-rw-rw-   0        0        0      572 2024-04-28 04:09:17.000000 IslandSheds-0.0.15/IslandSheds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-04-28 04:09:17.000000 IslandSheds-0.0.15/IslandSheds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 04:09:17.000000 IslandSheds-0.0.15/IslandSheds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-28 04:09:17.000000 IslandSheds-0.0.15/IslandSheds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-28 04:09:17.000000 IslandSheds-0.0.15/IslandSheds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      572 2024-04-28 04:09:17.788554 IslandSheds-0.0.15/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-28 04:09:17.789608 IslandSheds-0.0.15/setup.cfg
--rw-rw-rw-   0        0        0      952 2024-04-28 03:57:07.000000 IslandSheds-0.0.15/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 22:50:55.169384 islandsheds-0.0.16/
+drwxrwxrwx   0        0        0        0 2024-04-28 22:50:55.120380 islandsheds-0.0.16/IslandSheds/
+-rw-rw-rw-   0        0        0      893 2024-04-28 22:26:39.000000 islandsheds-0.0.16/IslandSheds/__init__.py
+-rw-rw-rw-   0        0        0     6227 2024-04-28 22:21:36.000000 islandsheds-0.0.16/IslandSheds/downloader.py
+drwxrwxrwx   0        0        0        0 2024-04-28 22:50:55.165646 islandsheds-0.0.16/IslandSheds.egg-info/
+-rw-rw-rw-   0        0        0      844 2024-04-28 22:50:54.000000 islandsheds-0.0.16/IslandSheds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-04-28 22:50:54.000000 islandsheds-0.0.16/IslandSheds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 22:50:54.000000 islandsheds-0.0.16/IslandSheds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-28 22:50:54.000000 islandsheds-0.0.16/IslandSheds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-28 22:50:54.000000 islandsheds-0.0.16/IslandSheds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-28 22:50:54.000000 islandsheds-0.0.16/IslandSheds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      844 2024-04-28 22:50:55.167079 islandsheds-0.0.16/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-28 22:50:55.169384 islandsheds-0.0.16/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2024-04-28 22:50:06.000000 islandsheds-0.0.16/setup.py
```

