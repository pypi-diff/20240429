# Comparing `tmp/tapsage_client-0.4.0.tar.gz` & `tmp/tapsage_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapsage_client-0.4.0.tar", last modified: Wed Apr 24 13:26:48 2024, max compression
+gzip compressed data, was "tapsage_client-0.5.0.tar", last modified: Mon Apr 29 14:25:32 2024, max compression
```

## Comparing `tapsage_client-0.4.0.tar` & `tapsage_client-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:26:48.546369 tapsage_client-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 13:26:40.000000 tapsage_client-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-24 13:26:48.546369 tapsage_client-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-24 13:26:40.000000 tapsage_client-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:26:48.546369 tapsage_client-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-24 13:26:40.000000 tapsage_client-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:26:48.542369 tapsage_client-0.4.0/tapsage/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-24 13:26:40.000000 tapsage_client-0.4.0/tapsage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-04-24 13:26:40.000000 tapsage_client-0.4.0/tapsage/tapsagebot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-24 13:26:40.000000 tapsage_client-0.4.0/tapsage/taptypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-24 13:26:40.000000 tapsage_client-0.4.0/tapsage/tapuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-24 13:26:40.000000 tapsage_client-0.4.0/tapsage/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:26:48.546369 tapsage_client-0.4.0/tapsage_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-24 13:26:48.000000 tapsage_client-0.4.0/tapsage_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 13:26:48.000000 tapsage_client-0.4.0/tapsage_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:26:48.000000 tapsage_client-0.4.0/tapsage_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:26:48.000000 tapsage_client-0.4.0/tapsage_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 13:26:48.000000 tapsage_client-0.4.0/tapsage_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:25:32.627716 tapsage_client-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 14:25:28.000000 tapsage_client-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-29 14:25:32.627716 tapsage_client-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-29 14:25:28.000000 tapsage_client-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:25:32.627716 tapsage_client-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-29 14:25:28.000000 tapsage_client-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:25:32.623716 tapsage_client-0.5.0/tapsage/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-29 14:25:28.000000 tapsage_client-0.5.0/tapsage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-29 14:25:28.000000 tapsage_client-0.5.0/tapsage/tapsagebot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-29 14:25:28.000000 tapsage_client-0.5.0/tapsage/taptypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-29 14:25:28.000000 tapsage_client-0.5.0/tapsage/tapuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-29 14:25:28.000000 tapsage_client-0.5.0/tapsage/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:25:32.627716 tapsage_client-0.5.0/tapsage_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-29 14:25:32.000000 tapsage_client-0.5.0/tapsage_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-29 14:25:32.000000 tapsage_client-0.5.0/tapsage_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:25:32.000000 tapsage_client-0.5.0/tapsage_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:25:32.000000 tapsage_client-0.5.0/tapsage_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 14:25:32.000000 tapsage_client-0.5.0/tapsage_client.egg-info/top_level.txt
```

### Comparing `tapsage_client-0.4.0/LICENSE` & `tapsage_client-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tapsage_client-0.4.0/PKG-INFO` & `tapsage_client-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapsage_client
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python client for Tapsage to streamline API interactions, enabling easy management and customization of AI-driven chatbots and image models.
 Home-page: https://github.com/mahdikiani/tapsage-python
 Author: Mahdi Kiani
 Author-email: mahdikiany@gmail.com
 License: Apache-2.0
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `tapsage_client-0.4.0/README.md` & `tapsage_client-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tapsage_client-0.4.0/setup.py` & `tapsage_client-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `tapsage_client-0.4.0/tapsage/tapsagebot.py` & `tapsage_client-0.5.0/tapsage/tapsagebot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import uuid
 
 import requests
-from .taptypes import (
+from tapsage.taptypes import (
     Message,
     MessageContent,
     MessageRequest,
     MessageStream,
     Session,
     SessionRequest,
     SessionUser,
```

### Comparing `tapsage_client-0.4.0/tapsage/taptypes.py` & `tapsage_client-0.5.0/tapsage/taptypes.py`

 * *Files identical despite different names*

### Comparing `tapsage_client-0.4.0/tapsage/tapuser.py` & `tapsage_client-0.5.0/tapsage/tapuser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from .taptypes import Bot, BotRequest
+from tapsage.taptypes import Bot, BotRequest
 
 
 class TapSageUser:
     API_V1 = "https://api.tapsage.com/api/v1"
 
     def __init__(self, api_key):
         self.api_key = api_key
```

### Comparing `tapsage_client-0.4.0/tapsage/test.py` & `tapsage_client-0.5.0/tapsage/test.py`

 * *Files identical despite different names*

### Comparing `tapsage_client-0.4.0/tapsage_client.egg-info/PKG-INFO` & `tapsage_client-0.5.0/tapsage_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapsage_client
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python client for Tapsage to streamline API interactions, enabling easy management and customization of AI-driven chatbots and image models.
 Home-page: https://github.com/mahdikiani/tapsage-python
 Author: Mahdi Kiani
 Author-email: mahdikiany@gmail.com
 License: Apache-2.0
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```
