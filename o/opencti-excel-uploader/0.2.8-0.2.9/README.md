# Comparing `tmp/opencti_excel_uploader-0.2.8.tar.gz` & `tmp/opencti_excel_uploader-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencti_excel_uploader-0.2.8.tar", last modified: Mon Apr 29 12:59:41 2024, max compression
+gzip compressed data, was "opencti_excel_uploader-0.2.9.tar", last modified: Mon Apr 29 13:21:36 2024, max compression
```

## Comparing `opencti_excel_uploader-0.2.8.tar` & `opencti_excel_uploader-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:59:41.640594 opencti_excel_uploader-0.2.8/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:59:41.640594 opencti_excel_uploader-0.2.8/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.8/README.md
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:59:41.636594 opencti_excel_uploader-0.2.8/opencti_excel_uploader/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader/__init__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1842 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader/__main__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader/models.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    10355 2024-04-29 12:59:03.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader/xlsx_utils.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    48307 2024-04-29 12:29:37.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader/xml_utils.py
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:59:41.640594 opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:59:41.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      472 2024-04-29 12:59:41.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-29 12:59:41.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-29 12:59:41.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/entry_points.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-29 12:59:41.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/requires.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-29 12:59:41.000000 opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/top_level.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-29 12:59:41.640594 opencti_excel_uploader-0.2.8/setup.cfg
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      891 2024-04-29 12:59:31.000000 opencti_excel_uploader-0.2.8/setup.py
+drwxr-xr-x   0 strat-ext-e-04 (1986003675) domain users (1986000513)        0 2024-04-29 13:21:36.399147 opencti_excel_uploader-0.2.9/
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      997 2024-04-29 13:21:36.399147 opencti_excel_uploader-0.2.9/PKG-INFO
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      436 2024-04-29 11:43:55.000000 opencti_excel_uploader-0.2.9/README.md
+drwxr-xr-x   0 strat-ext-e-04 (1986003675) domain users (1986000513)        0 2024-04-29 13:21:36.399147 opencti_excel_uploader-0.2.9/opencti_excel_uploader/
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)       27 2024-04-29 11:43:55.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader/__init__.py
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)     1842 2024-04-29 11:43:55.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader/__main__.py
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)    19553 2024-04-29 12:28:49.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader/models.py
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      146 2024-04-29 12:25:14.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader/test.py
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)    10350 2024-04-29 13:07:32.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader/xlsx_utils.py
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)    48307 2024-04-29 12:28:25.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader/xml_utils.py
+drwxr-xr-x   0 strat-ext-e-04 (1986003675) domain users (1986000513)        0 2024-04-29 13:21:36.399147 opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      997 2024-04-29 13:21:36.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      503 2024-04-29 13:21:36.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)        1 2024-04-29 13:21:36.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)       80 2024-04-29 13:21:36.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      114 2024-04-29 13:21:36.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/requires.txt
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)       23 2024-04-29 13:21:36.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/top_level.txt
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)       38 2024-04-29 13:21:36.399147 opencti_excel_uploader-0.2.9/setup.cfg
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      891 2024-04-29 13:21:11.000000 opencti_excel_uploader-0.2.9/setup.py
```

### Comparing `opencti_excel_uploader-0.2.8/PKG-INFO` & `opencti_excel_uploader-0.2.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 0.2.8
+Version: 0.2.9
 Summary: Uploader for cases and reports from Excel files
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-0.2.8/opencti_excel_uploader/__main__.py` & `opencti_excel_uploader-0.2.9/opencti_excel_uploader/__main__.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.8/opencti_excel_uploader/models.py` & `opencti_excel_uploader-0.2.9/opencti_excel_uploader/models.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.8/opencti_excel_uploader/xlsx_utils.py` & `opencti_excel_uploader-0.2.9/opencti_excel_uploader/xlsx_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     for fmt in formats:
         try:
             date=datetime.datetime.strptime(date, fmt)
             print(date, type(date))
             return date
         except ValueError:
             pass
-        return now
+    
+    return now
     
 def stix_id(entity_type):
     random_str = str(random.randint(1000, 9999))
     return f"{entity_type}--{str(uuid.uuid5(uuid.NAMESPACE_DNS, random_str))}"
 
 
 def load_excel(file):
@@ -298,15 +299,15 @@
         if key == "Vulnerabilities":
             related_objects.extend(process_vulnerabilities(df[key], instructions))
 
     return Report(
         name=data["Name"],
         description=data["Description"],
         objectLabel=[],
-        first_seen=published,
+        first_seen=now,
         confidence=90,
         objective=[],
         objectMarking="TLP:AMBER+STRICT",
         extRef=[data["External Reference"]].extend(external_ref_list),
         author="EEAS",
         relatedEntities=related_objects,
     )
```

### Comparing `opencti_excel_uploader-0.2.8/opencti_excel_uploader/xml_utils.py` & `opencti_excel_uploader-0.2.9/opencti_excel_uploader/xml_utils.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.8/opencti_excel_uploader.egg-info/PKG-INFO` & `opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 0.2.8
+Version: 0.2.9
 Summary: Uploader for cases and reports from Excel files
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-0.2.8/setup.py` & `opencti_excel_uploader-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="opencti-excel-uploader",
-    version="0.2.8",
+    version="0.2.9",
     packages=find_packages(),
     description="Uploader for cases and reports from Excel files",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="asz,jjk,eby",
     author_email="rnd@stratc.org",
     license="MIT",
```

