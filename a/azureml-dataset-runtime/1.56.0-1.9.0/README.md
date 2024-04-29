# Comparing `tmp/azureml_dataset_runtime-1.56.0-py3-none-any.whl.zip` & `tmp/azureml_dataset_runtime-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,9 @@
-Zip file size: 2258 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat      859 b- defN 24-Apr-29 18:32 azureml_dataset_runtime-1.56.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1248 b- defN 24-Apr-29 18:32 azureml_dataset_runtime-1.56.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-29 18:32 azureml_dataset_runtime-1.56.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-29 18:32 azureml_dataset_runtime-1.56.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      473 b- defN 24-Apr-29 18:32 azureml_dataset_runtime-1.56.0.dist-info/RECORD
-5 files, 2673 bytes uncompressed, 1360 bytes compressed:  49.1%
+Zip file size: 3195 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      120 b- defN 20-Jul-06 20:27 azureml_dataset_runtime-1.9.0.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat      859 b- defN 20-Jul-06 20:27 azureml_dataset_runtime-1.9.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      947 b- defN 20-Jul-06 20:27 azureml_dataset_runtime-1.9.0.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        1 b- defN 20-Jul-06 20:27 azureml_dataset_runtime-1.9.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 20-Jul-06 20:27 azureml_dataset_runtime-1.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1035 b- defN 20-Jul-06 20:27 azureml_dataset_runtime-1.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      695 b- defN 20-Jul-06 20:27 azureml_dataset_runtime-1.9.0.dist-info/RECORD
+7 files, 3754 bytes uncompressed, 1939 bytes compressed:  48.3%
```

## zipnote {}

```diff
@@ -1,16 +1,22 @@
-Filename: azureml_dataset_runtime-1.56.0.dist-info/LICENSE.txt
+Filename: azureml_dataset_runtime-1.9.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: azureml_dataset_runtime-1.56.0.dist-info/METADATA
+Filename: azureml_dataset_runtime-1.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_dataset_runtime-1.56.0.dist-info/WHEEL
+Filename: azureml_dataset_runtime-1.9.0.dist-info/metadata.json
 Comment: 
 
-Filename: azureml_dataset_runtime-1.56.0.dist-info/top_level.txt
+Filename: azureml_dataset_runtime-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_dataset_runtime-1.56.0.dist-info/RECORD
+Filename: azureml_dataset_runtime-1.9.0.dist-info/WHEEL
+Comment: 
+
+Filename: azureml_dataset_runtime-1.9.0.dist-info/METADATA
+Comment: 
+
+Filename: azureml_dataset_runtime-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `azureml_dataset_runtime-1.56.0.dist-info/LICENSE.txt` & `azureml_dataset_runtime-1.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_dataset_runtime-1.56.0.dist-info/METADATA` & `azureml_dataset_runtime-1.9.0.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-Metadata-Version: 2.1
-Name: azureml-dataset-runtime
-Version: 1.56.0
-Summary: The package is to coordinate dependencies within AzureML packages.     This package is internal, and is not intended to be used directly.
-Home-page: https://docs.microsoft.com/python/api/overview/azure/ml/?view=azure-ml-py
-Author: Microsoft Corp
-License: https://aka.ms/azureml-sdk-license
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: azureml-dataprep <5.2.0a,>=5.1.0a
-Requires-Dist: pyarrow >=0.17.0
-Requires-Dist: numpy !=1.19.3,<1.24 ; sys_platform == "linux"
-Requires-Dist: numpy !=1.19.4,<1.24 ; sys_platform == "win32"
-Provides-Extra: fuse
-Requires-Dist: fusepy <4.0.0,>=3.0.1 ; extra == 'fuse'
-Provides-Extra: pandas
-Requires-Dist: numpy <2.0.0,>=1.14.0 ; extra == 'pandas'
-Requires-Dist: pandas <2.0.0,>=0.23.4 ; extra == 'pandas'
-Provides-Extra: parquet
-Provides-Extra: pyspark
-Requires-Dist: pyspark ==2.3.0 ; extra == 'pyspark'
-Provides-Extra: scipy
-Requires-Dist: scipy <2.0.0,>=1.1.0 ; extra == 'scipy'
-
-# Azure Machine Learning SDK for Python
-
-The purpose of this package is to coordinate dependencies within AzureML packages. This package is internal, and is not intended to be used directly.
+Metadata-Version: 2.0
+Name: azureml-dataset-runtime
+Version: 1.9.0
+Summary: UNKNOWN
+Home-page: https://docs.microsoft.com/en-us/azure/machine-learning/service/
+Author: Microsoft Corp
+License: https://aka.ms/azureml-sdk-license
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+Provides-Extra: pyspark
+Provides-Extra: scipy
+Provides-Extra: parquet
+Provides-Extra: pandas
+Provides-Extra: fuse
+Requires-Dist: azureml-dataprep (~=1.9)
+Provides-Extra: fuse
+Requires-Dist: fusepy (>=3.0.1); extra == 'fuse'
+Provides-Extra: pandas
+Requires-Dist: numpy (>=1.14.0); extra == 'pandas'
+Requires-Dist: pandas (>=0.23.4); extra == 'pandas'
+Requires-Dist: pyarrow (>=0.15.*); extra == 'pandas'
+Provides-Extra: parquet
+Requires-Dist: pyarrow (>=0.15.*); extra == 'parquet'
+Provides-Extra: pyspark
+Requires-Dist: pyspark (==2.3.0); extra == 'pyspark'
+Provides-Extra: scipy
+Requires-Dist: scipy (>=1.1.0); extra == 'scipy'
+
+The purpose of this package is to coordinate dependencies within AzureML packages. It is not intended for public use.
+
+
```

