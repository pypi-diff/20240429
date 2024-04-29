# Comparing `tmp/Calculator_tvaino-0.0.5.tar.gz` & `tmp/Calculator_tvaino-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Calculator_tvaino-0.0.5.tar", last modified: Thu Mar 28 20:19:30 2024, max compression
+gzip compressed data, was "Calculator_tvaino-0.0.6.tar", last modified: Wed Apr  3 07:51:57 2024, max compression
```

## Comparing `Calculator_tvaino-0.0.5.tar` & `Calculator_tvaino-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 20:19:30.891275 Calculator_tvaino-0.0.5/
--rw-rw-rw-   0        0        0     1102 2024-03-19 16:40:28.000000 Calculator_tvaino-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2226 2024-03-28 20:19:30.889261 Calculator_tvaino-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1842 2024-03-28 20:13:17.000000 Calculator_tvaino-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-03-28 20:19:30.891275 Calculator_tvaino-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-03-28 20:19:22.000000 Calculator_tvaino-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-28 20:19:30.872296 Calculator_tvaino-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-03-28 20:19:30.887261 Calculator_tvaino-0.0.5/src/Calculator_tvaino.egg-info/
--rw-rw-rw-   0        0        0     2226 2024-03-28 20:19:30.000000 Calculator_tvaino-0.0.5/src/Calculator_tvaino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2024-03-28 20:19:30.000000 Calculator_tvaino-0.0.5/src/Calculator_tvaino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 20:19:30.000000 Calculator_tvaino-0.0.5/src/Calculator_tvaino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 20:19:30.000000 Calculator_tvaino-0.0.5/src/Calculator_tvaino.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 07:51:57.970665 Calculator_tvaino-0.0.6/
+-rw-rw-rw-   0        0        0     1102 2024-03-19 16:40:28.000000 Calculator_tvaino-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2226 2024-04-03 07:51:57.962596 Calculator_tvaino-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1842 2024-03-28 20:13:17.000000 Calculator_tvaino-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 07:51:57.970665 Calculator_tvaino-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-04-03 07:51:52.000000 Calculator_tvaino-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:51:57.930590 Calculator_tvaino-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 07:51:57.959094 Calculator_tvaino-0.0.6/src/Calculator_tvaino.egg-info/
+-rw-rw-rw-   0        0        0     2226 2024-04-03 07:51:57.000000 Calculator_tvaino-0.0.6/src/Calculator_tvaino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2024-04-03 07:51:57.000000 Calculator_tvaino-0.0.6/src/Calculator_tvaino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 07:51:57.000000 Calculator_tvaino-0.0.6/src/Calculator_tvaino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 07:51:57.000000 Calculator_tvaino-0.0.6/src/Calculator_tvaino.egg-info/top_level.txt
```

### Comparing `Calculator_tvaino-0.0.5/LICENSE` & `Calculator_tvaino-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Calculator_tvaino-0.0.5/PKG-INFO` & `Calculator_tvaino-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Calculator_tvaino
-Version: 0.0.5
+Version: 0.0.6
 Summary: Performs basic arithmetic operations
 Home-page: https://github.com/TuringCollegeSubmissions/tvaino-DWWP.1.5/tree/master/Calculator_pack
 Author: Tomas Vainoras
 Author-email: vainoras@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Calculator_tvaino-0.0.5/README.md` & `Calculator_tvaino-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `Calculator_tvaino-0.0.5/setup.py` & `Calculator_tvaino-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Package metadata
 NAME = 'Calculator_tvaino'
 DESCRIPTION = 'Performs basic arithmetic operations'
 URL = 'https://github.com/TuringCollegeSubmissions/tvaino-DWWP.1.5/tree/master/Calculator_pack'
 AUTHOR = 'Tomas Vainoras'
 EMAIL = 'vainoras@gmail.com'
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 
 # Package dependencies
 INSTALL_REQUIRES = [
     # List your dependencies herepip
 ]
 
 # Additional package metadata
```

### Comparing `Calculator_tvaino-0.0.5/src/Calculator_tvaino.egg-info/PKG-INFO` & `Calculator_tvaino-0.0.6/src/Calculator_tvaino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Calculator_tvaino
-Version: 0.0.5
+Version: 0.0.6
 Summary: Performs basic arithmetic operations
 Home-page: https://github.com/TuringCollegeSubmissions/tvaino-DWWP.1.5/tree/master/Calculator_pack
 Author: Tomas Vainoras
 Author-email: vainoras@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

