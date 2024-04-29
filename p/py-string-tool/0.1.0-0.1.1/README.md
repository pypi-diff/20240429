# Comparing `tmp/py_string_tool-0.1.0.tar.gz` & `tmp/py_string_tool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_string_tool-0.1.0.tar", last modified: Mon Apr 29 04:36:49 2024, max compression
+gzip compressed data, was "py_string_tool-0.1.1.tar", last modified: Mon Apr 29 04:54:39 2024, max compression
```

## Comparing `py_string_tool-0.1.0.tar` & `py_string_tool-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 04:36:49.572152 py_string_tool-0.1.0/
--rw-rw-rw-   0        0        0      255 2024-04-29 04:36:49.572152 py_string_tool-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 04:36:49.549024 py_string_tool-0.1.0/py_string_tool/
--rw-rw-rw-   0        0        0       63 2024-04-29 04:26:24.000000 py_string_tool-0.1.0/py_string_tool/__init__.py
--rw-rw-rw-   0        0        0      480 2024-04-29 04:18:10.000000 py_string_tool-0.1.0/py_string_tool/blackslash_replace.py
--rw-rw-rw-   0        0        0     6401 2024-04-29 04:20:41.000000 py_string_tool-0.1.0/py_string_tool/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:36:49.570157 py_string_tool-0.1.0/py_string_tool.egg-info/
--rw-rw-rw-   0        0        0      255 2024-04-29 04:36:49.000000 py_string_tool-0.1.0/py_string_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-29 04:36:49.000000 py_string_tool-0.1.0/py_string_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 04:36:49.000000 py_string_tool-0.1.0/py_string_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-29 04:36:49.000000 py_string_tool-0.1.0/py_string_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 04:36:49.572152 py_string_tool-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      300 2024-04-29 04:21:51.000000 py_string_tool-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:54:39.356625 py_string_tool-0.1.1/
+-rw-rw-rw-   0        0        0      255 2024-04-29 04:54:39.355628 py_string_tool-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 04:54:39.345655 py_string_tool-0.1.1/py_string_tool/
+-rw-rw-rw-   0        0        0       63 2024-04-29 04:54:03.000000 py_string_tool-0.1.1/py_string_tool/__init__.py
+-rw-rw-rw-   0        0        0      480 2024-04-29 04:18:10.000000 py_string_tool-0.1.1/py_string_tool/blackslash_replace.py
+-rw-rw-rw-   0        0        0     6401 2024-04-29 04:20:41.000000 py_string_tool-0.1.1/py_string_tool/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:54:39.353632 py_string_tool-0.1.1/py_string_tool.egg-info/
+-rw-rw-rw-   0        0        0      255 2024-04-29 04:54:39.000000 py_string_tool-0.1.1/py_string_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-29 04:54:39.000000 py_string_tool-0.1.1/py_string_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 04:54:39.000000 py_string_tool-0.1.1/py_string_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-29 04:54:39.000000 py_string_tool-0.1.1/py_string_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 04:54:39.356625 py_string_tool-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      300 2024-04-29 04:53:58.000000 py_string_tool-0.1.1/setup.py
```

### Comparing `py_string_tool-0.1.0/py_string_tool/utils.py` & `py_string_tool-0.1.1/py_string_tool/utils.py`

 * *Files identical despite different names*

