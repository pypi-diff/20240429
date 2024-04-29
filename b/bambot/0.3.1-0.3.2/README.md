# Comparing `tmp/bambot-0.3.1.tar.gz` & `tmp/bambot-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambot-0.3.1.tar", last modified: Mon Apr 29 00:03:28 2024, max compression
+gzip compressed data, was "bambot-0.3.2.tar", last modified: Mon Apr 29 02:12:27 2024, max compression
```

## Comparing `bambot-0.3.1.tar` & `bambot-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 00:03:28.988305 bambot-0.3.1/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1003 2024-04-29 00:03:28.988094 bambot-0.3.1/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      148 2024-04-27 21:13:32.000000 bambot-0.3.1/README.md
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 00:03:28.986493 bambot-0.3.1/bambot/
--rw-r--r--   0 spencerkinney   (501) staff       (20)       60 2024-04-27 22:56:54.000000 bambot-0.3.1/bambot/__init__.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1832 2024-04-28 22:59:21.000000 bambot-0.3.1/bambot/agent.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     7078 2024-04-28 23:10:48.000000 bambot-0.3.1/bambot/cli.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     2079 2024-04-28 23:07:57.000000 bambot-0.3.1/bambot/docker_utils.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      464 2024-04-28 23:09:41.000000 bambot-0.3.1/bambot/log_utils.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      709 2024-04-28 22:50:06.000000 bambot-0.3.1/bambot/logger.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      371 2024-04-28 08:09:43.000000 bambot-0.3.1/bambot/utils.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 00:03:28.987865 bambot-0.3.1/bambot.egg-info/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1003 2024-04-29 00:03:28.000000 bambot-0.3.1/bambot.egg-info/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      346 2024-04-29 00:03:28.000000 bambot-0.3.1/bambot.egg-info/SOURCES.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-04-29 00:03:28.000000 bambot-0.3.1/bambot.egg-info/dependency_links.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       39 2024-04-29 00:03:28.000000 bambot-0.3.1/bambot.egg-info/entry_points.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       18 2024-04-29 00:03:28.000000 bambot-0.3.1/bambot.egg-info/requires.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-04-29 00:03:28.000000 bambot-0.3.1/bambot.egg-info/top_level.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-04-29 00:03:28.988342 bambot-0.3.1/setup.cfg
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1205 2024-04-29 00:03:20.000000 bambot-0.3.1/setup.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 00:03:28.987541 bambot-0.3.1/tests/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1443 2024-04-27 21:53:17.000000 bambot-0.3.1/tests/test_bambot.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:12:27.335438 bambot-0.3.2/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1003 2024-04-29 02:12:27.335151 bambot-0.3.2/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      148 2024-04-27 21:13:32.000000 bambot-0.3.2/README.md
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:12:27.331355 bambot-0.3.2/bambot/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       60 2024-04-27 22:56:54.000000 bambot-0.3.2/bambot/__init__.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1832 2024-04-28 22:59:21.000000 bambot-0.3.2/bambot/agent.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     7544 2024-04-29 02:09:50.000000 bambot-0.3.2/bambot/cli.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2079 2024-04-28 23:07:57.000000 bambot-0.3.2/bambot/docker_utils.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      464 2024-04-28 23:09:41.000000 bambot-0.3.2/bambot/log_utils.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      709 2024-04-28 22:50:06.000000 bambot-0.3.2/bambot/logger.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:12:27.334183 bambot-0.3.2/bambot/templates/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      840 2024-04-28 07:24:46.000000 bambot-0.3.2/bambot/templates/Dockerfile.dashboard.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      755 2024-04-28 07:24:56.000000 bambot-0.3.2/bambot/templates/Dockerfile.lightweight.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       98 2024-04-27 20:00:14.000000 bambot-0.3.2/bambot/templates/Procfile.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      559 2024-04-27 21:53:04.000000 bambot-0.3.2/bambot/templates/agent_readme.md.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      332 2024-04-29 02:01:28.000000 bambot-0.3.2/bambot/templates/bot.py.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1862 2024-04-28 06:29:24.000000 bambot-0.3.2/bambot/templates/dashboard.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      296 2024-04-28 08:17:47.000000 bambot-0.3.2/bambot/templates/run.sh.j2
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      371 2024-04-28 08:09:43.000000 bambot-0.3.2/bambot/utils.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:12:27.334799 bambot-0.3.2/bambot.egg-info/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1003 2024-04-29 02:12:27.000000 bambot-0.3.2/bambot.egg-info/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      579 2024-04-29 02:12:27.000000 bambot-0.3.2/bambot.egg-info/SOURCES.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-04-29 02:12:27.000000 bambot-0.3.2/bambot.egg-info/dependency_links.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       39 2024-04-29 02:12:27.000000 bambot-0.3.2/bambot.egg-info/entry_points.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       18 2024-04-29 02:12:27.000000 bambot-0.3.2/bambot.egg-info/requires.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-04-29 02:12:27.000000 bambot-0.3.2/bambot.egg-info/top_level.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-04-29 02:12:27.335480 bambot-0.3.2/setup.cfg
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1266 2024-04-29 01:50:26.000000 bambot-0.3.2/setup.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-29 02:12:27.334513 bambot-0.3.2/tests/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1443 2024-04-27 21:53:17.000000 bambot-0.3.2/tests/test_bambot.py
```

### Comparing `bambot-0.3.1/PKG-INFO` & `bambot-0.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.3.1
+Version: 0.3.2
 Summary: Lightweight containers for AI agents
 Home-page: https://github.com/BamCorp/bambot
 Author: Bam Corp
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bambot-0.3.1/bambot/agent.py` & `bambot-0.3.2/bambot/agent.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.1/bambot/cli.py` & `bambot-0.3.2/bambot/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,30 +47,40 @@
 @click.option("--include-dashboard", "-d", is_flag=True, help="Include the Streamlit dashboard in the Docker image.")
 def build(bot_file, include_dashboard):
     """Build and generate deployment files for an AI agent."""
     bot_dir = os.getcwd()
     bot_path = os.path.join(bot_dir, bot_file)
 
     if not os.path.exists(bot_path):
-        echo_error(f"{bot_file} not found in the current directory.")
-        return
+        echo_warning(f"{bot_file} not found in the current directory.")
+        generate_default = click.confirm(
+            f"To continue, you must provide a {bot_file} file. Generate a default one?",
+            default=True,
+        )
+        if generate_default:
+            copy_template(env, "bot.py.j2", bot_path)
+            echo_info(f"Generated default {bot_file} file. Customize it to add your AI agent logic.")
+        else:
+            echo_info(f"Please create a {bot_file} file and run 'bam build' again.")
+            echo_info(f"Refer to GitHub for examples or help: https://github.com/Bam-Corp/bambot")
+            return
 
     docker_manager = DockerManager()
 
     if not docker_manager.is_docker_running():
         echo_error("Docker daemon is not running.")
         echo_warning("Please start the Docker daemon and try again.")
         echo_info("You can check the status of the Docker daemon using the following command:")
         echo_info("  docker info")
         echo_info("If Docker is not installed, you can download it from https://www.docker.com/get-started")
         return
 
     try:
         echo_info("Cleaning up unused containers and images...")
-        confirm_cleanup = click.confirm("Remove unused containers and images? Skip this step with 'No'", default=False)
+        confirm_cleanup = click.confirm("Remove unused containers and images? [y/N]", default=False)
         if confirm_cleanup:
             docker_manager.cleanup()
         else:
             echo_info("Skipping cleanup operation.")
 
         echo_info("Generating deployment files...")
         if include_dashboard:
@@ -79,15 +89,14 @@
         else:
             copy_template(env, "Dockerfile.lightweight.j2", os.path.join(bot_dir, "Dockerfile"))
             include_dashboard_value = "false"
         copy_template(env, "Procfile.j2", os.path.join(bot_dir, "Procfile"))
         copy_template(env, "agent_readme.md.j2", os.path.join(bot_dir, "agent_readme.md"))
         copy_template(env, "run.sh.j2", os.path.join(bot_dir, "run.sh"), include_dashboard=include_dashboard_value)
 
-        # Create a configuration file with the include_dashboard value
         config_file_path = os.path.join(bot_dir, "bambot.config")
         with open(config_file_path, "w") as config_file:
             config_file.write(f"include_dashboard={include_dashboard}")
 
         echo_info("Building Bam container image...")
         docker_manager.build_image(include_dashboard)
```

### Comparing `bambot-0.3.1/bambot/docker_utils.py` & `bambot-0.3.2/bambot/docker_utils.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.1/bambot/logger.py` & `bambot-0.3.2/bambot/logger.py`

 * *Files identical despite different names*

### Comparing `bambot-0.3.1/bambot.egg-info/PKG-INFO` & `bambot-0.3.2/bambot.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.3.1
+Version: 0.3.2
 Summary: Lightweight containers for AI agents
 Home-page: https://github.com/BamCorp/bambot
 Author: Bam Corp
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bambot-0.3.1/setup.py` & `bambot-0.3.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bambot",
-    version="0.3.1",
+    version="0.3.2",
     author="Bam Corp",
     author_email="spencer@bam.bot",
     description="Lightweight containers for AI agents",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BamCorp/bambot",
     packages=find_packages(),
+    package_data={
+        "bambot": ["templates/*"],
+    },
     install_requires=[
         "click",
         "jinja2",
         "tqdm",
     ],
     entry_points={
         "console_scripts": [
```

### Comparing `bambot-0.3.1/tests/test_bambot.py` & `bambot-0.3.2/tests/test_bambot.py`

 * *Files identical despite different names*

