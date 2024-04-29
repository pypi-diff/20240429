# Comparing `tmp/automea-0.0.4.tar.gz` & `tmp/automea-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automea-0.0.4.tar", last modified: Mon Mar  4 10:59:34 2024, max compression
+gzip compressed data, was "automea-0.0.5.tar", last modified: Mon Apr 29 07:52:55 2024, max compression
```

## Comparing `automea-0.0.4.tar` & `automea-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 vini       (501) staff       (20)        0 2024-03-04 10:59:34.866140 automea-0.0.4/
--rw-r--r--   0 vini       (501) staff       (20)     1075 2024-02-27 18:20:17.000000 automea-0.0.4/LICENSE
--rw-r--r--   0 vini       (501) staff       (20)     1083 2024-03-04 10:59:34.865959 automea-0.0.4/PKG-INFO
--rw-r--r--   0 vini       (501) staff       (20)      630 2024-02-27 18:23:57.000000 automea-0.0.4/README.md
-drwxr-xr-x   0 vini       (501) staff       (20)        0 2024-03-04 10:59:34.864737 automea-0.0.4/automea/
--rw-r--r--   0 vini       (501) staff       (20)    54207 2024-03-04 10:57:58.000000 automea-0.0.4/automea/__init__.py
-drwxr-xr-x   0 vini       (501) staff       (20)        0 2024-03-04 10:59:34.865506 automea-0.0.4/automea/training/
--rw-r--r--   0 vini       (501) staff       (20)     5451 2024-01-29 13:23:18.000000 automea-0.0.4/automea/training/models.py
--rw-r--r--   0 vini       (501) staff       (20)    13333 2024-02-27 17:20:57.000000 automea-0.0.4/automea/util.py
-drwxr-xr-x   0 vini       (501) staff       (20)        0 2024-03-04 10:59:34.865789 automea-0.0.4/automea.egg-info/
--rw-r--r--   0 vini       (501) staff       (20)     1083 2024-03-04 10:59:34.000000 automea-0.0.4/automea.egg-info/PKG-INFO
--rw-r--r--   0 vini       (501) staff       (20)      219 2024-03-04 10:59:34.000000 automea-0.0.4/automea.egg-info/SOURCES.txt
--rw-r--r--   0 vini       (501) staff       (20)        1 2024-03-04 10:59:34.000000 automea-0.0.4/automea.egg-info/dependency_links.txt
--rw-r--r--   0 vini       (501) staff       (20)        8 2024-03-04 10:59:34.000000 automea-0.0.4/automea.egg-info/top_level.txt
--rw-r--r--   0 vini       (501) staff       (20)      445 2024-03-04 10:59:28.000000 automea-0.0.4/pyproject.toml
--rw-r--r--   0 vini       (501) staff       (20)       38 2024-03-04 10:59:34.866188 automea-0.0.4/setup.cfg
+drwxr-xr-x   0 vini       (501) staff       (20)        0 2024-04-29 07:52:55.970856 automea-0.0.5/
+-rw-r--r--   0 vini       (501) staff       (20)     1075 2024-02-27 18:20:17.000000 automea-0.0.5/LICENSE
+-rw-r--r--   0 vini       (501) staff       (20)     1083 2024-04-29 07:52:55.970660 automea-0.0.5/PKG-INFO
+-rw-r--r--   0 vini       (501) staff       (20)      630 2024-02-27 18:23:57.000000 automea-0.0.5/README.md
+-rw-r--r--   0 vini       (501) staff       (20)      496 2024-04-29 07:52:18.000000 automea-0.0.5/pyproject.toml
+-rw-r--r--   0 vini       (501) staff       (20)       38 2024-04-29 07:52:55.970905 automea-0.0.5/setup.cfg
+drwxr-xr-x   0 vini       (501) staff       (20)        0 2024-04-29 07:52:55.967978 automea-0.0.5/src/
+-rw-r--r--   0 vini       (501) staff       (20)       30 2024-04-25 08:49:20.000000 automea-0.0.5/src/__init__.py
+-rw-r--r--   0 vini       (501) staff       (20)    95701 2024-04-09 12:33:21.000000 automea-0.0.5/src/__main__.py
+drwxr-xr-x   0 vini       (501) staff       (20)        0 2024-04-29 07:52:55.969116 automea-0.0.5/src/automea/
+-rw-r--r--   0 vini       (501) staff       (20)       30 2024-04-25 08:49:20.000000 automea-0.0.5/src/automea/__init__.py
+-rw-r--r--   0 vini       (501) staff       (20)    95701 2024-04-09 12:33:21.000000 automea-0.0.5/src/automea/__main__.py
+drwxr-xr-x   0 vini       (501) staff       (20)        0 2024-04-29 07:52:55.969927 automea-0.0.5/src/automea/training/
+-rw-r--r--   0 vini       (501) staff       (20)     5451 2024-01-29 13:23:18.000000 automea-0.0.5/src/automea/training/models.py
+-rw-r--r--   0 vini       (501) staff       (20)    13333 2024-02-27 17:20:57.000000 automea-0.0.5/src/automea/util.py
+drwxr-xr-x   0 vini       (501) staff       (20)        0 2024-04-29 07:52:55.970432 automea-0.0.5/src/automea.egg-info/
+-rw-r--r--   0 vini       (501) staff       (20)     1083 2024-04-29 07:52:55.000000 automea-0.0.5/src/automea.egg-info/PKG-INFO
+-rw-r--r--   0 vini       (501) staff       (20)      315 2024-04-29 07:52:55.000000 automea-0.0.5/src/automea.egg-info/SOURCES.txt
+-rw-r--r--   0 vini       (501) staff       (20)        1 2024-04-29 07:52:55.000000 automea-0.0.5/src/automea.egg-info/dependency_links.txt
+-rw-r--r--   0 vini       (501) staff       (20)       31 2024-04-29 07:52:55.000000 automea-0.0.5/src/automea.egg-info/top_level.txt
+-rw-r--r--   0 vini       (501) staff       (20)    13333 2024-02-27 17:20:57.000000 automea-0.0.5/src/util.py
```

### Comparing `automea-0.0.4/LICENSE` & `automea-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `automea-0.0.4/PKG-INFO` & `automea-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automea
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automated analysis of MEA datasets
 Author-email: Vinicius Hernandes <viniciusfhernandes@gmail.com>
 Project-URL: Homepage, https://gitlab.com/QMAI/papers/autoMEA
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `automea-0.0.4/README.md` & `automea-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `automea-0.0.4/automea/training/models.py` & `automea-0.0.5/src/automea/training/models.py`

 * *Files identical despite different names*

### Comparing `automea-0.0.4/automea/util.py` & `automea-0.0.5/src/automea/util.py`

 * *Files identical despite different names*

### Comparing `automea-0.0.4/automea.egg-info/PKG-INFO` & `automea-0.0.5/src/automea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automea
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automated analysis of MEA datasets
 Author-email: Vinicius Hernandes <viniciusfhernandes@gmail.com>
 Project-URL: Homepage, https://gitlab.com/QMAI/papers/autoMEA
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

