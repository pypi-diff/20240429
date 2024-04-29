# Comparing `tmp/wheelz_idp_validations-2.tar.gz` & `tmp/wheelz_idp_validations-2.0.1.tar.gz`

## Comparing `wheelz_idp_validations-2.tar` & `wheelz_idp_validations-2.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/LICESNSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/requirements.txt
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/__init__.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/id_sanitizer.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/pcv1_sanitizer.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/pcv2_sanitizer.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/sanitize_exception.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/exceptions/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/exceptions/date_exceptions.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/exceptions/full_name_exceptions.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/exceptions/gender_exceptions.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/exceptions/id_exceptions.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/exceptions/plate_exceptions.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/exceptions/vin_exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/sanitizers/__init__.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/sanitizers/cif.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/sanitizers/date.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/sanitizers/full_name.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/sanitizers/gender.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/sanitizers/id_number.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/sanitizers/plate.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/src/wheelz_idp_validations/sanitizers/vin.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/.gitignore
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/pyproject.toml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/readme.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 wheelz_idp_validations-2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/LICESNSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/requirements.txt
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/__init__.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/id_sanitizer.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/pcv1_sanitizer.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/pcv2_sanitizer.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/sanitize_exception.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/exceptions/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/exceptions/date_exceptions.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/exceptions/full_name_exceptions.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/exceptions/gender_exceptions.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/exceptions/id_exceptions.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/exceptions/plate_exceptions.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/exceptions/vin_exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/sanitizers/__init__.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/sanitizers/cif.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/sanitizers/date.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/sanitizers/full_name.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/sanitizers/gender.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/sanitizers/id_number.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/sanitizers/plate.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/sanitizers/vin.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/.gitignore
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/readme.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.0.1/PKG-INFO
```

### Comparing `wheelz_idp_validations-2/LICESNSE` & `wheelz_idp_validations-2.0.1/LICESNSE`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2/.github/workflows/python-publish.yml` & `wheelz_idp_validations-2.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2/src/wheelz_idp_validations/id_sanitizer.py` & `wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/id_sanitizer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from .sanitizers.id_number import sanitize_id_number
-from .sanitizers.gender import sanitize_gender
-from .sanitizers.full_name import sanitize_fullname
-from .sanitizers.date import sanitize_dates
+from wheelz_idp_validations.sanitizers.id_number import sanitize_id_number
+from wheelz_idp_validations.sanitizers.gender import sanitize_gender
+from wheelz_idp_validations.sanitizers.full_name import sanitize_fullname
+from wheelz_idp_validations.sanitizers.date import sanitize_dates
 
 
 def sanitize_id(response_dict):
     # Sanitize ID Number
-    response_dict["documentNumber"] = sanitize_id_number(response_dict["documentNumber"])
+    response_dict["documentNumber"] = sanitize_id_number(response_dict["documentNumber"], False)
     # Sanitize Gender
     response_dict["gender"] = sanitize_gender(response_dict["gender"])
     # Sanitize ID Full Name
     (response_dict["name"], response_dict["firstSurname"],
      response_dict["secondSurname"]) = (
         sanitize_fullname(response_dict["name"], response_dict["firstSurname"],
                           response_dict["secondSurname"]))
```

### Comparing `wheelz_idp_validations-2/src/wheelz_idp_validations/pcv1_sanitizer.py` & `wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/pcv1_sanitizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from sanitizers.plate import sanitize_plate
-from sanitizers.vin import sanitize_vin
-from sanitizers.date import sanitize_dates
+from wheelz_idp_validations.sanitizers.plate import sanitize_plate
+from wheelz_idp_validations.sanitizers.vin import sanitize_vin
+from wheelz_idp_validations.sanitizers.date import sanitize_dates
 
 
 def sanitize_pcv1(response_dict):
     # Sanitize Plate
     response_dict["matricula"] = sanitize_plate(response_dict["matricula"])
     # Sanitize VIN
     response_dict["serieNumBastidor"] = sanitize_vin(response_dict["serieNumBastidor"])
```

### Comparing `wheelz_idp_validations-2/src/wheelz_idp_validations/pcv2_sanitizer.py` & `wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/pcv2_sanitizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from sanitizers.plate import sanitize_plate
-from sanitizers.vin import sanitize_vin
-from sanitizers.date import sanitize_dates
+from wheelz_idp_validations.sanitizers.plate import sanitize_plate
+from wheelz_idp_validations.sanitizers.vin import sanitize_vin
+from wheelz_idp_validations.sanitizers.date import sanitize_dates
 
 
 def sanitize_pcv2(response_dict):
     # Sanitize Plate
     response_dict["A"] = sanitize_plate(response_dict["A"])
     # Sanitize VIN
     response_dict["E"] = sanitize_vin(response_dict["E"])
```

### Comparing `wheelz_idp_validations-2/src/wheelz_idp_validations/exceptions/date_exceptions.py` & `wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/exceptions/date_exceptions.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2/src/wheelz_idp_validations/exceptions/id_exceptions.py` & `wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/exceptions/id_exceptions.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2/src/wheelz_idp_validations/sanitizers/cif.py` & `wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/sanitizers/cif.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2/src/wheelz_idp_validations/sanitizers/date.py` & `wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/sanitizers/date.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import re
 
-
 def sanitize_dates(received_birth_date, received_expiration_date):
 
     # TODO Change format yyyy mm dd
     # Dates must match this pattern
     pattern = re.compile(r'\d{2}/\d{2}/\d{4}')
 
     processed_birth_date = pattern.search(received_birth_date)
```

### Comparing `wheelz_idp_validations-2/src/wheelz_idp_validations/sanitizers/full_name.py` & `wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/sanitizers/full_name.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2/src/wheelz_idp_validations/sanitizers/id_number.py` & `wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/sanitizers/id_number.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2/src/wheelz_idp_validations/sanitizers/plate.py` & `wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/sanitizers/plate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import re
+import logging
+
+# Configurar logging
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 def sanitize_plate(text):
     # Definir patrones para los diferentes tipos de matrículas
     patterns = [
-        r'\b\d{4}[BCDFGHJKLMNPQRSTVWXYZ]{3}\b',       # Tipo 1: 4 números seguidos de 3 letras no vocales
-        r'\b[A-Z]{1,3}-\d{6}\b',                       # Tipo 2: Hasta 3 letras, guion, 6 números
-        r'\b[A-Z]{1,2}-\d{4}-[A-Z]{1,2}\b',            # Tipo 3: 1-2 letras, guion, 4 números, guion, 1-2 letras
-        r'\bR\d{3}[A-Z]{3}\b',                         # Tipo 4: Una R, 3 números y 3 letras
-        r'\bH\d{4}[A-Z]{3}\b',                         # Tipo 5: Una H, 4 números y 3 letras
-        r'\bC\d{4}[A-Z]{3}\b',                         # Tipo 6: Una C, 4 números y 3 letras
+        r'\b\d{4}[BCDFGHJKLMNPQRSTVWXYZ]{3}\b',  # Tipo 1: 4 números seguidos de 3 letras no vocales
+        r'\b[A-Z]{1,3}\d{6}\b',                  # Tipo 2: Hasta 3 letras seguidas de 6 números
+        r'\b[A-Z]{1,2}\d{4}[A-Z]{1,2}\b',        # Tipo 3: 1-2 letras seguidas de 4 números y 1-2 letras
+        r'\bR\d{3}[A-Z]{3}\b',                   # Tipo 4: Una R, 3 números y 3 letras
+        r'\bH\d{4}[A-Z]{3}\b',                   # Tipo 5: Una H, 4 números y 3 letras
+        r'\bC\d{4}[A-Z]{3}\b',                   # Tipo 6: Una C, 4 números y 3 letras
     ]
 
+    # Comprobar si la entrada es una cadena vacía o solo contiene espacios
+    if not text.strip():
+        logging.info(f"Empty input received for plate processing: '{text}'")
+        return ""  # Retornar cadena vacía directamente si no hay entrada
+
     # Buscar la primera matrícula que coincida con alguno de los patrones
     for pattern in patterns:
         match = re.search(pattern, text.upper().replace(' ', ''))
         if match:
             return match.group(0)
-
-    # Si no se encuentra ninguna matrícula, lanzar excepción
-    raise InvalidPlateException("No valid plate found in the text")
-
-# Ejemplo de uso:
-"""
-text = 'El vehículo tiene la matrícula 1715JYL. Otro texto R123YHG, y más información H1234BBB.'
-first_plate = extract_first_plate(text)
-print(first_plate)  # Debería imprimir la primera matrícula válida encontrada
-"""
+    
+    # Registra que no se encontró una matrícula válida, incluyendo el texto original
+    logging.warning(f"No valid plate found in text: '{text}'")
+    return ""  # Retornar cadena vacía si no se encuentra matrícula
```

### Comparing `wheelz_idp_validations-2/src/wheelz_idp_validations/sanitizers/vin.py` & `wheelz_idp_validations-2.0.1/src/wheelz_idp_validations/sanitizers/vin.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2/pyproject.toml` & `wheelz_idp_validations-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/wheelz_idp_validations"]
 
 
 [project]
 name = "wheelz_idp_validations"
-version = "2"
+version = "2.0.1"
 authors = [
   { name="Lluis" },
 ]
 description = "Validation for spasnish documents"
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `wheelz_idp_validations-2/PKG-INFO` & `wheelz_idp_validations-2.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: wheelz_idp_validations
-Version: 2
+Version: 2.0.1
 Summary: Validation for spasnish documents
 Project-URL: Homepage, https://github.com/albertvazquezm/wheelz-idp-validations
 Project-URL: Issues, https://github.com/albertvazquezm/wheelz-idp-validationsissues
 Author: Lluis
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

