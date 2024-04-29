# Comparing `tmp/ml_validation-0.0.2.tar.gz` & `tmp/ml_validation-0.0.3.tar.gz`

## Comparing `ml_validation-0.0.2.tar` & `ml_validation-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ml_validation-0.0.2/ml_validation/validation.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ml_validation-0.0.2/ml_validation/callable/dummy.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ml_validation-0.0.2/ml_validation/callable/torch.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 ml_validation-0.0.2/ml_validation/database/database.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 ml_validation-0.0.2/ml_validation/database/yadisk.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ml_validation-0.0.2/ml_validation/experiment/metrics.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 ml_validation-0.0.2/ml_validation/experiment/ptbxl.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 ml_validation-0.0.2/ml_validation/experiment/report.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 ml_validation-0.0.2/.gitignore
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ml_validation-0.0.2/README.md
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 ml_validation-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 ml_validation-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/validation.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/callable/dummy.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/callable/torch.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/database/database.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/database/yadisk.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/experiment/metrics.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/experiment/ptbxl.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 ml_validation-0.0.3/ml_validation/experiment/report.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 ml_validation-0.0.3/.gitignore
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ml_validation-0.0.3/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 ml_validation-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 ml_validation-0.0.3/PKG-INFO
```

### Comparing `ml_validation-0.0.2/ml_validation/database/database.py` & `ml_validation-0.0.3/ml_validation/database/database.py`

 * *Files identical despite different names*

### Comparing `ml_validation-0.0.2/ml_validation/database/yadisk.py` & `ml_validation-0.0.3/ml_validation/database/yadisk.py`

 * *Files identical despite different names*

### Comparing `ml_validation-0.0.2/ml_validation/experiment/metrics.py` & `ml_validation-0.0.3/ml_validation/experiment/metrics.py`

 * *Files identical despite different names*

### Comparing `ml_validation-0.0.2/ml_validation/experiment/ptbxl.py` & `ml_validation-0.0.3/ml_validation/experiment/ptbxl.py`

 * *Files identical despite different names*

### Comparing `ml_validation-0.0.2/ml_validation/experiment/report.py` & `ml_validation-0.0.3/ml_validation/experiment/report.py`

 * *Files identical despite different names*

### Comparing `ml_validation-0.0.2/.gitignore` & `ml_validation-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ml_validation-0.0.2/pyproject.toml` & `ml_validation-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -20,42 +20,42 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ml_validation"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Viktor Moskalenko", email="moskalenkoviktor@list.ru" },
 ]
 description = "Package for machine learning validation"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "requests==2.31.0",
-    "tqdm==4.66.2",
-    "numpy==1.26.4",
-    "pandas==2.2.2",
-    "scikit-learn==1.4.2"
+    "requests >=2.31.0,<3.0.0",
+    "tqdm >=4.66.0,<5.0.0",
+    "numpy >=1.26.0,<2.0.0",
+    "pandas >=2.2.0,<3.0.0",
+    "scikit-learn >=1.4.0,<2.0.0"
 ]
 
 [project.optional-dependencies]
 test = [
-    "mypy==1.10.0",
-    "flake8==7.0.0",
-    "Flake8-pyproject==1.2.3",
-    "flake8-quotes==3.4.0",
-    "isort==5.13.2",
-    "nbqa==1.8.5",
-    "types-requests==2.31.0"
+    "mypy >=1.10.0,<2.0.0",
+    "flake8 >=7.0.0,<8.0.0",
+    "Flake8-pyproject >=1.2.0,<2.0.0",
+    "flake8-quotes >=3.4.0,<4.0.0",
+    "isort >=5.13.0,<6.0.0",
+    "nbqa >=1.8.0,<2.0.0",
+    "types-requests >=2.31.0,<3.0.0"
 ]
 
 [project.urls]
 Homepage = "https://gitlab.com/moskalenkoviktor/ml_validation"
 Issues = "https://gitlab.com/moskalenkoviktor/ml_validation/-/issues"
 
 [tool.hatch.build.targets.wheel]
```

### Comparing `ml_validation-0.0.2/PKG-INFO` & `ml_validation-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.3
 Name: ml_validation
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for machine learning validation
 Project-URL: Homepage, https://gitlab.com/moskalenkoviktor/ml_validation
 Project-URL: Issues, https://gitlab.com/moskalenkoviktor/ml_validation/-/issues
 Author-email: Viktor Moskalenko <moskalenkoviktor@list.ru>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: numpy==1.26.4
-Requires-Dist: pandas==2.2.2
-Requires-Dist: requests==2.31.0
-Requires-Dist: scikit-learn==1.4.2
-Requires-Dist: tqdm==4.66.2
+Requires-Dist: numpy<2.0.0,>=1.26.0
+Requires-Dist: pandas<3.0.0,>=2.2.0
+Requires-Dist: requests<3.0.0,>=2.31.0
+Requires-Dist: scikit-learn<2.0.0,>=1.4.0
+Requires-Dist: tqdm<5.0.0,>=4.66.0
 Provides-Extra: test
-Requires-Dist: flake8-pyproject==1.2.3; extra == 'test'
-Requires-Dist: flake8-quotes==3.4.0; extra == 'test'
-Requires-Dist: flake8==7.0.0; extra == 'test'
-Requires-Dist: isort==5.13.2; extra == 'test'
-Requires-Dist: mypy==1.10.0; extra == 'test'
-Requires-Dist: nbqa==1.8.5; extra == 'test'
-Requires-Dist: types-requests==2.31.0; extra == 'test'
+Requires-Dist: flake8-pyproject<2.0.0,>=1.2.0; extra == 'test'
+Requires-Dist: flake8-quotes<4.0.0,>=3.4.0; extra == 'test'
+Requires-Dist: flake8<8.0.0,>=7.0.0; extra == 'test'
+Requires-Dist: isort<6.0.0,>=5.13.0; extra == 'test'
+Requires-Dist: mypy<2.0.0,>=1.10.0; extra == 'test'
+Requires-Dist: nbqa<2.0.0,>=1.8.0; extra == 'test'
+Requires-Dist: types-requests<3.0.0,>=2.31.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # ML Validation
 
 TODO: написать инструкцию
 
 # Check repo
```

