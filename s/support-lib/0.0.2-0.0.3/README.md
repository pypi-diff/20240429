# Comparing `tmp/support_lib-0.0.2.tar.gz` & `tmp/support_lib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "support_lib-0.0.2.tar", last modified: Thu Apr 25 13:57:31 2024, max compression
+gzip compressed data, was "support_lib-0.0.3.tar", last modified: Mon Apr 29 12:58:07 2024, max compression
```

## Comparing `support_lib-0.0.2.tar` & `support_lib-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 darren.white   (501) staff       (20)        0 2024-04-25 13:57:31.363251 support_lib-0.0.2/
--rw-r--r--   0 darren.white   (501) staff       (20)     1091 2024-04-25 12:47:41.000000 support_lib-0.0.2/LICENSE
--rw-r--r--   0 darren.white   (501) staff       (20)      453 2024-04-25 13:57:31.363125 support_lib-0.0.2/PKG-INFO
--rw-r--r--   0 darren.white   (501) staff       (20)      142 2024-04-25 12:57:54.000000 support_lib-0.0.2/README.md
--rw-r--r--   0 darren.white   (501) staff       (20)       38 2024-04-25 13:57:31.363303 support_lib-0.0.2/setup.cfg
--rw-r--r--   0 darren.white   (501) staff       (20)      622 2024-04-25 13:57:16.000000 support_lib-0.0.2/setup.py
-drwxr-xr-x   0 darren.white   (501) staff       (20)        0 2024-04-25 13:57:31.362321 support_lib-0.0.2/support_lib/
--rw-r--r--   0 darren.white   (501) staff       (20)        0 2024-04-25 12:44:00.000000 support_lib-0.0.2/support_lib/__init__.py
--rw-r--r--   0 darren.white   (501) staff       (20)     4029 2024-04-25 12:44:37.000000 support_lib-0.0.2/support_lib/database.py
--rw-r--r--   0 darren.white   (501) staff       (20)     1961 2024-04-25 12:44:37.000000 support_lib-0.0.2/support_lib/email.py
--rwxr-xr-x   0 darren.white   (501) staff       (20)     1228 2024-04-25 12:44:37.000000 support_lib-0.0.2/support_lib/jira_api.py
--rw-r--r--   0 darren.white   (501) staff       (20)      918 2024-04-25 12:44:37.000000 support_lib-0.0.2/support_lib/logger.py
--rw-r--r--   0 darren.white   (501) staff       (20)     1057 2024-04-25 12:44:37.000000 support_lib-0.0.2/support_lib/mysql_db.py
--rw-r--r--   0 darren.white   (501) staff       (20)      727 2024-04-25 12:44:37.000000 support_lib-0.0.2/support_lib/opsgenie.py
-drwxr-xr-x   0 darren.white   (501) staff       (20)        0 2024-04-25 13:57:31.362944 support_lib-0.0.2/support_lib.egg-info/
--rw-r--r--   0 darren.white   (501) staff       (20)      453 2024-04-25 13:57:31.000000 support_lib-0.0.2/support_lib.egg-info/PKG-INFO
--rw-r--r--   0 darren.white   (501) staff       (20)      363 2024-04-25 13:57:31.000000 support_lib-0.0.2/support_lib.egg-info/SOURCES.txt
--rw-r--r--   0 darren.white   (501) staff       (20)        1 2024-04-25 13:57:31.000000 support_lib-0.0.2/support_lib.egg-info/dependency_links.txt
--rw-r--r--   0 darren.white   (501) staff       (20)       71 2024-04-25 13:57:31.000000 support_lib-0.0.2/support_lib.egg-info/requires.txt
--rw-r--r--   0 darren.white   (501) staff       (20)       12 2024-04-25 13:57:31.000000 support_lib-0.0.2/support_lib.egg-info/top_level.txt
+drwxr-xr-x   0 darren.white   (501) staff       (20)        0 2024-04-29 12:58:07.984841 support_lib-0.0.3/
+-rw-r--r--   0 darren.white   (501) staff       (20)     1091 2024-04-25 12:47:41.000000 support_lib-0.0.3/LICENSE
+-rw-r--r--   0 darren.white   (501) staff       (20)     1265 2024-04-29 12:58:07.984597 support_lib-0.0.3/PKG-INFO
+-rw-r--r--   0 darren.white   (501) staff       (20)      142 2024-04-25 12:57:54.000000 support_lib-0.0.3/README.md
+-rw-r--r--   0 darren.white   (501) staff       (20)      344 2024-04-29 12:55:20.000000 support_lib-0.0.3/pyproject.toml
+-rw-r--r--   0 darren.white   (501) staff       (20)       38 2024-04-29 12:58:07.984896 support_lib-0.0.3/setup.cfg
+drwxr-xr-x   0 darren.white   (501) staff       (20)        0 2024-04-29 12:58:07.983416 support_lib-0.0.3/support_lib/
+-rw-r--r--   0 darren.white   (501) staff       (20)        0 2024-04-25 12:44:00.000000 support_lib-0.0.3/support_lib/__init__.py
+-rw-r--r--   0 darren.white   (501) staff       (20)     4029 2024-04-25 12:44:37.000000 support_lib-0.0.3/support_lib/database.py
+-rw-r--r--   0 darren.white   (501) staff       (20)     1961 2024-04-25 12:44:37.000000 support_lib-0.0.3/support_lib/email.py
+-rwxr-xr-x   0 darren.white   (501) staff       (20)     1228 2024-04-25 12:44:37.000000 support_lib-0.0.3/support_lib/jira_api.py
+-rw-r--r--   0 darren.white   (501) staff       (20)      918 2024-04-25 12:44:37.000000 support_lib-0.0.3/support_lib/logger.py
+-rw-r--r--   0 darren.white   (501) staff       (20)     1057 2024-04-25 12:44:37.000000 support_lib-0.0.3/support_lib/mysql_db.py
+-rw-r--r--   0 darren.white   (501) staff       (20)      727 2024-04-25 12:44:37.000000 support_lib-0.0.3/support_lib/opsgenie.py
+drwxr-xr-x   0 darren.white   (501) staff       (20)        0 2024-04-29 12:58:07.984321 support_lib-0.0.3/support_lib.egg-info/
+-rw-r--r--   0 darren.white   (501) staff       (20)     1265 2024-04-29 12:58:07.000000 support_lib-0.0.3/support_lib.egg-info/PKG-INFO
+-rw-r--r--   0 darren.white   (501) staff       (20)      335 2024-04-29 12:58:07.000000 support_lib-0.0.3/support_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 darren.white   (501) staff       (20)        1 2024-04-29 12:58:07.000000 support_lib-0.0.3/support_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 darren.white   (501) staff       (20)       12 2024-04-29 12:58:07.000000 support_lib-0.0.3/support_lib.egg-info/top_level.txt
```

### Comparing `support_lib-0.0.2/LICENSE` & `support_lib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `support_lib-0.0.2/support_lib/database.py` & `support_lib-0.0.3/support_lib/database.py`

 * *Files identical despite different names*

### Comparing `support_lib-0.0.2/support_lib/email.py` & `support_lib-0.0.3/support_lib/email.py`

 * *Files identical despite different names*

### Comparing `support_lib-0.0.2/support_lib/jira_api.py` & `support_lib-0.0.3/support_lib/jira_api.py`

 * *Files identical despite different names*

### Comparing `support_lib-0.0.2/support_lib/logger.py` & `support_lib-0.0.3/support_lib/logger.py`

 * *Files identical despite different names*

### Comparing `support_lib-0.0.2/support_lib/mysql_db.py` & `support_lib-0.0.3/support_lib/mysql_db.py`

 * *Files identical despite different names*

### Comparing `support_lib-0.0.2/support_lib/opsgenie.py` & `support_lib-0.0.3/support_lib/opsgenie.py`

 * *Files identical despite different names*

