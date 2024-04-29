# Comparing `tmp/audiness-0.3.2.tar.gz` & `tmp/audiness-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiness-0.3.2.tar", max compression
+gzip compressed data, was "audiness-0.4.0.tar", max compression
```

## Comparing `audiness-0.3.2.tar` & `audiness-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1112 2024-02-17 20:42:20.911611 audiness-0.3.2/LICENSE
--rw-r--r--   0        0        0     4983 2024-04-01 20:55:34.004187 audiness-0.3.2/README.md
--rw-r--r--   0        0        0       39 2024-02-18 00:47:45.686574 audiness-0.3.2/audiness/__init__.py
--rw-r--r--   0        0        0       51 2024-02-18 00:47:45.686574 audiness-0.3.2/audiness/commands/__init__.py
--rw-r--r--   0        0        0     1353 2024-02-29 12:00:55.323746 audiness-0.3.2/audiness/commands/folders.py
--rw-r--r--   0        0        0      973 2024-03-05 22:22:18.529099 audiness-0.3.2/audiness/commands/policies.py
--rw-r--r--   0        0        0     2967 2024-04-10 21:42:07.914924 audiness-0.3.2/audiness/commands/scans.py
--rw-r--r--   0        0        0     1793 2024-03-05 22:23:39.485777 audiness-0.3.2/audiness/commands/server.py
--rw-r--r--   0        0        0      231 2024-02-29 12:00:55.323746 audiness-0.3.2/audiness/commands/software.py
--rw-r--r--   0        0        0      646 2024-03-05 20:35:05.159941 audiness-0.3.2/audiness/helpers.py
--rw-r--r--   0        0        0     1577 2024-03-05 22:22:18.530099 audiness-0.3.2/audiness/main.py
--rw-r--r--   0        0        0      703 2024-04-10 21:43:25.378827 audiness-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5801 1970-01-01 00:00:00.000000 audiness-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-02-17 20:42:20.911611 audiness-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4983 2024-04-01 20:55:34.004187 audiness-0.4.0/README.md
+-rw-r--r--   0        0        0       39 2024-02-18 00:47:45.686574 audiness-0.4.0/audiness/__init__.py
+-rw-r--r--   0        0        0       51 2024-02-18 00:47:45.686574 audiness-0.4.0/audiness/commands/__init__.py
+-rw-r--r--   0        0        0     1353 2024-02-29 12:00:55.323746 audiness-0.4.0/audiness/commands/folders.py
+-rw-r--r--   0        0        0      973 2024-03-05 22:22:18.529099 audiness-0.4.0/audiness/commands/policies.py
+-rw-r--r--   0        0        0     2967 2024-04-10 21:42:07.914924 audiness-0.4.0/audiness/commands/scans.py
+-rw-r--r--   0        0        0     1793 2024-03-05 22:23:39.485777 audiness-0.4.0/audiness/commands/server.py
+-rw-r--r--   0        0        0      231 2024-02-29 12:00:55.323746 audiness-0.4.0/audiness/commands/software.py
+-rw-r--r--   0        0        0      646 2024-03-05 20:35:05.159941 audiness-0.4.0/audiness/helpers.py
+-rw-r--r--   0        0        0     1577 2024-03-05 22:22:18.530099 audiness-0.4.0/audiness/main.py
+-rw-r--r--   0        0        0      674 2024-04-22 19:35:21.602743 audiness-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5797 1970-01-01 00:00:00.000000 audiness-0.4.0/PKG-INFO
```

### Comparing `audiness-0.3.2/LICENSE` & `audiness-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audiness-0.3.2/README.md` & `audiness-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `audiness-0.3.2/audiness/commands/folders.py` & `audiness-0.4.0/audiness/commands/folders.py`

 * *Files identical despite different names*

### Comparing `audiness-0.3.2/audiness/commands/policies.py` & `audiness-0.4.0/audiness/commands/policies.py`

 * *Files identical despite different names*

### Comparing `audiness-0.3.2/audiness/commands/scans.py` & `audiness-0.4.0/audiness/commands/scans.py`

 * *Files identical despite different names*

### Comparing `audiness-0.3.2/audiness/commands/server.py` & `audiness-0.4.0/audiness/commands/server.py`

 * *Files identical despite different names*

### Comparing `audiness-0.3.2/audiness/helpers.py` & `audiness-0.4.0/audiness/helpers.py`

 * *Files identical despite different names*

### Comparing `audiness-0.3.2/audiness/main.py` & `audiness-0.4.0/audiness/main.py`

 * *Files identical despite different names*

### Comparing `audiness-0.3.2/PKG-INFO` & `audiness-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: audiness
-Version: 0.3.2
+Version: 0.4.0
 Summary: CLI tool to interact with Tenable's Nessus
 Home-page: https://github.com/audiusGmbH/audiness
 License: MIT
 Keywords: vulnerabilites,nessus
 Author: Fabian Affolter
 Author-email: fabian-affolter@audius.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pytenable (>=1.4,<2.0)
-Requires-Dist: typer[all] (>=0.9,<0.10)
+Requires-Dist: typer (>=0.12,<0.13)
 Requires-Dist: validators (>=0.24,<0.25)
 Project-URL: Repository, https://github.com/audiusGmbH/audiness
 Description-Content-Type: text/markdown
 
 # audiness
 
 Helper scripts to interact with Nessus instances. The CLI allows one to perform tasks on a
```

