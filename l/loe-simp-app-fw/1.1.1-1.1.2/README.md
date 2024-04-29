# Comparing `tmp/loe_simp_app_fw-1.1.1.tar.gz` & `tmp/loe_simp_app_fw-1.1.2.tar.gz`

## Comparing `loe_simp_app_fw-1.1.1.tar` & `loe_simp_app_fw-1.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/config-example.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/src/loe_simp_app_fw/__init__.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/src/loe_simp_app_fw/config.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/src/loe_simp_app_fw/helper.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/src/loe_simp_app_fw/logger.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/tests/test_import.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/LICENSE
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/config-example.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/src/loe_simp_app_fw/__init__.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/src/loe_simp_app_fw/config.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/src/loe_simp_app_fw/helper.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/src/loe_simp_app_fw/logger.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/tests/test_import.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/PKG-INFO
```

### Comparing `loe_simp_app_fw-1.1.1/src/loe_simp_app_fw/config.py` & `loe_simp_app_fw-1.1.2/src/loe_simp_app_fw/config.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.1/src/loe_simp_app_fw/helper.py` & `loe_simp_app_fw-1.1.2/src/loe_simp_app_fw/helper.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.1/src/loe_simp_app_fw/logger.py` & `loe_simp_app_fw-1.1.2/src/loe_simp_app_fw/logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,104 @@
 import os
 import datetime
+from typing import Optional, IO
 from .helper import create_folder_if_not_exists, ProjectRootChanged
 
 # Do not write the Log until the explicit initialization of the logger
 
 class Logger:
     # Following parameters should be set at the top-level environment of the project
     _project_root_path = ""
     _log_folder_path = "" # The path of _example_config_path relative to _project_root_path
     
     # Internal variable
     _log_buffer = []
     _isInit = False
+    _log_file_handle: Optional[IO] = None
     
-    @staticmethod
-    def _log_location():
+    @classmethod
+    def _log_location(cls):
         file_name = f"{datetime.date.today()}.log"
-        return os.path.join(Logger._project_root_path, Logger._log_folder_path, file_name)
+        return os.path.join(cls._project_root_path, cls._log_folder_path, file_name)
 
-    @staticmethod
-    def _create_log_file():
-        if not os.path.isfile(Logger._log_location()) and not os.path.isdir(Logger._log_location()):
-            with open(Logger._log_location(), "w", encoding="utf-8") as f:
+    @classmethod
+    def _create_log_file(cls):
+        if not os.path.isfile(cls._log_location()) and not os.path.isdir(cls._log_location()):
+            with open(cls._log_location(), "w", encoding="utf-8") as f:
                 print("Create log file successfully.")
 
     def __init__(self, log_folder_path: str, project_root_path: str = os.getcwd()):
         """Init Logger
 
         Args:
             log_folder_path (str): path to log folder relative to project root path
             project_root_path (str, optional): path to project top-level directory. Defaults to os.getcwd().
+                                                The parent folder of that would be os.path.dirname(os.path.realpath(__file__)).
 
         Raises:
             ProjectRootChanged: Project root directory should not be changed once set
         """
         # Sanity check
-        if Logger._project_root_path and project_root_path and not os.path.samefile(project_root_path, Logger._project_root_path):
-            Logger.error("One should not change project root path twice")
+        if self._project_root_path and project_root_path and not os.path.samefile(project_root_path, self._project_root_path):
+            self.error("One should not change project root path twice")
             raise ProjectRootChanged
 
         # Save input
-        Logger._log_folder_path = log_folder_path
-        Logger._project_root_path = project_root_path
+        self._log_folder_path = log_folder_path
+        self._project_root_path = project_root_path
 
         # Create log folder
-        folder_name = os.path.join(Logger._project_root_path, Logger._log_folder_path)
+        folder_name = os.path.join(self._project_root_path, self._log_folder_path)
         if not os.path.isfile(folder_name) and not os.path.isdir(folder_name):
             create_folder_if_not_exists(folder_name)
 
+        # Create file IO handle
+        self._log_file_handle = open(self._log_location(), "a", encoding="utf-8")
+
         # Save previous logs
-        with open(Logger._log_location(), "a", encoding="utf-8") as f:
-            f.writelines(f"\n{datetime.datetime.now()} INIT Logger successful\n")
-            f.writelines("".join(Logger._log_buffer))
+        self._log_file_handle.writelines(f"\n{datetime.datetime.now()} INIT Logger successful\n")
+        self._log_file_handle.writelines("".join(self._log_buffer))
         
         # Empty log buffer
-        Logger._log_buffer = []
+        self._log_buffer = []
 
         # Update flags
-        Logger._isInit = True
-        print(f"Logger init process finished, Logger isInit is set to {Logger._isInit}")
+        self._isInit = True
+        print(f"Logger init process finished, Logger isInit is set to {self._isInit}")
 
-    @staticmethod
-    def info(msg: str) -> None:
-        Logger._log("INFO", msg)
-
-    @staticmethod
-    def debug(msg: str) -> None:
-        Logger._log("DEBUG", msg)
-
-    @staticmethod
-    def warning(msg: str) -> None:
-        Logger._log("WARNING", msg)
-
-    @staticmethod
-    def error(msg :str) -> None:
-        Logger._log("ERROR", msg)
+    @classmethod
+    def info(cls, msg: str) -> None:
+        cls._log("INFO", msg)
+
+    @classmethod
+    def debug(cls, msg: str) -> None:
+        cls._log("DEBUG", msg)
+
+    @classmethod
+    def warning(cls, msg: str) -> None:
+        cls._log("WARNING", msg)
+
+    @classmethod
+    def error(cls, msg :str) -> None:
+        cls._log("ERROR", msg)
 
-    @staticmethod
-    def _log(level: str, msg: str) -> None:
+    @classmethod
+    def _log(cls, level: str, msg: str) -> None:
         # Compose log
         composed_log_entry = f"{datetime.datetime.now()} {level.upper()}: {msg}\n"
-        if Logger._isInit:
+        if cls._isInit and isinstance(cls._log_file_handle, IO): 
+            # The file handler is only to make static checker happy
             # Write to file
             try:
-                with open(Logger._log_location(), "a", encoding="utf-8") as f:
-                    f.writelines(composed_log_entry)
+                cls._log_file_handle.writelines(composed_log_entry)
             except FileNotFoundError:
-                Logger._create_log_file()
+                cls._create_log_file()
         else:
             # Write to buffer, not file
-            Logger._log_buffer.append(composed_log_entry)
+            cls._log_buffer.append(composed_log_entry)
             print(composed_log_entry)
         return
         
 
 def logger_showoff() -> None:
     # Demonstrate the logger
     Logger("log")
```

### Comparing `loe_simp_app_fw-1.1.1/tests/test_import.py` & `loe_simp_app_fw-1.1.2/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.1/.gitignore` & `loe_simp_app_fw-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.1/LICENSE` & `loe_simp_app_fw-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.1/README.md` & `loe_simp_app_fw-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.1/pyproject.toml` & `loe_simp_app_fw-1.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "loe_simp_app_fw"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="loeeeee", email="95266635+loeeeee@users.noreply.github.com" },
 ]
 description = "A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `loe_simp_app_fw-1.1.1/PKG-INFO` & `loe_simp_app_fw-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: loe_simp_app_fw
-Version: 1.1.1
+Version: 1.1.2
 Summary: A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook.
 Project-URL: Homepage, https://github.com/loeeeee/loe-simp-app-fw
 Project-URL: Issues, https://github.com/loeeeee/loe-simp-app-fw/issues
 Author-email: loeeeee <95266635+loeeeee@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

