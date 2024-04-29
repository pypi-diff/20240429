# Comparing `tmp/tadl-0.1.0.tar.gz` & `tmp/tadl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tadl-0.1.0.tar", max compression
+gzip compressed data, was "tadl-0.1.1.tar", max compression
```

## Comparing `tadl-0.1.0.tar` & `tadl-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     6890 2024-04-28 23:50:07.613650 tadl-0.1.0/README.md
--rw-r--r--   0        0        0      455 2024-04-28 23:54:14.173540 tadl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      135 2024-04-28 23:58:21.973845 tadl-0.1.0/tadl/__init__.py
--rw-r--r--   0        0        0     3003 2024-04-28 21:47:19.218489 tadl-0.1.0/tadl/descriptor.py
--rw-r--r--   0        0        0     1857 2024-04-28 22:45:04.538629 tadl-0.1.0/tadl/match.py
--rw-r--r--   0        0        0     4672 2024-04-28 23:42:36.949794 tadl-0.1.0/tadl/query.py
--rw-r--r--   0        0        0     1866 2024-04-29 00:22:54.082305 tadl-0.1.0/tadl/query_batch.py
--rw-r--r--   0        0        0     1829 2024-04-28 23:58:21.981770 tadl-0.1.0/tadl/query_group.py
--rw-r--r--   0        0        0      204 2024-04-28 21:37:43.839846 tadl-0.1.0/tadl/query_interface.py
--rw-r--r--   0        0        0      206 2024-04-28 20:46:54.182822 tadl-0.1.0/tadl/types.py
--rw-r--r--   0        0        0     7274 1970-01-01 00:00:00.000000 tadl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6890 2024-04-28 23:50:07.613650 tadl-0.1.1/README.md
+-rw-r--r--   0        0        0      455 2024-04-29 01:12:15.347385 tadl-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      135 2024-04-28 23:58:21.973845 tadl-0.1.1/tadl/__init__.py
+-rw-r--r--   0        0        0     3003 2024-04-28 21:47:19.218489 tadl-0.1.1/tadl/descriptor.py
+-rw-r--r--   0        0        0     1857 2024-04-28 22:45:04.538629 tadl-0.1.1/tadl/match.py
+-rw-r--r--   0        0        0        0 2024-04-29 01:11:17.442666 tadl-0.1.1/tadl/py.typed
+-rw-r--r--   0        0        0     4672 2024-04-28 23:42:36.949794 tadl-0.1.1/tadl/query.py
+-rw-r--r--   0        0        0     1866 2024-04-29 00:22:54.082305 tadl-0.1.1/tadl/query_batch.py
+-rw-r--r--   0        0        0     1829 2024-04-28 23:58:21.981770 tadl-0.1.1/tadl/query_group.py
+-rw-r--r--   0        0        0      204 2024-04-28 21:37:43.839846 tadl-0.1.1/tadl/query_interface.py
+-rw-r--r--   0        0        0      206 2024-04-28 20:46:54.182822 tadl-0.1.1/tadl/types.py
+-rw-r--r--   0        0        0     7274 1970-01-01 00:00:00.000000 tadl-0.1.1/PKG-INFO
```

### Comparing `tadl-0.1.0/README.md` & `tadl-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tadl-0.1.0/tadl/descriptor.py` & `tadl-0.1.1/tadl/descriptor.py`

 * *Files identical despite different names*

### Comparing `tadl-0.1.0/tadl/match.py` & `tadl-0.1.1/tadl/match.py`

 * *Files identical despite different names*

### Comparing `tadl-0.1.0/tadl/query.py` & `tadl-0.1.1/tadl/query.py`

 * *Files identical despite different names*

### Comparing `tadl-0.1.0/tadl/query_batch.py` & `tadl-0.1.1/tadl/query_batch.py`

 * *Files identical despite different names*

### Comparing `tadl-0.1.0/tadl/query_group.py` & `tadl-0.1.1/tadl/query_group.py`

 * *Files identical despite different names*

### Comparing `tadl-0.1.0/PKG-INFO` & `tadl-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tadl
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Travis DePrato
 Author-email: hey@twavv.me
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

