# Comparing `tmp/matMulti-0.0.3.tar.gz` & `tmp/matMulti-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matMulti-0.0.3.tar", last modified: Wed Apr 24 19:34:06 2024, max compression
+gzip compressed data, was "matMulti-0.0.4.tar", last modified: Mon Apr 29 15:09:10 2024, max compression
```

## Comparing `matMulti-0.0.3.tar` & `matMulti-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxr-x   0 sajal     (1000) sajal     (1000)        0 2024-04-24 19:34:06.145174 matMulti-0.0.3/
--rw-rw-r--   0 sajal     (1000) sajal     (1000)     1153 2024-04-24 18:33:02.000000 matMulti-0.0.3/LICENSE.txt
--rw-rw-r--   0 sajal     (1000) sajal     (1000)       44 2024-04-24 18:32:29.000000 matMulti-0.0.3/MANIFEST.in
--rw-rw-r--   0 sajal     (1000) sajal     (1000)     1247 2024-04-24 19:34:06.145174 matMulti-0.0.3/PKG-INFO
--rw-rw-r--   0 sajal     (1000) sajal     (1000)      628 2024-04-24 19:33:05.000000 matMulti-0.0.3/README.txt
-drwxrwxr-x   0 sajal     (1000) sajal     (1000)        0 2024-04-24 19:34:06.141174 matMulti-0.0.3/matMulti.egg-info/
--rw-rw-r--   0 sajal     (1000) sajal     (1000)     1247 2024-04-24 19:34:06.000000 matMulti-0.0.3/matMulti.egg-info/PKG-INFO
--rw-rw-r--   0 sajal     (1000) sajal     (1000)      171 2024-04-24 19:34:06.000000 matMulti-0.0.3/matMulti.egg-info/SOURCES.txt
--rw-rw-r--   0 sajal     (1000) sajal     (1000)        1 2024-04-24 19:34:06.000000 matMulti-0.0.3/matMulti.egg-info/dependency_links.txt
--rw-rw-r--   0 sajal     (1000) sajal     (1000)        1 2024-04-24 19:34:06.000000 matMulti-0.0.3/matMulti.egg-info/top_level.txt
--rw-rw-r--   0 sajal     (1000) sajal     (1000)       38 2024-04-24 19:34:06.145174 matMulti-0.0.3/setup.cfg
--rw-rw-r--   0 sajal     (1000) sajal     (1000)      778 2024-04-24 19:32:38.000000 matMulti-0.0.3/setup.py
+drwxrwxr-x   0 sajal     (1000) sajal     (1000)        0 2024-04-29 15:09:10.310914 matMulti-0.0.4/
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)     1153 2024-04-24 18:33:02.000000 matMulti-0.0.4/LICENSE.txt
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)       44 2024-04-24 18:32:29.000000 matMulti-0.0.4/MANIFEST.in
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)     1247 2024-04-29 15:09:10.310914 matMulti-0.0.4/PKG-INFO
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)      628 2024-04-24 19:33:05.000000 matMulti-0.0.4/README.txt
+drwxrwxr-x   0 sajal     (1000) sajal     (1000)        0 2024-04-29 15:09:10.310914 matMulti-0.0.4/matMulti.egg-info/
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)     1247 2024-04-29 15:09:09.000000 matMulti-0.0.4/matMulti.egg-info/PKG-INFO
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)      210 2024-04-29 15:09:10.000000 matMulti-0.0.4/matMulti.egg-info/SOURCES.txt
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)        1 2024-04-29 15:09:09.000000 matMulti-0.0.4/matMulti.egg-info/dependency_links.txt
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)        8 2024-04-29 15:09:09.000000 matMulti-0.0.4/matMulti.egg-info/top_level.txt
+drwxrwxr-x   0 sajal     (1000) sajal     (1000)        0 2024-04-29 15:09:10.310914 matMulti-0.0.4/product/
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)        0 2024-04-24 19:33:09.000000 matMulti-0.0.4/product/__init__.py
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)      109 2024-04-24 19:33:12.000000 matMulti-0.0.4/product/product.py
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)       38 2024-04-29 15:09:10.310914 matMulti-0.0.4/setup.cfg
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)      779 2024-04-29 15:05:41.000000 matMulti-0.0.4/setup.py
```

### Comparing `matMulti-0.0.3/LICENSE.txt` & `matMulti-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `matMulti-0.0.3/PKG-INFO` & `matMulti-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matMulti
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to multiply two matrix of any dimensions
 Home-page: https://github.com/SajalDasShovon/Own-Simple-Python-Package
 Author: Sajal Das Shovon
 Author-email: shovon030cse.kuet@gmail.com
 License: MIT
 Keywords: matrixMultiplier
 Platform: UNKNOWN
```

### Comparing `matMulti-0.0.3/README.txt` & `matMulti-0.0.4/README.txt`

 * *Files identical despite different names*

### Comparing `matMulti-0.0.3/matMulti.egg-info/PKG-INFO` & `matMulti-0.0.4/matMulti.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matMulti
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to multiply two matrix of any dimensions
 Home-page: https://github.com/SajalDasShovon/Own-Simple-Python-Package
 Author: Sajal Das Shovon
 Author-email: shovon030cse.kuet@gmail.com
 License: MIT
 Keywords: matrixMultiplier
 Platform: UNKNOWN
```

### Comparing `matMulti-0.0.3/setup.py` & `matMulti-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,20 +9,20 @@
   'Operating System :: OS Independent',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='matMulti',
-  version='0.0.3',
+  version='0.0.4',
   description='A package to multiply two matrix of any dimensions',
   long_description=open('README.txt').read(),
   long_description_content_type='text/plain',
   url='https://github.com/SajalDasShovon/Own-Simple-Python-Package',  
   author='Sajal Das Shovon',
   author_email='shovon030cse.kuet@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='matrixMultiplier', 
   packages=find_packages(),
   install_requires=[''] 
-)
+)
```

