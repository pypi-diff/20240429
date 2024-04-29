# Comparing `tmp/shipyard_azureblob-0.2.0a2.tar.gz` & `tmp/shipyard_azureblob-0.2.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_azureblob-0.2.0a2.tar", max compression
+gzip compressed data, was "shipyard_azureblob-0.2.1a0.tar", max compression
```

## Comparing `shipyard_azureblob-0.2.0a2.tar` & `shipyard_azureblob-0.2.1a0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-07-24 19:47:59.855171 shipyard_azureblob-0.2.0a2/README.md
--rw-r--r--   0        0        0      544 2024-04-02 17:38:27.677828 shipyard_azureblob-0.2.0a2/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-12 18:48:21.823238 shipyard_azureblob-0.2.0a2/shipyard_azureblob/__init__.py
--rw-r--r--   0        0        0     9498 2024-04-01 13:13:53.708772 shipyard_azureblob-0.2.0a2/shipyard_azureblob/azureblob.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.431002 shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/__init__.py
--rw-r--r--   0        0        0      559 2024-03-14 04:10:25.267593 shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/authtest.py
--rw-r--r--   0        0        0     3914 2024-03-21 15:28:03.027401 shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/download.py
--rw-r--r--   0        0        0     3721 2024-03-14 04:10:25.268493 shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/move.py
--rw-r--r--   0        0        0     2173 2024-04-02 17:37:53.386191 shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/remove.py
--rw-r--r--   0        0        0     3838 2024-03-14 04:10:25.269404 shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/upload.py
--rw-r--r--   0        0        0     1644 2024-03-14 04:10:25.269708 shipyard_azureblob-0.2.0a2/shipyard_azureblob/exceptions.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 shipyard_azureblob-0.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 19:47:59.855171 shipyard_azureblob-0.2.1a0/README.md
+-rw-r--r--   0        0        0      544 2024-04-29 19:34:47.949482 shipyard_azureblob-0.2.1a0/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-12 18:48:21.823238 shipyard_azureblob-0.2.1a0/shipyard_azureblob/__init__.py
+-rw-r--r--   0        0        0     9482 2024-04-29 19:28:02.111488 shipyard_azureblob-0.2.1a0/shipyard_azureblob/azureblob.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.431002 shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/__init__.py
+-rw-r--r--   0        0        0      559 2024-03-14 04:10:25.267593 shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/authtest.py
+-rw-r--r--   0        0        0     3914 2024-03-21 15:28:03.027401 shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/download.py
+-rw-r--r--   0        0        0     3721 2024-03-14 04:10:25.268493 shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/move.py
+-rw-r--r--   0        0        0     2173 2024-04-18 20:05:24.170551 shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/remove.py
+-rw-r--r--   0        0        0     3837 2024-04-29 19:33:50.849788 shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/upload.py
+-rw-r--r--   0        0        0     1644 2024-03-14 04:10:25.269708 shipyard_azureblob-0.2.1a0/shipyard_azureblob/exceptions.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 shipyard_azureblob-0.2.1a0/PKG-INFO
```

### Comparing `shipyard_azureblob-0.2.0a2/pyproject.toml` & `shipyard_azureblob-0.2.1a0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "shipyard-azureblob"
-version = "0.2.0a2"
+version = "0.2.1a0"
 description = "A local client to connect with and work with Azure Blob"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_azureblob"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 azure-storage-blob = "^12.19.1"
-shipyard-bp-utils = "^1.1.1"
 shipyard-templates = "^0.7.0"
+shipyard-bp-utils = "^1.2.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shipyard_azureblob-0.2.0a2/shipyard_azureblob/azureblob.py` & `shipyard_azureblob-0.2.1a0/shipyard_azureblob/azureblob.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,18 +135,19 @@
             blob = self.container.get_blob_client(destination_full_path)
 
             with open(source_full_path, "rb") as data:
                 blob.upload_blob(data)
         except ExitCodeException:
             raise
         except ResourceExistsError as e:
-            raise exceptions.UploadError(
-                f"Failed to upload {source_full_path} to {self.container_name}/{destination_full_path}. "
-                f"File {destination_full_path} already exists in the container"
-            ) from e
+            logger.info(f'File "{destination_full_path}" already exists in the container. Overwriting...')
+            blob.delete_blob()
+            with open(source_full_path, "rb") as data:
+                blob.upload_blob(data)
+
         except Exception as e:
             raise exceptions.UploadError(
                 f"Failed to upload {source_full_path} to {self.container_name}/{destination_full_path}. "
                 f"Response from Azure: {e}"
             ) from e
 
         logger.info(
```

### Comparing `shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/authtest.py` & `shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/download.py` & `shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/download.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/move.py` & `shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/move.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/remove.py` & `shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/remove.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/upload.py` & `shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
         args = get_args()
         source_folder_name = args.source_folder_name
 
         destination_folder_name = shipyard.clean_folder_name(
             args.destination_folder_name
         )
         client = AzureBlobClient(args.connection_string, args.container_name)
-
         if args.source_file_name_match_type == "exact_match":
             source_full_path = shipyard.combine_folder_and_file_name(
                 folder_name=f"{os.getcwd()}/{source_folder_name}",
                 file_name=args.source_file_name,
             )
             destination_full_path = shipyard.determine_destination_full_path(
                 destination_folder_name=destination_folder_name,
```

### Comparing `shipyard_azureblob-0.2.0a2/shipyard_azureblob/exceptions.py` & `shipyard_azureblob-0.2.1a0/shipyard_azureblob/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.0a2/PKG-INFO` & `shipyard_azureblob-0.2.1a0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: shipyard-azureblob
-Version: 0.2.0a2
+Version: 0.2.1a0
 Summary: A local client to connect with and work with Azure Blob
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-storage-blob (>=12.19.1,<13.0.0)
-Requires-Dist: shipyard-bp-utils (>=1.1.1,<2.0.0)
+Requires-Dist: shipyard-bp-utils (>=1.2.1,<2.0.0)
 Requires-Dist: shipyard-templates (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
```

