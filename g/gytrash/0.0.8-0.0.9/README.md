# Comparing `tmp/gytrash-0.0.8.tar.gz` & `tmp/gytrash-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gytrash-0.0.8.tar", last modified: Sat Jun 26 18:34:23 2021, max compression
+gzip compressed data, was "gytrash-0.0.9.tar", last modified: Sat Jun 26 19:04:13 2021, max compression
```

## Comparing `gytrash-0.0.8.tar` & `gytrash-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-26 18:34:23.127625 gytrash-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-06-26 18:34:10.000000 gytrash-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-26 18:34:10.000000 gytrash-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2305 2021-06-26 18:34:23.127625 gytrash-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1399 2021-06-26 18:34:10.000000 gytrash-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-26 18:34:23.127625 gytrash-0.0.8/gytrash/
--rw-r--r--   0 runner    (1001) docker     (121)     3633 2021-06-26 18:34:10.000000 gytrash-0.0.8/gytrash/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2021-06-26 18:34:10.000000 gytrash-0.0.8/gytrash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-26 18:34:23.127625 gytrash-0.0.8/gytrash/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-06-26 18:34:10.000000 gytrash-0.0.8/gytrash/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3301 2021-06-26 18:34:10.000000 gytrash-0.0.8/gytrash/handlers/slack.py
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2021-06-26 18:34:10.000000 gytrash-0.0.8/gytrash/logging_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-26 18:34:23.127625 gytrash-0.0.8/gytrash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2305 2021-06-26 18:34:23.000000 gytrash-0.0.8/gytrash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      343 2021-06-26 18:34:23.000000 gytrash-0.0.8/gytrash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-26 18:34:23.000000 gytrash-0.0.8/gytrash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-26 18:34:23.000000 gytrash-0.0.8/gytrash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-06-26 18:34:23.000000 gytrash-0.0.8/gytrash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-06-26 18:34:23.000000 gytrash-0.0.8/gytrash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-26 18:34:23.127625 gytrash-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1843 2021-06-26 18:34:14.000000 gytrash-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-26 19:04:13.229675 gytrash-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-06-26 19:04:01.000000 gytrash-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-26 19:04:01.000000 gytrash-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2305 2021-06-26 19:04:13.229675 gytrash-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1399 2021-06-26 19:04:01.000000 gytrash-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-26 19:04:13.229675 gytrash-0.0.9/gytrash/
+-rw-r--r--   0 runner    (1001) docker     (121)     3633 2021-06-26 19:04:01.000000 gytrash-0.0.9/gytrash/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1622 2021-06-26 19:04:01.000000 gytrash-0.0.9/gytrash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-26 19:04:13.229675 gytrash-0.0.9/gytrash/handlers/
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2021-06-26 19:04:01.000000 gytrash-0.0.9/gytrash/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3330 2021-06-26 19:04:01.000000 gytrash-0.0.9/gytrash/handlers/slack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1301 2021-06-26 19:04:01.000000 gytrash-0.0.9/gytrash/logging_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-26 19:04:13.229675 gytrash-0.0.9/gytrash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2305 2021-06-26 19:04:13.000000 gytrash-0.0.9/gytrash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      343 2021-06-26 19:04:13.000000 gytrash-0.0.9/gytrash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-26 19:04:13.000000 gytrash-0.0.9/gytrash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-26 19:04:13.000000 gytrash-0.0.9/gytrash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-06-26 19:04:13.000000 gytrash-0.0.9/gytrash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-06-26 19:04:13.000000 gytrash-0.0.9/gytrash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-26 19:04:13.229675 gytrash-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1788 2021-06-26 19:04:04.000000 gytrash-0.0.9/setup.py
```

### Comparing `gytrash-0.0.8/LICENSE` & `gytrash-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gytrash-0.0.8/PKG-INFO` & `gytrash-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gytrash
-Version: 0.0.8
+Version: 0.0.9
 Summary: Useful things for Logging.
 Home-page: http://github.com/trejas/gytrash
 Author: Traey Hatch
 Author-email: thatch@newmathdata.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/trejas/gytrash
 Platform: UNKNOWN
```

### Comparing `gytrash-0.0.8/README.md` & `gytrash-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gytrash-0.0.8/gytrash/__about__.py` & `gytrash-0.0.9/gytrash/__about__.py`

 * *Files identical despite different names*

### Comparing `gytrash-0.0.8/gytrash/__init__.py` & `gytrash-0.0.9/gytrash/__init__.py`

 * *Files identical despite different names*

### Comparing `gytrash-0.0.8/gytrash/handlers/slack.py` & `gytrash-0.0.9/gytrash/handlers/slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         if slack_bot_token:
             self.slack_web_client = WebClient(token=slack_bot_token)
         else:
             self.slack_web_client = WebClient(token=os.environ["SLACK_BOT_TOKEN"])
         self.channel = channel
 
     def _send_log(self, message: str, channel: str):
+        print("Sending log")
         # Create a new onboarding tutorial.
         onboarding_tutorial = LogMessage(channel, message)
 
         # Get the onboarding message payload
         slack_payload = onboarding_tutorial.get_message_payload()
 
         # Post the onboarding message in Slack
```

### Comparing `gytrash-0.0.8/gytrash/logging_mixin.py` & `gytrash-0.0.9/gytrash/logging_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         """ A logger object.
         Returns:
             Logger
         """
         self._log = logging.getLogger(
             self.__class__.__module__ + "." + self.__class__.__name__
         )
-        self.log.setup_logging(log_level=10)
+        # self.log.setup_logging(log_level=10)
         return self._log
 
     def _set_context(self, context):
         if context is not None:
             set_context(self.log, context)
```

### Comparing `gytrash-0.0.8/gytrash.egg-info/PKG-INFO` & `gytrash-0.0.9/gytrash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gytrash
-Version: 0.0.8
+Version: 0.0.9
 Summary: Useful things for Logging.
 Home-page: http://github.com/trejas/gytrash
 Author: Traey Hatch
 Author-email: thatch@newmathdata.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/trejas/gytrash
 Platform: UNKNOWN
```

### Comparing `gytrash-0.0.8/setup.py` & `gytrash-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# Learn more: https://github.com/kennethreitz/setup.py
 
 import os
 import re
 import sys
 
 from codecs import open
 
@@ -21,15 +20,15 @@
 with open(os.path.join(repo_path, "gytrash", "__about__.py"), "r", "utf-8") as f:
     exec(f.read(), about)
 with open("README.md", "r", "utf-8") as f:
     readme = f.read()
 
 setup(
     name=about["__title__"],
-    version="0.0.8",
+    version="0.0.9",
     description=about["__description__"],
     long_description=readme,
     long_description_content_type="text/markdown",
     author=about["__author__"],
     author_email=about["__author_email__"],
     url=about["__url__"],
     packages=packages,
```

