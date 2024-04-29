# Comparing `tmp/opencti_excel_uploader-0.2.3.tar.gz` & `tmp/opencti_excel_uploader-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencti_excel_uploader-0.2.3.tar", last modified: Mon Apr 29 11:30:08 2024, max compression
+gzip compressed data, was "opencti_excel_uploader-0.2.4.tar", last modified: Mon Apr 29 12:07:30 2024, max compression
```

## Comparing `opencti_excel_uploader-0.2.3.tar` & `opencti_excel_uploader-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 11:30:08.815380 opencti_excel_uploader-0.2.3/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 11:30:08.815380 opencti_excel_uploader-0.2.3/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-29 10:12:52.000000 opencti_excel_uploader-0.2.3/README.md
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 11:30:08.811380 opencti_excel_uploader-0.2.3/opencti_excel_uploader/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 09:24:34.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader/__init__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1842 2024-04-29 09:42:26.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader/__main__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19522 2024-04-29 08:17:01.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader/models.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    10018 2024-04-29 10:59:41.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader/xlsx_utils.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    48204 2024-04-29 09:59:40.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader/xml_utils.py
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 11:30:08.815380 opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 11:30:08.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      472 2024-04-29 11:30:08.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-29 11:30:08.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-29 11:30:08.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/entry_points.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-29 11:30:08.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/requires.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-29 11:30:08.000000 opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/top_level.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-29 11:30:08.815380 opencti_excel_uploader-0.2.3/setup.cfg
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      891 2024-04-29 11:29:39.000000 opencti_excel_uploader-0.2.3/setup.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:07:30.983742 opencti_excel_uploader-0.2.4/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:07:30.983742 opencti_excel_uploader-0.2.4/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.4/README.md
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:07:30.975741 opencti_excel_uploader-0.2.4/opencti_excel_uploader/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader/__init__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1842 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader/__main__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader/models.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    10311 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader/xlsx_utils.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    48235 2024-04-29 12:04:56.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader/xml_utils.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 12:07:30.983742 opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      997 2024-04-29 12:07:30.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      472 2024-04-29 12:07:30.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-29 12:07:30.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-29 12:07:30.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-29 12:07:30.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/requires.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-29 12:07:30.000000 opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/top_level.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-29 12:07:30.983742 opencti_excel_uploader-0.2.4/setup.cfg
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      891 2024-04-29 12:06:01.000000 opencti_excel_uploader-0.2.4/setup.py
```

### Comparing `opencti_excel_uploader-0.2.3/PKG-INFO` & `opencti_excel_uploader-0.2.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 0.2.3
+Version: 0.2.4
 Summary: Uploader for cases and reports from Excel files
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-0.2.3/opencti_excel_uploader/__main__.py` & `opencti_excel_uploader-0.2.4/opencti_excel_uploader/__main__.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.3/opencti_excel_uploader/models.py` & `opencti_excel_uploader-0.2.4/opencti_excel_uploader/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime
+import datetime
 import uuid
 import os
 from pycti import OpenCTIApiClient
 from dotenv import load_dotenv
 import urllib3
 
 urllib3.disable_warnings()
@@ -34,15 +34,15 @@
         relatedEntities: list = [],
         extRef: str = "" or list[str],
     ):
         self.name = name
         self.incidentType = incidentType
         self.description = description
         self.objectLabel = objectLabel
-        self.first_seen = first_seen or datetime.now()
+        self.first_seen = first_seen or datetime.datetime.now()
         self.confidence = confidence
         self.objective = objective
         self.objectMarking = objectMarking
         self.relatedEntities = relatedEntities
         self.extRef = extRef
 
     def _eq_(self, other):
@@ -145,15 +145,15 @@
         relatedEntities: list = [],
         extRef: str = "",
         author: str = "",
     ):
         self.name = name
         self.description = description
         self.objectLabel = objectLabel
-        self.first_seen = first_seen or datetime.now()
+        self.first_seen = first_seen or datetime.datetime.now()
         self.confidence = confidence
         self.objective = objective
         self.objectMarking = objectMarking
         self.relatedEntities = relatedEntities
         self.extRef = extRef
         self.author = author
 
@@ -370,16 +370,16 @@
 
 
 class Event:
     def __init__(
         self,
         name: str = "",
         description: str = "",
-        start_date: datetime = datetime.now(),
-        end_date: datetime = datetime.now(),
+        start_date: datetime = datetime.datetime.now(),
+        end_date: datetime = datetime.datetime.now(),
         location: str = "",
     ):
         self.name = name
         self.description = description
         self.start_date = start_date
         self.end_date = end_date
         self.location = location
@@ -523,15 +523,15 @@
             }
 
 
 class Observable:
     def __init__(
         self,
         url: str = "",
-        date: datetime = datetime.now(),
+        date: datetime = datetime.datetime.now(),
         archivedUrl: str = "",
         language: list[str] = [],
     ):
         self.url = (
             url.replace("http://", "").replace("https://", "").replace("www.", "")
         )
         self.date = date
```

### Comparing `opencti_excel_uploader-0.2.3/opencti_excel_uploader/xlsx_utils.py` & `opencti_excel_uploader-0.2.4/opencti_excel_uploader/xlsx_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,24 @@
 import random
 from .xml_utils import create_bundle
 import openpyxl
 
 now = datetime.datetime.now()
 published = now.isoformat() + "Z"
 
-
+def parse_date(date):
+    formats = ["%Y-%m-%d", "%Y-%m-%d %H:%M:%S", "%Y-%m-%d %H:%M:%S.%f", "%Y-%d-%m", "%Y-%d-%m %H:%M:%S", "%Y-%d-%m %H:%M:%S.%f"]
+    
+    for fmt in formats:
+        try:
+            return datetime.datetime.strptime(date, fmt)
+        except ValueError:
+            pass
+        return datetime.datetime.now()
+    
 def stix_id(entity_type):
     random_str = str(random.randint(1000, 9999))
     return f"{entity_type}--{str(uuid.uuid5(uuid.NAMESPACE_DNS, random_str))}"
 
 
 def load_excel(file):
     # Load the workbook and get sheet names
@@ -71,15 +80,15 @@
     # Create a list of observables
     observables = []
     for _, row in observables_data.iterrows():
         if row["URL"] == "":
             break
         observable = Observable(
             url=row["URL"],
-            date=row["Datetime"],
+            date=parse_date(row["Datetime"]),
             archivedUrl=row["Archived link"],
             language=row["Language"],
         )
         observables.append(observable)
     return observables
 
 
@@ -146,16 +155,16 @@
 
     # Create a list of events
     events = []
     for _, row in event_data.iterrows():
         event = Event(
             name=row["Name"],
             description=row["Description"],
-            start_date=datetime.datetime.strptime(row["Start date"], "%Y-%m-%d"),
-            end_date=datetime.datetime.strptime(row["End date"], "%Y-%m-%d"),
+            start_date=parse_date(row["Start date"]),
+            end_date=parse_date(row["End date"]),
         )
         events.append(event)
     return events
 
 
 def process_attack_pattern(attack_pattern_df):
     # Find TTPs used in Incident
```

### Comparing `opencti_excel_uploader-0.2.3/opencti_excel_uploader/xml_utils.py` & `opencti_excel_uploader-0.2.4/opencti_excel_uploader/xml_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import xml.etree.ElementTree as ET
-from datetime import datetime
+import datetime
 from .models import (
     Incident,
     Narrative,
     Observable,
     Identity,
     Event,
     CourseOfAction,
@@ -98,15 +98,15 @@
                     try:
                         first_seen = (
                             (
                                 lookup_answer(
                                     "19eb9887-28c5-4660-852d-f4e547a88629",
                                     answers["answers"][i],
                                 )
-                                or [datetime.now().strftime("%Y-%m-%d")]
+                                or [datetime.datetime.now().strftime("%Y-%m-%d")]
                             )[0]
                             + ":"
                             + (
                                 lookup_answer(
                                     "529b4a66-8d7f-4270-9313-1773d04a539b",
                                     answers["answers"][i],
                                 )
@@ -246,15 +246,15 @@
                                             )[0],
                                             date=datetime.strptime(
                                                 (
                                                     lookup_answer(
                                                         dates[j], answers["answers"][i]
                                                     )
                                                     or [
-                                                        datetime.now().strftime(
+                                                        datetime.datetime.now().strftime(
                                                             "%Y-%m-%d"
                                                         )
                                                     ]
                                                 )[0],
                                                 "%Y-%m-%d",
                                             ),
                                             # archivedUrl=(lookup_answer(
@@ -471,15 +471,15 @@
                         )
                         first_seen = (
                             (
                                 lookup_answer(
                                     "ab21fa1f-18e6-4f0b-9403-47872d660a70",
                                     answers["answers"][i],
                                 )
-                                or [datetime.now().strftime("%Y-%m-%d")]
+                                or [datetime.datetime.now().strftime("%Y-%m-%d")]
                             )[0]
                             + ":"
                             + (
                                 lookup_answer(
                                     "516485e2-e8ea-4407-94c9-2137c25b34d4",
                                     answers["answers"][i],
                                 )
@@ -607,15 +607,15 @@
                                             urls[j], answers["answers"][i]
                                         )[0],
                                         date=datetime.strptime(
                                             (
                                                 lookup_answer(
                                                     dates[j], answers["answers"][i]
                                                 )
-                                                or [datetime.now().strftime("%Y-%m-%d")]
+                                                or [datetime.datetime.now().strftime("%Y-%m-%d")]
                                             )[0],
                                             "%Y-%m-%d",
                                         ),
                                         # archivedUrl=(lookup_answer(
                                         #     archivedUrls[j], answers["answers"][i]
                                         # ) or [""])[0],
                                     )
@@ -845,15 +845,15 @@
                                 lookup_answer(
                                     "b23a6792-c4d1-4f12-8111-9f26d18ee3a2",
                                     answers["answers"][i],
                                 )
                                 or [""]
                             )[0],
                             confidence=90,
-                            first_seen=datetime.now(),
+                            first_seen=datetime.datetime.now(),
                             objectMarking="TLP:AMBER+STRICT",
                             objective=[""],
                             objectLabel=[],
                         )
                     except Exception as e:
                         raise ValueError(
                             f"Error in creating basic incident #{i}, error {e}"
```

### Comparing `opencti_excel_uploader-0.2.3/opencti_excel_uploader.egg-info/PKG-INFO` & `opencti_excel_uploader-0.2.4/opencti_excel_uploader.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 0.2.3
+Version: 0.2.4
 Summary: Uploader for cases and reports from Excel files
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-0.2.3/setup.py` & `opencti_excel_uploader-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="opencti-excel-uploader",
-    version="0.2.3",
+    version="0.2.4",
     packages=find_packages(),
     description="Uploader for cases and reports from Excel files",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="asz,jjk,eby",
     author_email="rnd@stratc.org",
     license="MIT",
```

