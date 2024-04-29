# Comparing `tmp/bambot-0.3.0.tar.gz` & `tmp/bambot-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambot-0.3.0.tar", last modified: Sun Apr 28 23:22:58 2024, max compression
+gzip compressed data, was "bambot-0.3.1.tar", last modified: Mon Apr 29 00:03:28 2024, max compression
```

## Comparing `bambot-0.3.0.tar` & `bambot-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-28 23:22:58.669552 bambot-0.3.0/
--rw-r--r--   0 spencerkinney   (501) staff       (20)      850 2024-04-28 23:22:58.669357 bambot-0.3.0/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      148 2024-04-27 21:13:32.000000 bambot-0.3.0/README.md
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-28 23:22:58.667409 bambot-0.3.0/bambot/
--rw-r--r--   0 spencerkinney   (501) staff       (20)       60 2024-04-27 22:56:54.000000 bambot-0.3.0/bambot/__init__.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1832 2024-04-28 22:59:21.000000 bambot-0.3.0/bambot/agent.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     7078 2024-04-28 23:10:48.000000 bambot-0.3.0/bambot/cli.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     2079 2024-04-28 23:07:57.000000 bambot-0.3.0/bambot/docker_utils.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      464 2024-04-28 23:09:41.000000 bambot-0.3.0/bambot/log_utils.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      709 2024-04-28 22:50:06.000000 bambot-0.3.0/bambot/logger.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      371 2024-04-28 08:09:43.000000 bambot-0.3.0/bambot/utils.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-28 23:22:58.669143 bambot-0.3.0/bambot.egg-info/
--rw-r--r--   0 spencerkinney   (501) staff       (20)      850 2024-04-28 23:22:58.000000 bambot-0.3.0/bambot.egg-info/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      346 2024-04-28 23:22:58.000000 bambot-0.3.0/bambot.egg-info/SOURCES.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-04-28 23:22:58.000000 bambot-0.3.0/bambot.egg-info/dependency_links.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       39 2024-04-28 23:22:58.000000 bambot-0.3.0/bambot.egg-info/entry_points.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       18 2024-04-28 23:22:58.000000 bambot-0.3.0/bambot.egg-info/requires.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-04-28 23:22:58.000000 bambot-0.3.0/bambot.egg-info/top_level.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-04-28 23:22:58.669585 bambot-0.3.0/setup.cfg
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1065 2024-04-28 23:22:26.000000 bambot-0.3.0/setup.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-28 23:22:58.668752 bambot-0.3.0/tests/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1443 2024-04-27 21:53:17.000000 bambot-0.3.0/tests/test_bambot.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 00:03:28.988305 bambot-0.3.1/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1003 2024-04-29 00:03:28.988094 bambot-0.3.1/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      148 2024-04-27 21:13:32.000000 bambot-0.3.1/README.md
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 00:03:28.986493 bambot-0.3.1/bambot/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       60 2024-04-27 22:56:54.000000 bambot-0.3.1/bambot/__init__.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1832 2024-04-28 22:59:21.000000 bambot-0.3.1/bambot/agent.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     7078 2024-04-28 23:10:48.000000 bambot-0.3.1/bambot/cli.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2079 2024-04-28 23:07:57.000000 bambot-0.3.1/bambot/docker_utils.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      464 2024-04-28 23:09:41.000000 bambot-0.3.1/bambot/log_utils.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      709 2024-04-28 22:50:06.000000 bambot-0.3.1/bambot/logger.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      371 2024-04-28 08:09:43.000000 bambot-0.3.1/bambot/utils.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 00:03:28.987865 bambot-0.3.1/bambot.egg-info/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1003 2024-04-29 00:03:28.000000 bambot-0.3.1/bambot.egg-info/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      346 2024-04-29 00:03:28.000000 bambot-0.3.1/bambot.egg-info/SOURCES.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-04-29 00:03:28.000000 bambot-0.3.1/bambot.egg-info/dependency_links.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       39 2024-04-29 00:03:28.000000 bambot-0.3.1/bambot.egg-info/entry_points.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       18 2024-04-29 00:03:28.000000 bambot-0.3.1/bambot.egg-info/requires.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-04-29 00:03:28.000000 bambot-0.3.1/bambot.egg-info/top_level.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-04-29 00:03:28.988342 bambot-0.3.1/setup.cfg
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1205 2024-04-29 00:03:20.000000 bambot-0.3.1/setup.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 00:03:28.987541 bambot-0.3.1/tests/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1443 2024-04-27 21:53:17.000000 bambot-0.3.1/tests/test_bambot.py
```

### Comparing `bambot-0.3.0/bambot/agent.py` & `bambot-0.3.1/bambot/agent.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.0/bambot/cli.py` & `bambot-0.3.1/bambot/cli.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.0/bambot/docker_utils.py` & `bambot-0.3.1/bambot/docker_utils.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.0/bambot/logger.py` & `bambot-0.3.1/bambot/logger.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.0/tests/test_bambot.py` & `bambot-0.3.1/tests/test_bambot.py`

 * *Files identical despite different names*

