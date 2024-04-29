# Comparing `tmp/middleware-help-python-0.0.4.tar.gz` & `tmp/middleware-help-python-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "middleware-help-python-0.0.4.tar", last modified: Mon Apr 29 08:23:14 2024, max compression
+gzip compressed data, was "middleware-help-python-0.0.5.tar", last modified: Mon Apr 29 08:34:05 2024, max compression
```

## Comparing `middleware-help-python-0.0.4.tar` & `middleware-help-python-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 08:23:14.766522 middleware-help-python-0.0.4/
--rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      513 2024-04-29 08:23:14.764526 middleware-help-python-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 08:23:14.763529 middleware-help-python-0.0.4/middleware_help_python.egg-info/
--rw-rw-rw-   0        0        0      513 2024-04-29 08:23:14.000000 middleware-help-python-0.0.4/middleware_help_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2024-04-29 08:23:14.000000 middleware-help-python-0.0.4/middleware_help_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 08:23:14.000000 middleware-help-python-0.0.4/middleware_help_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-29 08:23:14.000000 middleware-help-python-0.0.4/middleware_help_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-29 08:23:14.000000 middleware-help-python-0.0.4/middleware_help_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 08:23:14.761542 middleware-help-python-0.0.4/middleware_helper/
--rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.0.4/middleware_helper/__init__.py
--rw-rw-rw-   0        0        0     3819 2024-04-29 08:22:08.000000 middleware-help-python-0.0.4/middleware_helper/mysql.py
--rw-rw-rw-   0        0        0     2155 2024-04-29 08:20:12.000000 middleware-help-python-0.0.4/middleware_helper/network.py
--rw-rw-rw-   0        0        0     1267 2024-04-29 08:21:12.000000 middleware-help-python-0.0.4/middleware_helper/redis.py
--rw-rw-rw-   0        0        0       42 2024-04-29 08:23:14.766522 middleware-help-python-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1136 2024-04-29 03:59:33.000000 middleware-help-python-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:34:05.407900 middleware-help-python-0.0.5/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      513 2024-04-29 08:34:05.405907 middleware-help-python-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 08:34:05.403912 middleware-help-python-0.0.5/middleware_help_python.egg-info/
+-rw-rw-rw-   0        0        0      513 2024-04-29 08:34:05.000000 middleware-help-python-0.0.5/middleware_help_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2024-04-29 08:34:05.000000 middleware-help-python-0.0.5/middleware_help_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 08:34:05.000000 middleware-help-python-0.0.5/middleware_help_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-29 08:34:05.000000 middleware-help-python-0.0.5/middleware_help_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-29 08:34:05.000000 middleware-help-python-0.0.5/middleware_help_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 08:34:05.401917 middleware-help-python-0.0.5/middleware_helper/
+-rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.0.5/middleware_helper/__init__.py
+-rw-rw-rw-   0        0        0     3819 2024-04-29 08:33:44.000000 middleware-help-python-0.0.5/middleware_helper/mysql.py
+-rw-rw-rw-   0        0        0     2155 2024-04-29 08:20:12.000000 middleware-help-python-0.0.5/middleware_helper/network.py
+-rw-rw-rw-   0        0        0     1267 2024-04-29 08:21:12.000000 middleware-help-python-0.0.5/middleware_helper/redis.py
+-rw-rw-rw-   0        0        0       42 2024-04-29 08:34:05.407900 middleware-help-python-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1136 2024-04-29 08:34:01.000000 middleware-help-python-0.0.5/setup.py
```

### Comparing `middleware-help-python-0.0.4/LICENSE` & `middleware-help-python-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.4/PKG-INFO` & `middleware-help-python-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.0.4/middleware_help_python.egg-info/PKG-INFO` & `middleware-help-python-0.0.5/middleware_help_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.0.4/middleware_helper/mysql.py` & `middleware-help-python-0.0.5/middleware_helper/mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class Mysql(object):
 
     def __init__(self, **mysql_params_map):
         port = mysql_params_map.get("port")
         if isinstance(port, list):
-            mysql_params_map["port"] = filter_system_port_list(data_port=port, default_port=6379)
+            mysql_params_map["port"] = filter_system_port_list(data_port=port, default_port=3306)
         self.conn = connect(
             host=mysql_params_map.get("host"),
             user=mysql_params_map.get("user"),
             port=mysql_params_map.get("port"),
             charset=mysql_params_map.get("charset"),
             password=mysql_params_map.get("password"),
             database=mysql_params_map.get("database")
```

### Comparing `middleware-help-python-0.0.4/middleware_helper/network.py` & `middleware-help-python-0.0.5/middleware_helper/network.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.4/middleware_helper/redis.py` & `middleware-help-python-0.0.5/middleware_helper/redis.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.4/setup.py` & `middleware-help-python-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='middleware-help-python',
-    version='0.0.4',
+    version='0.0.5',
     description='This is my middleware help package',
     long_description='This is my middleware help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/middleware-help-python',
     packages=find_packages(),
     install_requires=[
```

