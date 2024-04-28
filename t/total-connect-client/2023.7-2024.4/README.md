# Comparing `tmp/total_connect_client-2023.7.tar.gz` & `tmp/total_connect_client-2024.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "total_connect_client-2023.7.tar", last modified: Tue Jul  4 15:10:41 2023, max compression
+gzip compressed data, was "total_connect_client-2024.4.tar", last modified: Sun Apr 28 23:00:17 2024, max compression
```

## Comparing `total_connect_client-2023.7.tar` & `total_connect_client-2024.4.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-04 15:10:41.722420 total_connect_client-2023.7/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1075 2023-02-24 21:24:49.000000 total_connect_client-2023.7/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7505 2023-07-04 15:10:41.722420 total_connect_client-2023.7/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6893 2023-06-25 20:47:34.000000 total_connect_client-2023.7/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3229 2023-07-04 15:10:00.000000 total_connect_client-2023.7/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-07-04 15:10:41.722420 total_connect_client-2023.7/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-04 15:10:41.721420 total_connect_client-2023.7/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7368 2023-06-29 00:24:30.000000 total_connect_client-2023.7/tests/test_client_arm_disarm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2774 2023-02-24 21:24:49.000000 total_connect_client-2023.7/tests/test_client_authenticate.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2705 2023-02-24 21:24:49.000000 total_connect_client-2023.7/tests/test_client_get_panel_meta_data.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3445 2023-06-29 00:24:30.000000 total_connect_client-2023.7/tests/test_client_init.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2481 2023-04-29 22:02:21.000000 total_connect_client-2023.7/tests/test_client_misc.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6616 2023-06-29 00:24:30.000000 total_connect_client-2023.7/tests/test_client_request.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1867 2023-02-24 21:24:49.000000 total_connect_client-2023.7/tests/test_client_validate_usercode.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3332 2023-06-29 00:24:58.000000 total_connect_client-2023.7/tests/test_client_zone_bypass.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      467 2023-02-24 21:24:49.000000 total_connect_client-2023.7/tests/test_device.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7373 2023-04-29 21:52:35.000000 total_connect_client-2023.7/tests/test_location.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1996 2023-06-28 23:58:46.000000 total_connect_client-2023.7/tests/test_location_arm_disarm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4071 2023-06-29 00:24:30.000000 total_connect_client-2023.7/tests/test_partition.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1299 2023-02-24 21:24:49.000000 total_connect_client-2023.7/tests/test_user.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14210 2023-06-29 00:24:30.000000 total_connect_client-2023.7/tests/test_zone.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-04 15:10:41.722420 total_connect_client-2023.7/total_connect_client/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      699 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      516 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/__main__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      823 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/arm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1219 2023-06-24 19:33:36.000000 total_connect_client-2023.7/total_connect_client/bypass_all.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15022 2023-02-24 22:00:19.000000 total_connect_client-2023.7/total_connect_client/client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5608 2023-05-06 15:50:27.000000 total_connect_client-2023.7/total_connect_client/const.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1218 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/device.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      600 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/disarm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1370 2023-02-24 21:59:19.000000 total_connect_client-2023.7/total_connect_client/exceptions.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-04 15:10:41.722420 total_connect_client-2023.7/total_connect_client/live/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      762 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/live/auto_bypass.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1347 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/live/zwave.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15559 2023-06-24 19:33:41.000000 total_connect_client-2023.7/total_connect_client/location.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2236 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/partition.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      889 2023-05-06 16:48:15.000000 total_connect_client-2023.7/total_connect_client/sync.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2095 2023-02-24 21:24:49.000000 total_connect_client-2023.7/total_connect_client/user.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9604 2023-06-22 02:49:55.000000 total_connect_client-2023.7/total_connect_client/zone.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-04 15:10:41.722420 total_connect_client-2023.7/total_connect_client.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7505 2023-07-04 15:10:41.000000 total_connect_client-2023.7/total_connect_client.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1168 2023-07-04 15:10:41.000000 total_connect_client-2023.7/total_connect_client.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-04 15:10:41.000000 total_connect_client-2023.7/total_connect_client.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       12 2023-07-04 15:10:41.000000 total_connect_client-2023.7/total_connect_client.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       21 2023-07-04 15:10:41.000000 total_connect_client-2023.7/total_connect_client.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-28 23:00:17.119065 total_connect_client-2024.4/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1075 2023-02-24 21:24:49.000000 total_connect_client-2024.4/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7532 2024-04-28 23:00:17.119065 total_connect_client-2024.4/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6893 2023-11-30 02:02:31.000000 total_connect_client-2024.4/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3275 2024-04-28 23:00:07.000000 total_connect_client-2024.4/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-04-28 23:00:17.119065 total_connect_client-2024.4/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-28 23:00:17.118065 total_connect_client-2024.4/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7368 2023-06-29 00:24:30.000000 total_connect_client-2024.4/tests/test_client_arm_disarm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2774 2023-02-24 21:24:49.000000 total_connect_client-2024.4/tests/test_client_authenticate.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2705 2023-02-24 21:24:49.000000 total_connect_client-2024.4/tests/test_client_get_panel_meta_data.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3445 2023-06-29 00:24:30.000000 total_connect_client-2024.4/tests/test_client_init.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2481 2023-04-29 22:02:21.000000 total_connect_client-2024.4/tests/test_client_misc.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6616 2023-06-29 00:24:30.000000 total_connect_client-2024.4/tests/test_client_request.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1867 2023-02-24 21:24:49.000000 total_connect_client-2024.4/tests/test_client_validate_usercode.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3332 2023-11-30 02:02:31.000000 total_connect_client-2024.4/tests/test_client_zone_bypass.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      467 2023-02-24 21:24:49.000000 total_connect_client-2024.4/tests/test_device.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8037 2024-04-28 22:08:42.000000 total_connect_client-2024.4/tests/test_location.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1996 2023-11-30 02:02:31.000000 total_connect_client-2024.4/tests/test_location_arm_disarm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4071 2023-06-29 00:24:30.000000 total_connect_client-2024.4/tests/test_partition.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1299 2023-02-24 21:24:49.000000 total_connect_client-2024.4/tests/test_user.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14210 2023-11-30 02:02:31.000000 total_connect_client-2024.4/tests/test_zone.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-28 23:00:17.118065 total_connect_client-2024.4/total_connect_client/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      699 2023-02-24 21:24:49.000000 total_connect_client-2024.4/total_connect_client/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      516 2023-02-24 21:24:49.000000 total_connect_client-2024.4/total_connect_client/__main__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      823 2023-02-24 21:24:49.000000 total_connect_client-2024.4/total_connect_client/arm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1219 2023-11-30 02:02:31.000000 total_connect_client-2024.4/total_connect_client/bypass_all.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15022 2023-02-24 22:00:19.000000 total_connect_client-2024.4/total_connect_client/client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5732 2024-04-28 22:07:55.000000 total_connect_client-2024.4/total_connect_client/const.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2951 2023-12-02 01:55:12.000000 total_connect_client-2024.4/total_connect_client/device.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      600 2023-02-24 21:24:49.000000 total_connect_client-2024.4/total_connect_client/disarm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1370 2023-02-24 21:59:19.000000 total_connect_client-2024.4/total_connect_client/exceptions.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-28 23:00:17.119065 total_connect_client-2024.4/total_connect_client/live/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      762 2023-02-24 21:24:49.000000 total_connect_client-2024.4/total_connect_client/live/auto_bypass.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4081 2023-12-02 02:37:34.000000 total_connect_client-2024.4/total_connect_client/live/experimental.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1710 2023-11-30 02:02:31.000000 total_connect_client-2024.4/total_connect_client/live/zwave.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    18745 2023-12-02 02:40:27.000000 total_connect_client-2024.4/total_connect_client/location.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2236 2023-02-24 21:24:49.000000 total_connect_client-2024.4/total_connect_client/partition.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      889 2023-05-06 16:48:15.000000 total_connect_client-2024.4/total_connect_client/sync.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2095 2023-02-24 21:24:49.000000 total_connect_client-2024.4/total_connect_client/user.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9604 2023-11-30 02:02:31.000000 total_connect_client-2024.4/total_connect_client/zone.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-28 23:00:17.119065 total_connect_client-2024.4/total_connect_client.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7532 2024-04-28 23:00:17.000000 total_connect_client-2024.4/total_connect_client.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1210 2024-04-28 23:00:17.000000 total_connect_client-2024.4/total_connect_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-04-28 23:00:17.000000 total_connect_client-2024.4/total_connect_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       12 2024-04-28 23:00:17.000000 total_connect_client-2024.4/total_connect_client.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       21 2024-04-28 23:00:17.000000 total_connect_client-2024.4/total_connect_client.egg-info/top_level.txt
```

### Comparing `total_connect_client-2023.7/LICENSE` & `total_connect_client-2024.4/LICENSE`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/PKG-INFO` & `total_connect_client-2024.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: total_connect_client
-Version: 2023.7
+Version: 2024.4
 Summary: Interact with Total Connect 2 alarm systems
 Author-email: "Craig J. Midwinter" <craig.j.midwinter@gmail.com>
 Project-URL: Homepage, https://github.com/craigjmidwinter/total-connect-client
 Project-URL: Bug Tracker, https://github.com/craigjmidwinter/total-connect-client/issues
 Keywords: alarm,TotalConnect
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: zeep>=4.2.1
 
 # Total-Connect-Client
 Total-Connect-Client is a python client for interacting with the [TotalConnect2](https://totalconnect2.com) alarm system.
 
 Started by @craigjmidwinter to add alarm support for his personal HomeAssistant set-up, with later contributions from others.
 
 To use with Home Assistant, follow the instructions to set up [Total Connect](https://www.home-assistant.io/integrations/totalconnect/).
```

### Comparing `total_connect_client-2023.7/README.md` & `total_connect_client-2024.4/README.md`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/pyproject.toml` & `total_connect_client-2024.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name="total_connect_client"
-version="2023.7"
+version="2024.4"
 authors = [
   { name="Craig J. Midwinter", email="craig.j.midwinter@gmail.com" },
 ]
 description="Interact with Total Connect 2 alarm systems"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords=["alarm", "TotalConnect"]
-dependencies=["zeep>=4.1.0"]
+dependencies=["zeep>=4.2.1"]
 
 [project.urls]
 "Homepage" = "https://github.com/craigjmidwinter/total-connect-client"
 "Bug Tracker" = "https://github.com/craigjmidwinter/total-connect-client/issues"
 
 [tool.coverage.run]
 omit = [
@@ -33,32 +33,34 @@
 [tool.pylint."messages control"]
 disable = ["use-symbolic-message-instead", "too-few-public-methods", "too-many-instance-attributes", "logging-fstring-interpolation", "missing-function-docstring", "missing-class-docstring", "protected-access", "line-too-long", "duplicate-code"]
 
 [tool.tox]
 legacy_tox_ini = """
 
    [tox]
+    requires = 
+      tox>=4
+      virtualenv>=20.26
+
     env_list = 
         build
         lint
-        py311
-        py310
-        py39
+        py{39,310,311,312}
 
     #skip_missing_interpreters = True
 
     [testenv]
     setenv =
         LANG=en_US.UTF-8
         PYTHONPATH = {toxinidir}
-    commands = 
-        pytest --timeout=30 --cov=total_connect_client --cov-report term-missing -p no:sugar {posargs}
     deps = 
         -r{toxinidir}/requirements.txt
         -r{toxinidir}/requirements_test.txt
+    commands = 
+        pytest tests --timeout=30 --cov=total_connect_client --cov-report term-missing -p no:sugar {posargs}
 
     [testenv:lint]
     deps = 
         -r{toxinidir}/requirements.txt
         -r{toxinidir}/requirements_test.txt
     ignore_errors = True
     commands =
```

### Comparing `total_connect_client-2023.7/tests/test_client_arm_disarm.py` & `total_connect_client-2024.4/tests/test_client_arm_disarm.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/tests/test_client_authenticate.py` & `total_connect_client-2024.4/tests/test_client_authenticate.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/tests/test_client_get_panel_meta_data.py` & `total_connect_client-2024.4/tests/test_client_get_panel_meta_data.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/tests/test_client_init.py` & `total_connect_client-2024.4/tests/test_client_init.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/tests/test_client_misc.py` & `total_connect_client-2024.4/tests/test_client_misc.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/tests/test_client_request.py` & `total_connect_client-2024.4/tests/test_client_request.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/tests/test_client_validate_usercode.py` & `total_connect_client-2024.4/tests/test_client_validate_usercode.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/tests/test_client_zone_bypass.py` & `total_connect_client-2024.4/tests/test_client_zone_bypass.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/tests/test_location.py` & `total_connect_client-2024.4/tests/test_location.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 import unittest
 from copy import deepcopy
 from unittest.mock import Mock, patch
 
 import pytest
 from const import (
     LOCATION_INFO_BASIC_NORMAL,
+    METADATA_DISARMED,
     METADATA_DISARMED_LOW_BATTERY,
     RESPONSE_DISARMED,
     RESPONSE_GET_ZONE_DETAILS_SUCCESS,
 )
 
+from total_connect_client.const import ArmingState
 from total_connect_client.exceptions import PartialResponseError, TotalConnectError
 from total_connect_client.location import DEFAULT_USERCODE, TotalConnectLocation
 
 
 class TestTotalConnectLocation(unittest.TestCase):
     """Test TotalConnectLocation."""
 
@@ -169,7 +171,25 @@
         assert mock_client.validate_usercode.call_count == 1
 
         # now set it with a valid code
         mock_client.validate_usercode.return_value = True
         assert loc.set_usercode("1234") is True
         assert loc.usercode == "1234"
         assert mock_client.validate_usercode.call_count == 2
+
+
+def tests_update_status():
+    """Test location._update_status()."""
+    location = TotalConnectLocation(LOCATION_INFO_BASIC_NORMAL, Mock())
+
+    # known arming state should not produce an error
+    response = {
+        "PanelMetadataAndStatus": METADATA_DISARMED,
+        "ArmingState": ArmingState.DISARMED,
+    }
+    location._update_status(response)
+    assert location.arming_state == ArmingState.DISARMED
+
+    # unknown arming state should produce an error
+    with pytest.raises(TotalConnectError):
+        response["ArmingState"] = 99999
+        location._update_status(response)
```

### Comparing `total_connect_client-2023.7/tests/test_location_arm_disarm.py` & `total_connect_client-2024.4/tests/test_location_arm_disarm.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/tests/test_partition.py` & `total_connect_client-2024.4/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/tests/test_user.py` & `total_connect_client-2024.4/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/tests/test_zone.py` & `total_connect_client-2024.4/tests/test_zone.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/total_connect_client/__init__.py` & `total_connect_client-2024.4/total_connect_client/__init__.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/total_connect_client/__main__.py` & `total_connect_client-2024.4/total_connect_client/__main__.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/total_connect_client/arm.py` & `total_connect_client-2024.4/total_connect_client/arm.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/total_connect_client/bypass_all.py` & `total_connect_client-2024.4/total_connect_client/bypass_all.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/total_connect_client/client.py` & `total_connect_client-2024.4/total_connect_client/client.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/total_connect_client/const.py` & `total_connect_client-2024.4/total_connect_client/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     ARMED_STAY_NIGHT_INSTANT_PROA7 = 10220  # issue #177
     ARMED_STAY_NIGHT_INSTANT_BYPASS_PROA7 = 10221  # issue #177
     ARMED_CUSTOM_BYPASS = 10223
 
     ALARMING = 10207
     ALARMING_FIRE_SMOKE = 10212
     ALARMING_CARBON_MONOXIDE = 10213
+    ALARMING_CARBON_MONOXIDE_PROA7 = 10215
 
     ARMING = 10307
     DISARMING = 10308
 
     def is_arming(self):
         """Return true if the system is in the process of arming."""
         return self == ArmingState.ARMING
@@ -121,15 +122,18 @@
 
     def is_triggered_fire(self):
         """Return True if the system is triggered for fire or smoke."""
         return self == ArmingState.ALARMING_FIRE_SMOKE
 
     def is_triggered_gas(self):
         """Return True if the system is triggered for carbon monoxide."""
-        return self == ArmingState.ALARMING_CARBON_MONOXIDE
+        return self in (
+            ArmingState.ALARMING_CARBON_MONOXIDE,
+            ArmingState.ALARMING_CARBON_MONOXIDE_PROA7,
+        )
 
     def is_triggered(self):
         """Return True if the system is triggered in any way."""
         return (
             self.is_triggered_fire()
             or self.is_triggered_gas()
             or self.is_triggered_police()
```

### Comparing `total_connect_client-2023.7/total_connect_client/disarm.py` & `total_connect_client-2024.4/total_connect_client/disarm.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/total_connect_client/exceptions.py` & `total_connect_client-2024.4/total_connect_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/total_connect_client/live/auto_bypass.py` & `total_connect_client-2024.4/total_connect_client/live/auto_bypass.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/total_connect_client/live/zwave.py` & `total_connect_client-2024.4/total_connect_client/live/zwave.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,41 +20,67 @@
 DEVICE_ID = sys.argv[4]
 TYPE = sys.argv[5]
 LOCATION = sys.argv[6]
 
 TC = TotalConnectClient(USERNAME, PASSWORD)
 
 print("\n\n\nGetAutomationDeviceStatus\n\n\n")
-result = TC.request(f"GetAutomationDeviceStatus(self.token, {AUTOMATION_DEVICE})")
+try:
+    result = TC.request(
+        "GetAutomationDeviceStatus", 
+        (TC.token, AUTOMATION_DEVICE)
+    )
+    pprint(result)
+except Exception as err:
+    print(err)
 
-pprint(result)
 
 
 print("\n\n\nGetAutomationDeviceStatusExV1\n\n\n")
-result = TC.request(f"GetAutomationDeviceStatusExV1(self.token, {AUTOMATION_DEVICE})")
-
-pprint(result)
+try:
+    result = TC.request(
+        "GetAutomationDeviceStatusExV1",
+        (TC.token, AUTOMATION_DEVICE)
+    )
+    pprint(result)
+except Exception as err:
+    print(err)
 
 
 print("\n\n\nGetAllAutomationDeviceStatusExV1\n\n\n")
-result = TC.request(
-    f"GetAllAutomationDeviceStatusExV1(self.token, {AUTOMATION_DEVICE})"
-)
-
-pprint(result)
-
+try:
+    result = TC.request(
+        "GetAllAutomationDeviceStatusExV1",
+        (TC.token, AUTOMATION_DEVICE)
+    )
+    pprint(result)
+except Exception as err:
+    print(err)
 
 print("\n\n\nGetDeviceStatus\n\n\n")
 
 a = []
 a.append(DEVICE_ID)
 a.append(TYPE)
 b = []
 b.append(a)
 
-result = TC.request(f"GetDeviceStatus(self.token, {LOCATION}, {b})")
-
+try:
+    result = TC.request(
+        "GetDeviceStatus",
+        (TC.token, LOCATION, b)
+    )
+    pprint(result)
+except Exception as err:
+    print(err)
 
 print("\n\n\nGetAutomationLocks\n\n\n")
-result = TC.request(f"GetAutomationLocks(self.token, {AUTOMATION_DEVICE}, {DEVICE_ID})")
 
-pprint(result)
+try:
+    result = TC.request(
+        "GetAutomationLocks",
+        (TC.token, AUTOMATION_DEVICE, DEVICE_ID)
+    )
+    pprint(result)
+except Exception as err:
+    print(err)
+
```

### Comparing `total_connect_client-2023.7/total_connect_client/location.py` & `total_connect_client-2024.4/total_connect_client/location.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Total Connect Location."""
 
 import logging
 import typing
 
 from .const import PROJECT_URL, ArmingState, ArmType, _ResultCode
 from .device import TotalConnectDevice
-from .exceptions import (FeatureNotSupportedError, PartialResponseError,
-                         TotalConnectError)
+from .exceptions import (
+    FeatureNotSupportedError,
+    PartialResponseError,
+    TotalConnectError,
+)
 from .partition import TotalConnectPartition
 from .zone import TotalConnectZone
 
 DEFAULT_USERCODE = "-1"
 
 LOGGER = logging.getLogger(__name__)
 
@@ -77,49 +80,63 @@
             zones += str(status)
 
         return data + devices + partitions + zones
 
     def get_panel_meta_data(self):
         """Get all meta data about the alarm panel."""
         # see https://rs.alarmnet.com/TC21api/tc2.asmx?op=GetPanelMetaDataAndFullStatus
-        result = self.parent.request("GetPanelMetaDataAndFullStatusEx_V2", (
-            # to speed this up we could replace the first zero with
-            # the most recent ConfigurationSequenceNumber and the
-            # second with LastUpdatedTimestampTicks
-            self.parent.token, self.location_id, 0, 0, self._partition_list
-        ))
+        result = self.parent.request(
+            "GetPanelMetaDataAndFullStatusEx_V2",
+            (
+                # to speed this up we could replace the first zero with
+                # the most recent ConfigurationSequenceNumber and the
+                # second with LastUpdatedTimestampTicks
+                self.parent.token,
+                self.location_id,
+                0,
+                0,
+                self._partition_list,
+            ),
+        )
         self.parent.raise_for_resultcode(result)
 
         self._update_status(result)
         self._update_partitions(result)
         self._update_zones(result)
 
     def get_zone_details(self):
         """Get Zone details."""
-        result = self.parent.request("GetZonesListInStateEx_V1", (
-            # 0 is the ListIdentifierID, whatever that might be
-            self.parent.token, self.location_id, self._partition_list, 0
-        ))
+        result = self.parent.request(
+            "GetZonesListInStateEx_V1",
+            (
+                # 0 is the ListIdentifierID, whatever that might be
+                self.parent.token,
+                self.location_id,
+                self._partition_list,
+                0,
+            ),
+        )
 
         try:
             self.parent.raise_for_resultcode(result)
             self._update_zone_details(result)
         except FeatureNotSupportedError:
             LOGGER.warning(
                 "getting Zone Details is a feature not supported by "
                 "your Total Connect account or hardware"
             )
 
     def get_partition_details(self):
         """Get partition details for this location."""
         # see https://rs.alarmnet.com/TC21api/tc2.asmx?op=GetPartitionsDetails
 
-        result = self.parent.request("GetPartitionsDetails", (
-            self.parent.token, self.location_id, self.security_device_id
-        ))
+        result = self.parent.request(
+            "GetPartitionsDetails",
+            (self.parent.token, self.location_id, self.security_device_id),
+        )
         try:
             self.parent.raise_for_resultcode(result)
         except TotalConnectError:
             LOGGER.error(
                 f"Could not get partition details for "
                 f"device {self.security_device_id} at "
                 f"location {self.location_id}."
@@ -175,62 +192,89 @@
 
     def arm(self, arm_type, partition_id=None):
         """Arm the given partition. If no partition is given, arm all partitions."""
         # see https://rs.alarmnet.com/TC21api/tc2.asmx?op=ArmSecuritySystemPartitionsV1
         assert isinstance(arm_type, ArmType)
         partition_list = self._build_partition_list(partition_id)
 
-        result = self.parent.request("ArmSecuritySystemPartitionsV1", (
-            self.parent.token, self.location_id, self.security_device_id,
-            arm_type.value, self.usercode, partition_list
-        ))
+        result = self.parent.request(
+            "ArmSecuritySystemPartitionsV1",
+            (
+                self.parent.token,
+                self.location_id,
+                self.security_device_id,
+                arm_type.value,
+                self.usercode,
+                partition_list,
+            ),
+        )
         if _ResultCode.from_response(result) == _ResultCode.COMMAND_FAILED:
             LOGGER.warning("could not arm system; is a zone faulted?")
         self.parent.raise_for_resultcode(result)
         LOGGER.info(
             f"ARMED({arm_type}) partitions {partition_list} at {self.location_id}"
         )
 
     def disarm(self, partition_id=None):
         """Disarm the system."""
         # if no partition is given, disarm all partitions
         # see https://rs.alarmnet.com/TC21api/tc2.asmx?op=ArmSecuritySystemPartitionsV1
         partition_list = self._build_partition_list(partition_id)
 
-        result = self.parent.request("DisarmSecuritySystemPartitionsV1", (
-            self.parent.token, self.location_id, self.security_device_id,
-            self.usercode, partition_list
-        ))
+        result = self.parent.request(
+            "DisarmSecuritySystemPartitionsV1",
+            (
+                self.parent.token,
+                self.location_id,
+                self.security_device_id,
+                self.usercode,
+                partition_list,
+            ),
+        )
         self.parent.raise_for_resultcode(result)
         LOGGER.info(f"DISARMED partitions {partition_list} at {self.location_id}")
 
     def zone_bypass(self, zone_id: int):
         """Bypass a zone."""
-        result = self.parent.request("Bypass", (
-            self.parent.token, self.location_id, self.security_device_id, zone_id, self.usercode
-        ))
+        result = self.parent.request(
+            "Bypass",
+            (
+                self.parent.token,
+                self.location_id,
+                self.security_device_id,
+                zone_id,
+                self.usercode,
+            ),
+        )
         self.parent.raise_for_resultcode(result)
         LOGGER.info(f"BYPASSED {zone_id} at {self.location_id}")
         self.zones[zone_id]._mark_as_bypassed()
 
     def zone_bypass_all(self):
         """Bypass all faulted zones."""
         faulted_zones = []
         for zone_id, zone in self.zones.items():
             if zone.is_faulted():
                 faulted_zones.append(zone_id)
 
         if faulted_zones:
             zone_list = {"int": faulted_zones}
 
-            result = self.parent.request("BypassAll", (
-                self.parent.token, self.location_id, self.security_device_id, zone_list, self.usercode
-            ))
+            result = self.parent.request(
+                "BypassAll",
+                (
+                    self.parent.token,
+                    self.location_id,
+                    self.security_device_id,
+                    zone_list,
+                    self.usercode,
+                ),
+            )
             self.parent.raise_for_resultcode(result)
-            LOGGER.info(f"BYPASSED all zones at location {self.location_id}")          
+            LOGGER.info(f"BYPASSED all zones at location {self.location_id}")
 
     def clear_bypass(self):
         """Clear all bypassed zones."""
         self.disarm()
 
     def zone_status(self, zone_id: int):
         """Get status of a zone."""
@@ -243,29 +287,37 @@
         """NOT OPERATIONAL YET.
         Arm custom the system.  Return true if successful.
         """
         zones_list = {}
         zones_list[0] = {"ZoneID": "12", "ByPass": False, "ZoneStatus": 0}
         settings = {"ArmMode": "1", "ArmDelay": "5", "ZonesList": zones_list}
 
-        result = self.parent.request("CustomArmSecuritySystem", (
-            self.parent.token, self.location_id, self.security_device_id,
-            arm_type.value, self.usercode, settings
-        ))
+        result = self.parent.request(
+            "CustomArmSecuritySystem",
+            (
+                self.parent.token,
+                self.location_id,
+                self.security_device_id,
+                arm_type.value,
+                self.usercode,
+                settings,
+            ),
+        )
         self.parent.raise_for_resultcode(result)
         # TODO: returning the raw result is not right
         return result
 
     def get_custom_arm_settings(self):
         """NOT OPERATIONAL YET.
         Get custom arm settings.
         """
-        result = self.parent.request("GetCustomArmSettings", (
-            self.parent.token, self.location_id, self.security_device_id
-        ))
+        result = self.parent.request(
+            "GetCustomArmSettings",
+            (self.parent.token, self.location_id, self.security_device_id),
+        )
         self.parent.raise_for_resultcode(result)
         # TODO: returning the raw result is not right
         return result
 
     def _update_zone_details(self, result):
         """
         Update from GetZonesListInStateEx_V1.
@@ -273,15 +325,17 @@
         ZoneStatusInfoWithPartitionId provides additional info for setting up zones.
         If we used TotalConnectZone._update() it would overwrite missing data with None.
         """
         zone_info = ((result.get("ZoneStatus") or {}).get("Zones") or {}).get(
             "ZoneStatusInfoWithPartitionId"
         )
         if not zone_info:
-            LOGGER.warning("No zones found when starting TotalConnect. Try to sync your panel using the TotalConnect app or website.")
+            LOGGER.warning(
+                "No zones found when starting TotalConnect. Try to sync your panel using the TotalConnect app or website."
+            )
             LOGGER.debug(f"_update_zone_details result: {result}")
         else:
             for zonedata in zone_info:
                 self.zones[zonedata["ZoneID"]] = TotalConnectZone(zonedata, self)
 
     def _update_status(self, result):
         """Update from result."""
@@ -300,21 +354,23 @@
             raise PartialResponseError("no ArmingState", result)
         try:
             self.arming_state = ArmingState(astate)
         except ValueError:
             LOGGER.error(
                 f"unknown location ArmingState {astate} in {result}: please report at {PROJECT_URL}/issues"
             )
-            raise TotalConnectError(f"unknown location ArmingState {astate} in {result}") from None
+            raise TotalConnectError(
+                f"unknown location ArmingState {astate} in {result}"
+            ) from None
 
     def _update_partitions(self, result):
         """Update partition info from Partitions."""
-        pinfo = ((result.get("PanelMetadataAndStatus") or {}).get("Partitions") or {}).get(
-            "PartitionInfo"
-        )
+        pinfo = (
+            (result.get("PanelMetadataAndStatus") or {}).get("Partitions") or {}
+        ).get("PartitionInfo")
         if not pinfo:
             raise PartialResponseError("no PartitionInfo", result)
 
         # loop through partitions and update
         # NOTE: do not use keys because they don't line up with PartitionID
         for partition in pinfo:
             if "PartitionID" not in partition:
@@ -326,15 +382,17 @@
                 LOGGER.warning(f"Update provided for unknown partion {partition_id}")
 
     def _update_zones(self, result):
         """Update zone info from ZoneInfo or ZoneInfoEx."""
 
         data = (result.get("PanelMetadataAndStatus") or {}).get("Zones")
         if not data:
-            LOGGER.error("no zones found: sync your panel using TotalConnect app or website")
+            LOGGER.error(
+                "no zones found: sync your panel using TotalConnect app or website"
+            )
             # PartialResponseError would mean this is retryable without fixing
             # anything, and this needs fixing
             raise TotalConnectError("no zones found: panel sync required")
 
         zone_info = data.get("ZoneInfoEx") or data.get("ZoneInfo")
         if not zone_info:
             raise PartialResponseError("no ZoneInfoEx or ZoneInfo", result)
@@ -345,41 +403,115 @@
             zone = self.zones.get(zid)
             if zone:
                 zone._update(zonedata)
             else:
                 zone = TotalConnectZone(zonedata, self)
                 self.zones[zid] = zone
 
-            if zone.is_low_battery() and zone.can_be_bypassed and self.auto_bypass_low_battery:
+            if (
+                zone.is_low_battery()
+                and zone.can_be_bypassed
+                and self.auto_bypass_low_battery
+            ):
                 self.zone_bypass(zid)
 
     def sync_panel(self):
         """Syncronize the panel with the TotalConnect server."""
         result = self.parent.request(
             "SynchronizeSecurityPanel",
-            (self.parent.token, None, self.usercode, self.location_id, False)
+            (self.parent.token, None, self.usercode, self.location_id, False),
         )
         self.parent.raise_for_resultcode(result)
         self._sync_job_id = result.get("JobID")
         # Successful request so assume state is in progress
         self._sync_job_state = 1
         LOGGER.info(f"Started sync of panel for location {self.location_id}")
 
     def get_sync_status(self):
         """Get panel sync status from the TotalConnect server."""
         result = self.parent.request(
-            "GetSyncJobStatus", 
-            (self.parent.token, self._sync_job_id, self.location_id)
+            "GetSyncJobStatus", (self.parent.token, self._sync_job_id, self.location_id)
         )
 
         try:
             self.parent.raise_for_resultcode(result)
             job_state = result.get("JobState")
             if job_state == 1:
                 LOGGER.info(f"Panel sync for location {self.location_id} in progress")
             elif job_state == 2:
                 LOGGER.info(f"Panel sync for location {self.location_id} complete")
             else:
-                LOGGER.warning(f"Unknown panel sync status for location {self.location_id}")
+                LOGGER.warning(
+                    f"Unknown panel sync status for location {self.location_id}"
+                )
         except TotalConnectError:
-            LOGGER.error(f"Could not get status of Sync Job with ID {self._sync_job_id}")
-        
+            LOGGER.error(
+                f"Could not get status of Sync Job with ID {self._sync_job_id}"
+            )
+
+    def get_cameras(self):
+        """Get cameras for the location."""
+        result = self.parent.request(
+            "GetLocationAllCameraListEx", (self.parent.token, self.location_id)
+        )
+        self.parent.raise_for_resultcode(result)
+
+        if "AccountAllCameraList" not in result:
+            LOGGER.info(f"No cameras found for location {self.location_id}")
+            return
+
+        camera_list = result["AccountAllCameraList"]
+
+        if "WiFiDoorbellList" in camera_list:
+            self._get_doorbell(camera_list["WiFiDoorbellList"])
+
+        if "UnicornList" in camera_list:
+            self._get_unicorn(camera_list["UnicornList"])
+
+    def _get_doorbell(self, data):
+        """Find doorbell info."""
+        if not data or "WiFiDoorbellsList" not in data:
+            return
+
+        doorbells = data["WiFiDoorbellsList"]
+        if "WiFiDoorBellInfo" not in doorbells:
+            return
+
+        doorbell_list = doorbells["WiFiDoorBellInfo"]
+        for doorbell in doorbell_list:
+            id = doorbell["DeviceID"]
+            if id in self.devices:
+                self.devices[id].doorbell_info = doorbell
+
+    def _get_unicorn(self, data):
+        """Find uniforn info."""
+        if not data or "UnicornList" not in data:
+            return
+
+        unicorns = data["UnicornsList"]
+        if "UnicornInfo" not in unicorns:
+            return
+
+        unicorn_list = unicorns["UnicornInfo"]
+        for unicorn in unicorn_list:
+            id = unicorn["DeviceID"]
+            if id in self.devices:
+                self.devices[id].unicorn_info = unicorn
+
+    def get_video(self):
+        """Get video for the location."""
+        result = self.parent.request(
+            "GetVideoPIRLocationDeviceList", (self.parent.token, self.location_id)
+        )
+        self.parent.raise_for_resultcode(result)
+
+        if "VideoPIRList" not in result:
+            return
+
+        if "VideoPIRInfo" not in result["VideoPIRList"]:
+            return
+
+        video_list = result["VideoPIRList"]["VideoPIRInfo"]
+        for video in video_list:
+            id = video["DeviceID"]
+            if id in self.devices:
+                self.devices[id].video_info = video
```

### Comparing `total_connect_client-2023.7/total_connect_client/partition.py` & `total_connect_client-2024.4/total_connect_client/partition.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/total_connect_client/sync.py` & `total_connect_client-2024.4/total_connect_client/sync.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/total_connect_client/user.py` & `total_connect_client-2024.4/total_connect_client/user.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/total_connect_client/zone.py` & `total_connect_client-2024.4/total_connect_client/zone.py`

 * *Files identical despite different names*

### Comparing `total_connect_client-2023.7/total_connect_client.egg-info/PKG-INFO` & `total_connect_client-2024.4/total_connect_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
-Name: total-connect-client
-Version: 2023.7
+Name: total_connect_client
+Version: 2024.4
 Summary: Interact with Total Connect 2 alarm systems
 Author-email: "Craig J. Midwinter" <craig.j.midwinter@gmail.com>
 Project-URL: Homepage, https://github.com/craigjmidwinter/total-connect-client
 Project-URL: Bug Tracker, https://github.com/craigjmidwinter/total-connect-client/issues
 Keywords: alarm,TotalConnect
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: zeep>=4.2.1
 
 # Total-Connect-Client
 Total-Connect-Client is a python client for interacting with the [TotalConnect2](https://totalconnect2.com) alarm system.
 
 Started by @craigjmidwinter to add alarm support for his personal HomeAssistant set-up, with later contributions from others.
 
 To use with Home Assistant, follow the instructions to set up [Total Connect](https://www.home-assistant.io/integrations/totalconnect/).
```

### Comparing `total_connect_client-2023.7/total_connect_client.egg-info/SOURCES.txt` & `total_connect_client-2024.4/total_connect_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,8 +31,9 @@
 total_connect_client/zone.py
 total_connect_client.egg-info/PKG-INFO
 total_connect_client.egg-info/SOURCES.txt
 total_connect_client.egg-info/dependency_links.txt
 total_connect_client.egg-info/requires.txt
 total_connect_client.egg-info/top_level.txt
 total_connect_client/live/auto_bypass.py
+total_connect_client/live/experimental.py
 total_connect_client/live/zwave.py
```

