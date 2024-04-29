# Comparing `tmp/rlanutils-0.1.6.tar.gz` & `tmp/rlanutils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlanutils-0.1.6.tar", last modified: Mon Apr 29 03:23:09 2024, max compression
+gzip compressed data, was "rlanutils-0.1.7.tar", last modified: Mon Apr 29 03:31:56 2024, max compression
```

## Comparing `rlanutils-0.1.6.tar` & `rlanutils-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 03:23:09.850196 rlanutils-0.1.6/
--rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-29 03:23:09.850074 rlanutils-0.1.6/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)       78 2024-04-28 07:35:44.000000 rlanutils-0.1.6/README.md
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 03:23:09.846192 rlanutils-0.1.6/rlanutils/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-28 06:25:11.000000 rlanutils-0.1.6/rlanutils/__init__.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 03:23:09.847278 rlanutils-0.1.6/rlanutils/cv/
--rw-r--r--   0 rlan       (501) staff       (20)      315 2024-04-28 08:49:41.000000 rlanutils-0.1.6/rlanutils/cv/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     3430 2024-04-29 01:45:40.000000 rlanutils-0.1.6/rlanutils/cv/geometry.py
--rw-r--r--   0 rlan       (501) staff       (20)     2900 2024-04-28 08:49:32.000000 rlanutils-0.1.6/rlanutils/cv/graphics.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 03:23:09.847764 rlanutils-0.1.6/rlanutils/data_structure/
--rw-r--r--   0 rlan       (501) staff       (20)       82 2024-04-28 07:15:07.000000 rlanutils-0.1.6/rlanutils/data_structure/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)      646 2024-04-28 07:15:05.000000 rlanutils-0.1.6/rlanutils/data_structure/set.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 03:23:09.849334 rlanutils-0.1.6/rlanutils/io/
--rw-r--r--   0 rlan       (501) staff       (20)      624 2024-04-29 03:14:17.000000 rlanutils-0.1.6/rlanutils/io/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)      671 2024-04-29 03:19:35.000000 rlanutils-0.1.6/rlanutils/io/args.py
--rw-r--r--   0 rlan       (501) staff       (20)     1487 2024-04-28 07:19:30.000000 rlanutils-0.1.6/rlanutils/io/fs.py
--rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-04-28 07:16:44.000000 rlanutils-0.1.6/rlanutils/io/indices.py
--rw-r--r--   0 rlan       (501) staff       (20)      682 2024-04-28 07:16:21.000000 rlanutils-0.1.6/rlanutils/io/network.py
--rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-04-28 07:16:14.000000 rlanutils-0.1.6/rlanutils/io/parallelism.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 03:23:09.849713 rlanutils-0.1.6/rlanutils/plot/
--rw-r--r--   0 rlan       (501) staff       (20)      118 2024-04-28 07:15:29.000000 rlanutils-0.1.6/rlanutils/plot/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-04-28 07:17:37.000000 rlanutils-0.1.6/rlanutils/plot/color.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 03:23:09.846715 rlanutils-0.1.6/rlanutils.egg-info/
--rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-29 03:23:09.000000 rlanutils-0.1.6/rlanutils.egg-info/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)      540 2024-04-29 03:23:09.000000 rlanutils-0.1.6/rlanutils.egg-info/SOURCES.txt
--rw-r--r--   0 rlan       (501) staff       (20)        1 2024-04-29 03:23:09.000000 rlanutils-0.1.6/rlanutils.egg-info/dependency_links.txt
--rw-r--r--   0 rlan       (501) staff       (20)       35 2024-04-29 03:23:09.000000 rlanutils-0.1.6/rlanutils.egg-info/requires.txt
--rw-r--r--   0 rlan       (501) staff       (20)       10 2024-04-29 03:23:09.000000 rlanutils-0.1.6/rlanutils.egg-info/top_level.txt
--rw-r--r--   0 rlan       (501) staff       (20)       38 2024-04-29 03:23:09.850234 rlanutils-0.1.6/setup.cfg
--rw-r--r--   0 rlan       (501) staff       (20)      538 2024-04-29 03:22:48.000000 rlanutils-0.1.6/setup.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 03:31:56.612243 rlanutils-0.1.7/
+-rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-29 03:31:56.612115 rlanutils-0.1.7/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)       78 2024-04-28 07:35:44.000000 rlanutils-0.1.7/README.md
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 03:31:56.608530 rlanutils-0.1.7/rlanutils/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-28 06:25:11.000000 rlanutils-0.1.7/rlanutils/__init__.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 03:31:56.609512 rlanutils-0.1.7/rlanutils/cv/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-29 03:30:45.000000 rlanutils-0.1.7/rlanutils/cv/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     3430 2024-04-29 01:45:40.000000 rlanutils-0.1.7/rlanutils/cv/geometry.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2900 2024-04-28 08:49:32.000000 rlanutils-0.1.7/rlanutils/cv/graphics.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 03:31:56.609833 rlanutils-0.1.7/rlanutils/data_structure/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-29 03:31:00.000000 rlanutils-0.1.7/rlanutils/data_structure/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)      646 2024-04-28 07:15:05.000000 rlanutils-0.1.7/rlanutils/data_structure/set.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 03:31:56.611543 rlanutils-0.1.7/rlanutils/io/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-29 03:30:50.000000 rlanutils-0.1.7/rlanutils/io/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)      671 2024-04-29 03:19:35.000000 rlanutils-0.1.7/rlanutils/io/args.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1487 2024-04-28 07:19:30.000000 rlanutils-0.1.7/rlanutils/io/fs.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-04-28 07:16:44.000000 rlanutils-0.1.7/rlanutils/io/indices.py
+-rw-r--r--   0 rlan       (501) staff       (20)      682 2024-04-28 07:16:21.000000 rlanutils-0.1.7/rlanutils/io/network.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-04-28 07:16:14.000000 rlanutils-0.1.7/rlanutils/io/parallelism.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 03:31:56.611823 rlanutils-0.1.7/rlanutils/plot/
+-rw-r--r--   0 rlan       (501) staff       (20)      118 2024-04-28 07:15:29.000000 rlanutils-0.1.7/rlanutils/plot/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-04-28 07:17:37.000000 rlanutils-0.1.7/rlanutils/plot/color.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-29 03:31:56.609053 rlanutils-0.1.7/rlanutils.egg-info/
+-rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-29 03:31:56.000000 rlanutils-0.1.7/rlanutils.egg-info/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)      540 2024-04-29 03:31:56.000000 rlanutils-0.1.7/rlanutils.egg-info/SOURCES.txt
+-rw-r--r--   0 rlan       (501) staff       (20)        1 2024-04-29 03:31:56.000000 rlanutils-0.1.7/rlanutils.egg-info/dependency_links.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       35 2024-04-29 03:31:56.000000 rlanutils-0.1.7/rlanutils.egg-info/requires.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       10 2024-04-29 03:31:56.000000 rlanutils-0.1.7/rlanutils.egg-info/top_level.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       38 2024-04-29 03:31:56.612315 rlanutils-0.1.7/setup.cfg
+-rw-r--r--   0 rlan       (501) staff       (20)      538 2024-04-29 03:31:39.000000 rlanutils-0.1.7/setup.py
```

### Comparing `rlanutils-0.1.6/rlanutils/cv/geometry.py` & `rlanutils-0.1.7/rlanutils/cv/geometry.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.6/rlanutils/cv/graphics.py` & `rlanutils-0.1.7/rlanutils/cv/graphics.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.6/rlanutils/data_structure/set.py` & `rlanutils-0.1.7/rlanutils/data_structure/set.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.6/rlanutils/io/args.py` & `rlanutils-0.1.7/rlanutils/io/args.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.6/rlanutils/io/fs.py` & `rlanutils-0.1.7/rlanutils/io/fs.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.6/rlanutils/io/indices.py` & `rlanutils-0.1.7/rlanutils/io/indices.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.6/rlanutils/io/network.py` & `rlanutils-0.1.7/rlanutils/io/network.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.6/rlanutils/io/parallelism.py` & `rlanutils-0.1.7/rlanutils/io/parallelism.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.6/rlanutils/plot/color.py` & `rlanutils-0.1.7/rlanutils/plot/color.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.6/rlanutils.egg-info/SOURCES.txt` & `rlanutils-0.1.7/rlanutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.6/setup.py` & `rlanutils-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='rlanutils',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
     description='A handy tool that make your day to day programming much easier. ',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='brianlan',
     author_email='brianlanbo@gmail.com',
     url='https://gitlab.com/rlan/rlanutils',
```

