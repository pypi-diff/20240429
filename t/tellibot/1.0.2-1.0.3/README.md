# Comparing `tmp/tellibot-1.0.2.tar.gz` & `tmp/tellibot-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tellibot-1.0.2.tar", last modified: Mon Apr 29 16:11:29 2024, max compression
+gzip compressed data, was "tellibot-1.0.3.tar", last modified: Mon Apr 29 16:22:31 2024, max compression
```

## Comparing `tellibot-1.0.2.tar` & `tellibot-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 16:11:29.821304 tellibot-1.0.2/
--rw-rw-rw-   0        0        0     1084 2024-04-29 15:08:03.000000 tellibot-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      636 2024-04-29 16:11:29.774353 tellibot-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       76 2024-04-29 15:15:37.000000 tellibot-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 16:11:29.821304 tellibot-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      852 2024-04-29 16:11:07.000000 tellibot-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:11:29.506758 tellibot-1.0.2/tellibot/
--rw-rw-rw-   0        0        0     4737 2024-04-29 16:10:34.000000 tellibot-1.0.2/tellibot/argparse.py
--rw-rw-rw-   0        0        0      445 2024-04-28 21:17:41.000000 tellibot-1.0.2/tellibot/model.py
--rw-rw-rw-   0        0        0     4518 2024-04-29 16:11:00.000000 tellibot-1.0.2/tellibot/tellibot.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:11:29.742456 tellibot-1.0.2/tellibot.egg-info/
--rw-rw-rw-   0        0        0      636 2024-04-29 16:11:28.000000 tellibot-1.0.2/tellibot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-04-29 16:11:28.000000 tellibot-1.0.2/tellibot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 16:11:28.000000 tellibot-1.0.2/tellibot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-29 16:11:28.000000 tellibot-1.0.2/tellibot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2024-04-29 16:11:28.000000 tellibot-1.0.2/tellibot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 16:11:28.000000 tellibot-1.0.2/tellibot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 16:22:31.821901 tellibot-1.0.3/
+-rw-rw-rw-   0        0        0     1084 2024-04-29 15:08:03.000000 tellibot-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      636 2024-04-29 16:22:31.776180 tellibot-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       76 2024-04-29 15:15:37.000000 tellibot-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 16:22:31.821901 tellibot-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      852 2024-04-29 16:22:28.000000 tellibot-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:22:31.522215 tellibot-1.0.3/tellibot/
+-rw-rw-rw-   0        0        0     4737 2024-04-29 16:10:34.000000 tellibot-1.0.3/tellibot/argparse.py
+-rw-rw-rw-   0        0        0      445 2024-04-28 21:17:41.000000 tellibot-1.0.3/tellibot/model.py
+-rw-rw-rw-   0        0        0     4486 2024-04-29 16:22:15.000000 tellibot-1.0.3/tellibot/tellibot.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:22:31.748824 tellibot-1.0.3/tellibot.egg-info/
+-rw-rw-rw-   0        0        0      636 2024-04-29 16:22:31.000000 tellibot-1.0.3/tellibot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-04-29 16:22:31.000000 tellibot-1.0.3/tellibot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 16:22:31.000000 tellibot-1.0.3/tellibot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-29 16:22:31.000000 tellibot-1.0.3/tellibot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2024-04-29 16:22:31.000000 tellibot-1.0.3/tellibot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 16:22:31.000000 tellibot-1.0.3/tellibot.egg-info/top_level.txt
```

### Comparing `tellibot-1.0.2/LICENSE.txt` & `tellibot-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.2/PKG-INFO` & `tellibot-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellibot
-Version: 1.0.2
+Version: 1.0.3
 Summary: A drag and drop programming to create telegram bot
 Home-page: https://github.com/whoisjeeva/tellibot
 Author: Jeeva
 Author-email: support@gumify.me
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tellibot-1.0.2/setup.py` & `tellibot-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="tellibot",
-    version="1.0.2",
+    version="1.0.3",
     description="A drag and drop programming to create telegram bot",
     url="https://github.com/whoisjeeva/tellibot",
     author="Jeeva",
     author_email="support@gumify.me",
     license="MIT",
     packages=["tellibot"],
     install_requires=[
```

### Comparing `tellibot-1.0.2/tellibot/argparse.py` & `tellibot-1.0.3/tellibot/argparse.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.2/tellibot/tellibot.py` & `tellibot-1.0.3/tellibot/tellibot.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 import json
 import threading
 import asyncio
 import os
 import pymysql
 import sys
 
-from .interpreter.tellibot import TelliBot
+from interpreter.tellibot import TelliBot
 import model as model
-from .argparse import ArgParse
-from .util import colorify
-
+from argparse import ArgParse
 
 parser = ArgParse(argument_space_count=20, usage="gasper [path] [options]")
 parser.add_argument(["--help"], description="show help", is_flag=True)
 parser.add_argument(["--host", "-h"], description="mysql host")
 parser.add_argument(["--username", "-u"], description="mysql username")
 parser.add_argument(["--password", "-p"], description="mysql password")
 parser.add_argument(["--port"], description="mysql server port")
```

### Comparing `tellibot-1.0.2/tellibot.egg-info/PKG-INFO` & `tellibot-1.0.3/tellibot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellibot
-Version: 1.0.2
+Version: 1.0.3
 Summary: A drag and drop programming to create telegram bot
 Home-page: https://github.com/whoisjeeva/tellibot
 Author: Jeeva
 Author-email: support@gumify.me
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

