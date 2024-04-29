# Comparing `tmp/rlanutils-0.1.3.tar.gz` & `tmp/rlanutils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlanutils-0.1.3.tar", last modified: Sun Apr 28 08:49:56 2024, max compression
+gzip compressed data, was "rlanutils-0.1.4.tar", last modified: Sun Apr 28 13:18:59 2024, max compression
```

## Comparing `rlanutils-0.1.3.tar` & `rlanutils-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 08:49:56.869054 rlanutils-0.1.3/
--rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-28 08:49:56.868881 rlanutils-0.1.3/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)       78 2024-04-28 07:35:44.000000 rlanutils-0.1.3/README.md
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 08:49:56.864974 rlanutils-0.1.3/rlanutils/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-28 06:25:11.000000 rlanutils-0.1.3/rlanutils/__init__.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 08:49:56.866033 rlanutils-0.1.3/rlanutils/cv/
--rw-r--r--   0 rlan       (501) staff       (20)      315 2024-04-28 08:49:41.000000 rlanutils-0.1.3/rlanutils/cv/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     1475 2024-04-28 07:13:43.000000 rlanutils-0.1.3/rlanutils/cv/geometry.py
--rw-r--r--   0 rlan       (501) staff       (20)     2900 2024-04-28 08:49:32.000000 rlanutils-0.1.3/rlanutils/cv/graphics.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 08:49:56.866482 rlanutils-0.1.3/rlanutils/data_structure/
--rw-r--r--   0 rlan       (501) staff       (20)       82 2024-04-28 07:15:07.000000 rlanutils-0.1.3/rlanutils/data_structure/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)      646 2024-04-28 07:15:05.000000 rlanutils-0.1.3/rlanutils/data_structure/set.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 08:49:56.868209 rlanutils-0.1.3/rlanutils/io/
--rw-r--r--   0 rlan       (501) staff       (20)      569 2024-04-28 07:17:32.000000 rlanutils-0.1.3/rlanutils/io/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     1487 2024-04-28 07:19:30.000000 rlanutils-0.1.3/rlanutils/io/fs.py
--rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-04-28 07:16:44.000000 rlanutils-0.1.3/rlanutils/io/indices.py
--rw-r--r--   0 rlan       (501) staff       (20)      682 2024-04-28 07:16:21.000000 rlanutils-0.1.3/rlanutils/io/network.py
--rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-04-28 07:16:14.000000 rlanutils-0.1.3/rlanutils/io/parallelism.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 08:49:56.868543 rlanutils-0.1.3/rlanutils/plot/
--rw-r--r--   0 rlan       (501) staff       (20)      118 2024-04-28 07:15:29.000000 rlanutils-0.1.3/rlanutils/plot/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-04-28 07:17:37.000000 rlanutils-0.1.3/rlanutils/plot/color.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 08:49:56.865533 rlanutils-0.1.3/rlanutils.egg-info/
--rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-28 08:49:56.000000 rlanutils-0.1.3/rlanutils.egg-info/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)      519 2024-04-28 08:49:56.000000 rlanutils-0.1.3/rlanutils.egg-info/SOURCES.txt
--rw-r--r--   0 rlan       (501) staff       (20)        1 2024-04-28 08:49:56.000000 rlanutils-0.1.3/rlanutils.egg-info/dependency_links.txt
--rw-r--r--   0 rlan       (501) staff       (20)       35 2024-04-28 08:49:56.000000 rlanutils-0.1.3/rlanutils.egg-info/requires.txt
--rw-r--r--   0 rlan       (501) staff       (20)       10 2024-04-28 08:49:56.000000 rlanutils-0.1.3/rlanutils.egg-info/top_level.txt
--rw-r--r--   0 rlan       (501) staff       (20)       38 2024-04-28 08:49:56.869104 rlanutils-0.1.3/setup.cfg
--rw-r--r--   0 rlan       (501) staff       (20)      538 2024-04-28 08:49:52.000000 rlanutils-0.1.3/setup.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 13:18:59.674444 rlanutils-0.1.4/
+-rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-28 13:18:59.674303 rlanutils-0.1.4/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)       78 2024-04-28 07:35:44.000000 rlanutils-0.1.4/README.md
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 13:18:59.670235 rlanutils-0.1.4/rlanutils/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-04-28 06:25:11.000000 rlanutils-0.1.4/rlanutils/__init__.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 13:18:59.671403 rlanutils-0.1.4/rlanutils/cv/
+-rw-r--r--   0 rlan       (501) staff       (20)      315 2024-04-28 08:49:41.000000 rlanutils-0.1.4/rlanutils/cv/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     3423 2024-04-28 13:11:21.000000 rlanutils-0.1.4/rlanutils/cv/geometry.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2900 2024-04-28 08:49:32.000000 rlanutils-0.1.4/rlanutils/cv/graphics.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 13:18:59.671841 rlanutils-0.1.4/rlanutils/data_structure/
+-rw-r--r--   0 rlan       (501) staff       (20)       82 2024-04-28 07:15:07.000000 rlanutils-0.1.4/rlanutils/data_structure/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)      646 2024-04-28 07:15:05.000000 rlanutils-0.1.4/rlanutils/data_structure/set.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 13:18:59.673533 rlanutils-0.1.4/rlanutils/io/
+-rw-r--r--   0 rlan       (501) staff       (20)      569 2024-04-28 07:17:32.000000 rlanutils-0.1.4/rlanutils/io/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1487 2024-04-28 07:19:30.000000 rlanutils-0.1.4/rlanutils/io/fs.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-04-28 07:16:44.000000 rlanutils-0.1.4/rlanutils/io/indices.py
+-rw-r--r--   0 rlan       (501) staff       (20)      682 2024-04-28 07:16:21.000000 rlanutils-0.1.4/rlanutils/io/network.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-04-28 07:16:14.000000 rlanutils-0.1.4/rlanutils/io/parallelism.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 13:18:59.673916 rlanutils-0.1.4/rlanutils/plot/
+-rw-r--r--   0 rlan       (501) staff       (20)      118 2024-04-28 07:15:29.000000 rlanutils-0.1.4/rlanutils/plot/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-04-28 07:17:37.000000 rlanutils-0.1.4/rlanutils/plot/color.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-04-28 13:18:59.670787 rlanutils-0.1.4/rlanutils.egg-info/
+-rw-r--r--   0 rlan       (501) staff       (20)      343 2024-04-28 13:18:59.000000 rlanutils-0.1.4/rlanutils.egg-info/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)      519 2024-04-28 13:18:59.000000 rlanutils-0.1.4/rlanutils.egg-info/SOURCES.txt
+-rw-r--r--   0 rlan       (501) staff       (20)        1 2024-04-28 13:18:59.000000 rlanutils-0.1.4/rlanutils.egg-info/dependency_links.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       35 2024-04-28 13:18:59.000000 rlanutils-0.1.4/rlanutils.egg-info/requires.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       10 2024-04-28 13:18:59.000000 rlanutils-0.1.4/rlanutils.egg-info/top_level.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       38 2024-04-28 13:18:59.674493 rlanutils-0.1.4/setup.cfg
+-rw-r--r--   0 rlan       (501) staff       (20)      538 2024-04-28 09:49:59.000000 rlanutils-0.1.4/setup.py
```

### Comparing `rlanutils-0.1.3/rlanutils/cv/graphics.py` & `rlanutils-0.1.4/rlanutils/cv/graphics.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.3/rlanutils/data_structure/set.py` & `rlanutils-0.1.4/rlanutils/data_structure/set.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.3/rlanutils/io/__init__.py` & `rlanutils-0.1.4/rlanutils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.3/rlanutils/io/fs.py` & `rlanutils-0.1.4/rlanutils/io/fs.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.3/rlanutils/io/indices.py` & `rlanutils-0.1.4/rlanutils/io/indices.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.3/rlanutils/io/network.py` & `rlanutils-0.1.4/rlanutils/io/network.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.3/rlanutils/io/parallelism.py` & `rlanutils-0.1.4/rlanutils/io/parallelism.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.3/rlanutils/plot/color.py` & `rlanutils-0.1.4/rlanutils/plot/color.py`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.3/rlanutils.egg-info/SOURCES.txt` & `rlanutils-0.1.4/rlanutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rlanutils-0.1.3/setup.py` & `rlanutils-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='rlanutils',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     description='A handy tool that make your day to day programming much easier. ',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='brianlan',
     author_email='brianlanbo@gmail.com',
     url='https://gitlab.com/rlan/rlanutils',
```

