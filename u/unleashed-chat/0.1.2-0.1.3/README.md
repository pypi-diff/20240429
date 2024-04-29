# Comparing `tmp/unleashed_chat-0.1.2.tar.gz` & `tmp/unleashed_chat-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unleashed_chat-0.1.2.tar", last modified: Mon Apr 29 02:46:58 2024, max compression
+gzip compressed data, was "unleashed_chat-0.1.3.tar", last modified: Mon Apr 29 02:51:51 2024, max compression
```

## Comparing `unleashed_chat-0.1.2.tar` & `unleashed_chat-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 squash    (1000) squash    (1000)        0 2024-04-29 02:46:58.084993 unleashed_chat-0.1.2/
--rw-r--r--   0 squash    (1000) squash    (1000)     2094 2024-04-29 02:46:58.084993 unleashed_chat-0.1.2/PKG-INFO
--rw-r--r--   0 squash    (1000) squash    (1000)     1663 2024-04-29 01:54:21.000000 unleashed_chat-0.1.2/README.md
--rw-r--r--   0 squash    (1000) squash    (1000)       38 2024-04-29 02:46:58.084993 unleashed_chat-0.1.2/setup.cfg
--rw-r--r--   0 squash    (1000) squash    (1000)      782 2024-04-29 02:15:59.000000 unleashed_chat-0.1.2/setup.py
-drwxr-xr-x   0 squash    (1000) squash    (1000)        0 2024-04-29 02:46:58.084993 unleashed_chat-0.1.2/unleashed_chat/
--rw-r--r--   0 squash    (1000) squash    (1000)       71 2024-04-29 01:08:54.000000 unleashed_chat-0.1.2/unleashed_chat/__init__.py
--rw-r--r--   0 squash    (1000) squash    (1000)      424 2024-04-29 00:24:58.000000 unleashed_chat-0.1.2/unleashed_chat/cli.py
--rw-r--r--   0 squash    (1000) squash    (1000)     1555 2024-04-29 00:45:46.000000 unleashed_chat-0.1.2/unleashed_chat/config_handler.py
--rw-r--r--   0 squash    (1000) squash    (1000)      621 2024-04-29 01:45:20.000000 unleashed_chat-0.1.2/unleashed_chat/main.py
--rw-r--r--   0 squash    (1000) squash    (1000)     2342 2024-04-29 01:45:59.000000 unleashed_chat-0.1.2/unleashed_chat/openai_client.py
--rw-r--r--   0 squash    (1000) squash    (1000)      947 2024-04-29 01:45:07.000000 unleashed_chat-0.1.2/unleashed_chat/session.py
-drwxr-xr-x   0 squash    (1000) squash    (1000)        0 2024-04-29 02:46:58.084993 unleashed_chat-0.1.2/unleashed_chat.egg-info/
--rw-r--r--   0 squash    (1000) squash    (1000)     2094 2024-04-29 02:46:58.000000 unleashed_chat-0.1.2/unleashed_chat.egg-info/PKG-INFO
--rw-r--r--   0 squash    (1000) squash    (1000)      411 2024-04-29 02:46:58.000000 unleashed_chat-0.1.2/unleashed_chat.egg-info/SOURCES.txt
--rw-r--r--   0 squash    (1000) squash    (1000)        1 2024-04-29 02:46:58.000000 unleashed_chat-0.1.2/unleashed_chat.egg-info/dependency_links.txt
--rw-r--r--   0 squash    (1000) squash    (1000)       60 2024-04-29 02:46:58.000000 unleashed_chat-0.1.2/unleashed_chat.egg-info/entry_points.txt
--rw-r--r--   0 squash    (1000) squash    (1000)        7 2024-04-29 02:46:58.000000 unleashed_chat-0.1.2/unleashed_chat.egg-info/requires.txt
--rw-r--r--   0 squash    (1000) squash    (1000)       15 2024-04-29 02:46:58.000000 unleashed_chat-0.1.2/unleashed_chat.egg-info/top_level.txt
+drwxr-xr-x   0 squash    (1000) squash    (1000)        0 2024-04-29 02:51:51.534286 unleashed_chat-0.1.3/
+-rw-r--r--   0 squash    (1000) squash    (1000)     2094 2024-04-29 02:51:51.534286 unleashed_chat-0.1.3/PKG-INFO
+-rw-r--r--   0 squash    (1000) squash    (1000)     1663 2024-04-29 01:54:21.000000 unleashed_chat-0.1.3/README.md
+-rw-r--r--   0 squash    (1000) squash    (1000)       38 2024-04-29 02:51:51.534286 unleashed_chat-0.1.3/setup.cfg
+-rw-r--r--   0 squash    (1000) squash    (1000)      782 2024-04-29 02:51:43.000000 unleashed_chat-0.1.3/setup.py
+drwxr-xr-x   0 squash    (1000) squash    (1000)        0 2024-04-29 02:51:51.534286 unleashed_chat-0.1.3/unleashed_chat/
+-rw-r--r--   0 squash    (1000) squash    (1000)       71 2024-04-29 01:08:54.000000 unleashed_chat-0.1.3/unleashed_chat/__init__.py
+-rw-r--r--   0 squash    (1000) squash    (1000)      424 2024-04-29 00:24:58.000000 unleashed_chat-0.1.3/unleashed_chat/cli.py
+-rw-r--r--   0 squash    (1000) squash    (1000)     1629 2024-04-29 02:51:16.000000 unleashed_chat-0.1.3/unleashed_chat/config_handler.py
+-rw-r--r--   0 squash    (1000) squash    (1000)      621 2024-04-29 02:50:33.000000 unleashed_chat-0.1.3/unleashed_chat/main.py
+-rw-r--r--   0 squash    (1000) squash    (1000)     2342 2024-04-29 01:45:59.000000 unleashed_chat-0.1.3/unleashed_chat/openai_client.py
+-rw-r--r--   0 squash    (1000) squash    (1000)      947 2024-04-29 01:45:07.000000 unleashed_chat-0.1.3/unleashed_chat/session.py
+drwxr-xr-x   0 squash    (1000) squash    (1000)        0 2024-04-29 02:51:51.534286 unleashed_chat-0.1.3/unleashed_chat.egg-info/
+-rw-r--r--   0 squash    (1000) squash    (1000)     2094 2024-04-29 02:51:51.000000 unleashed_chat-0.1.3/unleashed_chat.egg-info/PKG-INFO
+-rw-r--r--   0 squash    (1000) squash    (1000)      411 2024-04-29 02:51:51.000000 unleashed_chat-0.1.3/unleashed_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 squash    (1000) squash    (1000)        1 2024-04-29 02:51:51.000000 unleashed_chat-0.1.3/unleashed_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 squash    (1000) squash    (1000)       60 2024-04-29 02:51:51.000000 unleashed_chat-0.1.3/unleashed_chat.egg-info/entry_points.txt
+-rw-r--r--   0 squash    (1000) squash    (1000)        7 2024-04-29 02:51:51.000000 unleashed_chat-0.1.3/unleashed_chat.egg-info/requires.txt
+-rw-r--r--   0 squash    (1000) squash    (1000)       15 2024-04-29 02:51:51.000000 unleashed_chat-0.1.3/unleashed_chat.egg-info/top_level.txt
```

### Comparing `unleashed_chat-0.1.2/PKG-INFO` & `unleashed_chat-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unleashed-chat
-Version: 0.1.2
+Version: 0.1.3
 Summary: A CLI wrapper for Unleashed.chat's chatbot service.
 Home-page: https://github.com/reecehunter/unleashed-chat
 Author: Reece Hunter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.1
```

### Comparing `unleashed_chat-0.1.2/README.md` & `unleashed_chat-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `unleashed_chat-0.1.2/setup.py` & `unleashed_chat-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='unleashed-chat',
-    version='0.1.2',
+    version='0.1.3',
     author="Reece Hunter",
     description="A CLI wrapper for Unleashed.chat's chatbot service.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/reecehunter/unleashed-chat",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `unleashed_chat-0.1.2/unleashed_chat/config_handler.py` & `unleashed_chat-0.1.3/unleashed_chat/config_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import configparser
 
 # Gets the configuration file.
 def get_config():
     config = configparser.ConfigParser()
     config.read('config.ini')
+    if 'Unleashed' not in config:
+        config.add_section('Unleashed')
     return config
 
 # Requests the user to input their Unleashed API key.
 def request_api_key():
     api_key = input("Please enter your Unleashed API key: ")
 
     config = get_config()
```

### Comparing `unleashed_chat-0.1.2/unleashed_chat/main.py` & `unleashed_chat-0.1.3/unleashed_chat/main.py`

 * *Files identical despite different names*

### Comparing `unleashed_chat-0.1.2/unleashed_chat/openai_client.py` & `unleashed_chat-0.1.3/unleashed_chat/openai_client.py`

 * *Files identical despite different names*

### Comparing `unleashed_chat-0.1.2/unleashed_chat/session.py` & `unleashed_chat-0.1.3/unleashed_chat/session.py`

 * *Files identical despite different names*

### Comparing `unleashed_chat-0.1.2/unleashed_chat.egg-info/PKG-INFO` & `unleashed_chat-0.1.3/unleashed_chat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unleashed-chat
-Version: 0.1.2
+Version: 0.1.3
 Summary: A CLI wrapper for Unleashed.chat's chatbot service.
 Home-page: https://github.com/reecehunter/unleashed-chat
 Author: Reece Hunter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.1
```

