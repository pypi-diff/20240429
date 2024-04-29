# Comparing `tmp/EasyLoggerAJM-0.1.tar.gz` & `tmp/EasyLoggerAJM-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyLoggerAJM-0.1.tar", last modified: Fri Mar  8 19:29:08 2024, max compression
+gzip compressed data, was "EasyLoggerAJM-0.5.tar", last modified: Mon Apr 29 12:57:28 2024, max compression
```

## Comparing `EasyLoggerAJM-0.1.tar` & `EasyLoggerAJM-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-08 19:29:08.128232 EasyLoggerAJM-0.1/
-drwxrwxrwx   0        0        0        0 2024-03-08 19:29:08.107906 EasyLoggerAJM-0.1/EasyLoggerAJM/
--rw-rw-rw-   0        0        0     4144 2024-03-08 19:24:07.000000 EasyLoggerAJM-0.1/EasyLoggerAJM/EasyLoggerAJM.py
--rw-rw-rw-   0        0        0       52 2024-03-08 19:24:07.000000 EasyLoggerAJM-0.1/EasyLoggerAJM/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-08 19:29:08.125240 EasyLoggerAJM-0.1/EasyLoggerAJM.egg-info/
--rw-rw-rw-   0        0        0      412 2024-03-08 19:29:08.000000 EasyLoggerAJM-0.1/EasyLoggerAJM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-03-08 19:29:08.000000 EasyLoggerAJM-0.1/EasyLoggerAJM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-08 19:29:08.000000 EasyLoggerAJM-0.1/EasyLoggerAJM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-03-08 19:29:08.000000 EasyLoggerAJM-0.1/EasyLoggerAJM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2024-03-08 19:21:34.000000 EasyLoggerAJM-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      412 2024-03-08 19:29:08.128232 EasyLoggerAJM-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-03-08 19:21:34.000000 EasyLoggerAJM-0.1/README.md
--rw-rw-rw-   0        0        0       86 2024-03-08 19:29:08.133192 EasyLoggerAJM-0.1/setup.cfg
--rw-rw-rw-   0        0        0      491 2024-03-08 19:24:29.000000 EasyLoggerAJM-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:57:28.324334 EasyLoggerAJM-0.5/
+drwxrwxrwx   0        0        0        0 2024-04-29 12:57:28.300397 EasyLoggerAJM-0.5/EasyLoggerAJM/
+-rw-rw-rw-   0        0        0     4525 2024-04-29 12:51:25.000000 EasyLoggerAJM-0.5/EasyLoggerAJM/EasyLoggerAJM.py
+-rw-rw-rw-   0        0        0       52 2024-03-08 19:24:07.000000 EasyLoggerAJM-0.5/EasyLoggerAJM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:57:28.320344 EasyLoggerAJM-0.5/EasyLoggerAJM.egg-info/
+-rw-rw-rw-   0        0        0      412 2024-04-29 12:57:28.000000 EasyLoggerAJM-0.5/EasyLoggerAJM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-29 12:57:28.000000 EasyLoggerAJM-0.5/EasyLoggerAJM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 12:57:28.000000 EasyLoggerAJM-0.5/EasyLoggerAJM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-29 12:57:28.000000 EasyLoggerAJM-0.5/EasyLoggerAJM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2024-03-08 19:21:34.000000 EasyLoggerAJM-0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      412 2024-04-29 12:57:28.325331 EasyLoggerAJM-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-03-08 19:21:34.000000 EasyLoggerAJM-0.5/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-29 12:57:28.329321 EasyLoggerAJM-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      491 2024-04-29 12:51:44.000000 EasyLoggerAJM-0.5/setup.py
```

### Comparing `EasyLoggerAJM-0.1/EasyLoggerAJM/EasyLoggerAJM.py` & `EasyLoggerAJM-0.5/EasyLoggerAJM/EasyLoggerAJM.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,22 +8,29 @@
 from datetime import datetime
 from os import makedirs
 from os.path import join, isdir
 
 
 class EasyLogger:
     def __init__(self, project_name=None, root_log_location="../logs",
-                 chosen_format='%(asctime)s | %(name)s | %(levelname)s | %(message)s', logger=None):
+                 chosen_format='%(asctime)s | %(name)s | %(levelname)s | %(message)s', logger=None, **kwargs):
 
         self._project_name = project_name
         self._root_log_location = root_log_location
         self._inner_log_fstructure = None
         self._log_location = None
 
-        self.timestamp = datetime.now().isoformat(timespec='minutes').replace(':',
+        if kwargs:
+            if 'timestamp' in kwargs and (isinstance(kwargs['timestamp'], datetime)
+                                          or isinstance(kwargs['timestamp'], str)):
+                self.timestamp = kwargs['timestamp']
+            else:
+                raise AttributeError("timestamp must be a datetime object or a string")
+        else:
+            self.timestamp = datetime.now().isoformat(timespec='minutes').replace(':',
                                                                               '')  # datetime.now().date().isoformat()
         self.formatter = logging.Formatter(chosen_format)
         self.logger_levels = ["DEBUG", "INFO", "ERROR"]
         if not logger:
             # Create a logger with a specified name and make sure propagate is True
             self.logger = logging.getLogger('logger')
         else:
```

### Comparing `EasyLoggerAJM-0.1/LICENSE.txt` & `EasyLoggerAJM-0.5/LICENSE.txt`

 * *Files identical despite different names*

