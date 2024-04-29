# Comparing `tmp/firex_blaze-1.8.tar.gz` & `tmp/firex_blaze-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/firex_blaze-1.8.tar", last modified: Wed Apr 14 19:44:46 2021, max compression
+gzip compressed data, was "dist/firex_blaze-1.9.tar", last modified: Thu Apr 15 13:52:15 2021, max compression
```

## Comparing `firex_blaze-1.8.tar` & `firex_blaze-1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-04-14 19:44:46.000000 firex_blaze-1.8/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1505 2021-04-14 19:44:34.000000 firex_blaze-1.8/LICENSE
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      103 2021-04-14 19:44:34.000000 firex_blaze-1.8/MANIFEST.in
--rw-r--r--   0 firex      (101) nogroup  (65533)      287 2021-04-14 19:44:46.000000 firex_blaze-1.8/PKG-INFO
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      254 2021-04-14 19:44:34.000000 firex_blaze-1.8/README.md
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2021-04-14 19:44:34.000000 firex_blaze-1.8/fastentrypoints.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-04-14 19:44:46.000000 firex_blaze-1.8/firex_blaze/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       92 2021-04-14 19:44:34.000000 firex_blaze-1.8/firex_blaze/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3050 2021-04-14 19:44:34.000000 firex_blaze-1.8/firex_blaze/__main__.py
--rw-r--r--   0 firex      (101) nogroup  (65533)      495 2021-04-14 19:44:46.000000 firex_blaze-1.8/firex_blaze/_version.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6477 2021-04-14 19:44:34.000000 firex_blaze-1.8/firex_blaze/blaze_event_consumer.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1737 2021-04-14 19:44:34.000000 firex_blaze-1.8/firex_blaze/blaze_helper.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4427 2021-04-14 19:44:34.000000 firex_blaze-1.8/firex_blaze/blaze_launcher.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      310 2021-04-14 19:44:34.000000 firex_blaze-1.8/firex_blaze/fast_blaze_helper.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-04-14 19:44:46.000000 firex_blaze-1.8/firex_blaze.egg-info/
--rw-r--r--   0 firex      (101) nogroup  (65533)      287 2021-04-14 19:44:46.000000 firex_blaze-1.8/firex_blaze.egg-info/PKG-INFO
--rw-r--r--   0 firex      (101) nogroup  (65533)      522 2021-04-14 19:44:46.000000 firex_blaze-1.8/firex_blaze.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-04-14 19:44:46.000000 firex_blaze-1.8/firex_blaze.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      154 2021-04-14 19:44:46.000000 firex_blaze-1.8/firex_blaze.egg-info/entry_points.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       29 2021-04-14 19:44:46.000000 firex_blaze-1.8/firex_blaze.egg-info/requires.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       12 2021-04-14 19:44:46.000000 firex_blaze-1.8/firex_blaze.egg-info/top_level.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-04-14 19:44:46.000000 firex_blaze-1.8/firex_blaze.egg-info/zip-safe
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      276 2021-04-14 19:44:46.000000 firex_blaze-1.8/setup.cfg
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      933 2021-04-14 19:44:34.000000 firex_blaze-1.8/setup.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2021-04-14 19:44:34.000000 firex_blaze-1.8/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-04-15 13:52:15.000000 firex_blaze-1.9/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1505 2021-04-15 13:52:02.000000 firex_blaze-1.9/LICENSE
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      103 2021-04-15 13:52:02.000000 firex_blaze-1.9/MANIFEST.in
+-rw-r--r--   0 firex      (101) nogroup  (65533)      287 2021-04-15 13:52:15.000000 firex_blaze-1.9/PKG-INFO
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      254 2021-04-15 13:52:02.000000 firex_blaze-1.9/README.md
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2021-04-15 13:52:02.000000 firex_blaze-1.9/fastentrypoints.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-04-15 13:52:15.000000 firex_blaze-1.9/firex_blaze/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       92 2021-04-15 13:52:02.000000 firex_blaze-1.9/firex_blaze/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3050 2021-04-15 13:52:02.000000 firex_blaze-1.9/firex_blaze/__main__.py
+-rw-r--r--   0 firex      (101) nogroup  (65533)      495 2021-04-15 13:52:15.000000 firex_blaze-1.9/firex_blaze/_version.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6477 2021-04-15 13:52:02.000000 firex_blaze-1.9/firex_blaze/blaze_event_consumer.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1737 2021-04-15 13:52:02.000000 firex_blaze-1.9/firex_blaze/blaze_helper.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4417 2021-04-15 13:52:02.000000 firex_blaze-1.9/firex_blaze/blaze_launcher.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      310 2021-04-15 13:52:02.000000 firex_blaze-1.9/firex_blaze/fast_blaze_helper.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-04-15 13:52:15.000000 firex_blaze-1.9/firex_blaze.egg-info/
+-rw-r--r--   0 firex      (101) nogroup  (65533)      287 2021-04-15 13:52:14.000000 firex_blaze-1.9/firex_blaze.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (101) nogroup  (65533)      522 2021-04-15 13:52:14.000000 firex_blaze-1.9/firex_blaze.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-04-15 13:52:14.000000 firex_blaze-1.9/firex_blaze.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      154 2021-04-15 13:52:14.000000 firex_blaze-1.9/firex_blaze.egg-info/entry_points.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       29 2021-04-15 13:52:14.000000 firex_blaze-1.9/firex_blaze.egg-info/requires.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       12 2021-04-15 13:52:14.000000 firex_blaze-1.9/firex_blaze.egg-info/top_level.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-04-15 13:52:14.000000 firex_blaze-1.9/firex_blaze.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      276 2021-04-15 13:52:15.000000 firex_blaze-1.9/setup.cfg
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      933 2021-04-15 13:52:02.000000 firex_blaze-1.9/setup.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2021-04-15 13:52:02.000000 firex_blaze-1.9/versioneer.py
```

### Comparing `firex_blaze-1.8/LICENSE` & `firex_blaze-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `firex_blaze-1.8/fastentrypoints.py` & `firex_blaze-1.9/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `firex_blaze-1.8/firex_blaze/__main__.py` & `firex_blaze-1.9/firex_blaze/__main__.py`

 * *Files identical despite different names*

### Comparing `firex_blaze-1.8/firex_blaze/blaze_event_consumer.py` & `firex_blaze-1.9/firex_blaze/blaze_event_consumer.py`

 * *Files identical despite different names*

### Comparing `firex_blaze-1.8/firex_blaze/blaze_helper.py` & `firex_blaze-1.9/firex_blaze/blaze_helper.py`

 * *Files identical despite different names*

### Comparing `firex_blaze-1.8/firex_blaze/blaze_launcher.py` & `firex_blaze-1.9/firex_blaze/blaze_launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,10 +95,10 @@
                 logger.debug("Blaze up after %.2f s" % (time.time() - self.start_time))
 
         return self.is_ready_for_tasks
 
 
     def get_pkg_version_info(self) -> PkgVersionInfo:
         import firex_blaze
-        return PkgVersionInfo(pkg=firex_blaze.__package__,
+        return PkgVersionInfo(pkg='firex-blaze',
                               version=firex_blaze.__version__,
                               commit=firex_blaze._version.get_versions()['full-revisionid'])
```

### Comparing `firex_blaze-1.8/firex_blaze.egg-info/SOURCES.txt` & `firex_blaze-1.9/firex_blaze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firex_blaze-1.8/setup.py` & `firex_blaze-1.9/setup.py`

 * *Files identical despite different names*

### Comparing `firex_blaze-1.8/versioneer.py` & `firex_blaze-1.9/versioneer.py`

 * *Files identical despite different names*

