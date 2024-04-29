# Comparing `tmp/youtubeuser-0.0.5.tar.gz` & `tmp/youtubeuser-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtubeuser-0.0.5.tar", last modified: Sun Apr 28 03:34:09 2024, max compression
+gzip compressed data, was "youtubeuser-0.0.6.tar", last modified: Sun Apr 28 03:46:48 2024, max compression
```

## Comparing `youtubeuser-0.0.5.tar` & `youtubeuser-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-28 03:34:09.559090 youtubeuser-0.0.5/
--rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-28 03:34:09.555090 youtubeuser-0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-28 03:34:09.555090 youtubeuser-0.0.5/YoutubeUser.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-28 03:34:09.000000 youtubeuser-0.0.5/YoutubeUser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      197 2024-04-28 03:34:09.000000 youtubeuser-0.0.5/YoutubeUser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-28 03:34:09.000000 youtubeuser-0.0.5/YoutubeUser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-28 03:34:09.000000 youtubeuser-0.0.5/YoutubeUser.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-28 03:34:09.000000 youtubeuser-0.0.5/YoutubeUser.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)      607 2024-04-28 03:34:04.000000 youtubeuser-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-28 03:34:09.559090 youtubeuser-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      609 2024-04-28 03:33:42.000000 youtubeuser-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-28 03:46:48.683612 youtubeuser-0.0.6/
+-rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-28 03:46:48.679612 youtubeuser-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-28 03:46:48.679612 youtubeuser-0.0.6/YoutubeUser.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-28 03:46:48.000000 youtubeuser-0.0.6/YoutubeUser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      197 2024-04-28 03:46:48.000000 youtubeuser-0.0.6/YoutubeUser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-28 03:46:48.000000 youtubeuser-0.0.6/YoutubeUser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-28 03:46:48.000000 youtubeuser-0.0.6/YoutubeUser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-28 03:46:48.000000 youtubeuser-0.0.6/YoutubeUser.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      629 2024-04-28 03:44:35.000000 youtubeuser-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-28 03:46:48.683612 youtubeuser-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-28 03:45:34.000000 youtubeuser-0.0.6/setup.py
```

### Comparing `youtubeuser-0.0.5/pyproject.toml` & `youtubeuser-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "YoutubeUser"
-version = "0.0.5"
+version = "0.0.6"
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
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.0.0", "setuptools>=40.8.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `youtubeuser-0.0.5/setup.py` & `youtubeuser-0.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name="YoutubeUser",
-    version='0.0.5',
+    version='0.0.6',
     author='R1TGAMING',
     author_email='rafisofyangaming1234@gmail.com',
     description='A Lib For Search Youtube User Or Channels',
   
     long_description_content_type='text/markdown',
-    url='https://github.com/R1TGAMING/YoutubeUser',
+   url='https://github.com/R1TGAMING/YoutubeUser',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
-  install_requires= ["requests>=2.25.1"]
+    install_requires= ["requests>=2.25.1"]
 )
```

