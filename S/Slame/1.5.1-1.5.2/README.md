# Comparing `tmp/Slame-1.5.1.tar.gz` & `tmp/Slame-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slame-1.5.1.tar", last modified: Fri Apr 19 09:45:49 2024, max compression
+gzip compressed data, was "Slame-1.5.2.tar", last modified: Mon Apr 29 14:48:21 2024, max compression
```

## Comparing `Slame-1.5.1.tar` & `Slame-1.5.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-19 09:45:49.691036 Slame-1.5.1/
--rw-rw-r--   0 dev       (1000) dev       (1000)      895 2024-04-19 09:45:49.691036 Slame-1.5.1/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)     2112 2024-03-24 11:40:44.000000 Slame-1.5.1/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-19 09:45:49.691036 Slame-1.5.1/Slame/
--rw-r--r--   0 dev       (1000) dev       (1000)      232 2024-04-19 09:45:15.000000 Slame-1.5.1/Slame/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-03-27 12:15:44.000000 Slame-1.5.1/Slame/menu.py
--rw-r--r--   0 dev       (1000) dev       (1000)    12287 2024-03-27 12:44:02.000000 Slame-1.5.1/Slame/slame.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-19 09:45:49.691036 Slame-1.5.1/Slame.egg-info/
--rw-r--r--   0 dev       (1000) dev       (1000)      895 2024-04-19 09:45:49.000000 Slame-1.5.1/Slame.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)      219 2024-04-19 09:45:49.000000 Slame-1.5.1/Slame.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        1 2024-04-19 09:45:49.000000 Slame-1.5.1/Slame.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       19 2024-04-19 09:45:49.000000 Slame-1.5.1/Slame.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        6 2024-04-19 09:45:49.000000 Slame-1.5.1/Slame.egg-info/top_level.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       38 2024-04-19 09:45:49.695036 Slame-1.5.1/setup.cfg
--rw-r--r--   0 dev       (1000) dev       (1000)     1253 2024-04-19 09:44:25.000000 Slame-1.5.1/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-29 14:48:21.162762 Slame-1.5.2/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      895 2024-04-29 14:48:21.162762 Slame-1.5.2/PKG-INFO
+-rw-r--r--   0 dev       (1000) dev       (1000)     2112 2024-03-24 11:40:44.000000 Slame-1.5.2/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-29 14:48:21.162762 Slame-1.5.2/Slame/
+-rw-r--r--   0 dev       (1000) dev       (1000)      233 2024-04-29 14:45:27.000000 Slame-1.5.2/Slame/__init__.py
+-rw-r--r--   0 dev       (1000) dev       (1000)    12287 2024-03-27 12:44:02.000000 Slame-1.5.2/Slame/slame.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-29 14:48:21.162762 Slame-1.5.2/Slame.egg-info/
+-rw-r--r--   0 dev       (1000) dev       (1000)      895 2024-04-29 14:48:21.000000 Slame-1.5.2/Slame.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) dev       (1000)      205 2024-04-29 14:48:21.000000 Slame-1.5.2/Slame.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)        1 2024-04-29 14:48:21.000000 Slame-1.5.2/Slame.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)       19 2024-04-29 14:48:21.000000 Slame-1.5.2/Slame.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)        6 2024-04-29 14:48:21.000000 Slame-1.5.2/Slame.egg-info/top_level.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)       38 2024-04-29 14:48:21.162762 Slame-1.5.2/setup.cfg
+-rw-r--r--   0 dev       (1000) dev       (1000)     1253 2024-04-29 14:48:11.000000 Slame-1.5.2/setup.py
```

### Comparing `Slame-1.5.1/PKG-INFO` & `Slame-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Slame
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python module for serving a web server and more
 Home-page: https://github.com/zhrexx/Slame/
 Author: ZHRXXgroup
 Author-email: info@zhrxxgroup.com
 License: MIT License, see LICENSE file
 Download-URL: https://zhrxxgroup.com/slame/download.php?file=Slame-1.3.tar.gz
 Platform: UNKNOWN
```

### Comparing `Slame-1.5.1/README.md` & `Slame-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `Slame-1.5.1/Slame/slame.py` & `Slame-1.5.2/Slame/slame.py`

 * *Files identical despite different names*

### Comparing `Slame-1.5.1/Slame.egg-info/PKG-INFO` & `Slame-1.5.2/Slame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Slame
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python module for serving a web server and more
 Home-page: https://github.com/zhrexx/Slame/
 Author: ZHRXXgroup
 Author-email: info@zhrxxgroup.com
 License: MIT License, see LICENSE file
 Download-URL: https://zhrxxgroup.com/slame/download.php?file=Slame-1.3.tar.gz
 Platform: UNKNOWN
```

### Comparing `Slame-1.5.1/setup.py` & `Slame-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """
 :authors: ZHRXXgroup
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 ZHRXXgroup
 """
 
-version = '1.5.1'
+version = '1.5.2'
 
 long_description  = "Slame is an Python Module for serving a webserver and in 1.2 we added Plugins you can use your own plugins in Slame or you can download plugins from other Peoples at https://zhrxxgroup.com/slame/spm/. SLAME DOCS: https://zhrxxgroup.com/slame or https://github.com/zhrexx/Slame, OUR WEBSITE: https://zhrxxgroup.com"
 
 
 
 setup(
     name="Slame",
```

