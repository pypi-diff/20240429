# Comparing `tmp/paradime_io-4.2.0.tar.gz` & `tmp/paradime_io-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradime_io-4.2.0.tar", max compression
+gzip compressed data, was "paradime_io-4.3.0.tar", max compression
```

## Comparing `paradime_io-4.2.0.tar` & `paradime_io-4.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1074 2024-04-26 14:03:32.017141 paradime_io-4.2.0/LICENSE
--rw-r--r--   0        0        0     1060 2024-04-26 14:03:32.017141 paradime_io-4.2.0/README.md
--rw-r--r--   0        0        0       84 2024-04-26 14:03:32.017141 paradime_io-4.2.0/paradime/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/audit_log/__init__.py
--rw-r--r--   0        0        0     1901 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/audit_log/client.py
--rw-r--r--   0        0        0      423 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/audit_log/types.py
--rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/bolt/__init__.py
--rw-r--r--   0        0        0    14252 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/bolt/client.py
--rw-r--r--   0        0        0      387 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/bolt/exception.py
--rw-r--r--   0        0        0     1609 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/bolt/types.py
--rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/custom_integration/__init__.py
--rw-r--r--   0        0        0    12369 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/custom_integration/client.py
--rw-r--r--   0        0        0    17115 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/custom_integration/types.py
--rw-r--r--   0        0        0      321 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/custom_integration/utils.py
--rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/users/__init__.py
--rw-r--r--   0        0        0     4052 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/users/client.py
--rw-r--r--   0        0        0      656 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/users/types.py
--rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/workspaces/__init__.py
--rw-r--r--   0        0        0      823 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/workspaces/client.py
--rw-r--r--   0        0        0       88 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/apis/workspaces/types.py
--rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/cli/__init__.py
--rw-r--r--   0        0        0     2885 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/cli/bolt.py
--rw-r--r--   0        0        0      538 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/cli/cli.py
--rw-r--r--   0        0        0     1002 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/cli/login.py
--rw-r--r--   0        0        0     1966 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/cli/rich_text_output.py
--rw-r--r--   0        0        0      351 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/cli/version.py
--rw-r--r--   0        0        0     3719 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/client/api_client.py
--rw-r--r--   0        0        0      231 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/client/api_exception.py
--rw-r--r--   0        0        0      974 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/client/paradime_cli_client.py
--rw-r--r--   0        0        0     1692 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/client/paradime_client.py
--rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/core/bolt/__init__.py
--rw-r--r--   0        0        0     5615 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/core/bolt/schedule.py
--rw-r--r--   0        0        0      376 2024-04-26 14:03:32.021141 paradime_io-4.2.0/paradime/version.py
--rw-r--r--   0        0        0     1156 2024-04-26 14:03:32.021141 paradime_io-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 paradime_io-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-29 12:46:29.916178 paradime_io-4.3.0/LICENSE
+-rw-r--r--   0        0        0     1060 2024-04-29 12:46:29.916178 paradime_io-4.3.0/README.md
+-rw-r--r--   0        0        0       84 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/audit_log/__init__.py
+-rw-r--r--   0        0        0     1901 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/audit_log/client.py
+-rw-r--r--   0        0        0      423 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/audit_log/types.py
+-rw-r--r--   0        0        0        0 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/bolt/__init__.py
+-rw-r--r--   0        0        0    14252 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/bolt/client.py
+-rw-r--r--   0        0        0      387 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/bolt/exception.py
+-rw-r--r--   0        0        0     1635 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/bolt/types.py
+-rw-r--r--   0        0        0        0 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/custom_integration/__init__.py
+-rw-r--r--   0        0        0    12369 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/custom_integration/client.py
+-rw-r--r--   0        0        0    17115 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/custom_integration/types.py
+-rw-r--r--   0        0        0      321 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/custom_integration/utils.py
+-rw-r--r--   0        0        0        0 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/users/__init__.py
+-rw-r--r--   0        0        0     4052 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/users/client.py
+-rw-r--r--   0        0        0      656 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/users/types.py
+-rw-r--r--   0        0        0        0 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/workspaces/__init__.py
+-rw-r--r--   0        0        0      823 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/workspaces/client.py
+-rw-r--r--   0        0        0       88 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/apis/workspaces/types.py
+-rw-r--r--   0        0        0        0 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/cli/__init__.py
+-rw-r--r--   0        0        0     2885 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/cli/bolt.py
+-rw-r--r--   0        0        0      538 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/cli/cli.py
+-rw-r--r--   0        0        0     1002 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/cli/login.py
+-rw-r--r--   0        0        0     1966 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/cli/rich_text_output.py
+-rw-r--r--   0        0        0      351 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/cli/version.py
+-rw-r--r--   0        0        0     3719 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/client/api_client.py
+-rw-r--r--   0        0        0      231 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/client/api_exception.py
+-rw-r--r--   0        0        0      974 2024-04-29 12:46:29.916178 paradime_io-4.3.0/paradime/client/paradime_cli_client.py
+-rw-r--r--   0        0        0     1692 2024-04-29 12:46:29.920178 paradime_io-4.3.0/paradime/client/paradime_client.py
+-rw-r--r--   0        0        0        0 2024-04-29 12:46:29.920178 paradime_io-4.3.0/paradime/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 12:46:29.920178 paradime_io-4.3.0/paradime/core/bolt/__init__.py
+-rw-r--r--   0        0        0     5615 2024-04-29 12:46:29.920178 paradime_io-4.3.0/paradime/core/bolt/schedule.py
+-rw-r--r--   0        0        0      376 2024-04-29 12:46:29.920178 paradime_io-4.3.0/paradime/version.py
+-rw-r--r--   0        0        0     1156 2024-04-29 12:46:29.920178 paradime_io-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 paradime_io-4.3.0/PKG-INFO
```

### Comparing `paradime_io-4.2.0/LICENSE` & `paradime_io-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/README.md` & `paradime_io-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/paradime/apis/audit_log/client.py` & `paradime_io-4.3.0/paradime/apis/audit_log/client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/paradime/apis/bolt/client.py` & `paradime_io-4.3.0/paradime/apis/bolt/client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/paradime/apis/bolt/types.py` & `paradime_io-4.3.0/paradime/apis/bolt/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 from typing import List, Optional
 
 from pydantic import BaseModel
 
 
 class BoltRunState(str, Enum):
+    STARTING = "STARTING"
     RUNNING = "RUNNING"
     SUCCESS = "SUCCESS"
     ERROR = "ERROR"
     FAILED = "FAILED"
     CANCELED = "CANCELED"
     SKIPPED = "SKIPPED"
```

### Comparing `paradime_io-4.2.0/paradime/apis/custom_integration/client.py` & `paradime_io-4.3.0/paradime/apis/custom_integration/client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/paradime/apis/custom_integration/types.py` & `paradime_io-4.3.0/paradime/apis/custom_integration/types.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/paradime/apis/users/client.py` & `paradime_io-4.3.0/paradime/apis/users/client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/paradime/apis/users/types.py` & `paradime_io-4.3.0/paradime/apis/users/types.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/paradime/apis/workspaces/client.py` & `paradime_io-4.3.0/paradime/apis/workspaces/client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/paradime/cli/bolt.py` & `paradime_io-4.3.0/paradime/cli/bolt.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/paradime/cli/cli.py` & `paradime_io-4.3.0/paradime/cli/cli.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/paradime/cli/login.py` & `paradime_io-4.3.0/paradime/cli/login.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/paradime/cli/rich_text_output.py` & `paradime_io-4.3.0/paradime/cli/rich_text_output.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/paradime/client/api_client.py` & `paradime_io-4.3.0/paradime/client/api_client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/paradime/client/paradime_cli_client.py` & `paradime_io-4.3.0/paradime/client/paradime_cli_client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/paradime/client/paradime_client.py` & `paradime_io-4.3.0/paradime/client/paradime_client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/paradime/core/bolt/schedule.py` & `paradime_io-4.3.0/paradime/core/bolt/schedule.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.2.0/pyproject.toml` & `paradime_io-4.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paradime-io"
-version = "4.2.0"
+version = "4.3.0"
 description = "Paradime - Python SDK"
 authors = ["Bhuvan Singla <bhuvan@paradime.io>", "Maximilian Mitchell <max@paradime.io>"]
 readme = "README.md"
 packages = [
 	{ include = "paradime", from = "." },
 ]
```

### Comparing `paradime_io-4.2.0/PKG-INFO` & `paradime_io-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradime-io
-Version: 4.2.0
+Version: 4.3.0
 Summary: Paradime - Python SDK
 Author: Bhuvan Singla
 Author-email: bhuvan@paradime.io
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: paradime-io Version: 4.2.0 Summary: Paradime -
+Metadata-Version: 2.1 Name: paradime-io Version: 4.3.0 Summary: Paradime -
 Python SDK Author: Bhuvan Singla Author-email: bhuvan@paradime.io Requires-
 Python: >=3.8 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: click (>=8.1.7,<9.0.0) Requires-Dist: croniter
 (>=2.0.2,<3.0.0) Requires-Dist: pydantic (==1.10.14) Requires-Dist: python-
```

