# Comparing `tmp/opencti_excel_uploader-0.2.2.tar.gz` & `tmp/opencti_excel_uploader-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencti_excel_uploader-0.2.2.tar", last modified: Mon Apr 29 11:21:24 2024, max compression
+gzip compressed data, was "opencti_excel_uploader-0.2.3.tar", last modified: Mon Apr 29 11:30:08 2024, max compression
```

## Comparing `opencti_excel_uploader-0.2.2.tar` & `opencti_excel_uploader-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 11:21:24.412473 opencti_excel_uploader-0.2.2/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 11:21:24.412473 opencti_excel_uploader-0.2.2/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-29 10:12:52.000000 opencti_excel_uploader-0.2.2/README.md
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 11:21:24.408473 opencti_excel_uploader-0.2.2/opencti-excel-uploader/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 09:24:34.000000 opencti_excel_uploader-0.2.2/opencti-excel-uploader/__init__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1842 2024-04-29 09:42:26.000000 opencti_excel_uploader-0.2.2/opencti-excel-uploader/__main__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19522 2024-04-29 08:17:01.000000 opencti_excel_uploader-0.2.2/opencti-excel-uploader/models.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    10018 2024-04-29 10:59:41.000000 opencti_excel_uploader-0.2.2/opencti-excel-uploader/xlsx_utils.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    48204 2024-04-29 09:59:40.000000 opencti_excel_uploader-0.2.2/opencti-excel-uploader/xml_utils.py
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 11:21:24.412473 opencti_excel_uploader-0.2.2/opencti_excel_uploader.egg-info/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 11:21:24.000000 opencti_excel_uploader-0.2.2/opencti_excel_uploader.egg-info/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      472 2024-04-29 11:21:24.000000 opencti_excel_uploader-0.2.2/opencti_excel_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-29 11:21:24.000000 opencti_excel_uploader-0.2.2/opencti_excel_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-29 11:21:24.000000 opencti_excel_uploader-0.2.2/opencti_excel_uploader.egg-info/entry_points.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-29 11:21:24.000000 opencti_excel_uploader-0.2.2/opencti_excel_uploader.egg-info/requires.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-29 11:21:24.000000 opencti_excel_uploader-0.2.2/opencti_excel_uploader.egg-info/top_level.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-29 11:21:24.412473 opencti_excel_uploader-0.2.2/setup.cfg
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      891 2024-04-29 11:21:14.000000 opencti_excel_uploader-0.2.2/setup.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 11:30:08.815380 opencti_excel_uploader-0.2.3/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 11:30:08.815380 opencti_excel_uploader-0.2.3/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-29 10:12:52.000000 opencti_excel_uploader-0.2.3/README.md
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 11:30:08.811380 opencti_excel_uploader-0.2.3/opencti_excel_uploader/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 09:24:34.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader/__init__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1842 2024-04-29 09:42:26.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader/__main__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19522 2024-04-29 08:17:01.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader/models.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    10018 2024-04-29 10:59:41.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader/xlsx_utils.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    48204 2024-04-29 09:59:40.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader/xml_utils.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 11:30:08.815380 opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 11:30:08.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      472 2024-04-29 11:30:08.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-29 11:30:08.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-29 11:30:08.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-29 11:30:08.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/requires.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-29 11:30:08.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/top_level.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-29 11:30:08.815380 opencti_excel_uploader-0.2.3/setup.cfg
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      891 2024-04-29 11:29:39.000000 opencti_excel_uploader-0.2.3/setup.py
```

### Comparing `opencti_excel_uploader-0.2.2/PKG-INFO` & `opencti_excel_uploader-0.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 0.2.2
+Version: 0.2.3
 Summary: Uploader for cases and reports from Excel files
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-0.2.2/opencti-excel-uploader/__main__.py` & `opencti_excel_uploader-0.2.3/opencti_excel_uploader/__main__.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.2/opencti-excel-uploader/models.py` & `opencti_excel_uploader-0.2.3/opencti_excel_uploader/models.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.2/opencti-excel-uploader/xlsx_utils.py` & `opencti_excel_uploader-0.2.3/opencti_excel_uploader/xlsx_utils.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.2/opencti-excel-uploader/xml_utils.py` & `opencti_excel_uploader-0.2.3/opencti_excel_uploader/xml_utils.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.2/opencti_excel_uploader.egg-info/PKG-INFO` & `opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 0.2.2
+Version: 0.2.3
 Summary: Uploader for cases and reports from Excel files
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-0.2.2/setup.py` & `opencti_excel_uploader-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="opencti-excel-uploader",
-    version="0.2.2",
+    version="0.2.3",
     packages=find_packages(),
     description="Uploader for cases and reports from Excel files",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="asz,jjk,eby",
     author_email="rnd@stratc.org",
     license="MIT",
```

