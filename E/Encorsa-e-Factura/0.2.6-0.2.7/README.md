# Comparing `tmp/encorsa_e_factura-0.2.6.tar.gz` & `tmp/encorsa_e_factura-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encorsa_e_factura-0.2.6.tar", last modified: Fri Apr 26 11:37:43 2024, max compression
+gzip compressed data, was "encorsa_e_factura-0.2.7.tar", last modified: Mon Apr 29 09:36:52 2024, max compression
```

## Comparing `encorsa_e_factura-0.2.6.tar` & `encorsa_e_factura-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 11:37:43.245446 encorsa_e_factura-0.2.6/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-26 11:37:27.000000 encorsa_e_factura-0.2.6/LICENCE
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-04-26 11:37:43.245446 encorsa_e_factura-0.2.6/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-26 11:37:27.000000 encorsa_e_factura-0.2.6/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-04-26 11:37:40.000000 encorsa_e_factura-0.2.6/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)      679 2024-04-26 11:37:43.245446 encorsa_e_factura-0.2.6/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 11:37:43.241446 encorsa_e_factura-0.2.6/src/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 11:37:43.245446 encorsa_e_factura-0.2.6/src/Encorsa_e_Factura/
--rw-r--r--   0 vsts      (1001) docker     (127)     7407 2024-04-26 11:37:27.000000 encorsa_e_factura-0.2.6/src/Encorsa_e_Factura/WebConRequestUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15500 2024-04-26 11:37:27.000000 encorsa_e_factura-0.2.6/src/Encorsa_e_Factura/XMLUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-04-26 11:37:27.000000 encorsa_e_factura-0.2.6/src/Encorsa_e_Factura/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      624 2024-04-26 11:37:27.000000 encorsa_e_factura-0.2.6/src/Encorsa_e_Factura/runLocaly.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18300 2024-04-26 11:37:27.000000 encorsa_e_factura-0.2.6/src/Encorsa_e_Factura/sincronizare.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-26 11:37:43.245446 encorsa_e_factura-0.2.6/src/Encorsa_e_Factura.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-04-26 11:37:43.000000 encorsa_e_factura-0.2.6/src/Encorsa_e_Factura.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-04-26 11:37:43.000000 encorsa_e_factura-0.2.6/src/Encorsa_e_Factura.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-26 11:37:43.000000 encorsa_e_factura-0.2.6/src/Encorsa_e_Factura.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-04-26 11:37:43.000000 encorsa_e_factura-0.2.6/src/Encorsa_e_Factura.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-04-26 11:37:43.000000 encorsa_e_factura-0.2.6/src/Encorsa_e_Factura.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-04-26 11:37:43.000000 encorsa_e_factura-0.2.6/src/Encorsa_e_Factura.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 09:36:52.947126 encorsa_e_factura-0.2.7/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-29 09:36:35.000000 encorsa_e_factura-0.2.7/LICENCE
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-04-29 09:36:52.947126 encorsa_e_factura-0.2.7/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-29 09:36:35.000000 encorsa_e_factura-0.2.7/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-04-29 09:36:50.000000 encorsa_e_factura-0.2.7/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)      679 2024-04-29 09:36:52.947126 encorsa_e_factura-0.2.7/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 09:36:52.947126 encorsa_e_factura-0.2.7/src/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 09:36:52.947126 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7507 2024-04-29 09:36:35.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/WebConRequestUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15500 2024-04-29 09:36:35.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/XMLUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-04-29 09:36:35.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      624 2024-04-29 09:36:35.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/runLocaly.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18434 2024-04-29 09:36:35.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/sincronizare.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 09:36:52.947126 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-04-29 09:36:52.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-04-29 09:36:52.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-29 09:36:52.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-04-29 09:36:52.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-04-29 09:36:52.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-04-29 09:36:52.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/top_level.txt
```

### Comparing `encorsa_e_factura-0.2.6/LICENCE` & `encorsa_e_factura-0.2.7/LICENCE`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.6/PKG-INFO` & `encorsa_e_factura-0.2.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Encorsa_e_Factura
-Version: 0.2.6
+Version: 0.2.7
 Summary: A small example package
 Home-page: https://encorsa.ro
 Author: Dan Popescu, Razvan Ogrezeanu
 Author-email: dan.popescu@encorsa.com, razvan.ogrezeanu@encorsa.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `encorsa_e_factura-0.2.6/README.md` & `encorsa_e_factura-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.6/setup.cfg` & `encorsa_e_factura-0.2.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Encorsa_e_Factura
-version = 0.2.6
+version = 0.2.7
 author = Dan Popescu, Razvan Ogrezeanu
 author_email = dan.popescu@encorsa.com, razvan.ogrezeanu@encorsa.com
 description = A small example package
 long_description = file: README.md
 url = https://encorsa.ro
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `encorsa_e_factura-0.2.6/src/Encorsa_e_Factura/WebConRequestUtils.py` & `encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/WebConRequestUtils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 try:
     from .XMLUtils import *
 except ImportError:
     from XMLUtils import *
 
 
-def create_webcon_body(parameters, xml_b64, pdf_b64, xml_file_data, id, cui, template_xml_path, wfd_id_duplicate, namespaces, document_type, id_anaf):
+def create_webcon_body(parameters, xml_b64, pdf_b64, xml_file_data, id, cui, template_xml_path, wfd_id_duplicate, namespaces, document_type, id_anaf, iso_data_creare):
 
     processor = XMLProcessor(template_xml_path, xml_file_data, namespaces)
     all_lists_data, extracted_data = processor.process_xml()
 
     item_lists_json = create_list_of_dicts(all_lists_data)
     form_fields_json = create_form_filed_json(extracted_data)
 
@@ -52,14 +52,15 @@
 
     if "webcon_parent_wfdid" in parameters and parameters['webcon_parent_wfdid'] is not None and parameters['webcon_parent_wfdid'] not in ['', 0]:
         body["parentInstanceId"] = parameters['webcon_parent_wfdid']
 
     add_value_to_form_field(parameters, "duplicate_wfdid_field_guid", body, wfd_id_duplicate)
     add_value_to_form_field(parameters, "tipInregistrare_Nota_sau_Factura", body, document_type)
     add_value_to_form_field(parameters, "ID_Descarcare_ANAF", body, id_anaf)
+    add_value_to_form_field(parameters, "Data_Creare_ANAF", body, iso_data_creare)
 
     return body
 
 def add_value_to_form_field(parameters, parameter_key, body, value):
     if value is None:
         value = ''
```

### Comparing `encorsa_e_factura-0.2.6/src/Encorsa_e_Factura/XMLUtils.py` & `encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/XMLUtils.py`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.6/src/Encorsa_e_Factura/runLocaly.py` & `encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/runLocaly.py`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.6/src/Encorsa_e_Factura/sincronizare.py` & `encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/sincronizare.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import xml.etree.ElementTree as ET
 from datetime import datetime
 import requests
 import zipfile
 from requests.auth import HTTPBasicAuth
 import argparse
+from datetime import datetime
 
 try:
     from .XMLUtils import *
 except:
     from XMLUtils import *
 
 try:
@@ -222,14 +223,16 @@
 
     for message in messages:
         # print(f'Processing message {current_message} of {len(messages)}')
         try:
             id_solicitare = message["id_solicitare"]
             id = message["id"]
             tip_factura = message["tip"]
+            iso_data_creare = datetime.strptime(message["data_creare"], "%Y%m%d%H%M")
+
             filtru_facturi = parameters.get('ANAF_invoice_type_filter_E_T_P_R', '')
 
             if filtru_facturi != '':
                 if tip_factura != filtru_facturi:
                     print(f"Skipping invoice with ANAF_ID: {id}, because type filters are applied. The filter is: {filtru_facturi})")
                     continue
             else:
@@ -295,15 +298,15 @@
                     continue
             
             pdf_content = xml_to_pdf_to_base64(xml_text, parameters)
             xml_bytes = str(xml_text).encode('utf-8')
             base64_encoded_xml = base64.b64encode(xml_bytes)
             base64_string_xml = base64_encoded_xml.decode('utf-8')
 
-            body = create_webcon_body(parameters, base64_string_xml, pdf_content, xml_text, invoice_id_element, company_id, local_xml_template_file_path, wfd_id_duplicate, local_namespaces, document_type, id)
+            body = create_webcon_body(parameters, base64_string_xml, pdf_content, xml_text, invoice_id_element, company_id, local_xml_template_file_path, wfd_id_duplicate, local_namespaces, document_type, id, iso_data_creare)
             response = create_invoice_instance(parameters, wtoken, body)
             print(f"{document_type} instance created with SUCCESS having WFD_ID: < {response['id']} >.")
         except Exception as ex:
             # Preparing and printing a detailed error message
             error_details = f"Error at processing message: {message}.\nError message: {str(ex)}"
             raise Exception(error_details)
         current_message += 1
```

### Comparing `encorsa_e_factura-0.2.6/src/Encorsa_e_Factura.egg-info/PKG-INFO` & `encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Encorsa_e_Factura
-Version: 0.2.6
+Version: 0.2.7
 Summary: A small example package
 Home-page: https://encorsa.ro
 Author: Dan Popescu, Razvan Ogrezeanu
 Author-email: dan.popescu@encorsa.com, razvan.ogrezeanu@encorsa.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

