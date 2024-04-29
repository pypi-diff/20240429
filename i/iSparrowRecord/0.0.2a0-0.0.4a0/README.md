# Comparing `tmp/isparrowrecord-0.0.2a0.tar.gz` & `tmp/isparrowrecord-0.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isparrowrecord-0.0.2a0.tar", last modified: Mon Apr 29 10:55:26 2024, max compression
+gzip compressed data, was "isparrowrecord-0.0.4a0.tar", last modified: Mon Apr 29 10:57:01 2024, max compression
```

## Comparing `isparrowrecord-0.0.2a0.tar` & `isparrowrecord-0.0.4a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:55:26.556200 isparrowrecord-0.0.2a0/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-29 10:55:20.000000 isparrowrecord-0.0.2a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13773 2024-04-29 10:55:26.556200 isparrowrecord-0.0.2a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-29 10:55:20.000000 isparrowrecord-0.0.2a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-29 10:55:20.000000 isparrowrecord-0.0.2a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:55:26.556200 isparrowrecord-0.0.2a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:55:26.552200 isparrowrecord-0.0.2a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:55:26.552200 isparrowrecord-0.0.2a0/src/iSparrowRecord/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-29 10:55:20.000000 isparrowrecord-0.0.2a0/src/iSparrowRecord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11178 2024-04-29 10:55:20.000000 isparrowrecord-0.0.2a0/src/iSparrowRecord/audio_recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-29 10:55:20.000000 isparrowrecord-0.0.2a0/src/iSparrowRecord/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-29 10:55:20.000000 isparrowrecord-0.0.2a0/src/iSparrowRecord/set_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-29 10:55:20.000000 isparrowrecord-0.0.2a0/src/iSparrowRecord/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:55:26.556200 isparrowrecord-0.0.2a0/src/iSparrowRecord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13773 2024-04-29 10:55:26.000000 isparrowrecord-0.0.2a0/src/iSparrowRecord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-29 10:55:26.000000 isparrowrecord-0.0.2a0/src/iSparrowRecord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:55:26.000000 isparrowrecord-0.0.2a0/src/iSparrowRecord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-29 10:55:26.000000 isparrowrecord-0.0.2a0/src/iSparrowRecord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 10:55:26.000000 isparrowrecord-0.0.2a0/src/iSparrowRecord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:01.175740 isparrowrecord-0.0.4a0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-29 10:56:57.000000 isparrowrecord-0.0.4a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13773 2024-04-29 10:57:01.175740 isparrowrecord-0.0.4a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-29 10:56:57.000000 isparrowrecord-0.0.4a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-29 10:56:57.000000 isparrowrecord-0.0.4a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:57:01.175740 isparrowrecord-0.0.4a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:01.171740 isparrowrecord-0.0.4a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:01.171740 isparrowrecord-0.0.4a0/src/iSparrowRecord/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-29 10:56:57.000000 isparrowrecord-0.0.4a0/src/iSparrowRecord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11178 2024-04-29 10:56:57.000000 isparrowrecord-0.0.4a0/src/iSparrowRecord/audio_recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-29 10:56:57.000000 isparrowrecord-0.0.4a0/src/iSparrowRecord/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-29 10:56:57.000000 isparrowrecord-0.0.4a0/src/iSparrowRecord/set_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-29 10:56:57.000000 isparrowrecord-0.0.4a0/src/iSparrowRecord/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:01.175740 isparrowrecord-0.0.4a0/src/iSparrowRecord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13773 2024-04-29 10:57:01.000000 isparrowrecord-0.0.4a0/src/iSparrowRecord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-29 10:57:01.000000 isparrowrecord-0.0.4a0/src/iSparrowRecord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:57:01.000000 isparrowrecord-0.0.4a0/src/iSparrowRecord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-29 10:57:01.000000 isparrowrecord-0.0.4a0/src/iSparrowRecord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 10:57:01.000000 isparrowrecord-0.0.4a0/src/iSparrowRecord.egg-info/top_level.txt
```

### Comparing `isparrowrecord-0.0.2a0/LICENSE` & `isparrowrecord-0.0.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `isparrowrecord-0.0.2a0/PKG-INFO` & `isparrowrecord-0.0.4a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iSparrowRecord
-Version: 0.0.2a0
+Version: 0.0.4a0
 Summary: Audio Recording Facilities for the iSparrow package
 Author-email: Inga Ulusoy <inga.ulusoy@uni-heidelberg.de>, Harald Mack <harald.mack@iwr.uni-heidelberg.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `isparrowrecord-0.0.2a0/pyproject.toml` & `isparrowrecord-0.0.4a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `isparrowrecord-0.0.2a0/src/iSparrowRecord/audio_recording.py` & `isparrowrecord-0.0.4a0/src/iSparrowRecord/audio_recording.py`

 * *Files identical despite different names*

### Comparing `isparrowrecord-0.0.2a0/src/iSparrowRecord/runner.py` & `isparrowrecord-0.0.4a0/src/iSparrowRecord/runner.py`

 * *Files identical despite different names*

### Comparing `isparrowrecord-0.0.2a0/src/iSparrowRecord/set_up.py` & `isparrowrecord-0.0.4a0/src/iSparrowRecord/set_up.py`

 * *Files identical despite different names*

### Comparing `isparrowrecord-0.0.2a0/src/iSparrowRecord/utils.py` & `isparrowrecord-0.0.4a0/src/iSparrowRecord/utils.py`

 * *Files identical despite different names*

### Comparing `isparrowrecord-0.0.2a0/src/iSparrowRecord.egg-info/PKG-INFO` & `isparrowrecord-0.0.4a0/src/iSparrowRecord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iSparrowRecord
-Version: 0.0.2a0
+Version: 0.0.4a0
 Summary: Audio Recording Facilities for the iSparrow package
 Author-email: Inga Ulusoy <inga.ulusoy@uni-heidelberg.de>, Harald Mack <harald.mack@iwr.uni-heidelberg.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

