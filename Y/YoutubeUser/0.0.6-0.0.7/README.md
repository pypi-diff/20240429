# Comparing `tmp/youtubeuser-0.0.6.tar.gz` & `tmp/youtubeuser-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtubeuser-0.0.6.tar", last modified: Sun Apr 28 03:46:48 2024, max compression
+gzip compressed data, was "youtubeuser-0.0.7.tar", last modified: Mon Apr 29 00:27:25 2024, max compression
```

## Comparing `youtubeuser-0.0.6.tar` & `youtubeuser-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-28 03:46:48.683612 youtubeuser-0.0.6/
--rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-28 03:46:48.679612 youtubeuser-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-28 03:46:48.679612 youtubeuser-0.0.6/YoutubeUser.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-28 03:46:48.000000 youtubeuser-0.0.6/YoutubeUser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      197 2024-04-28 03:46:48.000000 youtubeuser-0.0.6/YoutubeUser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-28 03:46:48.000000 youtubeuser-0.0.6/YoutubeUser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-28 03:46:48.000000 youtubeuser-0.0.6/YoutubeUser.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-28 03:46:48.000000 youtubeuser-0.0.6/YoutubeUser.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)      629 2024-04-28 03:44:35.000000 youtubeuser-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-28 03:46:48.683612 youtubeuser-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-28 03:45:34.000000 youtubeuser-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-29 00:27:25.565587 youtubeuser-0.0.7/
+-rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-29 00:27:25.565587 youtubeuser-0.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-29 00:27:25.561587 youtubeuser-0.0.7/YoutubeUser/
+-rw-r--r--   0 runner    (1000) runner    (1000)       54 2024-04-29 00:25:40.000000 youtubeuser-0.0.7/YoutubeUser/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      812 2024-04-29 00:22:51.000000 youtubeuser-0.0.7/YoutubeUser/getUser.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-29 00:27:25.565587 youtubeuser-0.0.7/YoutubeUser.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-04-29 00:27:25.000000 youtubeuser-0.0.7/YoutubeUser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      244 2024-04-29 00:27:25.000000 youtubeuser-0.0.7/YoutubeUser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-29 00:27:25.000000 youtubeuser-0.0.7/YoutubeUser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-29 00:27:25.000000 youtubeuser-0.0.7/YoutubeUser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-29 00:27:25.000000 youtubeuser-0.0.7/YoutubeUser.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      629 2024-04-28 03:44:35.000000 youtubeuser-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-29 00:27:25.565587 youtubeuser-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-29 00:26:33.000000 youtubeuser-0.0.7/setup.py
```

### Comparing `youtubeuser-0.0.6/pyproject.toml` & `youtubeuser-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `youtubeuser-0.0.6/setup.py` & `youtubeuser-0.0.7/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="YoutubeUser",
-    version='0.0.6',
+    version='0.0.7',
     author='R1TGAMING',
     author_email='rafisofyangaming1234@gmail.com',
     description='A Lib For Search Youtube User Or Channels',
   
     long_description_content_type='text/markdown',
    url='https://github.com/R1TGAMING/YoutubeUser',
-    packages=find_packages(),
+    packages=["YoutubeUser"],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
     install_requires= ["requests>=2.25.1"]
```

