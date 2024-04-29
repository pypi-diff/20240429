# Comparing `tmp/middleware-help-python-0.0.3.tar.gz` & `tmp/middleware-help-python-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "middleware-help-python-0.0.3.tar", last modified: Wed Apr 24 08:34:54 2024, max compression
+gzip compressed data, was "middleware-help-python-0.0.4.tar", last modified: Mon Apr 29 08:23:14 2024, max compression
```

## Comparing `middleware-help-python-0.0.3.tar` & `middleware-help-python-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 08:34:54.215968 middleware-help-python-0.0.3/
--rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      513 2024-04-24 08:34:54.213995 middleware-help-python-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 08:34:54.212993 middleware-help-python-0.0.3/middleware_help_python.egg-info/
--rw-rw-rw-   0        0        0      513 2024-04-24 08:34:54.000000 middleware-help-python-0.0.3/middleware_help_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2024-04-24 08:34:54.000000 middleware-help-python-0.0.3/middleware_help_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 08:34:54.000000 middleware-help-python-0.0.3/middleware_help_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-24 08:34:54.000000 middleware-help-python-0.0.3/middleware_help_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-24 08:34:54.000000 middleware-help-python-0.0.3/middleware_help_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 08:34:54.211002 middleware-help-python-0.0.3/middleware_helper/
--rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.0.3/middleware_helper/__init__.py
--rw-rw-rw-   0        0        0     3576 2024-04-24 08:34:08.000000 middleware-help-python-0.0.3/middleware_helper/mysql.py
--rw-rw-rw-   0        0        0     1036 2024-04-24 08:21:48.000000 middleware-help-python-0.0.3/middleware_helper/redis.py
--rw-rw-rw-   0        0        0       42 2024-04-24 08:34:54.216957 middleware-help-python-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1136 2024-04-24 08:34:41.000000 middleware-help-python-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:23:14.766522 middleware-help-python-0.0.4/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      513 2024-04-29 08:23:14.764526 middleware-help-python-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 08:23:14.763529 middleware-help-python-0.0.4/middleware_help_python.egg-info/
+-rw-rw-rw-   0        0        0      513 2024-04-29 08:23:14.000000 middleware-help-python-0.0.4/middleware_help_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2024-04-29 08:23:14.000000 middleware-help-python-0.0.4/middleware_help_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 08:23:14.000000 middleware-help-python-0.0.4/middleware_help_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-29 08:23:14.000000 middleware-help-python-0.0.4/middleware_help_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-29 08:23:14.000000 middleware-help-python-0.0.4/middleware_help_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 08:23:14.761542 middleware-help-python-0.0.4/middleware_helper/
+-rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.0.4/middleware_helper/__init__.py
+-rw-rw-rw-   0        0        0     3819 2024-04-29 08:22:08.000000 middleware-help-python-0.0.4/middleware_helper/mysql.py
+-rw-rw-rw-   0        0        0     2155 2024-04-29 08:20:12.000000 middleware-help-python-0.0.4/middleware_helper/network.py
+-rw-rw-rw-   0        0        0     1267 2024-04-29 08:21:12.000000 middleware-help-python-0.0.4/middleware_helper/redis.py
+-rw-rw-rw-   0        0        0       42 2024-04-29 08:23:14.766522 middleware-help-python-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1136 2024-04-29 03:59:33.000000 middleware-help-python-0.0.4/setup.py
```

### Comparing `middleware-help-python-0.0.3/LICENSE` & `middleware-help-python-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.3/PKG-INFO` & `middleware-help-python-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.0.3/middleware_help_python.egg-info/PKG-INFO` & `middleware-help-python-0.0.4/middleware_help_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.0.3/middleware_helper/mysql.py` & `middleware-help-python-0.0.4/middleware_helper/mysql.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,23 @@
 # Author:       mfkifhss2023
 # CreateDate:   2024/04/24
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from mysql.connector import connect
 from mysql.connector.cursor_cext import CMySQLCursor
+from middleware_helper.network import filter_system_port_list
 
 
 class Mysql(object):
 
     def __init__(self, **mysql_params_map):
+        port = mysql_params_map.get("port")
+        if isinstance(port, list):
+            mysql_params_map["port"] = filter_system_port_list(data_port=port, default_port=6379)
         self.conn = connect(
             host=mysql_params_map.get("host"),
             user=mysql_params_map.get("user"),
             port=mysql_params_map.get("port"),
             charset=mysql_params_map.get("charset"),
             password=mysql_params_map.get("password"),
             database=mysql_params_map.get("database")
```

### Comparing `middleware-help-python-0.0.3/setup.py` & `middleware-help-python-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='middleware-help-python',
-    version='0.0.3',
+    version='0.0.4',
     description='This is my middleware help package',
     long_description='This is my middleware help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/middleware-help-python',
     packages=find_packages(),
     install_requires=[
```

