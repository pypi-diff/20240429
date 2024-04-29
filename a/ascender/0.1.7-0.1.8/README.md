# Comparing `tmp/ascender-0.1.7.tar.gz` & `tmp/ascender-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascender-0.1.7.tar", max compression
+gzip compressed data, was "ascender-0.1.8.tar", max compression
```

## Comparing `ascender-0.1.7.tar` & `ascender-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35148 2023-12-19 19:36:15.353783 ascender-0.1.7/LICENSE
--rw-r--r--   0        0        0      953 2023-12-19 20:05:30.701956 ascender-0.1.7/README.md
--rw-r--r--   0        0        0      146 2024-04-28 15:55:58.332495 ascender-0.1.7/ascender/app.py
--rw-r--r--   0        0        0     3239 2024-04-28 15:02:31.682934 ascender-0.1.7/ascender/commands/projects.py
--rw-r--r--   0        0        0     1840 2023-12-19 21:08:03.713265 ascender-0.1.7/ascender/commands/runner.py
--rw-r--r--   0        0        0      132 2023-12-19 20:00:44.526193 ascender-0.1.7/ascender/launch.py
--rw-r--r--   0        0        0     7706 2024-04-28 15:20:59.369015 ascender-0.1.7/ascender/logic/projects.py
--rw-r--r--   0        0        0     2468 2024-04-29 17:03:19.552544 ascender-0.1.7/ascender/logic/runner.py
--rw-r--r--   0        0        0     2630 2024-04-29 17:03:29.352633 ascender-0.1.7/ascender/logic/versions.py
--rw-r--r--   0        0        0      179 2024-01-04 18:50:06.046792 ascender-0.1.7/ascender/settings.py
--rw-r--r--   0        0        0      655 2024-04-29 17:04:00.887738 ascender-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 ascender-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-12-19 19:36:15.353783 ascender-0.1.8/LICENSE
+-rw-r--r--   0        0        0      953 2023-12-19 20:05:30.701956 ascender-0.1.8/README.md
+-rw-r--r--   0        0        0      146 2024-04-28 15:55:58.332495 ascender-0.1.8/ascender/app.py
+-rw-r--r--   0        0        0     3239 2024-04-28 15:02:31.682934 ascender-0.1.8/ascender/commands/projects.py
+-rw-r--r--   0        0        0     1840 2023-12-19 21:08:03.713265 ascender-0.1.8/ascender/commands/runner.py
+-rw-r--r--   0        0        0      132 2023-12-19 20:00:44.526193 ascender-0.1.8/ascender/launch.py
+-rw-r--r--   0        0        0     7706 2024-04-28 15:20:59.369015 ascender-0.1.8/ascender/logic/projects.py
+-rw-r--r--   0        0        0     2525 2024-04-29 17:07:50.542961 ascender-0.1.8/ascender/logic/runner.py
+-rw-r--r--   0        0        0     2630 2024-04-29 17:08:02.073555 ascender-0.1.8/ascender/logic/versions.py
+-rw-r--r--   0        0        0      179 2024-01-04 18:50:06.046792 ascender-0.1.8/ascender/settings.py
+-rw-r--r--   0        0        0      655 2024-04-29 17:08:10.620914 ascender-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 ascender-0.1.8/PKG-INFO
```

### Comparing `ascender-0.1.7/LICENSE` & `ascender-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ascender-0.1.7/README.md` & `ascender-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ascender-0.1.7/ascender/commands/projects.py` & `ascender-0.1.8/ascender/commands/projects.py`

 * *Files identical despite different names*

### Comparing `ascender-0.1.7/ascender/commands/runner.py` & `ascender-0.1.8/ascender/commands/runner.py`

 * *Files identical despite different names*

### Comparing `ascender-0.1.7/ascender/logic/projects.py` & `ascender-0.1.8/ascender/logic/projects.py`

 * *Files identical despite different names*

### Comparing `ascender-0.1.7/ascender/logic/runner.py` & `ascender-0.1.8/ascender/logic/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 class RunnerLogic:
     console: Console
 
     def __init__(self, console: Console, command: str | None = None) -> None:
         self.command = "" if not command else command
+        self.toml_path = f"{os.getcwd()}/pyproject.toml"
         self.console = console
     
     def is_project(self):
         """
         Check if the current directory is an AscenderFramework project or not.
         """
         directory = os.getcwd()
```

### Comparing `ascender-0.1.7/ascender/logic/versions.py` & `ascender-0.1.8/ascender/logic/versions.py`

 * *Files identical despite different names*

### Comparing `ascender-0.1.7/pyproject.toml` & `ascender-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ascender"
-version = "0.1.7"
+version = "0.1.8"
 description = "The CLI tool for working with AscenderFramework: Installation, command execution and version management"
 authors = ["AscenderTeam"]
 repository = "https://github.com/AscenderTeam/AscenderCLI"
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `ascender-0.1.7/PKG-INFO` & `ascender-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascender
-Version: 0.1.7
+Version: 0.1.8
 Summary: The CLI tool for working with AscenderFramework: Installation, command execution and version management
 Home-page: https://github.com/AscenderTeam/AscenderCLI
 License: GPL-3.0
 Author: AscenderTeam
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

