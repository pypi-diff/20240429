# Comparing `tmp/easylogger4dev_alpha-0.1.2.tar.gz` & `tmp/easylogger4dev_alpha-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easylogger4dev_alpha-0.1.2.tar", last modified: Sun Apr 28 10:16:55 2024, max compression
+gzip compressed data, was "easylogger4dev_alpha-0.1.3.tar", last modified: Mon Apr 29 05:56:27 2024, max compression
```

## Comparing `easylogger4dev_alpha-0.1.2.tar` & `easylogger4dev_alpha-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 10:16:55.080000 easylogger4dev_alpha-0.1.2/
--rw-rw-rw-   0        0        0     1091 2024-04-27 23:51:28.000000 easylogger4dev_alpha-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      306 2024-04-28 10:16:56.000000 easylogger4dev_alpha-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-25 06:19:42.000000 easylogger4dev_alpha-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 10:16:55.110000 easylogger4dev_alpha-0.1.2/easylogger4dev_alpha/
--rw-rw-rw-   0        0        0       13 2024-04-28 10:15:46.000000 easylogger4dev_alpha-0.1.2/easylogger4dev_alpha/__init__.py
--rw-rw-rw-   0        0        0     8693 2024-04-28 06:21:52.000000 easylogger4dev_alpha-0.1.2/easylogger4dev_alpha/module.py
-drwxrwxrwx   0        0        0        0 2024-04-28 10:16:55.140000 easylogger4dev_alpha-0.1.2/easylogger4dev_alpha.egg-info/
--rw-rw-rw-   0        0        0      306 2024-04-28 10:16:56.000000 easylogger4dev_alpha-0.1.2/easylogger4dev_alpha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-04-28 10:16:56.000000 easylogger4dev_alpha-0.1.2/easylogger4dev_alpha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 10:16:56.000000 easylogger4dev_alpha-0.1.2/easylogger4dev_alpha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-28 10:16:56.000000 easylogger4dev_alpha-0.1.2/easylogger4dev_alpha.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-04-28 10:16:56.000000 easylogger4dev_alpha-0.1.2/easylogger4dev_alpha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 10:16:56.000000 easylogger4dev_alpha-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      397 2024-04-28 10:15:46.000000 easylogger4dev_alpha-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 10:16:55.170000 easylogger4dev_alpha-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2024-04-25 06:18:48.000000 easylogger4dev_alpha-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0     9271 2024-04-28 06:21:52.000000 easylogger4dev_alpha-0.1.2/tests/test_module.py
+drwxrwxrwx   0        0        0        0 2024-04-29 05:56:27.270000 easylogger4dev_alpha-0.1.3/
+-rw-rw-rw-   0        0        0     1091 2024-04-27 23:51:28.000000 easylogger4dev_alpha-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      306 2024-04-29 05:56:28.000000 easylogger4dev_alpha-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-25 06:19:42.000000 easylogger4dev_alpha-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 05:56:27.300000 easylogger4dev_alpha-0.1.3/easylogger4dev_alpha/
+-rw-rw-rw-   0        0        0     8697 2024-04-29 05:54:20.000000 easylogger4dev_alpha-0.1.3/easylogger4dev_alpha/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 05:56:27.330000 easylogger4dev_alpha-0.1.3/easylogger4dev_alpha.egg-info/
+-rw-rw-rw-   0        0        0      306 2024-04-29 05:56:28.000000 easylogger4dev_alpha-0.1.3/easylogger4dev_alpha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2024-04-29 05:56:28.000000 easylogger4dev_alpha-0.1.3/easylogger4dev_alpha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 05:56:28.000000 easylogger4dev_alpha-0.1.3/easylogger4dev_alpha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-29 05:56:28.000000 easylogger4dev_alpha-0.1.3/easylogger4dev_alpha.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-04-29 05:56:28.000000 easylogger4dev_alpha-0.1.3/easylogger4dev_alpha.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 05:56:28.000000 easylogger4dev_alpha-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      397 2024-04-29 05:54:30.000000 easylogger4dev_alpha-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 05:56:27.360000 easylogger4dev_alpha-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-25 06:18:48.000000 easylogger4dev_alpha-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     9271 2024-04-28 06:21:52.000000 easylogger4dev_alpha-0.1.3/tests/test_module.py
```

### Comparing `easylogger4dev_alpha-0.1.2/LICENSE.txt` & `easylogger4dev_alpha-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easylogger4dev_alpha-0.1.2/easylogger4dev_alpha/module.py` & `easylogger4dev_alpha-0.1.3/easylogger4dev_alpha/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,7 +204,9 @@
             return result
 
         return wrapper
 
     return log_decorator
 
 
+
+
```

### Comparing `easylogger4dev_alpha-0.1.2/tests/test_module.py` & `easylogger4dev_alpha-0.1.3/tests/test_module.py`

 * *Files identical despite different names*

