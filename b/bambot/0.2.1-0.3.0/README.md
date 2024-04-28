# Comparing `tmp/bambot-0.2.1.tar.gz` & `tmp/bambot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambot-0.2.1.tar", last modified: Sat Apr  6 23:22:46 2024, max compression
+gzip compressed data, was "bambot-0.3.0.tar", last modified: Sun Apr 28 23:22:58 2024, max compression
```

## Comparing `bambot-0.2.1.tar` & `bambot-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-06 23:22:46.578779 bambot-0.2.1/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1185 2024-04-06 23:22:46.578568 bambot-0.2.1/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      261 2024-04-06 20:04:16.000000 bambot-0.2.1/README.md
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-06 23:22:46.577265 bambot-0.2.1/bambot/
--rw-r--r--   0 spencerkinney   (501) staff       (20)       21 2024-04-06 20:30:19.000000 bambot-0.2.1/bambot/__init__.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     3132 2024-04-06 23:19:31.000000 bambot-0.2.1/bambot/core.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-06 23:22:46.578363 bambot-0.2.1/bambot.egg-info/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1185 2024-04-06 23:22:46.000000 bambot-0.2.1/bambot.egg-info/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      215 2024-04-06 23:22:46.000000 bambot-0.2.1/bambot.egg-info/SOURCES.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-04-06 23:22:46.000000 bambot-0.2.1/bambot.egg-info/dependency_links.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        9 2024-04-06 23:22:46.000000 bambot-0.2.1/bambot.egg-info/requires.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-04-06 23:22:46.000000 bambot-0.2.1/bambot.egg-info/top_level.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-04-06 23:22:46.578814 bambot-0.2.1/setup.cfg
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1130 2024-04-06 23:22:32.000000 bambot-0.2.1/setup.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-06 23:22:46.578050 bambot-0.2.1/tests/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1737 2024-04-06 22:55:58.000000 bambot-0.2.1/tests/test.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-28 23:22:58.669552 bambot-0.3.0/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      850 2024-04-28 23:22:58.669357 bambot-0.3.0/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      148 2024-04-27 21:13:32.000000 bambot-0.3.0/README.md
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-28 23:22:58.667409 bambot-0.3.0/bambot/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       60 2024-04-27 22:56:54.000000 bambot-0.3.0/bambot/__init__.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1832 2024-04-28 22:59:21.000000 bambot-0.3.0/bambot/agent.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     7078 2024-04-28 23:10:48.000000 bambot-0.3.0/bambot/cli.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2079 2024-04-28 23:07:57.000000 bambot-0.3.0/bambot/docker_utils.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      464 2024-04-28 23:09:41.000000 bambot-0.3.0/bambot/log_utils.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      709 2024-04-28 22:50:06.000000 bambot-0.3.0/bambot/logger.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      371 2024-04-28 08:09:43.000000 bambot-0.3.0/bambot/utils.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-28 23:22:58.669143 bambot-0.3.0/bambot.egg-info/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      850 2024-04-28 23:22:58.000000 bambot-0.3.0/bambot.egg-info/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      346 2024-04-28 23:22:58.000000 bambot-0.3.0/bambot.egg-info/SOURCES.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-04-28 23:22:58.000000 bambot-0.3.0/bambot.egg-info/dependency_links.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       39 2024-04-28 23:22:58.000000 bambot-0.3.0/bambot.egg-info/entry_points.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       18 2024-04-28 23:22:58.000000 bambot-0.3.0/bambot.egg-info/requires.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-04-28 23:22:58.000000 bambot-0.3.0/bambot.egg-info/top_level.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-04-28 23:22:58.669585 bambot-0.3.0/setup.cfg
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1065 2024-04-28 23:22:26.000000 bambot-0.3.0/setup.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-28 23:22:58.668752 bambot-0.3.0/tests/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1443 2024-04-27 21:53:17.000000 bambot-0.3.0/tests/test_bambot.py
```

### Comparing `bambot-0.2.1/PKG-INFO` & `bambot-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.2.1
-Summary: A Python package for interfacing with Bam foundational AI models.
+Version: 0.3.0
+Summary: Lightweight containers for AI agents
 Home-page: https://github.com/BamCorp/bambot
-Author: Bam Corp.
+Author: Bam Corp
 Author-email: spencer@bam.bot
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: requests
+Requires-Dist: click
+Requires-Dist: jinja2
+Requires-Dist: tqdm
 
 # Bambot
 
-Bambot is a Python package for interfacing with Bam foundational AI models which simplifies the process of integrating advanced data capabilities into your apps.
+Bambot is a container framework for AI agents
 
 ## Installation
 
 To install Bambot, run the following command:
-
 ```sh
 pip install bambot
+```
```

### Comparing `bambot-0.2.1/bambot.egg-info/PKG-INFO` & `bambot-0.3.0/bambot.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.2.1
-Summary: A Python package for interfacing with Bam foundational AI models.
+Version: 0.3.0
+Summary: Lightweight containers for AI agents
 Home-page: https://github.com/BamCorp/bambot
-Author: Bam Corp.
+Author: Bam Corp
 Author-email: spencer@bam.bot
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: requests
+Requires-Dist: click
+Requires-Dist: jinja2
+Requires-Dist: tqdm
 
 # Bambot
 
-Bambot is a Python package for interfacing with Bam foundational AI models which simplifies the process of integrating advanced data capabilities into your apps.
+Bambot is a container framework for AI agents
 
 ## Installation
 
 To install Bambot, run the following command:
-
 ```sh
 pip install bambot
+```
```

