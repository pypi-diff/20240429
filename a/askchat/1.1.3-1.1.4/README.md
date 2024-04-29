# Comparing `tmp/askchat-1.1.3.tar.gz` & `tmp/askchat-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askchat-1.1.3.tar", last modified: Thu Apr  4 13:38:48 2024, max compression
+gzip compressed data, was "askchat-1.1.4.tar", last modified: Mon Apr 29 16:06:11 2024, max compression
```

## Comparing `askchat-1.1.3.tar` & `askchat-1.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:38:48.648183 askchat-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 13:38:40.000000 askchat-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-04 13:38:40.000000 askchat-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-04 13:38:48.648183 askchat-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-04 13:38:40.000000 askchat-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:38:48.648183 askchat-1.1.3/askchat/
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-04 13:38:40.000000 askchat-1.1.3/askchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-04 13:38:40.000000 askchat-1.1.3/askchat/ask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-04 13:38:40.000000 askchat-1.1.3/askchat/askenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-04-04 13:38:40.000000 askchat-1.1.3/askchat/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:38:48.648183 askchat-1.1.3/askchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-04 13:38:48.000000 askchat-1.1.3/askchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-04 13:38:48.000000 askchat-1.1.3/askchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:38:48.000000 askchat-1.1.3/askchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-04 13:38:48.000000 askchat-1.1.3/askchat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:38:48.000000 askchat-1.1.3/askchat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 13:38:48.000000 askchat-1.1.3/askchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 13:38:48.000000 askchat-1.1.3/askchat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-04 13:38:48.648183 askchat-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-04 13:38:40.000000 askchat-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:38:48.648183 askchat-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 13:38:40.000000 askchat-1.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-04 13:38:40.000000 askchat-1.1.3/tests/test_askchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-04 13:38:40.000000 askchat-1.1.3/tests/test_askenv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:06:11.824930 askchat-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-29 16:06:00.000000 askchat-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-29 16:06:00.000000 askchat-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-29 16:06:11.824930 askchat-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-29 16:06:00.000000 askchat-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:06:11.820930 askchat-1.1.4/askchat/
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-29 16:06:00.000000 askchat-1.1.4/askchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-29 16:06:00.000000 askchat-1.1.4/askchat/ask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-29 16:06:00.000000 askchat-1.1.4/askchat/askenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-29 16:06:00.000000 askchat-1.1.4/askchat/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:06:11.820930 askchat-1.1.4/askchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-29 16:06:11.000000 askchat-1.1.4/askchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-29 16:06:11.000000 askchat-1.1.4/askchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:06:11.000000 askchat-1.1.4/askchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 16:06:11.000000 askchat-1.1.4/askchat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:06:11.000000 askchat-1.1.4/askchat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-29 16:06:11.000000 askchat-1.1.4/askchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 16:06:11.000000 askchat-1.1.4/askchat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-29 16:06:11.824930 askchat-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-29 16:06:00.000000 askchat-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:06:11.824930 askchat-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 16:06:00.000000 askchat-1.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-29 16:06:00.000000 askchat-1.1.4/tests/test_askchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-29 16:06:00.000000 askchat-1.1.4/tests/test_askenv.py
```

### Comparing `askchat-1.1.3/LICENSE` & `askchat-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `askchat-1.1.3/PKG-INFO` & `askchat-1.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: askchat
-Version: 1.1.3
+Version: 1.1.4
 Summary: Interact with ChatGPT in terminal via chattool
 Home-page: https://github.com/cubenlp/askchat
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: UNKNOWN
 Keywords: askchat
```

### Comparing `askchat-1.1.3/README.md` & `askchat-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `askchat-1.1.3/askchat/__init__.py` & `askchat-1.1.4/askchat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for askchat."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '1.1.3'
+__version__ = '1.1.4'
 
 import asyncio
 from pathlib import Path
 import click
 from dotenv import set_key
 import os
```

### Comparing `askchat-1.1.3/askchat/askenv.py` & `askchat-1.1.4/askchat/askenv.py`

 * *Files identical despite different names*

### Comparing `askchat-1.1.3/askchat/cli.py` & `askchat-1.1.4/askchat/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,13 +199,25 @@
             return
         chat.user(message_text)
     else:
         if not message_text:
             click.echo("Please specify message!")
             return
         chat.user(message_text)
-    # Add chat response
+    # additinal options
+    if option:
+        option = dict(option)
+        ints = ['max_tokens', 'n', 'top_logprobs', 'seed']
+        floats = ['temperature', 'presence_penalty', 'frequency_penalty', 'top_p']
+        for key, value in option.items():
+            if key in ints:
+                option[key] = int(value)
+            elif key in floats:
+                option[key] = float(value)
+    else:
+        option = {}
+    # Add chat responses
     chat.assistant(asyncio.run(show_resp(chat, **dict(option))))
     chat.save(LAST_CHAT_FILE, mode='w')
 
 if __name__ == '__main__':
     cli()
```

### Comparing `askchat-1.1.3/askchat.egg-info/PKG-INFO` & `askchat-1.1.4/askchat.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: askchat
-Version: 1.1.3
+Version: 1.1.4
 Summary: Interact with ChatGPT in terminal via chattool
 Home-page: https://github.com/cubenlp/askchat
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: UNKNOWN
 Keywords: askchat
```

### Comparing `askchat-1.1.3/setup.py` & `askchat-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-VERSION = '1.1.3'
+VERSION = '1.1.4'
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 requirements = ['chattool>=3.1.4', "python-dotenv>=0.17.0", 'Click>=8.0']
 
 test_requirements = ['pytest>=3']
```

### Comparing `askchat-1.1.3/tests/test_askchat.py` & `askchat-1.1.4/tests/test_askchat.py`

 * *Files identical despite different names*

### Comparing `askchat-1.1.3/tests/test_askenv.py` & `askchat-1.1.4/tests/test_askenv.py`

 * *Files identical despite different names*

