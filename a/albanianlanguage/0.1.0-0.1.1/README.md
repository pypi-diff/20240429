# Comparing `tmp/albanianlanguage-0.1.0.tar.gz` & `tmp/albanianlanguage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albanianlanguage-0.1.0.tar", last modified: Mon Apr 29 20:41:16 2024, max compression
+gzip compressed data, was "albanianlanguage-0.1.1.tar", last modified: Mon Apr 29 20:58:53 2024, max compression
```

## Comparing `albanianlanguage-0.1.0.tar` & `albanianlanguage-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-04-29 20:41:16.421014 albanianlanguage-0.1.0/
--rw-r--r--   0 flori      (501) staff       (20)     1075 2024-04-29 20:36:09.000000 albanianlanguage-0.1.0/LICENSE.md
--rw-r--r--   0 flori      (501) staff       (20)     2423 2024-04-29 20:41:16.420824 albanianlanguage-0.1.0/PKG-INFO
--rw-r--r--   0 flori      (501) staff       (20)     2009 2024-04-29 20:37:10.000000 albanianlanguage-0.1.0/README.md
-drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-04-29 20:41:16.417182 albanianlanguage-0.1.0/albanianlanguage/
--rw-r--r--   0 flori      (501) staff       (20)       33 2024-04-29 19:58:25.000000 albanianlanguage-0.1.0/albanianlanguage/__init__.py
--rw-r--r--   0 flori      (501) staff       (20)     1831 2024-04-29 20:14:56.000000 albanianlanguage-0.1.0/albanianlanguage/words.py
-drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-04-29 20:41:16.420462 albanianlanguage-0.1.0/albanianlanguage.egg-info/
--rw-r--r--   0 flori      (501) staff       (20)     2423 2024-04-29 20:41:16.000000 albanianlanguage-0.1.0/albanianlanguage.egg-info/PKG-INFO
--rw-r--r--   0 flori      (501) staff       (20)      283 2024-04-29 20:41:16.000000 albanianlanguage-0.1.0/albanianlanguage.egg-info/SOURCES.txt
--rw-r--r--   0 flori      (501) staff       (20)        1 2024-04-29 20:41:16.000000 albanianlanguage-0.1.0/albanianlanguage.egg-info/dependency_links.txt
--rw-r--r--   0 flori      (501) staff       (20)        4 2024-04-29 20:41:16.000000 albanianlanguage-0.1.0/albanianlanguage.egg-info/requires.txt
--rw-r--r--   0 flori      (501) staff       (20)       17 2024-04-29 20:41:16.000000 albanianlanguage-0.1.0/albanianlanguage.egg-info/top_level.txt
--rw-r--r--   0 flori      (501) staff       (20)       38 2024-04-29 20:41:16.421074 albanianlanguage-0.1.0/setup.cfg
--rw-r--r--   0 flori      (501) staff       (20)      610 2024-04-29 20:10:51.000000 albanianlanguage-0.1.0/setup.py
+drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-04-29 20:58:53.732392 albanianlanguage-0.1.1/
+-rw-r--r--   0 flori      (501) staff       (20)     1075 2024-04-29 20:36:09.000000 albanianlanguage-0.1.1/LICENSE.md
+-rw-r--r--   0 flori      (501) staff       (20)     2423 2024-04-29 20:58:53.731834 albanianlanguage-0.1.1/PKG-INFO
+-rw-r--r--   0 flori      (501) staff       (20)     2009 2024-04-29 20:37:10.000000 albanianlanguage-0.1.1/README.md
+drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-04-29 20:58:53.713638 albanianlanguage-0.1.1/albanianlanguage/
+-rw-r--r--   0 flori      (501) staff       (20)       33 2024-04-29 19:58:25.000000 albanianlanguage-0.1.1/albanianlanguage/__init__.py
+-rw-r--r--   0 flori      (501) staff       (20)     1831 2024-04-29 20:14:56.000000 albanianlanguage-0.1.1/albanianlanguage/words.py
+drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-04-29 20:58:53.731227 albanianlanguage-0.1.1/albanianlanguage.egg-info/
+-rw-r--r--   0 flori      (501) staff       (20)     2423 2024-04-29 20:58:53.000000 albanianlanguage-0.1.1/albanianlanguage.egg-info/PKG-INFO
+-rw-r--r--   0 flori      (501) staff       (20)      244 2024-04-29 20:58:53.000000 albanianlanguage-0.1.1/albanianlanguage.egg-info/SOURCES.txt
+-rw-r--r--   0 flori      (501) staff       (20)        1 2024-04-29 20:58:53.000000 albanianlanguage-0.1.1/albanianlanguage.egg-info/dependency_links.txt
+-rw-r--r--   0 flori      (501) staff       (20)       17 2024-04-29 20:58:53.000000 albanianlanguage-0.1.1/albanianlanguage.egg-info/top_level.txt
+-rw-r--r--   0 flori      (501) staff       (20)       38 2024-04-29 20:58:53.732452 albanianlanguage-0.1.1/setup.cfg
+-rw-r--r--   0 flori      (501) staff       (20)      617 2024-04-29 20:58:12.000000 albanianlanguage-0.1.1/setup.py
```

### Comparing `albanianlanguage-0.1.0/LICENSE.md` & `albanianlanguage-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `albanianlanguage-0.1.0/PKG-INFO` & `albanianlanguage-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albanianlanguage
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package with a few functionalities for albanian language.
 Home-page: http://github.com/florijanqosja/albanianlanguage
 Author: Florijan Qosja
 Author-email: florijanqosja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `albanianlanguage-0.1.0/README.md` & `albanianlanguage-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `albanianlanguage-0.1.0/albanianlanguage/words.py` & `albanianlanguage-0.1.1/albanianlanguage/words.py`

 * *Files identical despite different names*

### Comparing `albanianlanguage-0.1.0/albanianlanguage.egg-info/PKG-INFO` & `albanianlanguage-0.1.1/albanianlanguage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albanianlanguage
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package with a few functionalities for albanian language.
 Home-page: http://github.com/florijanqosja/albanianlanguage
 Author: Florijan Qosja
 Author-email: florijanqosja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `albanianlanguage-0.1.0/setup.py` & `albanianlanguage-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='albanianlanguage',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
-        'csv',
+        # none so fas
     ],
     author='Florijan Qosja',
     author_email='florijanqosja@gmail.com',
     description='A package with a few functionalities for albanian language.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='http://github.com/florijanqosja/albanianlanguage',
```

