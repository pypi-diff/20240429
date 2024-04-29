# Comparing `tmp/bambot-0.3.2.tar.gz` & `tmp/bambot-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambot-0.3.2.tar", last modified: Mon Apr 29 02:12:27 2024, max compression
+gzip compressed data, was "bambot-0.3.3.tar", last modified: Mon Apr 29 02:20:08 2024, max compression
```

## Comparing `bambot-0.3.2.tar` & `bambot-0.3.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:12:27.335438 bambot-0.3.2/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1003 2024-04-29 02:12:27.335151 bambot-0.3.2/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      148 2024-04-27 21:13:32.000000 bambot-0.3.2/README.md
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:12:27.331355 bambot-0.3.2/bambot/
--rw-r--r--   0 spencerkinney   (501) staff       (20)       60 2024-04-27 22:56:54.000000 bambot-0.3.2/bambot/__init__.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1832 2024-04-28 22:59:21.000000 bambot-0.3.2/bambot/agent.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     7544 2024-04-29 02:09:50.000000 bambot-0.3.2/bambot/cli.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     2079 2024-04-28 23:07:57.000000 bambot-0.3.2/bambot/docker_utils.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      464 2024-04-28 23:09:41.000000 bambot-0.3.2/bambot/log_utils.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      709 2024-04-28 22:50:06.000000 bambot-0.3.2/bambot/logger.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:12:27.334183 bambot-0.3.2/bambot/templates/
--rw-r--r--   0 spencerkinney   (501) staff       (20)      840 2024-04-28 07:24:46.000000 bambot-0.3.2/bambot/templates/Dockerfile.dashboard.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)      755 2024-04-28 07:24:56.000000 bambot-0.3.2/bambot/templates/Dockerfile.lightweight.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)       98 2024-04-27 20:00:14.000000 bambot-0.3.2/bambot/templates/Procfile.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)      559 2024-04-27 21:53:04.000000 bambot-0.3.2/bambot/templates/agent_readme.md.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)      332 2024-04-29 02:01:28.000000 bambot-0.3.2/bambot/templates/bot.py.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1862 2024-04-28 06:29:24.000000 bambot-0.3.2/bambot/templates/dashboard.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      296 2024-04-28 08:17:47.000000 bambot-0.3.2/bambot/templates/run.sh.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)      371 2024-04-28 08:09:43.000000 bambot-0.3.2/bambot/utils.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:12:27.334799 bambot-0.3.2/bambot.egg-info/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1003 2024-04-29 02:12:27.000000 bambot-0.3.2/bambot.egg-info/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      579 2024-04-29 02:12:27.000000 bambot-0.3.2/bambot.egg-info/SOURCES.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-04-29 02:12:27.000000 bambot-0.3.2/bambot.egg-info/dependency_links.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       39 2024-04-29 02:12:27.000000 bambot-0.3.2/bambot.egg-info/entry_points.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       18 2024-04-29 02:12:27.000000 bambot-0.3.2/bambot.egg-info/requires.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-04-29 02:12:27.000000 bambot-0.3.2/bambot.egg-info/top_level.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-04-29 02:12:27.335480 bambot-0.3.2/setup.cfg
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1266 2024-04-29 01:50:26.000000 bambot-0.3.2/setup.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:12:27.334513 bambot-0.3.2/tests/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1443 2024-04-27 21:53:17.000000 bambot-0.3.2/tests/test_bambot.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:20:08.810705 bambot-0.3.3/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1003 2024-04-29 02:20:08.810403 bambot-0.3.3/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      148 2024-04-27 21:13:32.000000 bambot-0.3.3/README.md
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:20:08.806458 bambot-0.3.3/bambot/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       60 2024-04-27 22:56:54.000000 bambot-0.3.3/bambot/__init__.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1832 2024-04-28 22:59:21.000000 bambot-0.3.3/bambot/agent.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     7643 2024-04-29 02:19:29.000000 bambot-0.3.3/bambot/cli.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2079 2024-04-28 23:07:57.000000 bambot-0.3.3/bambot/docker_utils.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      464 2024-04-28 23:09:41.000000 bambot-0.3.3/bambot/log_utils.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      709 2024-04-28 22:50:06.000000 bambot-0.3.3/bambot/logger.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:20:08.809294 bambot-0.3.3/bambot/templates/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      840 2024-04-28 07:24:46.000000 bambot-0.3.3/bambot/templates/Dockerfile.dashboard.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      755 2024-04-28 07:24:56.000000 bambot-0.3.3/bambot/templates/Dockerfile.lightweight.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       98 2024-04-27 20:00:14.000000 bambot-0.3.3/bambot/templates/Procfile.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      559 2024-04-27 21:53:04.000000 bambot-0.3.3/bambot/templates/agent_readme.md.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      332 2024-04-29 02:01:28.000000 bambot-0.3.3/bambot/templates/bot.py.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1862 2024-04-28 06:29:24.000000 bambot-0.3.3/bambot/templates/dashboard.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      296 2024-04-28 08:17:47.000000 bambot-0.3.3/bambot/templates/run.sh.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      371 2024-04-28 08:09:43.000000 bambot-0.3.3/bambot/utils.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:20:08.810037 bambot-0.3.3/bambot.egg-info/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1003 2024-04-29 02:20:08.000000 bambot-0.3.3/bambot.egg-info/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      579 2024-04-29 02:20:08.000000 bambot-0.3.3/bambot.egg-info/SOURCES.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-04-29 02:20:08.000000 bambot-0.3.3/bambot.egg-info/dependency_links.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       39 2024-04-29 02:20:08.000000 bambot-0.3.3/bambot.egg-info/entry_points.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       18 2024-04-29 02:20:08.000000 bambot-0.3.3/bambot.egg-info/requires.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-04-29 02:20:08.000000 bambot-0.3.3/bambot.egg-info/top_level.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-04-29 02:20:08.810808 bambot-0.3.3/setup.cfg
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1266 2024-04-29 02:19:03.000000 bambot-0.3.3/setup.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:20:08.809677 bambot-0.3.3/tests/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1443 2024-04-27 21:53:17.000000 bambot-0.3.3/tests/test_bambot.py
```

### Comparing `bambot-0.3.2/PKG-INFO` & `bambot-0.3.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.3.2
+Version: 0.3.3
 Summary: Lightweight containers for AI agents
 Home-page: https://github.com/BamCorp/bambot
 Author: Bam Corp
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bambot-0.3.2/bambot/agent.py` & `bambot-0.3.3/bambot/agent.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.2/bambot/cli.py` & `bambot-0.3.3/bambot/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # bambot/cli.py
 import os
 import click
 import shutil
-from jinja2 import Environment, PackageLoader
+from jinja2 import Environment, FileSystemLoader
+from pkg_resources import resource_filename
 from .docker_utils import DockerManager
 from .log_utils import LogManager
 from .utils import copy_template
 import subprocess
 import signal
 import sys
 import threading
 
-env = Environment(loader=PackageLoader("bambot", "templates"))
+templates_dir = resource_filename("bambot", "templates")
+env = Environment(loader=FileSystemLoader(templates_dir))
 
 def echo_error(message):
     click.echo(click.style(f"Error: {message}", fg="red"), err=True)
 
 def echo_warning(message):
     click.echo(click.style(f"Warning: {message}", fg="yellow"), err=True)
```

### Comparing `bambot-0.3.2/bambot/docker_utils.py` & `bambot-0.3.3/bambot/docker_utils.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.2/bambot/logger.py` & `bambot-0.3.3/bambot/logger.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.2/bambot/templates/Dockerfile.dashboard.j2` & `bambot-0.3.3/bambot/templates/Dockerfile.dashboard.j2`

 * *Files identical despite different names*

### Comparing `bambot-0.3.2/bambot/templates/Dockerfile.lightweight.j2` & `bambot-0.3.3/bambot/templates/Dockerfile.lightweight.j2`

 * *Files identical despite different names*

### Comparing `bambot-0.3.2/bambot/templates/agent_readme.md.j2` & `bambot-0.3.3/bambot/templates/agent_readme.md.j2`

 * *Files identical despite different names*

### Comparing `bambot-0.3.2/bambot/templates/dashboard.py` & `bambot-0.3.3/bambot/templates/dashboard.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.2/bambot.egg-info/PKG-INFO` & `bambot-0.3.3/bambot.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.3.2
+Version: 0.3.3
 Summary: Lightweight containers for AI agents
 Home-page: https://github.com/BamCorp/bambot
 Author: Bam Corp
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bambot-0.3.2/bambot.egg-info/SOURCES.txt` & `bambot-0.3.3/bambot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bambot-0.3.2/setup.py` & `bambot-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bambot",
-    version="0.3.2",
+    version="0.3.3",
     author="Bam Corp",
     author_email="spencer@bam.bot",
     description="Lightweight containers for AI agents",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BamCorp/bambot",
     packages=find_packages(),
```

### Comparing `bambot-0.3.2/tests/test_bambot.py` & `bambot-0.3.3/tests/test_bambot.py`

 * *Files identical despite different names*

