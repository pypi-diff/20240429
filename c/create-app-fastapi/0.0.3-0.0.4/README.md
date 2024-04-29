# Comparing `tmp/create-app-fastapi-0.0.3.tar.gz` & `tmp/create-app-fastapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create-app-fastapi-0.0.3.tar", last modified: Sat Apr 27 10:33:11 2024, max compression
+gzip compressed data, was "create-app-fastapi-0.0.4.tar", last modified: Mon Apr 29 12:17:13 2024, max compression
```

## Comparing `create-app-fastapi-0.0.3.tar` & `create-app-fastapi-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:33:11.122189 create-app-fastapi-0.0.3/
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      469 2024-04-27 10:33:11.122189 create-app-fastapi-0.0.3/PKG-INFO
-drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:33:11.122189 create-app-fastapi-0.0.3/create_app_fastapi.egg-info/
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      469 2024-04-27 10:33:11.000000 create-app-fastapi-0.0.3/create_app_fastapi.egg-info/PKG-INFO
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      296 2024-04-27 10:33:11.000000 create-app-fastapi-0.0.3/create_app_fastapi.egg-info/SOURCES.txt
--rw-rw-r--   0 bosco     (1000) bosco     (1000)        1 2024-04-27 10:33:11.000000 create-app-fastapi-0.0.3/create_app_fastapi.egg-info/dependency_links.txt
--rw-rw-r--   0 bosco     (1000) bosco     (1000)       65 2024-04-27 10:33:11.000000 create-app-fastapi-0.0.3/create_app_fastapi.egg-info/entry_points.txt
--rw-rw-r--   0 bosco     (1000) bosco     (1000)       15 2024-04-27 10:33:11.000000 create-app-fastapi-0.0.3/create_app_fastapi.egg-info/top_level.txt
-drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:33:11.122189 create-app-fastapi-0.0.3/projectfastapi/
--rw-rw-r--   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:16:31.000000 create-app-fastapi-0.0.3/projectfastapi/__init__.py
--rw-rw-r--   0 bosco     (1000) bosco     (1000)     3580 2024-04-27 10:28:48.000000 create-app-fastapi-0.0.3/projectfastapi/main.py
--rw-rw-r--   0 bosco     (1000) bosco     (1000)     2202 2024-04-26 13:06:58.000000 create-app-fastapi-0.0.3/projectfastapi/source.py
--rw-rw-r--   0 bosco     (1000) bosco     (1000)       38 2024-04-27 10:33:11.122189 create-app-fastapi-0.0.3/setup.cfg
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      673 2024-04-27 10:30:09.000000 create-app-fastapi-0.0.3/setup.py
+drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-04-29 12:17:13.268347 create-app-fastapi-0.0.4/
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)      599 2024-04-29 12:17:13.268347 create-app-fastapi-0.0.4/PKG-INFO
+drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-04-29 12:17:13.268347 create-app-fastapi-0.0.4/create_app_fastapi.egg-info/
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)      599 2024-04-29 12:17:13.000000 create-app-fastapi-0.0.4/create_app_fastapi.egg-info/PKG-INFO
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)      296 2024-04-29 12:17:13.000000 create-app-fastapi-0.0.4/create_app_fastapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)        1 2024-04-29 12:17:13.000000 create-app-fastapi-0.0.4/create_app_fastapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)       65 2024-04-29 12:17:13.000000 create-app-fastapi-0.0.4/create_app_fastapi.egg-info/entry_points.txt
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)       15 2024-04-29 12:17:13.000000 create-app-fastapi-0.0.4/create_app_fastapi.egg-info/top_level.txt
+drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-04-29 12:17:13.268347 create-app-fastapi-0.0.4/projectfastapi/
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:16:31.000000 create-app-fastapi-0.0.4/projectfastapi/__init__.py
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     3973 2024-04-29 12:17:04.000000 create-app-fastapi-0.0.4/projectfastapi/main.py
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     2202 2024-04-26 13:06:58.000000 create-app-fastapi-0.0.4/projectfastapi/source.py
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)       38 2024-04-29 12:17:13.268347 create-app-fastapi-0.0.4/setup.cfg
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)      807 2024-04-29 12:17:00.000000 create-app-fastapi-0.0.4/setup.py
```

### Comparing `create-app-fastapi-0.0.3/projectfastapi/main.py` & `create-app-fastapi-0.0.4/projectfastapi/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-import os, platform, sys, subprocess, threading, time
+import os, platform, sys, subprocess, threading, time, argparse
 from .source import getFileData
 
 def main():
 
+    parser = argparse.ArgumentParser(prog ='create-app-fastapi', description="Create fastapi project") 
+    parser.add_argument('name', metavar ='NAME', type = str, help ='create a project in this name')
+    parser.add_argument('-v','--version',action='version',
+                    version='%(prog)s 0.0.4', help ="show program's version number and exit")
+    args = parser.parse_args()
+
     curdir= os.getcwd()
     platformOS= platform.system()
     threadStop= False
 
     # terminal color code
     RED = "\033[31m"
     GREEN = "\033[32m"
     RESET = "\033[0m"
 
     # Inputs
-    name= input("Project name: ")
+    name= args.name
     virENV= input("Virtual environment name (default 'venv'): ")
     virENV= virENV if virENV else 'venv'
 
     # get file data
     fileData= getFileData(name, virENV)
 
     # create folders and files
@@ -104,8 +110,10 @@
 
     Note: activate virtual environment before run source {GREEN}main.py{RESET}
     {GREEN}Have a nice day! {RESET}
     """)
 
     openvs= input("Open project in VS Code? (y/n): ")
     if openvs.lower() == 'y':
-        run("code .")
+        run("code .")
+
+main()
```

### Comparing `create-app-fastapi-0.0.3/projectfastapi/source.py` & `create-app-fastapi-0.0.4/projectfastapi/source.py`

 * *Files identical despite different names*

### Comparing `create-app-fastapi-0.0.3/setup.py` & `create-app-fastapi-0.0.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from setuptools import setup, find_packages
 
 setup( 
 	name="create-app-fastapi", 
-	version="0.0.3", 
+	version="0.0.4", 
 	author="Ravishnu", 
 	author_email="ravishnu60@gmail.com", 
 	packages=find_packages(), 
 	description="Package to create fastapi project", 
-	long_description="A package used to create fastAPI project structure with virtual environment and dependencies.", 
+	long_description="""A package used to create fastAPI project structure with virtual environment and dependencies.
+    Once you install this package use below command to create fastapi project,
+    
+    create-app-fastapi project-name
+    
+    """, 
 	long_description_content_type="text/markdown", 
 	python_requires='>=3.9', 
 	install_requires=[],
 	entry_points ={ 
 		'console_scripts': [ 
 			'create-app-fastapi=projectfastapi.main:main'
 		]
```

