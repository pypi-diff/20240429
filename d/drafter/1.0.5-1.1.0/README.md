# Comparing `tmp/drafter-1.0.5.tar.gz` & `tmp/drafter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drafter-1.0.5.tar", last modified: Mon Apr  1 19:01:23 2024, max compression
+gzip compressed data, was "drafter-1.1.0.tar", last modified: Mon Apr 29 14:09:28 2024, max compression
```

## Comparing `drafter-1.0.5.tar` & `drafter-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 19:01:23.594720 drafter-1.0.5/
--rw-rw-rw-   0        0        0     1075 2021-09-26 08:48:54.000000 drafter-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      766 2024-04-01 19:01:23.593714 drafter-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       57 2023-09-04 16:32:22.000000 drafter-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 19:01:23.592643 drafter-1.0.5/drafter.egg-info/
--rw-rw-rw-   0        0        0      766 2024-04-01 19:01:23.000000 drafter-1.0.5/drafter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-01 19:01:23.000000 drafter-1.0.5/drafter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 19:01:23.000000 drafter-1.0.5/drafter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-01 19:01:23.000000 drafter-1.0.5/drafter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-01 19:01:23.000000 drafter-1.0.5/drafter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    59440 2024-04-01 19:01:10.000000 drafter-1.0.5/drafter.py
--rw-rw-rw-   0        0        0       80 2023-08-30 14:30:23.000000 drafter-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 19:01:23.594720 drafter-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1220 2023-09-09 13:39:14.000000 drafter-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:09:28.620414 drafter-1.1.0/
+-rw-rw-rw-   0        0        0     1075 2021-09-26 08:48:54.000000 drafter-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      766 2024-04-29 14:09:28.620414 drafter-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2023-09-04 16:32:22.000000 drafter-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 14:09:28.619418 drafter-1.1.0/drafter.egg-info/
+-rw-rw-rw-   0        0        0      766 2024-04-29 14:09:28.000000 drafter-1.1.0/drafter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-29 14:09:28.000000 drafter-1.1.0/drafter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 14:09:28.000000 drafter-1.1.0/drafter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-29 14:09:28.000000 drafter-1.1.0/drafter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-29 14:09:28.000000 drafter-1.1.0/drafter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1027 2024-04-25 16:30:29.000000 drafter-1.1.0/drafter.py
+-rw-rw-rw-   0        0        0       80 2023-08-30 14:30:23.000000 drafter-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 14:09:28.620414 drafter-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-09-09 13:39:14.000000 drafter-1.1.0/setup.py
```

### Comparing `drafter-1.0.5/LICENSE.txt` & `drafter-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drafter-1.0.5/PKG-INFO` & `drafter-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drafter
-Version: 1.0.5
+Version: 1.1.0
 Summary: Student-friendly full stack web development library.
 Home-page: https://github.com/drafter-edu/drafter
 Author: acbart
 Author-email: acbart@udel.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Education
```

### Comparing `drafter-1.0.5/drafter.egg-info/PKG-INFO` & `drafter-1.1.0/drafter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drafter
-Version: 1.0.5
+Version: 1.1.0
 Summary: Student-friendly full stack web development library.
 Home-page: https://github.com/drafter-edu/drafter
 Author: acbart
 Author-email: acbart@udel.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Education
```

### Comparing `drafter-1.0.5/setup.py` & `drafter-1.1.0/setup.py`

 * *Files identical despite different names*

