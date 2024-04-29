# Comparing `tmp/opencti_excel_uploader-0.1.tar.gz` & `tmp/opencti_excel_uploader-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencti_excel_uploader-0.1.tar", last modified: Thu Apr 25 15:21:25 2024, max compression
+gzip compressed data, was "opencti_excel_uploader-0.2.1.tar", last modified: Mon Apr 29 09:42:49 2024, max compression
```

## Comparing `opencti_excel_uploader-0.1.tar` & `opencti_excel_uploader-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-25 15:21:25.549017 opencti_excel_uploader-0.1/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1027 2024-04-25 15:21:25.549017 opencti_excel_uploader-0.1/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      468 2024-04-25 11:23:46.000000 opencti_excel_uploader-0.1/README.md
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-25 15:21:25.549017 opencti_excel_uploader-0.1/opencti_excel_uploader/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-25 10:54:59.000000 opencti_excel_uploader-0.1/opencti_excel_uploader/__init__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    18750 2024-04-25 10:54:59.000000 opencti_excel_uploader-0.1/opencti_excel_uploader/models.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      426 2024-04-25 15:18:49.000000 opencti_excel_uploader-0.1/opencti_excel_uploader/setup_opencti_config.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      778 2024-04-25 11:33:03.000000 opencti_excel_uploader-0.1/opencti_excel_uploader/xlsx_processing.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     9682 2024-04-25 10:54:59.000000 opencti_excel_uploader-0.1/opencti_excel_uploader/xlsx_utils.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    49054 2024-04-25 11:31:42.000000 opencti_excel_uploader-0.1/opencti_excel_uploader/xml_utls.py
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-25 15:21:25.549017 opencti_excel_uploader-0.1/opencti_excel_uploader.egg-info/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1027 2024-04-25 15:21:25.000000 opencti_excel_uploader-0.1/opencti_excel_uploader.egg-info/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      476 2024-04-25 15:21:25.000000 opencti_excel_uploader-0.1/opencti_excel_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-25 15:21:25.000000 opencti_excel_uploader-0.1/opencti_excel_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-25 15:21:25.000000 opencti_excel_uploader-0.1/opencti_excel_uploader.egg-info/requires.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-25 15:21:25.000000 opencti_excel_uploader-0.1/opencti_excel_uploader.egg-info/top_level.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-25 15:21:25.549017 opencti_excel_uploader-0.1/setup.cfg
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      750 2024-04-25 15:11:34.000000 opencti_excel_uploader-0.1/setup.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 09:42:49.628038 opencti_excel_uploader-0.2.1/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      721 2024-04-29 09:42:49.628038 opencti_excel_uploader-0.2.1/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      160 2024-04-29 08:17:01.000000 opencti_excel_uploader-0.2.1/README.md
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 09:42:49.620038 opencti_excel_uploader-0.2.1/opencti-excel-uploader/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 09:24:34.000000 opencti_excel_uploader-0.2.1/opencti-excel-uploader/__init__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1842 2024-04-29 09:42:26.000000 opencti_excel_uploader-0.2.1/opencti-excel-uploader/__main__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19522 2024-04-29 08:17:01.000000 opencti_excel_uploader-0.2.1/opencti-excel-uploader/models.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    10018 2024-04-29 08:44:37.000000 opencti_excel_uploader-0.2.1/opencti-excel-uploader/xlsx_utils.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    49096 2024-04-29 08:35:29.000000 opencti_excel_uploader-0.2.1/opencti-excel-uploader/xml_utils.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-29 09:42:49.628038 opencti_excel_uploader-0.2.1/opencti_excel_uploader.egg-info/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      721 2024-04-29 09:42:49.000000 opencti_excel_uploader-0.2.1/opencti_excel_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      472 2024-04-29 09:42:49.000000 opencti_excel_uploader-0.2.1/opencti_excel_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-29 09:42:49.000000 opencti_excel_uploader-0.2.1/opencti_excel_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-29 09:42:49.000000 opencti_excel_uploader-0.2.1/opencti_excel_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-29 09:42:49.000000 opencti_excel_uploader-0.2.1/opencti_excel_uploader.egg-info/requires.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-29 09:42:49.000000 opencti_excel_uploader-0.2.1/opencti_excel_uploader.egg-info/top_level.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-29 09:42:49.628038 opencti_excel_uploader-0.2.1/setup.cfg
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      891 2024-04-29 09:05:04.000000 opencti_excel_uploader-0.2.1/setup.py
```

### Comparing `opencti_excel_uploader-0.1/opencti_excel_uploader/models.py` & `opencti_excel_uploader-0.2.1/opencti-excel-uploader/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,23 @@
 from dotenv import load_dotenv
 import urllib3
 
 urllib3.disable_warnings()
 
 load_dotenv()
 
-opencti_client = OpenCTIApiClient(
-    os.getenv("OPENCTI_URL"),
-    os.getenv("OPENCTI_TOKEN"),
-    log_level=os.getenv("OPENCTI_LOG_LEVEL", "error"),
-)
+
+def get_opencti_client():
+    url = os.getenv("OPENCTI_URL")
+    token = os.getenv("OPENCTI_TOKEN")
+    if not url or not token:
+        raise ValueError(
+            "OPENCTI_URL and OPENCTI_TOKEN must be set in the environment."
+        )
+    return OpenCTIApiClient(url, token)
 
 
 class Incident:
     def __init__(
         self,
         name: str,
         incidentType: str,
@@ -46,14 +50,15 @@
             return self.name == other.name
         return False
 
     def __hash__(self):
         return hash(self.name)
 
     def create_stix_dict(self):
+        opencti_client = get_opencti_client()
         octi_id = opencti_client.incident.read(
             filters={
                 "mode": "and",
                 "filters": [{"key": "name", "values": self.name}],
                 "filterGroups": [],
             },
             customAttributes="standard_id",
@@ -85,14 +90,15 @@
                     "marking-definition--826578e1-40ad-459f-bc73-ede076f81f37"
                 ],
                 "object_refs": [],
                 "external_references": external_references,
             }
 
     def add_marking(self):
+        opencti_client = get_opencti_client()
         marking_read = opencti_client.marking_definition.read(
             filters={
                 "mode": "and",
                 "filters": [{"key": "definition", "values": self.objectMarking}],
                 "filterGroups": [],
             }
         )
@@ -156,14 +162,15 @@
             return self.name == other.name
         return False
 
     def __hash__(self):
         return hash(self.name)
 
     def create_stix_dict(self):
+        opencti_client = get_opencti_client()
         octi_id = opencti_client.incident.read(
             filters={
                 "mode": "and",
                 "filters": [{"key": "name", "values": self.name}],
                 "filterGroups": [],
             },
             customAttributes="standard_id",
@@ -189,14 +196,15 @@
                     }
                 ],
             }
         else:
             raise ValueError("Report already exists")
 
     def find_author(self):
+        opencti_client = get_opencti_client()
         """Search by name to see if author already exists"""
         author_entity = opencti_client.identity.read(
             filters={
                 "mode": "and",
                 "filters": [{"key": "name", "values": self.author}],
                 "filterGroups": [],
             },
@@ -209,14 +217,15 @@
                 "identity_class": author_entity["identity_class"],
             }
             return author_dict
         else:
             return None
 
     def add_marking(self):
+        opencti_client = get_opencti_client()
         marking_read = opencti_client.marking_definition.read(
             filters={
                 "mode": "and",
                 "filters": [{"key": "definition", "values": self.objectMarking}],
                 "filterGroups": [],
             }
         )
@@ -260,14 +269,15 @@
     ):
         self.technique = technique
         self.tactic = tactic
         self.stage = stage
         self.description = description
 
     def create_stix_dict(self):
+        opencti_client = get_opencti_client()
         octi_id = opencti_client.attack_pattern.read(
             filters={
                 "mode": "and",
                 "filters": [{"key": "name", "values": self.technique}],
                 "filterGroups": [],
             },
             customAttributes="standard_id",
@@ -288,14 +298,15 @@
         extRef: str = "",
     ):
         self.name = name
         self.description = description
         self.extRef = extRef
 
     def create_stix_dict(self):
+        opencti_client = get_opencti_client()
         octi_id = opencti_client.campaign.read(
             filters={
                 "mode": "and",
                 "filters": [{"key": "name", "values": self.name}],
                 "filterGroups": [],
             },
             customAttributes="standard_id",
@@ -330,14 +341,15 @@
         extRef: str = "",
     ):
         self.name = name
         self.description = description
         self.extRef = extRef
 
     def create_stix_dict(self):
+        opencti_client = get_opencti_client()
         octi_id = opencti_client.course_of_action.read(
             filters={
                 "mode": "and",
                 "filters": [{"key": "name", "values": self.name}],
                 "filterGroups": [],
             },
             customAttributes="standard_id",
@@ -373,14 +385,15 @@
         self.location = location
 
     def fuzzy_match(self):
         """Search by date and location and keywords to see if event can be found"""
         pass
 
     def create_stix_dict(self):
+        opencti_client = get_opencti_client()
         octi_id = opencti_client.event.read(
             filters={
                 "mode": "and",
                 "filters": [{"key": "name", "values": self.name}],
                 "filterGroups": [],
             },
             customAttributes="standard_id",
@@ -416,14 +429,15 @@
         self.idClass = idClass
 
     def fuzzy_match(self):
         """Search by alias or names w/ without middle name or title to see if identity already exists"""
         pass
 
     def create_stix_dict(self):
+        opencti_client = get_opencti_client()
         if self.idClass == "Individual" or self.idClass == "Organization":
             octi_id = opencti_client.identity.read(
                 filters={
                     "mode": "and",
                     "filters": [{"key": "name", "values": self.name}],
                     "filterGroups": [],
                 },
@@ -488,14 +502,15 @@
         name: str = "",
         description: str = "",
     ):
         self.name = name
         self.description = description
 
     def create_stix_dict(self):
+        opencti_client = get_opencti_client()
         octi_id = opencti_client.narrative.read(
             filters={
                 "mode": "and",
                 "filters": [{"key": "name", "values": self.name}],
                 "filterGroups": [],
             },
             customAttributes="standard_id",
@@ -524,14 +539,15 @@
         self.language = language
 
     def find_channel(self):
         """Search by domain and keywords to see if channel exists"""
         pass
 
     def create_stix_dict(self):
+        opencti_client = get_opencti_client()
         octi_id = opencti_client.stix_cyber_observable.read(
             filters={
                 "mode": "and",
                 "filters": [{"key": "value", "values": self.url}],
                 "filterGroups": [],
             },
             customAttributes="standard_id",
@@ -565,14 +581,15 @@
         name: str = "",
         alias: str = "",
     ):
         self.name = name
         self.alias = alias
 
     def create_stix_dict(self):
+        opencti_client = get_opencti_client()
         octi_id = opencti_client.threat_actor.read(
             filters={
                 "mode": "and",
                 "filters": [{"key": "name", "values": self.name}],
                 "filterGroups": [],
             },
             customAttributes="standard_id",
@@ -591,14 +608,15 @@
         name: str = "",
         description: str = "",
     ):
         self.name = name
         self.description = description
 
     def create_stix_dict(self):
+        opencti_client = get_opencti_client()
         octi_id = opencti_client.vulnerability.read(
             filters={
                 "mode": "and",
                 "filters": [{"key": "name", "values": self.name}],
                 "filterGroups": [],
             },
             customAttributes="standard_id",
```

### Comparing `opencti_excel_uploader-0.1/opencti_excel_uploader/xlsx_utils.py` & `opencti_excel_uploader-0.2.1/opencti-excel-uploader/xlsx_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import pandas as pd
-from opencti_excel_uploader.models import (
+from .models import (
     # Incident,
     Narrative,
     Observable,
     Identity,
     Event,
     Campaign,
     Vulnerability,
     CourseOfAction,
     AttackPattern,
     ThreatActor,
     Report,
-    opencti_client,
+    get_opencti_client,
 )
 import uuid
 import datetime
 import os
 import json
 import random
-from opencti_excel_uploader.xml_utils import create_bundle
+from .xml_utils import create_bundle
 import openpyxl
 
 now = datetime.datetime.now()
 published = now.isoformat() + "Z"
 
 
 def stix_id(entity_type):
@@ -30,15 +30,15 @@
     return f"{entity_type}--{str(uuid.uuid5(uuid.NAMESPACE_DNS, random_str))}"
 
 
 def load_excel(file):
     # Load the workbook and get sheet names
     sheets = openpyxl.load_workbook(file).sheetnames
     df = {}
-
+    print(f"Loading {file}...", flush=True)
     for sheet in sheets:
         # Read each sheet into a DataFrame
         sheet_df = pd.read_excel(file, sheet_name=sheet, engine="openpyxl")
 
         # Normalize column names by removing all whitespaces
         sheet_df.columns = [col.strip() for col in sheet_df.columns]
 
@@ -80,14 +80,15 @@
             language=row["Language"],
         )
         observables.append(observable)
     return observables
 
 
 def process_identity(identity_data, instructions):
+    opencti_client = get_opencti_client()
     # Drop first row with instructions
     if instructions:
         identity_data = identity_data.drop(0)
 
     # Create a list of identities
     identities = []
     for _, row in identity_data.iterrows():
@@ -248,20 +249,20 @@
 
 def process_report(df):
     # Initialize related objects and external references
     related_objects = []
     external_ref_list = []
     data = df["Incident"]
     instructions = True
-
+    print("Processing Report...", flush=True)
     # Check length of data
     if len(data) == 1:
         instructions = False
     else:
-        print("Dropping first row with instructions for all sheets.")
+        print("Dropping first row with instructions for all sheets.", flush=True)
 
     data = data.iloc[-1]
 
     # Retrieve related objects
     for key in df.keys():
         if key == "Threat Actor":
             related_objects.extend(process_threat_actor(df[key], instructions))
@@ -302,22 +303,25 @@
 
 def excel_to_json(file):
     df = load_excel(file)
     report = process_report(df)
     bundle = create_bundle(report)
     for item in bundle["objects"]:
         print(item)
-    with open(f"./excel_workbenches/{report.name}.json", "w") as f:
-        print(f"Writing {report.name}.json to 'excel_workbenches' folder.")
+    desktop_path = os.path.join(os.path.expanduser("~"), "Desktop")
+    with open(os.path.join(desktop_path, f"{report.name}.json"), "w") as f:
+        print(f"Writing {report.name}.json to the desktop.", flush=True)
         json.dump(bundle, f)
 
 
 def folder_to_json(folder):
+    print(f"Converting all Excel files in {folder} to JSON", flush=True)
     for root, _, files in os.walk(folder):
+        print(f"Searching {root} for Excel files.", flush=True)
         # If the folder has no xlsx files, skip
         if not any(file.endswith(".xlsx") for file in files):
-            print(f"No Excel files found in {root}. Moving to next folder.")
+            print(f"No Excel files found in {root}. Moving to next folder.", flush=True)
             continue
         for file in files:
             if file.endswith(".xlsx"):
-                print(f"Converting {os.path.join(root, file)} to JSON")
+                print(f"Converting {os.path.join(root, file)} to JSON", flush=True)
                 excel_to_json(os.path.join(root, file))
```

### Comparing `opencti_excel_uploader-0.1/opencti_excel_uploader/xml_utls.py` & `opencti_excel_uploader-0.2.1/opencti-excel-uploader/xml_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import xml.etree.ElementTree as ET
 from datetime import datetime
-from opencti_excel_uploader.models import (
+from .models import (
     Incident,
     Narrative,
     Observable,
     Identity,
     Event,
     CourseOfAction,
     AttackPattern,
@@ -38,17 +38,17 @@
             current_question_id = element.attrib["id"]
             qns[current_question_id] = {
                 "question": element.text,
                 "possible_answers": {},
             }
         elif element.tag == "Answer":
             if current_question_id:
-                qns[current_question_id]["possible_answers"][element.attrib["id"]] = (
-                    element.text
-                )
+                qns[current_question_id]["possible_answers"][
+                    element.attrib["id"]
+                ] = element.text
     return qns
 
 
 def get_qids(root):
     """Prints question titles and their IDs to a file"""
     survey_id = root.findall(".//Survey")[0].attrib["alias"]
     with open(f"./qids/{survey_titles[survey_id]}_qids.txt", "w") as f:
@@ -974,15 +974,15 @@
                 "x_opencti_color": "#d84315",
                 "x_opencti_order": 3,
                 "name": "TLP:AMBER+STRICT",
                 "type": "marking-definition",
             }
         ],
     }
-
+    print(f"Creating bundle for basic incident #{i}", flush=True)
     objects = []
     # Create object list
     object_list = [r.create_stix_dict() for r in i.relatedEntities if r]
     object_ids = [r["id"] for r in object_list if r]
 
     # Create the incident dictionary
     incident_dict = i.create_stix_dict()
@@ -1049,8 +1049,8 @@
 
 def folder_qids(folder):
     for root, dirs, files in os.walk(folder):
         for file in files:
             if file.endswith(".xml"):
                 print(f"Extracting QIDs from {os.path.join(root, file)}")
                 xml = load_xml(os.path.join(root, file))
-                get_qids(xml)
+                get_qids(xml)
```

### Comparing `opencti_excel_uploader-0.1/setup.py` & `opencti_excel_uploader-0.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
-    name="opencti_excel_uploader",
-    version="0.1",
+    name="opencti-excel-uploader",
+    version="0.2.1",
     packages=find_packages(),
     description="Uploader for cases and reports from Excel files",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="asz,jjk,eby",
     author_email="rnd@stratc.org",
     license="MIT",
@@ -18,8 +18,13 @@
         "urllib3>=2.2.1,<3.0.0",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    entry_points={
+        "console_scripts": [
+            "opencti-excel-uploader=opencti_excel_uploader.__main__:main"
+        ]
+    },
 )
```

