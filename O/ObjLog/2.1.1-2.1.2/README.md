# Comparing `tmp/objlog-2.1.1.tar.gz` & `tmp/objlog-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objlog-2.1.1.tar", max compression
+gzip compressed data, was "objlog-2.1.2.tar", max compression
```

## Comparing `objlog-2.1.1.tar` & `objlog-2.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      846 2024-03-08 16:21:48.232459 objlog-2.1.1/LICENSE
--rw-r--r--   0        0        0    13862 2024-03-08 17:07:36.707784 objlog-2.1.1/README.md
--rw-r--r--   0        0        0     1632 2024-03-08 16:21:48.251774 objlog-2.1.1/objlog/Base/LogMessage.py
--rw-r--r--   0        0        0    14704 2024-04-26 16:28:14.643601 objlog-2.1.1/objlog/Base/LogNode.py
--rw-r--r--   0        0        0      113 2023-12-15 01:33:55.464872 objlog-2.1.1/objlog/Base/__init__.py
--rw-r--r--   0        0        0      287 2024-03-08 16:21:48.252460 objlog-2.1.1/objlog/Base/internal.py
--rw-r--r--   0        0        0     2025 2024-03-08 16:21:48.252807 objlog-2.1.1/objlog/LogMessages.py
--rw-r--r--   0        0        0      110 2024-03-08 16:21:48.253857 objlog-2.1.1/objlog/__init__.py
--rw-r--r--   0        0        0     2213 2024-03-08 16:21:48.254279 objlog-2.1.1/objlog/utils.py
--rw-r--r--   0        0        0      501 2024-04-26 16:28:50.352643 objlog-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    14528 1970-01-01 00:00:00.000000 objlog-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0      846 2024-03-08 16:21:48.232459 objlog-2.1.2/LICENSE
+-rw-r--r--   0        0        0    13862 2024-03-08 17:07:36.707784 objlog-2.1.2/README.md
+-rw-r--r--   0        0        0     1632 2024-03-08 16:21:48.251774 objlog-2.1.2/objlog/Base/LogMessage.py
+-rw-r--r--   0        0        0    14751 2024-04-29 16:33:58.125179 objlog-2.1.2/objlog/Base/LogNode.py
+-rw-r--r--   0        0        0      113 2023-12-15 01:33:55.464872 objlog-2.1.2/objlog/Base/__init__.py
+-rw-r--r--   0        0        0      287 2024-03-08 16:21:48.252460 objlog-2.1.2/objlog/Base/internal.py
+-rw-r--r--   0        0        0     2025 2024-03-08 16:21:48.252807 objlog-2.1.2/objlog/LogMessages.py
+-rw-r--r--   0        0        0      110 2024-03-08 16:21:48.253857 objlog-2.1.2/objlog/__init__.py
+-rw-r--r--   0        0        0     2213 2024-03-08 16:21:48.254279 objlog-2.1.2/objlog/utils.py
+-rw-r--r--   0        0        0      501 2024-04-29 16:34:23.028787 objlog-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0    14528 1970-01-01 00:00:00.000000 objlog-2.1.2/PKG-INFO
```

### Comparing `objlog-2.1.1/LICENSE` & `objlog-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `objlog-2.1.1/README.md` & `objlog-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `objlog-2.1.1/objlog/Base/LogMessage.py` & `objlog-2.1.2/objlog/Base/LogMessage.py`

 * *Files identical despite different names*

### Comparing `objlog-2.1.1/objlog/Base/LogNode.py` & `objlog-2.1.2/objlog/Base/LogNode.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,17 @@
         if log_file:
             with self.open(log_file) as f:
                 self.log_len = len(f.readlines())
                 if self.log_len > max_log_messages:
                     # chop the file
                     lines = f.readlines()
                     lines = lines[-max_log_messages:]
-                    with self.open(log_file, "w") as f2:
+                    with self.open(log_file, "w+") as f2:
                         f2.writelines(lines)
+                    self.log_len = len(lines)
         else:
             self.log_len = 0
 
         # check if log exists (in the file system), and if so, clear it
         if isinstance(log_file, str) and wipe_log_file_on_init:
             # your IDE might say that this code is broken, but it's not.
             # i'm aware that it should probably be lit on fire and thrown into a volcano, but it works for now.
```

### Comparing `objlog-2.1.1/objlog/LogMessages.py` & `objlog-2.1.2/objlog/LogMessages.py`

 * *Files identical despite different names*

### Comparing `objlog-2.1.1/objlog/utils.py` & `objlog-2.1.2/objlog/utils.py`

 * *Files identical despite different names*

### Comparing `objlog-2.1.1/PKG-INFO` & `objlog-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ObjLog
-Version: 2.1.1
+Version: 2.1.2
 Summary: Logging, Objectified.
 Home-page: https://github.com/Kokonico/ObjLog
 License: Zlib
 Keywords: logging,object,objectified,log,logger,loggers,OOP,python,python3,python3.10,python3.11,python3.12
 Author: Kokonico
 Author-email: kokonico@duck.com
 Requires-Python: >=3.10,<4.0
```

