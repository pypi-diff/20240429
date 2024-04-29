# Comparing `tmp/dealcloud_sdk-0.1.1.tar.gz` & `tmp/dealcloud_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dealcloud_sdk-0.1.1.tar", max compression
+gzip compressed data, was "dealcloud_sdk-0.1.2.tar", max compression
```

## Comparing `dealcloud_sdk-0.1.1.tar` & `dealcloud_sdk-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      252 2024-03-14 12:12:18.117092 dealcloud_sdk-0.1.1/dealcloud_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-11-06 11:56:34.889796 dealcloud_sdk-0.1.1/dealcloud_sdk/base/__init__.py
--rw-r--r--   0        0        0     5656 2024-04-29 08:34:25.616882 dealcloud_sdk-0.1.1/dealcloud_sdk/base/dealcloud_base.py
--rw-r--r--   0        0        0        0 2023-11-07 09:28:04.246374 dealcloud_sdk-0.1.1/dealcloud_sdk/constants/__init__.py
--rw-r--r--   0        0        0       59 2023-10-04 16:21:51.277012 dealcloud_sdk-0.1.1/dealcloud_sdk/constants/auth.py
--rw-r--r--   0        0        0      121 2024-01-25 10:35:36.678604 dealcloud_sdk-0.1.1/dealcloud_sdk/constants/data.py
--rw-r--r--   0        0        0      129 2024-03-18 10:15:20.435449 dealcloud_sdk-0.1.1/dealcloud_sdk/constants/env_var_names.py
--rw-r--r--   0        0        0      174 2023-10-05 14:33:06.110575 dealcloud_sdk-0.1.1/dealcloud_sdk/constants/field_types.py
--rw-r--r--   0        0        0       70 2023-10-06 09:39:33.747233 dealcloud_sdk-0.1.1/dealcloud_sdk/constants/request.py
--rw-r--r--   0        0        0        0 2023-11-06 11:45:10.885728 dealcloud_sdk-0.1.1/dealcloud_sdk/data/__init__.py
--rw-r--r--   0        0        0    31181 2024-04-29 08:34:25.619882 dealcloud_sdk-0.1.1/dealcloud_sdk/data/dealcloud_data.py
--rw-r--r--   0        0        0      927 2024-01-31 14:27:15.843418 dealcloud_sdk-0.1.1/dealcloud_sdk/dealcloud.py
--rw-r--r--   0        0        0        0 2023-11-06 13:48:45.012295 dealcloud_sdk-0.1.1/dealcloud_sdk/factories/__init__.py
--rw-r--r--   0        0        0     1644 2024-03-18 10:17:02.976036 dealcloud_sdk-0.1.1/dealcloud_sdk/factories/from_env.py
--rw-r--r--   0        0        0      780 2024-01-31 14:27:15.946422 dealcloud_sdk-0.1.1/dealcloud_sdk/factories/from_json.py
--rw-r--r--   0        0        0      795 2024-01-31 14:27:15.935116 dealcloud_sdk-0.1.1/dealcloud_sdk/factories/from_yaml.py
--rw-r--r--   0        0        0        0 2023-10-04 13:19:31.316137 dealcloud_sdk-0.1.1/dealcloud_sdk/models/__init__.py
--rw-r--r--   0        0        0      241 2023-10-05 16:44:49.714586 dealcloud_sdk-0.1.1/dealcloud_sdk/models/auth.py
--rw-r--r--   0        0        0      155 2023-10-05 12:30:40.677272 dealcloud_sdk-0.1.1/dealcloud_sdk/models/data.py
--rw-r--r--   0        0        0      145 2023-11-06 14:40:22.072704 dealcloud_sdk-0.1.1/dealcloud_sdk/models/factory_models.py
--rw-r--r--   0        0        0     3608 2024-01-31 14:27:15.834092 dealcloud_sdk-0.1.1/dealcloud_sdk/models/schema.py
--rw-r--r--   0        0        0        0 2023-11-07 09:24:48.186581 dealcloud_sdk-0.1.1/dealcloud_sdk/schema/__init__.py
--rw-r--r--   0        0        0     5321 2024-01-31 14:27:15.930893 dealcloud_sdk-0.1.1/dealcloud_sdk/schema/dealcloud_schema.py
--rw-r--r--   0        0        0        0 2023-10-04 13:08:41.142141 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/__init__.py
--rw-r--r--   0        0        0      424 2023-10-10 09:54:28.814387 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/common_argument_parse.py
--rw-r--r--   0        0        0     2287 2024-01-31 14:27:15.880200 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/data_utils.py
--rw-r--r--   0        0        0      435 2023-10-04 13:11:34.863016 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/get_key.py
--rw-r--r--   0        0        0      366 2024-01-24 17:34:26.860779 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/process_response_errors.py
--rw-r--r--   0        0        0     5932 2024-02-13 10:13:00.411356 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/request_retry.py
--rw-r--r--   0        0        0      235 2023-10-06 13:40:35.214076 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/resolve_references.py
--rw-r--r--   0        0        0      331 2024-01-31 14:27:15.873919 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/validation.py
--rw-r--r--   0        0        0     9638 2024-04-29 08:40:01.855357 dealcloud_sdk-0.1.1/LICENSE
--rw-r--r--   0        0        0      861 2024-04-29 09:07:10.243665 dealcloud_sdk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    29075 2024-04-29 09:04:58.727112 dealcloud_sdk-0.1.1/README.md
--rw-r--r--   0        0        0    29079 1970-01-01 00:00:00.000000 dealcloud_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      252 2024-03-14 12:12:18.117092 dealcloud_sdk-0.1.2/dealcloud_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-06 11:56:34.889796 dealcloud_sdk-0.1.2/dealcloud_sdk/base/__init__.py
+-rw-r--r--   0        0        0     5656 2024-04-29 08:34:25.616882 dealcloud_sdk-0.1.2/dealcloud_sdk/base/dealcloud_base.py
+-rw-r--r--   0        0        0        0 2023-11-07 09:28:04.246374 dealcloud_sdk-0.1.2/dealcloud_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       59 2023-10-04 16:21:51.277012 dealcloud_sdk-0.1.2/dealcloud_sdk/constants/auth.py
+-rw-r--r--   0        0        0      121 2024-01-25 10:35:36.678604 dealcloud_sdk-0.1.2/dealcloud_sdk/constants/data.py
+-rw-r--r--   0        0        0      129 2024-03-18 10:15:20.435449 dealcloud_sdk-0.1.2/dealcloud_sdk/constants/env_var_names.py
+-rw-r--r--   0        0        0      174 2023-10-05 14:33:06.110575 dealcloud_sdk-0.1.2/dealcloud_sdk/constants/field_types.py
+-rw-r--r--   0        0        0       70 2023-10-06 09:39:33.747233 dealcloud_sdk-0.1.2/dealcloud_sdk/constants/request.py
+-rw-r--r--   0        0        0        0 2023-11-06 11:45:10.885728 dealcloud_sdk-0.1.2/dealcloud_sdk/data/__init__.py
+-rw-r--r--   0        0        0    31181 2024-04-29 08:34:25.619882 dealcloud_sdk-0.1.2/dealcloud_sdk/data/dealcloud_data.py
+-rw-r--r--   0        0        0      927 2024-01-31 14:27:15.843418 dealcloud_sdk-0.1.2/dealcloud_sdk/dealcloud.py
+-rw-r--r--   0        0        0        0 2023-11-06 13:48:45.012295 dealcloud_sdk-0.1.2/dealcloud_sdk/factories/__init__.py
+-rw-r--r--   0        0        0     1644 2024-03-18 10:17:02.976036 dealcloud_sdk-0.1.2/dealcloud_sdk/factories/from_env.py
+-rw-r--r--   0        0        0      780 2024-01-31 14:27:15.946422 dealcloud_sdk-0.1.2/dealcloud_sdk/factories/from_json.py
+-rw-r--r--   0        0        0      795 2024-01-31 14:27:15.935116 dealcloud_sdk-0.1.2/dealcloud_sdk/factories/from_yaml.py
+-rw-r--r--   0        0        0        0 2023-10-04 13:19:31.316137 dealcloud_sdk-0.1.2/dealcloud_sdk/models/__init__.py
+-rw-r--r--   0        0        0      241 2023-10-05 16:44:49.714586 dealcloud_sdk-0.1.2/dealcloud_sdk/models/auth.py
+-rw-r--r--   0        0        0      155 2023-10-05 12:30:40.677272 dealcloud_sdk-0.1.2/dealcloud_sdk/models/data.py
+-rw-r--r--   0        0        0      145 2023-11-06 14:40:22.072704 dealcloud_sdk-0.1.2/dealcloud_sdk/models/factory_models.py
+-rw-r--r--   0        0        0     3608 2024-01-31 14:27:15.834092 dealcloud_sdk-0.1.2/dealcloud_sdk/models/schema.py
+-rw-r--r--   0        0        0        0 2023-11-07 09:24:48.186581 dealcloud_sdk-0.1.2/dealcloud_sdk/schema/__init__.py
+-rw-r--r--   0        0        0     5321 2024-01-31 14:27:15.930893 dealcloud_sdk-0.1.2/dealcloud_sdk/schema/dealcloud_schema.py
+-rw-r--r--   0        0        0        0 2023-10-04 13:08:41.142141 dealcloud_sdk-0.1.2/dealcloud_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      424 2023-10-10 09:54:28.814387 dealcloud_sdk-0.1.2/dealcloud_sdk/utils/common_argument_parse.py
+-rw-r--r--   0        0        0     2287 2024-01-31 14:27:15.880200 dealcloud_sdk-0.1.2/dealcloud_sdk/utils/data_utils.py
+-rw-r--r--   0        0        0      435 2023-10-04 13:11:34.863016 dealcloud_sdk-0.1.2/dealcloud_sdk/utils/get_key.py
+-rw-r--r--   0        0        0      366 2024-01-24 17:34:26.860779 dealcloud_sdk-0.1.2/dealcloud_sdk/utils/process_response_errors.py
+-rw-r--r--   0        0        0     5932 2024-02-13 10:13:00.411356 dealcloud_sdk-0.1.2/dealcloud_sdk/utils/request_retry.py
+-rw-r--r--   0        0        0      235 2023-10-06 13:40:35.214076 dealcloud_sdk-0.1.2/dealcloud_sdk/utils/resolve_references.py
+-rw-r--r--   0        0        0      331 2024-01-31 14:27:15.873919 dealcloud_sdk-0.1.2/dealcloud_sdk/utils/validation.py
+-rw-r--r--   0        0        0     9638 2024-04-29 08:40:01.855357 dealcloud_sdk-0.1.2/LICENSE
+-rw-r--r--   0        0        0      861 2024-04-29 09:14:51.874272 dealcloud_sdk-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    29075 2024-04-29 09:13:45.565266 dealcloud_sdk-0.1.2/README.md
+-rw-r--r--   0        0        0    29079 1970-01-01 00:00:00.000000 dealcloud_sdk-0.1.2/PKG-INFO
```

### Comparing `dealcloud_sdk-0.1.1/dealcloud_sdk/base/dealcloud_base.py` & `dealcloud_sdk-0.1.2/dealcloud_sdk/base/dealcloud_base.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.1/dealcloud_sdk/data/dealcloud_data.py` & `dealcloud_sdk-0.1.2/dealcloud_sdk/data/dealcloud_data.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.1/dealcloud_sdk/dealcloud.py` & `dealcloud_sdk-0.1.2/dealcloud_sdk/dealcloud.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.1/dealcloud_sdk/factories/from_env.py` & `dealcloud_sdk-0.1.2/dealcloud_sdk/factories/from_env.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.1/dealcloud_sdk/factories/from_json.py` & `dealcloud_sdk-0.1.2/dealcloud_sdk/factories/from_json.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.1/dealcloud_sdk/factories/from_yaml.py` & `dealcloud_sdk-0.1.2/dealcloud_sdk/factories/from_yaml.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.1/dealcloud_sdk/models/schema.py` & `dealcloud_sdk-0.1.2/dealcloud_sdk/models/schema.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.1/dealcloud_sdk/schema/dealcloud_schema.py` & `dealcloud_sdk-0.1.2/dealcloud_sdk/schema/dealcloud_schema.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.1/dealcloud_sdk/utils/data_utils.py` & `dealcloud_sdk-0.1.2/dealcloud_sdk/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.1/dealcloud_sdk/utils/request_retry.py` & `dealcloud_sdk-0.1.2/dealcloud_sdk/utils/request_retry.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.1/LICENSE` & `dealcloud_sdk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.1/pyproject.toml` & `dealcloud_sdk-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dealcloud_sdk"
-version = "0.1.1"
+version = "0.1.2"
 description = "DealCloud SDK is a wrapper around the DealCloud API, designed to assist clients and partners to build on top of our platform quickly and easily."
 authors = ["Will James <will.james@intapp.com>"]
 readme = "README.md"
 packages = [{include = "dealcloud_sdk"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
```

### Comparing `dealcloud_sdk-0.1.1/README.md` & `dealcloud_sdk-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
          5. [Understanding Errors](#understanding-errors)
       4. [Delete Data](#delete-data) 
 
 # Installation
 ## pip
 Install using pip with:
 ```bash
-pip install dealcloud_sdk
+pip install dealcloud-sdk
 ```
 # Usage
 
 ## Creating a client and authenticating
 `dealcloud_sdk`'s main entrypoint is the `DealCloud` class. When it is instantiated, the object is scoped to a given DealCloud environment, by passing the site URL and API credentials as arguments:
 
 ```python
```

### Comparing `dealcloud_sdk-0.1.1/PKG-INFO` & `dealcloud_sdk-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dealcloud-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: DealCloud SDK is a wrapper around the DealCloud API, designed to assist clients and partners to build on top of our platform quickly and easily.
 Author: Will James
 Author-email: will.james@intapp.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -55,15 +55,15 @@
          5. [Understanding Errors](#understanding-errors)
       4. [Delete Data](#delete-data) 
 
 # Installation
 ## pip
 Install using pip with:
 ```bash
-pip install dealcloud_sdk
+pip install dealcloud-sdk
 ```
 # Usage
 
 ## Creating a client and authenticating
 `dealcloud_sdk`'s main entrypoint is the `DealCloud` class. When it is instantiated, the object is scoped to a given DealCloud environment, by passing the site URL and API credentials as arguments:
 
 ```python
```

