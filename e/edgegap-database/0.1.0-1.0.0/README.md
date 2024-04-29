# Comparing `tmp/edgegap_database-0.1.0.tar.gz` & `tmp/edgegap_database-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_database-0.1.0.tar", max compression
+gzip compressed data, was "edgegap_database-1.0.0.tar", max compression
```

## Comparing `edgegap_database-0.1.0.tar` & `edgegap_database-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.387671 edgegap_database-0.1.0/LICENSE
--rw-r--r--   0        0        0     2180 2024-04-29 14:47:44.435202 edgegap_database-0.1.0/README.md
--rw-r--r--   0        0        0      386 2024-04-25 13:10:38.953085 edgegap_database-0.1.0/edgegap_database/__init__.py
--rw-r--r--   0        0        0      624 2024-04-25 15:14:43.477927 edgegap_database-0.1.0/edgegap_database/_base.py
--rw-r--r--   0        0        0      452 2024-04-25 13:10:38.953272 edgegap_database-0.1.0/edgegap_database/_configuration.py
--rw-r--r--   0        0        0     1004 2024-04-27 04:24:27.843726 edgegap_database-0.1.0/edgegap_database/_engine.py
--rw-r--r--   0        0        0      885 2024-04-25 13:10:38.953460 edgegap_database-0.1.0/edgegap_database/_factory.py
--rw-r--r--   0        0        0      253 2024-04-25 13:10:38.953551 edgegap_database-0.1.0/edgegap_database/_model.py
--rw-r--r--   0        0        0     2555 2024-04-27 03:45:50.877085 edgegap_database-0.1.0/edgegap_database/_operator.py
--rw-r--r--   0        0        0      509 2024-04-25 13:10:38.953733 edgegap_database-0.1.0/edgegap_database/_session.py
--rw-r--r--   0        0        0      325 2024-04-25 13:10:38.953823 edgegap_database-0.1.0/edgegap_database/errors/__init__.py
--rw-r--r--   0        0        0      698 2024-04-25 13:10:38.954025 edgegap_database-0.1.0/edgegap_database/errors/_exceptions.py
--rw-r--r--   0        0        0      484 2024-04-25 13:10:38.954108 edgegap_database-0.1.0/edgegap_database/errors/_factory.py
--rw-r--r--   0        0        0      542 2024-04-29 14:48:34.022065 edgegap_database-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2950 1970-01-01 00:00:00.000000 edgegap_database-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 18:13:42.710660 edgegap_database-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2180 2024-04-29 18:13:42.710660 edgegap_database-1.0.0/README.md
+-rw-r--r--   0        0        0      386 2024-04-29 18:13:42.710660 edgegap_database-1.0.0/edgegap_database/__init__.py
+-rw-r--r--   0        0        0      624 2024-04-29 18:13:42.710660 edgegap_database-1.0.0/edgegap_database/_base.py
+-rw-r--r--   0        0        0      452 2024-04-29 18:13:42.710660 edgegap_database-1.0.0/edgegap_database/_configuration.py
+-rw-r--r--   0        0        0     1004 2024-04-29 18:13:42.710660 edgegap_database-1.0.0/edgegap_database/_engine.py
+-rw-r--r--   0        0        0      885 2024-04-29 18:13:42.710660 edgegap_database-1.0.0/edgegap_database/_factory.py
+-rw-r--r--   0        0        0      253 2024-04-29 18:13:42.710660 edgegap_database-1.0.0/edgegap_database/_model.py
+-rw-r--r--   0        0        0     2555 2024-04-29 18:13:42.710660 edgegap_database-1.0.0/edgegap_database/_operator.py
+-rw-r--r--   0        0        0      509 2024-04-29 18:13:42.710660 edgegap_database-1.0.0/edgegap_database/_session.py
+-rw-r--r--   0        0        0      325 2024-04-29 18:13:42.710660 edgegap_database-1.0.0/edgegap_database/errors/__init__.py
+-rw-r--r--   0        0        0      698 2024-04-29 18:13:42.710660 edgegap_database-1.0.0/edgegap_database/errors/_exceptions.py
+-rw-r--r--   0        0        0      484 2024-04-29 18:13:42.710660 edgegap_database-1.0.0/edgegap_database/errors/_factory.py
+-rw-r--r--   0        0        0      542 2024-04-29 18:13:59.198748 edgegap_database-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 edgegap_database-1.0.0/PKG-INFO
```

### Comparing `edgegap_database-0.1.0/LICENSE` & `edgegap_database-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_database-0.1.0/README.md` & `edgegap_database-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_database-0.1.0/edgegap_database/_base.py` & `edgegap_database-1.0.0/edgegap_database/_base.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-0.1.0/edgegap_database/_engine.py` & `edgegap_database-1.0.0/edgegap_database/_engine.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-0.1.0/edgegap_database/_factory.py` & `edgegap_database-1.0.0/edgegap_database/_factory.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-0.1.0/edgegap_database/_operator.py` & `edgegap_database-1.0.0/edgegap_database/_operator.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-0.1.0/edgegap_database/errors/_exceptions.py` & `edgegap_database-1.0.0/edgegap_database/errors/_exceptions.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-0.1.0/pyproject.toml` & `edgegap_database-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-database"
-version = "0.1.0"
+version = "1.0.0"
 description = "The Edgegap Database library includes various tools and helpers for interacting with Database and Migrations. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 psycopg-c = "^3.1.18"
```

### Comparing `edgegap_database-0.1.0/PKG-INFO` & `edgegap_database-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: edgegap-database
-Version: 0.1.0
+Version: 1.0.0
 Summary: The Edgegap Database library includes various tools and helpers for interacting with Database and Migrations. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: psycopg-c (>=3.1.18,<4.0.0)
 Requires-Dist: psycopg2 (>=2.9.9,<3.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: sqlmodel (>=0.0.16,<0.0.17)
 Description-Content-Type: text/markdown
```

