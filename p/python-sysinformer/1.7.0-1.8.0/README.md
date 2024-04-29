# Comparing `tmp/python_sysinformer-1.7.0.tar.gz` & `tmp/python_sysinformer-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_sysinformer-1.7.0.tar", max compression
+gzip compressed data, was "python_sysinformer-1.8.0.tar", max compression
```

## Comparing `python_sysinformer-1.7.0.tar` & `python_sysinformer-1.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2024-04-29 02:43:11.603674 python_sysinformer-1.7.0/LICENSE
--rw-r--r--   0        0        0     5404 2024-04-29 02:43:11.603674 python_sysinformer-1.7.0/README.md
--rw-r--r--   0        0        0     1593 2024-04-29 02:43:40.263374 python_sysinformer-1.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-29 02:43:11.607674 python_sysinformer-1.7.0/src/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 02:43:11.607674 python_sysinformer-1.7.0/src/config/__init__.py
--rw-r--r--   0        0        0     1102 2024-04-29 02:43:11.607674 python_sysinformer-1.7.0/src/config/config_parser.py
--rw-r--r--   0        0        0     1233 2024-04-29 02:43:11.607674 python_sysinformer-1.7.0/src/config/default_config.py
--rw-r--r--   0        0        0      221 2024-04-29 02:43:11.607674 python_sysinformer-1.7.0/src/constants.py
--rw-r--r--   0        0        0        0 2024-04-29 02:43:11.607674 python_sysinformer-1.7.0/src/core/__init__.py
--rw-r--r--   0        0        0     4448 2024-04-29 02:43:11.607674 python_sysinformer-1.7.0/src/core/containers.py
--rw-r--r--   0        0        0     6261 2024-04-29 02:43:11.607674 python_sysinformer-1.7.0/src/core/cpu.py
--rw-r--r--   0        0        0     2041 2024-04-29 02:43:11.607674 python_sysinformer-1.7.0/src/core/disks.py
--rw-r--r--   0        0        0     3745 2024-04-29 02:43:11.607674 python_sysinformer-1.7.0/src/core/latency.py
--rw-r--r--   0        0        0     5730 2024-04-29 02:43:11.607674 python_sysinformer-1.7.0/src/core/memory.py
--rw-r--r--   0        0        0     2597 2024-04-29 02:43:11.611674 python_sysinformer-1.7.0/src/core/networking.py
--rw-r--r--   0        0        0     2764 2024-04-29 02:43:11.611674 python_sysinformer-1.7.0/src/core/processes.py
--rw-r--r--   0        0        0     2605 2024-04-29 02:43:11.611674 python_sysinformer-1.7.0/src/core/services.py
--rw-r--r--   0        0        0     5877 2024-04-29 02:43:11.611674 python_sysinformer-1.7.0/src/core/system.py
--rw-r--r--   0        0        0     4417 2024-04-29 02:43:11.611674 python_sysinformer-1.7.0/src/main.py
--rw-r--r--   0        0        0        0 2024-04-29 02:43:11.611674 python_sysinformer-1.7.0/src/utilities/__init__.py
--rw-r--r--   0        0        0      442 2024-04-29 02:43:11.611674 python_sysinformer-1.7.0/src/utilities/exceptions.py
--rw-r--r--   0        0        0      560 2024-04-29 02:43:11.611674 python_sysinformer-1.7.0/src/utilities/utils.py
--rw-r--r--   0        0        0     6124 1970-01-01 00:00:00.000000 python_sysinformer-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-29 15:58:52.052566 python_sysinformer-1.8.0/LICENSE
+-rw-r--r--   0        0        0     5404 2024-04-29 15:58:52.052566 python_sysinformer-1.8.0/README.md
+-rw-r--r--   0        0        0     1623 2024-04-29 15:59:19.648468 python_sysinformer-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/config/__init__.py
+-rw-r--r--   0        0        0     1102 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/config/config_parser.py
+-rw-r--r--   0        0        0     1233 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/config/default_config.py
+-rw-r--r--   0        0        0      221 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/constants.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/core/__init__.py
+-rw-r--r--   0        0        0     4448 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/core/containers.py
+-rw-r--r--   0        0        0     6261 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/core/cpu.py
+-rw-r--r--   0        0        0     2041 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/core/disks.py
+-rw-r--r--   0        0        0     3745 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/core/latency.py
+-rw-r--r--   0        0        0     5730 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/core/memory.py
+-rw-r--r--   0        0        0     2597 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/core/networking.py
+-rw-r--r--   0        0        0     2764 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/core/processes.py
+-rw-r--r--   0        0        0     2605 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/core/services.py
+-rw-r--r--   0        0        0     4865 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/core/system.py
+-rw-r--r--   0        0        0     4417 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/main.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/utilities/__init__.py
+-rw-r--r--   0        0        0      442 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/utilities/exceptions.py
+-rw-r--r--   0        0        0      560 2024-04-29 15:58:52.056566 python_sysinformer-1.8.0/src/utilities/utils.py
+-rw-r--r--   0        0        0     6124 1970-01-01 00:00:00.000000 python_sysinformer-1.8.0/PKG-INFO
```

### Comparing `python_sysinformer-1.7.0/LICENSE` & `python_sysinformer-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.7.0/README.md` & `python_sysinformer-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.7.0/pyproject.toml` & `python_sysinformer-1.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-SysInformer"
-version = "1.7.0"
+version = "1.8.0"
 description = "A simple system information tool for Linux"
 authors = ["Timothy Bryant <timothybryant3@gmail.com>"]
 readme = "README.md"
 packages = [{include = "src", from = "."}]
 # classifiers = ["Private :: Do not Upload"]
 
 [tool.poetry.dependencies]
@@ -57,15 +57,15 @@
     "test",
     "feat",
     ":boom:",
     "BREAKING_CHANGE",
 ]
 major_tags = [":boom:", "BREAKING_CHANGE"]
 minor_tags = ["feat"]
-patch_tags = ["fix", "perf", "style", "docs", "ci", "test"]
+patch_tags = ["fix", "perf", "style", "docs", "ci", "test", "refactor", "chore", "build"]
 
 [tool.semantic_release]
 version_toml = [
     "pyproject.toml:tool.poetry.version",
 ]
 branch = "main"
 changelog_file = "CHANGELOG.md"
```

### Comparing `python_sysinformer-1.7.0/src/config/config_parser.py` & `python_sysinformer-1.8.0/src/config/config_parser.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.7.0/src/config/default_config.py` & `python_sysinformer-1.8.0/src/config/default_config.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.7.0/src/core/containers.py` & `python_sysinformer-1.8.0/src/core/containers.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.7.0/src/core/cpu.py` & `python_sysinformer-1.8.0/src/core/cpu.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.7.0/src/core/disks.py` & `python_sysinformer-1.8.0/src/core/disks.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.7.0/src/core/latency.py` & `python_sysinformer-1.8.0/src/core/latency.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.7.0/src/core/memory.py` & `python_sysinformer-1.8.0/src/core/memory.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.7.0/src/core/networking.py` & `python_sysinformer-1.8.0/src/core/networking.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.7.0/src/core/processes.py` & `python_sysinformer-1.8.0/src/core/processes.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.7.0/src/core/services.py` & `python_sysinformer-1.8.0/src/core/services.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.7.0/src/core/system.py` & `python_sysinformer-1.8.0/src/core/system.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,18 @@
 import os
 import datetime
 import platform
 import subprocess
 import time
 import re
-
+import distro
 
 from src.utilities.utils import print_bold_kv, print_title
 
 
-# def get_last_boot_time() -> float:
-#     """Returns the last boot time as a float for macOS."""
-#     if platform.system() == "Darwin":
-#         try:
-#             result = subprocess.run(
-#                 ["sysctl", "-n", "kern.boottime"],
-#                 capture_output=True,
-#                 text=True,
-#                 check=True,
-#             ).stdout.strip()
-#             if match := re.search(r"sec = (\d+)", result):
-#                 return float(match[1])
-#             else:
-#                 raise ValueError("Could not parse kern.boottime output")
-#         except (subprocess.CalledProcessError, ValueError) as e:
-#             print(f"An error occurred while getting last boot time: {e}")
-#             return 0.0
-#     else:
-#         try:
-#             result = subprocess.run(
-#                 ["uptime", "-s"],
-#                 capture_output=True,
-#                 text=True,
-#                 check=True,
-#             ).stdout.strip()
-#             return float(result)
-#         except subprocess.CalledProcessError as e:
-#             print(f"An error occurred while getting last boot time: {e}")
-#             return 0.0
-
-
 def get_last_boot_time() -> str:
     """Returns the last boot time as a date and time string."""
     if platform.system() == "Darwin":
         try:
             result = subprocess.run(
                 ["sysctl", "-n", "kern.boottime"],
                 capture_output=True,
@@ -56,51 +25,55 @@
                     "%Y-%m-%d %H:%M:%S"
                 )
             else:
                 raise ValueError("Could not parse kern.boottime output")
         except (subprocess.CalledProcessError, ValueError) as e:
             print(f"An error occurred while getting last boot time: {e}")
             return "Error obtaining last boot time"
-    else:  # Assuming this else branch is for Linux
+    elif platform.system() == "Linux":
         try:
             return subprocess.run(
                 ["uptime", "-s"],
                 capture_output=True,
                 text=True,
                 check=True,
             ).stdout.strip()
         except subprocess.CalledProcessError as e:
             print(f"An error occurred while getting last boot time: {e}")
             return "Error obtaining last boot time"
+    else:
+        return "Not supported on this OS"
 
 
 def get_system_uptime() -> str:
     """Returns the system uptime as a string."""
     if platform.system() == "Linux":
         try:
             uptime_seconds = time.time() - os.stat("/proc/1").st_ctime
             days, rem = divmod(uptime_seconds, 86400)
             hours, rem = divmod(rem, 3600)
             minutes, _ = divmod(rem, 60)
             return f"{int(days)} days, {int(hours)} hours, {int(minutes)} minutes"
         except Exception as e:
             print(f"An error occurred while getting system uptime on Linux: {e}")
             return "Error in obtaining uptime"
-    else:
+    elif platform.system() == "Darwin":
         try:
             uptime_output = subprocess.run(
                 ["uptime"],
                 capture_output=True,
                 text=True,
                 check=True,
             ).stdout.strip()
             return ", ".join(uptime_output.split(",")[:2])
         except subprocess.CalledProcessError as e:
             print(f"An error occurred while getting system uptime: {e}")
             return "Error in obtaining uptime"
+    else:
+        return "Not supported on this OS"
 
 
 def get_user_count_unix(path: str) -> int:
     """Counts the number of user directories in the given path for Unix systems."""
     try:
         # Exclude the "Shared" folder from the count
         return len(
@@ -128,18 +101,18 @@
         "users_nb": 0,
         "current_date": time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()),
     }
 
     system_info["uptime"] = get_system_uptime()
     system_info["last_boot_date"] = get_last_boot_time()
     if system_info["os_type"] == "Linux":
-        import distro  # distro is a Linux-specific package
-
         system_info["dist"] = distro.name()
-        system_info["dist_version"] = distro.version()
+        system_info["dist_version"] = (
+            platform.freedesktop_os_release().get("VERSION") or distro.version()
+        )
         system_info["users_nb"] = get_user_count_unix("/home")
 
     elif system_info["os_type"] == "Darwin":
         system_info["dist"] = "macOS"
         system_info["dist_version"] = platform.mac_ver()[0]
         system_info["users_nb"] = get_user_count_unix("/Users")
```

### Comparing `python_sysinformer-1.7.0/src/main.py` & `python_sysinformer-1.8.0/src/main.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.7.0/src/utilities/utils.py` & `python_sysinformer-1.8.0/src/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.7.0/PKG-INFO` & `python_sysinformer-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sysinformer
-Version: 1.7.0
+Version: 1.8.0
 Summary: A simple system information tool for Linux
 Author: Timothy Bryant
 Author-email: timothybryant3@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

