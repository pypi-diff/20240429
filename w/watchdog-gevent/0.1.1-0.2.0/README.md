# Comparing `tmp/watchdog_gevent-0.1.1.tar.gz` & `tmp/watchdog_gevent-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/watchdog_gevent-0.1.1.tar", last modified: Wed Oct  3 05:37:36 2018, max compression
+gzip compressed data, was "watchdog_gevent-0.2.0.tar", last modified: Mon Apr 29 12:53:51 2024, max compression
```

## Comparing `watchdog_gevent-0.1.1.tar` & `watchdog_gevent-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2018-10-03 05:37:36.000000 watchdog_gevent-0.1.1/
--rw-r--r--   0 bogdan     (501) staff       (20)      327 2018-10-03 05:37:36.000000 watchdog_gevent-0.1.1/PKG-INFO
--rw-r--r--   0 bogdan     (501) staff       (20)      556 2017-12-08 14:22:27.000000 watchdog_gevent-0.1.1/LICENSE
--rw-r--r--   0 bogdan     (501) staff       (20)       16 2018-10-03 05:33:26.000000 watchdog_gevent-0.1.1/MANIFEST.in
--rw-r--r--   0 bogdan     (501) staff       (20)     1290 2018-10-03 05:33:39.000000 watchdog_gevent-0.1.1/README.md
--rw-r--r--   0 bogdan     (501) staff       (20)      908 2018-10-03 05:36:30.000000 watchdog_gevent-0.1.1/setup.py
--rw-r--r--   0 bogdan     (501) staff       (20)      276 2018-10-03 05:37:36.000000 watchdog_gevent-0.1.1/setup.cfg
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2018-10-03 05:37:36.000000 watchdog_gevent-0.1.1/watchdog_gevent/
--rw-r--r--   0 bogdan     (501) staff       (20)      382 2018-10-03 05:37:13.000000 watchdog_gevent-0.1.1/watchdog_gevent/__init__.py
--rw-r--r--   0 bogdan     (501) staff       (20)     3988 2017-12-08 17:20:55.000000 watchdog_gevent-0.1.1/watchdog_gevent/observers.py
-drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2018-10-03 05:37:36.000000 watchdog_gevent-0.1.1/watchdog_gevent.egg-info/
--rw-r--r--   0 bogdan     (501) staff       (20)      327 2018-10-03 05:37:36.000000 watchdog_gevent-0.1.1/watchdog_gevent.egg-info/PKG-INFO
--rw-r--r--   0 bogdan     (501) staff       (20)      299 2018-10-03 05:37:36.000000 watchdog_gevent-0.1.1/watchdog_gevent.egg-info/SOURCES.txt
--rw-r--r--   0 bogdan     (501) staff       (20)       26 2018-10-03 05:37:36.000000 watchdog_gevent-0.1.1/watchdog_gevent.egg-info/requires.txt
--rw-r--r--   0 bogdan     (501) staff       (20)       16 2018-10-03 05:37:36.000000 watchdog_gevent-0.1.1/watchdog_gevent.egg-info/top_level.txt
--rw-r--r--   0 bogdan     (501) staff       (20)        1 2018-10-03 05:37:36.000000 watchdog_gevent-0.1.1/watchdog_gevent.egg-info/dependency_links.txt
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2024-04-29 12:53:51.159481 watchdog_gevent-0.2.0/
+-rw-r--r--   0 bogdan     (501) staff       (20)      556 2024-04-29 12:37:35.000000 watchdog_gevent-0.2.0/LICENSE
+-rw-r--r--   0 bogdan     (501) staff       (20)       16 2024-04-29 12:37:35.000000 watchdog_gevent-0.2.0/MANIFEST.in
+-rw-r--r--   0 bogdan     (501) staff       (20)      568 2024-04-29 12:53:51.159429 watchdog_gevent-0.2.0/PKG-INFO
+-rw-r--r--   0 bogdan     (501) staff       (20)     1226 2024-04-29 12:37:35.000000 watchdog_gevent-0.2.0/README.md
+-rw-r--r--   0 bogdan     (501) staff       (20)      276 2024-04-29 12:53:51.159659 watchdog_gevent-0.2.0/setup.cfg
+-rw-r--r--   0 bogdan     (501) staff       (20)     1110 2024-04-29 12:46:37.000000 watchdog_gevent-0.2.0/setup.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2024-04-29 12:53:51.158270 watchdog_gevent-0.2.0/tests/
+-rw-r--r--   0 bogdan     (501) staff       (20)     1391 2024-04-29 12:53:33.000000 watchdog_gevent-0.2.0/tests/test_observer.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2024-04-29 12:53:51.158458 watchdog_gevent-0.2.0/watchdog_gevent/
+-rw-r--r--   0 bogdan     (501) staff       (20)      382 2024-04-29 12:53:43.000000 watchdog_gevent-0.2.0/watchdog_gevent/__init__.py
+-rw-r--r--   0 bogdan     (501) staff       (20)     4021 2024-04-29 12:42:02.000000 watchdog_gevent-0.2.0/watchdog_gevent/observers.py
+drwxr-xr-x   0 bogdan     (501) staff       (20)        0 2024-04-29 12:53:51.159067 watchdog_gevent-0.2.0/watchdog_gevent.egg-info/
+-rw-r--r--   0 bogdan     (501) staff       (20)      568 2024-04-29 12:53:51.000000 watchdog_gevent-0.2.0/watchdog_gevent.egg-info/PKG-INFO
+-rw-r--r--   0 bogdan     (501) staff       (20)      322 2024-04-29 12:53:51.000000 watchdog_gevent-0.2.0/watchdog_gevent.egg-info/SOURCES.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)        1 2024-04-29 12:53:51.000000 watchdog_gevent-0.2.0/watchdog_gevent.egg-info/dependency_links.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)       90 2024-04-29 12:53:51.000000 watchdog_gevent-0.2.0/watchdog_gevent.egg-info/requires.txt
+-rw-r--r--   0 bogdan     (501) staff       (20)       16 2024-04-29 12:53:51.000000 watchdog_gevent-0.2.0/watchdog_gevent.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `watchdog_gevent-0.1.1/LICENSE` & `watchdog_gevent-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `watchdog_gevent-0.1.1/README.md` & `watchdog_gevent-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 
 * [gevent] 1.1+
 * [watchdog] 0.8+
 
 
 ## Setup
 
-Use [pipenv][pipenv] (or plain pip) to install the package:
-
-    pipenv install watchdog_gevent
+    pip install watchdog_gevent
 
 
 ## Usage
 
 Just import and use its observer:
 
 ``` python
```

### Comparing `watchdog_gevent-0.1.1/watchdog_gevent/observers.py` & `watchdog_gevent-0.2.0/watchdog_gevent/observers.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,16 @@
         return None
 
 
 class GeventEmitter(EventEmitter):
     """gevent-based emitter.
     """
 
-    def __init__(self, event_queue, watch, timeout=DEFAULT_EMITTER_TIMEOUT):
-        EventEmitter.__init__(self, event_queue, watch, timeout)
+    def __init__(self, event_queue, watch, timeout=DEFAULT_EMITTER_TIMEOUT, event_filter=None):
+        EventEmitter.__init__(self, event_queue, watch, timeout, event_filter)
 
         self._hub = gevent.get_hub()
         self._watchlist = set()
         self._workers = gevent.pool.Group()
         self._add(watch.path, watch.is_recursive)
 
     def queue_events(self, timeout):
```

