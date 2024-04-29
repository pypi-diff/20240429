# Comparing `tmp/mlops_ods-0.1.202404251341.tar.gz` & `tmp/mlops_ods-0.1.202404292030.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_ods-0.1.202404251341.tar", max compression
+gzip compressed data, was "mlops_ods-0.1.202404292030.tar", max compression
```

## Comparing `mlops_ods-0.1.202404251341.tar` & `mlops_ods-0.1.202404292030.tar`

### file list

```diff
@@ -1,19 +1,25 @@
--rw-r--r--   0        0        0      804 2024-04-25 13:40:46.554124 mlops_ods-0.1.202404251341/README.md
--rw-r--r--   0        0        0      785 2024-04-25 13:41:16.646138 mlops_ods-0.1.202404251341/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 13:40:46.586124 mlops_ods-0.1.202404251341/src/mlops_ods/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 13:40:46.586124 mlops_ods-0.1.202404251341/src/mlops_ods/app/__init__.py
--rw-r--r--   0        0        0       50 2024-04-25 13:40:46.586124 mlops_ods-0.1.202404251341/src/mlops_ods/app/example.py
--rw-r--r--   0        0        0       69 2024-04-25 13:40:46.590124 mlops_ods-0.1.202404251341/src/mlops_ods/conf/config.yaml
--rw-r--r--   0        0        0      287 2024-04-25 13:40:46.590124 mlops_ods-0.1.202404251341/src/mlops_ods/conf/features/features.yaml
--rw-r--r--   0        0        0      103 2024-04-25 13:40:46.590124 mlops_ods-0.1.202404251341/src/mlops_ods/conf/model/fast.yaml
--rw-r--r--   0        0        0      103 2024-04-25 13:40:46.590124 mlops_ods-0.1.202404251341/src/mlops_ods/conf/model/slow.yaml
--rw-r--r--   0        0        0      146 2024-04-25 13:40:46.590124 mlops_ods-0.1.202404251341/src/mlops_ods/conf/settings/predict.yaml
--rw-r--r--   0        0        0      183 2024-04-25 13:40:46.590124 mlops_ods-0.1.202404251341/src/mlops_ods/conf/settings/train.yaml
--rw-r--r--   0        0        0      702 2024-04-25 13:40:46.590124 mlops_ods-0.1.202404251341/src/mlops_ods/config.py
--rw-r--r--   0        0        0  9730898 2024-04-25 13:40:46.618124 mlops_ods-0.1.202404251341/src/mlops_ods/notebooks/eda.ipynb
--rw-r--r--   0        0        0    51114 2024-04-25 13:40:46.618124 mlops_ods-0.1.202404251341/src/mlops_ods/notebooks/model.ipynb
--rw-r--r--   0        0        0     2364 2024-04-25 13:40:46.618124 mlops_ods-0.1.202404251341/src/mlops_ods/train_predict.py
--rw-r--r--   0        0        0        0 2024-04-25 13:40:46.618124 mlops_ods-0.1.202404251341/src/mlops_ods/utils/__init__.py
--rw-r--r--   0        0        0     2262 2024-04-25 13:40:46.618124 mlops_ods-0.1.202404251341/src/mlops_ods/utils/utils_etl.py
--rw-r--r--   0        0        0     2138 2024-04-25 13:40:46.618124 mlops_ods-0.1.202404251341/src/mlops_ods/utils/utils_model.py
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 mlops_ods-0.1.202404251341/PKG-INFO
+-rw-r--r--   0        0        0     1015 2024-04-29 20:29:55.641301 mlops_ods-0.1.202404292030/README.md
+-rw-r--r--   0        0        0      785 2024-04-29 20:30:19.617339 mlops_ods-0.1.202404292030/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 20:29:55.673301 mlops_ods-0.1.202404292030/src/mlops_ods/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 20:29:55.673301 mlops_ods-0.1.202404292030/src/mlops_ods/app/__init__.py
+-rw-r--r--   0        0        0       50 2024-04-29 20:29:55.673301 mlops_ods-0.1.202404292030/src/mlops_ods/app/example.py
+-rw-r--r--   0        0        0       69 2024-04-29 20:29:55.673301 mlops_ods-0.1.202404292030/src/mlops_ods/conf/config.yaml
+-rw-r--r--   0        0        0      287 2024-04-29 20:29:55.673301 mlops_ods-0.1.202404292030/src/mlops_ods/conf/features/features.yaml
+-rw-r--r--   0        0        0      103 2024-04-29 20:29:55.673301 mlops_ods-0.1.202404292030/src/mlops_ods/conf/model/fast.yaml
+-rw-r--r--   0        0        0      103 2024-04-29 20:29:55.673301 mlops_ods-0.1.202404292030/src/mlops_ods/conf/model/slow.yaml
+-rw-r--r--   0        0        0      146 2024-04-29 20:29:55.673301 mlops_ods-0.1.202404292030/src/mlops_ods/conf/settings/predict.yaml
+-rw-r--r--   0        0        0      183 2024-04-29 20:29:55.673301 mlops_ods-0.1.202404292030/src/mlops_ods/conf/settings/train.yaml
+-rw-r--r--   0        0        0      702 2024-04-29 20:29:55.673301 mlops_ods-0.1.202404292030/src/mlops_ods/config.py
+-rw-r--r--   0        0        0  9730898 2024-04-29 20:29:55.701301 mlops_ods-0.1.202404292030/src/mlops_ods/notebooks/eda.ipynb
+-rw-r--r--   0        0        0    51114 2024-04-29 20:29:55.701301 mlops_ods-0.1.202404292030/src/mlops_ods/notebooks/model.ipynb
+-rw-r--r--   0        0        0     7740 2024-04-29 20:29:55.705301 mlops_ods-0.1.202404292030/src/mlops_ods/snakemake_scripts/dag.svg
+-rw-r--r--   0        0        0      647 2024-04-29 20:29:55.705301 mlops_ods-0.1.202404292030/src/mlops_ods/snakemake_scripts/model_fit.py
+-rw-r--r--   0        0        0      624 2024-04-29 20:29:55.705301 mlops_ods-0.1.202404292030/src/mlops_ods/snakemake_scripts/model_fit_bigger.py
+-rw-r--r--   0        0        0      268 2024-04-29 20:29:55.705301 mlops_ods-0.1.202404292030/src/mlops_ods/snakemake_scripts/preprocess_data_base.py
+-rw-r--r--   0        0        0     1046 2024-04-29 20:29:55.705301 mlops_ods-0.1.202404292030/src/mlops_ods/snakemake_scripts/preprocess_data_research.py
+-rw-r--r--   0        0        0      628 2024-04-29 20:29:55.705301 mlops_ods-0.1.202404292030/src/mlops_ods/snakemake_scripts/snakemake_steps.md
+-rw-r--r--   0        0        0     2364 2024-04-29 20:29:55.705301 mlops_ods-0.1.202404292030/src/mlops_ods/train_predict.py
+-rw-r--r--   0        0        0        0 2024-04-29 20:29:55.705301 mlops_ods-0.1.202404292030/src/mlops_ods/utils/__init__.py
+-rw-r--r--   0        0        0     2262 2024-04-29 20:29:55.705301 mlops_ods-0.1.202404292030/src/mlops_ods/utils/utils_etl.py
+-rw-r--r--   0        0        0     2138 2024-04-29 20:29:55.705301 mlops_ods-0.1.202404292030/src/mlops_ods/utils/utils_model.py
+-rw-r--r--   0        0        0     1855 1970-01-01 00:00:00.000000 mlops_ods-0.1.202404292030/PKG-INFO
```

### Comparing `mlops_ods-0.1.202404251341/README.md` & `mlops_ods-0.1.202404292030/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # MLOps ODS
 This project for ml model with MLOps instruments
 
-the methodology of repo (github flow - one main branch, and developing in other brunches):
+the methodology of repo (GitHub flow - one main branch, and developing in other brunches):
 - main branch: 'master'
 - other branches: 'fix-', 'feature-', 'model-', 'experiment-'
 
+```commandline
+poetry build --format=wheel
+```
+
 Docker image (build / run):
 ```commandline
 docker build . -t mlops_ods_image
 docker run -it mlops_ods_image /bin/bash
 ```
 build for linux:
 ```commandline
@@ -22,7 +26,16 @@
 documentation of jupyter notebooks with quarto:
 ```commandline
 quarto render
 
 quarto preview  src/mlops_ods/notebooks/eda.ipynb
 quarto render src/mlops_ods/notebooks/eda.ipynb --to html
 ```
+
+snakemake command inside docker:
+```commandline
+snakemake --cores 10
+snakemake --dag | dot -Tsvg > dag.svg
+
+docker ps
+docker cp <CONTAINER ID>:/app/dag.svg .
+```
```

### Comparing `mlops_ods-0.1.202404251341/pyproject.toml` & `mlops_ods-0.1.202404292030/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlops_ods"
-version = "0.1.202404251341"
+version = "0.1.202404292030"
 description = ""
 authors = ["Iuliia Fokina"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.2.2"
```

### Comparing `mlops_ods-0.1.202404251341/src/mlops_ods/config.py` & `mlops_ods-0.1.202404292030/src/mlops_ods/config.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202404251341/src/mlops_ods/notebooks/eda.ipynb` & `mlops_ods-0.1.202404292030/src/mlops_ods/notebooks/eda.ipynb`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202404251341/src/mlops_ods/notebooks/model.ipynb` & `mlops_ods-0.1.202404292030/src/mlops_ods/notebooks/model.ipynb`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202404251341/src/mlops_ods/train_predict.py` & `mlops_ods-0.1.202404292030/src/mlops_ods/train_predict.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202404251341/src/mlops_ods/utils/utils_etl.py` & `mlops_ods-0.1.202404292030/src/mlops_ods/utils/utils_etl.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202404251341/src/mlops_ods/utils/utils_model.py` & `mlops_ods-0.1.202404292030/src/mlops_ods/utils/utils_model.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202404251341/PKG-INFO` & `mlops_ods-0.1.202404292030/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops_ods
-Version: 0.1.202404251341
+Version: 0.1.202404292030
 Summary: 
 Author: Iuliia Fokina
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -20,18 +20,22 @@
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Description-Content-Type: text/markdown
 
 # MLOps ODS
 This project for ml model with MLOps instruments
 
-the methodology of repo (github flow - one main branch, and developing in other brunches):
+the methodology of repo (GitHub flow - one main branch, and developing in other brunches):
 - main branch: 'master'
 - other branches: 'fix-', 'feature-', 'model-', 'experiment-'
 
+```commandline
+poetry build --format=wheel
+```
+
 Docker image (build / run):
 ```commandline
 docker build . -t mlops_ods_image
 docker run -it mlops_ods_image /bin/bash
 ```
 build for linux:
 ```commandline
@@ -46,7 +50,16 @@
 ```commandline
 quarto render
 
 quarto preview  src/mlops_ods/notebooks/eda.ipynb
 quarto render src/mlops_ods/notebooks/eda.ipynb --to html
 ```
 
+snakemake command inside docker:
+```commandline
+snakemake --cores 10
+snakemake --dag | dot -Tsvg > dag.svg
+
+docker ps
+docker cp <CONTAINER ID>:/app/dag.svg .
+```
+
```

