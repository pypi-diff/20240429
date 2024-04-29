# Comparing `tmp/tellibot-1.0.4.tar.gz` & `tmp/tellibot-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tellibot-1.0.4.tar", last modified: Mon Apr 29 16:27:24 2024, max compression
+gzip compressed data, was "tellibot-1.0.5.tar", last modified: Mon Apr 29 16:30:18 2024, max compression
```

## Comparing `tellibot-1.0.4.tar` & `tellibot-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 16:27:24.269695 tellibot-1.0.4/
--rw-rw-rw-   0        0        0     1084 2024-04-29 15:08:03.000000 tellibot-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      636 2024-04-29 16:27:24.222291 tellibot-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       76 2024-04-29 15:15:37.000000 tellibot-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 16:27:24.269695 tellibot-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      852 2024-04-29 16:27:17.000000 tellibot-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:27:24.001641 tellibot-1.0.4/tellibot/
--rw-rw-rw-   0        0        0     4737 2024-04-29 16:10:34.000000 tellibot-1.0.4/tellibot/argparse.py
--rw-rw-rw-   0        0        0      445 2024-04-28 21:17:41.000000 tellibot-1.0.4/tellibot/model.py
--rw-rw-rw-   0        0        0     4486 2024-04-29 16:25:12.000000 tellibot-1.0.4/tellibot/tellibot.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:27:24.191012 tellibot-1.0.4/tellibot.egg-info/
--rw-rw-rw-   0        0        0      636 2024-04-29 16:27:23.000000 tellibot-1.0.4/tellibot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-04-29 16:27:23.000000 tellibot-1.0.4/tellibot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 16:27:23.000000 tellibot-1.0.4/tellibot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-29 16:27:23.000000 tellibot-1.0.4/tellibot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2024-04-29 16:27:23.000000 tellibot-1.0.4/tellibot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 16:27:23.000000 tellibot-1.0.4/tellibot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 16:30:18.993071 tellibot-1.0.5/
+-rw-rw-rw-   0        0        0     1084 2024-04-29 15:08:03.000000 tellibot-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      636 2024-04-29 16:30:18.990079 tellibot-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       76 2024-04-29 15:15:37.000000 tellibot-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 16:30:18.993071 tellibot-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      852 2024-04-29 16:30:07.000000 tellibot-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:30:18.862782 tellibot-1.0.5/tellibot/
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:30:04.000000 tellibot-1.0.5/tellibot/__init__.py
+-rw-rw-rw-   0        0        0     4737 2024-04-29 16:10:34.000000 tellibot-1.0.5/tellibot/argparse.py
+-rw-rw-rw-   0        0        0      445 2024-04-28 21:17:41.000000 tellibot-1.0.5/tellibot/model.py
+-rw-rw-rw-   0        0        0     4486 2024-04-29 16:25:12.000000 tellibot-1.0.5/tellibot/tellibot.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:30:18.985076 tellibot-1.0.5/tellibot.egg-info/
+-rw-rw-rw-   0        0        0      636 2024-04-29 16:30:18.000000 tellibot-1.0.5/tellibot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-04-29 16:30:18.000000 tellibot-1.0.5/tellibot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 16:30:18.000000 tellibot-1.0.5/tellibot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-29 16:30:18.000000 tellibot-1.0.5/tellibot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2024-04-29 16:30:18.000000 tellibot-1.0.5/tellibot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 16:30:18.000000 tellibot-1.0.5/tellibot.egg-info/top_level.txt
```

### Comparing `tellibot-1.0.4/LICENSE.txt` & `tellibot-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.4/PKG-INFO` & `tellibot-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellibot
-Version: 1.0.4
+Version: 1.0.5
 Summary: A drag and drop programming to create telegram bot
 Home-page: https://github.com/whoisjeeva/tellibot
 Author: Jeeva
 Author-email: support@gumify.me
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tellibot-1.0.4/setup.py` & `tellibot-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="tellibot",
-    version="1.0.4",
+    version="1.0.5",
     description="A drag and drop programming to create telegram bot",
     url="https://github.com/whoisjeeva/tellibot",
     author="Jeeva",
     author_email="support@gumify.me",
     license="MIT",
     packages=["tellibot"],
     install_requires=[
```

### Comparing `tellibot-1.0.4/tellibot/argparse.py` & `tellibot-1.0.5/tellibot/argparse.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.4/tellibot/tellibot.py` & `tellibot-1.0.5/tellibot/tellibot.py`

 * *Files identical despite different names*

### Comparing `tellibot-1.0.4/tellibot.egg-info/PKG-INFO` & `tellibot-1.0.5/tellibot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellibot
-Version: 1.0.4
+Version: 1.0.5
 Summary: A drag and drop programming to create telegram bot
 Home-page: https://github.com/whoisjeeva/tellibot
 Author: Jeeva
 Author-email: support@gumify.me
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

