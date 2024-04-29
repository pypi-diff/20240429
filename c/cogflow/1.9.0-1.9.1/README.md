# Comparing `tmp/cogflow-1.9.0.tar.gz` & `tmp/cogflow-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogflow-1.9.0.tar", last modified: Mon Apr 29 15:01:32 2024, max compression
+gzip compressed data, was "cogflow-1.9.1.tar", last modified: Mon Apr 29 15:47:01 2024, max compression
```

## Comparing `cogflow-1.9.0.tar` & `cogflow-1.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 15:01:32.752730 cogflow-1.9.0/
--rw-rw-rw-   0        0        0     4421 2024-04-29 15:01:32.739980 cogflow-1.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     3266 2024-04-29 14:02:24.000000 cogflow-1.9.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 15:01:32.642263 cogflow-1.9.0/cogflow/
--rw-rw-rw-   0        0        0     5163 2024-04-29 15:01:23.000000 cogflow-1.9.0/cogflow/__init__.py
--rw-rw-rw-   0        0        0     5526 2024-04-29 11:24:36.000000 cogflow-1.9.0/cogflow/dataset_plugin.py
--rw-rw-rw-   0        0        0     9770 2024-04-29 09:33:07.000000 cogflow-1.9.0/cogflow/kubeflowplugin.py
--rw-rw-rw-   0        0        0    12971 2024-04-29 11:24:36.000000 cogflow-1.9.0/cogflow/mlflowplugin.py
--rw-rw-rw-   0        0        0     3105 2024-04-27 05:28:26.000000 cogflow-1.9.0/cogflow/plugin_config.py
--rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.9.0/cogflow/plugin_status.py
--rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.9.0/cogflow/pluginerrors.py
--rw-rw-rw-   0        0        0     9581 2024-04-27 05:28:26.000000 cogflow-1.9.0/cogflow/pluginmanager.py
-drwxrwxrwx   0        0        0        0 2024-04-29 15:01:32.676672 cogflow-1.9.0/cogflow.egg-info/
--rw-rw-rw-   0        0        0     4421 2024-04-29 15:01:32.000000 cogflow-1.9.0/cogflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-04-29 15:01:32.000000 cogflow-1.9.0/cogflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 15:01:32.000000 cogflow-1.9.0/cogflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2024-04-29 15:01:32.000000 cogflow-1.9.0/cogflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-29 15:01:32.000000 cogflow-1.9.0/cogflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 15:01:32.752730 cogflow-1.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1868 2024-04-29 14:01:34.000000 cogflow-1.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 15:01:32.715689 cogflow-1.9.0/tests/
--rw-rw-rw-   0        0        0        0 2024-04-19 10:16:11.000000 cogflow-1.9.0/tests/__init__.py
--rw-rw-rw-   0        0        0    10088 2024-04-27 04:47:53.000000 cogflow-1.9.0/tests/test_dataset_plugin.py
--rw-rw-rw-   0        0        0     5377 2024-04-27 04:47:53.000000 cogflow-1.9.0/tests/test_kubeflowplugin.py
--rw-rw-rw-   0        0        0    14187 2024-04-29 11:23:09.000000 cogflow-1.9.0/tests/test_mlflowplugin.py
--rw-rw-rw-   0        0        0     7877 2024-04-29 11:23:09.000000 cogflow-1.9.0/tests/test_plugin_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:47:01.686782 cogflow-1.9.1/
+-rw-rw-rw-   0        0        0     4421 2024-04-29 15:47:01.681199 cogflow-1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3266 2024-04-29 14:02:24.000000 cogflow-1.9.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 15:47:01.610095 cogflow-1.9.1/cogflow/
+-rw-rw-rw-   0        0        0     5559 2024-04-29 15:33:53.000000 cogflow-1.9.1/cogflow/__init__.py
+-rw-rw-rw-   0        0        0     5526 2024-04-29 11:24:36.000000 cogflow-1.9.1/cogflow/dataset_plugin.py
+-rw-rw-rw-   0        0        0     9770 2024-04-29 09:33:07.000000 cogflow-1.9.1/cogflow/kubeflowplugin.py
+-rw-rw-rw-   0        0        0    12971 2024-04-29 11:24:36.000000 cogflow-1.9.1/cogflow/mlflowplugin.py
+-rw-rw-rw-   0        0        0     3100 2024-04-29 15:35:25.000000 cogflow-1.9.1/cogflow/plugin_config.py
+-rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.9.1/cogflow/plugin_status.py
+-rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.9.1/cogflow/pluginerrors.py
+-rw-rw-rw-   0        0        0     9593 2024-04-29 15:44:34.000000 cogflow-1.9.1/cogflow/pluginmanager.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:47:01.636812 cogflow-1.9.1/cogflow.egg-info/
+-rw-rw-rw-   0        0        0     4421 2024-04-29 15:47:01.000000 cogflow-1.9.1/cogflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-04-29 15:47:01.000000 cogflow-1.9.1/cogflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 15:47:01.000000 cogflow-1.9.1/cogflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2024-04-29 15:47:01.000000 cogflow-1.9.1/cogflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-29 15:47:01.000000 cogflow-1.9.1/cogflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 15:47:01.686782 cogflow-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1868 2024-04-29 15:46:22.000000 cogflow-1.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:47:01.668236 cogflow-1.9.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-19 10:16:11.000000 cogflow-1.9.1/tests/__init__.py
+-rw-rw-rw-   0        0        0    10088 2024-04-27 04:47:53.000000 cogflow-1.9.1/tests/test_dataset_plugin.py
+-rw-rw-rw-   0        0        0     5377 2024-04-27 04:47:53.000000 cogflow-1.9.1/tests/test_kubeflowplugin.py
+-rw-rw-rw-   0        0        0    14187 2024-04-29 11:23:09.000000 cogflow-1.9.1/tests/test_mlflowplugin.py
+-rw-rw-rw-   0        0        0     7877 2024-04-29 11:23:09.000000 cogflow-1.9.1/tests/test_plugin_manager.py
```

### Comparing `cogflow-1.9.0/PKG-INFO` & `cogflow-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogflow
-Version: 1.9.0
+Version: 1.9.1
 Summary: cog modules
 Home-page: UNKNOWN
 Author: Sai_kireeti
 Author-email: sai.kireeti@hiro-microdatacenters.nl
 License: UNKNOWN
 Description: 
         # CogFlow
```

### Comparing `cogflow-1.9.0/README.md` & `cogflow-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.0/cogflow/__init__.py` & `cogflow-1.9.1/cogflow/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,32 +78,41 @@
 set_experiment = MlflowPlugin().set_experiment
 get_artifact_uri = MlflowPlugin().get_artifact_uri
 start_run = MlflowPlugin().start_run
 end_run = MlflowPlugin().end_run
 log_param = MlflowPlugin().log_param
 log_metric = MlflowPlugin().log_metric
 log_model = MlflowPlugin().log_model
+pyfunc = MlflowPlugin().pyfunc
+mlflow = MlflowPlugin().mlflow
+sklearn = MlflowPlugin().sklearn
+cogclient = MlflowPlugin().cogclient
+tensorflow = MlflowPlugin().tensorflow
+pytorch = MlflowPlugin().pytorch
+models = MlflowPlugin().models
+
 
 add_model_access = CogContainer().add_model_access
 pipeline = KubeflowPlugin().pipeline
 create_component_from_func = KubeflowPlugin().create_component_from_func
 client = KubeflowPlugin().client
 load_component_from_url = KubeflowPlugin().load_component_from_url
 input_path = KubeflowPlugin().input_path
 output_path = KubeflowPlugin().output_path
 serve_model_v2 = KubeflowPlugin().serve_model_v2
 serve_model_v1 = KubeflowPlugin().serve_model_v1
 get_model_url = KubeflowPlugin().get_model_url
+kfp = KubeflowPlugin().kfp
+
 
 create_minio_client = DatasetPlugin().create_minio_client
 query_endpoint_and_download_file = DatasetPlugin().query_endpoint_and_download_file
 save_to_minio = DatasetPlugin().save_to_minio
 delete_from_minio = DatasetPlugin().delete_from_minio
 
-
 __all__ = [
     # Methods from MlflowPlugin
     'delete_registered_model',
     'search_registered_models',
     'load_model',
     'register_model',
     'autolog',
@@ -113,29 +122,36 @@
     'set_experiment',
     'get_artifact_uri',
     'start_run',
     'end_run',
     'log_param',
     'log_metric',
     'log_model',
+    'pyfunc',
+    'mlflow',
+    'sklearn',
+    'cogclient',
+    'tensorflow',
+    'pytorch',
+    'models',
 
     # Method from CogContainer
     'add_model_access',
 
     # Methods from KubeflowPlugin
     'pipeline',
     'create_component_from_func',
     'client',
     'load_component_from_url',
     'input_path',
     'output_path',
     'serve_model_v2',
     'serve_model_v1',
     'get_model_url',
+    'kfp',
 
     # Methods from DatasetPlugin
     'create_minio_client',
     'query_endpoint_and_download_file',
     'save_to_minio',
     'delete_from_minio',
 ]
-
```

### Comparing `cogflow-1.9.0/cogflow/dataset_plugin.py` & `cogflow-1.9.1/cogflow/dataset_plugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.0/cogflow/kubeflowplugin.py` & `cogflow-1.9.1/cogflow/kubeflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.0/cogflow/mlflowplugin.py` & `cogflow-1.9.1/cogflow/mlflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.0/cogflow/plugin_config.py` & `cogflow-1.9.1/cogflow/plugin_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,10 +57,10 @@
 
 COGFLOW_DB_USERNAME = "DB_USER"
 COGFLOW_DB_PASSWORD = "DB_PASSWORD"
 COGFLOW_DB_HOST = "DB_HOST"
 COGFLOW_DB_PORT = "DB_PORT"
 COGFLOW_DB_NAME = "DB_NAME"
 
-MINIO_ENDPOINT_URL = "MINIO_ENDPOINT_URL"
-MINIO_ACCESS_KEY = "MINIO_ACCESS_KEY"
-MINIO_SECRET_ACCESS_KEY = "MINIO_SECRET_ACCESS_KEY"
+MINIO_ENDPOINT_URL = "MLFLOW_S3_ENDPOINT_URL"
+MINIO_ACCESS_KEY = "ACCESS_KEY_ID"
+MINIO_SECRET_ACCESS_KEY = "SECRET_ACCESS_KEY"
```

### Comparing `cogflow-1.9.0/cogflow/plugin_status.py` & `cogflow-1.9.1/cogflow/plugin_status.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.0/cogflow/pluginmanager.py` & `cogflow-1.9.1/cogflow/pluginmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     Attributes:
     """
 
     def __init__(self):
         """
         Initializes the PluginManager with plugin classes.
         """
-        self.config_file_path = os.getenv(plugin_config.COGFLOW_CONFIG_FILE_PATH)
+        self.config_file_path = os.path.join(os.path.dirname(__file__), 'cogflow_config.ini')
 
     def connect_to_cogflow_db(self, dialect="postgresql+psycopg2"):
         """
         Create and return an SQLAlchemy engine for a any database.
 
         Args:
             dialect (str): The connection string for the database. By default postgres DB
```

### Comparing `cogflow-1.9.0/cogflow.egg-info/PKG-INFO` & `cogflow-1.9.1/cogflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogflow
-Version: 1.9.0
+Version: 1.9.1
 Summary: cog modules
 Home-page: UNKNOWN
 Author: Sai_kireeti
 Author-email: sai.kireeti@hiro-microdatacenters.nl
 License: UNKNOWN
 Description: 
         # CogFlow
```

### Comparing `cogflow-1.9.0/setup.py` & `cogflow-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # Read the content of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="cogflow",
-    version="1.9.0",
+    version="1.9.1",
     author="Sai_kireeti",
     author_email="sai.kireeti@hiro-microdatacenters.nl",
     description="cog modules",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
```

### Comparing `cogflow-1.9.0/tests/test_dataset_plugin.py` & `cogflow-1.9.1/tests/test_dataset_plugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.0/tests/test_kubeflowplugin.py` & `cogflow-1.9.1/tests/test_kubeflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.0/tests/test_mlflowplugin.py` & `cogflow-1.9.1/tests/test_mlflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.0/tests/test_plugin_manager.py` & `cogflow-1.9.1/tests/test_plugin_manager.py`

 * *Files identical despite different names*

