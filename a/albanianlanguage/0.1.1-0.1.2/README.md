# Comparing `tmp/albanianlanguage-0.1.1.tar.gz` & `tmp/albanianlanguage-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albanianlanguage-0.1.1.tar", last modified: Mon Apr 29 20:58:53 2024, max compression
+gzip compressed data, was "albanianlanguage-0.1.2.tar", last modified: Mon Apr 29 21:05:18 2024, max compression
```

## Comparing `albanianlanguage-0.1.1.tar` & `albanianlanguage-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-04-29 20:58:53.732392 albanianlanguage-0.1.1/
--rw-r--r--   0 flori      (501) staff       (20)     1075 2024-04-29 20:36:09.000000 albanianlanguage-0.1.1/LICENSE.md
--rw-r--r--   0 flori      (501) staff       (20)     2423 2024-04-29 20:58:53.731834 albanianlanguage-0.1.1/PKG-INFO
--rw-r--r--   0 flori      (501) staff       (20)     2009 2024-04-29 20:37:10.000000 albanianlanguage-0.1.1/README.md
-drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-04-29 20:58:53.713638 albanianlanguage-0.1.1/albanianlanguage/
--rw-r--r--   0 flori      (501) staff       (20)       33 2024-04-29 19:58:25.000000 albanianlanguage-0.1.1/albanianlanguage/__init__.py
--rw-r--r--   0 flori      (501) staff       (20)     1831 2024-04-29 20:14:56.000000 albanianlanguage-0.1.1/albanianlanguage/words.py
-drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-04-29 20:58:53.731227 albanianlanguage-0.1.1/albanianlanguage.egg-info/
--rw-r--r--   0 flori      (501) staff       (20)     2423 2024-04-29 20:58:53.000000 albanianlanguage-0.1.1/albanianlanguage.egg-info/PKG-INFO
--rw-r--r--   0 flori      (501) staff       (20)      244 2024-04-29 20:58:53.000000 albanianlanguage-0.1.1/albanianlanguage.egg-info/SOURCES.txt
--rw-r--r--   0 flori      (501) staff       (20)        1 2024-04-29 20:58:53.000000 albanianlanguage-0.1.1/albanianlanguage.egg-info/dependency_links.txt
--rw-r--r--   0 flori      (501) staff       (20)       17 2024-04-29 20:58:53.000000 albanianlanguage-0.1.1/albanianlanguage.egg-info/top_level.txt
--rw-r--r--   0 flori      (501) staff       (20)       38 2024-04-29 20:58:53.732452 albanianlanguage-0.1.1/setup.cfg
--rw-r--r--   0 flori      (501) staff       (20)      617 2024-04-29 20:58:12.000000 albanianlanguage-0.1.1/setup.py
+drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-04-29 21:05:18.909413 albanianlanguage-0.1.2/
+-rw-r--r--   0 flori      (501) staff       (20)     1075 2024-04-29 20:36:09.000000 albanianlanguage-0.1.2/LICENSE.md
+-rw-r--r--   0 flori      (501) staff       (20)     2423 2024-04-29 21:05:18.908732 albanianlanguage-0.1.2/PKG-INFO
+-rw-r--r--   0 flori      (501) staff       (20)     2009 2024-04-29 20:37:10.000000 albanianlanguage-0.1.2/README.md
+drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-04-29 21:05:18.882640 albanianlanguage-0.1.2/albanianlanguage/
+-rw-r--r--   0 flori      (501) staff       (20)       33 2024-04-29 19:58:25.000000 albanianlanguage-0.1.2/albanianlanguage/__init__.py
+-rw-r--r--   0 flori      (501) staff       (20) 12203635 2024-04-29 20:10:19.000000 albanianlanguage-0.1.2/albanianlanguage/words.csv
+-rw-r--r--   0 flori      (501) staff       (20)     1831 2024-04-29 20:14:56.000000 albanianlanguage-0.1.2/albanianlanguage/words.py
+drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-04-29 21:05:18.907836 albanianlanguage-0.1.2/albanianlanguage.egg-info/
+-rw-r--r--   0 flori      (501) staff       (20)     2423 2024-04-29 21:05:18.000000 albanianlanguage-0.1.2/albanianlanguage.egg-info/PKG-INFO
+-rw-r--r--   0 flori      (501) staff       (20)      271 2024-04-29 21:05:18.000000 albanianlanguage-0.1.2/albanianlanguage.egg-info/SOURCES.txt
+-rw-r--r--   0 flori      (501) staff       (20)        1 2024-04-29 21:05:18.000000 albanianlanguage-0.1.2/albanianlanguage.egg-info/dependency_links.txt
+-rw-r--r--   0 flori      (501) staff       (20)       17 2024-04-29 21:05:18.000000 albanianlanguage-0.1.2/albanianlanguage.egg-info/top_level.txt
+-rw-r--r--   0 flori      (501) staff       (20)       38 2024-04-29 21:05:18.909489 albanianlanguage-0.1.2/setup.cfg
+-rw-r--r--   0 flori      (501) staff       (20)      671 2024-04-29 21:05:12.000000 albanianlanguage-0.1.2/setup.py
```

### Comparing `albanianlanguage-0.1.1/LICENSE.md` & `albanianlanguage-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `albanianlanguage-0.1.1/PKG-INFO` & `albanianlanguage-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albanianlanguage
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package with a few functionalities for albanian language.
 Home-page: http://github.com/florijanqosja/albanianlanguage
 Author: Florijan Qosja
 Author-email: florijanqosja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `albanianlanguage-0.1.1/README.md` & `albanianlanguage-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `albanianlanguage-0.1.1/albanianlanguage/words.py` & `albanianlanguage-0.1.2/albanianlanguage/words.py`

 * *Files identical despite different names*

### Comparing `albanianlanguage-0.1.1/albanianlanguage.egg-info/PKG-INFO` & `albanianlanguage-0.1.2/albanianlanguage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albanianlanguage
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package with a few functionalities for albanian language.
 Home-page: http://github.com/florijanqosja/albanianlanguage
 Author: Florijan Qosja
 Author-email: florijanqosja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `albanianlanguage-0.1.1/setup.py` & `albanianlanguage-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='albanianlanguage',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         # none so fas
     ],
     author='Florijan Qosja',
+    package_data={'albanianlanguage': ['words.csv']},
     author_email='florijanqosja@gmail.com',
     description='A package with a few functionalities for albanian language.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='http://github.com/florijanqosja/albanianlanguage',
     classifiers=[
         'Programming Language :: Python :: 3',
```

