# Comparing `tmp/youtubeuser-0.0.8.tar.gz` & `tmp/youtubeuser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtubeuser-0.0.8.tar", last modified: Mon Apr 29 00:35:38 2024, max compression
+gzip compressed data, was "youtubeuser-1.0.1.tar", last modified: Mon Apr 29 01:33:40 2024, max compression
```

## Comparing `youtubeuser-0.0.8.tar` & `youtubeuser-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-29 00:35:38.260953 youtubeuser-0.0.8/
--rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-29 00:35:38.260953 youtubeuser-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-29 00:35:38.260953 youtubeuser-0.0.8/YoutubeUser.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-29 00:35:37.000000 youtubeuser-0.0.8/YoutubeUser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      244 2024-04-29 00:35:37.000000 youtubeuser-0.0.8/YoutubeUser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-29 00:35:37.000000 youtubeuser-0.0.8/YoutubeUser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-29 00:35:37.000000 youtubeuser-0.0.8/YoutubeUser.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-29 00:35:37.000000 youtubeuser-0.0.8/YoutubeUser.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)      629 2024-04-29 00:35:32.000000 youtubeuser-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-29 00:35:38.260953 youtubeuser-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-29 00:35:06.000000 youtubeuser-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-29 00:35:38.260953 youtubeuser-0.0.8/youtubeuser/
--rw-r--r--   0 runner    (1000) runner    (1000)       54 2024-04-29 00:32:54.000000 youtubeuser-0.0.8/youtubeuser/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      812 2024-04-29 00:32:54.000000 youtubeuser-0.0.8/youtubeuser/getUser.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-29 01:33:40.663444 youtubeuser-1.0.1/
+-rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-29 01:33:40.659444 youtubeuser-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-29 01:33:40.659444 youtubeuser-1.0.1/YoutubeUser.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-29 01:33:40.000000 youtubeuser-1.0.1/YoutubeUser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      241 2024-04-29 01:33:40.000000 youtubeuser-1.0.1/YoutubeUser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-29 01:33:40.000000 youtubeuser-1.0.1/YoutubeUser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-29 01:33:40.000000 youtubeuser-1.0.1/YoutubeUser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-29 01:33:40.000000 youtubeuser-1.0.1/YoutubeUser.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      649 2024-04-29 01:33:25.000000 youtubeuser-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-29 01:33:40.663444 youtubeuser-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-29 01:33:19.000000 youtubeuser-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-29 01:33:40.655444 youtubeuser-1.0.1/youtubeuser/
+-rw-r--r--   0 runner    (1000) runner    (1000)       48 2024-04-29 01:30:46.000000 youtubeuser-1.0.1/youtubeuser/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      812 2024-04-29 01:31:15.000000 youtubeuser-1.0.1/youtubeuser/user.py
```

### Comparing `youtubeuser-0.0.8/pyproject.toml` & `youtubeuser-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "YoutubeUser"
-version = "0.0.8"
+version = "1.0.1"
 description = "A Lib For Search Youtube Channels Or User"
 authors = ["R1TGAMING"]
 
 [tool.poetry.dependencies]
 python = ">=3.10.0,<3.12"
 requests = "^2.31.0"
 setuptools = "^69.5.1"
@@ -16,9 +16,9 @@
 
 [tool.ruff]
 # https://beta.ruff.rs/docs/configuration/
 select = ['E', 'W', 'F', 'I', 'B', 'C4', 'ARG', 'SIM']
 ignore = ['W291', 'W292', 'W293']
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "setuptools>=40.8.0"]
+requires = ["poetry-core>=1.0.0", "setuptools>=40.8.0", "requests>=2.31.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `youtubeuser-0.0.8/setup.py` & `youtubeuser-1.0.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="YoutubeUser",
-    version='0.0.8',
+    version='1.0.1',
     author='R1TGAMING',
     author_email='rafisofyangaming1234@gmail.com',
     description='A Lib For Search Youtube User Or Channels',
   
     long_description_content_type='text/markdown',
    url='https://github.com/R1TGAMING/YoutubeUser',
     packages=["youtubeuser"],
```

### Comparing `youtubeuser-0.0.8/youtubeuser/getUser.py` & `youtubeuser-1.0.1/youtubeuser/user.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
 
-def GetInfo(channel_name : str) :
+def getUser(channel_name : str) :
   youtube = requests.get(f"https://www.googleapis.com/youtube/v3/search?part=snippet&type=channel&q={channel_name}&key=AIzaSyDBfcnjBerpgTFI5VCk_f3Rh-T_bc9LbEQ")
   if youtube.status_code == 200 :
      #get channel
       getchannel = youtube.json()["items"][0]
     
       channel_name = getchannel["snippet"]["title"]
```

