# Comparing `tmp/ml_validation-0.0.3.tar.gz` & `tmp/ml_validation-0.0.4.tar.gz`

## Comparing `ml_validation-0.0.3.tar` & `ml_validation-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/validation.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/callable/dummy.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/callable/torch.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/database/database.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/database/yadisk.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/experiment/metrics.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/experiment/ptbxl.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/experiment/report.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 ml_validation-0.0.3/.gitignore
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ml_validation-0.0.3/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 ml_validation-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 ml_validation-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ml_validation-0.0.4/ml_validation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ml_validation-0.0.4/ml_validation/validation.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 ml_validation-0.0.4/ml_validation/callable/__init__.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ml_validation-0.0.4/ml_validation/callable/dummy.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ml_validation-0.0.4/ml_validation/callable/torch.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ml_validation-0.0.4/ml_validation/database/__init__.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 ml_validation-0.0.4/ml_validation/database/database.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 ml_validation-0.0.4/ml_validation/database/yadisk.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ml_validation-0.0.4/ml_validation/experiment/metrics.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 ml_validation-0.0.4/ml_validation/experiment/ptbxl.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 ml_validation-0.0.4/ml_validation/experiment/report.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 ml_validation-0.0.4/.gitignore
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ml_validation-0.0.4/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 ml_validation-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 ml_validation-0.0.4/PKG-INFO
```

### Comparing `ml_validation-0.0.3/ml_validation/database/database.py` & `ml_validation-0.0.4/ml_validation/database/database.py`

 * *Files identical despite different names*

### Comparing `ml_validation-0.0.3/ml_validation/database/yadisk.py` & `ml_validation-0.0.4/ml_validation/database/yadisk.py`

 * *Files identical despite different names*

### Comparing `ml_validation-0.0.3/ml_validation/experiment/metrics.py` & `ml_validation-0.0.4/ml_validation/experiment/metrics.py`

 * *Files identical despite different names*

### Comparing `ml_validation-0.0.3/ml_validation/experiment/ptbxl.py` & `ml_validation-0.0.4/ml_validation/experiment/ptbxl.py`

 * *Files identical despite different names*

### Comparing `ml_validation-0.0.3/ml_validation/experiment/report.py` & `ml_validation-0.0.4/ml_validation/experiment/report.py`

 * *Files identical despite different names*

### Comparing `ml_validation-0.0.3/.gitignore` & `ml_validation-0.0.4/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -155,10 +155,12 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
+# Package specific
 dataset/
 datasets/
-__*
+__*.json
+__*.ipynb
```

### Comparing `ml_validation-0.0.3/pyproject.toml` & `ml_validation-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ml_validation"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Viktor Moskalenko", email="moskalenkoviktor@list.ru" },
 ]
 description = "Package for machine learning validation"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `ml_validation-0.0.3/PKG-INFO` & `ml_validation-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ml_validation
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package for machine learning validation
 Project-URL: Homepage, https://gitlab.com/moskalenkoviktor/ml_validation
 Project-URL: Issues, https://gitlab.com/moskalenkoviktor/ml_validation/-/issues
 Author-email: Viktor Moskalenko <moskalenkoviktor@list.ru>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

