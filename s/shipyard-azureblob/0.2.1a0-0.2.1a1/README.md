# Comparing `tmp/shipyard_azureblob-0.2.1a0.tar.gz` & `tmp/shipyard_azureblob-0.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_azureblob-0.2.1a0.tar", max compression
+gzip compressed data, was "shipyard_azureblob-0.2.1a1.tar", max compression
```

## Comparing `shipyard_azureblob-0.2.1a0.tar` & `shipyard_azureblob-0.2.1a1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-07-24 19:47:59.855171 shipyard_azureblob-0.2.1a0/README.md
--rw-r--r--   0        0        0      544 2024-04-29 19:34:47.949482 shipyard_azureblob-0.2.1a0/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-12 18:48:21.823238 shipyard_azureblob-0.2.1a0/shipyard_azureblob/__init__.py
--rw-r--r--   0        0        0     9482 2024-04-29 19:28:02.111488 shipyard_azureblob-0.2.1a0/shipyard_azureblob/azureblob.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.431002 shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/__init__.py
--rw-r--r--   0        0        0      559 2024-03-14 04:10:25.267593 shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/authtest.py
--rw-r--r--   0        0        0     3914 2024-03-21 15:28:03.027401 shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/download.py
--rw-r--r--   0        0        0     3721 2024-03-14 04:10:25.268493 shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/move.py
--rw-r--r--   0        0        0     2173 2024-04-18 20:05:24.170551 shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/remove.py
--rw-r--r--   0        0        0     3837 2024-04-29 19:33:50.849788 shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/upload.py
--rw-r--r--   0        0        0     1644 2024-03-14 04:10:25.269708 shipyard_azureblob-0.2.1a0/shipyard_azureblob/exceptions.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 shipyard_azureblob-0.2.1a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 19:47:59.855171 shipyard_azureblob-0.2.1a1/README.md
+-rw-r--r--   0        0        0      544 2024-04-29 19:48:43.554157 shipyard_azureblob-0.2.1a1/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-12 18:48:21.823238 shipyard_azureblob-0.2.1a1/shipyard_azureblob/__init__.py
+-rw-r--r--   0        0        0     9482 2024-04-29 19:28:02.111488 shipyard_azureblob-0.2.1a1/shipyard_azureblob/azureblob.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.431002 shipyard_azureblob-0.2.1a1/shipyard_azureblob/cli/__init__.py
+-rw-r--r--   0        0        0      559 2024-03-14 04:10:25.267593 shipyard_azureblob-0.2.1a1/shipyard_azureblob/cli/authtest.py
+-rw-r--r--   0        0        0     3914 2024-03-21 15:28:03.027401 shipyard_azureblob-0.2.1a1/shipyard_azureblob/cli/download.py
+-rw-r--r--   0        0        0     3721 2024-03-14 04:10:25.268493 shipyard_azureblob-0.2.1a1/shipyard_azureblob/cli/move.py
+-rw-r--r--   0        0        0     2173 2024-04-29 19:45:09.995921 shipyard_azureblob-0.2.1a1/shipyard_azureblob/cli/remove.py
+-rw-r--r--   0        0        0     3837 2024-04-29 19:33:50.849788 shipyard_azureblob-0.2.1a1/shipyard_azureblob/cli/upload.py
+-rw-r--r--   0        0        0     1644 2024-03-14 04:10:25.269708 shipyard_azureblob-0.2.1a1/shipyard_azureblob/exceptions.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 shipyard_azureblob-0.2.1a1/PKG-INFO
```

### Comparing `shipyard_azureblob-0.2.1a0/pyproject.toml` & `shipyard_azureblob-0.2.1a1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "shipyard-azureblob"
-version = "0.2.1a0"
+version = "0.2.1a1"
 description = "A local client to connect with and work with Azure Blob"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_azureblob"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 azure-storage-blob = "^12.19.1"
-shipyard-templates = "^0.7.0"
 shipyard-bp-utils = "^1.2.1"
+shipyard-templates = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shipyard_azureblob-0.2.1a0/shipyard_azureblob/azureblob.py` & `shipyard_azureblob-0.2.1a1/shipyard_azureblob/azureblob.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/authtest.py` & `shipyard_azureblob-0.2.1a1/shipyard_azureblob/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/download.py` & `shipyard_azureblob-0.2.1a1/shipyard_azureblob/cli/download.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/move.py` & `shipyard_azureblob-0.2.1a1/shipyard_azureblob/cli/move.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/remove.py` & `shipyard_azureblob-0.2.1a1/shipyard_azureblob/cli/remove.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     elif args.source_file_name_match_type == "regex_match":
         file_names = client.find_blob_file_names(prefix=source_folder_name)
         matching_file_names = shipyard.find_all_file_matches(
             file_names, re.compile(args.source_file_name)
         )
         if number_of_matches := len(matching_file_names) == 0:
             logger.error("No file matches found")
-            sys.exit(client.EXIT_CODE_NO_MATCHES_FOUND)
+            sys.exit(client.EXIT_CODE_FILE_MATCH_ERROR)
 
         logger.info(f"{number_of_matches} files found. Preparing to delete...")
         for index, file_name in enumerate(matching_file_names, start=1):
             logger.info(f"Deleting file {index} of {number_of_matches}")
             client.remove(file_name=file_name)
```

### Comparing `shipyard_azureblob-0.2.1a0/shipyard_azureblob/cli/upload.py` & `shipyard_azureblob-0.2.1a1/shipyard_azureblob/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.1a0/shipyard_azureblob/exceptions.py` & `shipyard_azureblob-0.2.1a1/shipyard_azureblob/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.1a0/PKG-INFO` & `shipyard_azureblob-0.2.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-azureblob
-Version: 0.2.1a0
+Version: 0.2.1a1
 Summary: A local client to connect with and work with Azure Blob
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

