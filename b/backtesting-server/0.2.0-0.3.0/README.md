# Comparing `tmp/backtesting_server-0.2.0.tar.gz` & `tmp/backtesting_server-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtesting_server-0.2.0.tar", max compression
+gzip compressed data, was "backtesting_server-0.3.0.tar", max compression
```

## Comparing `backtesting_server-0.2.0.tar` & `backtesting_server-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 backtesting_server-0.2.0/LICENSE
--rw-r--r--   0        0        0      604 2024-04-23 15:00:09.200833 backtesting_server-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1858 2024-04-15 23:43:05.933161 backtesting_server-0.2.0/README.md
--rw-r--r--   0        0        0      185 2024-04-16 22:17:04.776709 backtesting_server-0.2.0/src/backtesting_server/__init__.py
--rw-r--r--   0        0        0    12947 2024-04-20 16:32:39.226041 backtesting_server-0.2.0/src/backtesting_server/main.py
--rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 backtesting_server-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 backtesting_server-0.3.0/LICENSE
+-rw-r--r--   0        0        0      604 2024-04-29 14:41:20.099564 backtesting_server-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1858 2024-04-15 23:43:05.933161 backtesting_server-0.3.0/README.md
+-rw-r--r--   0        0        0      185 2024-04-16 22:17:04.776709 backtesting_server-0.3.0/src/backtesting_server/__init__.py
+-rw-r--r--   0        0        0    20813 2024-04-29 13:07:23.104806 backtesting_server-0.3.0/src/backtesting_server/main.py
+-rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 backtesting_server-0.3.0/PKG-INFO
```

### Comparing `backtesting_server-0.2.0/LICENSE` & `backtesting_server-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `backtesting_server-0.2.0/pyproject.toml` & `backtesting_server-0.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "backtesting-server"
-version = "0.2.0"
+version = "0.3.0"
 description = "Package to interact with MySQL server, recording results of the backtesting."
 authors = ["hnewey7 <hnewey7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `backtesting_server-0.2.0/README.md` & `backtesting_server-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `backtesting_server-0.2.0/PKG-INFO` & `backtesting_server-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backtesting-server
-Version: 0.2.0
+Version: 0.3.0
 Summary: Package to interact with MySQL server, recording results of the backtesting.
 License: MIT
 Author: hnewey7
 Author-email: hnewey7@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

