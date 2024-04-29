# Comparing `tmp/bambot-0.3.7.tar.gz` & `tmp/bambot-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambot-0.3.7.tar", last modified: Mon Apr 29 04:47:37 2024, max compression
+gzip compressed data, was "bambot-0.3.8.tar", last modified: Mon Apr 29 19:51:48 2024, max compression
```

## Comparing `bambot-0.3.7.tar` & `bambot-0.3.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 04:47:37.484378 bambot-0.3.7/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1027 2024-04-29 04:47:37.484055 bambot-0.3.7/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      148 2024-04-27 21:13:32.000000 bambot-0.3.7/README.md
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 04:47:37.480764 bambot-0.3.7/bambot/
--rw-r--r--   0 spencerkinney   (501) staff       (20)       60 2024-04-27 22:56:54.000000 bambot-0.3.7/bambot/__init__.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1832 2024-04-28 22:59:21.000000 bambot-0.3.7/bambot/agent.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     7479 2024-04-29 04:41:54.000000 bambot-0.3.7/bambot/cli.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     7127 2024-04-29 04:38:11.000000 bambot-0.3.7/bambot/docker_utils.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      464 2024-04-28 23:09:41.000000 bambot-0.3.7/bambot/log_utils.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      708 2024-04-29 03:05:28.000000 bambot-0.3.7/bambot/logger.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     2016 2024-04-29 03:00:30.000000 bambot-0.3.7/bambot/remote_utils.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 04:47:37.483182 bambot-0.3.7/bambot/templates/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1103 2024-04-29 04:41:19.000000 bambot-0.3.7/bambot/templates/Dockerfile.dashboard.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1020 2024-04-29 04:41:13.000000 bambot-0.3.7/bambot/templates/Dockerfile.lightweight.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)       98 2024-04-27 20:00:14.000000 bambot-0.3.7/bambot/templates/Procfile.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)      559 2024-04-27 21:53:04.000000 bambot-0.3.7/bambot/templates/agent_readme.md.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)      332 2024-04-29 02:01:28.000000 bambot-0.3.7/bambot/templates/bot.py.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1862 2024-04-28 06:29:24.000000 bambot-0.3.7/bambot/templates/dashboard.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      296 2024-04-28 08:17:47.000000 bambot-0.3.7/bambot/templates/run.sh.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)      371 2024-04-28 08:09:43.000000 bambot-0.3.7/bambot/utils.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 04:47:37.483688 bambot-0.3.7/bambot.egg-info/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1027 2024-04-29 04:47:37.000000 bambot-0.3.7/bambot.egg-info/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      602 2024-04-29 04:47:37.000000 bambot-0.3.7/bambot.egg-info/SOURCES.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-04-29 04:47:37.000000 bambot-0.3.7/bambot.egg-info/dependency_links.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       39 2024-04-29 04:47:37.000000 bambot-0.3.7/bambot.egg-info/entry_points.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       27 2024-04-29 04:47:37.000000 bambot-0.3.7/bambot.egg-info/requires.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-04-29 04:47:37.000000 bambot-0.3.7/bambot.egg-info/top_level.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-04-29 04:47:37.484428 bambot-0.3.7/setup.cfg
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1296 2024-04-29 04:47:24.000000 bambot-0.3.7/setup.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 04:47:37.483454 bambot-0.3.7/tests/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1443 2024-04-27 21:53:17.000000 bambot-0.3.7/tests/test_bambot.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 19:51:48.870691 bambot-0.3.8/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1027 2024-04-29 19:51:48.870329 bambot-0.3.8/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      148 2024-04-29 19:41:11.000000 bambot-0.3.8/README.md
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 19:51:48.867340 bambot-0.3.8/bambot/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       60 2024-04-29 19:41:11.000000 bambot-0.3.8/bambot/__init__.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1832 2024-04-29 19:41:11.000000 bambot-0.3.8/bambot/agent.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     7479 2024-04-29 19:41:11.000000 bambot-0.3.8/bambot/cli.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     7127 2024-04-29 19:41:11.000000 bambot-0.3.8/bambot/docker_utils.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      464 2024-04-29 19:41:11.000000 bambot-0.3.8/bambot/log_utils.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      708 2024-04-29 19:41:11.000000 bambot-0.3.8/bambot/logger.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2016 2024-04-29 19:41:11.000000 bambot-0.3.8/bambot/remote_utils.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 19:51:48.869474 bambot-0.3.8/bambot/templates/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1103 2024-04-29 19:41:11.000000 bambot-0.3.8/bambot/templates/Dockerfile.dashboard.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1020 2024-04-29 19:41:11.000000 bambot-0.3.8/bambot/templates/Dockerfile.lightweight.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       98 2024-04-29 19:41:11.000000 bambot-0.3.8/bambot/templates/Procfile.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      559 2024-04-29 19:41:11.000000 bambot-0.3.8/bambot/templates/agent_readme.md.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      332 2024-04-29 19:41:11.000000 bambot-0.3.8/bambot/templates/bot.py.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1862 2024-04-29 19:41:11.000000 bambot-0.3.8/bambot/templates/dashboard.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      296 2024-04-29 19:41:11.000000 bambot-0.3.8/bambot/templates/run.sh.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      371 2024-04-29 19:41:11.000000 bambot-0.3.8/bambot/utils.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 19:51:48.869935 bambot-0.3.8/bambot.egg-info/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1027 2024-04-29 19:51:48.000000 bambot-0.3.8/bambot.egg-info/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      602 2024-04-29 19:51:48.000000 bambot-0.3.8/bambot.egg-info/SOURCES.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-04-29 19:51:48.000000 bambot-0.3.8/bambot.egg-info/dependency_links.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       39 2024-04-29 19:51:48.000000 bambot-0.3.8/bambot.egg-info/entry_points.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       27 2024-04-29 19:51:48.000000 bambot-0.3.8/bambot.egg-info/requires.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-04-29 19:51:48.000000 bambot-0.3.8/bambot.egg-info/top_level.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-04-29 19:51:48.870744 bambot-0.3.8/setup.cfg
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1285 2024-04-29 19:51:16.000000 bambot-0.3.8/setup.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 19:51:48.869626 bambot-0.3.8/tests/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1443 2024-04-29 19:41:11.000000 bambot-0.3.8/tests/test_bambot.py
```

### Comparing `bambot-0.3.7/PKG-INFO` & `bambot-0.3.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.3.7
+Version: 0.3.8
 Summary: Lightweight containers for AI agents
 Home-page: https://github.com/BamCorp/bambot
 Author: Bam Corp
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bambot-0.3.7/bambot/agent.py` & `bambot-0.3.8/bambot/agent.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.7/bambot/cli.py` & `bambot-0.3.8/bambot/cli.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.7/bambot/docker_utils.py` & `bambot-0.3.8/bambot/docker_utils.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.7/bambot/logger.py` & `bambot-0.3.8/bambot/logger.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.7/bambot/remote_utils.py` & `bambot-0.3.8/bambot/remote_utils.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.7/bambot/templates/Dockerfile.dashboard.j2` & `bambot-0.3.8/bambot/templates/Dockerfile.dashboard.j2`

 * *Files identical despite different names*

### Comparing `bambot-0.3.7/bambot/templates/Dockerfile.lightweight.j2` & `bambot-0.3.8/bambot/templates/Dockerfile.lightweight.j2`

 * *Files identical despite different names*

### Comparing `bambot-0.3.7/bambot/templates/agent_readme.md.j2` & `bambot-0.3.8/bambot/templates/agent_readme.md.j2`

 * *Files identical despite different names*

### Comparing `bambot-0.3.7/bambot/templates/dashboard.py` & `bambot-0.3.8/bambot/templates/dashboard.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.7/bambot.egg-info/PKG-INFO` & `bambot-0.3.8/bambot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.3.7
+Version: 0.3.8
 Summary: Lightweight containers for AI agents
 Home-page: https://github.com/BamCorp/bambot
 Author: Bam Corp
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bambot-0.3.7/bambot.egg-info/SOURCES.txt` & `bambot-0.3.8/bambot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bambot-0.3.7/setup.py` & `bambot-0.3.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-# setup.py
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bambot",
-    version="0.3.7",
+    version="0.3.8",
     author="Bam Corp",
     author_email="spencer@bam.bot",
     description="Lightweight containers for AI agents",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BamCorp/bambot",
     packages=find_packages(),
     package_data={
-        "bambot": ["templates/*"]
+        "bambot": ["templates/*"],
     },
     install_requires=[
         "click",
         "jinja2",
         "tqdm",
-        "requests",
+        "requests"
     ],
     entry_points={
         "console_scripts": [
             "bam=bambot.cli:cli",
         ],
     },
     classifiers=[
```

### Comparing `bambot-0.3.7/tests/test_bambot.py` & `bambot-0.3.8/tests/test_bambot.py`

 * *Files identical despite different names*

