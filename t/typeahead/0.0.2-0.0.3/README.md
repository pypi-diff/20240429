# Comparing `tmp/typeahead-0.0.2.tar.gz` & `tmp/typeahead-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeahead-0.0.2.tar", last modified: Mon Apr 29 15:17:31 2024, max compression
+gzip compressed data, was "typeahead-0.0.3.tar", last modified: Mon Apr 29 15:19:39 2024, max compression
```

## Comparing `typeahead-0.0.2.tar` & `typeahead-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 15:17:30.715973 typeahead-0.0.2/
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      568 2024-04-29 15:17:30.712891 typeahead-0.0.2/PKG-INFO
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       38 2024-04-29 15:17:30.716974 typeahead-0.0.2/setup.cfg
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      725 2024-04-29 15:16:18.000000 typeahead-0.0.2/setup.py
-drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 15:17:30.616822 typeahead-0.0.2/typeahead/
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       31 2024-04-29 15:12:40.000000 typeahead-0.0.2/typeahead/__init__.py
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)     3376 2024-01-19 11:27:49.000000 typeahead-0.0.2/typeahead/auto_complete.py
-drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 15:17:30.692173 typeahead-0.0.2/typeahead.egg-info/
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      568 2024-04-29 15:17:30.000000 typeahead-0.0.2/typeahead.egg-info/PKG-INFO
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      189 2024-04-29 15:17:30.000000 typeahead-0.0.2/typeahead.egg-info/SOURCES.txt
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        1 2024-04-29 15:17:30.000000 typeahead-0.0.2/typeahead.egg-info/dependency_links.txt
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       10 2024-04-29 15:17:30.000000 typeahead-0.0.2/typeahead.egg-info/top_level.txt
+drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 15:19:39.455265 typeahead-0.0.3/
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      568 2024-04-29 15:19:39.451752 typeahead-0.0.3/PKG-INFO
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       38 2024-04-29 15:19:39.456265 typeahead-0.0.3/setup.cfg
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      725 2024-04-29 15:19:31.000000 typeahead-0.0.3/setup.py
+drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 15:19:39.333260 typeahead-0.0.3/typeahead/
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       35 2024-04-29 15:19:06.000000 typeahead-0.0.3/typeahead/__init__.py
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)     3376 2024-01-19 11:27:49.000000 typeahead-0.0.3/typeahead/auto_complete.py
+drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 15:19:39.426569 typeahead-0.0.3/typeahead.egg-info/
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      568 2024-04-29 15:19:39.000000 typeahead-0.0.3/typeahead.egg-info/PKG-INFO
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      189 2024-04-29 15:19:39.000000 typeahead-0.0.3/typeahead.egg-info/SOURCES.txt
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        1 2024-04-29 15:19:39.000000 typeahead-0.0.3/typeahead.egg-info/dependency_links.txt
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       10 2024-04-29 15:19:39.000000 typeahead-0.0.3/typeahead.egg-info/top_level.txt
```

### Comparing `typeahead-0.0.2/PKG-INFO` & `typeahead-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeahead
-Version: 0.0.2
+Version: 0.0.3
 Summary: Typeahead feature
 Home-page: UNKNOWN
 Author: techy_cereal 
 Author-email: alexanderjmilliken@gmail.com
 License: UNKNOWN
 Keywords: python,typeahead,auto complete
 Platform: UNKNOWN
```

### Comparing `typeahead-0.0.2/setup.py` & `typeahead-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Typeahead feature'
 
 # Setting up
 setup(
     name="typeahead",
     version=VERSION,
     author="techy_cereal ",
```

### Comparing `typeahead-0.0.2/typeahead/auto_complete.py` & `typeahead-0.0.3/typeahead/auto_complete.py`

 * *Files identical despite different names*

### Comparing `typeahead-0.0.2/typeahead.egg-info/PKG-INFO` & `typeahead-0.0.3/typeahead.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeahead
-Version: 0.0.2
+Version: 0.0.3
 Summary: Typeahead feature
 Home-page: UNKNOWN
 Author: techy_cereal 
 Author-email: alexanderjmilliken@gmail.com
 License: UNKNOWN
 Keywords: python,typeahead,auto complete
 Platform: UNKNOWN
```

