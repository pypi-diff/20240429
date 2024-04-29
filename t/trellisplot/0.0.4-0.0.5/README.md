# Comparing `tmp/trellisplot-0.0.4.tar.gz` & `tmp/trellisplot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trellisplot-0.0.4.tar", last modified: Mon Apr 29 18:30:19 2024, max compression
+gzip compressed data, was "trellisplot-0.0.5.tar", last modified: Mon Apr 29 18:40:05 2024, max compression
```

## Comparing `trellisplot-0.0.4.tar` & `trellisplot-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 18:30:19.857569 trellisplot-0.0.4/
--rw-rw-rw-   0        0        0      604 2024-04-29 18:30:19.854958 trellisplot-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-29 18:30:19.859014 trellisplot-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      888 2024-04-29 18:30:12.000000 trellisplot-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 18:30:19.828690 trellisplot-0.0.4/trellisplot/
--rw-rw-rw-   0        0        0       22 2024-01-09 20:12:41.000000 trellisplot-0.0.4/trellisplot/__init__.py
--rw-rw-rw-   0        0        0    13677 2024-04-29 17:57:01.000000 trellisplot-0.0.4/trellisplot/plot.py
--rw-rw-rw-   0        0        0     9178 2024-04-29 16:38:40.000000 trellisplot-0.0.4/trellisplot/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 18:30:19.852432 trellisplot-0.0.4/trellisplot.egg-info/
--rw-rw-rw-   0        0        0      604 2024-04-29 18:30:17.000000 trellisplot-0.0.4/trellisplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-04-29 18:30:19.000000 trellisplot-0.0.4/trellisplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 18:30:17.000000 trellisplot-0.0.4/trellisplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-29 18:30:17.000000 trellisplot-0.0.4/trellisplot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-29 18:30:17.000000 trellisplot-0.0.4/trellisplot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 18:40:05.305980 trellisplot-0.0.5/
+-rw-rw-rw-   0        0        0      604 2024-04-29 18:40:05.288699 trellisplot-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-29 18:40:05.305980 trellisplot-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-04-29 18:39:26.000000 trellisplot-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:40:05.101001 trellisplot-0.0.5/trellisplot/
+-rw-rw-rw-   0        0        0       22 2024-01-09 20:12:41.000000 trellisplot-0.0.5/trellisplot/__init__.py
+-rw-rw-rw-   0        0        0    13677 2024-04-29 18:34:07.000000 trellisplot-0.0.5/trellisplot/plot.py
+-rw-rw-rw-   0        0        0     9178 2024-04-29 16:38:40.000000 trellisplot-0.0.5/trellisplot/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:40:05.285708 trellisplot-0.0.5/trellisplot.egg-info/
+-rw-rw-rw-   0        0        0      604 2024-04-29 18:40:02.000000 trellisplot-0.0.5/trellisplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-04-29 18:40:04.000000 trellisplot-0.0.5/trellisplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 18:40:02.000000 trellisplot-0.0.5/trellisplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-29 18:40:02.000000 trellisplot-0.0.5/trellisplot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 18:40:02.000000 trellisplot-0.0.5/trellisplot.egg-info/top_level.txt
```

### Comparing `trellisplot-0.0.4/PKG-INFO` & `trellisplot-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trellisplot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Trellis plot tool
 Author: Ethan S. Lee
 Author-email: <sukraelee@gmail.com>
 Keywords: python,trellisplot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `trellisplot-0.0.4/setup.py` & `trellisplot-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'Trellis plot tool'
 LONG_DESCRIPTION = 'Package to plot trellis functionality. Updated with width normalization, new default colormap, and reduced boxplot'
 
 # Setting up
 setup(
         name="trellisplot", 
         version=VERSION,
```

### Comparing `trellisplot-0.0.4/trellisplot/plot.py` & `trellisplot-0.0.5/trellisplot/plot.py`

 * *Files identical despite different names*

### Comparing `trellisplot-0.0.4/trellisplot/utils.py` & `trellisplot-0.0.5/trellisplot/utils.py`

 * *Files identical despite different names*

### Comparing `trellisplot-0.0.4/trellisplot.egg-info/PKG-INFO` & `trellisplot-0.0.5/trellisplot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trellisplot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Trellis plot tool
 Author: Ethan S. Lee
 Author-email: <sukraelee@gmail.com>
 Keywords: python,trellisplot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

