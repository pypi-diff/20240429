# Comparing `tmp/opencti_excel_uploader-0.2.7.tar.gz` & `tmp/opencti_excel_uploader-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencti_excel_uploader-0.2.7.tar", last modified: Mon Apr 29 12:37:17 2024, max compression
+gzip compressed data, was "opencti_excel_uploader-0.2.8.tar", last modified: Mon Apr 29 12:59:41 2024, max compression
```

## Comparing `opencti_excel_uploader-0.2.7.tar` & `opencti_excel_uploader-0.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:37:17.901418 opencti_excel_uploader-0.2.7/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:37:17.901418 opencti_excel_uploader-0.2.7/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.7/README.md
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:37:17.901418 opencti_excel_uploader-0.2.7/opencti_excel_uploader/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.7/opencti_excel_uploader/__init__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1842 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.7/opencti_excel_uploader/__main__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.7/opencti_excel_uploader/models.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    10317 2024-04-29 12:36:59.000000 opencti_excel_uploader-0.2.7/opencti_excel_uploader/xlsx_utils.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    48307 2024-04-29 12:29:37.000000 opencti_excel_uploader-0.2.7/opencti_excel_uploader/xml_utils.py
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:37:17.901418 opencti_excel_uploader-0.2.7/opencti_excel_uploader.egg-info/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:37:17.000000 opencti_excel_uploader-0.2.7/opencti_excel_uploader.egg-info/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      472 2024-04-29 12:37:17.000000 opencti_excel_uploader-0.2.7/opencti_excel_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-29 12:37:17.000000 opencti_excel_uploader-0.2.7/opencti_excel_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-29 12:37:17.000000 opencti_excel_uploader-0.2.7/opencti_excel_uploader.egg-info/entry_points.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-29 12:37:17.000000 opencti_excel_uploader-0.2.7/opencti_excel_uploader.egg-info/requires.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-29 12:37:17.000000 opencti_excel_uploader-0.2.7/opencti_excel_uploader.egg-info/top_level.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-29 12:37:17.901418 opencti_excel_uploader-0.2.7/setup.cfg
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      891 2024-04-29 12:37:04.000000 opencti_excel_uploader-0.2.7/setup.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:59:41.640594 opencti_excel_uploader-0.2.8/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:59:41.640594 opencti_excel_uploader-0.2.8/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.8/README.md
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:59:41.636594 opencti_excel_uploader-0.2.8/opencti_excel_uploader/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader/__init__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1842 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader/__main__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader/models.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    10355 2024-04-29 12:59:03.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader/xlsx_utils.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    48307 2024-04-29 12:29:37.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader/xml_utils.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:59:41.640594 opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:59:41.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      472 2024-04-29 12:59:41.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-29 12:59:41.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-29 12:59:41.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-29 12:59:41.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/requires.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-29 12:59:41.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/top_level.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-29 12:59:41.640594 opencti_excel_uploader-0.2.8/setup.cfg
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      891 2024-04-29 12:59:31.000000 opencti_excel_uploader-0.2.8/setup.py
```

### Comparing `opencti_excel_uploader-0.2.7/PKG-INFO` & `opencti_excel_uploader-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 0.2.7
+Version: 0.2.8
 Summary: Uploader for cases and reports from Excel files
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-0.2.7/opencti_excel_uploader/__main__.py` & `opencti_excel_uploader-0.2.8/opencti_excel_uploader/__main__.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.7/opencti_excel_uploader/models.py` & `opencti_excel_uploader-0.2.8/opencti_excel_uploader/models.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.7/opencti_excel_uploader/xlsx_utils.py` & `opencti_excel_uploader-0.2.8/opencti_excel_uploader/xlsx_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,18 +25,20 @@
 published = now.isoformat() + "Z"
 
 def parse_date(date):
     formats = ["%Y-%m-%d", "%Y-%m-%d %H:%M:%S", "%Y-%m-%d %H:%M:%S.%f", "%Y-%d-%m", "%Y-%d-%m %H:%M:%S", "%Y-%d-%m %H:%M:%S.%f"]
     
     for fmt in formats:
         try:
-            return datetime.datetime.strptime(date, fmt)
+            date=datetime.datetime.strptime(date, fmt)
+            print(date, type(date))
+            return date
         except ValueError:
             pass
-        return datetime.datetime.now()
+        return now
     
 def stix_id(entity_type):
     random_str = str(random.randint(1000, 9999))
     return f"{entity_type}--{str(uuid.uuid5(uuid.NAMESPACE_DNS, random_str))}"
 
 
 def load_excel(file):
```

### Comparing `opencti_excel_uploader-0.2.7/opencti_excel_uploader/xml_utils.py` & `opencti_excel_uploader-0.2.8/opencti_excel_uploader/xml_utils.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.7/opencti_excel_uploader.egg-info/PKG-INFO` & `opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 0.2.7
+Version: 0.2.8
 Summary: Uploader for cases and reports from Excel files
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-0.2.7/setup.py` & `opencti_excel_uploader-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="opencti-excel-uploader",
-    version="0.2.7",
+    version="0.2.8",
     packages=find_packages(),
     description="Uploader for cases and reports from Excel files",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="asz,jjk,eby",
     author_email="rnd@stratc.org",
     license="MIT",
```

