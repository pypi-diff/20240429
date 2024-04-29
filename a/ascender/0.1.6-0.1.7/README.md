# Comparing `tmp/ascender-0.1.6.tar.gz` & `tmp/ascender-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascender-0.1.6.tar", max compression
+gzip compressed data, was "ascender-0.1.7.tar", max compression
```

## Comparing `ascender-0.1.6.tar` & `ascender-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35148 2023-12-19 19:36:15.353783 ascender-0.1.6/LICENSE
--rw-r--r--   0        0        0      953 2023-12-19 20:05:30.701956 ascender-0.1.6/README.md
--rw-r--r--   0        0        0      146 2023-12-19 20:01:36.639816 ascender-0.1.6/ascender/app.py
--rw-r--r--   0        0        0     3239 2024-04-28 15:02:31.682934 ascender-0.1.6/ascender/commands/projects.py
--rw-r--r--   0        0        0     1840 2023-12-19 21:08:03.713265 ascender-0.1.6/ascender/commands/runner.py
--rw-r--r--   0        0        0      132 2023-12-19 20:00:44.526193 ascender-0.1.6/ascender/launch.py
--rw-r--r--   0        0        0     7706 2024-04-28 15:20:59.369015 ascender-0.1.6/ascender/logic/projects.py
--rw-r--r--   0        0        0     2278 2023-12-19 20:29:16.219795 ascender-0.1.6/ascender/logic/runner.py
--rw-r--r--   0        0        0     2462 2024-04-28 15:09:06.733790 ascender-0.1.6/ascender/logic/versions.py
--rw-r--r--   0        0        0      179 2024-01-04 18:50:06.046792 ascender-0.1.6/ascender/settings.py
--rw-r--r--   0        0        0      655 2024-04-28 15:21:09.881646 ascender-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 ascender-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-12-19 19:36:15.353783 ascender-0.1.7/LICENSE
+-rw-r--r--   0        0        0      953 2023-12-19 20:05:30.701956 ascender-0.1.7/README.md
+-rw-r--r--   0        0        0      146 2024-04-28 15:55:58.332495 ascender-0.1.7/ascender/app.py
+-rw-r--r--   0        0        0     3239 2024-04-28 15:02:31.682934 ascender-0.1.7/ascender/commands/projects.py
+-rw-r--r--   0        0        0     1840 2023-12-19 21:08:03.713265 ascender-0.1.7/ascender/commands/runner.py
+-rw-r--r--   0        0        0      132 2023-12-19 20:00:44.526193 ascender-0.1.7/ascender/launch.py
+-rw-r--r--   0        0        0     7706 2024-04-28 15:20:59.369015 ascender-0.1.7/ascender/logic/projects.py
+-rw-r--r--   0        0        0     2468 2024-04-29 17:03:19.552544 ascender-0.1.7/ascender/logic/runner.py
+-rw-r--r--   0        0        0     2630 2024-04-29 17:03:29.352633 ascender-0.1.7/ascender/logic/versions.py
+-rw-r--r--   0        0        0      179 2024-01-04 18:50:06.046792 ascender-0.1.7/ascender/settings.py
+-rw-r--r--   0        0        0      655 2024-04-29 17:04:00.887738 ascender-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 ascender-0.1.7/PKG-INFO
```

### Comparing `ascender-0.1.6/LICENSE` & `ascender-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ascender-0.1.6/README.md` & `ascender-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ascender-0.1.6/ascender/commands/projects.py` & `ascender-0.1.7/ascender/commands/projects.py`

 * *Files identical despite different names*

### Comparing `ascender-0.1.6/ascender/commands/runner.py` & `ascender-0.1.7/ascender/commands/runner.py`

 * *Files identical despite different names*

### Comparing `ascender-0.1.6/ascender/logic/projects.py` & `ascender-0.1.7/ascender/logic/projects.py`

 * *Files identical despite different names*

### Comparing `ascender-0.1.6/ascender/logic/runner.py` & `ascender-0.1.7/ascender/logic/runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from rich.console import Console
+from toml import load
 
 import os
 import subprocess
 
 from ascender.settings import IS_UNIX
 
 
@@ -15,15 +16,19 @@
     
     def is_project(self):
         """
         Check if the current directory is an AscenderFramework project or not.
         """
         directory = os.getcwd()
 
-        if os.path.exists(f"{directory}/.asc_venv") and os.path.exists(f"{directory}/start.py") and os.path.exists(f"{directory}/core"):
+        if os.path.exists(f"{directory}/start.py") and os.path.exists(f"{directory}/core") and os.path.exists(f"{directory}/pyproject.toml"):
+            toml_data = load(self.toml_path)
+            if toml_data["tool"]["poetry"]["name"] != "ascender-framework":
+                return False
+            
             return True
 
     def invoke(self):
         if not self.is_project():
             self.console.print("[red]Error:[/red] [bold]Cannot recognize project directory[/bold]")
             self.console.print("[bold yellow]Make sure you are in the root of any AscenderFramework project.[/bold yellow]")
             return
```

### Comparing `ascender-0.1.6/ascender/logic/versions.py` & `ascender-0.1.7/ascender/logic/versions.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,19 @@
     
     def is_project(self):
         """
         Check if the current directory is an AscenderFramework project or not.
         """
         directory = os.getcwd()
 
-        if os.path.exists(f"{directory}/.asc_venv") and os.path.exists(f"{directory}/start.py") and os.path.exists(f"{directory}/core"):
+        if os.path.exists(f"{directory}/start.py") and os.path.exists(f"{directory}/core") and os.path.exists(f"{directory}/pyproject.toml"):
+            toml_data = load(self.toml_path)
+            if toml_data["tool"]["poetry"]["name"] != "ascender-framework":
+                return False
+            
             return True
 
     def get_versions(self):
         repo_name = "AscenderTeam/AscenderFramework"
         url = f"https://api.github.com/repos/{repo_name}/releases"
 
         response = requests.get(url)
```

### Comparing `ascender-0.1.6/pyproject.toml` & `ascender-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ascender"
-version = "0.1.6"
+version = "0.1.7"
 description = "The CLI tool for working with AscenderFramework: Installation, command execution and version management"
 authors = ["AscenderTeam"]
 repository = "https://github.com/AscenderTeam/AscenderCLI"
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `ascender-0.1.6/PKG-INFO` & `ascender-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascender
-Version: 0.1.6
+Version: 0.1.7
 Summary: The CLI tool for working with AscenderFramework: Installation, command execution and version management
 Home-page: https://github.com/AscenderTeam/AscenderCLI
 License: GPL-3.0
 Author: AscenderTeam
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

