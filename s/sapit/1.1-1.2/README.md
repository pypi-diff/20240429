# Comparing `tmp/sapit-1.1.tar.gz` & `tmp/sapit-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapit-1.1.tar", last modified: Tue Apr 23 22:47:19 2024, max compression
+gzip compressed data, was "sapit-1.2.tar", last modified: Mon Apr 29 17:19:06 2024, max compression
```

## Comparing `sapit-1.1.tar` & `sapit-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 22:47:19.659031 sapit-1.1/
--rw-rw-rw-   0        0        0       80 2024-04-23 22:47:19.644040 sapit-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 22:47:19.581076 sapit-1.1/sapit/
--rw-rw-rw-   0        0        0       21 2024-04-23 22:25:03.000000 sapit-1.1/sapit/__init__.py
--rw-rw-rw-   0        0        0      201 2024-04-23 22:25:00.000000 sapit-1.1/sapit/main.py
-drwxrwxrwx   0        0        0        0 2024-04-23 22:47:19.642041 sapit-1.1/sapit.egg-info/
--rw-rw-rw-   0        0        0       80 2024-04-23 22:47:19.000000 sapit-1.1/sapit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-04-23 22:47:19.000000 sapit-1.1/sapit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 22:47:19.000000 sapit-1.1/sapit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-23 22:47:19.000000 sapit-1.1/sapit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-23 22:47:19.000000 sapit-1.1/sapit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-23 22:47:19.000000 sapit-1.1/sapit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 22:47:19.660031 sapit-1.1/setup.cfg
--rw-rw-rw-   0        0        0      302 2024-04-23 22:46:05.000000 sapit-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:19:06.195123 sapit-1.2/
+-rw-rw-rw-   0        0        0      208 2024-04-29 17:19:06.192125 sapit-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 17:19:06.140090 sapit-1.2/sapit/
+-rw-rw-rw-   0        0        0       45 2024-04-29 16:19:52.000000 sapit-1.2/sapit/__init__.py
+-rw-rw-rw-   0        0        0     1240 2024-04-29 17:13:22.000000 sapit-1.2/sapit/main.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:19:06.189131 sapit-1.2/sapit.egg-info/
+-rw-rw-rw-   0        0        0      208 2024-04-29 17:19:05.000000 sapit-1.2/sapit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-04-29 17:19:06.000000 sapit-1.2/sapit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 17:19:05.000000 sapit-1.2/sapit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-29 17:19:05.000000 sapit-1.2/sapit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-04-29 17:19:05.000000 sapit-1.2/sapit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-29 17:19:05.000000 sapit-1.2/sapit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 17:19:06.196123 sapit-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      439 2024-04-29 17:14:20.000000 sapit-1.2/setup.py
```

