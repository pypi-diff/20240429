# Comparing `tmp/opencti_excel_uploader-0.2.4.tar.gz` & `tmp/opencti_excel_uploader-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencti_excel_uploader-0.2.4.tar", last modified: Mon Apr 29 12:07:30 2024, max compression
+gzip compressed data, was "opencti_excel_uploader-0.2.5.tar", last modified: Mon Apr 29 12:13:14 2024, max compression
```

## Comparing `opencti_excel_uploader-0.2.4.tar` & `opencti_excel_uploader-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:07:30.983742 opencti_excel_uploader-0.2.4/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:07:30.983742 opencti_excel_uploader-0.2.4/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.4/README.md
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:07:30.975741 opencti_excel_uploader-0.2.4/opencti_excel_uploader/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader/__init__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1842 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader/__main__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader/models.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    10311 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader/xlsx_utils.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    48235 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader/xml_utils.py
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:07:30.983742 opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:07:30.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      472 2024-04-29 12:07:30.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-29 12:07:30.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-29 12:07:30.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/entry_points.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-29 12:07:30.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/requires.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-29 12:07:30.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/top_level.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-29 12:07:30.983742 opencti_excel_uploader-0.2.4/setup.cfg
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      891 2024-04-29 12:06:01.000000 opencti_excel_uploader-0.2.4/setup.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:13:14.645659 opencti_excel_uploader-0.2.5/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:13:14.645659 opencti_excel_uploader-0.2.5/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.5/README.md
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:13:14.633659 opencti_excel_uploader-0.2.5/opencti_excel_uploader/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader/__init__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1842 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader/__main__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader/models.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    10302 2024-04-29 12:12:52.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader/xlsx_utils.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    48235 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader/xml_utils.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:13:14.645659 opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:13:14.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      472 2024-04-29 12:13:14.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-29 12:13:14.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-29 12:13:14.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-29 12:13:14.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/requires.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-29 12:13:14.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/top_level.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-29 12:13:14.645659 opencti_excel_uploader-0.2.5/setup.cfg
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      891 2024-04-29 12:13:03.000000 opencti_excel_uploader-0.2.5/setup.py
```

### Comparing `opencti_excel_uploader-0.2.4/PKG-INFO` & `opencti_excel_uploader-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 0.2.4
+Version: 0.2.5
 Summary: Uploader for cases and reports from Excel files
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-0.2.4/opencti_excel_uploader/__main__.py` & `opencti_excel_uploader-0.2.5/opencti_excel_uploader/__main__.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.4/opencti_excel_uploader/models.py` & `opencti_excel_uploader-0.2.5/opencti_excel_uploader/models.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.4/opencti_excel_uploader/xlsx_utils.py` & `opencti_excel_uploader-0.2.5/opencti_excel_uploader/xlsx_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 published = now.isoformat() + "Z"
 
 def parse_date(date):
     formats = ["%Y-%m-%d", "%Y-%m-%d %H:%M:%S", "%Y-%m-%d %H:%M:%S.%f", "%Y-%d-%m", "%Y-%d-%m %H:%M:%S", "%Y-%d-%m %H:%M:%S.%f"]
     
     for fmt in formats:
         try:
-            return datetime.datetime.strptime(date, fmt)
+            return datetime.strptime(date, fmt)
         except ValueError:
             pass
         return datetime.datetime.now()
     
 def stix_id(entity_type):
     random_str = str(random.randint(1000, 9999))
     return f"{entity_type}--{str(uuid.uuid5(uuid.NAMESPACE_DNS, random_str))}"
```

### Comparing `opencti_excel_uploader-0.2.4/opencti_excel_uploader/xml_utils.py` & `opencti_excel_uploader-0.2.5/opencti_excel_uploader/xml_utils.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/PKG-INFO` & `opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 0.2.4
+Version: 0.2.5
 Summary: Uploader for cases and reports from Excel files
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-0.2.4/setup.py` & `opencti_excel_uploader-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="opencti-excel-uploader",
-    version="0.2.4",
+    version="0.2.5",
     packages=find_packages(),
     description="Uploader for cases and reports from Excel files",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="asz,jjk,eby",
     author_email="rnd@stratc.org",
     license="MIT",
```

