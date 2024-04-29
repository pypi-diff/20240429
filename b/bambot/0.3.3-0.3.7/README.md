# Comparing `tmp/bambot-0.3.3.tar.gz` & `tmp/bambot-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambot-0.3.3.tar", last modified: Mon Apr 29 02:20:08 2024, max compression
+gzip compressed data, was "bambot-0.3.7.tar", last modified: Mon Apr 29 04:47:37 2024, max compression
```

## Comparing `bambot-0.3.3.tar` & `bambot-0.3.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:20:08.810705 bambot-0.3.3/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1003 2024-04-29 02:20:08.810403 bambot-0.3.3/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      148 2024-04-27 21:13:32.000000 bambot-0.3.3/README.md
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:20:08.806458 bambot-0.3.3/bambot/
--rw-r--r--   0 spencerkinney   (501) staff       (20)       60 2024-04-27 22:56:54.000000 bambot-0.3.3/bambot/__init__.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1832 2024-04-28 22:59:21.000000 bambot-0.3.3/bambot/agent.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     7643 2024-04-29 02:19:29.000000 bambot-0.3.3/bambot/cli.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     2079 2024-04-28 23:07:57.000000 bambot-0.3.3/bambot/docker_utils.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      464 2024-04-28 23:09:41.000000 bambot-0.3.3/bambot/log_utils.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      709 2024-04-28 22:50:06.000000 bambot-0.3.3/bambot/logger.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:20:08.809294 bambot-0.3.3/bambot/templates/
--rw-r--r--   0 spencerkinney   (501) staff       (20)      840 2024-04-28 07:24:46.000000 bambot-0.3.3/bambot/templates/Dockerfile.dashboard.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)      755 2024-04-28 07:24:56.000000 bambot-0.3.3/bambot/templates/Dockerfile.lightweight.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)       98 2024-04-27 20:00:14.000000 bambot-0.3.3/bambot/templates/Procfile.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)      559 2024-04-27 21:53:04.000000 bambot-0.3.3/bambot/templates/agent_readme.md.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)      332 2024-04-29 02:01:28.000000 bambot-0.3.3/bambot/templates/bot.py.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1862 2024-04-28 06:29:24.000000 bambot-0.3.3/bambot/templates/dashboard.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      296 2024-04-28 08:17:47.000000 bambot-0.3.3/bambot/templates/run.sh.j2
--rw-r--r--   0 spencerkinney   (501) staff       (20)      371 2024-04-28 08:09:43.000000 bambot-0.3.3/bambot/utils.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:20:08.810037 bambot-0.3.3/bambot.egg-info/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1003 2024-04-29 02:20:08.000000 bambot-0.3.3/bambot.egg-info/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      579 2024-04-29 02:20:08.000000 bambot-0.3.3/bambot.egg-info/SOURCES.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-04-29 02:20:08.000000 bambot-0.3.3/bambot.egg-info/dependency_links.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       39 2024-04-29 02:20:08.000000 bambot-0.3.3/bambot.egg-info/entry_points.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       18 2024-04-29 02:20:08.000000 bambot-0.3.3/bambot.egg-info/requires.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-04-29 02:20:08.000000 bambot-0.3.3/bambot.egg-info/top_level.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-04-29 02:20:08.810808 bambot-0.3.3/setup.cfg
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1266 2024-04-29 02:19:03.000000 bambot-0.3.3/setup.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:20:08.809677 bambot-0.3.3/tests/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1443 2024-04-27 21:53:17.000000 bambot-0.3.3/tests/test_bambot.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 04:47:37.484378 bambot-0.3.7/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1027 2024-04-29 04:47:37.484055 bambot-0.3.7/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      148 2024-04-27 21:13:32.000000 bambot-0.3.7/README.md
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 04:47:37.480764 bambot-0.3.7/bambot/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       60 2024-04-27 22:56:54.000000 bambot-0.3.7/bambot/__init__.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1832 2024-04-28 22:59:21.000000 bambot-0.3.7/bambot/agent.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     7479 2024-04-29 04:41:54.000000 bambot-0.3.7/bambot/cli.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     7127 2024-04-29 04:38:11.000000 bambot-0.3.7/bambot/docker_utils.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      464 2024-04-28 23:09:41.000000 bambot-0.3.7/bambot/log_utils.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      708 2024-04-29 03:05:28.000000 bambot-0.3.7/bambot/logger.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2016 2024-04-29 03:00:30.000000 bambot-0.3.7/bambot/remote_utils.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 04:47:37.483182 bambot-0.3.7/bambot/templates/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1103 2024-04-29 04:41:19.000000 bambot-0.3.7/bambot/templates/Dockerfile.dashboard.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1020 2024-04-29 04:41:13.000000 bambot-0.3.7/bambot/templates/Dockerfile.lightweight.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       98 2024-04-27 20:00:14.000000 bambot-0.3.7/bambot/templates/Procfile.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      559 2024-04-27 21:53:04.000000 bambot-0.3.7/bambot/templates/agent_readme.md.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      332 2024-04-29 02:01:28.000000 bambot-0.3.7/bambot/templates/bot.py.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1862 2024-04-28 06:29:24.000000 bambot-0.3.7/bambot/templates/dashboard.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      296 2024-04-28 08:17:47.000000 bambot-0.3.7/bambot/templates/run.sh.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      371 2024-04-28 08:09:43.000000 bambot-0.3.7/bambot/utils.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 04:47:37.483688 bambot-0.3.7/bambot.egg-info/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1027 2024-04-29 04:47:37.000000 bambot-0.3.7/bambot.egg-info/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      602 2024-04-29 04:47:37.000000 bambot-0.3.7/bambot.egg-info/SOURCES.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-04-29 04:47:37.000000 bambot-0.3.7/bambot.egg-info/dependency_links.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       39 2024-04-29 04:47:37.000000 bambot-0.3.7/bambot.egg-info/entry_points.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       27 2024-04-29 04:47:37.000000 bambot-0.3.7/bambot.egg-info/requires.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-04-29 04:47:37.000000 bambot-0.3.7/bambot.egg-info/top_level.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-04-29 04:47:37.484428 bambot-0.3.7/setup.cfg
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1296 2024-04-29 04:47:24.000000 bambot-0.3.7/setup.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 04:47:37.483454 bambot-0.3.7/tests/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1443 2024-04-27 21:53:17.000000 bambot-0.3.7/tests/test_bambot.py
```

### Comparing `bambot-0.3.3/PKG-INFO` & `bambot-0.3.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.3.3
+Version: 0.3.7
 Summary: Lightweight containers for AI agents
 Home-page: https://github.com/BamCorp/bambot
 Author: Bam Corp
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: jinja2
 Requires-Dist: tqdm
+Requires-Dist: requests
 
 # Bambot
 
 Bambot is a container framework for AI agents
 
 ## Installation
```

### Comparing `bambot-0.3.3/bambot/agent.py` & `bambot-0.3.7/bambot/agent.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.3/bambot/cli.py` & `bambot-0.3.7/bambot/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 import click
 import shutil
 from jinja2 import Environment, FileSystemLoader
 from pkg_resources import resource_filename
 from .docker_utils import DockerManager
 from .log_utils import LogManager
 from .utils import copy_template
-import subprocess
 import signal
-import sys
 import threading
 
+
 templates_dir = resource_filename("bambot", "templates")
 env = Environment(loader=FileSystemLoader(templates_dir))
 
 def echo_error(message):
     click.echo(click.style(f"Error: {message}", fg="red"), err=True)
 
 def echo_warning(message):
@@ -96,20 +95,24 @@
         copy_template(env, "run.sh.j2", os.path.join(bot_dir, "run.sh"), include_dashboard=include_dashboard_value)
 
         config_file_path = os.path.join(bot_dir, "bambot.config")
         with open(config_file_path, "w") as config_file:
             config_file.write(f"include_dashboard={include_dashboard}")
 
         echo_info("Building Bam container image...")
-        docker_manager.build_image(include_dashboard)
+        try:
+            docker_manager.build_image(include_dashboard)
+        except RuntimeError as e:
+            echo_error(f"Failed to build Docker image: {str(e)}")
+            return
 
         echo_info("Deployment files prepared successfully!")
         echo_info("You can now run the 'bam run' command to start your AI agent container.")
     except Exception as e:
-        echo_error(str(e))
+        echo_error(f"An unexpected error occurred: {str(e)}")
 
 @cli.command()
 @click.option("--bot-file", "-b", default="bot.py", help="Name of the bot file (e.g., my_bot.py).")
 def run(bot_file):
     """Run an AI agent locally."""
     bot_dir = os.getcwd()
     bot_path = os.path.join(bot_dir, bot_file)
@@ -164,22 +167,14 @@
         # Terminate the log thread
         log_thread.join(timeout=5)
 
         echo_info("AI agent execution completed.")
     except Exception as e:
         echo_error(str(e))
 
-
-def run_streamlit_app():
-    try:
-        os.chdir("bambot")  # Change to the bambot directory
-        subprocess.run(["python", "-m", "streamlit", "run", "dashboard.py", "--server.port=8501", "--server.address=0.0.0.0"])
-    except Exception as e:
-        echo_error(f"Error running Streamlit app: {e}")
-
 @cli.command()
 def clean():
     """Clean up generated deployment files."""
     bot_dir = os.getcwd()
     files_to_remove = [
         "Dockerfile",
         "Procfile",
```

### Comparing `bambot-0.3.3/bambot/logger.py` & `bambot-0.3.7/bambot/logger.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 
     def error(self, message):
         self.logger.error(message)
 
     def stop(self):
         for handler in self.logger.handlers:
             handler.close()
-        self.logger.removeHandler(handler)
+        self.logger.removeHandler(handler)
```

### Comparing `bambot-0.3.3/bambot/templates/Dockerfile.dashboard.j2` & `bambot-0.3.7/bambot/templates/Dockerfile.dashboard.j2`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,32 @@
+# bambot/templates/Dockerfile.dashboard.j2
 FROM python:3.9-bullseye
 
 WORKDIR /app
 
 # Install required packages for pyarrow
 RUN apt-get update && apt-get install -y \
     cmake \
     build-essential \
     && rm -rf /var/lib/apt/lists/*
 
-# Install Python dependencies
-COPY requirements.txt ./
+# Install required packages for the app
+RUN pip install --no-cache-dir click tqdm jinja2 requests
+
+# Copy the requirements.txt file if it exists, otherwise create an empty file
+COPY requirements.txt* ./
+RUN touch requirements.txt
+
+# Install additional packages from requirements.txt
 RUN pip install --no-cache-dir -r requirements.txt \
     && pip install --no-cache-dir "pyarrow==10.0.1" \
     && pip install --no-cache-dir streamlit
 
 # Copy the bot file and bambot directory
-COPY {{ bot_file }} ./
+COPY bot.py ./
 COPY bambot/ bambot/
 
 # Set the PYTHONUNBUFFERED environment variable to ensure real-time output
 ENV PYTHONUNBUFFERED=1
 
 # Disable Python's generation of .pyc files
 ENV PYTHONDONTWRITEBYTECODE=1
```

### Comparing `bambot-0.3.3/bambot/templates/Dockerfile.lightweight.j2` & `bambot-0.3.7/bambot/templates/Dockerfile.lightweight.j2`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,33 @@
+# bambot/templates/Dockerfile.lightweight.j2
 FROM python:3.9-alpine
 
 WORKDIR /app
 
 # Install the required packages
 RUN apk add --no-cache \
     build-base \
     musl-dev \
     libffi-dev
 
 # Copy the bambot directory
 COPY bambot/ bambot/
 
-# Install Python dependencies
-COPY requirements.txt ./
+# Install required packages for the app
+RUN pip install --no-cache-dir click tqdm jinja2 requests
+
+# Copy the requirements.txt file if it exists, otherwise create an empty file
+COPY requirements.txt* ./
+RUN touch requirements.txt
+
+# Install additional packages from requirements.txt
 RUN pip install --no-cache-dir -r requirements.txt
 
 # Copy the bot file
-COPY {{ bot_file }} ./
+COPY bot.py ./
 
 # Remove the build dependencies
 RUN apk del \
     build-base \
     musl-dev \
     libffi-dev
```

### Comparing `bambot-0.3.3/bambot/templates/agent_readme.md.j2` & `bambot-0.3.7/bambot/templates/agent_readme.md.j2`

 * *Files identical despite different names*

### Comparing `bambot-0.3.3/bambot/templates/dashboard.py` & `bambot-0.3.7/bambot/templates/dashboard.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.3/bambot.egg-info/PKG-INFO` & `bambot-0.3.7/bambot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.3.3
+Version: 0.3.7
 Summary: Lightweight containers for AI agents
 Home-page: https://github.com/BamCorp/bambot
 Author: Bam Corp
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: jinja2
 Requires-Dist: tqdm
+Requires-Dist: requests
 
 # Bambot
 
 Bambot is a container framework for AI agents
 
 ## Installation
```

### Comparing `bambot-0.3.3/bambot.egg-info/SOURCES.txt` & `bambot-0.3.7/bambot.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 setup.py
 bambot/__init__.py
 bambot/agent.py
 bambot/cli.py
 bambot/docker_utils.py
 bambot/log_utils.py
 bambot/logger.py
+bambot/remote_utils.py
 bambot/utils.py
 bambot.egg-info/PKG-INFO
 bambot.egg-info/SOURCES.txt
 bambot.egg-info/dependency_links.txt
 bambot.egg-info/entry_points.txt
 bambot.egg-info/requires.txt
 bambot.egg-info/top_level.txt
```

### Comparing `bambot-0.3.3/setup.py` & `bambot-0.3.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
+# setup.py
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bambot",
-    version="0.3.3",
+    version="0.3.7",
     author="Bam Corp",
     author_email="spencer@bam.bot",
     description="Lightweight containers for AI agents",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BamCorp/bambot",
     packages=find_packages(),
     package_data={
-        "bambot": ["templates/*"],
+        "bambot": ["templates/*"]
     },
     install_requires=[
         "click",
         "jinja2",
         "tqdm",
+        "requests",
     ],
     entry_points={
         "console_scripts": [
             "bam=bambot.cli:cli",
         ],
     },
     classifiers=[
```

### Comparing `bambot-0.3.3/tests/test_bambot.py` & `bambot-0.3.7/tests/test_bambot.py`

 * *Files identical despite different names*

