# Comparing `tmp/finestock-0.0.3.tar.gz` & `tmp/finestock-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finestock-0.0.3.tar", last modified: Fri Apr 26 09:26:30 2024, max compression
+gzip compressed data, was "finestock-0.0.4.tar", last modified: Mon Apr 29 09:38:22 2024, max compression
```

## Comparing `finestock-0.0.3.tar` & `finestock-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 09:26:30.818812 finestock-0.0.3/
--rw-rw-rw-   0        0        0      589 2024-04-26 09:26:30.817813 finestock-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       82 2024-04-26 09:06:06.000000 finestock-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 09:26:30.795232 finestock-0.0.3/finestock/
--rw-rw-rw-   0        0        0      394 2024-04-26 09:26:20.000000 finestock-0.0.3/finestock/__init__.py
--rw-rw-rw-   0        0        0      374 2024-04-26 07:06:05.000000 finestock-0.0.3/finestock/api_fcatory.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:26:30.810814 finestock-0.0.3/finestock/ebest/
--rw-rw-rw-   0        0        0       24 2024-04-26 07:04:26.000000 finestock-0.0.3/finestock/ebest/__init__.py
--rw-rw-rw-   0        0        0       28 2024-04-26 06:59:49.000000 finestock-0.0.3/finestock/ebest/ebest.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:26:30.813811 finestock-0.0.3/finestock/kis/
--rw-rw-rw-   0        0        0       45 2024-04-26 09:22:42.000000 finestock-0.0.3/finestock/kis/__init__.py
--rw-rw-rw-   0        0        0       22 2024-04-26 07:05:14.000000 finestock-0.0.3/finestock/kis/kis.py
--rw-rw-rw-   0        0        0       23 2024-04-26 07:03:18.000000 finestock-0.0.3/finestock/kis/kis_v.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:26:30.816811 finestock-0.0.3/finestock/model/
--rw-rw-rw-   0        0        0        0 2024-04-26 06:49:59.000000 finestock-0.0.3/finestock/model/__init__.py
--rw-rw-rw-   0        0        0      527 2024-04-26 06:50:39.000000 finestock-0.0.3/finestock/model/price.py
--rw-rw-rw-   0        0        0      939 2024-04-26 06:50:51.000000 finestock-0.0.3/finestock/model/trade.py
--rw-rw-rw-   0        0        0     1146 2024-04-26 06:54:39.000000 finestock-0.0.3/finestock/path.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:26:30.808806 finestock-0.0.3/finestock.egg-info/
--rw-rw-rw-   0        0        0      589 2024-04-26 09:26:30.000000 finestock-0.0.3/finestock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2024-04-26 09:26:30.000000 finestock-0.0.3/finestock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 09:26:30.000000 finestock-0.0.3/finestock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-26 09:14:09.000000 finestock-0.0.3/finestock.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2024-04-26 09:26:30.000000 finestock-0.0.3/finestock.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-26 09:26:30.000000 finestock-0.0.3/finestock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 09:26:30.818812 finestock-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      774 2024-04-26 09:26:27.000000 finestock-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:38:22.656931 finestock-0.0.4/
+-rw-rw-rw-   0        0        0      589 2024-04-29 09:38:22.655931 finestock-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2024-04-26 09:06:06.000000 finestock-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 09:38:22.619005 finestock-0.0.4/finestock/
+-rw-rw-rw-   0        0        0      394 2024-04-29 09:38:16.000000 finestock-0.0.4/finestock/__init__.py
+-rw-rw-rw-   0        0        0      374 2024-04-26 07:06:05.000000 finestock-0.0.4/finestock/api_fcatory.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:38:22.644024 finestock-0.0.4/finestock/ebest/
+-rw-rw-rw-   0        0        0       24 2024-04-26 07:04:26.000000 finestock-0.0.4/finestock/ebest/__init__.py
+-rw-rw-rw-   0        0        0       28 2024-04-26 06:59:49.000000 finestock-0.0.4/finestock/ebest/ebest.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:38:22.651038 finestock-0.0.4/finestock/kis/
+-rw-rw-rw-   0        0        0       45 2024-04-26 09:22:42.000000 finestock-0.0.4/finestock/kis/__init__.py
+-rw-rw-rw-   0        0        0       22 2024-04-26 07:05:14.000000 finestock-0.0.4/finestock/kis/kis.py
+-rw-rw-rw-   0        0        0       23 2024-04-26 07:03:18.000000 finestock-0.0.4/finestock/kis/kis_v.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:38:22.654917 finestock-0.0.4/finestock/model/
+-rw-rw-rw-   0        0        0       42 2024-04-29 09:34:33.000000 finestock-0.0.4/finestock/model/__init__.py
+-rw-rw-rw-   0        0        0      527 2024-04-26 06:50:39.000000 finestock-0.0.4/finestock/model/price.py
+-rw-rw-rw-   0        0        0      939 2024-04-26 06:50:51.000000 finestock-0.0.4/finestock/model/trade.py
+-rw-rw-rw-   0        0        0     1146 2024-04-26 06:54:39.000000 finestock-0.0.4/finestock/path.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:38:22.635083 finestock-0.0.4/finestock.egg-info/
+-rw-rw-rw-   0        0        0      589 2024-04-29 09:38:22.000000 finestock-0.0.4/finestock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      480 2024-04-29 09:38:22.000000 finestock-0.0.4/finestock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 09:38:22.000000 finestock-0.0.4/finestock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-26 09:14:09.000000 finestock-0.0.4/finestock.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2024-04-29 09:38:22.000000 finestock-0.0.4/finestock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-29 09:38:22.000000 finestock-0.0.4/finestock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 09:38:22.656931 finestock-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      774 2024-04-29 09:38:05.000000 finestock-0.0.4/setup.py
```

### Comparing `finestock-0.0.3/PKG-INFO` & `finestock-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finestock
-Version: 0.0.3
+Version: 0.0.4
 Summary: Korean Stock OpenAPI Package(EBest, KIS) creation written by alshin
 Home-page: https://github.com/shinalok/fine-stock-api
 Author: A.Lok, Shin
 Author-email: shinalok357@gmail.com
 Keywords: ebest,kis,openapi,stock,kr
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `finestock-0.0.3/finestock/model/price.py` & `finestock-0.0.4/finestock/model/price.py`

 * *Files identical despite different names*

### Comparing `finestock-0.0.3/finestock/model/trade.py` & `finestock-0.0.4/finestock/model/trade.py`

 * *Files identical despite different names*

### Comparing `finestock-0.0.3/finestock/path.py` & `finestock-0.0.4/finestock/path.py`

 * *Files identical despite different names*

### Comparing `finestock-0.0.3/finestock.egg-info/PKG-INFO` & `finestock-0.0.4/finestock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finestock
-Version: 0.0.3
+Version: 0.0.4
 Summary: Korean Stock OpenAPI Package(EBest, KIS) creation written by alshin
 Home-page: https://github.com/shinalok/fine-stock-api
 Author: A.Lok, Shin
 Author-email: shinalok357@gmail.com
 Keywords: ebest,kis,openapi,stock,kr
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `finestock-0.0.3/setup.py` & `finestock-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='finestock',
-    version='0.0.3',
+    version='0.0.4',
     description='Korean Stock OpenAPI Package(EBest, KIS) creation written by alshin',
     author='A.Lok, Shin',
     author_email='shinalok357@gmail.com',
     url='https://github.com/shinalok/fine-stock-api',
     install_requires=['websockets','asyncio', 'requests',],
     packages=find_packages(exclude=[]),
     keywords=['ebest', 'kis', 'openapi', 'stock', 'kr'],
```

