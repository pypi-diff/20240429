# Comparing `tmp/edgegap_scheduling-0.1.1.tar.gz` & `tmp/edgegap_scheduling-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_scheduling-0.1.1.tar", max compression
+gzip compressed data, was "edgegap_scheduling-1.0.0.tar", max compression
```

## Comparing `edgegap_scheduling-0.1.1.tar` & `edgegap_scheduling-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.375580 edgegap_scheduling-0.1.1/LICENSE
--rw-r--r--   0        0        0     2164 2024-04-29 14:47:02.455878 edgegap_scheduling-0.1.1/README.md
--rw-r--r--   0        0        0      280 2024-04-29 15:32:04.063791 edgegap_scheduling-0.1.1/edgegap_scheduling/__init__.py
--rw-r--r--   0        0        0      128 2024-04-25 13:10:38.954379 edgegap_scheduling-0.1.1/edgegap_scheduling/_depends.py
--rw-r--r--   0        0        0     3389 2024-04-29 15:32:04.067876 edgegap_scheduling-0.1.1/edgegap_scheduling/_runner.py
--rw-r--r--   0        0        0     3855 2024-04-29 15:32:04.060315 edgegap_scheduling-0.1.1/edgegap_scheduling/_scheduler.py
--rw-r--r--   0        0        0     1025 2024-04-25 13:10:38.955042 edgegap_scheduling-0.1.1/edgegap_scheduling/_signature.py
--rw-r--r--   0        0        0      482 2024-04-25 13:10:38.955122 edgegap_scheduling-0.1.1/edgegap_scheduling/_singleton.py
--rw-r--r--   0        0        0     1233 2024-04-25 13:10:38.955206 edgegap_scheduling-0.1.1/edgegap_scheduling/_sleep.py
--rw-r--r--   0        0        0      188 2024-04-25 13:10:38.955422 edgegap_scheduling-0.1.1/edgegap_scheduling/_state.py
--rw-r--r--   0        0        0     2780 2024-04-29 15:32:04.056350 edgegap_scheduling-0.1.1/edgegap_scheduling/_task.py
--rw-r--r--   0        0        0      132 2024-04-25 20:04:14.788186 edgegap_scheduling-0.1.1/edgegap_scheduling/errors/__init__.py
--rw-r--r--   0        0        0      103 2024-04-25 20:04:14.717257 edgegap_scheduling-0.1.1/edgegap_scheduling/errors/_errors.py
--rw-r--r--   0        0        0      501 2024-04-29 15:32:27.445016 edgegap_scheduling-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 edgegap_scheduling-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 18:13:42.714660 edgegap_scheduling-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2164 2024-04-29 18:13:42.714660 edgegap_scheduling-1.0.0/README.md
+-rw-r--r--   0        0        0      280 2024-04-29 18:13:42.714660 edgegap_scheduling-1.0.0/edgegap_scheduling/__init__.py
+-rw-r--r--   0        0        0      128 2024-04-29 18:13:42.714660 edgegap_scheduling-1.0.0/edgegap_scheduling/_depends.py
+-rw-r--r--   0        0        0     3389 2024-04-29 18:13:42.714660 edgegap_scheduling-1.0.0/edgegap_scheduling/_runner.py
+-rw-r--r--   0        0        0     3855 2024-04-29 18:13:42.714660 edgegap_scheduling-1.0.0/edgegap_scheduling/_scheduler.py
+-rw-r--r--   0        0        0     1025 2024-04-29 18:13:42.714660 edgegap_scheduling-1.0.0/edgegap_scheduling/_signature.py
+-rw-r--r--   0        0        0      482 2024-04-29 18:13:42.714660 edgegap_scheduling-1.0.0/edgegap_scheduling/_singleton.py
+-rw-r--r--   0        0        0     1233 2024-04-29 18:13:42.714660 edgegap_scheduling-1.0.0/edgegap_scheduling/_sleep.py
+-rw-r--r--   0        0        0      188 2024-04-29 18:13:42.714660 edgegap_scheduling-1.0.0/edgegap_scheduling/_state.py
+-rw-r--r--   0        0        0     2780 2024-04-29 18:13:42.714660 edgegap_scheduling-1.0.0/edgegap_scheduling/_task.py
+-rw-r--r--   0        0        0      132 2024-04-29 18:13:42.714660 edgegap_scheduling-1.0.0/edgegap_scheduling/errors/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-29 18:13:42.714660 edgegap_scheduling-1.0.0/edgegap_scheduling/errors/_errors.py
+-rw-r--r--   0        0        0      501 2024-04-29 18:14:07.926795 edgegap_scheduling-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 edgegap_scheduling-1.0.0/PKG-INFO
```

### Comparing `edgegap_scheduling-0.1.1/LICENSE` & `edgegap_scheduling-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-0.1.1/README.md` & `edgegap_scheduling-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-0.1.1/edgegap_scheduling/_runner.py` & `edgegap_scheduling-1.0.0/edgegap_scheduling/_runner.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-0.1.1/edgegap_scheduling/_scheduler.py` & `edgegap_scheduling-1.0.0/edgegap_scheduling/_scheduler.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-0.1.1/edgegap_scheduling/_signature.py` & `edgegap_scheduling-1.0.0/edgegap_scheduling/_signature.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-0.1.1/edgegap_scheduling/_sleep.py` & `edgegap_scheduling-1.0.0/edgegap_scheduling/_sleep.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-0.1.1/edgegap_scheduling/_task.py` & `edgegap_scheduling-1.0.0/edgegap_scheduling/_task.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-0.1.1/PKG-INFO` & `edgegap_scheduling-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: edgegap-scheduling
-Version: 0.1.1
+Version: 1.0.0
 Summary: The Edgegap Scheduling library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: edgegap-logging (>=0.1.2,<0.2.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pytimeparse (>=1.1.8,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Edgegap Scheduling Library
```

