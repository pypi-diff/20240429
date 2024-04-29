# Comparing `tmp/opencti_excel_uploader-0.2.5.tar.gz` & `tmp/opencti_excel_uploader-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencti_excel_uploader-0.2.5.tar", last modified: Mon Apr 29 12:13:14 2024, max compression
+gzip compressed data, was "opencti_excel_uploader-0.2.6.tar", last modified: Mon Apr 29 12:29:56 2024, max compression
```

## Comparing `opencti_excel_uploader-0.2.5.tar` & `opencti_excel_uploader-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:13:14.645659 opencti_excel_uploader-0.2.5/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:13:14.645659 opencti_excel_uploader-0.2.5/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.5/README.md
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:13:14.633659 opencti_excel_uploader-0.2.5/opencti_excel_uploader/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader/__init__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1842 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader/__main__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader/models.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    10302 2024-04-29 12:12:52.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader/xlsx_utils.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    48235 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader/xml_utils.py
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:13:14.645659 opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:13:14.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      472 2024-04-29 12:13:14.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-29 12:13:14.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-29 12:13:14.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/entry_points.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-29 12:13:14.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/requires.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-29 12:13:14.000000 opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/top_level.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-29 12:13:14.645659 opencti_excel_uploader-0.2.5/setup.cfg
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      891 2024-04-29 12:13:03.000000 opencti_excel_uploader-0.2.5/setup.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:29:56.835189 opencti_excel_uploader-0.2.6/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:29:56.835189 opencti_excel_uploader-0.2.6/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.6/README.md
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:29:56.831189 opencti_excel_uploader-0.2.6/opencti_excel_uploader/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.6/opencti_excel_uploader/__init__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1842 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.6/opencti_excel_uploader/__main__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.6/opencti_excel_uploader/models.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    10311 2024-04-29 12:29:37.000000 opencti_excel_uploader-0.2.6/opencti_excel_uploader/xlsx_utils.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    48307 2024-04-29 12:29:37.000000 opencti_excel_uploader-0.2.6/opencti_excel_uploader/xml_utils.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:29:56.831189 opencti_excel_uploader-0.2.6/opencti_excel_uploader.egg-info/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:29:56.000000 opencti_excel_uploader-0.2.6/opencti_excel_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      472 2024-04-29 12:29:56.000000 opencti_excel_uploader-0.2.6/opencti_excel_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-29 12:29:56.000000 opencti_excel_uploader-0.2.6/opencti_excel_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-29 12:29:56.000000 opencti_excel_uploader-0.2.6/opencti_excel_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-29 12:29:56.000000 opencti_excel_uploader-0.2.6/opencti_excel_uploader.egg-info/requires.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-29 12:29:56.000000 opencti_excel_uploader-0.2.6/opencti_excel_uploader.egg-info/top_level.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-29 12:29:56.835189 opencti_excel_uploader-0.2.6/setup.cfg
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      891 2024-04-29 12:29:42.000000 opencti_excel_uploader-0.2.6/setup.py
```

### Comparing `opencti_excel_uploader-0.2.5/PKG-INFO` & `opencti_excel_uploader-0.2.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 0.2.5
+Version: 0.2.6
 Summary: Uploader for cases and reports from Excel files
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-0.2.5/opencti_excel_uploader/__main__.py` & `opencti_excel_uploader-0.2.6/opencti_excel_uploader/__main__.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.5/opencti_excel_uploader/models.py` & `opencti_excel_uploader-0.2.6/opencti_excel_uploader/models.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.5/opencti_excel_uploader/xlsx_utils.py` & `opencti_excel_uploader-0.2.6/opencti_excel_uploader/xlsx_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 published = now.isoformat() + "Z"
 
 def parse_date(date):
     formats = ["%Y-%m-%d", "%Y-%m-%d %H:%M:%S", "%Y-%m-%d %H:%M:%S.%f", "%Y-%d-%m", "%Y-%d-%m %H:%M:%S", "%Y-%d-%m %H:%M:%S.%f"]
     
     for fmt in formats:
         try:
-            return datetime.strptime(date, fmt)
+            return datetime.datetime.strptime(date, fmt)
         except ValueError:
             pass
         return datetime.datetime.now()
     
 def stix_id(entity_type):
     random_str = str(random.randint(1000, 9999))
     return f"{entity_type}--{str(uuid.uuid5(uuid.NAMESPACE_DNS, random_str))}"
```

### Comparing `opencti_excel_uploader-0.2.5/opencti_excel_uploader/xml_utils.py` & `opencti_excel_uploader-0.2.6/opencti_excel_uploader/xml_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                                 lookup_answer(
                                     "db6f8243-d32d-46e1-85e0-0686245fd9ff",  # Author email
                                     answers["answers"][i],
                                 )
                                 or [""]
                             )[0],
                             confidence=90,
-                            first_seen=datetime.strptime(
+                            first_seen=datetime.datetime.strptime(
                                 first_seen, "%Y-%m-%d:%H:%M:%S"
                             ),
                             objectMarking="TLP:AMBER+STRICT",
                             objectLabel=all_labels,
                             objective=(
                                 lookup_answer(
                                     "1737b237-0010-4853-b5c8-5499423cc6de",
@@ -240,15 +240,15 @@
                             if lookup_answer(urls[j], answers["answers"][i]):
                                 if lookup_answer(dates[j], answers["answers"][i]):
                                     incident.relatedEntities.append(
                                         Observable(
                                             url=lookup_answer(
                                                 urls[j], answers["answers"][i]
                                             )[0],
-                                            date=datetime.strptime(
+                                            date=datetime.datetime.strptime(
                                                 (
                                                     lookup_answer(
                                                         dates[j], answers["answers"][i]
                                                     )
                                                     or [
                                                         datetime.datetime.now().strftime(
                                                             "%Y-%m-%d"
@@ -343,22 +343,22 @@
                                         "933be5c4-865a-46d3-8ff8-8545aecdeb13",
                                         answers["answers"][i],
                                     )[0],
                                     location=lookup_answer(
                                         "bd866e29-7564-4cff-bb8b-a271862d9bd1",
                                         answers["answers"][i],
                                     )[0],
-                                    start_date=datetime.strptime(
+                                    start_date=datetime.datetime.strptime(
                                         lookup_answer(
                                             "d670e193-bc6f-42a1-ad80-8b2e4f3eb479",
                                             answers["answers"][i],
                                         )[0],
                                         "%Y-%m-%d",
                                     ),
-                                    end_date=datetime.strptime(
+                                    end_date=datetime.datetime.strptime(
                                         lookup_answer(
                                             "4753628d-5713-4814-8e0a-d40c79371a0e",
                                             answers["answers"][i],
                                         )[0],
                                         "%Y-%m-%d",
                                     ),
                                 )
@@ -513,15 +513,15 @@
                                 lookup_answer(
                                     "0e47734c-195c-4a25-ad44-421b36a1ac86",
                                     answers["answers"][i],
                                 )
                                 or [""]
                             )[0],
                             confidence=90,
-                            first_seen=datetime.strptime(
+                            first_seen=datetime.datetime.strptime(
                                 first_seen, "%Y-%m-%d:%H:%M:%S"
                             ),
                             objectMarking="TLP:AMBER+STRICT",
                             objectLabel=all_labels,
                             objective=[""],
                             extRef=(
                                 lookup_answer(
@@ -602,15 +602,15 @@
                         try:
                             if lookup_answer(urls[j], answers["answers"][i]):
                                 incident.relatedEntities.append(
                                     Observable(
                                         url=lookup_answer(
                                             urls[j], answers["answers"][i]
                                         )[0],
-                                        date=datetime.strptime(
+                                        date=datetime.datetime.strptime(
                                             (
                                                 lookup_answer(
                                                     dates[j], answers["answers"][i]
                                                 )
                                                 or [datetime.datetime.now().strftime("%Y-%m-%d")]
                                             )[0],
                                             "%Y-%m-%d",
@@ -693,22 +693,22 @@
                                         "87f89323-0167-4b5a-ab39-a0a2e36c56d8",
                                         answers["answers"][i],
                                     )[0],
                                     location=lookup_answer(
                                         "dad80ad3-138b-48e5-bee9-9b11d08a6747",
                                         answers["answers"][i],
                                     )[0],
-                                    start_date=datetime.strptime(
+                                    start_date=datetime.datetime.strptime(
                                         lookup_answer(
                                             "889e207d-5671-469b-82ab-6322c6ab6f52",
                                             answers["answers"][i],
                                         )[0],
                                         "%Y-%m-%d",
                                     ),
-                                    end_date=datetime.strptime(
+                                    end_date=datetime.datetime.strptime(
                                         lookup_answer(
                                             "0979109c-3c7e-4b8f-a3dc-c80f7e321e5f",
                                             answers["answers"][i],
                                         )[0],
                                         "%Y-%m-%d",
                                     ),
                                 )
```

### Comparing `opencti_excel_uploader-0.2.5/opencti_excel_uploader.egg-info/PKG-INFO` & `opencti_excel_uploader-0.2.6/opencti_excel_uploader.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 0.2.5
+Version: 0.2.6
 Summary: Uploader for cases and reports from Excel files
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-0.2.5/setup.py` & `opencti_excel_uploader-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="opencti-excel-uploader",
-    version="0.2.5",
+    version="0.2.6",
     packages=find_packages(),
     description="Uploader for cases and reports from Excel files",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="asz,jjk,eby",
     author_email="rnd@stratc.org",
     license="MIT",
```

