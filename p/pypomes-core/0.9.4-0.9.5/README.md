# Comparing `tmp/pypomes_core-0.9.4.tar.gz` & `tmp/pypomes_core-0.9.5.tar.gz`

## Comparing `pypomes_core-0.9.4.tar` & `pypomes_core-0.9.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    24384 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.9.5/PKG-INFO
```

### Comparing `pypomes_core-0.9.4/src/pypomes_core/.ruff.toml` & `pypomes_core-0.9.5/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.4/src/pypomes_core/__init__.py` & `pypomes_core-0.9.5/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.4/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.9.5/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.4/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.9.5/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.4/src/pypomes_core/email_pomes.py` & `pypomes_core-0.9.5/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.4/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.9.5/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.4/src/pypomes_core/env_pomes.py` & `pypomes_core-0.9.5/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.4/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.9.5/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.4/src/pypomes_core/file_pomes.py` & `pypomes_core-0.9.5/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.4/src/pypomes_core/json_pomes.py` & `pypomes_core-0.9.5/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.4/src/pypomes_core/list_pomes.py` & `pypomes_core-0.9.5/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.4/src/pypomes_core/str_pomes.py` & `pypomes_core-0.9.5/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.4/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.9.5/src/pypomes_core/validation_msgs.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,17 +65,21 @@
         "en": "Invalid value {}: must be less than {}",
         "pt": "Valor {} inválido: deve ser menor que {}",
     },
     118: {
         "en": "Invalid value {}: must be greater than {}",
         "pt": "Valor {} inválido: deve ser maior que {}",
     },
+    119: {
+        "en": "Invalid value {}: {}",
+        "pt": "Valor {} inválido: {}",
+    },
     121: {
-        "en": "Invalid value {} {}",
-        "pt": "Valor {} inválido {}",
+        "en": "Invalid value {}",
+        "pt": "Valor {} inválido",
     },
     122: {
         "en": "Invalid value {}: length shorter than {}",
         "pt": "Valor {} inválido: comprimento menor que {}",
     },
     123: {
         "en": "Invalid value {}: length longer than {}",
```

### Comparing `pypomes_core-0.9.4/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.9.5/src/pypomes_core/validation_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,18 +533,14 @@
         elif isinstance(arg, str) and arg.startswith("@"):
             result += " " + arg
         elif isinstance(arg, str) and arg.find(" ") > 0:
             result = result.replace("{}", arg, 1)
         else:
             result = result.replace("{}", f"'{arg}'", 1)
 
-    # remove a trailing marker, if one exists
-    if result.endswith(" {}"):
-        result = result[:-3]
-
     return result
 
 
 def validate_format_errors(errors: list[str]) -> list[dict]:
     """
     Build and return a list of dicts from the list of errors *errors*.
```

### Comparing `pypomes_core-0.9.4/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.9.5/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.4/LICENSE` & `pypomes_core-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.4/pyproject.toml` & `pypomes_core-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.9.4"
+version = "0.9.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.9.4/PKG-INFO` & `pypomes_core-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.9.4
+Version: 0.9.5
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

