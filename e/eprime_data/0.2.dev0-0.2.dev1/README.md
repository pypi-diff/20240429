# Comparing `tmp/eprime_data-0.2.dev0.tar.gz` & `tmp/eprime_data-0.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eprime_data-0.2.dev0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "eprime_data-0.2.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `eprime_data-0.2.dev0.tar` & `eprime_data-0.2.dev1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2729 2024-04-29 14:07:21.506799 eprime_data-0.2.dev0/.gitignore
--rw-r--r--   0        0        0     1073 2024-04-29 13:50:49.074138 eprime_data-0.2.dev0/LICENSE
--rw-r--r--   0        0        0      125 2024-04-29 13:51:53.987008 eprime_data-0.2.dev0/README.md
--rw-r--r--   0        0        0      459 2024-04-29 16:12:35.555676 eprime_data-0.2.dev0/eprime_data/__init__.py
--rw-r--r--   0        0        0     3186 2024-04-29 16:05:49.600798 eprime_data-0.2.dev0/eprime_data/__main__.py
--rw-r--r--   0        0        0      357 2024-04-29 14:25:02.149348 eprime_data-0.2.dev0/eprime_data/constants.py
--rw-r--r--   0        0        0      811 2024-04-29 14:29:49.137905 eprime_data-0.2.dev0/eprime_data/dataframe.py
--rw-r--r--   0        0        0     1658 2024-04-29 14:21:55.678214 eprime_data-0.2.dev0/eprime_data/dict_tab_data.py
--rw-r--r--   0        0        0     3980 2024-04-29 16:05:17.960257 eprime_data-0.2.dev0/eprime_data/lib.py
--rw-r--r--   0        0        0      539 2024-04-29 16:13:21.612450 eprime_data-0.2.dev0/pyproject.toml
--rw-r--r--   0        0        0      360 1970-01-01 00:00:00.000000 eprime_data-0.2.dev0/PKG-INFO
+-rw-r--r--   0        0        0     2729 2024-04-29 14:07:21.506799 eprime_data-0.2.dev1/.gitignore
+-rw-r--r--   0        0        0     1073 2024-04-29 13:50:49.074138 eprime_data-0.2.dev1/LICENSE
+-rw-r--r--   0        0        0      125 2024-04-29 13:51:53.987008 eprime_data-0.2.dev1/README.md
+-rw-r--r--   0        0        0      459 2024-04-29 16:18:01.861145 eprime_data-0.2.dev1/eprime_data/__init__.py
+-rw-r--r--   0        0        0     3186 2024-04-29 16:05:49.600798 eprime_data-0.2.dev1/eprime_data/__main__.py
+-rw-r--r--   0        0        0      357 2024-04-29 14:25:02.149348 eprime_data-0.2.dev1/eprime_data/constants.py
+-rw-r--r--   0        0        0      811 2024-04-29 14:29:49.137905 eprime_data-0.2.dev1/eprime_data/dataframe.py
+-rw-r--r--   0        0        0     1658 2024-04-29 14:21:55.678214 eprime_data-0.2.dev1/eprime_data/dict_tab_data.py
+-rw-r--r--   0        0        0     3980 2024-04-29 16:05:17.960257 eprime_data-0.2.dev1/eprime_data/lib.py
+-rw-r--r--   0        0        0      539 2024-04-29 16:17:46.896895 eprime_data-0.2.dev1/pyproject.toml
+-rw-r--r--   0        0        0      360 1970-01-01 00:00:00.000000 eprime_data-0.2.dev1/PKG-INFO
```

### Comparing `eprime_data-0.2.dev0/.gitignore` & `eprime_data-0.2.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `eprime_data-0.2.dev0/LICENSE` & `eprime_data-0.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `eprime_data-0.2.dev0/eprime_data/__main__.py` & `eprime_data-0.2.dev1/eprime_data/__main__.py`

 * *Files identical despite different names*

### Comparing `eprime_data-0.2.dev0/eprime_data/dataframe.py` & `eprime_data-0.2.dev1/eprime_data/dataframe.py`

 * *Files identical despite different names*

### Comparing `eprime_data-0.2.dev0/eprime_data/dict_tab_data.py` & `eprime_data-0.2.dev1/eprime_data/dict_tab_data.py`

 * *Files identical despite different names*

### Comparing `eprime_data-0.2.dev0/eprime_data/lib.py` & `eprime_data-0.2.dev1/eprime_data/lib.py`

 * *Files identical despite different names*

### Comparing `eprime_data-0.2.dev0/pyproject.toml` & `eprime_data-0.2.dev1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 requires-python = ">=3.8"
 dependencies =  []
 
 [project.optional-dependencies]
 pandas = ["pandas>=2.1"]
 
 [project.scripts]
-pyexam = "eprime_data.__main__:run"
+pyexam = "eprime_data.__main__:cli"
 
 [project.urls]
 Home = "https://github.com/lindemann09/eprime-data"
```

