# Comparing `tmp/udi_interface-3.3.4.tar.gz` & `tmp/udi_interface-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udi_interface-3.3.4.tar", last modified: Thu Mar 28 00:00:48 2024, max compression
+gzip compressed data, was "udi_interface-3.3.5.tar", last modified: Mon Apr 29 12:43:15 2024, max compression
```

## Comparing `udi_interface-3.3.4.tar` & `udi_interface-3.3.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 admin     (1001) admin     (1001)        0 2024-03-28 00:00:48.856079 udi_interface-3.3.4/
--rwxrwxrwx   0 admin     (1001) admin     (1001)     1068 2023-07-05 13:05:47.000000 udi_interface-3.3.4/LICENSE
--rw-r--r--   0 admin     (1001) admin     (1001)     2418 2024-03-28 00:00:48.856211 udi_interface-3.3.4/PKG-INFO
--rwxrwxrwx   0 admin     (1001) admin     (1001)     1769 2023-07-05 13:05:47.000000 udi_interface-3.3.4/README.md
--rwxrwxrwx   0 admin     (1001) admin     (1001)      224 2024-03-28 00:00:48.856723 udi_interface-3.3.4/setup.cfg
--rwxrw-r--   0 admin     (1001) admin     (1001)     1514 2024-02-27 13:56:52.000000 udi_interface-3.3.4/setup.py
-drwxr-xr-x   0 admin     (1001) admin     (1001)        0 2024-03-28 00:00:48.854793 udi_interface-3.3.4/udi_interface/
--rwxrw-r--   0 admin     (1001) admin     (1001)     1629 2024-03-27 23:56:53.000000 udi_interface-3.3.4/udi_interface/__init__.py
--rwxrw-r--   0 admin     (1001) admin     (1001)     6362 2024-03-19 20:20:13.000000 udi_interface-3.3.4/udi_interface/custom.py
--rwxrw-r--   0 admin     (1001) admin     (1001)    65274 2024-03-20 20:32:06.000000 udi_interface-3.3.4/udi_interface/interface.py
--rw-r--r--   0 admin     (1001) admin     (1001)     2964 2024-01-25 19:13:19.000000 udi_interface-3.3.4/udi_interface/isy.py
--rwxrw-r--   0 admin     (1001) admin     (1001)     7126 2024-03-20 20:09:23.000000 udi_interface-3.3.4/udi_interface/node.py
--rwxrw-r--   0 admin     (1001) admin     (1001)     5514 2024-03-27 23:47:45.000000 udi_interface-3.3.4/udi_interface/oauth.py
--rwxr-xr-x   0 admin     (1001) admin     (1001)     3276 2023-12-22 20:03:53.000000 udi_interface-3.3.4/udi_interface/polylogger.py
--rw-r--r--   0 admin     (1001) admin     (1001)      873 2024-01-25 19:13:19.000000 udi_interface-3.3.4/udi_interface/startupdiag.py
--rwxrw-r--   0 admin     (1001) admin     (1001)     2345 2024-01-05 14:26:37.000000 udi_interface-3.3.4/udi_interface/test.py
--rwxr-xr-x   0 admin     (1001) admin     (1001)     4004 2024-01-25 19:13:19.000000 udi_interface-3.3.4/udi_interface/udi_interface.py
-drwxr-xr-x   0 admin     (1001) admin     (1001)        0 2024-03-28 00:00:48.855929 udi_interface-3.3.4/udi_interface.egg-info/
--rwxrwxrwx   0 admin     (1001) admin     (1001)     2418 2024-03-28 00:00:48.000000 udi_interface-3.3.4/udi_interface.egg-info/PKG-INFO
--rwxrwxrwx   0 admin     (1001) admin     (1001)      509 2024-03-28 00:00:48.000000 udi_interface-3.3.4/udi_interface.egg-info/SOURCES.txt
--rwxrwxrwx   0 admin     (1001) admin     (1001)        1 2024-03-28 00:00:48.000000 udi_interface-3.3.4/udi_interface.egg-info/dependency_links.txt
--rwxrwxrwx   0 admin     (1001) admin     (1001)        1 2023-07-05 20:51:23.000000 udi_interface-3.3.4/udi_interface.egg-info/not-zip-safe
--rwxrwxrwx   0 admin     (1001) admin     (1001)       92 2024-03-28 00:00:48.000000 udi_interface-3.3.4/udi_interface.egg-info/requires.txt
--rwxrwxrwx   0 admin     (1001) admin     (1001)       14 2024-03-28 00:00:48.000000 udi_interface-3.3.4/udi_interface.egg-info/top_level.txt
+drwxr-xr-x   0 admin     (1001) admin     (1001)        0 2024-04-29 12:43:15.318079 udi_interface-3.3.5/
+-rwxrwxrwx   0 admin     (1001) admin     (1001)     1068 2023-07-05 13:05:47.000000 udi_interface-3.3.5/LICENSE
+-rw-r--r--   0 admin     (1001) admin     (1001)     2418 2024-04-29 12:43:15.318219 udi_interface-3.3.5/PKG-INFO
+-rwxrwxrwx   0 admin     (1001) admin     (1001)     1769 2023-07-05 13:05:47.000000 udi_interface-3.3.5/README.md
+-rwxrwxrwx   0 admin     (1001) admin     (1001)      224 2024-04-29 12:43:15.318754 udi_interface-3.3.5/setup.cfg
+-rwxrw-r--   0 admin     (1001) admin     (1001)     1514 2024-02-27 13:56:52.000000 udi_interface-3.3.5/setup.py
+drwxr-xr-x   0 admin     (1001) admin     (1001)        0 2024-04-29 12:43:15.316623 udi_interface-3.3.5/udi_interface/
+-rwxrw-r--   0 admin     (1001) admin     (1001)     1630 2024-04-29 12:41:59.000000 udi_interface-3.3.5/udi_interface/__init__.py
+-rwxrw-r--   0 admin     (1001) admin     (1001)     6362 2024-03-19 20:20:13.000000 udi_interface-3.3.5/udi_interface/custom.py
+-rwxrw-r--   0 admin     (1001) admin     (1001)    65274 2024-03-20 20:32:06.000000 udi_interface-3.3.5/udi_interface/interface.py
+-rw-r--r--   0 admin     (1001) admin     (1001)     2964 2024-01-25 19:13:19.000000 udi_interface-3.3.5/udi_interface/isy.py
+-rwxrw-r--   0 admin     (1001) admin     (1001)     7126 2024-03-20 20:09:23.000000 udi_interface-3.3.5/udi_interface/node.py
+-rwxrw-r--   0 admin     (1001) admin     (1001)     6804 2024-04-29 12:38:02.000000 udi_interface-3.3.5/udi_interface/oauth.py
+-rwxr-xr-x   0 admin     (1001) admin     (1001)     3276 2023-12-22 20:03:53.000000 udi_interface-3.3.5/udi_interface/polylogger.py
+-rw-r--r--   0 admin     (1001) admin     (1001)      873 2024-01-25 19:13:19.000000 udi_interface-3.3.5/udi_interface/startupdiag.py
+-rwxrw-r--   0 admin     (1001) admin     (1001)     2345 2024-01-05 14:26:37.000000 udi_interface-3.3.5/udi_interface/test.py
+-rwxr-xr-x   0 admin     (1001) admin     (1001)     4004 2024-01-25 19:13:19.000000 udi_interface-3.3.5/udi_interface/udi_interface.py
+drwxr-xr-x   0 admin     (1001) admin     (1001)        0 2024-04-29 12:43:15.317916 udi_interface-3.3.5/udi_interface.egg-info/
+-rwxrwxrwx   0 admin     (1001) admin     (1001)     2418 2024-04-29 12:43:15.000000 udi_interface-3.3.5/udi_interface.egg-info/PKG-INFO
+-rwxrwxrwx   0 admin     (1001) admin     (1001)      509 2024-04-29 12:43:15.000000 udi_interface-3.3.5/udi_interface.egg-info/SOURCES.txt
+-rwxrwxrwx   0 admin     (1001) admin     (1001)        1 2024-04-29 12:43:15.000000 udi_interface-3.3.5/udi_interface.egg-info/dependency_links.txt
+-rwxrwxrwx   0 admin     (1001) admin     (1001)        1 2023-07-05 20:51:23.000000 udi_interface-3.3.5/udi_interface.egg-info/not-zip-safe
+-rwxrwxrwx   0 admin     (1001) admin     (1001)       92 2024-04-29 12:43:15.000000 udi_interface-3.3.5/udi_interface.egg-info/requires.txt
+-rwxrwxrwx   0 admin     (1001) admin     (1001)       14 2024-04-29 12:43:15.000000 udi_interface-3.3.5/udi_interface.egg-info/top_level.txt
```

### Comparing `udi_interface-3.3.4/LICENSE` & `udi_interface-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.4/PKG-INFO` & `udi_interface-3.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udi_interface
-Version: 3.3.4
+Version: 3.3.5
 Summary: UDI Python Interface for Polyglot version 3
 Home-page: https://github.com/UniversalDevicesInc/udi_python_interface
 Author: Universal Devices Inc.
 Author-email: bpaauwe@yahoo.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `udi_interface-3.3.4/README.md` & `udi_interface-3.3.5/README.md`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.4/setup.py` & `udi_interface-3.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.4/udi_interface/__init__.py` & `udi_interface-3.3.5/udi_interface/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '3.3.4'
+__version__ = '3.3.5'
 __description__ = 'UDI Python Interface for Polyglot version 3'
 __url__ = 'https://github.com/UniversalDevicesInc/udi_python_interface'
 __author__ = 'Universal Devices Inc.'
 __authoremail__ = 'bpaauwe@yahoo.com'
 __license__ = 'MIT'
 
 import traceback
@@ -32,8 +32,8 @@
     LOGGER.info('UDI interface initialized')
 
     LOGGER.info('{} {} Starting...'.format(__description__, __version__))
 except Exception as error:
     # If logger was not able to start, at least write a crash.log file in the current directory
     writeCrashInfo(traceback.format_exc())
     # Will work if polylogger was able to initialize
-    LOGGER.error('UDI interface initializaton failure: {}'.format(traceback.format_exc()))
+    LOGGER.error('UDI interface initialization failure: {}'.format(traceback.format_exc()))
```

### Comparing `udi_interface-3.3.4/udi_interface/custom.py` & `udi_interface-3.3.5/udi_interface/custom.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.4/udi_interface/interface.py` & `udi_interface-3.3.5/udi_interface/interface.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.4/udi_interface/isy.py` & `udi_interface-3.3.5/udi_interface/isy.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.4/udi_interface/node.py` & `udi_interface-3.3.5/udi_interface/node.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.4/udi_interface/polylogger.py` & `udi_interface-3.3.5/udi_interface/polylogger.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.4/udi_interface/startupdiag.py` & `udi_interface-3.3.5/udi_interface/startupdiag.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.4/udi_interface/test.py` & `udi_interface-3.3.5/udi_interface/test.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.4/udi_interface/udi_interface.py` & `udi_interface-3.3.5/udi_interface/udi_interface.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.4/udi_interface.egg-info/PKG-INFO` & `udi_interface-3.3.5/udi_interface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udi-interface
-Version: 3.3.4
+Version: 3.3.5
 Summary: UDI Python Interface for Polyglot version 3
 Home-page: https://github.com/UniversalDevicesInc/udi_python_interface
 Author: Universal Devices Inc.
 Author-email: bpaauwe@yahoo.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

