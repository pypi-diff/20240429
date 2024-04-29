# Comparing `tmp/esanom-3.0.3.748519.tar.gz` & `tmp/esanom-3.0.3.748842.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esanom-3.0.3.748519.tar", max compression
+gzip compressed data, was "esanom-3.0.3.748842.tar", max compression
```

## Comparing `esanom-3.0.3.748519.tar` & `esanom-3.0.3.748842.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0        0 2024-04-29 07:37:58.875832 esanom-3.0.3.748519/README.md
--rw-r--r--   0        0        0        0 2024-04-29 07:37:59.327828 esanom-3.0.3.748519/esanom/__init__.py
--rw-r--r--   0        0        0      446 2024-04-29 07:38:01.535812 esanom-3.0.3.748519/pyproject.toml
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 esanom-3.0.3.748519/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-29 07:43:21.522181 esanom-3.0.3.748842/README.md
+-rw-r--r--   0        0        0       35 2024-04-29 07:43:21.978221 esanom-3.0.3.748842/esanom/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 07:43:21.978221 esanom-3.0.3.748842/esanom/__init__.py
+-rw-r--r--   0        0        0      446 2024-04-29 07:43:24.182411 esanom-3.0.3.748842/pyproject.toml
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 esanom-3.0.3.748842/PKG-INFO
```

### Comparing `esanom-3.0.3.748519/PKG-INFO` & `esanom-3.0.3.748842/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esanom
-Version: 3.0.3.748519
+Version: 3.0.3.748842
 Summary: ESANOM
 Author: Zafar Iqbal
 Author-email: zaf@sparc.space
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

