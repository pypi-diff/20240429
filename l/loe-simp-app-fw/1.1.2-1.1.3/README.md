# Comparing `tmp/loe_simp_app_fw-1.1.2.tar.gz` & `tmp/loe_simp_app_fw-1.1.3.tar.gz`

## Comparing `loe_simp_app_fw-1.1.2.tar` & `loe_simp_app_fw-1.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/config-example.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/src/loe_simp_app_fw/__init__.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/src/loe_simp_app_fw/config.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/src/loe_simp_app_fw/helper.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/src/loe_simp_app_fw/logger.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/tests/test_import.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/LICENSE
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/config-example.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/src/loe_simp_app_fw/__init__.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/src/loe_simp_app_fw/config.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/src/loe_simp_app_fw/helper.py
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/src/loe_simp_app_fw/logger.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/tests/test_import.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/LICENSE
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/PKG-INFO
```

### Comparing `loe_simp_app_fw-1.1.2/src/loe_simp_app_fw/config.py` & `loe_simp_app_fw-1.1.3/src/loe_simp_app_fw/config.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.2/src/loe_simp_app_fw/helper.py` & `loe_simp_app_fw-1.1.3/src/loe_simp_app_fw/helper.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.2/src/loe_simp_app_fw/logger.py` & `loe_simp_app_fw-1.1.3/src/loe_simp_app_fw/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import datetime
+from io import TextIOWrapper
 from typing import Optional, IO
 from .helper import create_folder_if_not_exists, ProjectRootChanged
 
 # Do not write the Log until the explicit initialization of the logger
 
 class Logger:
     # Following parameters should be set at the top-level environment of the project
@@ -81,15 +82,15 @@
     def error(cls, msg :str) -> None:
         cls._log("ERROR", msg)
 
     @classmethod
     def _log(cls, level: str, msg: str) -> None:
         # Compose log
         composed_log_entry = f"{datetime.datetime.now()} {level.upper()}: {msg}\n"
-        if cls._isInit and isinstance(cls._log_file_handle, IO): 
+        if cls._isInit and isinstance(cls._log_file_handle, TextIOWrapper): 
             # The file handler is only to make static checker happy
             # Write to file
             try:
                 cls._log_file_handle.writelines(composed_log_entry)
             except FileNotFoundError:
                 cls._create_log_file()
         else:
```

### Comparing `loe_simp_app_fw-1.1.2/tests/test_import.py` & `loe_simp_app_fw-1.1.3/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.2/.gitignore` & `loe_simp_app_fw-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.2/LICENSE` & `loe_simp_app_fw-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.2/README.md` & `loe_simp_app_fw-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.2/PKG-INFO` & `loe_simp_app_fw-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: loe_simp_app_fw
-Version: 1.1.2
+Version: 1.1.3
 Summary: A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook.
 Project-URL: Homepage, https://github.com/loeeeee/loe-simp-app-fw
 Project-URL: Issues, https://github.com/loeeeee/loe-simp-app-fw/issues
 Author-email: loeeeee <95266635+loeeeee@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

