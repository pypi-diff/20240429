# Comparing `tmp/wheelz_idp_validations-2.0.2.tar.gz` & `tmp/wheelz_idp_validations-2.1.0.tar.gz`

## Comparing `wheelz_idp_validations-2.0.2.tar` & `wheelz_idp_validations-2.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/LICESNSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/requirements.txt
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/__init__.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/id_sanitizer.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/pcv1_sanitizer.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/pcv2_sanitizer.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/sanitize_exception.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/exceptions/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/exceptions/date_exceptions.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/exceptions/full_name_exceptions.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/exceptions/gender_exceptions.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/exceptions/id_exceptions.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/exceptions/plate_exceptions.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/exceptions/vin_exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/sanitizers/__init__.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/sanitizers/cif.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/sanitizers/date.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/sanitizers/full_name.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/sanitizers/gender.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/sanitizers/id_number.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/sanitizers/plate.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/sanitizers/vin.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/.gitignore
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/pyproject.toml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/readme.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/LICESNSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/requirements.txt
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/id_sanitizer.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/pcv1_sanitizer.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/pcv2_sanitizer.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/sanitize_exception.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/exceptions/__init__.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/exceptions/date_exceptions.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/exceptions/full_name_exceptions.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/exceptions/gender_exceptions.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/exceptions/id_exceptions.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/exceptions/plate_exceptions.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/exceptions/vin_exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/sanitizers/__init__.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/sanitizers/cif.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/sanitizers/date.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/sanitizers/full_name.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/sanitizers/gender.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/sanitizers/id_number.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/sanitizers/plate.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/sanitizers/vin.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/.gitignore
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/readme.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.0/PKG-INFO
```

### Comparing `wheelz_idp_validations-2.0.2/LICESNSE` & `wheelz_idp_validations-2.1.0/LICESNSE`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.0.2/.github/workflows/python-publish.yml` & `wheelz_idp_validations-2.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/id_sanitizer.py` & `wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/id_sanitizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from wheelz_idp_validations.sanitizers.id_number import sanitize_id_number
 from wheelz_idp_validations.sanitizers.gender import sanitize_gender
-from wheelz_idp_validations.sanitizers.full_name import sanitize_fullname
 from wheelz_idp_validations.sanitizers.date import sanitize_dates
 
 
 def sanitize_id(response_dict):
     # Sanitize ID Number
     response_dict["documentNumber"] = sanitize_id_number(response_dict["documentNumber"], False)
+    
     # Sanitize Gender
     response_dict["gender"] = sanitize_gender(response_dict["gender"])
-    # Sanitize ID Full Name
-    (response_dict["name"], response_dict["firstSurname"],
-     response_dict["secondSurname"]) = (
-        sanitize_fullname(response_dict["name"], response_dict["firstSurname"],
-                          response_dict["secondSurname"]))
+    
     # Sanitize Birth Date and Expiration Date
-    response_dict["birthDate"], response_dict["expirationDate"] = (
-        sanitize_dates(response_dict["birthDate"], response_dict["expirationDate"]))
+    response_dict["birthDate"] = sanitize_dates(response_dict["birthDate"])
+    response_dict["expirationDate"] = sanitize_dates(response_dict["expirationDate"])
```

### Comparing `wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/pcv1_sanitizer.py` & `wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/pcv1_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/pcv2_sanitizer.py` & `wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/pcv2_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/exceptions/id_exceptions.py` & `wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/exceptions/id_exceptions.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/sanitizers/cif.py` & `wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/sanitizers/cif.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/sanitizers/full_name.py` & `wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/sanitizers/full_name.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/sanitizers/gender.py` & `wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/sanitizers/gender.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/sanitizers/id_number.py` & `wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/sanitizers/id_number.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/sanitizers/plate.py` & `wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/sanitizers/plate.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.0.2/src/wheelz_idp_validations/sanitizers/vin.py` & `wheelz_idp_validations-2.1.0/src/wheelz_idp_validations/sanitizers/vin.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.0.2/pyproject.toml` & `wheelz_idp_validations-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/wheelz_idp_validations"]
 
 
 [project]
 name = "wheelz_idp_validations"
-version = "2.0.2"
+version = "2.1.0"
 authors = [
   { name="Lluis" },
 ]
 description = "Validation for spasnish documents"
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `wheelz_idp_validations-2.0.2/PKG-INFO` & `wheelz_idp_validations-2.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: wheelz_idp_validations
-Version: 2.0.2
+Version: 2.1.0
 Summary: Validation for spasnish documents
 Project-URL: Homepage, https://github.com/albertvazquezm/wheelz-idp-validations
 Project-URL: Issues, https://github.com/albertvazquezm/wheelz-idp-validationsissues
 Author: Lluis
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

