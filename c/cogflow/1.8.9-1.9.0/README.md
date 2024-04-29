# Comparing `tmp/cogflow-1.8.9.tar.gz` & `tmp/cogflow-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogflow-1.8.9.tar", last modified: Wed Apr 24 08:59:08 2024, max compression
+gzip compressed data, was "cogflow-1.9.0.tar", last modified: Mon Apr 29 15:01:32 2024, max compression
```

## Comparing `cogflow-1.8.9.tar` & `cogflow-1.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 08:59:08.972492 cogflow-1.8.9/
--rw-rw-rw-   0        0        0      401 2024-04-24 08:59:08.968953 cogflow-1.8.9/PKG-INFO
--rw-rw-rw-   0        0        0     4024 2024-04-15 10:04:49.000000 cogflow-1.8.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 08:59:08.918280 cogflow-1.8.9/cogflow/
--rw-rw-rw-   0        0        0      729 2024-04-19 11:20:35.000000 cogflow-1.8.9/cogflow/__init__.py
--rw-rw-rw-   0        0        0     5495 2024-04-24 08:46:03.000000 cogflow-1.8.9/cogflow/dataset_plugin.py
--rw-rw-rw-   0        0        0     8953 2024-04-19 10:48:05.000000 cogflow-1.8.9/cogflow/kubeflowplugin.py
--rw-rw-rw-   0        0        0    11091 2024-04-24 08:11:12.000000 cogflow-1.8.9/cogflow/mlflowplugin.py
--rw-rw-rw-   0        0        0     3056 2024-04-24 08:54:37.000000 cogflow-1.8.9/cogflow/plugin_config.py
--rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.8.9/cogflow/plugin_status.py
--rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.8.9/cogflow/pluginerrors.py
--rw-rw-rw-   0        0        0    11063 2024-04-24 08:56:47.000000 cogflow-1.8.9/cogflow/pluginmanager.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:59:08.940042 cogflow-1.8.9/cogflow.egg-info/
--rw-rw-rw-   0        0        0      401 2024-04-24 08:59:08.000000 cogflow-1.8.9/cogflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-04-24 08:59:08.000000 cogflow-1.8.9/cogflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 08:59:08.000000 cogflow-1.8.9/cogflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2024-04-24 08:59:08.000000 cogflow-1.8.9/cogflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-24 08:59:08.000000 cogflow-1.8.9/cogflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 08:59:08.972492 cogflow-1.8.9/setup.cfg
--rw-rw-rw-   0        0        0     1646 2024-04-24 08:46:38.000000 cogflow-1.8.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:59:08.963721 cogflow-1.8.9/tests/
--rw-rw-rw-   0        0        0        0 2024-04-19 10:16:11.000000 cogflow-1.8.9/tests/__init__.py
--rw-rw-rw-   0        0        0    10080 2024-04-23 12:47:04.000000 cogflow-1.8.9/tests/test_dataset_plugin.py
--rw-rw-rw-   0        0        0     5369 2024-04-22 07:43:51.000000 cogflow-1.8.9/tests/test_kubeflowplugin.py
--rw-rw-rw-   0        0        0    14194 2024-04-23 12:47:04.000000 cogflow-1.8.9/tests/test_mlflowplugin.py
--rw-rw-rw-   0        0        0     7868 2024-04-23 12:47:04.000000 cogflow-1.8.9/tests/test_plugin_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:01:32.752730 cogflow-1.9.0/
+-rw-rw-rw-   0        0        0     4421 2024-04-29 15:01:32.739980 cogflow-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3266 2024-04-29 14:02:24.000000 cogflow-1.9.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 15:01:32.642263 cogflow-1.9.0/cogflow/
+-rw-rw-rw-   0        0        0     5163 2024-04-29 15:01:23.000000 cogflow-1.9.0/cogflow/__init__.py
+-rw-rw-rw-   0        0        0     5526 2024-04-29 11:24:36.000000 cogflow-1.9.0/cogflow/dataset_plugin.py
+-rw-rw-rw-   0        0        0     9770 2024-04-29 09:33:07.000000 cogflow-1.9.0/cogflow/kubeflowplugin.py
+-rw-rw-rw-   0        0        0    12971 2024-04-29 11:24:36.000000 cogflow-1.9.0/cogflow/mlflowplugin.py
+-rw-rw-rw-   0        0        0     3105 2024-04-27 05:28:26.000000 cogflow-1.9.0/cogflow/plugin_config.py
+-rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.9.0/cogflow/plugin_status.py
+-rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.9.0/cogflow/pluginerrors.py
+-rw-rw-rw-   0        0        0     9581 2024-04-27 05:28:26.000000 cogflow-1.9.0/cogflow/pluginmanager.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:01:32.676672 cogflow-1.9.0/cogflow.egg-info/
+-rw-rw-rw-   0        0        0     4421 2024-04-29 15:01:32.000000 cogflow-1.9.0/cogflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-04-29 15:01:32.000000 cogflow-1.9.0/cogflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 15:01:32.000000 cogflow-1.9.0/cogflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2024-04-29 15:01:32.000000 cogflow-1.9.0/cogflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-29 15:01:32.000000 cogflow-1.9.0/cogflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 15:01:32.752730 cogflow-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1868 2024-04-29 14:01:34.000000 cogflow-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:01:32.715689 cogflow-1.9.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-19 10:16:11.000000 cogflow-1.9.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    10088 2024-04-27 04:47:53.000000 cogflow-1.9.0/tests/test_dataset_plugin.py
+-rw-rw-rw-   0        0        0     5377 2024-04-27 04:47:53.000000 cogflow-1.9.0/tests/test_kubeflowplugin.py
+-rw-rw-rw-   0        0        0    14187 2024-04-29 11:23:09.000000 cogflow-1.9.0/tests/test_mlflowplugin.py
+-rw-rw-rw-   0        0        0     7877 2024-04-29 11:23:09.000000 cogflow-1.9.0/tests/test_plugin_manager.py
```

### Comparing `cogflow-1.8.9/cogflow/dataset_plugin.py` & `cogflow-1.9.0/cogflow/dataset_plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,109 +1,85 @@
 """
 This module provides functionality related to Dataset upload via plugin.
 """
-
 import io
 import os
-
 import requests
 from minio import Minio
-from . import plugin_config
+from . import plugin_config, PluginManager
 
 
 class DatasetPlugin:
     """
     A class to handle dataset-related operations.
-
     Attributes:
         None
     """
-
     def __init__(self):
         """
         Initializes DatasetPlugin with environment variables.
         """
         # Retrieve MinIO connection details from environment variables
         self.minio_endpoint = os.getenv(plugin_config.MINIO_ENDPOINT_URL)
         self.minio_access_key = os.getenv(plugin_config.MINIO_ACCESS_KEY)
         self.minio_secret_key = os.getenv(plugin_config.MINIO_SECRET_ACCESS_KEY)
-
-    @staticmethod
-    def version():
-        """
-        Retrieve the version of the DatasetPlugin.
-
-        Returns:
-            str: Version of the DatasetPlugin.
-        """
-        return None
-
-    def is_alive(self):
-        """
-        Check if DatasetPlugin is accessible.
-
-        Returns:
-            None
-        """
-        return None
+        self.section = "dataset_plugin"
 
     def create_minio_client(self):
         """
         Creates a MinIO client object.
-
         Returns:
             Minio: The MinIO client object.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(self.section)
         return Minio(
             self.minio_endpoint,
             access_key=self.minio_access_key,
             secret_key=self.minio_secret_key,
             secure=False,
         )  # Change to True if using HTTPS
 
     def query_endpoint_and_download_file(self, url, output_file, bucket_name):
         """
         Queries an endpoint and downloads a file from it.
-
         Args:
             url (str): The URL of the endpoint.
             output_file (str): The name of the output file to save.
-
         Returns:
             tuple: A tuple containing a boolean indicating success and the file URL if successful.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(self.section)
         try:
             response = requests.get(url)
             if response.status_code == 200:
                 self.save_to_minio(response.content, output_file, bucket_name)
                 return True
             print(f"Request failed with status code {response.status_code}")
             raise Exception("Request could not be successful due to error")
-
         except requests.exceptions.RequestException as exp:
             print(f"An error occurred: {exp}")
             raise Exception("Exception occurred during the requested operation")
 
     def save_to_minio(self, file_content, output_file, bucket_name):
         """
         Saves a file to MinIO.
-
         Args:
             file_content (bytes): The content of the file to be uploaded.
             output_file (str): The name of the file to be uploaded.
             bucket_name (str): The name of the bucket to upload the file to.
-
         Returns:
             str: The presigned URL of the uploaded file.
         """
-
+        # Verify plugin activation
+        PluginManager().verify_activation(self.section)
         # Initialize MinIO client
         minio_client = self.create_minio_client()
         object_name = output_file
-
         # Check if the bucket exists, if not, create it
         bucket_exists = minio_client.bucket_exists(bucket_name)
         if not bucket_exists:
             try:
                 minio_client.make_bucket(bucket_name)
                 print(f"Bucket '{bucket_name}' created successfully.")
             except Exception as exp:
@@ -128,25 +104,24 @@
         except Exception as err:
             print(f"Error uploading file: {err}")
             raise Exception(f"Error uploading file: {err}")
 
     def delete_from_minio(self, object_name, bucket_name):
         """
         Deletes a file from MinIO.
-
         Args:
             object_name (str): The name of the object (file) to be deleted.
             bucket_name (str): The name of the bucket containing the file.
-
         Returns:
             bool: True if the file was successfully deleted, False otherwise.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(self.section)
         # Initialize MinIO client
         minio_client = self.create_minio_client()
-
         try:
             # Check if the object exists
             object_exists = minio_client.stat_object(bucket_name, object_name)
             if object_exists:
                 # Delete the object from the bucket
                 minio_client.remove_object(bucket_name, object_name)
                 print(
```

### Comparing `cogflow-1.8.9/cogflow/kubeflowplugin.py` & `cogflow-1.9.0/cogflow/kubeflowplugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     V1beta1SKLearnSpec,
     constants,
     utils,
 )
 from kubernetes import client
 from kubernetes.client import V1ObjectMeta
 from kubernetes.client.models import V1EnvVar
-from . import plugin_config
+from . import plugin_config, PluginManager
 
 
 class CogContainer(kfp.dsl._container_op.Container):
     """
     Subclass of Container to add model access environment variables.
     """
 
@@ -38,14 +38,17 @@
     def add_model_access(self):
         """
         Adds model access environment variables to the container.
 
         Returns:
             CogContainer: Container instance with added environment variables.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
         return (
             self.add_env_variable(
                 V1EnvVar(
                     name=plugin_config.TRACKING_URI,
                     value=os.getenv(plugin_config.TRACKING_URI),
                 )
             )
@@ -82,46 +85,32 @@
         self.kfp = kfp
         self.kfp.dsl._container_op.Container.AddModelAccess = (
             CogContainer.add_model_access
         )
         self.kfp.dsl._container_op.ContainerOp.AddModelAccess = (
             CogContainer.add_model_access
         )
-
-    @staticmethod
-    def version():
-        """
-        Retrieve the version of the Kubeflow Pipelines SDK.
-
-        Returns:
-            str: Version of the Kubeflow Pipelines SDK.
-        """
-        return kfp.__version__
-
-    def is_alive(self):
-        """
-        Check if Kubeflow is accessible.
-
-        Returns:
-            None
-        """
-        return None
+        self.config_file_path = os.getenv(plugin_config.COGFLOW_CONFIG_FILE_PATH)
+        self.section = "kubeflow_plugin"
 
     @staticmethod
     def pipeline(name=None, description=None):
         """
         Decorator function to define Kubeflow Pipelines.
 
         Args:
             name (str, optional): Name of the pipeline. Defaults to None.
             description (str, optional): Description of the pipeline. Defaults to None.
 
         Returns:
             Callable: Decorator for defining Kubeflow Pipelines.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
         return dsl.pipeline(name=name, description=description)
 
     def create_component_from_func(
         self,
         func,
         output_component_file=None,
         base_image=None,
@@ -138,14 +127,17 @@
             packages_to_install (List[str], optional): List of additional Python packages
             to install in the component.
             Defaults to None.
 
         Returns:
             kfp.components.ComponentSpec: Component specification.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
         training_var = kfp.components.create_component_from_func(
             func=func,
             output_component_file=output_component_file,
             base_image=base_image,
             packages_to_install=packages_to_install,
         )
         self.kfp.dsl._container_op.ContainerOp.AddModelAccess = (
@@ -157,53 +149,65 @@
     def client():
         """
         Get the Kubeflow Pipeline client.
 
         Returns:
             kfp.Client: Kubeflow Pipeline client instance.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
         return kfp.Client()
 
     @staticmethod
     def load_component_from_url(url):
         """
         Load a component from a URL.
 
         Args:
             url (str): URL to load the component from.
 
         Returns:
             kfp.components.ComponentSpec: Loaded component specification.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
         return kfp.components.load_component_from_url(url)
 
     @staticmethod
     def input_path(label: str):
         """
         Create an InputPath component.
 
         Args:
             label (str): Label for the input path.
 
         Returns:
             InputPath: InputPath component instance.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
         return kfp.components.InputPath(label)
 
     @staticmethod
     def output_path(label: str):
         """
         Create an OutputPath component.
 
         Args:
             label (str): Label for the output path.
 
         Returns:
             OutputPath: OutputPath component instance.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
         return kfp.components.OutputPath(label)
 
     @staticmethod
     def serve_model_v2(model_uri: str, name: str = None):
         """
         Create a kserve instance.
 
@@ -211,14 +215,17 @@
             model_uri (str): URI of the model.
             name (str, optional): Name of the kserve instance. If not provided,
             a default name will be generated.
 
         Returns:
             None
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
         namespace = utils.get_default_target_namespace()
         if name is None:
             now = datetime.now()
             v = now.strftime("%d%M")
             name = f"predictor_model{v}"
         isvc_name = name
         predictor = V1beta1PredictorSpec(
@@ -256,14 +263,16 @@
             model_uri (str): URI of the model.
             name (str, optional): Name of the kserve instance. If not provided,
             a default name will be generated.
 
         Returns:
             None
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
 
         isvc_name = name
         namespace = utils.get_default_target_namespace()
         isvc = V1beta1InferenceService(
             api_version=constants.KSERVE_V1BETA1,
             kind=constants.KSERVE_KIND,
             metadata=V1ObjectMeta(
@@ -290,13 +299,16 @@
 
         Args:
             model_name (str): Name of the deployed model.
 
         Returns:
             str: URL of the deployed model.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
         kclient = KServeClient()
 
         time.sleep(plugin_config.TIMER_IN_SEC)
         isvc_resp = kclient.get(model_name)
         isvc_url = isvc_resp["status"]["address"]["url"]
         return isvc_url
```

### Comparing `cogflow-1.8.9/cogflow/mlflowplugin.py` & `cogflow-1.9.0/cogflow/mlflowplugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import pandas as pd
 import requests
 from mlflow.models.signature import ModelSignature
 from mlflow.tracking import MlflowClient
 from scipy.sparse import csr_matrix, csc_matrix
 
-from . import plugin_config
+from . import plugin_config, PluginManager
 
 
 class CogModel(ml.pyfunc.PythonModel):
     """
     A custom Mlflow PythonModel implementation for demonstration purposes.
     """
 
@@ -72,23 +72,28 @@
         self.mlflow = ml
         self.sklearn = ml.sklearn
         self.cogclient = MlflowClient()
         self.pyfunc = ml.pyfunc
         self.tensorflow = ml.tensorflow
         self.pytorch = ml.pytorch
         self.models = ml.models
+        self.config_file_path = os.getenv(plugin_config.COGFLOW_CONFIG_FILE_PATH)
+        self.section = "mlflow_plugin"
 
     def is_alive(self):
         """
         Check if Mlflow UI is accessible.
 
         Returns:
             tuple: A tuple containing a boolean indicating if Mlflow UI is accessible
              and the status code of the response.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
         try:
             response = requests.get(os.getenv(plugin_config.TRACKING_URI))
 
             if response.status_code == 200:
                 pass
             else:
                 print(
@@ -116,167 +121,209 @@
 
         Args:
             model_name (str): The name of the registered model to delete.
 
         Returns:
             bool: True if the model was successfully deleted, False otherwise.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
         return self.cogclient.delete_registered_model(model_name)
 
     def search_registered_models(self):
         """
         Searches for registered models.
 
         Returns:
             list: A list of registered model objects matching the search criteria.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
         registered_models = self.cogclient.search_registered_models()
         return registered_models
 
-    def load_model(self, model_name: str, model_version: int):
+    def load_model(self, model_uri: str, dst_path=None):
         """
-        Loads a model from Mlflow.
+        Loads a model from the specified Mlflow model URI.
 
         Args:
-            model_name (str): The name of the registered Mlflow model.
-            model_version (int): The version of the registered Mlflow model.
+            model_uri (str): The URI of the Mlflow model to load.
+            dst_path (str, optional): Optional path where the model will be downloaded and saved.
+             If not provided, the model will be loaded without saving.
 
         Returns:
-            loaded_model: The loaded model.
+            loaded_model: The loaded Mlflow model.
         """
-        model_uri = f"models:/{model_name}/{model_version}"
-        loaded_model = ml.sklearn.load_model(model_uri)
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        loaded_model = ml.sklearn.load_model(model_uri, dst_path)
         return loaded_model
 
     def register_model(self, model, model_uri):
         """
         Registers the given model with Mlflow.
 
         Args:
             model: The model object to register.
             model_uri (str): The Mlflow model URI.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
         return ml.register_model(model, model_uri)
 
     def autolog(self):
         """
         Enable automatic logging of parameters, metrics, and models with Mlflow.
 
         Returns:
             None
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
         return self.mlflow.autolog()
 
     def create_registered_model(self, name):
         """
         Create a registered model.
 
         Args:
             name (str): Name of the registered model.
 
         Returns:
             str: ID of the created registered model.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
         return self.cogclient.create_registered_model(name)
 
     def create_model_version(self, name, source):
         """
         Create a model version for a registered model.
 
         Args:
             name (str): Name of the registered model.
             source (str): Source path or URI of the model.
 
         Returns:
             str: ID of the created model version.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
         return self.cogclient.create_model_version(name, source)
 
     def set_tracking_uri(self, tracking_uri):
         """
         Set the Mlflow tracking URI.
 
         Args:
             tracking_uri (str): The URI of the Mlflow tracking server.
 
         Returns:
             None
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
         return self.mlflow.set_tracking_uri(tracking_uri)
 
     def set_experiment(self, experiment_name):
         """
-        Set the active MLflow experiment.
+        Set the active Mlflow experiment.
 
         Args:
             experiment_name (str): The name of the experiment to set as active.
 
         Returns:
             None
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
         return self.mlflow.set_experiment(experiment_name)
 
     def get_artifact_uri(self, run_id=None):
         """
         Get the artifact URI of the current or specified Mlflow run.
 
         Args:
             run_id (str, optional): ID of the Mlflow run. If not provided,
             the current run's artifact URI is returned.
 
         Returns:
             str: Artifact URI of the specified Mlflow run.
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
         return self.mlflow.get_artifact_uri(run_id)
 
     def start_run(self, run_name=None):
         """
         Start a Mlflow run.
 
         Args:
             run_name (str): Name of the Mlflow run.
 
         Returns:
             Mlflow Run object
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
         return self.mlflow.start_run(run_name=run_name)
 
     def end_run(self):
         """
         End a Mlflow run.
 
         Returns:
             Mlflow Run object
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
         return self.mlflow.end_run()
 
     def log_param(self, *args):
         """
         Log parameters to the Mlflow run.
 
         Args:
             run: Mlflow Run object returned by start_mlflow_run method.
             param: Containing parameters to log.
 
         Returns:
             None
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
         return self.mlflow.log_param(*args)
 
     def log_metric(self, *args):
         """
         Log metrics to the Mlflow run.
 
         Args:
             run: Mlflow Run object returned by start_mlflow_run method.
             metric: Containing metrics to log.
 
         Returns:
             None
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
         return self.mlflow.log_metric(*args)
 
     def log_model(
         self,
         sk_model,
         artifact_path,
         conda_env=None,
@@ -334,14 +381,17 @@
         Returns:
             Model: The logged scikit-learn model.
 
         Raises:
             Exception: If an error occurs during the logging process.
 
         """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
         return self.mlflow.sklearn.log_model(
             sk_model=sk_model,
             artifact_path=artifact_path,
             conda_env=conda_env,
             code_paths=code_paths,
             serialization_format=serialization_format,
             registered_model_name=registered_model_name,
```

### Comparing `cogflow-1.8.9/cogflow/plugin_config.py` & `cogflow-1.9.0/cogflow/plugin_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,18 +36,20 @@
      Used for accessing and storing data.
     MINIO_ACCESS_KEY (str): The access key for MinIO authentication. Used with
      MINIO_SECRET_ACCESS_KEY for secure access to MinIO.
     MINIO_SECRET_ACCESS_KEY (str): The secret access key for MinIO authentication. Combined with
      MINIO_ACCESS_KEY for secure access.
 """
 
+COGFLOW_CONFIG_FILE_PATH = "COGFLOW_CONFIG_FILE_PATH"
+
 TRACKING_URI = "MLFLOW_TRACKING_URI"
 S3_ENDPOINT_URL = "MLFLOW_S3_ENDPOINT_URL"
-ACCESS_KEY_ID = "AWS_ACCESS_KEY_ID"
-SECRET_ACCESS_KEY = "AWS_SECRET_ACCESS_KEY"
+ACCESS_KEY_ID = "ACCESS_KEY_ID"
+SECRET_ACCESS_KEY = "SECRET_ACCESS_KEY"
 TIMER_IN_SEC = 10
 ML_TOOL = "mlflow"
 
 ML_DB_USERNAME = "ML_DB_USERNAME"
 ML_DB_PASSWORD = "ML_DB_PASSWORD"
 ML_DB_HOST = "ML_DB_HOST"
 ML_DB_PORT = "ML_DB_PORT"
```

### Comparing `cogflow-1.8.9/cogflow/plugin_status.py` & `cogflow-1.9.0/cogflow/plugin_status.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.9/cogflow/pluginmanager.py` & `cogflow-1.9.0/cogflow/pluginmanager.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,30 +2,22 @@
 Plugin Manager Module
 
 This module provides a PluginManager class responsible for managing plugins such as MlflowPlugin,
 KubeflowPlugin, and DatasetPlugin.
 It also includes functions to activate, deactivate, and check the status of plugins.
 
 Attributes:
-    mlplugin (class): The Mlflow plugin class.
-    kfplugin (class): The Kubeflow plugin class.
-    dsplugin (class): The Dataset plugin class.
 """
 
-import importlib
+import os
 import pandas as pd
 from sqlalchemy import create_engine, Column, FLOAT, BIGINT, String
 from sqlalchemy.orm import declarative_base
 from . import plugin_config
-from .kubeflowplugin import KubeflowPlugin
-from .mlflowplugin import MlflowPlugin
-from .dataset_plugin import DatasetPlugin
-from . import plugin_status
-from .plugin_status import plugin_statuses
-
+import configparser
 
 Base = declarative_base()
 
 
 class ModelTraining(Base):
     """
     SQLAlchemy ORM class representing the 'Model_training' table in the PostgreSQL database.
@@ -60,171 +52,21 @@
 
 
 class PluginManager:
     """
     Class responsible for managing plugins.
 
     Attributes:
-        mlplugin (class): The Mlflow plugin class.
-        kfplugin (class): The Kubeflow plugin class.
-        dsplugin (class): The Dataset plugin class.
     """
 
     def __init__(self):
         """
         Initializes the PluginManager with plugin classes.
         """
-        self.mlplugin = MlflowPlugin
-        self.kfplugin = KubeflowPlugin
-        self.dsplugin = DatasetPlugin
-
-    @staticmethod
-    def plugin_names():
-        """
-        Returns a list of plugin names.
-
-        Returns:
-            list: A list of plugin names.
-        """
-        return ["MlflowPlugin", "KubeflowPlugin", "DatasetPlugin"]
-
-    def check_is_alive(self, name):
-        """
-        Checks if the plugin is alive.
-
-        Args:
-            name (str): The name of the plugin.
-
-        Returns:
-            tuple: A tuple containing the status and status code.
-        """
-        name.is_alive(self)
-
-    def version(self, name):
-        """
-        Gets the version of the plugin.
-
-        Args:
-            name (str): The name of the plugin.
-        """
-        name.version()
-
-    @staticmethod
-    def activate_all_plugins():
-        """
-        Activates all plugins.
-        """
-        plugins = PluginManager.plugin_names()
-        for plugin_name in plugins:
-            PluginManager.activate_plugin(plugin_name)
-
-    @staticmethod
-    def deactivate_all_plugins():
-        """
-        Deactivates all plugins.
-        """
-        plugins = PluginManager.plugin_names()
-        for plugin_name in plugins:
-            PluginManager.deactivate_plugin(plugin_name)
-
-    @staticmethod
-    def activate_plugin(name):
-        """
-        Activates a specific plugin.
-
-        Args:
-            name (str): The name of the plugin to activate.
-        """
-        if name not in plugin_statuses:
-            print(f"{name} does not exist.")
-            return
-        if plugin_statuses.get(name) == "activated":
-            print(f"{name} already in activated status")
-        else:
-            plugin_statuses[name] = "activated"
-            # Reload plugin_status module to reflect changes
-            importlib.reload(plugin_status)
-
-            updated_dict = plugin_status.plugin_statuses
-
-            updated_dict.update(plugin_statuses)
-
-            print(f"{name} is now {plugin_statuses.get(name)}")
-
-    @staticmethod
-    def deactivate_plugin(name):
-        """
-        Deactivates a specific plugin.
-
-        Args:
-            name (str): The name of the plugin to deactivate.
-        """
-        if name not in plugin_statuses:
-            print(f"{name} does not exist.")
-            return
-        if plugin_statuses.get(name) == "deactivated":
-            print(f"{name} already in deactivated status")
-        else:
-            plugin_statuses[name] = "deactivated"
-            # Reload plugin_status module to reflect changes
-            importlib.reload(plugin_status)
-
-            updated_dict = plugin_status.plugin_statuses
-
-            updated_dict.update(plugin_statuses)
-
-            print(f"{name} is now {plugin_statuses.get(name)}")
-
-    @staticmethod
-    def plugin_status():
-        """
-        Prints the status of all plugins.
-        """
-        print(plugin_statuses)
-
-    def get_plugin(self, name):
-        """
-        Gets a specific plugin.
-
-        Args:
-            name (str): The name of the plugin to get.
-        """
-        try:
-            PluginManager.version(self, name=name)
-            PluginManager.check_is_alive(self, name=name)
-        except Exception as e:
-            print(f"Plugin error : {e}")
-
-    def get_mlflow_plugin(self):
-        """
-        Gets the Mlflow plugin if activated.
-        """
-        if plugin_statuses.get("MlflowPlugin") == "activated":
-            # If activated, get the plugin
-            PluginManager.get_plugin(self, name=self.mlplugin)
-            return MlflowPlugin()
-        print("MlflowPlugin is in deactivated status")
-
-    def get_kflow_plugin(self):
-        """
-        Gets the Kubeflow plugin if activated.
-        """
-        if plugin_statuses.get("KubeflowPlugin") == "activated":
-            PluginManager.get_plugin(self, name=self.kfplugin)
-            return KubeflowPlugin()
-        print("KubeflowPlugin is in deactivated status")
-
-    def get_dataset_plugin(self):
-        """
-        Gets the Dataset plugin if activated.
-        """
-        if plugin_statuses.get("DatasetPlugin") == "activated":
-            PluginManager.get_plugin(self, name=self.dsplugin)
-            return DatasetPlugin()
-        print("DatasetPlugin is in deactivated status")
+        self.config_file_path = os.getenv(plugin_config.COGFLOW_CONFIG_FILE_PATH)
 
     def connect_to_cogflow_db(self, dialect="postgresql+psycopg2"):
         """
         Create and return an SQLAlchemy engine for a any database.
 
         Args:
             dialect (str): The connection string for the database. By default postgres DB
@@ -311,7 +153,86 @@
         JOIN metrics m ON p.run_uuid = m.run_uuid
         JOIN runs r ON p.run_uuid = r.run_uuid;
         """
         engine = self.connect_to_mlflow_db()
 
         df = pd.read_sql_query(metric_query, engine)
         return df
+
+    def get_config_value(self, config_file_path, section, key="activation_key"):
+        """
+        Reads the activation status of a plugin from an INI configuration file.
+
+        Args:
+            config_file_path (str): The path to the INI configuration file.
+            section (str): The section in the INI file that contains the plugin settings.
+            key (str, optional): The key used to store activation status in the section. Default is 'activation_key'.
+
+        Returns:
+            bool: True if the plugin is activated, False otherwise.
+            str or None: The value of the key if no exceptions occur and the plugin is activated.
+        """
+        if not config_file_path:
+            raise FileNotFoundError("Configuration file path not provided.")
+
+        # Create a ConfigParser instance
+        config = configparser.ConfigParser()
+
+        try:
+            # Read the INI configuration file
+            config.read(config_file_path)
+
+            # Check if the configuration file is empty or improperly formatted
+            if not config.sections():
+                raise Exception(
+                    "Configuration file is empty or not properly formatted."
+                )
+
+            # Check if the specified section exists in the configuration file
+            if section not in config:
+                raise KeyError(
+                    f"Section '{section}' not found in the configuration file. "
+                    f"Please correct section name in configuration file."
+                )
+
+            value = config.get(section, key, fallback=None)
+
+            # Check if the key value can be converted to boolean
+            if value is not None:
+                try:
+                    # Try to convert the value to boolean
+                    activation_status = config.getboolean(section, key, fallback=False)
+                    return activation_status
+                except ValueError:
+                    # If conversion to boolean fails, return the value as a string
+                    return value
+            else:
+                raise KeyError(
+                    f"Key '{key}' not found in section '{section}' of the configuration file."
+                    f" Please correct key name in configuration file"
+                )
+
+        except (FileNotFoundError, KeyError, Exception) as e:
+            # Stop execution immediately and raise the exception with a specific message
+            raise Exception(f"Error : {str(e)}")
+
+    def verify_activation(self, section):
+        """
+        Verify if the plugin is activated.
+
+        Raises:
+            Exception: If the plugin is not activated.
+        """
+        try:
+            # Call read_activation_status to check the activation status
+            activation_status = self.get_config_value(self.config_file_path, section)
+            # Raise an exception if the activation status is False
+            if not activation_status:
+                raise Exception(
+                    "Plugin is not activated. Please activate the plugin before performing this action."
+                )
+
+        except Exception as e:
+            error_message = f"{str(e)}"
+            # Log or print the error message if necessary
+            print(error_message)
+            raise
```

### Comparing `cogflow-1.8.9/setup.py` & `cogflow-1.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,27 @@
     classifiers (List[str]): A list of classifiers for the package.
     python_requires (str): The version of Python required by the package.
 
 """
 
 from setuptools import setup, find_packages
 
+# Read the content of your README file
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
 setup(
     name="cogflow",
-    version="1.8.9",
+    version="1.9.0",
     author="Sai_kireeti",
     author_email="sai.kireeti@hiro-microdatacenters.nl",
     description="cog modules",
     packages=find_packages(),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     install_requires=[
         "mlflow==2.10.2",
         "kfp==1.8.22",
         "boto3==1.34.73",
         "tenacity==8.2.3",
         "pandas==2.0.3",
         "numpy==1.24.3",
```

### Comparing `cogflow-1.8.9/tests/test_dataset_plugin.py` & `cogflow-1.9.0/tests/test_dataset_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 from unittest.mock import patch, MagicMock
 
 import minio
 import requests
 
-from cogflow.cogflow.dataset_plugin import DatasetPlugin
+from cogflow.cogflow.plugins.dataset_plugin import DatasetPlugin
 
 
 class TestDatasetPlugin(unittest.TestCase):
     @patch("requests.get")
     @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.save_to_minio")
     def test_query_endpoint_and_download_file_success(
         self, mock_save_to_minio, mock_requests_get
```

### Comparing `cogflow-1.8.9/tests/test_kubeflowplugin.py` & `cogflow-1.9.0/tests/test_kubeflowplugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import unittest
 from unittest.mock import patch, MagicMock
 
 from kubernetes.client.models import V1EnvVar
 
-from cogflow.cogflow.kubeflowplugin import KubeflowPlugin, CogContainer
+from cogflow.cogflow.plugins.kubeflowplugin import KubeflowPlugin, CogContainer
 from cogflow.cogflow import plugin_config
 
 
 class TestKubeflowPlugin(unittest.TestCase):
     def setUp(self):
         self.kfp_plugin = KubeflowPlugin()
```

### Comparing `cogflow-1.8.9/tests/test_mlflowplugin.py` & `cogflow-1.9.0/tests/test_mlflowplugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
     Test module for cases related to mlflow_plugin
 """
 
 import unittest
 from unittest.mock import patch, MagicMock
 from mlflow.exceptions import MlflowException
-from cogflow.cogflow.mlflowplugin import MlflowPlugin
+from cogflow.cogflow.model import MlflowPlugin
 
 
 class TestMlflowPlugin(unittest.TestCase):
     """
     Test Class for cases related to mlflow_plugin
     """
```

### Comparing `cogflow-1.8.9/tests/test_plugin_manager.py` & `cogflow-1.9.0/tests/test_plugin_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
     This file contains unittest for PluginManager methods
 """
 
 import unittest
 from io import StringIO
 from unittest.mock import patch
 from cogflow.cogflow.pluginmanager import PluginManager
-from cogflow.cogflow.mlflowplugin import MlflowPlugin
-from cogflow.cogflow.kubeflowplugin import KubeflowPlugin
-from cogflow.cogflow.dataset_plugin import DatasetPlugin
+from cogflow.cogflow.model import MlflowPlugin
+from cogflow.cogflow.plugins.kubeflowplugin import KubeflowPlugin
+from cogflow.cogflow.plugins.dataset_plugin import DatasetPlugin
 from cogflow.cogflow.plugin_status import plugin_statuses
 
 
 class TestPluginManager(unittest.TestCase):
     """
     Test class for PluginManger
     """
```

