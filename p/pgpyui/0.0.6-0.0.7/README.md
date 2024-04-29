# Comparing `tmp/pgpyui-0.0.6.tar.gz` & `tmp/pgpyui-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgpyui-0.0.6.tar", last modified: Sun Apr 28 13:06:37 2024, max compression
+gzip compressed data, was "pgpyui-0.0.7.tar", last modified: Sun Apr 28 15:39:16 2024, max compression
```

## Comparing `pgpyui-0.0.6.tar` & `pgpyui-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 13:06:37.004277 pgpyui-0.0.6/
--rw-rw-rw-   0        0        0     4214 2024-04-28 13:06:37.003276 pgpyui-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3636 2024-04-28 13:04:55.000000 pgpyui-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 13:06:36.996280 pgpyui-0.0.6/pgpyui/
--rw-rw-rw-   0        0        0      149 2024-04-28 11:37:14.000000 pgpyui-0.0.6/pgpyui/__init__.py
--rw-rw-rw-   0        0        0     2284 2024-04-25 14:17:42.000000 pgpyui-0.0.6/pgpyui/button.py
--rw-rw-rw-   0        0        0     2451 2024-04-28 11:31:24.000000 pgpyui-0.0.6/pgpyui/checkbox.py
--rw-rw-rw-   0        0        0     2608 2024-04-28 11:21:59.000000 pgpyui-0.0.6/pgpyui/slider.py
--rw-rw-rw-   0        0        0     6072 2024-04-28 11:21:52.000000 pgpyui-0.0.6/pgpyui/textarea.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:06:37.002275 pgpyui-0.0.6/pgpyui.egg-info/
--rw-rw-rw-   0        0        0     4214 2024-04-28 13:06:36.000000 pgpyui-0.0.6/pgpyui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-04-28 13:06:36.000000 pgpyui-0.0.6/pgpyui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 13:06:36.000000 pgpyui-0.0.6/pgpyui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-28 13:06:36.000000 pgpyui-0.0.6/pgpyui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-28 13:06:36.000000 pgpyui-0.0.6/pgpyui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 13:06:37.004277 pgpyui-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      822 2024-04-28 12:58:58.000000 pgpyui-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:39:16.097591 pgpyui-0.0.7/
+-rw-rw-rw-   0        0        0     4214 2024-04-28 15:39:16.097591 pgpyui-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3636 2024-04-28 15:38:52.000000 pgpyui-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 15:39:16.090592 pgpyui-0.0.7/pgpyui/
+-rw-rw-rw-   0        0        0      149 2024-04-28 11:37:14.000000 pgpyui-0.0.7/pgpyui/__init__.py
+-rw-rw-rw-   0        0        0     2284 2024-04-25 14:17:42.000000 pgpyui-0.0.7/pgpyui/button.py
+-rw-rw-rw-   0        0        0     2451 2024-04-28 11:31:24.000000 pgpyui-0.0.7/pgpyui/checkbox.py
+-rw-rw-rw-   0        0        0     2183 2024-04-28 12:59:30.000000 pgpyui-0.0.7/pgpyui/radio.py
+-rw-rw-rw-   0        0        0     2608 2024-04-28 11:21:59.000000 pgpyui-0.0.7/pgpyui/slider.py
+-rw-rw-rw-   0        0        0     6072 2024-04-28 11:21:52.000000 pgpyui-0.0.7/pgpyui/textarea.py
+drwxrwxrwx   0        0        0        0 2024-04-28 15:39:16.096591 pgpyui-0.0.7/pgpyui.egg-info/
+-rw-rw-rw-   0        0        0     4214 2024-04-28 15:39:15.000000 pgpyui-0.0.7/pgpyui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-04-28 15:39:16.000000 pgpyui-0.0.7/pgpyui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 15:39:15.000000 pgpyui-0.0.7/pgpyui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-28 15:39:15.000000 pgpyui-0.0.7/pgpyui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-28 15:39:15.000000 pgpyui-0.0.7/pgpyui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 15:39:16.098596 pgpyui-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      822 2024-04-28 15:38:45.000000 pgpyui-0.0.7/setup.py
```

### Comparing `pgpyui-0.0.6/PKG-INFO` & `pgpyui-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pgpyui
-Version: 0.0.6
+Version: 0.0.7
 Summary: The package is an add-on for Pygame to create a user interface on the screen.
 Home-page: https://pypi.org/project/pgpyui/
 Author: Memdved
 Author-email: mixail.vilyukov@icloud.com
 Project-URL: GitHub, https://github.com/Memdved
 Keywords: ui gui pgpyui pygame
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.25.1
 
-# pgpyui 0.0.6
+# pgpyui 0.0.7
 
 pgpyui is an add-on module for pygame to create a user interface.
 
 ## Installation
 
 ```
 pip install pgpyui
```

### Comparing `pgpyui-0.0.6/README.md` & `pgpyui-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pgpyui 0.0.6
+# pgpyui 0.0.7
 
 pgpyui is an add-on module for pygame to create a user interface.
 
 ## Installation
 
 ```
 pip install pgpyui
```

### Comparing `pgpyui-0.0.6/pgpyui/button.py` & `pgpyui-0.0.7/pgpyui/button.py`

 * *Files identical despite different names*

### Comparing `pgpyui-0.0.6/pgpyui/checkbox.py` & `pgpyui-0.0.7/pgpyui/checkbox.py`

 * *Files identical despite different names*

### Comparing `pgpyui-0.0.6/pgpyui/slider.py` & `pgpyui-0.0.7/pgpyui/slider.py`

 * *Files identical despite different names*

### Comparing `pgpyui-0.0.6/pgpyui/textarea.py` & `pgpyui-0.0.7/pgpyui/textarea.py`

 * *Files identical despite different names*

### Comparing `pgpyui-0.0.6/pgpyui.egg-info/PKG-INFO` & `pgpyui-0.0.7/pgpyui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pgpyui
-Version: 0.0.6
+Version: 0.0.7
 Summary: The package is an add-on for Pygame to create a user interface on the screen.
 Home-page: https://pypi.org/project/pgpyui/
 Author: Memdved
 Author-email: mixail.vilyukov@icloud.com
 Project-URL: GitHub, https://github.com/Memdved
 Keywords: ui gui pgpyui pygame
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.25.1
 
-# pgpyui 0.0.6
+# pgpyui 0.0.7
 
 pgpyui is an add-on module for pygame to create a user interface.
 
 ## Installation
 
 ```
 pip install pgpyui
```

### Comparing `pgpyui-0.0.6/setup.py` & `pgpyui-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='pgpyui',
-  version='0.0.6',
+  version='0.0.7',
   author='Memdved',
   author_email='mixail.vilyukov@icloud.com',
   description='The package is an add-on for Pygame to create a user interface on the screen.',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://pypi.org/project/pgpyui/',
   packages=find_packages(),
```

