# Comparing `tmp/djecorator-1.0.1.tar.gz` & `tmp/djecorator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djecorator-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "djecorator-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `djecorator-1.0.1.tar` & `djecorator-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3078 2024-04-28 21:56:13.477752 djecorator-1.0.1/.gitignore
--rw-r--r--   0        0        0     1086 2024-04-28 21:38:12.088814 djecorator-1.0.1/LICENSE
--rw-r--r--   0        0        0      411 2024-04-29 02:05:48.209193 djecorator-1.0.1/README.md
--rw-r--r--   0        0        0     1293 2024-04-28 22:51:57.093817 djecorator-1.0.1/djecorator.py
--rw-r--r--   0        0        0      383 2024-04-29 02:06:01.375380 djecorator-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      238 1970-01-01 00:00:00.000000 djecorator-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3078 2024-04-28 21:56:13.477752 djecorator-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1086 2024-04-28 21:38:12.088814 djecorator-1.0.2/LICENSE
+-rw-r--r--   0        0        0      411 2024-04-29 02:05:48.209193 djecorator-1.0.2/README.md
+-rw-r--r--   0        0        0     1293 2024-04-28 22:51:57.093817 djecorator-1.0.2/djecorator.py
+-rw-r--r--   0        0        0      404 2024-04-29 05:33:35.321079 djecorator-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 djecorator-1.0.2/PKG-INFO
```

### Comparing `djecorator-1.0.1/.gitignore` & `djecorator-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `djecorator-1.0.1/LICENSE` & `djecorator-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djecorator-1.0.1/djecorator.py` & `djecorator-1.0.2/djecorator.py`

 * *Files identical despite different names*

