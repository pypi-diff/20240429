# Comparing `tmp/dealcloud_sdk-0.1.0.tar.gz` & `tmp/dealcloud_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dealcloud_sdk-0.1.0.tar", max compression
+gzip compressed data, was "dealcloud_sdk-0.1.1.tar", max compression
```

## Comparing `dealcloud_sdk-0.1.0.tar` & `dealcloud_sdk-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      252 2024-03-14 12:12:18.117092 dealcloud_sdk-0.1.0/dealcloud_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-11-06 11:56:34.889796 dealcloud_sdk-0.1.0/dealcloud_sdk/base/__init__.py
--rw-r--r--   0        0        0     5656 2024-04-29 08:34:25.616882 dealcloud_sdk-0.1.0/dealcloud_sdk/base/dealcloud_base.py
--rw-r--r--   0        0        0        0 2023-11-07 09:28:04.246374 dealcloud_sdk-0.1.0/dealcloud_sdk/constants/__init__.py
--rw-r--r--   0        0        0       59 2023-10-04 16:21:51.277012 dealcloud_sdk-0.1.0/dealcloud_sdk/constants/auth.py
--rw-r--r--   0        0        0      121 2024-01-25 10:35:36.678604 dealcloud_sdk-0.1.0/dealcloud_sdk/constants/data.py
--rw-r--r--   0        0        0      129 2024-03-18 10:15:20.435449 dealcloud_sdk-0.1.0/dealcloud_sdk/constants/env_var_names.py
--rw-r--r--   0        0        0      174 2023-10-05 14:33:06.110575 dealcloud_sdk-0.1.0/dealcloud_sdk/constants/field_types.py
--rw-r--r--   0        0        0       70 2023-10-06 09:39:33.747233 dealcloud_sdk-0.1.0/dealcloud_sdk/constants/request.py
--rw-r--r--   0        0        0        0 2023-11-06 11:45:10.885728 dealcloud_sdk-0.1.0/dealcloud_sdk/data/__init__.py
--rw-r--r--   0        0        0    31181 2024-04-29 08:34:25.619882 dealcloud_sdk-0.1.0/dealcloud_sdk/data/dealcloud_data.py
--rw-r--r--   0        0        0      927 2024-01-31 14:27:15.843418 dealcloud_sdk-0.1.0/dealcloud_sdk/dealcloud.py
--rw-r--r--   0        0        0        0 2023-11-06 13:48:45.012295 dealcloud_sdk-0.1.0/dealcloud_sdk/factories/__init__.py
--rw-r--r--   0        0        0     1644 2024-03-18 10:17:02.976036 dealcloud_sdk-0.1.0/dealcloud_sdk/factories/from_env.py
--rw-r--r--   0        0        0      780 2024-01-31 14:27:15.946422 dealcloud_sdk-0.1.0/dealcloud_sdk/factories/from_json.py
--rw-r--r--   0        0        0      795 2024-01-31 14:27:15.935116 dealcloud_sdk-0.1.0/dealcloud_sdk/factories/from_yaml.py
--rw-r--r--   0        0        0        0 2023-10-04 13:19:31.316137 dealcloud_sdk-0.1.0/dealcloud_sdk/models/__init__.py
--rw-r--r--   0        0        0      241 2023-10-05 16:44:49.714586 dealcloud_sdk-0.1.0/dealcloud_sdk/models/auth.py
--rw-r--r--   0        0        0      155 2023-10-05 12:30:40.677272 dealcloud_sdk-0.1.0/dealcloud_sdk/models/data.py
--rw-r--r--   0        0        0      145 2023-11-06 14:40:22.072704 dealcloud_sdk-0.1.0/dealcloud_sdk/models/factory_models.py
--rw-r--r--   0        0        0     3608 2024-01-31 14:27:15.834092 dealcloud_sdk-0.1.0/dealcloud_sdk/models/schema.py
--rw-r--r--   0        0        0        0 2023-11-07 09:24:48.186581 dealcloud_sdk-0.1.0/dealcloud_sdk/schema/__init__.py
--rw-r--r--   0        0        0     5321 2024-01-31 14:27:15.930893 dealcloud_sdk-0.1.0/dealcloud_sdk/schema/dealcloud_schema.py
--rw-r--r--   0        0        0        0 2023-10-04 13:08:41.142141 dealcloud_sdk-0.1.0/dealcloud_sdk/utils/__init__.py
--rw-r--r--   0        0        0      424 2023-10-10 09:54:28.814387 dealcloud_sdk-0.1.0/dealcloud_sdk/utils/common_argument_parse.py
--rw-r--r--   0        0        0     2287 2024-01-31 14:27:15.880200 dealcloud_sdk-0.1.0/dealcloud_sdk/utils/data_utils.py
--rw-r--r--   0        0        0      435 2023-10-04 13:11:34.863016 dealcloud_sdk-0.1.0/dealcloud_sdk/utils/get_key.py
--rw-r--r--   0        0        0      366 2024-01-24 17:34:26.860779 dealcloud_sdk-0.1.0/dealcloud_sdk/utils/process_response_errors.py
--rw-r--r--   0        0        0     5932 2024-02-13 10:13:00.411356 dealcloud_sdk-0.1.0/dealcloud_sdk/utils/request_retry.py
--rw-r--r--   0        0        0      235 2023-10-06 13:40:35.214076 dealcloud_sdk-0.1.0/dealcloud_sdk/utils/resolve_references.py
--rw-r--r--   0        0        0      331 2024-01-31 14:27:15.873919 dealcloud_sdk-0.1.0/dealcloud_sdk/utils/validation.py
--rw-r--r--   0        0        0     9638 2024-04-29 08:40:01.855357 dealcloud_sdk-0.1.0/LICENSE
--rw-r--r--   0        0        0      861 2024-04-29 08:54:52.822422 dealcloud_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    29955 2024-01-31 14:38:33.384940 dealcloud_sdk-0.1.0/README.md
--rw-r--r--   0        0        0    29948 1970-01-01 00:00:00.000000 dealcloud_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      252 2024-03-14 12:12:18.117092 dealcloud_sdk-0.1.1/dealcloud_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-06 11:56:34.889796 dealcloud_sdk-0.1.1/dealcloud_sdk/base/__init__.py
+-rw-r--r--   0        0        0     5656 2024-04-29 08:34:25.616882 dealcloud_sdk-0.1.1/dealcloud_sdk/base/dealcloud_base.py
+-rw-r--r--   0        0        0        0 2023-11-07 09:28:04.246374 dealcloud_sdk-0.1.1/dealcloud_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       59 2023-10-04 16:21:51.277012 dealcloud_sdk-0.1.1/dealcloud_sdk/constants/auth.py
+-rw-r--r--   0        0        0      121 2024-01-25 10:35:36.678604 dealcloud_sdk-0.1.1/dealcloud_sdk/constants/data.py
+-rw-r--r--   0        0        0      129 2024-03-18 10:15:20.435449 dealcloud_sdk-0.1.1/dealcloud_sdk/constants/env_var_names.py
+-rw-r--r--   0        0        0      174 2023-10-05 14:33:06.110575 dealcloud_sdk-0.1.1/dealcloud_sdk/constants/field_types.py
+-rw-r--r--   0        0        0       70 2023-10-06 09:39:33.747233 dealcloud_sdk-0.1.1/dealcloud_sdk/constants/request.py
+-rw-r--r--   0        0        0        0 2023-11-06 11:45:10.885728 dealcloud_sdk-0.1.1/dealcloud_sdk/data/__init__.py
+-rw-r--r--   0        0        0    31181 2024-04-29 08:34:25.619882 dealcloud_sdk-0.1.1/dealcloud_sdk/data/dealcloud_data.py
+-rw-r--r--   0        0        0      927 2024-01-31 14:27:15.843418 dealcloud_sdk-0.1.1/dealcloud_sdk/dealcloud.py
+-rw-r--r--   0        0        0        0 2023-11-06 13:48:45.012295 dealcloud_sdk-0.1.1/dealcloud_sdk/factories/__init__.py
+-rw-r--r--   0        0        0     1644 2024-03-18 10:17:02.976036 dealcloud_sdk-0.1.1/dealcloud_sdk/factories/from_env.py
+-rw-r--r--   0        0        0      780 2024-01-31 14:27:15.946422 dealcloud_sdk-0.1.1/dealcloud_sdk/factories/from_json.py
+-rw-r--r--   0        0        0      795 2024-01-31 14:27:15.935116 dealcloud_sdk-0.1.1/dealcloud_sdk/factories/from_yaml.py
+-rw-r--r--   0        0        0        0 2023-10-04 13:19:31.316137 dealcloud_sdk-0.1.1/dealcloud_sdk/models/__init__.py
+-rw-r--r--   0        0        0      241 2023-10-05 16:44:49.714586 dealcloud_sdk-0.1.1/dealcloud_sdk/models/auth.py
+-rw-r--r--   0        0        0      155 2023-10-05 12:30:40.677272 dealcloud_sdk-0.1.1/dealcloud_sdk/models/data.py
+-rw-r--r--   0        0        0      145 2023-11-06 14:40:22.072704 dealcloud_sdk-0.1.1/dealcloud_sdk/models/factory_models.py
+-rw-r--r--   0        0        0     3608 2024-01-31 14:27:15.834092 dealcloud_sdk-0.1.1/dealcloud_sdk/models/schema.py
+-rw-r--r--   0        0        0        0 2023-11-07 09:24:48.186581 dealcloud_sdk-0.1.1/dealcloud_sdk/schema/__init__.py
+-rw-r--r--   0        0        0     5321 2024-01-31 14:27:15.930893 dealcloud_sdk-0.1.1/dealcloud_sdk/schema/dealcloud_schema.py
+-rw-r--r--   0        0        0        0 2023-10-04 13:08:41.142141 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      424 2023-10-10 09:54:28.814387 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/common_argument_parse.py
+-rw-r--r--   0        0        0     2287 2024-01-31 14:27:15.880200 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/data_utils.py
+-rw-r--r--   0        0        0      435 2023-10-04 13:11:34.863016 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/get_key.py
+-rw-r--r--   0        0        0      366 2024-01-24 17:34:26.860779 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/process_response_errors.py
+-rw-r--r--   0        0        0     5932 2024-02-13 10:13:00.411356 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/request_retry.py
+-rw-r--r--   0        0        0      235 2023-10-06 13:40:35.214076 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/resolve_references.py
+-rw-r--r--   0        0        0      331 2024-01-31 14:27:15.873919 dealcloud_sdk-0.1.1/dealcloud_sdk/utils/validation.py
+-rw-r--r--   0        0        0     9638 2024-04-29 08:40:01.855357 dealcloud_sdk-0.1.1/LICENSE
+-rw-r--r--   0        0        0      861 2024-04-29 09:07:10.243665 dealcloud_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    29075 2024-04-29 09:04:58.727112 dealcloud_sdk-0.1.1/README.md
+-rw-r--r--   0        0        0    29079 1970-01-01 00:00:00.000000 dealcloud_sdk-0.1.1/PKG-INFO
```

### Comparing `dealcloud_sdk-0.1.0/dealcloud_sdk/base/dealcloud_base.py` & `dealcloud_sdk-0.1.1/dealcloud_sdk/base/dealcloud_base.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.0/dealcloud_sdk/data/dealcloud_data.py` & `dealcloud_sdk-0.1.1/dealcloud_sdk/data/dealcloud_data.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.0/dealcloud_sdk/dealcloud.py` & `dealcloud_sdk-0.1.1/dealcloud_sdk/dealcloud.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.0/dealcloud_sdk/factories/from_env.py` & `dealcloud_sdk-0.1.1/dealcloud_sdk/factories/from_env.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.0/dealcloud_sdk/factories/from_json.py` & `dealcloud_sdk-0.1.1/dealcloud_sdk/factories/from_json.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.0/dealcloud_sdk/factories/from_yaml.py` & `dealcloud_sdk-0.1.1/dealcloud_sdk/factories/from_yaml.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.0/dealcloud_sdk/models/schema.py` & `dealcloud_sdk-0.1.1/dealcloud_sdk/models/schema.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.0/dealcloud_sdk/schema/dealcloud_schema.py` & `dealcloud_sdk-0.1.1/dealcloud_sdk/schema/dealcloud_schema.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.0/dealcloud_sdk/utils/data_utils.py` & `dealcloud_sdk-0.1.1/dealcloud_sdk/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.0/dealcloud_sdk/utils/request_retry.py` & `dealcloud_sdk-0.1.1/dealcloud_sdk/utils/request_retry.py`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.0/LICENSE` & `dealcloud_sdk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dealcloud_sdk-0.1.0/pyproject.toml` & `dealcloud_sdk-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dealcloud_sdk"
-version = "0.1.0"
+version = "0.1.1"
 description = "DealCloud SDK is a wrapper around the DealCloud API, designed to assist clients and partners to build on top of our platform quickly and easily."
 authors = ["Will James <will.james@intapp.com>"]
 readme = "README.md"
 packages = [{include = "dealcloud_sdk"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
```

### Comparing `dealcloud_sdk-0.1.0/README.md` & `dealcloud_sdk-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,1873 +1,1818 @@
-00000000: 215b 4465 616c 436c 6f75 645d 282f 6465  ![DealCloud](/de
-00000010: 616c 636c 6f75 642e 6a70 6729 0d0a 3c68  alcloud.jpg)..<h
-00000020: 313e 6465 616c 636c 6f75 645f 7364 6b3c  1>dealcloud_sdk<
-00000030: 2f68 313e 0d0a 3c70 2061 6c69 676e 3d22  /h1>..<p align="
-00000040: 6365 6e74 6572 223e 0d0a 3c61 2068 7265  center">..<a hre
-00000050: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000060: 622e 636f 6d2f 7073 662f 626c 6163 6b22  b.com/psf/black"
-00000070: 3e3c 696d 6720 616c 743d 2243 6f64 6520  ><img alt="Code 
-00000080: 7374 796c 653a 2062 6c61 636b 2220 7372  style: black" sr
-00000090: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-000000a0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-000000b0: 636f 6465 2532 3073 7479 6c65 2d62 6c61  code%20style-bla
-000000c0: 636b 2d30 3030 3030 302e 7376 6722 3e3c  ck-000000.svg"><
-000000d0: 2f61 3e0d 0a3c 696d 6720 7372 633d 2263  /a>..<img src="c
-000000e0: 6f76 6572 6167 652e 7376 6722 3e0d 0a3c  overage.svg">..<
-000000f0: 2f70 3e0d 0a0d 0a41 2077 7261 7070 6572  /p>....A wrapper
-00000100: 2061 726f 756e 6420 7468 6520 4465 616c   around the Deal
-00000110: 436c 6f75 6420 4150 492c 2064 6573 6967  Cloud API, desig
-00000120: 6e65 6420 746f 2061 7373 6973 7420 7573  ned to assist us
-00000130: 6572 732c 2063 6c69 656e 7473 2061 6e64  ers, clients and
-00000140: 2070 6172 746e 6572 7320 746f 2062 7569   partners to bui
-00000150: 6c64 206f 6e20 746f 7020 6f66 206f 7572  ld on top of our
-00000160: 2070 6c61 7466 6f72 6d27 7320 4150 492e   platform's API.
-00000170: 0d0a 0d0a 2320 436f 6e74 656e 7473 0d0a  ....# Contents..
-00000180: 312e 205b 496e 7374 616c 6c61 7469 6f6e  1. [Installation
-00000190: 5d28 2369 6e73 7461 6c6c 6174 696f 6e29  ](#installation)
-000001a0: 0d0a 2020 2031 2e20 5b57 6974 6820 7069  ..   1. [With pi
-000001b0: 705d 2823 7069 7029 0d0a 2020 2032 2e20  p](#pip)..   2. 
-000001c0: 5b4c 6f63 616c 6c79 5d28 2362 7569 6c64  [Locally](#build
-000001d0: 2d61 6e64 2d69 6e73 7461 6c6c 2d6c 6f63  -and-install-loc
-000001e0: 616c 6c79 290d 0a32 2e20 5b55 7361 6765  ally)..2. [Usage
-000001f0: 5d28 2375 7361 6765 290d 0a20 2020 312e  ](#usage)..   1.
-00000200: 205b 4372 6561 7469 6e67 2061 2063 6c69   [Creating a cli
-00000210: 656e 7420 616e 6420 6175 7468 656e 7469  ent and authenti
-00000220: 6361 7469 6e67 5d28 2363 7265 6174 696e  cating](#creatin
-00000230: 672d 612d 636c 6965 6e74 2d61 6e64 2d61  g-a-client-and-a
-00000240: 7574 6865 6e74 6963 6174 696e 6729 0d0a  uthenticating)..
-00000250: 2020 2032 2e20 5b53 6563 7572 656c 7920     2. [Securely 
-00000260: 6c6f 6164 696e 6720 6372 6564 656e 7469  loading credenti
-00000270: 616c 735d 2823 7365 6375 7265 6c79 2d6c  als](#securely-l
-00000280: 6f61 6469 6e67 2d63 7265 6465 6e74 6961  oading-credentia
-00000290: 6c73 290d 0a20 2020 2020 2031 2e20 5b55  ls)..      1. [U
-000002a0: 7369 6e67 2045 6e76 6972 6f6e 6d65 6e74  sing Environment
-000002b0: 2056 6172 6961 626c 6573 5d28 2375 7369   Variables](#usi
-000002c0: 6e67 2d65 6e76 6972 6f6e 6d65 6e74 2d76  ng-environment-v
-000002d0: 6172 6961 626c 6573 290d 0a20 2020 2020  ariables)..     
-000002e0: 2032 2e20 5b55 7369 6e67 204a 534f 4e20   2. [Using JSON 
-000002f0: 436f 6e66 6967 2046 696c 655d 2823 7573  Config File](#us
-00000300: 696e 672d 6a73 6f6e 2d63 6f6e 6669 672d  ing-json-config-
-00000310: 6669 6c65 290d 0a20 2020 2020 2033 2e20  file)..      3. 
-00000320: 5b55 7369 6e67 2059 414d 4c20 436f 6e66  [Using YAML Conf
-00000330: 6967 2046 696c 655d 2823 7573 696e 672d  ig File](#using-
-00000340: 7961 6d6c 2d63 6f6e 6669 672d 6669 6c65  yaml-config-file
-00000350: 290d 0a20 2020 332e 205b 5363 6865 6d61  )..   3. [Schema
-00000360: 2051 7565 7279 696e 675d 2823 7363 6865   Querying](#sche
-00000370: 6d61 2d71 7565 7279 696e 6729 0d0a 2020  ma-querying)..  
-00000380: 2020 2020 312e 205b 4765 7420 5573 6572      1. [Get User
-00000390: 735d 2823 6765 742d 7573 6572 7329 0d0a  s](#get-users)..
-000003a0: 2020 2020 2020 322e 205b 4765 7420 4375        2. [Get Cu
-000003b0: 7272 656e 6369 6573 5d28 2367 6574 2d63  rrencies](#get-c
-000003c0: 7572 7265 6e63 6965 7329 0d0a 2020 2020  urrencies)..    
-000003d0: 2020 332e 205b 4765 7420 4f62 6a65 6374    3. [Get Object
-000003e0: 735d 2823 6765 742d 6f62 6a65 6374 7329  s](#get-objects)
-000003f0: 0d0a 2020 2020 2020 342e 205b 4765 7420  ..      4. [Get 
-00000400: 4669 656c 6473 5d28 2367 6574 2d66 6965  Fields](#get-fie
-00000410: 6c64 7329 0d0a 2020 2020 2020 352e 205b  lds)..      5. [
-00000420: 4765 7420 5363 6865 6d61 5d28 2367 6574  Get Schema](#get
-00000430: 2d73 6368 656d 6129 0d0a 2020 2034 2e20  -schema)..   4. 
-00000440: 5b44 6174 6120 4f70 6572 6174 696f 6e73  [Data Operations
-00000450: 5d28 2364 6174 612d 6f70 6572 6174 696f  ](#data-operatio
-00000460: 6e73 290d 0a20 2020 2020 2031 2e20 5b4c  ns)..      1. [L
-00000470: 6973 7420 436f 6e66 6967 7572 6564 2056  ist Configured V
-00000480: 6965 7773 5d28 236c 6973 742d 636f 6e66  iews](#list-conf
-00000490: 6967 7572 6564 2d76 6965 7773 290d 0a20  igured-views).. 
-000004a0: 2020 2020 2032 2e20 5b52 6561 6420 4461       2. [Read Da
-000004b0: 7461 5d28 2372 6561 642d 6461 7461 290d  ta](#read-data).
-000004c0: 0a20 2020 2020 2020 2020 312e 205b 5265  .         1. [Re
+00000000: 3c68 313e 6465 616c 636c 6f75 645f 7364  <h1>dealcloud_sd
+00000010: 6b3c 2f68 313e 0d0a 0d0a 4120 7772 6170  k</h1>....A wrap
+00000020: 7065 7220 6172 6f75 6e64 2074 6865 2044  per around the D
+00000030: 6561 6c43 6c6f 7564 2041 5049 2c20 6465  ealCloud API, de
+00000040: 7369 676e 6564 2074 6f20 6173 7369 7374  signed to assist
+00000050: 2075 7365 7273 2c20 636c 6965 6e74 7320   users, clients 
+00000060: 616e 6420 7061 7274 6e65 7273 2074 6f20  and partners to 
+00000070: 6275 696c 6420 6f6e 2074 6f70 206f 6620  build on top of 
+00000080: 6f75 7220 706c 6174 666f 726d 2773 2041  our platform's A
+00000090: 5049 2e0d 0a0d 0a23 2043 6f6e 7465 6e74  PI.....# Content
+000000a0: 730d 0a31 2e20 5b49 6e73 7461 6c6c 6174  s..1. [Installat
+000000b0: 696f 6e5d 2823 696e 7374 616c 6c61 7469  ion](#installati
+000000c0: 6f6e 290d 0a20 2020 312e 205b 5769 7468  on)..   1. [With
+000000d0: 2070 6970 5d28 2370 6970 290d 0a20 2020   pip](#pip)..   
+000000e0: 322e 205b 4c6f 6361 6c6c 795d 2823 6275  2. [Locally](#bu
+000000f0: 696c 642d 616e 642d 696e 7374 616c 6c2d  ild-and-install-
+00000100: 6c6f 6361 6c6c 7929 0d0a 322e 205b 5573  locally)..2. [Us
+00000110: 6167 655d 2823 7573 6167 6529 0d0a 2020  age](#usage)..  
+00000120: 2031 2e20 5b43 7265 6174 696e 6720 6120   1. [Creating a 
+00000130: 636c 6965 6e74 2061 6e64 2061 7574 6865  client and authe
+00000140: 6e74 6963 6174 696e 675d 2823 6372 6561  nticating](#crea
+00000150: 7469 6e67 2d61 2d63 6c69 656e 742d 616e  ting-a-client-an
+00000160: 642d 6175 7468 656e 7469 6361 7469 6e67  d-authenticating
+00000170: 290d 0a20 2020 322e 205b 5365 6375 7265  )..   2. [Secure
+00000180: 6c79 206c 6f61 6469 6e67 2063 7265 6465  ly loading crede
+00000190: 6e74 6961 6c73 5d28 2373 6563 7572 656c  ntials](#securel
+000001a0: 792d 6c6f 6164 696e 672d 6372 6564 656e  y-loading-creden
+000001b0: 7469 616c 7329 0d0a 2020 2020 2020 312e  tials)..      1.
+000001c0: 205b 5573 696e 6720 456e 7669 726f 6e6d   [Using Environm
+000001d0: 656e 7420 5661 7269 6162 6c65 735d 2823  ent Variables](#
+000001e0: 7573 696e 672d 656e 7669 726f 6e6d 656e  using-environmen
+000001f0: 742d 7661 7269 6162 6c65 7329 0d0a 2020  t-variables)..  
+00000200: 2020 2020 322e 205b 5573 696e 6720 4a53      2. [Using JS
+00000210: 4f4e 2043 6f6e 6669 6720 4669 6c65 5d28  ON Config File](
+00000220: 2375 7369 6e67 2d6a 736f 6e2d 636f 6e66  #using-json-conf
+00000230: 6967 2d66 696c 6529 0d0a 2020 2020 2020  ig-file)..      
+00000240: 332e 205b 5573 696e 6720 5941 4d4c 2043  3. [Using YAML C
+00000250: 6f6e 6669 6720 4669 6c65 5d28 2375 7369  onfig File](#usi
+00000260: 6e67 2d79 616d 6c2d 636f 6e66 6967 2d66  ng-yaml-config-f
+00000270: 696c 6529 0d0a 2020 2033 2e20 5b53 6368  ile)..   3. [Sch
+00000280: 656d 6120 5175 6572 7969 6e67 5d28 2373  ema Querying](#s
+00000290: 6368 656d 612d 7175 6572 7969 6e67 290d  chema-querying).
+000002a0: 0a20 2020 2020 2031 2e20 5b47 6574 2055  .      1. [Get U
+000002b0: 7365 7273 5d28 2367 6574 2d75 7365 7273  sers](#get-users
+000002c0: 290d 0a20 2020 2020 2032 2e20 5b47 6574  )..      2. [Get
+000002d0: 2043 7572 7265 6e63 6965 735d 2823 6765   Currencies](#ge
+000002e0: 742d 6375 7272 656e 6369 6573 290d 0a20  t-currencies).. 
+000002f0: 2020 2020 2033 2e20 5b47 6574 204f 626a       3. [Get Obj
+00000300: 6563 7473 5d28 2367 6574 2d6f 626a 6563  ects](#get-objec
+00000310: 7473 290d 0a20 2020 2020 2034 2e20 5b47  ts)..      4. [G
+00000320: 6574 2046 6965 6c64 735d 2823 6765 742d  et Fields](#get-
+00000330: 6669 656c 6473 290d 0a20 2020 2020 2035  fields)..      5
+00000340: 2e20 5b47 6574 2053 6368 656d 615d 2823  . [Get Schema](#
+00000350: 6765 742d 7363 6865 6d61 290d 0a20 2020  get-schema)..   
+00000360: 342e 205b 4461 7461 204f 7065 7261 7469  4. [Data Operati
+00000370: 6f6e 735d 2823 6461 7461 2d6f 7065 7261  ons](#data-opera
+00000380: 7469 6f6e 7329 0d0a 2020 2020 2020 312e  tions)..      1.
+00000390: 205b 4c69 7374 2043 6f6e 6669 6775 7265   [List Configure
+000003a0: 6420 5669 6577 735d 2823 6c69 7374 2d63  d Views](#list-c
+000003b0: 6f6e 6669 6775 7265 642d 7669 6577 7329  onfigured-views)
+000003c0: 0d0a 2020 2020 2020 322e 205b 5265 6164  ..      2. [Read
+000003d0: 2044 6174 615d 2823 7265 6164 2d64 6174   Data](#read-dat
+000003e0: 6129 0d0a 2020 2020 2020 2020 2031 2e20  a)..         1. 
+000003f0: 5b52 6561 6469 6e67 2044 6174 6120 6672  [Reading Data fr
+00000400: 6f6d 2061 6e20 4f62 6a65 6374 5d28 2372  om an Object](#r
+00000410: 6561 6469 6e67 2d64 6174 612d 6672 6f6d  eading-data-from
+00000420: 2d61 6e2d 6f62 6a65 6374 290d 0a20 2020  -an-object)..   
+00000430: 2020 2020 2020 2020 2031 2e20 5b52 6573           1. [Res
+00000440: 6f6c 7669 6e67 2074 6f20 4e61 6d65 206f  olving to Name o
+00000450: 7220 746f 2049 445d 2823 7265 736f 6c76  r to ID](#resolv
+00000460: 696e 672d 746f 2d6e 616d 652d 6f72 2d74  ing-to-name-or-t
+00000470: 6f2d 6964 290d 0a20 2020 2020 2020 2020  o-id)..         
+00000480: 2020 2032 2e20 5b52 6561 6469 6e67 2061     2. [Reading a
+00000490: 2053 7562 7365 7420 6f66 2046 6965 6c64   Subset of Field
+000004a0: 735d 2823 7265 6164 696e 672d 612d 7375  s](#reading-a-su
+000004b0: 6273 6574 2d6f 662d 6669 656c 6473 290d  bset-of-fields).
+000004c0: 0a20 2020 2020 2020 2020 322e 205b 5265  .         2. [Re
 000004d0: 6164 696e 6720 4461 7461 2066 726f 6d20  ading Data from 
-000004e0: 616e 204f 626a 6563 745d 2823 7265 6164  an Object](#read
-000004f0: 696e 672d 6461 7461 2d66 726f 6d2d 616e  ing-data-from-an
-00000500: 2d6f 626a 6563 7429 0d0a 2020 2020 2020  -object)..      
-00000510: 2020 2020 2020 312e 205b 5265 736f 6c76        1. [Resolv
-00000520: 696e 6720 746f 204e 616d 6520 6f72 2074  ing to Name or t
-00000530: 6f20 4944 5d28 2372 6573 6f6c 7669 6e67  o ID](#resolving
-00000540: 2d74 6f2d 6e61 6d65 2d6f 722d 746f 2d69  -to-name-or-to-i
-00000550: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
-00000560: 322e 205b 5265 6164 696e 6720 6120 5375  2. [Reading a Su
-00000570: 6273 6574 206f 6620 4669 656c 6473 5d28  bset of Fields](
-00000580: 2372 6561 6469 6e67 2d61 2d73 7562 7365  #reading-a-subse
-00000590: 742d 6f66 2d66 6965 6c64 7329 0d0a 2020  t-of-fields)..  
-000005a0: 2020 2020 2020 2032 2e20 5b52 6561 6469         2. [Readi
-000005b0: 6e67 2044 6174 6120 6672 6f6d 2061 2056  ng Data from a V
-000005c0: 6965 775d 2823 7265 6164 696e 672d 6461  iew](#reading-da
-000005d0: 7461 2d66 726f 6d2d 612d 7669 6577 2920  ta-from-a-view) 
-000005e0: 0d0a 2020 2020 2020 2020 2020 2020 312e  ..            1.
-000005f0: 205b 5573 696e 6720 6120 4669 6c74 6572   [Using a Filter
-00000600: 2057 6865 6e20 5265 6164 696e 6720 5669   When Reading Vi
-00000610: 6577 2044 6174 615d 2823 7573 696e 672d  ew Data](#using-
-00000620: 612d 6669 6c74 6572 2d77 6865 6e2d 7265  a-filter-when-re
-00000630: 6164 696e 672d 7669 6577 2d64 6174 6129  ading-view-data)
-00000640: 200d 0a20 2020 2020 2033 2e20 5b43 7265   ..      3. [Cre
-00000650: 6174 652c 2055 7064 6174 652c 2055 7073  ate, Update, Ups
-00000660: 6572 7420 4461 7461 5d28 2363 7265 6174  ert Data](#creat
-00000670: 652d 7570 6461 7465 2d61 6e64 2d75 7073  e-update-and-ups
-00000680: 6572 742d 6461 7461 290d 0a20 2020 2020  ert-data)..     
-00000690: 2020 2020 312e 205b 4669 656c 6420 4d61      1. [Field Ma
-000006a0: 7070 696e 675d 2823 6669 656c 642d 6d61  pping](#field-ma
-000006b0: 7070 696e 6729 0d0a 2020 2020 2020 2020  pping)..        
-000006c0: 2032 2e20 5b43 7265 6174 6520 4461 7461   2. [Create Data
-000006d0: 5d28 2363 7265 6174 652d 6461 7461 290d  ](#create-data).
-000006e0: 0a20 2020 2020 2020 2020 332e 205b 5570  .         3. [Up
-000006f0: 6461 7465 2044 6174 615d 2823 7570 6461  date Data](#upda
-00000700: 7465 2d64 6174 6129 0d0a 2020 2020 2020  te-data)..      
-00000710: 2020 2034 2e20 5b55 7073 6572 7420 4461     4. [Upsert Da
-00000720: 7461 5d28 2375 7073 6572 742d 6461 7461  ta](#upsert-data
-00000730: 290d 0a20 2020 2020 2020 2020 352e 205b  )..         5. [
-00000740: 556e 6465 7273 7461 6e64 696e 6720 4572  Understanding Er
-00000750: 726f 7273 5d28 2375 6e64 6572 7374 616e  rors](#understan
-00000760: 6469 6e67 2d65 7272 6f72 7329 0d0a 2020  ding-errors)..  
-00000770: 2020 2020 342e 205b 4465 6c65 7465 2044      4. [Delete D
-00000780: 6174 615d 2823 6465 6c65 7465 2d64 6174  ata](#delete-dat
-00000790: 6129 200d 0a0d 0a23 2049 6e73 7461 6c6c  a) ....# Install
-000007a0: 6174 696f 6e0d 0a23 2320 7069 700d 0a49  ation..## pip..I
-000007b0: 6e73 7461 6c6c 2075 7369 6e67 2070 6970  nstall using pip
-000007c0: 2077 6974 683a 0d0a 6060 6062 6173 680d   with:..```bash.
-000007d0: 0a70 6970 2069 6e73 7461 6c6c 2064 6561  .pip install dea
-000007e0: 6c63 6c6f 7564 5f73 646b 0d0a 6060 600d  lcloud_sdk..```.
-000007f0: 0a23 2320 4275 696c 6420 616e 6420 696e  .## Build and in
-00000800: 7374 616c 6c20 6c6f 6361 6c6c 790d 0a60  stall locally..`
-00000810: 6465 616c 636c 6f75 645f 7364 6b60 2069  dealcloud_sdk` i
-00000820: 7320 6275 696c 7420 7573 696e 6720 5b70  s built using [p
-00000830: 6f65 7472 795d 2868 7474 7073 3a2f 2f70  oetry](https://p
-00000840: 7974 686f 6e2d 706f 6574 7279 2e6f 7267  ython-poetry.org
-00000850: 2f29 2c20 656e 7375 7265 2074 6861 7420  /), ensure that 
-00000860: 6974 2069 7320 696e 7374 616c 6c65 6420  it is installed 
-00000870: 6f6e 2079 6f75 7220 6d61 6368 696e 652e  on your machine.
-00000880: 0d0a 6060 6062 6173 680d 0a67 6974 2063  ..```bash..git c
-00000890: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
-000008a0: 6875 622e 636f 6d2f 7763 742d 6a61 6d65  hub.com/wct-jame
-000008b0: 732f 6465 616c 636c 6f75 645f 7364 6b2e  s/dealcloud_sdk.
-000008c0: 6769 740d 0a0d 0a63 6420 6465 616c 636c  git....cd dealcl
-000008d0: 6f75 645f 7364 6b0d 0a0d 0a70 6f65 7472  oud_sdk....poetr
-000008e0: 7920 696e 7374 616c 6c0d 0a0d 0a70 6f65  y install....poe
-000008f0: 7472 7920 6275 696c 640d 0a60 6060 0d0a  try build..```..
-00000900: 5468 6973 2077 696c 6c20 7072 6f64 7563  This will produc
-00000910: 6520 6120 7768 6565 6c20 282e 7768 6c29  e a wheel (.whl)
-00000920: 2066 696c 6520 696e 2074 6865 2060 6465   file in the `de
-00000930: 616c 636c 6f75 645f 7364 6b2f 6469 7374  alcloud_sdk/dist
-00000940: 6020 6469 7265 6374 6f72 792e 0d0a 546f  ` directory...To
-00000950: 2069 6e73 7461 6c6c 2074 6865 2070 6163   install the pac
-00000960: 6b61 6765 2066 726f 6d20 7468 6520 7768  kage from the wh
-00000970: 6565 6c2c 2069 6e20 616e 6f74 6865 7220  eel, in another 
-00000980: 7079 7468 6f6e 2070 726f 6a65 6374 3a0d  python project:.
-00000990: 0a60 6060 6261 7368 0d0a 7069 7020 696e  .```bash..pip in
-000009a0: 7374 616c 6c20 2270 6174 682f 746f 2f64  stall "path/to/d
-000009b0: 6561 6c63 6c6f 7564 5f73 646b 2f64 6973  ealcloud_sdk/dis
-000009c0: 742f 6465 616c 636c 6f75 645f 7364 6b2d  t/dealcloud_sdk-
-000009d0: 582e 592e 5a2d 6e6f 6e65 2d61 6e79 2e77  X.Y.Z-none-any.w
-000009e0: 686c 220d 0a60 6060 0d0a 7768 6572 6520  hl"..```..where 
-000009f0: 7468 6520 7061 7468 2069 7320 7468 6520  the path is the 
-00000a00: 6162 736f 6c75 7465 2070 6174 6820 746f  absolute path to
-00000a10: 2079 6f75 7220 2e77 686c 2066 696c 652e   your .whl file.
-00000a20: 0d0a 0d0a 0d0a 2320 5573 6167 650d 0a0d  ......# Usage...
-00000a30: 0a23 2320 4372 6561 7469 6e67 2061 2063  .## Creating a c
-00000a40: 6c69 656e 7420 616e 6420 6175 7468 656e  lient and authen
-00000a50: 7469 6361 7469 6e67 0d0a 6064 6561 6c63  ticating..`dealc
-00000a60: 6c6f 7564 5f73 646b 6027 7320 6d61 696e  loud_sdk`'s main
-00000a70: 2065 6e74 7279 706f 696e 7420 6973 2074   entrypoint is t
-00000a80: 6865 2060 4465 616c 436c 6f75 6460 2063  he `DealCloud` c
-00000a90: 6c61 7373 2e20 5768 656e 2069 7420 6973  lass. When it is
-00000aa0: 2069 6e73 7461 6e74 6961 7465 642c 2074   instantiated, t
-00000ab0: 6865 206f 626a 6563 7420 6973 2073 636f  he object is sco
-00000ac0: 7065 6420 746f 2061 2067 6976 656e 2044  ped to a given D
-00000ad0: 6561 6c43 6c6f 7564 2065 6e76 6972 6f6e  ealCloud environ
-00000ae0: 6d65 6e74 2c20 6279 2070 6173 7369 6e67  ment, by passing
-00000af0: 2074 6865 2073 6974 6520 5552 4c20 616e   the site URL an
-00000b00: 6420 4150 4920 6372 6564 656e 7469 616c  d API credential
-00000b10: 7320 6173 2061 7267 756d 656e 7473 3a0d  s as arguments:.
-00000b20: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
-00000b30: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
-00000b40: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
-00000b50: 640d 0a0d 0a64 6320 3d20 4465 616c 436c  d....dc = DealCl
-00000b60: 6f75 6428 0d0a 2020 2073 6974 655f 7572  oud(..   site_ur
-00000b70: 6c3d 2263 6c69 656e 742e 6465 616c 636c  l="client.dealcl
-00000b80: 6f75 642e 636f 6d22 2c0d 0a20 2020 636c  oud.com",..   cl
-00000b90: 6965 6e74 5f69 643d 2231 3233 3435 222c  ient_id="12345",
-00000ba0: 0d0a 2020 2063 6c69 656e 745f 7365 6372  ..   client_secr
-00000bb0: 6574 3d22 796f 7572 5f63 6c69 656e 745f  et="your_client_
-00000bc0: 7365 6372 6574 222c 0d0a 290d 0a60 6060  secret",..)..```
-00000bd0: 0d0a 0d0a 3e20 5b21 5741 524e 494e 475d  ....> [!WARNING]
-00000be0: 0d0a 3e20 5768 696c 7374 2073 7569 7461  ..> Whilst suita
-00000bf0: 626c 6520 666f 7220 6c6f 6361 6c20 6465  ble for local de
-00000c00: 7665 6c6f 706d 656e 742c 2074 6865 2061  velopment, the a
-00000c10: 626f 7665 2069 6d70 6c65 6d65 6e74 6174  bove implementat
-00000c20: 696f 6e20 6973 2069 6e73 6563 7572 6520  ion is insecure 
-00000c30: 6966 2079 6f75 206b 6565 7020 636f 6465  if you keep code
-00000c40: 2069 6e20 6f6e 6c69 6e65 2072 6570 6f73   in online repos
-00000c50: 6974 6f72 6965 7320 7375 6368 2061 7320  itories such as 
-00000c60: 4769 7448 7562 2e20 506c 6561 7365 2073  GitHub. Please s
-00000c70: 6565 2074 6865 2062 656c 6f77 2065 7861  ee the below exa
-00000c80: 6d70 6c65 7320 666f 7220 6d6f 7265 2073  mples for more s
-00000c90: 6563 7572 6520 696d 706c 656d 656e 7461  ecure implementa
-00000ca0: 7469 6f6e 732e 2020 0d0a 0d0a 2323 2053  tions.  ....## S
-00000cb0: 6563 7572 656c 7920 6c6f 6164 696e 6720  ecurely loading 
-00000cc0: 6372 6564 656e 7469 616c 730d 0a23 2323  credentials..###
-00000cd0: 2055 7369 6e67 2045 6e76 6972 6f6e 6d65   Using Environme
-00000ce0: 6e74 2056 6172 6961 626c 6573 0d0a 5768  nt Variables..Wh
-00000cf0: 6572 6520 7468 6520 656e 7669 726f 6e6d  ere the environm
-00000d00: 656e 7420 7661 7269 6162 6c65 7320 636f  ent variables co
-00000d10: 6e74 6169 6e20 7468 6520 7265 6c65 7661  ntain the releva
-00000d20: 6e74 2076 616c 7565 732e 2054 6865 7365  nt values. These
-00000d30: 2063 616e 2062 6520 6c6f 6164 6564 2066   can be loaded f
-00000d40: 726f 6d20 6120 2e65 6e76 2066 696c 6520  rom a .env file 
-00000d50: 7573 696e 6720 7468 6520 6070 7974 686f  using the `pytho
-00000d60: 6e2d 646f 7465 6e76 6020 5b50 7950 6920  n-dotenv` [PyPi 
-00000d70: 7061 636b 6167 655d 2868 7474 7073 3a2f  package](https:/
-00000d80: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000d90: 742f 7079 7468 6f6e 2d64 6f74 656e 762f  t/python-dotenv/
-00000da0: 292e 0d0a 0d0a 6060 6070 7974 686f 6e0d  ).....```python.
-00000db0: 0a66 726f 6d20 6465 616c 636c 6f75 645f  .from dealcloud_
-00000dc0: 7364 6b20 696d 706f 7274 2044 6561 6c43  sdk import DealC
-00000dd0: 6c6f 7564 0d0a 6672 6f6d 206f 7320 696d  loud..from os im
-00000de0: 706f 7274 2067 6574 656e 760d 0a0d 0a64  port getenv....d
-00000df0: 6320 3d20 4465 616c 436c 6f75 6428 0d0a  c = DealCloud(..
-00000e00: 2020 2020 7369 7465 5f75 726c 3d67 6574      site_url=get
-00000e10: 656e 7628 2244 435f 4554 4c5f 5349 5445  env("DC_ETL_SITE
-00000e20: 5f55 524c 2229 2c0d 0a20 2020 2063 6c69  _URL"),..    cli
-00000e30: 656e 745f 6964 3d67 6574 656e 7628 2244  ent_id=getenv("D
-00000e40: 435f 4554 4c5f 434c 4945 4e54 5f49 4422  C_ETL_CLIENT_ID"
-00000e50: 292c 0d0a 2020 2020 636c 6965 6e74 5f73  ),..    client_s
-00000e60: 6563 7265 743d 6765 7465 6e76 2822 4443  ecret=getenv("DC
-00000e70: 5f45 544c 5f41 5049 5f4b 4559 2229 2c0d  _ETL_API_KEY"),.
-00000e80: 0a29 0d0a 6060 600d 0a23 2323 2055 7369  .)..```..### Usi
-00000e90: 6e67 204a 534f 4e20 436f 6e66 6967 2046  ng JSON Config F
-00000ea0: 696c 650d 0a47 6976 656e 2061 204a 534f  ile..Given a JSO
-00000eb0: 4e20 6669 6c65 2069 6e20 7468 6520 6265  N file in the be
-00000ec0: 6c6f 7720 666f 726d 6174 3a0d 0a60 6060  low format:..```
-00000ed0: 6a73 6f6e 0d0a 7b0d 0a20 2022 7369 7465  json..{..  "site
-00000ee0: 5f75 726c 223a 2022 636c 6965 6e74 2e64  _url": "client.d
-00000ef0: 6561 6c63 6c6f 7564 2e63 6f6d 222c 0d0a  ealcloud.com",..
-00000f00: 2020 2263 6c69 656e 745f 6964 223a 2031    "client_id": 1
-00000f10: 3233 3435 2c0d 0a20 2022 636c 6965 6e74  2345,..  "client
-00000f20: 5f73 6563 7265 7422 3a20 2279 6f75 725f  _secret": "your_
-00000f30: 636c 6965 6e74 5f73 6563 7265 7422 0d0a  client_secret"..
-00000f40: 7d0d 0a60 6060 0d0a 5468 6520 4465 616c  }..```..The Deal
-00000f50: 436c 6f75 6420 6f62 6a65 6374 2063 616e  Cloud object can
-00000f60: 2062 6520 6372 6561 7465 6420 6173 2062   be created as b
-00000f70: 656c 6f77 3a0d 0a0d 0a60 6060 7079 7468  elow:....```pyth
-00000f80: 6f6e 0d0a 6672 6f6d 2064 6561 6c63 6c6f  on..from dealclo
-00000f90: 7564 5f73 646b 2069 6d70 6f72 7420 4465  ud_sdk import De
-00000fa0: 616c 436c 6f75 640d 0a0d 0a64 6320 3d20  alCloud....dc = 
-00000fb0: 4465 616c 436c 6f75 642e 6672 6f6d 5f6a  DealCloud.from_j
-00000fc0: 736f 6e28 2270 6174 682f 746f 2f6a 736f  son("path/to/jso
-00000fd0: 6e5f 636f 6e66 6967 5f66 696c 652e 6a73  n_config_file.js
-00000fe0: 6f6e 2229 0d0a 6060 600d 0a53 696d 696c  on")..```..Simil
-00000ff0: 6172 6c79 2c20 6966 2074 6865 2063 7265  arly, if the cre
-00001000: 6465 6e74 6961 6c73 2061 7265 2073 746f  dentials are sto
-00001010: 7265 6420 6173 2070 6172 7420 6f66 2061  red as part of a
-00001020: 206c 6172 6765 7220 4a53 4f4e 2063 6f6e   larger JSON con
-00001030: 6669 6720 6669 6c65 2c20 6120 6b65 7920  fig file, a key 
-00001040: 7061 7468 2063 616e 2062 6520 7061 7373  path can be pass
-00001050: 6564 2061 7320 7468 6520 7365 636f 6e64  ed as the second
-00001060: 2061 7267 756d 656e 742c 2064 6972 6563   argument, direc
-00001070: 7469 6e67 2020 6044 6561 6c43 6c6f 7564  ting  `DealCloud
-00001080: 6020 746f 2074 6865 2070 6174 6820 6f66  ` to the path of
-00001090: 2074 6865 2063 7265 6465 6e74 6961 6c73   the credentials
-000010a0: 2069 6e20 7468 6520 7769 6465 7220 4a53   in the wider JS
-000010b0: 4f4e 2e20 466f 7220 6578 616d 706c 653a  ON. For example:
-000010c0: 0d0a 6060 606a 736f 6e0d 0a7b 0d0a 2020  ..```json..{..  
-000010d0: 2020 226f 7468 6572 223a 205b 312c 322c    "other": [1,2,
-000010e0: 335d 2c0d 0a20 2020 2022 6372 6564 7322  3],..    "creds"
-000010f0: 3a7b 0d0a 2020 2020 2020 2020 2264 6322  :{..        "dc"
-00001100: 3a7b 0d0a 2020 2020 2020 2020 2020 2273  :{..          "s
-00001110: 6974 655f 7572 6c22 3a20 2263 6c69 656e  ite_url": "clien
-00001120: 742e 6465 616c 636c 6f75 642e 636f 6d22  t.dealcloud.com"
-00001130: 2c0d 0a20 2020 2020 2020 2020 2022 636c  ,..          "cl
-00001140: 6965 6e74 5f69 6422 3a20 3132 3334 352c  ient_id": 12345,
-00001150: 0d0a 2020 2020 2020 2020 2020 2263 6c69  ..          "cli
-00001160: 656e 745f 7365 6372 6574 223a 2022 796f  ent_secret": "yo
-00001170: 7572 5f63 6c69 656e 745f 7365 6372 6574  ur_client_secret
-00001180: 220d 0a20 2020 2020 2020 207d 0d0a 2020  "..        }..  
-00001190: 2020 7d0d 0a7d 0d0a 6060 600d 0a0d 0a60    }..}..```....`
-000011a0: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2064  ``python..from d
-000011b0: 6561 6c63 6c6f 7564 5f73 646b 2069 6d70  ealcloud_sdk imp
-000011c0: 6f72 7420 4465 616c 436c 6f75 640d 0a0d  ort DealCloud...
-000011d0: 0a64 6320 3d20 4465 616c 436c 6f75 642e  .dc = DealCloud.
-000011e0: 6672 6f6d 5f6a 736f 6e28 2270 6174 682f  from_json("path/
-000011f0: 746f 2f6a 736f 6e5f 636f 6e66 6967 5f66  to/json_config_f
-00001200: 696c 652e 6a73 6f6e 222c 2022 6372 6564  ile.json", "cred
-00001210: 732e 6463 2229 0d0a 6060 600d 0a23 2323  s.dc")..```..###
-00001220: 2055 7369 6e67 2059 414d 4c20 436f 6e66   Using YAML Conf
-00001230: 6967 2046 696c 650d 0a47 6976 656e 2061  ig File..Given a
-00001240: 2059 414d 4c20 6669 6c65 2069 6e20 7468   YAML file in th
-00001250: 6520 6265 6c6f 7720 666f 726d 6174 3a0d  e below format:.
-00001260: 0a60 6060 7961 6d6c 0d0a 7369 7465 5f75  .```yaml..site_u
-00001270: 726c 3a20 2263 6c69 656e 742e 6465 616c  rl: "client.deal
-00001280: 636c 6f75 642e 636f 6d22 0d0a 636c 6965  cloud.com"..clie
-00001290: 6e74 5f69 643a 2031 3233 3435 0d0a 636c  nt_id: 12345..cl
-000012a0: 6965 6e74 5f73 6563 7265 743a 2022 796f  ient_secret: "yo
-000012b0: 7572 5f63 6c69 656e 745f 7365 6372 6574  ur_client_secret
-000012c0: 220d 0a60 6060 0d0a 5468 6520 4465 616c  "..```..The Deal
-000012d0: 436c 6f75 6420 6f62 6a65 6374 2063 616e  Cloud object can
-000012e0: 2062 6520 6372 6561 7465 6420 6173 2062   be created as b
-000012f0: 656c 6f77 3a0d 0a0d 0a60 6060 7079 7468  elow:....```pyth
-00001300: 6f6e 0d0a 6672 6f6d 2064 6561 6c63 6c6f  on..from dealclo
-00001310: 7564 5f73 646b 2069 6d70 6f72 7420 4465  ud_sdk import De
-00001320: 616c 436c 6f75 640d 0a0d 0a64 6320 3d20  alCloud....dc = 
-00001330: 4465 616c 436c 6f75 642e 6672 6f6d 5f79  DealCloud.from_y
-00001340: 616d 6c28 2270 6174 682f 746f 2f79 616d  aml("path/to/yam
-00001350: 6c5f 636f 6e66 6967 5f66 696c 652e 6a73  l_config_file.js
-00001360: 6f6e 2229 0d0a 6060 600d 0a53 696d 696c  on")..```..Simil
-00001370: 6172 6c79 2c20 6966 2074 6865 2063 7265  arly, if the cre
-00001380: 6465 6e74 6961 6c73 2061 7265 2073 746f  dentials are sto
-00001390: 7265 6420 6173 2070 6172 7420 6f66 2061  red as part of a
-000013a0: 206c 6172 6765 7220 5941 4d4c 2063 6f6e   larger YAML con
-000013b0: 6669 6720 6669 6c65 2c20 6120 6b65 7920  fig file, a key 
-000013c0: 7061 7468 2063 616e 2062 6520 7061 7373  path can be pass
-000013d0: 6564 2061 7320 7468 6520 7365 636f 6e64  ed as the second
-000013e0: 2061 7267 756d 656e 742c 2064 6972 6563   argument, direc
-000013f0: 7469 6e67 2020 6044 6561 6c43 6c6f 7564  ting  `DealCloud
-00001400: 6020 746f 2074 6865 2070 6174 6820 6f66  ` to the path of
-00001410: 2074 6865 2063 7265 6465 6e74 6961 6c73   the credentials
-00001420: 2069 6e20 7468 6520 7769 6465 7220 5941   in the wider YA
-00001430: 4d4c 2e20 466f 7220 6578 616d 706c 653a  ML. For example:
-00001440: 0d0a 6060 6079 616d 6c0d 0a6f 7468 6572  ..```yaml..other
-00001450: 3a0d 0a20 202d 2031 0d0a 2020 2d20 320d  :..  - 1..  - 2.
-00001460: 0a20 202d 2033 0d0a 6372 6564 733a 0d0a  .  - 3..creds:..
-00001470: 2020 6463 3a0d 0a20 2020 2073 6974 655f    dc:..    site_
-00001480: 7572 6c3a 2022 636c 6965 6e74 2e64 6561  url: "client.dea
-00001490: 6c63 6c6f 7564 2e63 6f6d 220d 0a20 2020  lcloud.com"..   
-000014a0: 2063 6c69 656e 745f 6964 3a20 3132 3334   client_id: 1234
-000014b0: 350d 0a20 2020 2063 6c69 656e 745f 7365  5..    client_se
-000014c0: 6372 6574 3a20 2279 6f75 725f 636c 6965  cret: "your_clie
-000014d0: 6e74 5f73 6563 7265 7422 0d0a 6060 600d  nt_secret"..```.
-000014e0: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
-000014f0: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
-00001500: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
-00001510: 640d 0a0d 0a64 6320 3d20 4465 616c 436c  d....dc = DealCl
-00001520: 6f75 642e 6672 6f6d 5f79 616d 6c28 2270  oud.from_yaml("p
-00001530: 6174 682f 746f 2f79 616d 6c5f 636f 6e66  ath/to/yaml_conf
-00001540: 6967 5f66 696c 652e 6a73 6f6e 222c 2022  ig_file.json", "
-00001550: 6372 6564 732e 6463 2229 0d0a 6060 600d  creds.dc")..```.
-00001560: 0a0d 0a23 2320 5363 6865 6d61 2051 7565  ...## Schema Que
-00001570: 7279 696e 670d 0a54 6865 2044 6561 6c43  rying..The DealC
-00001580: 6c6f 7564 2041 5049 2061 6c6c 6f77 7320  loud API allows 
-00001590: 796f 7520 746f 2071 7565 7279 2074 6865  you to query the
-000015a0: 2073 6368 656d 6120 6f66 2061 2067 6976   schema of a giv
-000015b0: 656e 2073 6974 652e 2054 6865 2060 4465  en site. The `De
-000015c0: 616c 436c 6f75 6460 2063 6c61 7373 2070  alCloud` class p
-000015d0: 726f 7669 6465 7320 6163 6365 7373 2074  rovides access t
-000015e0: 6f20 7468 6520 7363 6865 6d61 2065 6e64  o the schema end
-000015f0: 706f 696e 7473 2074 6872 6f75 6768 2074  points through t
-00001600: 6865 2066 6f6c 6c6f 7769 6e67 206d 6574  he following met
-00001610: 686f 6473 3a0d 0a3e 2054 6865 2073 6368  hods:..> The sch
-00001620: 656d 6120 6d6f 6465 6c73 2061 7265 2064  ema models are d
-00001630: 6566 696e 6564 2075 7369 6e67 205b 5079  efined using [Py
-00001640: 6461 6e74 6963 5d28 6874 7470 733a 2f2f  dantic](https://
-00001650: 7079 6461 6e74 6963 2e64 6576 2f29 2c20  pydantic.dev/), 
-00001660: 666f 7220 636c 6561 7220 7661 6c69 6461  for clear valida
-00001670: 7469 6f6e 2c20 7374 7261 6967 6874 666f  tion, straightfo
-00001680: 7277 6172 6420 6174 7472 6962 7574 6520  rward attribute 
-00001690: 6163 6365 7373 2061 6e64 2049 4445 2061  access and IDE a
-000016a0: 7373 6973 7461 6e63 652e 0d0a 3e20 5468  ssistance...> Th
-000016b0: 6573 6520 6d6f 6465 6c73 2063 616e 2062  ese models can b
-000016c0: 6520 666f 756e 6420 696e 2074 6865 205b  e found in the [
-000016d0: 6d6f 6465 6c73 5d28 2f64 6561 6c63 6c6f  models](/dealclo
-000016e0: 7564 5f73 646b 2f6d 6f64 656c 7329 2064  ud_sdk/models) d
-000016f0: 6972 6563 746f 7279 2e0d 0a0d 0a23 2323  irectory.....###
-00001700: 2047 6574 2055 7365 7273 0d0a 0d0a 6044   Get Users....`D
-00001710: 6561 6c43 6c6f 7564 2e67 6574 5f75 7365  ealCloud.get_use
-00001720: 7273 2829 6020 7769 6c6c 2072 6574 7572  rs()` will retur
-00001730: 6e20 616c 6c20 7573 6572 7320 696e 2074  n all users in t
-00001740: 6865 2073 6974 652e 2053 7065 6369 6669  he site. Specifi
-00001750: 6361 6c6c 792c 2061 6e20 6172 7261 7920  cally, an array 
-00001760: 6f66 2060 5573 6572 6020 6f62 6a65 6374  of `User` object
-00001770: 7320 2873 6565 205b 7468 6520 5573 6572  s (see [the User
-00001780: 206f 626a 6563 745d 282f 6465 616c 636c   object](/dealcl
-00001790: 6f75 645f 7364 6b2f 6d6f 6465 6c73 2f73  oud_sdk/models/s
-000017a0: 6368 656d 612e 7079 234c 3639 2d4c 3735  chema.py#L69-L75
-000017b0: 2929 2e20 5468 6520 6172 6775 6d65 6e74  )). The argument
-000017c0: 3a20 6061 6374 6976 655f 6f6e 6c79 6020  : `active_only` 
-000017d0: 6973 2061 2062 6f6f 6c65 616e 2074 6861  is a boolean tha
-000017e0: 7420 6361 6e20 6265 2070 6173 7365 642c  t can be passed,
-000017f0: 2069 6620 7472 7565 2c20 7468 6520 6675   if true, the fu
-00001800: 6e63 7469 6f6e 2077 696c 6c20 6f6e 6c79  nction will only
-00001810: 2072 6574 7572 6e20 6163 7469 7665 2075   return active u
-00001820: 7365 7273 2e0d 0a0d 0a45 7861 6d70 6c65  sers.....Example
-00001830: 3a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  :....```python..
-00001840: 6672 6f6d 2064 6561 6c63 6c6f 7564 5f73  from dealcloud_s
-00001850: 646b 2069 6d70 6f72 7420 4465 616c 436c  dk import DealCl
-00001860: 6f75 640d 0a0d 0a64 6320 3d20 4465 616c  oud....dc = Deal
-00001870: 436c 6f75 642e 6672 6f6d 5f79 616d 6c28  Cloud.from_yaml(
-00001880: 2270 6174 682f 746f 2f79 616d 6c5f 636f  "path/to/yaml_co
-00001890: 6e66 6967 5f66 696c 652e 6a73 6f6e 2229  nfig_file.json")
-000018a0: 0d0a 0d0a 7573 6572 7320 3d20 6463 2e67  ....users = dc.g
-000018b0: 6574 5f75 7365 7273 2829 0d0a 0d0a 666f  et_users()....fo
-000018c0: 7220 7573 6572 2069 6e20 7573 6572 733a  r user in users:
-000018d0: 0d0a 2020 2020 7072 696e 7428 6622 7b75  ..    print(f"{u
-000018e0: 7365 722e 6e61 6d65 7d3a 207b 7573 6572  ser.name}: {user
-000018f0: 2e65 6d61 696c 7d22 290d 0a60 6060 0d0a  .email}")..```..
-00001900: 5769 6c6c 206f 7574 7075 743a 0d0a 6060  Will output:..``
-00001910: 6062 6173 680d 0a55 7365 7220 313a 2075  `bash..User 1: u
-00001920: 7365 7231 4065 6d61 696c 2e63 6f6d 0d0a  ser1@email.com..
-00001930: 5573 6572 2032 3a20 7573 6572 3240 656d  User 2: user2@em
-00001940: 6169 6c2e 636f 6d0d 0a55 7365 7220 333a  ail.com..User 3:
-00001950: 2075 7365 7233 4065 6d61 696c 2e63 6f6d   user3@email.com
-00001960: 0d0a 5573 6572 2034 3a20 7573 6572 3440  ..User 4: user4@
-00001970: 656d 6169 6c2e 636f 6d0d 0a2e 2e2e 6574  email.com.....et
-00001980: 630d 0a60 6060 0d0a 2323 2320 4765 7420  c..```..### Get 
-00001990: 4375 7272 656e 6369 6573 0d0a 6044 6561  Currencies..`Dea
-000019a0: 6c43 6c6f 7564 2e67 6574 5f63 7572 7265  lCloud.get_curre
-000019b0: 6e63 6965 7328 2960 2077 696c 6c20 7265  ncies()` will re
-000019c0: 7475 726e 2074 6865 2063 7572 7265 6e63  turn the currenc
-000019d0: 7920 636f 6465 7320 6f66 2061 6c6c 2065  y codes of all e
-000019e0: 6e61 626c 6564 2063 7572 7265 6e63 6965  nabled currencie
-000019f0: 7320 696e 2074 6865 2073 6974 652e 0d0a  s in the site...
-00001a00: 4578 616d 706c 653a 0d0a 0d0a 6060 6070  Example:....```p
-00001a10: 7974 686f 6e0d 0a66 726f 6d20 6465 616c  ython..from deal
-00001a20: 636c 6f75 645f 7364 6b20 696d 706f 7274  cloud_sdk import
-00001a30: 2044 6561 6c43 6c6f 7564 0d0a 0d0a 6463   DealCloud....dc
-00001a40: 203d 2044 6561 6c43 6c6f 7564 2e66 726f   = DealCloud.fro
-00001a50: 6d5f 7961 6d6c 2822 7061 7468 2f74 6f2f  m_yaml("path/to/
-00001a60: 7961 6d6c 5f63 6f6e 6669 675f 6669 6c65  yaml_config_file
-00001a70: 2e6a 736f 6e22 290d 0a0d 0a63 7572 7265  .json")....curre
-00001a80: 6e63 6965 7320 3d20 6463 2e67 6574 5f63  ncies = dc.get_c
-00001a90: 7572 7265 6e63 6965 7328 290d 0a0d 0a66  urrencies()....f
-00001aa0: 6f72 2063 6379 2069 6e20 6375 7272 656e  or ccy in curren
-00001ab0: 6369 6573 3a0d 0a20 2020 2070 7269 6e74  cies:..    print
-00001ac0: 2863 6379 290d 0a60 6060 0d0a 5769 6c6c  (ccy)..```..Will
-00001ad0: 206f 7574 7075 743a 0d0a 6060 6062 6173   output:..```bas
-00001ae0: 680d 0a47 4250 0d0a 5553 440d 0a45 5552  h..GBP..USD..EUR
-00001af0: 0d0a 2e2e 2e65 7463 0d0a 6060 600d 0a0d  .....etc..```...
-00001b00: 0a23 2323 2047 6574 204f 626a 6563 7473  .### Get Objects
-00001b10: 0d0a 6044 6561 6c43 6c6f 7564 2e67 6574  ..`DealCloud.get
-00001b20: 5f6f 626a 6563 7428 2960 2077 696c 6c20  _object()` will 
-00001b30: 7265 7475 726e 2061 6c6c 2063 6f6e 6669  return all confi
-00001b40: 6775 7265 6420 6f62 6a65 6374 7320 696e  gured objects in
-00001b50: 2074 6865 2073 6974 652e 2053 7065 6369   the site. Speci
-00001b60: 6669 6361 6c6c 792c 2061 6e20 6172 7261  fically, an arra
-00001b70: 7920 6f66 2060 4f62 6a65 6374 6020 6f62  y of `Object` ob
-00001b80: 6a65 6374 7320 2873 6565 205b 7468 6520  jects (see [the 
-00001b90: 4f62 6a65 6374 206f 626a 6563 745d 282f  Object object](/
-00001ba0: 6465 616c 636c 6f75 645f 7364 6b2f 6d6f  dealcloud_sdk/mo
-00001bb0: 6465 6c73 2f73 6368 656d 612e 7079 234c  dels/schema.py#L
-00001bc0: 362d 4c31 3629 292e 0d0a 4578 616d 706c  6-L16))...Exampl
-00001bd0: 653a 0d0a 0d0a 6060 6070 7974 686f 6e0d  e:....```python.
-00001be0: 0a66 726f 6d20 6465 616c 636c 6f75 645f  .from dealcloud_
-00001bf0: 7364 6b20 696d 706f 7274 2044 6561 6c43  sdk import DealC
-00001c00: 6c6f 7564 0d0a 0d0a 6463 203d 2044 6561  loud....dc = Dea
-00001c10: 6c43 6c6f 7564 2e66 726f 6d5f 7961 6d6c  lCloud.from_yaml
-00001c20: 2822 7061 7468 2f74 6f2f 7961 6d6c 5f63  ("path/to/yaml_c
-00001c30: 6f6e 6669 675f 6669 6c65 2e6a 736f 6e22  onfig_file.json"
-00001c40: 290d 0a0d 0a6f 626a 6563 7473 203d 2064  )....objects = d
-00001c50: 632e 6765 745f 6f62 6a65 6374 7328 290d  c.get_objects().
-00001c60: 0a0d 0a66 6f72 206f 626a 2069 6e20 6f62  ...for obj in ob
-00001c70: 6a65 6374 733a 0d0a 2020 2020 7072 696e  jects:..    prin
-00001c80: 7428 6622 7b6f 626a 2e61 7069 4e61 6d65  t(f"{obj.apiName
-00001c90: 7d3a 207b 6f62 6a2e 706c 7572 616c 4e61  }: {obj.pluralNa
-00001ca0: 6d65 7d2c 207b 6f62 6a2e 7369 6e67 756c  me}, {obj.singul
-00001cb0: 6172 4e61 6d65 7d22 290d 0a60 6060 0d0a  arName}")..```..
-00001cc0: 5769 6c6c 206f 7574 7075 743a 0d0a 6060  Will output:..``
-00001cd0: 6062 6173 680d 0a43 6f6d 7061 6e79 3a20  `bash..Company: 
-00001ce0: 436f 6d70 616e 6965 732c 2043 6f6d 7061  Companies, Compa
-00001cf0: 6e79 0d0a 436f 6e74 6163 743a 2043 6f6e  ny..Contact: Con
-00001d00: 7461 6374 732c 2043 6f6e 7461 6374 0d0a  tacts, Contact..
-00001d10: 436f 6d70 616e 7941 6464 7265 7373 3a20  CompanyAddress: 
-00001d20: 436f 6d70 616e 7920 4164 6472 6573 7365  Company Addresse
-00001d30: 732c 2043 6f6d 7061 6e79 2041 6464 7265  s, Company Addre
-00001d40: 7373 0d0a 2e2e 2e65 7463 0d0a 6060 600d  ss.....etc..```.
-00001d50: 0a0d 0a23 2320 4765 7420 4669 656c 6473  ...## Get Fields
-00001d60: 0d0a 6044 6561 6c43 6c6f 7564 2e67 6574  ..`DealCloud.get
-00001d70: 5f66 6965 6c64 7328 2960 2070 726f 7669  _fields()` provi
-00001d80: 6465 7320 7468 6520 6162 696c 6974 7920  des the ability 
-00001d90: 746f 2072 6574 7572 6e20 6669 656c 6473  to return fields
-00001da0: 2063 6f6e 6669 6775 7265 6420 696e 2074   configured in t
-00001db0: 6865 2073 6974 652e 2053 7065 6369 6669  he site. Specifi
-00001dc0: 6361 6c6c 792c 2061 6e20 6172 7261 7920  cally, an array 
-00001dd0: 6f66 2060 4669 656c 6460 206f 626a 6563  of `Field` objec
-00001de0: 7473 2028 7365 6520 5b74 6865 2046 6965  ts (see [the Fie
-00001df0: 6c64 206f 626a 6563 745d 282f 6465 616c  ld object](/deal
-00001e00: 636c 6f75 645f 7364 6b2f 6d6f 6465 6c73  cloud_sdk/models
-00001e10: 2f73 6368 656d 612e 7079 234c 3239 2d4c  /schema.py#L29-L
-00001e20: 3533 2929 2e0d 0a0d 0a54 6865 7265 2061  53)).....There a
-00001e30: 7265 2074 6872 6565 2077 6179 7320 746f  re three ways to
-00001e40: 2071 7565 7279 2066 6f72 2066 6965 6c64   query for field
-00001e50: 733a 0d0a 312e 205f 5f41 6c6c 2046 6965  s:..1. __All Fie
-00001e60: 6c64 735f 5f3a 2063 616c 6c20 6044 6561  lds__: call `Dea
-00001e70: 6c43 6c6f 7564 2e67 6574 5f66 6965 6c64  lCloud.get_field
-00001e80: 7328 2960 2077 6974 6820 6e6f 2061 7267  s()` with no arg
-00001e90: 756d 656e 7473 2074 6f20 7265 7475 726e  uments to return
-00001ea0: 2061 6c6c 2066 6965 6c64 732e 0d0a 0d0a   all fields.....
-00001eb0: 6060 6070 7974 686f 6e0d 0a66 726f 6d20  ```python..from 
-00001ec0: 6465 616c 636c 6f75 645f 7364 6b20 696d  dealcloud_sdk im
-00001ed0: 706f 7274 2044 6561 6c43 6c6f 7564 0d0a  port DealCloud..
-00001ee0: 0d0a 6463 203d 2044 6561 6c43 6c6f 7564  ..dc = DealCloud
-00001ef0: 2e66 726f 6d5f 7961 6d6c 2822 7061 7468  .from_yaml("path
-00001f00: 2f74 6f2f 7961 6d6c 5f63 6f6e 6669 675f  /to/yaml_config_
-00001f10: 6669 6c65 2e6a 736f 6e22 290d 0a0d 0a66  file.json")....f
-00001f20: 6965 6c64 7320 3d20 6463 2e67 6574 5f66  ields = dc.get_f
-00001f30: 6965 6c64 7328 290d 0a60 6060 0d0a 6066  ields()..```..`f
-00001f40: 6965 6c64 7360 2077 696c 6c20 636f 6e74  ields` will cont
-00001f50: 6169 6e20 6120 6c69 7374 206f 6620 6046  ain a list of `F
-00001f60: 6965 6c64 6020 6f62 6a65 6374 7320 636f  ield` objects co
-00001f70: 6e74 6169 6e69 6e67 2061 6c6c 2063 6f6e  ntaining all con
-00001f80: 6669 6775 7265 6420 6669 656c 6473 2069  figured fields i
-00001f90: 6e20 7468 6520 7369 7465 2e0d 0a0d 0a0d  n the site......
-00001fa0: 0a32 2e20 5f5f 416c 6c20 4669 656c 6473  .2. __All Fields
-00001fb0: 2066 6f72 2061 6e20 4f62 6a65 6374 5f5f   for an Object__
-00001fc0: 3a20 6361 6c6c 2060 4465 616c 436c 6f75  : call `DealClou
-00001fd0: 642e 6765 745f 6669 656c 6473 286f 626a  d.get_fields(obj
-00001fe0: 6563 745f 6964 3d22 4f62 6a65 6374 4e61  ect_id="ObjectNa
-00001ff0: 6d65 2229 6020 7769 7468 2060 6f62 6a65  me")` with `obje
-00002000: 6374 5f69 6460 2073 6574 2074 6f20 7468  ct_id` set to th
-00002010: 6520 6465 7369 7265 6420 6f62 6a65 6374  e desired object
-00002020: 2061 7069 206e 616d 652c 206f 7220 6f62   api name, or ob
-00002030: 6a65 6374 2069 642c 2074 6f20 7265 7475  ject id, to retu
-00002040: 726e 2061 6c6c 2066 6965 6c64 7320 636f  rn all fields co
-00002050: 6e66 6967 7572 6564 2066 6f72 2074 6861  nfigured for tha
-00002060: 7420 6f62 6a65 6374 2e0d 0a0d 0a60 6060  t object.....```
-00002070: 7079 7468 6f6e 0d0a 6672 6f6d 2064 6561  python..from dea
-00002080: 6c63 6c6f 7564 5f73 646b 2069 6d70 6f72  lcloud_sdk impor
-00002090: 7420 4465 616c 436c 6f75 640d 0a0d 0a64  t DealCloud....d
-000020a0: 6320 3d20 4465 616c 436c 6f75 642e 6672  c = DealCloud.fr
-000020b0: 6f6d 5f79 616d 6c28 2270 6174 682f 746f  om_yaml("path/to
-000020c0: 2f79 616d 6c5f 636f 6e66 6967 5f66 696c  /yaml_config_fil
-000020d0: 652e 6a73 6f6e 2229 0d0a 0d0a 6669 656c  e.json")....fiel
-000020e0: 6473 203d 2064 632e 6765 745f 6669 656c  ds = dc.get_fiel
-000020f0: 6473 2822 436f 6d70 616e 7922 290d 0a60  ds("Company")..`
-00002100: 6060 0d0a 6066 6965 6c64 7360 2077 696c  ``..`fields` wil
-00002110: 6c20 636f 6e74 6169 6e20 6120 6c69 7374  l contain a list
-00002120: 206f 6620 6046 6965 6c64 6020 6f62 6a65   of `Field` obje
-00002130: 6374 732c 2063 6f6e 7461 696e 696e 6720  cts, containing 
-00002140: 616c 6c20 6669 656c 6473 2063 6f6e 6669  all fields confi
-00002150: 6775 7265 6420 696e 2074 6865 2022 436f  gured in the "Co
-00002160: 6d70 616e 7922 206f 626a 6563 742e 0d0a  mpany" object...
-00002170: 0d0a 0d0a 332e 205f 5f41 2046 6965 6c64  ....3. __A Field
-00002180: 2062 7920 4669 656c 6420 4944 5f5f 3a20   by Field ID__: 
-00002190: 6361 6c6c 2060 4465 616c 436c 6f75 642e  call `DealCloud.
-000021a0: 6765 745f 6669 656c 6473 2866 6965 6c64  get_fields(field
-000021b0: 5f69 643d 3132 3334 2960 2077 6974 6820  _id=1234)` with 
-000021c0: 6066 6965 6c64 5f69 6460 2073 6574 2074  `field_id` set t
-000021d0: 6f20 7468 6520 4944 206f 6620 7468 6520  o the ID of the 
-000021e0: 6465 7369 7265 6420 6669 656c 642e 0d0a  desired field...
-000021f0: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
-00002200: 6d20 6465 616c 636c 6f75 645f 7364 6b20  m dealcloud_sdk 
-00002210: 696d 706f 7274 2044 6561 6c43 6c6f 7564  import DealCloud
-00002220: 0d0a 0d0a 6463 203d 2044 6561 6c43 6c6f  ....dc = DealClo
-00002230: 7564 2e66 726f 6d5f 7961 6d6c 2822 7061  ud.from_yaml("pa
-00002240: 7468 2f74 6f2f 7961 6d6c 5f63 6f6e 6669  th/to/yaml_confi
-00002250: 675f 6669 6c65 2e6a 736f 6e22 290d 0a0d  g_file.json")...
-00002260: 0a66 6965 6c64 203d 2064 632e 6765 745f  .field = dc.get_
-00002270: 6669 656c 6473 2866 6965 6c64 5f69 643d  fields(field_id=
-00002280: 3132 3334 290d 0a60 6060 0d0a 6066 6965  1234)..```..`fie
-00002290: 6c64 6020 7769 6c6c 2063 6f6e 7461 696e  ld` will contain
-000022a0: 2061 2073 696e 676c 6520 6046 6965 6c64   a single `Field
-000022b0: 6020 6f62 6a65 6374 2c20 6465 7363 7269  ` object, descri
-000022c0: 6269 6e67 2074 6865 2066 6965 6c64 2077  bing the field w
-000022d0: 6974 6820 4944 2060 3132 3334 602e 0d0a  ith ID `1234`...
-000022e0: 0d0a 2323 2320 4765 7420 5363 6865 6d61  ..### Get Schema
-000022f0: 0d0a 6044 6561 6c43 6c6f 7564 2e67 6574  ..`DealCloud.get
-00002300: 5f73 6368 656d 6128 2960 2069 7320 6120  _schema()` is a 
-00002310: 6d65 7468 6f64 2074 6861 7420 7769 6c6c  method that will
-00002320: 2072 6574 7572 6e20 7468 6520 6675 6c6c   return the full
-00002330: 2044 6561 6c43 6c6f 7564 2073 6368 656d   DealCloud schem
-00002340: 6120 696e 2061 2073 696e 676c 6520 6f62  a in a single ob
-00002350: 6a65 6374 2028 7365 6520 5b74 6865 2053  ject (see [the S
-00002360: 6368 656d 6120 6f62 6a65 6374 5d28 6465  chema object](de
-00002370: 616c 636c 6f75 645f 7364 6b2f 6d6f 6465  alcloud_sdk/mode
-00002380: 6c73 2f73 6368 656d 612e 7079 234c 3633  ls/schema.py#L63
-00002390: 2d4c 3636 2929 2e0d 0a54 6865 206d 6574  -L66))...The met
-000023a0: 686f 6420 7461 6b65 7320 7468 6520 6172  hod takes the ar
-000023b0: 6775 6d65 6e74 3a20 606b 6579 5f74 7970  gument: `key_typ
-000023c0: 6560 2c20 7768 6963 6820 6465 7363 7269  e`, which descri
-000023d0: 6265 7320 7768 6963 6820 6669 656c 6420  bes which field 
-000023e0: 7769 6c6c 2062 6520 7573 6564 2061 7320  will be used as 
-000023f0: 6b65 7973 2069 6e20 7468 6520 6e65 7374  keys in the nest
-00002400: 6564 206f 626a 6563 7420 7374 7275 6374  ed object struct
-00002410: 7572 6520 6465 7363 7269 6269 6e67 2074  ure describing t
-00002420: 6865 2073 6368 656d 612e 200d 0a0d 0a54  he schema. ....T
-00002430: 6865 206f 7074 696f 6e73 2061 7265 3a0d  he options are:.
-00002440: 0a2d 2060 6170 6960 202d 2054 6865 2041  .- `api` - The A
-00002450: 5049 206e 616d 650d 0a2d 2060 6469 7370  PI name..- `disp
-00002460: 6c61 7960 202d 2054 6865 2064 6973 706c  lay` - The displ
-00002470: 6179 206e 616d 650d 0a2d 2060 6964 6020  ay name..- `id` 
-00002480: 2d20 5468 6520 6f62 6a65 6374 2f66 6965  - The object/fie
-00002490: 6c64 2049 440d 0a0d 0a55 7361 6765 2045  ld ID....Usage E
-000024a0: 7861 6d70 6c65 3a0d 0a0d 0a60 6060 7079  xample:....```py
-000024b0: 7468 6f6e 0d0a 6672 6f6d 2064 6561 6c63  thon..from dealc
-000024c0: 6c6f 7564 5f73 646b 2069 6d70 6f72 7420  loud_sdk import 
-000024d0: 4465 616c 436c 6f75 640d 0a0d 0a64 6320  DealCloud....dc 
-000024e0: 3d20 4465 616c 436c 6f75 642e 6672 6f6d  = DealCloud.from
-000024f0: 5f79 616d 6c28 2270 6174 682f 746f 2f79  _yaml("path/to/y
-00002500: 616d 6c5f 636f 6e66 6967 5f66 696c 652e  aml_config_file.
-00002510: 6a73 6f6e 2229 0d0a 0d0a 7363 6865 6d61  json")....schema
-00002520: 203d 2064 632e 6765 745f 7363 6865 6d61   = dc.get_schema
-00002530: 2822 6170 6922 290d 0a60 6060 0d0a 6073  ("api")..```..`s
-00002540: 6368 656d 6160 2077 696c 6c20 636f 6e74  chema` will cont
-00002550: 6169 6e20 7468 6520 6120 6053 6368 656d  ain the a `Schem
-00002560: 6160 206f 626a 6563 7420 7769 7468 2074  a` object with t
-00002570: 6865 2041 5049 206e 616d 6573 2061 7320  he API names as 
-00002580: 6b65 7973 2c20 6173 2062 656c 6f77 3a20  keys, as below: 
-00002590: 0d0a 0d0a 6061 7069 6020 4578 616d 706c  ....`api` Exampl
-000025a0: 653a 0d0a 6060 6070 7974 686f 6e0d 0a7b  e:..```python..{
-000025b0: 0d0a 2020 2243 6f6d 7061 6e79 4150 494e  ..  "CompanyAPIN
-000025c0: 616d 6522 3a20 7b0d 0a20 2020 2022 436f  ame": {..    "Co
-000025d0: 6d70 616e 794f 626a 6563 744d 6574 6144  mpanyObjectMetaD
-000025e0: 6174 6122 3a20 222e 2e2e 222c 0d0a 2020  ata": "...",..  
-000025f0: 2020 2243 6f6d 7061 6e79 4f62 6a65 6374    "CompanyObject
-00002600: 4669 656c 6473 223a 207b 0d0a 2020 2020  Fields": {..    
-00002610: 2020 2246 6965 6c64 3141 5049 4e61 6d65    "Field1APIName
-00002620: 223a 207b 0d0a 2020 2020 2020 2020 2246  ": {..        "F
-00002630: 6965 6c64 314d 6574 6144 6174 6122 3a20  ield1MetaData": 
-00002640: 222e 2e2e 220d 0a20 2020 2020 207d 0d0a  "..."..      }..
-00002650: 2020 2020 7d0d 0a20 207d 0d0a 7d0d 0a60      }..  }..}..`
-00002660: 6060 0d0a 6064 6973 706c 6179 6020 4578  ``..`display` Ex
-00002670: 616d 706c 653a 0d0a 6060 6070 7974 686f  ample:..```pytho
-00002680: 6e0d 0a7b 0d0a 2020 2243 6f6d 7061 6e79  n..{..  "Company
-00002690: 2044 6973 706c 6179 204e 616d 6522 3a20   Display Name": 
-000026a0: 7b0d 0a20 2020 2022 436f 6d70 616e 794f  {..    "CompanyO
-000026b0: 626a 6563 744d 6574 6144 6174 6122 3a20  bjectMetaData": 
-000026c0: 222e 2e2e 222c 0d0a 2020 2020 2243 6f6d  "...",..    "Com
-000026d0: 7061 6e79 4f62 6a65 6374 4669 656c 6473  panyObjectFields
-000026e0: 223a 207b 0d0a 2020 2020 2020 2246 6965  ": {..      "Fie
-000026f0: 6c64 2031 2044 6973 706c 6179 204e 616d  ld 1 Display Nam
-00002700: 6522 3a20 7b0d 0a20 2020 2020 2020 2022  e": {..        "
-00002710: 4669 656c 6431 4d65 7461 4461 7461 223a  Field1MetaData":
-00002720: 2022 2e2e 2e22 0d0a 2020 2020 2020 7d0d   "..."..      }.
-00002730: 0a20 2020 207d 0d0a 2020 7d0d 0a7d 0d0a  .    }..  }..}..
-00002740: 6060 600d 0a60 6964 6020 4578 616d 706c  ```..`id` Exampl
-00002750: 653a 0d0a 3e20 4e6f 7465 2074 6865 2049  e:..> Note the I
-00002760: 4420 6f66 2074 6865 2022 436f 6d70 616e  D of the "Compan
-00002770: 7922 206f 626a 6563 7420 6973 2031 3233  y" object is 123
-00002780: 3435 2061 6e64 2074 6865 2049 4420 6f66  45 and the ID of
-00002790: 2074 6865 2022 4669 656c 6420 3122 2066   the "Field 1" f
-000027a0: 6965 6c64 2069 7320 3132 3334 3536 200d  ield is 123456 .
-000027b0: 0a60 6060 7079 7468 6f6e 0d0a 7b0d 0a20  .```python..{.. 
-000027c0: 2031 3233 3435 3a20 7b0d 0a20 2020 2022   12345: {..    "
-000027d0: 436f 6d70 616e 794f 626a 6563 744d 6574  CompanyObjectMet
-000027e0: 6144 6174 6122 3a20 222e 2e2e 222c 0d0a  aData": "...",..
-000027f0: 2020 2020 2243 6f6d 7061 6e79 4f62 6a65      "CompanyObje
-00002800: 6374 4669 656c 6473 223a 207b 0d0a 2020  ctFields": {..  
-00002810: 2020 2020 3132 3334 3536 3a20 7b0d 0a20      123456: {.. 
-00002820: 2020 2020 2020 2022 4669 656c 6431 4d65         "Field1Me
-00002830: 7461 4461 7461 223a 2022 2e2e 2e22 0d0a  taData": "..."..
-00002840: 2020 2020 2020 7d0d 0a20 2020 207d 0d0a        }..    }..
-00002850: 2020 7d0d 0a7d 0d0a 6060 600d 0a0d 0a23    }..}..```....#
-00002860: 2320 4461 7461 204f 7065 7261 7469 6f6e  # Data Operation
-00002870: 730d 0a54 6865 2060 4465 616c 436c 6f75  s..The `DealClou
-00002880: 6460 206f 626a 6563 7420 7072 6f76 6964  d` object provid
-00002890: 6573 206d 6574 686f 6473 2074 6f20 4372  es methods to Cr
-000028a0: 6561 7465 2c20 5265 6164 2c20 5570 6461  eate, Read, Upda
-000028b0: 7465 2061 6e64 2044 656c 6574 6520 6461  te and Delete da
-000028c0: 7461 2069 6e20 6275 6c6b 2e20 4173 2069  ta in bulk. As i
-000028d0: 7473 2064 6566 6175 6c74 2062 6568 6176  ts default behav
-000028e0: 696f 7572 2c20 7768 656e 2077 6f72 6b69  iour, when worki
-000028f0: 6e67 2077 6974 6820 7369 7465 2064 6174  ng with site dat
-00002900: 612c 2074 6865 206c 6962 7261 7279 2075  a, the library u
-00002910: 7365 7320 4461 7461 4672 616d 6573 2077  ses DataFrames w
-00002920: 6974 680d 0a74 6865 205b 5061 6e64 6173  ith..the [Pandas
-00002930: 5d28 6874 7470 733a 2f2f 7061 6e64 6173  ](https://pandas
-00002940: 2e70 7964 6174 612e 6f72 672f 2920 6c69  .pydata.org/) li
-00002950: 6272 6172 792c 2068 6f77 6576 6572 2074  brary, however t
-00002960: 6865 206f 7074 696f 6e20 6973 2061 7661  he option is ava
-00002970: 696c 6162 6c65 2066 6f72 2069 7420 746f  ilable for it to
-00002980: 2077 6f72 6b20 7769 7468 206a 7573 7420   work with just 
-00002990: 7079 7468 6f6e 2073 7461 6e64 6172 6420  python standard 
-000029a0: 6461 7461 2074 7970 6573 2e0d 0a0d 0a23  data types.....#
-000029b0: 2323 204c 6973 7420 436f 6e66 6967 7572  ## List Configur
-000029c0: 6564 2056 6965 7773 0d0a 6044 6561 6c43  ed Views..`DealC
-000029d0: 6c6f 7564 2e6c 6973 745f 636f 6e66 6967  loud.list_config
-000029e0: 7572 6564 5f76 6965 7773 2829 6020 7265  ured_views()` re
-000029f0: 7475 726e 7320 6120 6052 6f77 7360 2028  turns a `Rows` (
-00002a00: 7365 6520 5b74 6865 2052 6f77 7320 6f62  see [the Rows ob
-00002a10: 6a65 6374 5d28 2f64 6561 6c63 6c6f 7564  ject](/dealcloud
-00002a20: 5f73 646b 2f6d 6f64 656c 732f 6461 7461  _sdk/models/data
-00002a30: 2e70 7923 4c34 2d4c 3829 2920 636f 6e74  .py#L4-L8)) cont
-00002a40: 6169 6e69 6e67 2061 6c6c 2063 6f6e 6669  aining all confi
-00002a50: 6775 7265 6420 7669 6577 7320 696e 2074  gured views in t
-00002a60: 6865 2073 6974 652e 0d0a 5468 6520 6172  he site...The ar
-00002a70: 6775 6d65 6e74 2060 6973 5f70 7269 7661  gument `is_priva
-00002a80: 7465 6020 6361 6e20 6265 2070 6173 7365  te` can be passe
-00002a90: 6420 6173 2061 2062 6f6f 6c65 616e 2c20  d as a boolean, 
-00002aa0: 7768 6572 6520 6966 2074 7275 652c 206f  where if true, o
-00002ab0: 6e6c 7920 7072 6976 6174 6520 7669 6577  nly private view
-00002ac0: 7320 746f 2028 696e 636c 7564 696e 6720  s to (including 
-00002ad0: 7669 6577 7320 7368 6172 6564 2077 6974  views shared wit
-00002ae0: 6829 2074 6865 2061 7574 6865 6e74 6963  h) the authentic
-00002af0: 6174 6564 2075 7365 7220 7769 6c6c 2062  ated user will b
-00002b00: 6520 7265 7475 726e 6564 2e0d 0a0d 0a45  e returned.....E
-00002b10: 7861 6d70 6c65 3a0d 0a0d 0a60 6060 7079  xample:....```py
-00002b20: 7468 6f6e 0d0a 6672 6f6d 2064 6561 6c63  thon..from dealc
-00002b30: 6c6f 7564 5f73 646b 2069 6d70 6f72 7420  loud_sdk import 
-00002b40: 4465 616c 436c 6f75 640d 0a0d 0a64 6320  DealCloud....dc 
-00002b50: 3d20 4465 616c 436c 6f75 642e 6672 6f6d  = DealCloud.from
-00002b60: 5f79 616d 6c28 2270 6174 682f 746f 2f79  _yaml("path/to/y
-00002b70: 616d 6c5f 636f 6e66 6967 5f66 696c 652e  aml_config_file.
-00002b80: 6a73 6f6e 2229 0d0a 0d0a 7669 6577 7320  json")....views 
-00002b90: 3d20 6463 2e6c 6973 745f 636f 6e66 6967  = dc.list_config
-00002ba0: 7572 6564 5f76 6965 7773 2829 0d0a 6060  ured_views()..``
-00002bb0: 600d 0a60 7669 6577 7360 2077 696c 6c20  `..`views` will 
-00002bc0: 636f 6e74 6169 6e20 6120 7375 6d6d 6172  contain a summar
-00002bd0: 7920 6f66 2063 6f6e 6669 6775 7265 6420  y of configured 
-00002be0: 7669 6577 732e 0d0a 0d0a 2323 2320 5265  views.....### Re
-00002bf0: 6164 2044 6174 610d 0a60 4465 616c 436c  ad Data..`DealCl
-00002c00: 6f75 642e 7265 6164 5f64 6174 6128 2960  oud.read_data()`
-00002c10: 2061 6c6c 6f77 7320 7573 6572 7320 746f   allows users to
-00002c20: 2072 6561 6420 6461 7461 2066 726f 6d20   read data from 
-00002c30: 6120 4465 616c 436c 6f75 6420 6f62 6a65  a DealCloud obje
-00002c40: 6374 2069 6e74 6f20 6120 6070 616e 6461  ct into a `panda
-00002c50: 732e 4461 7461 4672 616d 6560 206f 7220  s.DataFrame` or 
-00002c60: 6120 6c69 7374 206f 6620 7079 7468 6f6e  a list of python
-00002c70: 2064 6963 7469 6f6e 6172 6965 732e 0d0a   dictionaries...
-00002c80: 3e20 5b21 494d 504f 5254 414e 545d 200d  > [!IMPORTANT] .
-00002c90: 0a3e 204f 6e6c 7920 6f6e 6520 6f66 206f  .> Only one of o
-00002ca0: 626a 6563 745f 6964 206f 7220 7669 6577  bject_id or view
-00002cb0: 5f69 6420 6361 6e20 6265 2070 6f70 756c  _id can be popul
-00002cc0: 6174 6564 0d0a 2020 2020 2020 2020 0d0a  ated..        ..
-00002cd0: 4172 6775 6d65 6e74 733a 0d0a 0d0a 2d20  Arguments:....- 
-00002ce0: 6f62 6a65 6374 5f69 6420 6055 6e69 6f6e  object_id `Union
-00002cf0: 5b69 6e74 2c20 7374 725d 603a 2074 6865  [int, str]`: the
-00002d00: 206f 626a 6563 7420 746f 2070 756c 6c20   object to pull 
-00002d10: 6461 7461 2066 726f 6d0d 0a2d 2076 6965  data from..- vie
-00002d20: 775f 6964 2060 556e 696f 6e5b 696e 742c  w_id `Union[int,
-00002d30: 2073 7472 5d60 3a20 7468 6520 7669 6577   str]`: the view
-00002d40: 2074 6f20 7075 6c6c 2064 6174 6120 6672   to pull data fr
-00002d50: 6f6d 0d0a 2d20 6f75 7470 7574 2060 7374  om..- output `st
-00002d60: 7260 3a20 6070 616e 6461 7360 206f 7220  r`: `pandas` or 
-00002d70: 606c 6973 7460 2c20 6465 6369 6465 7320  `list`, decides 
-00002d80: 7468 6520 6f75 7470 7574 2066 6f72 6d61  the output forma
-00002d90: 742c 2060 7061 6e64 6173 6020 6973 2064  t, `pandas` is d
-00002da0: 6566 6175 6c74 0d0a 2d20 7265 736f 6c76  efault..- resolv
-00002db0: 6520 6073 7472 603a 2066 6f72 2070 616e  e `str`: for pan
-00002dc0: 6461 732c 2077 6865 7265 2066 6965 6c64  das, where field
-00002dd0: 7320 636f 6e74 6169 6e20 616e 206f 626a  s contain an obj
-00002de0: 6563 7420 2863 686f 6963 652c 2072 6566  ect (choice, ref
-00002df0: 6572 656e 6365 2c20 7573 6572 292c 2072  erence, user), r
-00002e00: 6573 6f6c 7665 2074 6f20 7468 6520 6964  esolve to the id
-00002e10: 206f 7220 6e61 6d65 0d0a 2d20 7669 6577   or name..- view
-00002e20: 5f66 696c 7465 7220 606c 6973 745b 6469  _filter `list[di
-00002e30: 6374 5d60 3a20 636f 6c75 6d6e 2071 7565  ct]`: column que
-00002e40: 7269 6573 2074 6f20 2273 7570 706c 7920  ries to "supply 
-00002e50: 7661 6c75 6520 6c61 7465 7222 2069 6e20  value later" in 
-00002e60: 7669 6577 732c 2073 6565 3a20 6874 7470  views, see: http
-00002e70: 733a 2f2f 6170 692e 646f 6373 2e64 6561  s://api.docs.dea
-00002e80: 6c63 6c6f 7564 2e63 6f6d 2f64 6f63 732f  lcloud.com/docs/
-00002e90: 6461 7461 2f72 6f77 732f 7669 6577 5f64  data/rows/view_d
-00002ea0: 6574 6169 6c73 0d0a 2d20 6669 656c 6473  etails..- fields
-00002eb0: 2060 6c69 7374 5b73 7472 5d60 3a20 6966   `list[str]`: if
-00002ec0: 206e 6f74 2060 4e6f 6e65 602c 2072 6574   not `None`, ret
-00002ed0: 7572 6e20 6f6e 6c79 2066 6965 6c64 7320  urn only fields 
-00002ee0: 696e 2074 6865 206c 6973 742e 200d 0a2d  in the list. ..-
-00002ef0: 2071 7565 7279 2060 7374 7260 3a20 6120   query `str`: a 
-00002f00: 4465 616c 436c 6f75 6420 726f 7773 2071  DealCloud rows q
-00002f10: 7565 7279 2073 7472 696e 6720 746f 2072  uery string to r
-00002f20: 6571 7565 7374 2073 7065 6369 6669 6320  equest specific 
-00002f30: 696e 666f 726d 6174 696f 6e2c 2073 6565  information, see
-00002f40: 3a20 6874 7470 733a 2f2f 6170 692e 646f  : https://api.do
-00002f50: 6373 2e64 6561 6c63 6c6f 7564 2e63 6f6d  cs.dealcloud.com
-00002f60: 2f64 6f63 732f 6461 7461 2f72 6f77 732f  /docs/data/rows/
-00002f70: 7175 6572 790d 0a2d 2069 6e63 6c75 6465  query..- include
-00002f80: 5f6e 756c 6c73 2060 626f 6f6c 603a 2069  _nulls `bool`: i
-00002f90: 6620 7472 7565 2c20 6e75 6c6c 2063 6f6c  f true, null col
-00002fa0: 756d 6e73 2077 696c 6c20 616c 736f 2062  umns will also b
-00002fb0: 6520 7265 7475 726e 6564 0d0a 2d20 636f  e returned..- co
-00002fc0: 6c75 6d6e 5f68 6561 6465 7273 2060 7374  lumn_headers `st
-00002fd0: 7260 3a20 7370 6563 6966 6965 7320 7468  r`: specifies th
-00002fe0: 6520 7661 6c75 6520 7479 7065 206f 6620  e value type of 
-00002ff0: 7468 6520 7265 7475 726e 2066 6965 6c64  the return field
-00003000: 206b 6579 732f 636f 6c75 6d6e 206e 616d   keys/column nam
-00003010: 6573 2e0d 0a20 202d 2060 6170 6960 203d  es...  - `api` =
-00003020: 2046 6965 6c64 2041 5049 204e 616d 650d   Field API Name.
-00003030: 0a20 202d 2060 6e61 6d65 6020 3d20 4669  .  - `name` = Fi
-00003040: 656c 6420 4469 7370 6c61 7920 4e61 6d65  eld Display Name
-00003050: 0d0a 2020 2d20 6069 6460 203d 2046 6965  ..  - `id` = Fie
-00003060: 6c64 2049 440d 0a0d 0a23 2323 2320 5265  ld ID....#### Re
-00003070: 6164 696e 6720 4461 7461 2066 726f 6d20  ading Data from 
-00003080: 616e 204f 626a 6563 740d 0a45 7861 6d70  an Object..Examp
-00003090: 6c65 3a0d 0a0d 0a60 6060 7079 7468 6f6e  le:....```python
-000030a0: 0d0a 6672 6f6d 2064 6561 6c63 6c6f 7564  ..from dealcloud
-000030b0: 5f73 646b 2069 6d70 6f72 7420 4465 616c  _sdk import Deal
-000030c0: 436c 6f75 640d 0a0d 0a64 6320 3d20 4465  Cloud....dc = De
-000030d0: 616c 436c 6f75 642e 6672 6f6d 5f79 616d  alCloud.from_yam
-000030e0: 6c28 2270 6174 682f 746f 2f79 616d 6c5f  l("path/to/yaml_
-000030f0: 636f 6e66 6967 5f66 696c 652e 6a73 6f6e  config_file.json
-00003100: 2229 0d0a 0d0a 6461 7461 203d 2064 632e  ")....data = dc.
-00003110: 7265 6164 5f64 6174 6128 2243 6f6d 7061  read_data("Compa
-00003120: 6e79 2229 0d0a 6060 600d 0a60 6461 7461  ny")..```..`data
-00003130: 6020 7769 6c6c 2062 6520 6120 6070 616e  ` will be a `pan
-00003140: 6461 732e 4461 7461 4672 616d 6560 2061  das.DataFrame` a
-00003150: 7320 6265 6c6f 773a 0d0a 0d0a 7c20 456e  s below:....| En
-00003160: 7472 7949 6420 7c20 436f 6d70 616e 794e  tryId | CompanyN
-00003170: 616d 6520 7c20 436f 6d70 616e 7954 7970  ame | CompanyTyp
-00003180: 6520 2020 2020 2020 2020 2020 2020 2020  e               
-00003190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031d0: 2020 2020 2020 2020 2020 2020 207c 0d0a               |..
-000031e0: 7c2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  |---------|-----
-000031f0: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
-00003200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003260: 2d7c 0d0a 7c20 3132 3334 3520 2020 7c20  -|..| 12345   | 
-00003270: 436f 6d70 616e 7931 2020 2020 7c20 5b7b  Company1    | [{
-00003280: 2773 6571 4e75 6d62 6572 273a 2033 2c20  'seqNumber': 3, 
-00003290: 2769 7341 7574 6f50 6466 273a 2046 616c  'isAutoPdf': Fal
-000032a0: 7365 2c20 2769 6427 3a20 3331 3937 3738  se, 'id': 319778
-000032b0: 302c 2027 6e61 6d65 273a 2027 4c69 6d69  0, 'name': 'Limi
-000032c0: 7465 6420 5061 7274 6e65 7227 2c20 2765  ted Partner', 'e
-000032d0: 6e74 7279 4c69 7374 4964 273a 202d 367d  ntryListId': -6}
-000032e0: 5d20 2020 207c 0d0a 7c20 3132 3334 3620  ]    |..| 12346 
-000032f0: 2020 7c20 436f 6d70 616e 7932 2020 2020    | Company2    
-00003300: 7c20 5b7b 2773 6571 4e75 6d62 6572 273a  | [{'seqNumber':
-00003310: 2031 2c20 2769 7341 7574 6f50 6466 273a   1, 'isAutoPdf':
-00003320: 2046 616c 7365 2c20 2769 6427 3a20 3331   False, 'id': 31
-00003330: 3937 3738 322c 2027 6e61 6d65 273a 2027  97782, 'name': '
-00003340: 4f70 6572 6174 696e 6720 436f 6d70 616e  Operating Compan
-00003350: 7927 2c20 2765 6e74 7279 4c69 7374 4964  y', 'entryListId
-00003360: 273a 202d 367d 5d20 207c 0d0a 7c20 3132  ': -6}]  |..| 12
-00003370: 3334 3720 2020 7c20 436f 6d70 616e 7933  347   | Company3
-00003380: 2020 2020 7c20 5b7b 2773 6571 4e75 6d62      | [{'seqNumb
-00003390: 6572 273a 2033 2c20 2769 7341 7574 6f50  er': 3, 'isAutoP
-000033a0: 6466 273a 2046 616c 7365 2c20 2769 6427  df': False, 'id'
-000033b0: 3a20 3331 3937 3738 302c 2027 6e61 6d65  : 3197780, 'name
-000033c0: 273a 2027 4c69 6d69 7465 6420 5061 7274  ': 'Limited Part
-000033d0: 6e65 7227 2c20 2765 6e74 7279 4c69 7374  ner', 'entryList
-000033e0: 4964 273a 202d 367d 5d20 2020 207c 0d0a  Id': -6}]    |..
-000033f0: 0d0a 546f 2072 6574 7572 6e20 6120 7079  ..To return a py
-00003400: 7468 6f6e 2060 6c69 7374 6020 696e 7374  thon `list` inst
-00003410: 6561 6420 6f66 2061 2060 7061 6e64 6173  ead of a `pandas
-00003420: 2e44 6174 6146 7261 6d65 603a 0d0a 0d0a  .DataFrame`:....
-00003430: 6060 6070 7974 686f 6e0d 0a66 726f 6d20  ```python..from 
-00003440: 6465 616c 636c 6f75 645f 7364 6b20 696d  dealcloud_sdk im
-00003450: 706f 7274 2044 6561 6c43 6c6f 7564 0d0a  port DealCloud..
-00003460: 0d0a 6463 203d 2044 6561 6c43 6c6f 7564  ..dc = DealCloud
-00003470: 2e66 726f 6d5f 7961 6d6c 2822 7061 7468  .from_yaml("path
-00003480: 2f74 6f2f 7961 6d6c 5f63 6f6e 6669 675f  /to/yaml_config_
-00003490: 6669 6c65 2e6a 736f 6e22 290d 0a0d 0a64  file.json")....d
-000034a0: 6174 6120 3d20 6463 2e72 6561 645f 6461  ata = dc.read_da
-000034b0: 7461 2822 436f 6d70 616e 7922 2c20 6f75  ta("Company", ou
-000034c0: 7470 7574 3d22 6c69 7374 2229 0d0a 6060  tput="list")..``
-000034d0: 600d 0a60 6461 7461 6020 7769 6c6c 2062  `..`data` will b
-000034e0: 6520 6120 606c 6973 7460 206f 6620 6064  e a `list` of `d
-000034f0: 6963 7460 7320 6173 2062 656c 6f77 3a0d  ict`s as below:.
-00003500: 0a60 6060 7079 7468 6f6e 0d0a 5b0d 0a20  .```python..[.. 
-00003510: 2020 207b 0d0a 2020 2020 2020 2020 2745     {..        'E
-00003520: 6e74 7279 4964 273a 2031 3233 3435 2c0d  ntryId': 12345,.
-00003530: 0a20 2020 2020 2020 2027 436f 6d70 616e  .        'Compan
-00003540: 794e 616d 6527 3a20 2743 6f6d 7061 6e79  yName': 'Company
-00003550: 3127 2c0d 0a20 2020 2020 2020 2027 436f  1',..        'Co
-00003560: 6d70 616e 7954 7970 6527 3a20 5b0d 0a20  mpanyType': [.. 
-00003570: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
-00003580: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00003590: 7365 714e 756d 6265 7227 3a20 332c 0d0a  seqNumber': 3,..
-000035a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035b0: 2769 7341 7574 6f50 6466 273a 2046 616c  'isAutoPdf': Fal
-000035c0: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-000035d0: 2020 2020 2027 6964 273a 2033 3139 3737       'id': 31977
-000035e0: 3830 2c0d 0a20 2020 2020 2020 2020 2020  80,..           
-000035f0: 2020 2020 2027 6e61 6d65 273a 2027 4c69       'name': 'Li
-00003600: 6d69 7465 6420 5061 7274 6e65 7227 2c0d  mited Partner',.
-00003610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003620: 2027 656e 7472 794c 6973 7449 6427 3a20   'entryListId': 
-00003630: 2d36 0d0a 2020 2020 2020 2020 2020 2020  -6..            
-00003640: 207d 0d0a 2020 2020 2020 205d 2c0d 0a20   }..       ],.. 
-00003650: 2020 207d 2c0d 0a20 2020 207b 0d0a 2020     },..    {..  
-00003660: 2020 2020 2745 6e74 7279 4964 273a 2031      'EntryId': 1
-00003670: 3233 3436 2c0d 0a20 2020 2020 2027 436f  2346,..      'Co
-00003680: 6d70 616e 794e 616d 6527 3a20 2743 6f6d  mpanyName': 'Com
-00003690: 7061 6e79 3227 2c0d 0a20 2020 2020 2027  pany2',..      '
-000036a0: 436f 6d70 616e 7954 7970 6527 3a20 5b0d  CompanyType': [.
-000036b0: 0a20 2020 2020 2020 2020 7b0d 0a20 2020  .         {..   
-000036c0: 2020 2020 2020 2020 2027 7365 714e 756d           'seqNum
-000036d0: 6265 7227 3a20 312c 0d0a 2020 2020 2020  ber': 1,..      
-000036e0: 2020 2020 2020 2769 7341 7574 6f50 6466        'isAutoPdf
-000036f0: 273a 2046 616c 7365 2c0d 0a20 2020 2020  ': False,..     
-00003700: 2020 2020 2020 2027 6964 273a 2033 3139         'id': 319
-00003710: 3737 3832 2c0d 0a20 2020 2020 2020 2020  7782,..         
-00003720: 2020 2027 6e61 6d65 273a 2027 4f70 6572     'name': 'Oper
-00003730: 6174 696e 6720 436f 6d70 616e 7927 2c0d  ating Company',.
-00003740: 0a20 2020 2020 2020 2020 2020 2027 656e  .            'en
-00003750: 7472 794c 6973 7449 6427 3a20 2d36 0d0a  tryListId': -6..
-00003760: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-00003770: 2020 5d0d 0a20 2020 207d 2c0d 0a20 2020    ]..    },..   
-00003780: 207b 0d0a 2020 2020 2020 2027 456e 7472   {..       'Entr
-00003790: 7949 6427 3a20 3132 3334 372c 0d0a 2020  yId': 12347,..  
-000037a0: 2020 2020 2020 2743 6f6d 7061 6e79 4e61        'CompanyNa
-000037b0: 6d65 273a 2027 436f 6d70 616e 7933 272c  me': 'Company3',
-000037c0: 0d0a 2020 2020 2020 2020 2743 6f6d 7061  ..        'Compa
-000037d0: 6e79 5479 7065 273a 205b 0d0a 2020 2020  nyType': [..    
-000037e0: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-000037f0: 2020 2020 2020 2020 2020 2773 6571 4e75            'seqNu
-00003800: 6d62 6572 273a 2034 2c0d 0a20 2020 2020  mber': 4,..     
-00003810: 2020 2020 2020 2020 2020 2027 6973 4175             'isAu
-00003820: 746f 5064 6627 3a20 4661 6c73 652c 0d0a  toPdf': False,..
-00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003840: 2769 6427 3a20 3331 3937 3737 392c 0d0a  'id': 3197779,..
-00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003860: 276e 616d 6527 3a20 2753 6572 7669 6365  'name': 'Service
-00003870: 2050 726f 7669 6465 7227 2c0d 0a20 2020   Provider',..   
-00003880: 2020 2020 2020 2020 2020 2020 2027 656e               'en
-00003890: 7472 794c 6973 7449 6427 3a20 2d36 0d0a  tryListId': -6..
-000038a0: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
-000038b0: 2020 2020 2020 5d0d 0a20 2020 207d 2c0d        ]..    },.
-000038c0: 0a20 5d0d 0a60 6060 0d0a 0d0a 2323 2323  . ]..```....####
-000038d0: 2320 5265 736f 6c76 696e 6720 746f 204e  # Resolving to N
-000038e0: 616d 6520 6f72 2074 6f20 4944 0d0a 3e20  ame or to ID..> 
-000038f0: 5b21 4e4f 5445 5d0d 0a3e 2054 6865 2066  [!NOTE]..> The f
-00003900: 6f6c 6c6f 7769 6e67 206d 6574 686f 6473  ollowing methods
-00003910: 206f 6e6c 7920 6170 706c 7920 746f 2077   only apply to w
-00003920: 6865 7265 2061 2060 7061 6e64 6173 2e44  here a `pandas.D
-00003930: 6174 6146 7261 6d65 6020 6973 2072 6574  ataFrame` is ret
-00003940: 7572 6e65 642e 0d0a 0d0a 4368 6f69 6365  urned.....Choice
-00003950: 2c20 5265 6665 7265 6e63 6520 616e 6420  , Reference and 
-00003960: 5573 6572 2066 6965 6c64 7320 6170 7065  User fields appe
-00003970: 6172 2061 7320 6c69 7374 7320 6f66 2064  ar as lists of d
-00003980: 6963 7469 6f6e 6172 6965 7320 6173 2073  ictionaries as s
-00003990: 6565 6e20 696e 2074 6865 205b 6162 6f76  een in the [abov
-000039a0: 6520 6578 616d 706c 655d 2823 7265 6164  e example](#read
-000039b0: 696e 672d 6461 7461 2d66 726f 6d2d 616e  ing-data-from-an
-000039c0: 2d6f 626a 6563 7429 2062 7920 6465 6661  -object) by defa
-000039d0: 756c 742e 0d0a 0d0a 546f 2072 6573 6f6c  ult.....To resol
-000039e0: 7665 2074 6865 7365 2066 6965 6c64 7320  ve these fields 
-000039f0: 746f 2061 206d 6f72 6520 7265 6164 6162  to a more readab
-00003a00: 6c65 2060 6e61 6d65 6020 7661 6c75 653a  le `name` value:
-00003a10: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a66  ....```python..f
-00003a20: 726f 6d20 6465 616c 636c 6f75 645f 7364  rom dealcloud_sd
-00003a30: 6b20 696d 706f 7274 2044 6561 6c43 6c6f  k import DealClo
-00003a40: 7564 0d0a 0d0a 6463 203d 2044 6561 6c43  ud....dc = DealC
-00003a50: 6c6f 7564 2e66 726f 6d5f 7961 6d6c 2822  loud.from_yaml("
-00003a60: 7061 7468 2f74 6f2f 7961 6d6c 5f63 6f6e  path/to/yaml_con
-00003a70: 6669 675f 6669 6c65 2e6a 736f 6e22 290d  fig_file.json").
-00003a80: 0a0d 0a64 6174 6120 3d20 6463 2e72 6561  ...data = dc.rea
-00003a90: 645f 6461 7461 2822 436f 6d70 616e 7922  d_data("Company"
-00003aa0: 2c20 7265 736f 6c76 653d 226e 616d 6522  , resolve="name"
-00003ab0: 290d 0a60 6060 0d0a 6064 6174 6160 2077  )..```..`data` w
-00003ac0: 696c 6c20 6265 2061 2060 7061 6e64 6173  ill be a `pandas
-00003ad0: 2e44 6174 6146 7261 6d65 6020 6173 2062  .DataFrame` as b
-00003ae0: 656c 6f77 3a0d 0a0d 0a7c 2045 6e74 7279  elow:....| Entry
-00003af0: 4964 207c 2043 6f6d 7061 6e79 4e61 6d65  Id | CompanyName
-00003b00: 207c 2043 6f6d 7061 6e79 5479 7065 2020   | CompanyType  
-00003b10: 2020 2020 2020 7c0d 0a7c 2d2d 2d2d 2d2d        |..|------
-00003b20: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
-00003b30: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
-00003b40: 2d2d 2d2d 2d2d 7c0d 0a7c 2031 3233 3435  ------|..| 12345
-00003b50: 2020 207c 2043 6f6d 7061 6e79 3120 2020     | Company1   
-00003b60: 207c 204c 696d 6974 6564 2050 6172 746e   | Limited Partn
-00003b70: 6572 2020 2020 7c0d 0a7c 2031 3233 3436  er    |..| 12346
-00003b80: 2020 207c 2043 6f6d 7061 6e79 3220 2020     | Company2   
-00003b90: 207c 204f 7065 7261 7469 6e67 2043 6f6d   | Operating Com
-00003ba0: 7061 6e79 2020 7c0d 0a7c 2031 3233 3437  pany  |..| 12347
-00003bb0: 2020 207c 2043 6f6d 7061 6e79 3320 2020     | Company3   
-00003bc0: 207c 204c 696d 6974 6564 2050 6172 746e   | Limited Partn
-00003bd0: 6572 2020 2020 7c0d 0a0d 0a54 6f20 7265  er    |....To re
-00003be0: 736f 6c76 6520 7468 6520 6669 656c 6473  solve the fields
-00003bf0: 2074 6f20 616e 2060 6964 6020 7661 6c75   to an `id` valu
-00003c00: 653a 0d0a 0d0a 6060 6070 7974 686f 6e0d  e:....```python.
-00003c10: 0a66 726f 6d20 6465 616c 636c 6f75 645f  .from dealcloud_
-00003c20: 7364 6b20 696d 706f 7274 2044 6561 6c43  sdk import DealC
-00003c30: 6c6f 7564 0d0a 0d0a 6463 203d 2044 6561  loud....dc = Dea
-00003c40: 6c43 6c6f 7564 2e66 726f 6d5f 7961 6d6c  lCloud.from_yaml
-00003c50: 2822 7061 7468 2f74 6f2f 7961 6d6c 5f63  ("path/to/yaml_c
-00003c60: 6f6e 6669 675f 6669 6c65 2e6a 736f 6e22  onfig_file.json"
-00003c70: 290d 0a0d 0a64 6174 6120 3d20 6463 2e72  )....data = dc.r
-00003c80: 6561 645f 6461 7461 2822 436f 6d70 616e  ead_data("Compan
-00003c90: 7922 2c20 7265 736f 6c76 653d 2269 6422  y", resolve="id"
-00003ca0: 290d 0a60 6060 0d0a 6064 6174 6160 2077  )..```..`data` w
-00003cb0: 696c 6c20 6265 2061 2060 7061 6e64 6173  ill be a `pandas
-00003cc0: 2e44 6174 6146 7261 6d65 6020 6173 2062  .DataFrame` as b
-00003cd0: 656c 6f77 3a0d 0a0d 0a7c 2045 6e74 7279  elow:....| Entry
-00003ce0: 4964 207c 2043 6f6d 7061 6e79 4e61 6d65  Id | CompanyName
-00003cf0: 207c 2043 6f6d 7061 6e79 5479 7065 207c   | CompanyType |
-00003d00: 0d0a 7c2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ..|---------|---
-00003d10: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
-00003d20: 2d2d 2d2d 2d2d 2d2d 7c0d 0a7c 2031 3233  --------|..| 123
-00003d30: 3435 2020 207c 2043 6f6d 7061 6e79 3120  45   | Company1 
-00003d40: 2020 207c 2033 3139 3737 3830 2020 2020     | 3197780    
-00003d50: 207c 0d0a 7c20 3132 3334 3620 2020 7c20   |..| 12346   | 
-00003d60: 436f 6d70 616e 7932 2020 2020 7c20 3331  Company2    | 31
-00003d70: 3937 3738 3220 2020 2020 7c0d 0a7c 2031  97782     |..| 1
-00003d80: 3233 3437 2020 207c 2043 6f6d 7061 6e79  2347   | Company
-00003d90: 3320 2020 207c 2033 3139 3737 3830 2020  3    | 3197780  
-00003da0: 2020 207c 0d0a 0d0a 2323 2323 2320 5265     |....##### Re
-00003db0: 6164 696e 6720 6120 5375 6273 6574 206f  ading a Subset o
-00003dc0: 6620 4669 656c 6473 0d0a 546f 2072 6561  f Fields..To rea
-00003dd0: 6420 6120 7370 6563 6966 6963 2073 6574  d a specific set
-00003de0: 206f 6620 6669 656c 6473 2066 726f 6d20   of fields from 
-00003df0: 616e 206f 626a 6563 742c 2070 6173 7320  an object, pass 
-00003e00: 6120 6c69 7374 206f 6620 4465 616c 436c  a list of DealCl
-00003e10: 6f75 6420 6669 656c 6420 4150 4920 6e61  oud field API na
-00003e20: 6d65 7320 746f 2074 6865 2061 7267 756d  mes to the argum
-00003e30: 656e 7420 6066 6965 6c64 7360 3a0d 0a0d  ent `fields`:...
-00003e40: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
-00003e50: 2064 6561 6c63 6c6f 7564 5f73 646b 2069   dealcloud_sdk i
-00003e60: 6d70 6f72 7420 4465 616c 436c 6f75 640d  mport DealCloud.
-00003e70: 0a0d 0a64 6320 3d20 4465 616c 436c 6f75  ...dc = DealClou
-00003e80: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
-00003e90: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
-00003ea0: 5f66 696c 652e 6a73 6f6e 2229 0d0a 0d0a  _file.json")....
-00003eb0: 6461 7461 203d 2064 632e 7265 6164 5f64  data = dc.read_d
-00003ec0: 6174 6128 2243 6f6d 7061 6e79 222c 2066  ata("Company", f
-00003ed0: 6965 6c64 733d 5b22 436f 6d70 616e 794e  ields=["CompanyN
-00003ee0: 616d 6522 5d29 0d0a 6060 600d 0a60 6461  ame"])..```..`da
-00003ef0: 7461 6020 7769 6c6c 2062 6520 6120 6070  ta` will be a `p
-00003f00: 616e 6461 732e 4461 7461 4672 616d 6560  andas.DataFrame`
-00003f10: 2061 7320 6265 6c6f 773a 0d0a 0d0a 7c20   as below:....| 
-00003f20: 456e 7472 7949 6420 7c20 436f 6d70 616e  EntryId | Compan
-00003f30: 794e 616d 6520 7c0d 0a7c 2d2d 2d2d 2d2d  yName |..|------
-00003f40: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
-00003f50: 2d7c 0d0a 7c20 3132 3334 3520 2020 7c20  -|..| 12345   | 
-00003f60: 436f 6d70 616e 7931 2020 2020 7c0d 0a7c  Company1    |..|
-00003f70: 2031 3233 3436 2020 207c 2043 6f6d 7061   12346   | Compa
-00003f80: 6e79 3220 2020 207c 0d0a 7c20 3132 3334  ny2    |..| 1234
-00003f90: 3720 2020 7c20 436f 6d70 616e 7933 2020  7   | Company3  
-00003fa0: 2020 7c0d 0a0d 0a23 2323 2323 2055 7369    |....##### Usi
-00003fb0: 6e67 2051 7565 7269 6573 2074 6f20 5265  ng Queries to Re
-00003fc0: 6164 2044 6174 610d 0a41 2071 7565 7279  ad Data..A query
-00003fd0: 2063 616e 2062 6520 7061 7373 6564 2074   can be passed t
-00003fe0: 6f20 7468 6520 4465 616c 436c 6f75 6420  o the DealCloud 
-00003ff0: 7265 7175 6573 7420 666f 7220 6461 7461  request for data
-00004000: 2074 6f20 7265 7475 726e 206d 6f72 6520   to return more 
-00004010: 7370 6563 6966 6963 2069 6e66 6f72 6d61  specific informa
-00004020: 7469 6f6e 2c20 616e 6420 7265 6475 6365  tion, and reduce
-00004030: 2074 6865 2076 6f6c 756d 6520 6f66 2069   the volume of i
-00004040: 6e63 6f6d 696e 6720 6461 7461 2e0d 0a54  ncoming data...T
-00004050: 6f20 7573 6520 6120 7175 6572 792c 2070  o use a query, p
-00004060: 6173 7320 7468 6520 7175 6572 7920 7374  ass the query st
-00004070: 7269 6e67 2074 6f20 7468 6520 6071 7565  ring to the `que
-00004080: 7279 6020 6172 6775 6d65 6e74 2e0d 0a54  ry` argument...T
-00004090: 6865 2061 7661 696c 6162 6c65 2071 7565  he available que
-000040a0: 7279 206f 7065 7261 7469 6f6e 7320 6172  ry operations ar
-000040b0: 6520 6265 6c6f 773a 0d0a 0d0a 7c20 4e61  e below:....| Na
-000040c0: 6d65 2020 2020 2020 2020 2020 207c 2051  me           | Q
-000040d0: 7565 7279 204f 7065 7261 7469 6f6e 207c  uery Operation |
-000040e0: 0d0a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..|-------------
-000040f0: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
-00004100: 2d2d 2d2d 2d7c 0d0a 7c20 4571 7561 6c73  -----|..| Equals
-00004110: 2020 2020 2020 2020 207c 2024 6571 2020           | $eq  
-00004120: 2020 2020 2020 2020 2020 207c 0d0a 7c20             |..| 
-00004130: 436f 6e74 6169 6e73 2020 2020 2020 207c  Contains       |
-00004140: 2024 636f 6e74 6169 6e73 2020 2020 2020   $contains      
-00004150: 207c 0d0a 7c20 4772 6561 7465 7220 2020   |..| Greater   
-00004160: 2020 2020 207c 2024 6774 2020 2020 2020       | $gt      
-00004170: 2020 2020 2020 207c 0d0a 7c20 4772 6561         |..| Grea
-00004180: 7465 724f 7245 7175 616c 207c 2024 6774  terOrEqual | $gt
-00004190: 6520 2020 2020 2020 2020 2020 207c 0d0a  e            |..
-000041a0: 7c20 4c65 7373 2020 2020 2020 2020 2020  | Less          
-000041b0: 207c 2024 6c74 2020 2020 2020 2020 2020   | $lt          
-000041c0: 2020 207c 0d0a 7c20 4c65 7373 4f72 4571     |..| LessOrEq
-000041d0: 7561 6c73 2020 207c 2024 6c74 6520 2020  uals   | $lte   
-000041e0: 2020 2020 2020 2020 207c 0d0a 7c20 5374           |..| St
-000041f0: 6172 7473 5769 7468 2020 2020 207c 2024  artsWith     | $
-00004200: 7374 6172 7473 7769 7468 2020 2020 207c  startswith     |
-00004210: 0d0a 7c20 496e 2020 2020 2020 2020 2020  ..| In          
-00004220: 2020 207c 2024 696e 2020 2020 2020 2020     | $in        
-00004230: 2020 2020 207c 0d0a 7c20 4265 7477 6565       |..| Betwee
-00004240: 6e20 2020 2020 2020 207c 2024 6265 7477  n        | $betw
-00004250: 6565 6e20 2020 2020 2020 207c 0d0a 7c20  een        |..| 
-00004260: 4e6f 7449 6e20 2020 2020 2020 2020 207c  NotIn          |
-00004270: 2024 6e69 6e20 2020 2020 2020 2020 2020   $nin           
-00004280: 207c 0d0a 7c20 4e6f 7445 7175 616c 546f   |..| NotEqualTo
-00004290: 2020 2020 207c 2024 6e6f 7420 2020 2020       | $not     
-000042a0: 2020 2020 2020 207c 0d0a 7c20 456e 6473         |..| Ends
-000042b0: 5769 7468 2020 2020 2020 207c 2024 656e  With       | $en
-000042c0: 6473 7769 7468 2020 2020 2020 207c 0d0a  dswith       |..
-000042d0: 7c20 4f72 2020 2020 2020 2020 2020 2020  | Or            
-000042e0: 207c 2024 6f72 2020 2020 2020 2020 2020   | $or          
-000042f0: 2020 207c 0d0a 7c20 416e 6420 2020 2020     |..| And     
-00004300: 2020 2020 2020 207c 2024 616e 6420 2020         | $and   
-00004310: 2020 2020 2020 2020 207c 0d0a 0d0a 6060           |....``
-00004320: 6070 7974 686f 6e0d 0a66 726f 6d20 6465  `python..from de
-00004330: 616c 636c 6f75 645f 7364 6b20 696d 706f  alcloud_sdk impo
-00004340: 7274 2044 6561 6c43 6c6f 7564 0d0a 0d0a  rt DealCloud....
-00004350: 6463 203d 2044 6561 6c43 6c6f 7564 2e66  dc = DealCloud.f
-00004360: 726f 6d5f 7961 6d6c 2822 7061 7468 2f74  rom_yaml("path/t
-00004370: 6f2f 7961 6d6c 5f63 6f6e 6669 675f 6669  o/yaml_config_fi
-00004380: 6c65 2e6a 736f 6e22 290d 0a0d 0a64 632e  le.json")....dc.
-00004390: 7265 6164 5f64 6174 6128 2243 6f6d 7061  read_data("Compa
-000043a0: 6e79 222c 2071 7565 7279 3d22 7b43 6f6d  ny", query="{Com
-000043b0: 7061 6e79 4e61 6d65 3a20 7b24 636f 6e74  panyName: {$cont
-000043c0: 6169 6e73 3a20 5c22 315c 227d 7d22 290d  ains: \"1\"}}").
-000043d0: 0a60 6060 0d0a 6064 6174 6160 2077 696c  .```..`data` wil
-000043e0: 6c20 6265 2061 2060 7061 6e64 6173 2e44  l be a `pandas.D
-000043f0: 6174 6146 7261 6d65 6020 6173 2062 656c  ataFrame` as bel
-00004400: 6f77 3a0d 0a0d 0a7c 2045 6e74 7279 4964  ow:....| EntryId
-00004410: 207c 2043 6f6d 7061 6e79 4e61 6d65 207c   | CompanyName |
-00004420: 2043 6f6d 7061 6e79 5479 7065 207c 0d0a   CompanyType |..
-00004430: 7c2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  |---------|-----
-00004440: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
-00004450: 2d2d 2d2d 2d2d 7c0d 0a7c 2031 3233 3435  ------|..| 12345
-00004460: 2020 207c 2043 6f6d 7061 6e79 3120 2020     | Company1   
-00004470: 207c 2033 3139 3737 3830 2020 2020 207c   | 3197780     |
-00004480: 0d0a 0d0a 536f 6d65 206f 7468 6572 2065  ....Some other e
-00004490: 7861 6d70 6c65 2071 7565 7279 2073 7472  xample query str
-000044a0: 696e 6773 2061 7265 2062 656c 6f77 3a0d  ings are below:.
-000044b0: 0a46 696c 7465 7220 6f6e 2065 7863 6c75  .Filter on exclu
-000044c0: 6469 6e67 2072 6563 6f72 6473 2077 6974  ding records wit
-000044d0: 6820 6120 7370 6563 6966 6963 2072 6566  h a specific ref
-000044e0: 6572 656e 6365 2076 616c 7565 3a0d 0a0d  erence value:...
-000044f0: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
-00004500: 2064 6561 6c63 6c6f 7564 5f73 646b 2069   dealcloud_sdk i
-00004510: 6d70 6f72 7420 4465 616c 436c 6f75 640d  mport DealCloud.
-00004520: 0a0d 0a64 6320 3d20 4465 616c 436c 6f75  ...dc = DealClou
-00004530: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
-00004540: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
-00004550: 5f66 696c 652e 6a73 6f6e 2229 0d0a 0d0a  _file.json")....
-00004560: 6463 2e72 6561 645f 6461 7461 2822 436f  dc.read_data("Co
-00004570: 6d70 616e 7922 2c20 7175 6572 793d 227b  mpany", query="{
-00004580: 436f 7665 7261 6765 5065 7273 6f6e 3a20  CoveragePerson: 
-00004590: 7b24 6e69 6e3a 205b 3537 3835 5d7d 2229  {$nin: [5785]}")
-000045a0: 0d0a 6060 600d 0a46 696c 7465 7220 7573  ..```..Filter us
-000045b0: 696e 6720 4f72 3a0d 0a0d 0a60 6060 7079  ing Or:....```py
-000045c0: 7468 6f6e 0d0a 6672 6f6d 2064 6561 6c63  thon..from dealc
-000045d0: 6c6f 7564 5f73 646b 2069 6d70 6f72 7420  loud_sdk import 
-000045e0: 4465 616c 436c 6f75 640d 0a0d 0a64 6320  DealCloud....dc 
-000045f0: 3d20 4465 616c 436c 6f75 642e 6672 6f6d  = DealCloud.from
-00004600: 5f79 616d 6c28 2270 6174 682f 746f 2f79  _yaml("path/to/y
-00004610: 616d 6c5f 636f 6e66 6967 5f66 696c 652e  aml_config_file.
-00004620: 6a73 6f6e 2229 0d0a 0d0a 6463 2e72 6561  json")....dc.rea
-00004630: 645f 6461 7461 2822 436f 6d70 616e 7922  d_data("Company"
-00004640: 2c20 7175 6572 793d 227b 246f 723a 205b  , query="{$or: [
-00004650: 7b43 6f6d 7061 6e79 4e61 6d65 3a20 5c22  {CompanyName: \"
-00004660: 4465 616c 436c 6f75 645c 227d 2c7b 436f  DealCloud\"},{Co
-00004670: 6d70 616e 794e 616d 653a 205c 2241 5049  mpanyName: \"API
-00004680: 2045 6e74 7279 5c22 7d5d 7d22 290d 0a60   Entry\"}]}")..`
-00004690: 6060 0d0a 0d0a 2323 2323 2052 6561 6469  ``....#### Readi
-000046a0: 6e67 2044 6174 6120 6672 6f6d 2061 2056  ng Data from a V
-000046b0: 6965 770d 0a54 6f20 7265 6164 2064 6174  iew..To read dat
-000046c0: 6120 6672 6f6d 2061 2076 6965 7720 7769  a from a view wi
-000046d0: 7468 2049 443a 2060 3132 3334 3560 0d0a  th ID: `12345`..
-000046e0: 0d0a 4578 616d 706c 653a 0d0a 0d0a 6060  ..Example:....``
-000046f0: 6070 7974 686f 6e0d 0a66 726f 6d20 6465  `python..from de
-00004700: 616c 636c 6f75 645f 7364 6b20 696d 706f  alcloud_sdk impo
-00004710: 7274 2044 6561 6c43 6c6f 7564 0d0a 0d0a  rt DealCloud....
-00004720: 6463 203d 2044 6561 6c43 6c6f 7564 2e66  dc = DealCloud.f
-00004730: 726f 6d5f 7961 6d6c 2822 7061 7468 2f74  rom_yaml("path/t
-00004740: 6f2f 7961 6d6c 5f63 6f6e 6669 675f 6669  o/yaml_config_fi
-00004750: 6c65 2e6a 736f 6e22 290d 0a0d 0a64 6174  le.json")....dat
-00004760: 6120 3d20 6463 2e72 6561 645f 6461 7461  a = dc.read_data
-00004770: 2876 6965 775f 6964 3d31 3233 3435 290d  (view_id=12345).
-00004780: 0a60 6060 0d0a 416c 7465 726e 6174 6976  .```..Alternativ
-00004790: 656c 792c 2069 6620 7468 6520 7669 6577  ely, if the view
-000047a0: 2069 7320 6e61 6d65 643a 2022 4d79 2043   is named: "My C
-000047b0: 6f6d 7061 6e79 2056 6965 7722 3a0d 0a0d  ompany View":...
-000047c0: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
-000047d0: 2064 6561 6c63 6c6f 7564 5f73 646b 2069   dealcloud_sdk i
-000047e0: 6d70 6f72 7420 4465 616c 436c 6f75 640d  mport DealCloud.
-000047f0: 0a0d 0a64 6320 3d20 4465 616c 436c 6f75  ...dc = DealClou
-00004800: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
-00004810: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
-00004820: 5f66 696c 652e 6a73 6f6e 2229 0d0a 0d0a  _file.json")....
-00004830: 6461 7461 203d 2064 632e 7265 6164 5f64  data = dc.read_d
-00004840: 6174 6128 7669 6577 5f69 643d 224d 7920  ata(view_id="My 
-00004850: 436f 6d70 616e 7920 5669 6577 2229 0d0a  Company View")..
-00004860: 6060 600d 0a0d 0a60 6461 7461 6020 7769  ```....`data` wi
-00004870: 6c6c 2062 6520 6120 6070 616e 6461 732e  ll be a `pandas.
-00004880: 4461 7461 4672 616d 6560 2061 7320 6265  DataFrame` as be
-00004890: 6c6f 773a 0d0a 0d0a 7c20 456e 7472 7949  low:....| EntryI
-000048a0: 6420 7c20 436f 6d70 616e 794e 616d 6520  d | CompanyName 
-000048b0: 7c20 436f 6d70 616e 7954 7970 6520 2020  | CompanyType   
-000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004910: 2020 2020 2020 2020 207c 0d0a 7c2d 2d2d           |..|---
-00004920: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00004930: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
-00004940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0d0a  -------------|..
-000049a0: 7c20 3132 3334 3520 2020 7c20 436f 6d70  | 12345   | Comp
-000049b0: 616e 7931 2020 2020 7c20 5b7b 2773 6571  any1    | [{'seq
-000049c0: 4e75 6d62 6572 273a 2033 2c20 2769 7341  Number': 3, 'isA
-000049d0: 7574 6f50 6466 273a 2046 616c 7365 2c20  utoPdf': False, 
-000049e0: 2769 6427 3a20 3331 3937 3738 302c 2027  'id': 3197780, '
-000049f0: 6e61 6d65 273a 2027 4c69 6d69 7465 6420  name': 'Limited 
-00004a00: 5061 7274 6e65 7227 2c20 2765 6e74 7279  Partner', 'entry
-00004a10: 4c69 7374 4964 273a 202d 367d 5d20 2020  ListId': -6}]   
-00004a20: 207c 0d0a 7c20 3132 3334 3620 2020 7c20   |..| 12346   | 
-00004a30: 436f 6d70 616e 7932 2020 2020 7c20 5b7b  Company2    | [{
-00004a40: 2773 6571 4e75 6d62 6572 273a 2031 2c20  'seqNumber': 1, 
-00004a50: 2769 7341 7574 6f50 6466 273a 2046 616c  'isAutoPdf': Fal
-00004a60: 7365 2c20 2769 6427 3a20 3331 3937 3738  se, 'id': 319778
-00004a70: 322c 2027 6e61 6d65 273a 2027 4f70 6572  2, 'name': 'Oper
-00004a80: 6174 696e 6720 436f 6d70 616e 7927 2c20  ating Company', 
-00004a90: 2765 6e74 7279 4c69 7374 4964 273a 202d  'entryListId': -
-00004aa0: 367d 5d20 207c 0d0a 7c20 3132 3334 3720  6}]  |..| 12347 
-00004ab0: 2020 7c20 436f 6d70 616e 7933 2020 2020    | Company3    
-00004ac0: 7c20 5b7b 2773 6571 4e75 6d62 6572 273a  | [{'seqNumber':
-00004ad0: 2033 2c20 2769 7341 7574 6f50 6466 273a   3, 'isAutoPdf':
-00004ae0: 2046 616c 7365 2c20 2769 6427 3a20 3331   False, 'id': 31
-00004af0: 3937 3738 302c 2027 6e61 6d65 273a 2027  97780, 'name': '
-00004b00: 4c69 6d69 7465 6420 5061 7274 6e65 7227  Limited Partner'
-00004b10: 2c20 2765 6e74 7279 4c69 7374 4964 273a  , 'entryListId':
-00004b20: 202d 367d 5d20 2020 207c 0d0a 0d0a 2323   -6}]    |....##
-00004b30: 2323 2320 5573 696e 6720 6120 4669 6c74  ### Using a Filt
-00004b40: 6572 2057 6865 6e20 5265 6164 696e 6720  er When Reading 
-00004b50: 5669 6577 2044 6174 610d 0a57 6865 6e20  View Data..When 
-00004b60: 7265 6164 696e 6720 6461 7461 2066 726f  reading data fro
-00004b70: 6d20 6120 7669 6577 2c20 7768 6963 6820  m a view, which 
-00004b80: 6861 7320 2253 7570 706c 7920 5661 6c75  has "Supply Valu
-00004b90: 6520 4c61 7465 7222 2066 696c 7465 7273  e Later" filters
-00004ba0: 2063 6f6e 6669 6775 7265 642c 2074 6865   configured, the
-00004bb0: 2066 696c 7465 7220 7661 6c75 6573 2063   filter values c
-00004bc0: 616e 2062 6520 7072 6f76 6964 6564 2062  an be provided b
-00004bd0: 7920 7061 7373 696e 6720 7468 656d 2074  y passing them t
-00004be0: 6f20 7468 6520 6076 6965 775f 6669 6c74  o the `view_filt
-00004bf0: 6572 6020 6172 6775 6d65 6e74 2069 6e20  er` argument in 
-00004c00: 6120 606c 6973 7460 206f 6620 6064 6963  a `list` of `dic
-00004c10: 7460 732e 2046 6f72 206d 6f72 6520 696e  t`s. For more in
-00004c20: 666f 726d 6174 696f 6e20 6f6e 2074 6865  formation on the
-00004c30: 6972 2066 6f72 6d61 742c 2070 6c65 6173  ir format, pleas
-00004c40: 6520 7365 6520 7468 6520 5b41 5049 2044  e see the [API D
-00004c50: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-00004c60: 7470 733a 2f2f 6170 692e 646f 6373 2e64  tps://api.docs.d
-00004c70: 6561 6c63 6c6f 7564 2e63 6f6d 2f64 6f63  ealcloud.com/doc
-00004c80: 732f 6461 7461 2f72 6f77 732f 7669 6577  s/data/rows/view
-00004c90: 5f64 6574 6169 6c73 292e 0d0a 0d0a 466f  _details).....Fo
-00004ca0: 7220 4578 616d 706c 652c 2073 7570 706c  r Example, suppl
-00004cb0: 7969 6e67 2061 2022 436f 6d70 616e 7954  ying a "CompanyT
-00004cc0: 7970 6522 2066 696c 7465 7220 7661 6c75  ype" filter valu
-00004cd0: 6520 746f 2066 696c 7465 7220 666f 7220  e to filter for 
-00004ce0: 6f6e 6c79 2022 4c69 6d69 7465 6420 5061  only "Limited Pa
-00004cf0: 7274 6e65 7222 2063 6f6d 7061 6e69 6573  rtner" companies
-00004d00: 3a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  :....```python..
-00004d10: 6672 6f6d 2064 6561 6c63 6c6f 7564 5f73  from dealcloud_s
-00004d20: 646b 2069 6d70 6f72 7420 4465 616c 436c  dk import DealCl
-00004d30: 6f75 640d 0a0d 0a64 6320 3d20 4465 616c  oud....dc = Deal
-00004d40: 436c 6f75 642e 6672 6f6d 5f79 616d 6c28  Cloud.from_yaml(
-00004d50: 2270 6174 682f 746f 2f79 616d 6c5f 636f  "path/to/yaml_co
-00004d60: 6e66 6967 5f66 696c 652e 6a73 6f6e 2229  nfig_file.json")
-00004d70: 0d0a 0d0a 6461 7461 203d 2064 632e 7265  ....data = dc.re
-00004d80: 6164 5f64 6174 6128 0d0a 2020 2076 6965  ad_data(..   vie
-00004d90: 775f 6964 203d 2022 4d79 2043 6f6d 7061  w_id = "My Compa
-00004da0: 6e79 2056 6965 7722 2c0d 0a20 2020 7669  ny View",..   vi
-00004db0: 6577 5f66 696c 7465 7220 3d20 5b0d 0a20  ew_filter = [.. 
-00004dc0: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-00004dd0: 2022 636f 6c75 6d6e 223a 2243 6f6d 7061   "column":"Compa
-00004de0: 6e79 5479 7065 222c 0d0a 2020 2020 2020  nyType",..      
-00004df0: 2020 2022 7661 6c75 6522 3a20 5b33 3139     "value": [319
-00004e00: 3737 3830 5d0d 0a20 2020 2020 207d 0d0a  7780]..      }..
-00004e10: 2020 205d 0d0a 290d 0a60 6060 0d0a 6064     ]..)..```..`d
-00004e20: 6174 6160 2077 696c 6c20 6265 2061 2060  ata` will be a `
-00004e30: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
-00004e40: 6020 6173 2062 656c 6f77 3a0d 0a0d 0a7c  ` as below:....|
-00004e50: 2045 6e74 7279 4964 207c 2043 6f6d 7061   EntryId | Compa
-00004e60: 6e79 4e61 6d65 207c 2043 6f6d 7061 6e79  nyName | Company
-00004e70: 5479 7065 2020 2020 2020 2020 2020 2020  Type            
-00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ed0: 7c0d 0a7c 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  |..|---------|--
-00004ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
-00004ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004f10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004f50: 2d2d 2d2d 7c0d 0a7c 2031 3233 3435 2020  ----|..| 12345  
-00004f60: 207c 2043 6f6d 7061 6e79 3120 2020 207c   | Company1    |
-00004f70: 205b 7b27 7365 714e 756d 6265 7227 3a20   [{'seqNumber': 
-00004f80: 332c 2027 6973 4175 746f 5064 6627 3a20  3, 'isAutoPdf': 
-00004f90: 4661 6c73 652c 2027 6964 273a 2033 3139  False, 'id': 319
-00004fa0: 3737 3830 2c20 276e 616d 6527 3a20 274c  7780, 'name': 'L
-00004fb0: 696d 6974 6564 2050 6172 746e 6572 272c  imited Partner',
-00004fc0: 2027 656e 7472 794c 6973 7449 6427 3a20   'entryListId': 
-00004fd0: 2d36 7d5d 2020 2020 7c0d 0a7c 2031 3233  -6}]    |..| 123
-00004fe0: 3437 2020 207c 2043 6f6d 7061 6e79 3320  47   | Company3 
-00004ff0: 2020 207c 205b 7b27 7365 714e 756d 6265     | [{'seqNumbe
-00005000: 7227 3a20 332c 2027 6973 4175 746f 5064  r': 3, 'isAutoPd
-00005010: 6627 3a20 4661 6c73 652c 2027 6964 273a  f': False, 'id':
-00005020: 2033 3139 3737 3830 2c20 276e 616d 6527   3197780, 'name'
-00005030: 3a20 274c 696d 6974 6564 2050 6172 746e  : 'Limited Partn
-00005040: 6572 272c 2027 656e 7472 794c 6973 7449  er', 'entryListI
-00005050: 6427 3a20 2d36 7d5d 2020 2020 7c0d 0a0d  d': -6}]    |...
-00005060: 0a0d 0a23 2323 2043 7265 6174 652c 2055  ...### Create, U
-00005070: 7064 6174 6520 616e 6420 5570 7365 7274  pdate and Upsert
-00005080: 2044 6174 610d 0a60 4465 616c 436c 6f75   Data..`DealClou
-00005090: 642e 696e 7365 7274 5f64 6174 6128 2960  d.insert_data()`
-000050a0: 2c20 6044 6561 6c43 6c6f 7564 2e75 7064  , `DealCloud.upd
-000050b0: 6174 655f 6461 7461 2829 602c 2060 4465  ate_data()`, `De
-000050c0: 616c 436c 6f75 642e 7570 7365 7274 5f64  alCloud.upsert_d
-000050d0: 6174 6128 2960 2061 7265 206d 6574 686f  ata()` are metho
-000050e0: 6473 2077 6869 6368 2070 726f 7669 6465  ds which provide
-000050f0: 2074 6865 2061 6269 6c69 7479 2074 6f20   the ability to 
-00005100: 6372 6561 7465 2c20 7570 6461 7465 2061  create, update a
-00005110: 6e64 2075 7073 6572 7420 6461 7461 2072  nd upsert data r
-00005120: 6573 7065 6374 6976 656c 792e 0d0a 5468  espectively...Th
-00005130: 6573 6520 6d65 7468 6f64 7320 6861 7665  ese methods have
-00005140: 2074 6865 2073 616d 6520 6172 6775 6d65   the same argume
-00005150: 6e74 2070 6174 7465 726e 3a0d 0a0d 0a41  nt pattern:....A
-00005160: 7267 756d 656e 7473 3a0d 0a2d 206f 626a  rguments:..- obj
-00005170: 6563 745f 6170 695f 6e61 6d65 2060 7374  ect_api_name `st
-00005180: 7260 3a20 7468 6520 6f62 6a65 6374 2041  r`: the object A
-00005190: 5049 206e 616d 6520 746f 2077 7269 7465  PI name to write
-000051a0: 2064 6174 6120 746f 0d0a 2d20 6461 7461   data to..- data
-000051b0: 2060 556e 696f 6e5b 6c69 7374 5b64 6963   `Union[list[dic
-000051c0: 745d 2c20 7064 2e44 6174 6146 7261 6d65  t], pd.DataFrame
-000051d0: 5d60 3a20 7468 6520 6461 7461 2074 6f20  ]`: the data to 
-000051e0: 6265 2073 656e 7420 746f 2044 6561 6c43  be sent to DealC
-000051f0: 6c6f 7564 2e0d 0a2d 2075 7365 5f64 6561  loud...- use_dea
-00005200: 6c63 6c6f 7564 5f69 6473 2060 626f 6f6c  lcloud_ids `bool
-00005210: 603a 2044 6566 6175 6c74 2069 7320 6054  `: Default is `T
-00005220: 7275 6560 2049 6620 6054 7275 6560 2c20  rue` If `True`, 
-00005230: 4465 616c 436c 6f75 6420 456e 7472 7949  DealCloud EntryI
-00005240: 6473 206d 7573 7420 6265 2075 7365 6420  ds must be used 
-00005250: 746f 2072 6566 6572 656e 6365 2072 6563  to reference rec
-00005260: 6f72 6473 2061 6e64 2063 686f 6963 6520  ords and choice 
-00005270: 7661 6c75 6573 2e20 4966 2060 4661 6c73  values. If `Fals
-00005280: 6560 2c20 7573 6520 6120 636f 6c75 6d6e  e`, use a column
-00005290: 2061 7320 6120 6c6f 6f6b 7570 2c20 6465   as a lookup, de
-000052a0: 6669 6e65 6420 6279 2074 6865 206c 6f6f  fined by the loo
-000052b0: 6b75 705f 636f 6c75 6d6e 2061 7267 756d  kup_column argum
-000052c0: 656e 742e 0d0a 2d20 6c6f 6f6b 7570 5f63  ent...- lookup_c
-000052d0: 6f6c 756d 6e20 6073 7472 603a 2069 6620  olumn `str`: if 
-000052e0: 6075 7365 5f64 6561 6c63 6c6f 7564 5f69  `use_dealcloud_i
-000052f0: 6473 6020 6973 2060 4661 6c73 6560 2c20  ds` is `False`, 
-00005300: 7468 6973 2064 6566 696e 6573 2074 6865  this defines the
-00005310: 2063 6f6c 756d 6e20 746f 2062 6520 7573   column to be us
-00005320: 6564 2061 7320 6120 6c6f 6f6b 7570 2e0d  ed as a lookup..
-00005330: 0a2d 206f 7574 7075 7460 7374 7260 3a20  .- output`str`: 
-00005340: 606c 6973 7460 206f 7220 6070 616e 6461  `list` or `panda
-00005350: 7360 2c20 6465 6669 6e65 7320 7468 6520  s`, defines the 
-00005360: 6f75 7470 7574 2066 6f72 6d61 7420 7265  output format re
-00005370: 7475 726e 6564 2066 726f 6d20 7468 6520  turned from the 
-00005380: 6675 6e63 7469 6f6e 0d0a 0d0a 5265 7475  function....Retu
-00005390: 726e 733a 0d0a 2020 2060 556e 696f 6e5b  rns:..   `Union[
-000053a0: 6c69 7374 5b64 6963 745d 2c20 7064 2e44  list[dict], pd.D
-000053b0: 6174 6146 7261 6d65 5d60 3a20 7468 6520  ataFrame]`: the 
-000053c0: 6461 7461 2072 6574 7572 6e65 6420 6672  data returned fr
-000053d0: 6f6d 2074 6865 2064 6174 6120 6f70 6572  om the data oper
-000053e0: 6174 696f 6e2e 0d0a 0d0a 3e20 5b21 494d  ation.....> [!IM
-000053f0: 504f 5254 414e 545d 0d0a 3e20 5768 656e  PORTANT]..> When
-00005400: 206e 6f74 2075 7369 6e67 2060 7573 655f   not using `use_
-00005410: 6465 616c 636c 6f75 645f 6964 7360 2c20  dealcloud_ids`, 
-00005420: 666f 7220 5265 6665 7265 6e63 6520 6669  for Reference fi
-00005430: 656c 6473 2c20 7265 6665 7265 6e63 6520  elds, reference 
-00005440: 6279 2072 6563 6f72 6420 456e 7472 7949  by record EntryI
-00005450: 642e 2046 6f72 2063 686f 6963 6520 6669  d. For choice fi
-00005460: 656c 6473 2c20 7573 6520 7468 6520 6368  elds, use the ch
-00005470: 6f69 6365 2076 616c 7565 2049 442e 2046  oice value ID. F
-00005480: 6f72 2075 7365 7220 6669 656c 6473 2c20  or user fields, 
-00005490: 7573 6520 7468 6520 7573 6572 2049 4420  use the user ID 
-000054a0: 2866 726f 6d20 6044 6561 6c43 6c6f 7564  (from `DealCloud
-000054b0: 2e67 6574 5f75 7365 7273 2829 6029 2e20  .get_users()`). 
-000054c0: 0d0a 3e20 5768 656e 2075 7369 6e67 2060  ..> When using `
-000054d0: 7573 655f 6465 616c 636c 6f75 645f 6964  use_dealcloud_id
-000054e0: 7360 2c20 666f 7220 5265 6665 7265 6e63  s`, for Referenc
-000054f0: 6520 6669 656c 6473 2c20 7265 6665 7265  e fields, refere
-00005500: 6e63 6520 6279 2074 6865 206c 6f6f 6b75  nce by the looku
-00005510: 7020 636f 6c75 6d6e 206f 6e20 7468 6520  p column on the 
-00005520: 7265 6665 7265 6e63 6564 206f 626a 6563  referenced objec
-00005530: 742e 2046 6f72 2063 686f 6963 6520 6669  t. For choice fi
-00005540: 656c 6473 2c20 7573 6520 7468 6520 6368  elds, use the ch
-00005550: 6f69 6365 2066 6965 6c64 2064 6973 706c  oice field displ
-00005560: 6179 206e 616d 652e 2046 6f72 2075 7365  ay name. For use
-00005570: 7220 6669 656c 6473 2c20 7573 6520 7468  r fields, use th
-00005580: 6520 7573 6572 2065 6d61 696c 2061 6464  e user email add
-00005590: 7265 7373 2e0d 0a0d 0a23 2323 2323 2046  ress.....##### F
-000055a0: 6965 6c64 204d 6170 7069 6e67 0d0a 416c  ield Mapping..Al
-000055b0: 6c20 636f 6c75 6d6e 7320 7061 7373 6564  l columns passed
-000055c0: 2074 6f20 7468 6520 6372 6561 7465 2c20   to the create, 
-000055d0: 7570 6461 7465 2061 6e64 2075 7073 6572  update and upser
-000055e0: 7420 6d65 7468 6f64 7320 6d75 7374 206d  t methods must m
-000055f0: 6174 6368 2062 7920 5f41 5049 204e 616d  atch by _API Nam
-00005600: 655f 2e20 4966 2061 2063 6f6c 756d 6e20  e_. If a column 
-00005610: 7061 7373 6564 2074 6f20 7468 6520 6d65  passed to the me
-00005620: 7468 6f64 2064 6f65 7320 6e6f 7420 6578  thod does not ex
-00005630: 6973 7420 696e 2074 6865 2073 6974 6520  ist in the site 
-00005640: 6279 2041 5049 206e 616d 652c 2074 6865  by API name, the
-00005650: 6e20 6120 604b 6579 4572 726f 7260 2077  n a `KeyError` w
-00005660: 696c 6c20 6265 2072 6169 7365 643a 0d0a  ill be raised:..
-00005670: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
-00005680: 6d20 6465 616c 636c 6f75 645f 7364 6b20  m dealcloud_sdk 
-00005690: 696d 706f 7274 2044 6561 6c43 6c6f 7564  import DealCloud
-000056a0: 0d0a 0d0a 6463 203d 2044 6561 6c43 6c6f  ....dc = DealClo
-000056b0: 7564 2e66 726f 6d5f 7961 6d6c 2822 7061  ud.from_yaml("pa
-000056c0: 7468 2f74 6f2f 7961 6d6c 5f63 6f6e 6669  th/to/yaml_confi
-000056d0: 675f 6669 6c65 2e6a 736f 6e22 290d 0a0d  g_file.json")...
-000056e0: 0a74 6f5f 7365 6e64 203d 205b 0d0a 2020  .to_send = [..  
-000056f0: 7b0d 0a20 2020 2020 2022 436f 6d70 616e  {..      "Compan
-00005700: 794e 616d 6522 3a20 2254 6573 7420 436f  yName": "Test Co
-00005710: 6d70 616e 7920 3122 2c0d 0a20 2020 2020  mpany 1",..     
-00005720: 2022 556e 6d61 7070 6162 6c65 436f 6c75   "UnmappableColu
-00005730: 6d6e 223a 2022 466f 6f22 2c0d 0a20 207d  mn": "Foo",..  }
-00005740: 0d0a 5d0d 0a72 6573 706f 6e73 6573 203d  ..]..responses =
-00005750: 2064 632e 696e 7365 7274 5f64 6174 6128   dc.insert_data(
-00005760: 2243 6f6d 7061 6e79 222c 2074 6f5f 7365  "Company", to_se
-00005770: 6e64 290d 0a60 6060 0d0a 5769 6c6c 2052  nd)..```..Will R
-00005780: 6574 7572 6e0d 0a60 6060 6261 7368 0d0a  eturn..```bash..
-00005790: 5472 6163 6562 6163 6b2e 2e2e 0d0a 4b65  Traceback.....Ke
-000057a0: 7945 7272 6f72 3a20 226d 6170 7069 6e67  yError: "mapping
-000057b0: 2065 7272 6f72 2c20 636f 756c 6420 6e6f   error, could no
-000057c0: 7420 6d61 703a 205b 2755 6e6d 6170 7061  t map: ['Unmappa
-000057d0: 626c 6543 6f6c 756d 6e27 5d22 0d0a 6060  bleColumn']"..``
-000057e0: 600d 0a0d 0a23 2323 2320 4372 6561 7465  `....#### Create
-000057f0: 2044 6174 610d 0a45 7861 6d70 6c65 2c20   Data..Example, 
-00005800: 746f 2069 6e73 6572 7420 6461 7461 2069  to insert data i
-00005810: 6e74 6f20 7468 6520 2243 6f6d 7061 6e79  nto the "Company
-00005820: 2220 6f62 6a65 6374 2066 726f 6d20 6120  " object from a 
-00005830: 6c69 7374 3a0d 0a0d 0a60 6060 7079 7468  list:....```pyth
-00005840: 6f6e 0d0a 6672 6f6d 2064 6561 6c63 6c6f  on..from dealclo
-00005850: 7564 5f73 646b 2069 6d70 6f72 7420 4465  ud_sdk import De
-00005860: 616c 436c 6f75 640d 0a0d 0a64 6320 3d20  alCloud....dc = 
-00005870: 4465 616c 436c 6f75 642e 6672 6f6d 5f79  DealCloud.from_y
-00005880: 616d 6c28 2270 6174 682f 746f 2f79 616d  aml("path/to/yam
-00005890: 6c5f 636f 6e66 6967 5f66 696c 652e 6a73  l_config_file.js
-000058a0: 6f6e 2229 0d0a 0d0a 746f 5f73 656e 6420  on")....to_send 
-000058b0: 3d20 5b0d 0a20 207b 0d0a 2020 2020 2020  = [..  {..      
-000058c0: 2243 6f6d 7061 6e79 4e61 6d65 223a 2022  "CompanyName": "
-000058d0: 5465 7374 2043 6f6d 7061 6e79 2031 222c  Test Company 1",
-000058e0: 0d0a 2020 2020 2020 2243 6f6d 7061 6e79  ..      "Company
-000058f0: 5479 7065 223a 2031 3233 3435 2c0d 0a20  Type": 12345,.. 
-00005900: 2020 2020 2022 4275 7369 6e65 7373 4465       "BusinessDe
-00005910: 7363 7269 7074 696f 6e22 3a20 2248 6572  scription": "Her
-00005920: 6520 6973 2061 2062 7573 696e 6573 7320  e is a business 
-00005930: 6465 7363 7269 7074 696f 6e22 2c0d 0a20  description",.. 
-00005940: 2020 2020 2022 5365 6374 6f72 223a 2031       "Sector": 1
-00005950: 3433 3231 2c0d 0a20 207d 0d0a 5d0d 0a72  4321,..  }..]..r
-00005960: 6573 706f 6e73 6573 203d 2064 632e 696e  esponses = dc.in
-00005970: 7365 7274 5f64 6174 6128 2243 6f6d 7061  sert_data("Compa
-00005980: 6e79 222c 2074 6f5f 7365 6e64 290d 0a60  ny", to_send)..`
-00005990: 6060 0d0a 4966 2073 7563 6365 7373 6675  ``..If successfu
-000059a0: 6c2c 2060 7265 7370 6f6e 7365 7360 2077  l, `responses` w
-000059b0: 696c 6c20 636f 6e74 6169 6e20 7468 6520  ill contain the 
-000059c0: 6265 6c6f 7720 2d20 6e6f 7465 2074 6861  below - note tha
-000059d0: 7420 6045 6e74 7279 4964 6020 6973 206e  t `EntryId` is n
-000059e0: 6f77 2069 6e63 6c75 6465 643a 0d0a 6060  ow included:..``
-000059f0: 6070 7974 686f 6e0d 0a5b 0d0a 2020 2020  `python..[..    
-00005a00: 7b0d 0a20 2020 2020 2020 2022 456e 7472  {..        "Entr
-00005a10: 7949 6422 3a20 3233 3435 3637 2c0d 0a20  yId": 234567,.. 
-00005a20: 2020 2020 2020 2022 436f 6d70 616e 794e         "CompanyN
-00005a30: 616d 6522 3a20 2254 6573 7420 436f 6d70  ame": "Test Comp
-00005a40: 616e 7920 3122 2c0d 0a20 2020 2020 2020  any 1",..       
-00005a50: 2022 436f 6d70 616e 7954 7970 6522 3a20   "CompanyType": 
-00005a60: 3132 3334 352c 0d0a 2020 2020 2020 2020  12345,..        
-00005a70: 2242 7573 696e 6573 7344 6573 6372 6970  "BusinessDescrip
-00005a80: 7469 6f6e 223a 2022 4865 7265 2069 7320  tion": "Here is 
-00005a90: 6120 6275 7369 6e65 7373 2064 6573 6372  a business descr
-00005aa0: 6970 7469 6f6e 222c 0d0a 2020 2020 2020  iption",..      
-00005ab0: 2020 2253 6563 746f 7222 3a20 3134 3332    "Sector": 1432
-00005ac0: 312c 0d0a 2020 2020 7d0d 0a5d 0d0a 6060  1,..    }..]..``
-00005ad0: 600d 0a45 7861 6d70 6c65 2c20 746f 2069  `..Example, to i
-00005ae0: 6e73 6572 7420 6461 7461 2069 6e74 6f20  nsert data into 
-00005af0: 7468 6520 2243 6f6d 7061 6e79 2220 6f62  the "Company" ob
-00005b00: 6a65 6374 2066 726f 6d20 6120 4353 562c  ject from a CSV,
-00005b10: 2075 7369 6e67 2060 7061 6e64 6173 603a   using `pandas`:
-00005b20: 0d0a 0d0a 4353 5620 4669 6c65 2028 6063  ....CSV File (`c
-00005b30: 6f6d 7061 6e79 2e63 7376 6029 3a0d 0a0d  ompany.csv`):...
-00005b40: 0a7c 2043 6f6d 7061 6e79 4e61 6d65 207c  .| CompanyName |
-00005b50: 2043 6f6d 7061 6e79 5479 7065 207c 0d0a   CompanyType |..
-00005b60: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  |-------------|-
-00005b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0d 0a7c  ------------|..|
-00005b80: 2043 6f6d 7061 6e79 3120 2020 207c 2033   Company1    | 3
-00005b90: 3139 3737 3830 2020 2020 207c 0d0a 7c20  197780     |..| 
-00005ba0: 436f 6d70 616e 7932 2020 2020 7c20 3331  Company2    | 31
-00005bb0: 3937 3738 3220 2020 2020 7c0d 0a7c 2043  97782     |..| C
-00005bc0: 6f6d 7061 6e79 3320 2020 207c 2033 3139  ompany3    | 319
-00005bd0: 3737 3830 2020 2020 207c 0d0a 0d0a 6060  7780     |....``
-00005be0: 6070 7974 686f 6e0d 0a69 6d70 6f72 7420  `python..import 
-00005bf0: 7061 6e64 6173 2061 7320 7064 0d0a 6672  pandas as pd..fr
-00005c00: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
-00005c10: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
-00005c20: 640d 0a0d 0a64 6320 3d20 4465 616c 436c  d....dc = DealCl
-00005c30: 6f75 642e 6672 6f6d 5f79 616d 6c28 2270  oud.from_yaml("p
-00005c40: 6174 682f 746f 2f79 616d 6c5f 636f 6e66  ath/to/yaml_conf
-00005c50: 6967 5f66 696c 652e 6a73 6f6e 2229 0d0a  ig_file.json")..
-00005c60: 0d0a 746f 5f73 656e 6420 3d20 7064 2e72  ..to_send = pd.r
-00005c70: 6561 645f 6373 7628 2263 6f6d 7061 6e79  ead_csv("company
-00005c80: 2e63 7376 2229 0d0a 7265 7370 6f6e 7365  .csv")..response
-00005c90: 7320 3d20 6463 2e69 6e73 6572 745f 6461  s = dc.insert_da
-00005ca0: 7461 2822 436f 6d70 616e 7922 2c20 746f  ta("Company", to
-00005cb0: 5f73 656e 6429 0d0a 6060 600d 0a45 7861  _send)..```..Exa
-00005cc0: 6d70 6c65 2c20 746f 2069 6e73 6572 7420  mple, to insert 
-00005cd0: 6461 7461 2069 6e74 6f20 7468 6520 2243  data into the "C
-00005ce0: 6f6d 7061 6e79 2220 6f62 6a65 6374 2075  ompany" object u
-00005cf0: 7369 6e67 2022 4578 7465 726e 616c 5379  sing "ExternalSy
-00005d00: 7374 656d 4944 2220 6173 2061 206c 6f6f  stemID" as a loo
-00005d10: 6b75 7020 636f 6c75 6d6e 3a0d 0a0d 0a60  kup column:....`
-00005d20: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2064  ``python..from d
-00005d30: 6561 6c63 6c6f 7564 5f73 646b 2069 6d70  ealcloud_sdk imp
-00005d40: 6f72 7420 4465 616c 436c 6f75 640d 0a0d  ort DealCloud...
-00005d50: 0a64 6320 3d20 4465 616c 436c 6f75 642e  .dc = DealCloud.
-00005d60: 6672 6f6d 5f79 616d 6c28 2270 6174 682f  from_yaml("path/
-00005d70: 746f 2f79 616d 6c5f 636f 6e66 6967 5f66  to/yaml_config_f
-00005d80: 696c 652e 6a73 6f6e 2229 0d0a 0d0a 746f  ile.json")....to
-00005d90: 5f73 656e 6420 3d20 5b0d 0a20 207b 0d0a  _send = [..  {..
-00005da0: 2020 2020 2020 2243 6f6d 7061 6e79 4e61        "CompanyNa
-00005db0: 6d65 223a 2022 5465 7374 2043 6f6d 7061  me": "Test Compa
-00005dc0: 6e79 2031 222c 0d0a 2020 2020 2020 2243  ny 1",..      "C
-00005dd0: 6f6d 7061 6e79 5479 7065 223a 2022 4f70  ompanyType": "Op
-00005de0: 6572 6174 696e 6720 436f 6d70 616e 7922  erating Company"
-00005df0: 2c0d 0a20 2020 2020 2022 4275 7369 6e65  ,..      "Busine
-00005e00: 7373 4465 7363 7269 7074 696f 6e22 3a20  ssDescription": 
-00005e10: 2248 6572 6520 6973 2061 2062 7573 696e  "Here is a busin
-00005e20: 6573 7320 6465 7363 7269 7074 696f 6e22  ess description"
-00005e30: 2c0d 0a20 2020 2020 2022 5365 6374 6f72  ,..      "Sector
-00005e40: 223a 2022 3631 3245 3946 4634 2d31 4438  ": "612E9FF4-1D8
-00005e50: 432d 3431 4237 2d42 3845 442d 3244 3143  C-41B7-B8ED-2D1C
-00005e60: 3135 3234 3034 3334 222c 0d0a 2020 7d0d  15240434",..  }.
-00005e70: 0a5d 0d0a 0d0a 7265 7370 6f6e 7365 7320  .]....responses 
-00005e80: 3d20 6463 2e69 6e73 6572 745f 6461 7461  = dc.insert_data
-00005e90: 280d 0a20 2020 6f62 6a65 6374 5f61 7069  (..   object_api
-00005ea0: 5f6e 616d 6520 3d20 2243 6f6d 7061 6e79  _name = "Company
-00005eb0: 222c 0d0a 2020 2064 6174 6120 3d20 746f  ",..   data = to
-00005ec0: 5f73 656e 642c 0d0a 2020 2075 7365 5f64  _send,..   use_d
-00005ed0: 6561 6c63 6c6f 7564 5f69 6473 203d 2046  ealcloud_ids = F
-00005ee0: 616c 7365 2c0d 0a20 2020 6c6f 6f6b 7570  alse,..   lookup
-00005ef0: 5f63 6f6c 756d 6e20 3d20 2245 7874 6572  _column = "Exter
-00005f00: 6e61 6c53 7973 7465 6d49 4422 0d0a 290d  nalSystemID"..).
-00005f10: 0a60 6060 0d0a 2323 2323 2055 7064 6174  .```..#### Updat
-00005f20: 6520 4461 7461 0d0a 546f 2075 7064 6174  e Data..To updat
-00005f30: 6520 6578 6973 7469 6e67 2073 6974 6520  e existing site 
-00005f40: 6461 7461 2c20 7468 6520 7072 6f63 6573  data, the proces
-00005f50: 7320 6973 2073 696d 696c 6172 2c20 6578  s is similar, ex
-00005f60: 6365 7074 206f 626a 6563 7473 206d 7573  cept objects mus
-00005f70: 7420 696e 636c 7564 6520 6045 6e74 7279  t include `Entry
-00005f80: 4964 602c 206f 7220 6120 7661 6c69 6420  Id`, or a valid 
-00005f90: 7072 696d 6172 7920 6b65 7920 6279 2060  primary key by `
-00005fa0: 6c6f 6f6b 7570 5f63 6f6c 756d 6e60 2e0d  lookup_column`..
-00005fb0: 0a0d 0a45 7861 6d70 6c65 2c20 746f 2075  ...Example, to u
-00005fc0: 7064 6174 6520 6461 7461 2069 6e20 7468  pdate data in th
-00005fd0: 6520 2243 6f6d 7061 6e79 2220 6f62 6a65  e "Company" obje
-00005fe0: 6374 2066 726f 6d20 6120 6c69 7374 3a0d  ct from a list:.
-00005ff0: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
-00006000: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
-00006010: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
-00006020: 640d 0a0d 0a64 6320 3d20 4465 616c 436c  d....dc = DealCl
-00006030: 6f75 642e 6672 6f6d 5f79 616d 6c28 2270  oud.from_yaml("p
-00006040: 6174 682f 746f 2f79 616d 6c5f 636f 6e66  ath/to/yaml_conf
-00006050: 6967 5f66 696c 652e 6a73 6f6e 2229 0d0a  ig_file.json")..
-00006060: 0d0a 746f 5f73 656e 6420 3d20 5b0d 0a20  ..to_send = [.. 
-00006070: 207b 0d0a 2020 2020 2020 2245 6e74 7279   {..      "Entry
-00006080: 4964 223a 2032 3334 3536 372c 0d0a 2020  Id": 234567,..  
-00006090: 2020 2020 2242 7573 696e 6573 7344 6573      "BusinessDes
-000060a0: 6372 6970 7469 6f6e 223a 2022 4865 7265  cription": "Here
-000060b0: 2069 7320 616e 2075 7064 6174 6564 2062   is an updated b
-000060c0: 7573 696e 6573 7320 6465 7363 7269 7074  usiness descript
-000060d0: 696f 6e21 222c 0d0a 2020 7d0d 0a5d 0d0a  ion!",..  }..]..
-000060e0: 7265 7370 6f6e 7365 7320 3d20 6463 2e69  responses = dc.i
-000060f0: 6e73 6572 745f 6461 7461 2822 436f 6d70  nsert_data("Comp
-00006100: 616e 7922 2c20 746f 5f73 656e 6429 0d0a  any", to_send)..
-00006110: 6060 600d 0a49 6620 7375 6363 6573 7366  ```..If successf
-00006120: 756c 2c20 6072 6573 706f 6e73 6573 6020  ul, `responses` 
-00006130: 7769 6c6c 2063 6f6e 7461 696e 2074 6865  will contain the
-00006140: 2062 656c 6f77 3a0d 0a60 6060 7079 7468   below:..```pyth
-00006150: 6f6e 0d0a 5b0d 0a20 2020 207b 0d0a 2020  on..[..    {..  
-00006160: 2020 2020 2020 2245 6e74 7279 4964 223a        "EntryId":
-00006170: 2032 3334 3536 372c 0d0a 2020 2020 2020   234567,..      
-00006180: 2020 2243 6f6d 7061 6e79 4e61 6d65 223a    "CompanyName":
-00006190: 2022 5465 7374 2043 6f6d 7061 6e79 2031   "Test Company 1
-000061a0: 222c 0d0a 2020 2020 2020 2020 2243 6f6d  ",..        "Com
-000061b0: 7061 6e79 5479 7065 223a 2031 3233 3435  panyType": 12345
-000061c0: 2c0d 0a20 2020 2020 2020 2022 4275 7369  ,..        "Busi
-000061d0: 6e65 7373 4465 7363 7269 7074 696f 6e22  nessDescription"
-000061e0: 3a20 2248 6572 6520 6973 2061 6e20 7570  : "Here is an up
-000061f0: 6461 7465 6420 6275 7369 6e65 7373 2064  dated business d
-00006200: 6573 6372 6970 7469 6f6e 2122 2c0d 0a20  escription!",.. 
-00006210: 2020 2020 2020 2022 5365 6374 6f72 223a         "Sector":
-00006220: 2031 3433 3231 2c0d 0a20 2020 207d 0d0a   14321,..    }..
-00006230: 5d0d 0a60 6060 0d0a 4578 616d 706c 652c  ]..```..Example,
-00006240: 2074 6f20 7570 6461 7465 2064 6174 6120   to update data 
-00006250: 696e 2074 6865 2022 436f 6d70 616e 7922  in the "Company"
-00006260: 206f 626a 6563 7420 6672 6f6d 2061 206c   object from a l
-00006270: 6973 742c 2075 7369 6e67 2074 6865 2060  ist, using the `
-00006280: 6c6f 6f6b 7570 5f63 6f6c 756d 6e60 2c20  lookup_column`, 
-00006290: 6045 7874 6572 6e61 6c53 7973 7465 6d49  `ExternalSystemI
-000062a0: 6460 3a0d 0a0d 0a60 6060 7079 7468 6f6e  d`:....```python
-000062b0: 0d0a 6672 6f6d 2064 6561 6c63 6c6f 7564  ..from dealcloud
-000062c0: 5f73 646b 2069 6d70 6f72 7420 4465 616c  _sdk import Deal
-000062d0: 436c 6f75 640d 0a0d 0a64 6320 3d20 4465  Cloud....dc = De
-000062e0: 616c 436c 6f75 642e 6672 6f6d 5f79 616d  alCloud.from_yam
-000062f0: 6c28 2270 6174 682f 746f 2f79 616d 6c5f  l("path/to/yaml_
-00006300: 636f 6e66 6967 5f66 696c 652e 6a73 6f6e  config_file.json
-00006310: 2229 0d0a 0d0a 746f 5f73 656e 6420 3d20  ")....to_send = 
-00006320: 5b0d 0a20 207b 0d0a 2020 2020 2020 2245  [..  {..      "E
-00006330: 7874 6572 6e61 6c53 7973 7465 6d49 6422  xternalSystemId"
-00006340: 3a20 2246 3632 3841 4643 382d 3533 3243  : "F628AFC8-532C
-00006350: 2d34 3036 432d 4244 4536 2d41 3738 3246  -406C-BDE6-A782F
-00006360: 3033 3530 3844 3522 2c0d 0a20 2020 2020  03508D5",..     
-00006370: 2022 4275 7369 6e65 7373 4465 7363 7269   "BusinessDescri
-00006380: 7074 696f 6e22 3a20 2248 6572 6520 6973  ption": "Here is
-00006390: 2061 6e20 7570 6461 7465 6420 6275 7369   an updated busi
-000063a0: 6e65 7373 2064 6573 6372 6970 7469 6f6e  ness description
-000063b0: 2122 2c0d 0a20 207d 0d0a 5d0d 0a72 6573  !",..  }..]..res
-000063c0: 706f 6e73 6573 203d 2064 632e 696e 7365  ponses = dc.inse
-000063d0: 7274 5f64 6174 6128 0d0a 2020 206f 626a  rt_data(..   obj
-000063e0: 6563 745f 6170 695f 6e61 6d65 203d 2022  ect_api_name = "
-000063f0: 436f 6d70 616e 7922 2c0d 0a20 2020 6461  Company",..   da
-00006400: 7461 203d 2074 6f5f 7365 6e64 2c0d 0a20  ta = to_send,.. 
-00006410: 2020 7573 655f 6465 616c 636c 6f75 645f    use_dealcloud_
-00006420: 6964 7320 3d20 4661 6c73 652c 0d0a 2020  ids = False,..  
-00006430: 206c 6f6f 6b75 705f 636f 6c75 6d6e 203d   lookup_column =
-00006440: 2022 4578 7465 726e 616c 5379 7374 656d   "ExternalSystem
-00006450: 4964 220d 0a29 0d0a 6060 600d 0a0d 0a23  Id"..)..```....#
-00006460: 2323 2320 5570 7365 7274 2044 6174 610d  ### Upsert Data.
-00006470: 0a55 7073 6572 7469 6e67 2064 6174 6120  .Upserting data 
-00006480: 6973 2061 206d 6574 686f 6420 7468 6174  is a method that
-00006490: 2063 6f6d 6269 6e65 7320 696e 7365 7274   combines insert
-000064a0: 2061 6e64 2075 7064 6174 652e 2049 6620   and update. If 
-000064b0: 6120 7265 636f 7264 2065 7869 7374 7320  a record exists 
-000064c0: 616e 6420 6361 6e20 6265 2066 6f75 6e64  and can be found
-000064d0: 2062 7920 6045 6e74 7279 4964 6020 6f72   by `EntryId` or
-000064e0: 2061 2060 6c6f 6f6b 7570 5f63 6f6c 756d   a `lookup_colum
-000064f0: 6e60 2074 6865 6e20 6974 2077 696c 6c20  n` then it will 
-00006500: 6265 2075 7064 6174 6564 2c20 6966 206e  be updated, if n
-00006510: 6f74 2c20 6974 2077 696c 6c20 6265 2063  ot, it will be c
-00006520: 7265 6174 6564 206e 6577 2e0d 0a0d 0a45  reated new.....E
-00006530: 7861 6d70 6c65 2c20 746f 2075 7073 6572  xample, to upser
-00006540: 7420 6461 7461 2069 6e20 7468 6520 2243  t data in the "C
-00006550: 6f6d 7061 6e79 2220 6f62 6a65 6374 2066  ompany" object f
-00006560: 726f 6d20 6120 6c69 7374 3a0d 0a0d 0a60  rom a list:....`
-00006570: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2064  ``python..from d
-00006580: 6561 6c63 6c6f 7564 5f73 646b 2069 6d70  ealcloud_sdk imp
-00006590: 6f72 7420 4465 616c 436c 6f75 640d 0a0d  ort DealCloud...
-000065a0: 0a64 6320 3d20 4465 616c 436c 6f75 642e  .dc = DealCloud.
-000065b0: 6672 6f6d 5f79 616d 6c28 2270 6174 682f  from_yaml("path/
-000065c0: 746f 2f79 616d 6c5f 636f 6e66 6967 5f66  to/yaml_config_f
-000065d0: 696c 652e 6a73 6f6e 2229 0d0a 0d0a 746f  ile.json")....to
-000065e0: 5f73 656e 6420 3d20 5b0d 0a20 2020 7b0d  _send = [..   {.
-000065f0: 0a20 2020 2022 456e 7472 7949 6422 3a20  .    "EntryId": 
-00006600: 3233 3435 3637 2c20 200d 0a20 2020 2022  234567,  ..    "
-00006610: 436f 6d70 616e 794e 616d 6522 3a20 2254  CompanyName": "T
-00006620: 6573 7420 436f 6d70 616e 7920 3122 2c0d  est Company 1",.
-00006630: 0a20 2020 2022 436f 6d70 616e 7954 7970  .    "CompanyTyp
-00006640: 6522 3a20 3132 3334 352c 0d0a 2020 2020  e": 12345,..    
-00006650: 2242 7573 696e 6573 7344 6573 6372 6970  "BusinessDescrip
-00006660: 7469 6f6e 223a 2022 4865 7265 2069 7320  tion": "Here is 
-00006670: 616e 2075 7064 6174 6564 2062 7573 696e  an updated busin
-00006680: 6573 7320 6465 7363 7269 7074 696f 6e22  ess description"
-00006690: 2c0d 0a20 2020 2022 5365 6374 6f72 223a  ,..    "Sector":
-000066a0: 2031 3433 3231 2c0d 0a20 2020 7d2c 0d0a   14321,..   },..
-000066b0: 2020 207b 0d0a 2020 2020 2243 6f6d 7061     {..    "Compa
-000066c0: 6e79 4e61 6d65 223a 2022 5465 7374 2043  nyName": "Test C
-000066d0: 6f6d 7061 6e79 2032 222c 0d0a 2020 2020  ompany 2",..    
-000066e0: 2243 6f6d 7061 6e79 5479 7065 223a 2031  "CompanyType": 1
-000066f0: 3233 3435 2c0d 0a20 2020 2022 4275 7369  2345,..    "Busi
-00006700: 6e65 7373 4465 7363 7269 7074 696f 6e22  nessDescription"
-00006710: 3a20 2248 6572 6520 6973 2061 2062 7573  : "Here is a bus
-00006720: 696e 6573 7320 6465 7363 7269 7074 696f  iness descriptio
-00006730: 6e20 666f 7220 6120 6e65 7720 636f 6d70  n for a new comp
-00006740: 616e 7922 2c0d 0a20 2020 2022 5365 6374  any",..    "Sect
-00006750: 6f72 223a 2031 3433 3231 2c0d 0a20 2020  or": 14321,..   
-00006760: 7d2c 0d0a 5d0d 0a72 6573 706f 6e73 6573  },..]..responses
-00006770: 203d 2064 632e 696e 7365 7274 5f64 6174   = dc.insert_dat
-00006780: 6128 2243 6f6d 7061 6e79 222c 2074 6f5f  a("Company", to_
-00006790: 7365 6e64 290d 0a60 6060 0d0a 4966 2073  send)..```..If s
-000067a0: 7563 6365 7373 6675 6c2c 2060 7265 7370  uccessful, `resp
-000067b0: 6f6e 7365 7360 2077 696c 6c20 636f 6e74  onses` will cont
-000067c0: 6169 6e20 7468 6520 6265 6c6f 772c 206e  ain the below, n
-000067d0: 6f74 6520 7468 6174 2074 6865 2022 5465  ote that the "Te
-000067e0: 7374 2043 6f6d 7061 6e79 2032 2220 6e6f  st Company 2" no
-000067f0: 7720 6861 7320 616e 2060 456e 7472 7949  w has an `EntryI
-00006800: 6460 2061 7320 6974 2068 6173 2062 6565  d` as it has bee
-00006810: 6e20 6372 6561 7465 643a 0d0a 6060 6070  n created:..```p
-00006820: 7974 686f 6e0d 0a5b 0d0a 2020 207b 0d0a  ython..[..   {..
-00006830: 2020 2020 2245 6e74 7279 4964 223a 2032      "EntryId": 2
-00006840: 3334 3536 372c 2020 0d0a 2020 2020 2243  34567,  ..    "C
-00006850: 6f6d 7061 6e79 4e61 6d65 223a 2022 5465  ompanyName": "Te
-00006860: 7374 2043 6f6d 7061 6e79 2031 222c 0d0a  st Company 1",..
-00006870: 2020 2020 2243 6f6d 7061 6e79 5479 7065      "CompanyType
-00006880: 223a 2031 3233 3435 2c0d 0a20 2020 2022  ": 12345,..    "
-00006890: 4275 7369 6e65 7373 4465 7363 7269 7074  BusinessDescript
-000068a0: 696f 6e22 3a20 2248 6572 6520 6973 2061  ion": "Here is a
-000068b0: 6e20 7570 6461 7465 6420 6275 7369 6e65  n updated busine
-000068c0: 7373 2064 6573 6372 6970 7469 6f6e 222c  ss description",
-000068d0: 0d0a 2020 2020 2253 6563 746f 7222 3a20  ..    "Sector": 
-000068e0: 3134 3332 312c 0d0a 2020 207d 2c0d 0a20  14321,..   },.. 
-000068f0: 2020 7b0d 0a20 2020 2022 456e 7472 7949    {..    "EntryI
-00006900: 6422 3a20 3233 3435 3638 2c0d 0a20 2020  d": 234568,..   
-00006910: 2022 436f 6d70 616e 794e 616d 6522 3a20   "CompanyName": 
-00006920: 2254 6573 7420 436f 6d70 616e 7920 3222  "Test Company 2"
-00006930: 2c0d 0a20 2020 2022 436f 6d70 616e 7954  ,..    "CompanyT
-00006940: 7970 6522 3a20 3132 3334 352c 0d0a 2020  ype": 12345,..  
-00006950: 2020 2242 7573 696e 6573 7344 6573 6372    "BusinessDescr
-00006960: 6970 7469 6f6e 223a 2022 4865 7265 2069  iption": "Here i
-00006970: 7320 6120 6275 7369 6e65 7373 2064 6573  s a business des
-00006980: 6372 6970 7469 6f6e 2066 6f72 2061 206e  cription for a n
-00006990: 6577 2063 6f6d 7061 6e79 222c 0d0a 2020  ew company",..  
-000069a0: 2020 2253 6563 746f 7222 3a20 3134 3332    "Sector": 1432
-000069b0: 312c 0d0a 2020 207d 2c0d 0a5d 0d0a 6060  1,..   },..]..``
-000069c0: 600d 0a23 2323 2320 556e 6465 7273 7461  `..#### Understa
-000069d0: 6e64 696e 6720 4572 726f 7273 0d0a 5468  nding Errors..Th
-000069e0: 6520 6461 7461 206f 7065 7261 7469 6f6e  e data operation
-000069f0: 206d 6574 686f 6473 2072 6169 7365 2065   methods raise e
-00006a00: 7272 6f72 7320 696e 2061 206e 756d 6265  rrors in a numbe
-00006a10: 7220 6f66 2077 6179 732c 2077 6865 6e20  r of ways, when 
-00006a20: 6075 7365 5f64 6561 6c63 6c6f 7564 5f69  `use_dealcloud_i
-00006a30: 6473 6020 6973 2060 4661 6c73 6560 2c20  ds` is `False`, 
-00006a40: 6572 726f 7273 2061 7265 2066 6564 2062  errors are fed b
-00006a50: 6163 6b20 6672 6f6d 2074 6865 2041 5049  ack from the API
-00006a60: 2069 6e74 6f20 7468 6520 6461 7461 2072   into the data r
-00006a70: 6574 7572 6e65 6420 6672 6f6d 2074 6865  eturned from the
-00006a80: 2066 756e 6374 696f 6e2e 0d0a 4578 616d   function...Exam
-00006a90: 706c 652c 2069 6620 7468 6520 7365 6374  ple, if the sect
-00006aa0: 6f72 2031 3233 3435 2064 6f65 7320 6e6f  or 12345 does no
-00006ab0: 7420 6578 6973 743a 0d0a 0d0a 6060 6070  t exist:....```p
-00006ac0: 7974 686f 6e0d 0a66 726f 6d20 6465 616c  ython..from deal
-00006ad0: 636c 6f75 645f 7364 6b20 696d 706f 7274  cloud_sdk import
-00006ae0: 2044 6561 6c43 6c6f 7564 0d0a 0d0a 6463   DealCloud....dc
-00006af0: 203d 2044 6561 6c43 6c6f 7564 2e66 726f   = DealCloud.fro
-00006b00: 6d5f 7961 6d6c 2822 7061 7468 2f74 6f2f  m_yaml("path/to/
-00006b10: 7961 6d6c 5f63 6f6e 6669 675f 6669 6c65  yaml_config_file
-00006b20: 2e6a 736f 6e22 290d 0a0d 0a74 6f5f 7365  .json")....to_se
-00006b30: 6e64 203d 205b 0d0a 2020 2020 7b27 436f  nd = [..    {'Co
-00006b40: 6d70 616e 794e 616d 6527 3a20 2754 4553  mpanyName': 'TES
-00006b50: 545f 5550 4441 5445 4427 2c20 2253 6563  T_UPDATED', "Sec
-00006b60: 746f 7222 3a20 3132 3334 357d 0d0a 5d0d  tor": 12345}..].
-00006b70: 0a72 6573 706f 6e73 6573 203d 2064 632e  .responses = dc.
-00006b80: 696e 7365 7274 5f64 6174 6128 2257 4a5f  insert_data("WJ_
-00006b90: 436f 6d70 616e 7922 2c20 746f 5f73 656e  Company", to_sen
-00006ba0: 6429 0d0a 6060 600d 0a60 7265 7370 6f6e  d)..```..`respon
-00006bb0: 7365 7360 2077 696c 6c20 636f 6e74 6169  ses` will contai
-00006bc0: 6e2e 0d0a 6060 6070 7974 686f 6e0d 0a5b  n...```python..[
-00006bd0: 7b27 456e 7472 7949 6427 3a20 2d31 2c0d  {'EntryId': -1,.
-00006be0: 0a20 2027 436f 6d70 616e 794e 616d 6527  .  'CompanyName'
-00006bf0: 3a20 2754 4553 545f 5550 4441 5445 4427  : 'TEST_UPDATED'
-00006c00: 2c0d 0a20 2027 5365 6374 6f72 273a 204e  ,..  'Sector': N
-00006c10: 6f6e 652c 0d0a 2020 2745 7272 6f72 7327  one,..  'Errors'
-00006c20: 3a20 5b7b 2766 6965 6c64 273a 2027 5365  : [{'field': 'Se
-00006c30: 6374 6f72 272c 0d0a 2020 2020 2763 6f64  ctor',..    'cod
-00006c40: 6527 3a20 3530 3036 2c0d 0a20 2020 2027  e': 5006,..    '
-00006c50: 6465 7363 7269 7074 696f 6e27 3a20 274f  description': 'O
-00006c60: 6e65 206f 7220 6d6f 7265 2072 6566 6572  ne or more refer
-00006c70: 656e 6365 6420 656e 7472 6965 7320 6172  enced entries ar
-00006c80: 6520 6e6f 7420 7661 6c69 6420 666f 7220  e not valid for 
-00006c90: 7468 6973 2066 6965 6c64 2e27 7d5d 7d5d  this field.'}]}]
-00006ca0: 0d0a 6060 600d 0a3e 205b 214e 4f54 455d  ..```..> [!NOTE]
-00006cb0: 0d0a 3e20 496e 2074 6869 7320 6361 7365  ..> In this case
-00006cc0: 2c20 7468 6520 7265 636f 7264 2068 6173  , the record has
-00006cd0: 206e 6f74 2062 6565 6e20 6372 6561 7465   not been create
-00006ce0: 6420 696e 2074 6865 2073 6974 652e 2057  d in the site. W
-00006cf0: 6865 6e20 6d75 6c74 6970 6c65 2072 6563  hen multiple rec
-00006d00: 6f72 6473 2061 7265 2074 7279 696e 6720  ords are trying 
-00006d10: 746f 2062 6520 6d61 6465 2061 6e64 2061  to be made and a
-00006d20: 6e79 206f 6e65 2066 6169 6c73 2069 6e20  ny one fails in 
-00006d30: 7468 6973 2077 6179 2c20 6e6f 6e65 206f  this way, none o
-00006d40: 6620 7468 6520 7265 636f 7264 7320 696e  f the records in
-00006d50: 2074 6861 7420 6772 6f75 7020 7769 6c6c   that group will
-00006d60: 2062 6520 6372 6561 7465 642e 2057 6865   be created. Whe
-00006d70: 6e20 6120 6c61 7267 6520 766f 6c75 6d65  n a large volume
-00006d80: 206f 6620 7265 636f 7264 7320 6172 6520   of records are 
-00006d90: 6265 696e 6720 6372 6561 7465 642c 2060  being created, `
-00006da0: 4465 616c 436c 6f75 6460 2068 616e 646c  DealCloud` handl
-00006db0: 6573 2062 7265 616b 696e 6720 7468 6520  es breaking the 
-00006dc0: 6c61 7267 6520 766f 6c75 6d65 206f 6620  large volume of 
-00006dd0: 6461 7461 2069 6e74 6f20 6d75 6c74 6970  data into multip
-00006de0: 6c65 2070 6167 6573 2e20 496e 2074 6869  le pages. In thi
-00006df0: 7320 6361 7365 2c20 7768 6572 6520 7468  s case, where th
-00006e00: 6572 6520 6973 2061 6e20 6572 726f 7220  ere is an error 
-00006e10: 6f6e 2061 2072 6563 6f72 6420 696e 2061  on a record in a
-00006e20: 2070 6167 652c 2061 6c6c 206f 6620 7468   page, all of th
-00006e30: 6520 7265 636f 7264 7320 696e 2074 6861  e records in tha
-00006e40: 7420 7061 6765 2077 696c 6c20 6e6f 7420  t page will not 
-00006e50: 6265 2063 7265 6174 6564 2f75 7064 6174  be created/updat
-00006e60: 6564 2e0d 0a0d 0a57 6865 6e20 6075 7365  ed.....When `use
-00006e70: 5f64 6561 6c63 6c6f 7564 5f69 6473 6020  _dealcloud_ids` 
-00006e80: 6973 2060 5472 7565 602c 2061 6e64 206c  is `True`, and l
-00006e90: 6f6f 6b75 7020 7661 6c75 6573 2061 7265  ookup values are
-00006ea0: 2075 7365 642c 2074 6865 2063 7265 6174   used, the creat
-00006eb0: 652f 7570 6461 7465 2f75 7073 6572 7420  e/update/upsert 
-00006ec0: 6d65 7468 6f64 7320 6172 6520 6c65 7373  methods are less
-00006ed0: 2070 726f 6e65 2074 6f20 2266 6169 6c69   prone to "faili
-00006ee0: 6e67 2220 6572 726f 7273 2e20 5468 6973  ng" errors. This
-00006ef0: 2069 7320 6265 6361 7573 652c 2077 6865   is because, whe
-00006f00: 6e20 6120 7661 6c75 6520 6973 2062 6569  n a value is bei
-00006f10: 6e67 2072 6573 6f6c 7665 6420 7468 726f  ng resolved thro
-00006f20: 7567 6820 6120 606c 6f6f 6b75 705f 636f  ugh a `lookup_co
-00006f30: 6c75 6d6e 602c 2061 2076 616c 7565 2074  lumn`, a value t
-00006f40: 6861 7420 6361 6e6e 6f74 2062 6520 666f  hat cannot be fo
-00006f50: 756e 6420 7769 6c6c 2072 6573 756c 7420  und will result 
-00006f60: 696e 2061 6e20 6572 726f 7220 6265 696e  in an error bein
-00006f70: 6720 6c6f 6767 6564 2074 6f20 7468 6520  g logged to the 
-00006f80: 636f 6e66 6967 7572 6564 206c 6f67 6765  configured logge
-00006f90: 722e 2048 6f77 6576 6572 2c20 6173 2074  r. However, as t
-00006fa0: 6865 2072 6563 6f72 6420 7072 6f67 7265  he record progre
-00006fb0: 7373 6573 2c20 7468 6520 756e 2d72 6573  sses, the un-res
-00006fc0: 6f6c 7661 626c 6520 7661 6c75 6520 7769  olvable value wi
-00006fd0: 6c6c 2073 696d 706c 7920 6265 2062 6c61  ll simply be bla
-00006fe0: 6e6b 2e20 5468 6520 6c6f 6773 2061 7070  nk. The logs app
-00006ff0: 6561 7220 6173 2062 656c 6f77 3a0d 0a0d  ear as below:...
-00007000: 0a46 6f72 2063 686f 6963 6520 6669 656c  .For choice fiel
-00007010: 6473 3a0d 0a60 6060 6261 7368 0d0a 4552  ds:..```bash..ER
-00007020: 524f 523a 2043 686f 6963 6520 6d61 7070  ROR: Choice mapp
-00007030: 696e 6720 6572 726f 7220 6f6e 3a20 7b6f  ing error on: {o
-00007040: 626a 6563 747d 2c20 7b66 6965 6c64 7d2c  bject}, {field},
-00007050: 2063 6f75 6c64 206e 6f74 2066 696e 6420   could not find 
-00007060: 7661 6c75 653a 207b 7661 6c75 657d 0d0a  value: {value}..
-00007070: 6060 600d 0a46 6f72 2072 6566 6572 656e  ```..For referen
-00007080: 6365 2066 6965 6c64 733a 0d0a 6060 6062  ce fields:..```b
-00007090: 6173 680d 0a45 5252 4f52 3a20 5265 6665  ash..ERROR: Refe
-000070a0: 7265 6e63 6520 6d61 7070 696e 6720 6572  rence mapping er
-000070b0: 726f 7220 6f6e 3a20 7b6f 626a 6563 747d  ror on: {object}
-000070c0: 2c20 7b66 6965 6c64 7d2c 2063 6f75 6c64  , {field}, could
-000070d0: 206e 6f74 2066 696e 6420 7661 6c75 653a   not find value:
-000070e0: 207b 7661 6c75 657d 0d0a 6060 600d 0a46   {value}..```..F
-000070f0: 6f72 2075 7365 7220 6669 656c 6473 3a0d  or user fields:.
-00007100: 0a60 6060 6261 7368 0d0a 4552 524f 523a  .```bash..ERROR:
-00007110: 2055 7365 7220 6d61 7070 696e 6720 6572   User mapping er
-00007120: 726f 7220 6f6e 3a20 7b6f 626a 6563 747d  ror on: {object}
-00007130: 2c20 7b66 6965 6c64 7d2c 2063 6f75 6c64  , {field}, could
-00007140: 206e 6f74 2066 696e 6420 7661 6c75 653a   not find value:
-00007150: 207b 7661 6c75 657d 0d0a 6060 600d 0a0d   {value}..```...
-00007160: 0a57 6865 6e20 7573 696e 6720 6044 6561  .When using `Dea
-00007170: 6c43 6c6f 7564 2e75 7064 6174 655f 6461  lCloud.update_da
-00007180: 7461 2829 602c 2069 6620 616e 2060 456e  ta()`, if an `En
-00007190: 7472 7949 6460 2063 616e 6e6f 7420 6265  tryId` cannot be
-000071a0: 206c 6f63 6174 6564 2c20 796f 7520 7769   located, you wi
-000071b0: 6c6c 2073 6565 2074 6865 2066 6f6c 6c6f  ll see the follo
-000071c0: 7769 6e67 2065 7272 6f72 3a0d 0a60 6060  wing error:..```
-000071d0: 6261 7368 0d0a 4552 524f 523a 2050 7269  bash..ERROR: Pri
-000071e0: 6d61 7279 204b 6579 2065 7272 6f72 206f  mary Key error o
-000071f0: 6e20 6f62 6a65 6374 3a20 7b6f 626a 6563  n object: {objec
-00007200: 747d 2c20 7265 636f 7264 2066 6f75 6e64  t}, record found
-00007210: 2077 6974 686f 7574 2027 456e 7472 7949   without 'EntryI
-00007220: 6427 2066 6965 6c64 2e0d 0a60 6060 0d0a  d' field...```..
-00007230: 0d0a 2323 2320 4465 6c65 7465 2044 6174  ..### Delete Dat
-00007240: 610d 0a60 4465 616c 436c 6f75 642e 6465  a..`DealCloud.de
-00007250: 6c65 7465 5f64 6174 6128 2960 2070 726f  lete_data()` pro
-00007260: 7669 6465 7320 7468 6520 6162 696c 6974  vides the abilit
-00007270: 7920 746f 2064 656c 6574 6520 6461 7461  y to delete data
-00007280: 2066 726f 6d20 616e 206f 626a 6563 7420   from an object 
-00007290: 6279 2074 6865 2060 456e 7472 7949 6460  by the `EntryId`
-000072a0: 2e20 546f 2075 7365 2069 742c 2073 696d  . To use it, sim
-000072b0: 706c 7920 7061 7373 2074 6865 206f 626a  ply pass the obj
-000072c0: 6563 7420 6170 6920 6e61 6d65 2074 6f20  ect api name to 
-000072d0: 7468 6520 606f 626a 6563 745f 6170 695f  the `object_api_
-000072e0: 6e61 6d65 6020 6172 6775 6d65 6e74 0d0a  name` argument..
-000072f0: 616e 6420 6120 606c 6973 7460 206f 6620  and a `list` of 
-00007300: 6045 6e74 7279 4964 6073 2074 6f20 7468  `EntryId`s to th
-00007310: 6520 6072 6563 6f72 6473 6020 6172 6775  e `records` argu
-00007320: 6d65 6e74 2e0d 0a0d 0a45 7861 6d70 6c65  ment.....Example
-00007330: 2074 6f20 6465 6c65 7465 2074 776f 2072   to delete two r
-00007340: 6563 6f72 6473 2077 6974 6820 7468 6520  ecords with the 
-00007350: 456e 7472 7949 6473 2060 3132 3334 3531  EntryIds `123451
-00007360: 6020 616e 6420 6031 3233 3436 603a 0d0a  ` and `12346`:..
-00007370: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
-00007380: 6d20 6465 616c 636c 6f75 645f 7364 6b20  m dealcloud_sdk 
-00007390: 696d 706f 7274 2044 6561 6c43 6c6f 7564  import DealCloud
-000073a0: 0d0a 0d0a 6463 203d 2044 6561 6c43 6c6f  ....dc = DealClo
-000073b0: 7564 2e66 726f 6d5f 7961 6d6c 2822 7061  ud.from_yaml("pa
-000073c0: 7468 2f74 6f2f 7961 6d6c 5f63 6f6e 6669  th/to/yaml_confi
-000073d0: 675f 6669 6c65 2e6a 736f 6e22 290d 0a0d  g_file.json")...
-000073e0: 0a72 6573 706f 6e73 6520 3d20 6463 2e64  .response = dc.d
-000073f0: 656c 6574 655f 6461 7461 280d 0a20 2020  elete_data(..   
-00007400: 6f62 6a65 6374 5f61 7069 5f6e 616d 653d  object_api_name=
-00007410: 2243 6f6d 7061 6e79 222c 0d0a 2020 2072  "Company",..   r
-00007420: 6563 6f72 6473 3d5b 3132 3334 352c 2031  ecords=[12345, 1
-00007430: 3233 3436 5d0d 0a29 0d0a 6060 600d 0a60  2346]..)..```..`
-00007440: 7265 7370 6f6e 7365 6020 7769 6c6c 2063  response` will c
-00007450: 6f6e 7461 696e 3a0d 0a60 6060 7079 7468  ontain:..```pyth
-00007460: 6f6e 0d0a 5b0d 0a20 2020 7b27 656e 7472  on..[..   {'entr
-00007470: 7949 6427 3a20 3132 3334 352c 2027 6669  yId': 12345, 'fi
-00007480: 656c 6449 6427 3a20 302c 2027 726f 7749  eldId': 0, 'rowI
-00007490: 6427 3a20 3439 3335 3635 302c 2027 6973  d': 4935650, 'is
-000074a0: 4e6f 4461 7461 273a 2046 616c 7365 7d2c  NoData': False},
-000074b0: 0d0a 2020 207b 2765 6e74 7279 4964 273a  ..   {'entryId':
-000074c0: 2031 3233 3436 2c20 2766 6965 6c64 4964   12346, 'fieldId
-000074d0: 273a 2030 2c20 2772 6f77 4964 273a 2034  ': 0, 'rowId': 4
-000074e0: 3933 3536 3530 2c20 2769 734e 6f44 6174  935650, 'isNoDat
-000074f0: 6127 3a20 4661 6c73 657d 2c0d 0a5d 0d0a  a': False},..]..
-00007500: 6060 60                                  ```
+000004e0: 6120 5669 6577 5d28 2372 6561 6469 6e67  a View](#reading
+000004f0: 2d64 6174 612d 6672 6f6d 2d61 2d76 6965  -data-from-a-vie
+00000500: 7729 200d 0a20 2020 2020 2020 2020 2020  w) ..           
+00000510: 2031 2e20 5b55 7369 6e67 2061 2046 696c   1. [Using a Fil
+00000520: 7465 7220 5768 656e 2052 6561 6469 6e67  ter When Reading
+00000530: 2056 6965 7720 4461 7461 5d28 2375 7369   View Data](#usi
+00000540: 6e67 2d61 2d66 696c 7465 722d 7768 656e  ng-a-filter-when
+00000550: 2d72 6561 6469 6e67 2d76 6965 772d 6461  -reading-view-da
+00000560: 7461 2920 0d0a 2020 2020 2020 332e 205b  ta) ..      3. [
+00000570: 4372 6561 7465 2c20 5570 6461 7465 2c20  Create, Update, 
+00000580: 5570 7365 7274 2044 6174 615d 2823 6372  Upsert Data](#cr
+00000590: 6561 7465 2d75 7064 6174 652d 616e 642d  eate-update-and-
+000005a0: 7570 7365 7274 2d64 6174 6129 0d0a 2020  upsert-data)..  
+000005b0: 2020 2020 2020 2031 2e20 5b46 6965 6c64         1. [Field
+000005c0: 204d 6170 7069 6e67 5d28 2366 6965 6c64   Mapping](#field
+000005d0: 2d6d 6170 7069 6e67 290d 0a20 2020 2020  -mapping)..     
+000005e0: 2020 2020 322e 205b 4372 6561 7465 2044      2. [Create D
+000005f0: 6174 615d 2823 6372 6561 7465 2d64 6174  ata](#create-dat
+00000600: 6129 0d0a 2020 2020 2020 2020 2033 2e20  a)..         3. 
+00000610: 5b55 7064 6174 6520 4461 7461 5d28 2375  [Update Data](#u
+00000620: 7064 6174 652d 6461 7461 290d 0a20 2020  pdate-data)..   
+00000630: 2020 2020 2020 342e 205b 5570 7365 7274        4. [Upsert
+00000640: 2044 6174 615d 2823 7570 7365 7274 2d64   Data](#upsert-d
+00000650: 6174 6129 0d0a 2020 2020 2020 2020 2035  ata)..         5
+00000660: 2e20 5b55 6e64 6572 7374 616e 6469 6e67  . [Understanding
+00000670: 2045 7272 6f72 735d 2823 756e 6465 7273   Errors](#unders
+00000680: 7461 6e64 696e 672d 6572 726f 7273 290d  tanding-errors).
+00000690: 0a20 2020 2020 2034 2e20 5b44 656c 6574  .      4. [Delet
+000006a0: 6520 4461 7461 5d28 2364 656c 6574 652d  e Data](#delete-
+000006b0: 6461 7461 2920 0d0a 0d0a 2320 496e 7374  data) ....# Inst
+000006c0: 616c 6c61 7469 6f6e 0d0a 2323 2070 6970  allation..## pip
+000006d0: 0d0a 496e 7374 616c 6c20 7573 696e 6720  ..Install using 
+000006e0: 7069 7020 7769 7468 3a0d 0a60 6060 6261  pip with:..```ba
+000006f0: 7368 0d0a 7069 7020 696e 7374 616c 6c20  sh..pip install 
+00000700: 6465 616c 636c 6f75 645f 7364 6b0d 0a60  dealcloud_sdk..`
+00000710: 6060 0d0a 2320 5573 6167 650d 0a0d 0a23  ``..# Usage....#
+00000720: 2320 4372 6561 7469 6e67 2061 2063 6c69  # Creating a cli
+00000730: 656e 7420 616e 6420 6175 7468 656e 7469  ent and authenti
+00000740: 6361 7469 6e67 0d0a 6064 6561 6c63 6c6f  cating..`dealclo
+00000750: 7564 5f73 646b 6027 7320 6d61 696e 2065  ud_sdk`'s main e
+00000760: 6e74 7279 706f 696e 7420 6973 2074 6865  ntrypoint is the
+00000770: 2060 4465 616c 436c 6f75 6460 2063 6c61   `DealCloud` cla
+00000780: 7373 2e20 5768 656e 2069 7420 6973 2069  ss. When it is i
+00000790: 6e73 7461 6e74 6961 7465 642c 2074 6865  nstantiated, the
+000007a0: 206f 626a 6563 7420 6973 2073 636f 7065   object is scope
+000007b0: 6420 746f 2061 2067 6976 656e 2044 6561  d to a given Dea
+000007c0: 6c43 6c6f 7564 2065 6e76 6972 6f6e 6d65  lCloud environme
+000007d0: 6e74 2c20 6279 2070 6173 7369 6e67 2074  nt, by passing t
+000007e0: 6865 2073 6974 6520 5552 4c20 616e 6420  he site URL and 
+000007f0: 4150 4920 6372 6564 656e 7469 616c 7320  API credentials 
+00000800: 6173 2061 7267 756d 656e 7473 3a0d 0a0d  as arguments:...
+00000810: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
+00000820: 2064 6561 6c63 6c6f 7564 5f73 646b 2069   dealcloud_sdk i
+00000830: 6d70 6f72 7420 4465 616c 436c 6f75 640d  mport DealCloud.
+00000840: 0a0d 0a64 6320 3d20 4465 616c 436c 6f75  ...dc = DealClou
+00000850: 6428 0d0a 2020 2073 6974 655f 7572 6c3d  d(..   site_url=
+00000860: 2263 6c69 656e 742e 6465 616c 636c 6f75  "client.dealclou
+00000870: 642e 636f 6d22 2c0d 0a20 2020 636c 6965  d.com",..   clie
+00000880: 6e74 5f69 643d 2231 3233 3435 222c 0d0a  nt_id="12345",..
+00000890: 2020 2063 6c69 656e 745f 7365 6372 6574     client_secret
+000008a0: 3d22 796f 7572 5f63 6c69 656e 745f 7365  ="your_client_se
+000008b0: 6372 6574 222c 0d0a 290d 0a60 6060 0d0a  cret",..)..```..
+000008c0: 0d0a 3e20 5b21 5741 524e 494e 475d 0d0a  ..> [!WARNING]..
+000008d0: 3e20 5768 696c 7374 2073 7569 7461 626c  > Whilst suitabl
+000008e0: 6520 666f 7220 6c6f 6361 6c20 6465 7665  e for local deve
+000008f0: 6c6f 706d 656e 742c 2074 6865 2061 626f  lopment, the abo
+00000900: 7665 2069 6d70 6c65 6d65 6e74 6174 696f  ve implementatio
+00000910: 6e20 6973 2069 6e73 6563 7572 6520 6966  n is insecure if
+00000920: 2079 6f75 206b 6565 7020 636f 6465 2069   you keep code i
+00000930: 6e20 6f6e 6c69 6e65 2072 6570 6f73 6974  n online reposit
+00000940: 6f72 6965 7320 7375 6368 2061 7320 4769  ories such as Gi
+00000950: 7448 7562 2e20 506c 6561 7365 2073 6565  tHub. Please see
+00000960: 2074 6865 2062 656c 6f77 2065 7861 6d70   the below examp
+00000970: 6c65 7320 666f 7220 6d6f 7265 2073 6563  les for more sec
+00000980: 7572 6520 696d 706c 656d 656e 7461 7469  ure implementati
+00000990: 6f6e 732e 2020 0d0a 0d0a 2323 2053 6563  ons.  ....## Sec
+000009a0: 7572 656c 7920 6c6f 6164 696e 6720 6372  urely loading cr
+000009b0: 6564 656e 7469 616c 730d 0a23 2323 2055  edentials..### U
+000009c0: 7369 6e67 2045 6e76 6972 6f6e 6d65 6e74  sing Environment
+000009d0: 2056 6172 6961 626c 6573 0d0a 0d0a 5768   Variables....Wh
+000009e0: 6572 6520 7468 6520 656e 7669 726f 6e6d  ere the environm
+000009f0: 656e 7420 7661 7269 6162 6c65 7320 636f  ent variables co
+00000a00: 6e74 6169 6e20 7468 6520 7265 6c65 7661  ntain the releva
+00000a10: 6e74 2076 616c 7565 732e 2054 6865 7365  nt values. These
+00000a20: 2063 616e 2062 6520 6c6f 6164 6564 2066   can be loaded f
+00000a30: 726f 6d20 6120 2e65 6e76 2066 696c 6520  rom a .env file 
+00000a40: 7573 696e 6720 7468 6520 6070 7974 686f  using the `pytho
+00000a50: 6e2d 646f 7465 6e76 6020 5b50 7950 6920  n-dotenv` [PyPi 
+00000a60: 7061 636b 6167 655d 2868 7474 7073 3a2f  package](https:/
+00000a70: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000a80: 742f 7079 7468 6f6e 2d64 6f74 656e 762f  t/python-dotenv/
+00000a90: 292e 0d0a 0d0a 5468 6520 6465 6661 756c  ).....The defaul
+00000aa0: 7420 656e 7669 726f 6e6d 656e 7420 7661  t environment va
+00000ab0: 7269 6162 6c65 206e 616d 6573 2061 7265  riable names are
+00000ac0: 2c20 7468 6573 6520 6361 6e20 6265 206f  , these can be o
+00000ad0: 7665 7272 6964 6465 6e20 6966 2064 6573  verridden if des
+00000ae0: 6972 6564 3a0d 0a60 6060 0d0a 4443 5f53  ired:..```..DC_S
+00000af0: 444b 5f53 4954 455f 5552 4c0d 0a44 435f  DK_SITE_URL..DC_
+00000b00: 5344 4b5f 434c 4945 4e54 5f49 440d 0a44  SDK_CLIENT_ID..D
+00000b10: 435f 5344 4b5f 434c 4945 4e54 5f53 4543  C_SDK_CLIENT_SEC
+00000b20: 5245 540d 0a60 6060 0d0a 0d0a 6060 6070  RET..```....```p
+00000b30: 7974 686f 6e0d 0a66 726f 6d20 6465 616c  ython..from deal
+00000b40: 636c 6f75 645f 7364 6b20 696d 706f 7274  cloud_sdk import
+00000b50: 2044 6561 6c43 6c6f 7564 0d0a 0d0a 6463   DealCloud....dc
+00000b60: 203d 2044 6561 6c43 6c6f 7564 2829 2e66   = DealCloud().f
+00000b70: 726f 6d5f 656e 7628 290d 0a60 6060 0d0a  rom_env()..```..
+00000b80: 546f 206f 7665 7272 6964 6520 7468 6520  To override the 
+00000b90: 6465 6661 756c 7420 656e 7669 726f 6e6d  default environm
+00000ba0: 656e 7420 7661 7269 6162 6c65 206e 616d  ent variable nam
+00000bb0: 6573 3a0d 0a60 6060 7079 7468 6f6e 0d0a  es:..```python..
+00000bc0: 6672 6f6d 2064 6561 6c63 6c6f 7564 5f73  from dealcloud_s
+00000bd0: 646b 2069 6d70 6f72 7420 4465 616c 436c  dk import DealCl
+00000be0: 6f75 640d 0a0d 0a64 6320 3d20 4465 616c  oud....dc = Deal
+00000bf0: 436c 6f75 6428 292e 6672 6f6d 5f65 6e76  Cloud().from_env
+00000c00: 280d 0a20 2073 6974 655f 7572 6c5f 656e  (..  site_url_en
+00000c10: 765f 6e61 6d65 3d22 4f56 4552 5249 4444  v_name="OVERRIDD
+00000c20: 454e 5f53 4954 455f 4b45 5922 2c0d 0a20  EN_SITE_KEY",.. 
+00000c30: 2063 6c69 656e 745f 6964 5f65 6e76 5f6e   client_id_env_n
+00000c40: 616d 653d 224f 5645 5252 4944 4445 4e5f  ame="OVERRIDDEN_
+00000c50: 434c 4945 4e54 5f49 445f 4b45 5922 2c0d  CLIENT_ID_KEY",.
+00000c60: 0a20 2063 6c69 656e 745f 7365 6372 6574  .  client_secret
+00000c70: 5f65 6e76 5f6e 616d 653d 224f 5645 5252  _env_name="OVERR
+00000c80: 4944 4445 4e5f 434c 4945 4e54 5f53 4543  IDDEN_CLIENT_SEC
+00000c90: 5245 545f 4b45 5922 2c0d 0a29 0d0a 6060  RET_KEY",..)..``
+00000ca0: 600d 0a23 2323 2055 7369 6e67 204a 534f  `..### Using JSO
+00000cb0: 4e20 436f 6e66 6967 2046 696c 650d 0a47  N Config File..G
+00000cc0: 6976 656e 2061 204a 534f 4e20 6669 6c65  iven a JSON file
+00000cd0: 2069 6e20 7468 6520 6265 6c6f 7720 666f   in the below fo
+00000ce0: 726d 6174 3a0d 0a60 6060 6a73 6f6e 0d0a  rmat:..```json..
+00000cf0: 7b0d 0a20 2022 7369 7465 5f75 726c 223a  {..  "site_url":
+00000d00: 2022 636c 6965 6e74 2e64 6561 6c63 6c6f   "client.dealclo
+00000d10: 7564 2e63 6f6d 222c 0d0a 2020 2263 6c69  ud.com",..  "cli
+00000d20: 656e 745f 6964 223a 2031 3233 3435 2c0d  ent_id": 12345,.
+00000d30: 0a20 2022 636c 6965 6e74 5f73 6563 7265  .  "client_secre
+00000d40: 7422 3a20 2279 6f75 725f 636c 6965 6e74  t": "your_client
+00000d50: 5f73 6563 7265 7422 0d0a 7d0d 0a60 6060  _secret"..}..```
+00000d60: 0d0a 5468 6520 4465 616c 436c 6f75 6420  ..The DealCloud 
+00000d70: 6f62 6a65 6374 2063 616e 2062 6520 6372  object can be cr
+00000d80: 6561 7465 6420 6173 2062 656c 6f77 3a0d  eated as below:.
+00000d90: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
+00000da0: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
+00000db0: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
+00000dc0: 640d 0a0d 0a64 6320 3d20 4465 616c 436c  d....dc = DealCl
+00000dd0: 6f75 642e 6672 6f6d 5f6a 736f 6e28 2270  oud.from_json("p
+00000de0: 6174 682f 746f 2f6a 736f 6e5f 636f 6e66  ath/to/json_conf
+00000df0: 6967 5f66 696c 652e 6a73 6f6e 2229 0d0a  ig_file.json")..
+00000e00: 6060 600d 0a53 696d 696c 6172 6c79 2c20  ```..Similarly, 
+00000e10: 6966 2074 6865 2063 7265 6465 6e74 6961  if the credentia
+00000e20: 6c73 2061 7265 2073 746f 7265 6420 6173  ls are stored as
+00000e30: 2070 6172 7420 6f66 2061 206c 6172 6765   part of a large
+00000e40: 7220 4a53 4f4e 2063 6f6e 6669 6720 6669  r JSON config fi
+00000e50: 6c65 2c20 6120 6b65 7920 7061 7468 2063  le, a key path c
+00000e60: 616e 2062 6520 7061 7373 6564 2061 7320  an be passed as 
+00000e70: 7468 6520 7365 636f 6e64 2061 7267 756d  the second argum
+00000e80: 656e 742c 2064 6972 6563 7469 6e67 2020  ent, directing  
+00000e90: 6044 6561 6c43 6c6f 7564 6020 746f 2074  `DealCloud` to t
+00000ea0: 6865 2070 6174 6820 6f66 2074 6865 2063  he path of the c
+00000eb0: 7265 6465 6e74 6961 6c73 2069 6e20 7468  redentials in th
+00000ec0: 6520 7769 6465 7220 4a53 4f4e 2e20 466f  e wider JSON. Fo
+00000ed0: 7220 6578 616d 706c 653a 0d0a 6060 606a  r example:..```j
+00000ee0: 736f 6e0d 0a7b 0d0a 2020 2020 226f 7468  son..{..    "oth
+00000ef0: 6572 223a 205b 312c 322c 335d 2c0d 0a20  er": [1,2,3],.. 
+00000f00: 2020 2022 6372 6564 7322 3a7b 0d0a 2020     "creds":{..  
+00000f10: 2020 2020 2020 2264 6322 3a7b 0d0a 2020        "dc":{..  
+00000f20: 2020 2020 2020 2020 2273 6974 655f 7572          "site_ur
+00000f30: 6c22 3a20 2263 6c69 656e 742e 6465 616c  l": "client.deal
+00000f40: 636c 6f75 642e 636f 6d22 2c0d 0a20 2020  cloud.com",..   
+00000f50: 2020 2020 2020 2022 636c 6965 6e74 5f69         "client_i
+00000f60: 6422 3a20 3132 3334 352c 0d0a 2020 2020  d": 12345,..    
+00000f70: 2020 2020 2020 2263 6c69 656e 745f 7365        "client_se
+00000f80: 6372 6574 223a 2022 796f 7572 5f63 6c69  cret": "your_cli
+00000f90: 656e 745f 7365 6372 6574 220d 0a20 2020  ent_secret"..   
+00000fa0: 2020 2020 207d 0d0a 2020 2020 7d0d 0a7d       }..    }..}
+00000fb0: 0d0a 6060 600d 0a0d 0a60 6060 7079 7468  ..```....```pyth
+00000fc0: 6f6e 0d0a 6672 6f6d 2064 6561 6c63 6c6f  on..from dealclo
+00000fd0: 7564 5f73 646b 2069 6d70 6f72 7420 4465  ud_sdk import De
+00000fe0: 616c 436c 6f75 640d 0a0d 0a64 6320 3d20  alCloud....dc = 
+00000ff0: 4465 616c 436c 6f75 642e 6672 6f6d 5f6a  DealCloud.from_j
+00001000: 736f 6e28 2270 6174 682f 746f 2f6a 736f  son("path/to/jso
+00001010: 6e5f 636f 6e66 6967 5f66 696c 652e 6a73  n_config_file.js
+00001020: 6f6e 222c 2022 6372 6564 732e 6463 2229  on", "creds.dc")
+00001030: 0d0a 6060 600d 0a23 2323 2055 7369 6e67  ..```..### Using
+00001040: 2059 414d 4c20 436f 6e66 6967 2046 696c   YAML Config Fil
+00001050: 650d 0a47 6976 656e 2061 2059 414d 4c20  e..Given a YAML 
+00001060: 6669 6c65 2069 6e20 7468 6520 6265 6c6f  file in the belo
+00001070: 7720 666f 726d 6174 3a0d 0a60 6060 7961  w format:..```ya
+00001080: 6d6c 0d0a 7369 7465 5f75 726c 3a20 2263  ml..site_url: "c
+00001090: 6c69 656e 742e 6465 616c 636c 6f75 642e  lient.dealcloud.
+000010a0: 636f 6d22 0d0a 636c 6965 6e74 5f69 643a  com"..client_id:
+000010b0: 2031 3233 3435 0d0a 636c 6965 6e74 5f73   12345..client_s
+000010c0: 6563 7265 743a 2022 796f 7572 5f63 6c69  ecret: "your_cli
+000010d0: 656e 745f 7365 6372 6574 220d 0a60 6060  ent_secret"..```
+000010e0: 0d0a 5468 6520 4465 616c 436c 6f75 6420  ..The DealCloud 
+000010f0: 6f62 6a65 6374 2063 616e 2062 6520 6372  object can be cr
+00001100: 6561 7465 6420 6173 2062 656c 6f77 3a0d  eated as below:.
+00001110: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
+00001120: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
+00001130: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
+00001140: 640d 0a0d 0a64 6320 3d20 4465 616c 436c  d....dc = DealCl
+00001150: 6f75 642e 6672 6f6d 5f79 616d 6c28 2270  oud.from_yaml("p
+00001160: 6174 682f 746f 2f79 616d 6c5f 636f 6e66  ath/to/yaml_conf
+00001170: 6967 5f66 696c 652e 6a73 6f6e 2229 0d0a  ig_file.json")..
+00001180: 6060 600d 0a53 696d 696c 6172 6c79 2c20  ```..Similarly, 
+00001190: 6966 2074 6865 2063 7265 6465 6e74 6961  if the credentia
+000011a0: 6c73 2061 7265 2073 746f 7265 6420 6173  ls are stored as
+000011b0: 2070 6172 7420 6f66 2061 206c 6172 6765   part of a large
+000011c0: 7220 5941 4d4c 2063 6f6e 6669 6720 6669  r YAML config fi
+000011d0: 6c65 2c20 6120 6b65 7920 7061 7468 2063  le, a key path c
+000011e0: 616e 2062 6520 7061 7373 6564 2061 7320  an be passed as 
+000011f0: 7468 6520 7365 636f 6e64 2061 7267 756d  the second argum
+00001200: 656e 742c 2064 6972 6563 7469 6e67 2020  ent, directing  
+00001210: 6044 6561 6c43 6c6f 7564 6020 746f 2074  `DealCloud` to t
+00001220: 6865 2070 6174 6820 6f66 2074 6865 2063  he path of the c
+00001230: 7265 6465 6e74 6961 6c73 2069 6e20 7468  redentials in th
+00001240: 6520 7769 6465 7220 5941 4d4c 2e20 466f  e wider YAML. Fo
+00001250: 7220 6578 616d 706c 653a 0d0a 6060 6079  r example:..```y
+00001260: 616d 6c0d 0a6f 7468 6572 3a0d 0a20 202d  aml..other:..  -
+00001270: 2031 0d0a 2020 2d20 320d 0a20 202d 2033   1..  - 2..  - 3
+00001280: 0d0a 6372 6564 733a 0d0a 2020 6463 3a0d  ..creds:..  dc:.
+00001290: 0a20 2020 2073 6974 655f 7572 6c3a 2022  .    site_url: "
+000012a0: 636c 6965 6e74 2e64 6561 6c63 6c6f 7564  client.dealcloud
+000012b0: 2e63 6f6d 220d 0a20 2020 2063 6c69 656e  .com"..    clien
+000012c0: 745f 6964 3a20 3132 3334 350d 0a20 2020  t_id: 12345..   
+000012d0: 2063 6c69 656e 745f 7365 6372 6574 3a20   client_secret: 
+000012e0: 2279 6f75 725f 636c 6965 6e74 5f73 6563  "your_client_sec
+000012f0: 7265 7422 0d0a 6060 600d 0a0d 0a60 6060  ret"..```....```
+00001300: 7079 7468 6f6e 0d0a 6672 6f6d 2064 6561  python..from dea
+00001310: 6c63 6c6f 7564 5f73 646b 2069 6d70 6f72  lcloud_sdk impor
+00001320: 7420 4465 616c 436c 6f75 640d 0a0d 0a64  t DealCloud....d
+00001330: 6320 3d20 4465 616c 436c 6f75 642e 6672  c = DealCloud.fr
+00001340: 6f6d 5f79 616d 6c28 2270 6174 682f 746f  om_yaml("path/to
+00001350: 2f79 616d 6c5f 636f 6e66 6967 5f66 696c  /yaml_config_fil
+00001360: 652e 6a73 6f6e 222c 2022 6372 6564 732e  e.json", "creds.
+00001370: 6463 2229 0d0a 6060 600d 0a0d 0a23 2320  dc")..```....## 
+00001380: 5363 6865 6d61 2051 7565 7279 696e 670d  Schema Querying.
+00001390: 0a54 6865 2044 6561 6c43 6c6f 7564 2041  .The DealCloud A
+000013a0: 5049 2061 6c6c 6f77 7320 796f 7520 746f  PI allows you to
+000013b0: 2071 7565 7279 2074 6865 2073 6368 656d   query the schem
+000013c0: 6120 6f66 2061 2067 6976 656e 2073 6974  a of a given sit
+000013d0: 652e 2054 6865 2060 4465 616c 436c 6f75  e. The `DealClou
+000013e0: 6460 2063 6c61 7373 2070 726f 7669 6465  d` class provide
+000013f0: 7320 6163 6365 7373 2074 6f20 7468 6520  s access to the 
+00001400: 7363 6865 6d61 2065 6e64 706f 696e 7473  schema endpoints
+00001410: 2074 6872 6f75 6768 2074 6865 2066 6f6c   through the fol
+00001420: 6c6f 7769 6e67 206d 6574 686f 6473 3a0d  lowing methods:.
+00001430: 0a3e 2054 6865 2073 6368 656d 6120 6d6f  .> The schema mo
+00001440: 6465 6c73 2061 7265 2064 6566 696e 6564  dels are defined
+00001450: 2075 7369 6e67 205b 5079 6461 6e74 6963   using [Pydantic
+00001460: 5d28 6874 7470 733a 2f2f 7079 6461 6e74  ](https://pydant
+00001470: 6963 2e64 6576 2f29 2c20 666f 7220 636c  ic.dev/), for cl
+00001480: 6561 7220 7661 6c69 6461 7469 6f6e 2c20  ear validation, 
+00001490: 7374 7261 6967 6874 666f 7277 6172 6420  straightforward 
+000014a0: 6174 7472 6962 7574 6520 6163 6365 7373  attribute access
+000014b0: 2061 6e64 2049 4445 2061 7373 6973 7461   and IDE assista
+000014c0: 6e63 652e 0d0a 0d0a 2323 2320 4765 7420  nce.....### Get 
+000014d0: 5573 6572 730d 0a0d 0a60 4465 616c 436c  Users....`DealCl
+000014e0: 6f75 642e 6765 745f 7573 6572 7328 2960  oud.get_users()`
+000014f0: 2077 696c 6c20 7265 7475 726e 2061 6c6c   will return all
+00001500: 2075 7365 7273 2069 6e20 7468 6520 7369   users in the si
+00001510: 7465 2e20 5370 6563 6966 6963 616c 6c79  te. Specifically
+00001520: 2c20 616e 2061 7272 6179 206f 6620 6055  , an array of `U
+00001530: 7365 7260 206f 626a 6563 7473 2e20 5468  ser` objects. Th
+00001540: 6520 6172 6775 6d65 6e74 3a20 6061 6374  e argument: `act
+00001550: 6976 655f 6f6e 6c79 6020 6973 2061 2062  ive_only` is a b
+00001560: 6f6f 6c65 616e 2074 6861 7420 6361 6e20  oolean that can 
+00001570: 6265 2070 6173 7365 642c 2069 6620 7472  be passed, if tr
+00001580: 7565 2c20 7468 6520 6675 6e63 7469 6f6e  ue, the function
+00001590: 2077 696c 6c20 6f6e 6c79 2072 6574 7572   will only retur
+000015a0: 6e20 6163 7469 7665 2075 7365 7273 2e0d  n active users..
+000015b0: 0a0d 0a45 7861 6d70 6c65 3a0d 0a0d 0a60  ...Example:....`
+000015c0: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2064  ``python..from d
+000015d0: 6561 6c63 6c6f 7564 5f73 646b 2069 6d70  ealcloud_sdk imp
+000015e0: 6f72 7420 4465 616c 436c 6f75 640d 0a0d  ort DealCloud...
+000015f0: 0a64 6320 3d20 4465 616c 436c 6f75 642e  .dc = DealCloud.
+00001600: 6672 6f6d 5f79 616d 6c28 2270 6174 682f  from_yaml("path/
+00001610: 746f 2f79 616d 6c5f 636f 6e66 6967 5f66  to/yaml_config_f
+00001620: 696c 652e 6a73 6f6e 2229 0d0a 0d0a 7573  ile.json")....us
+00001630: 6572 7320 3d20 6463 2e67 6574 5f75 7365  ers = dc.get_use
+00001640: 7273 2829 0d0a 0d0a 666f 7220 7573 6572  rs()....for user
+00001650: 2069 6e20 7573 6572 733a 0d0a 2020 2020   in users:..    
+00001660: 7072 696e 7428 6622 7b75 7365 722e 6e61  print(f"{user.na
+00001670: 6d65 7d3a 207b 7573 6572 2e65 6d61 696c  me}: {user.email
+00001680: 7d22 290d 0a60 6060 0d0a 5769 6c6c 206f  }")..```..Will o
+00001690: 7574 7075 743a 0d0a 6060 6062 6173 680d  utput:..```bash.
+000016a0: 0a55 7365 7220 313a 2075 7365 7231 4065  .User 1: user1@e
+000016b0: 6d61 696c 2e63 6f6d 0d0a 5573 6572 2032  mail.com..User 2
+000016c0: 3a20 7573 6572 3240 656d 6169 6c2e 636f  : user2@email.co
+000016d0: 6d0d 0a55 7365 7220 333a 2075 7365 7233  m..User 3: user3
+000016e0: 4065 6d61 696c 2e63 6f6d 0d0a 5573 6572  @email.com..User
+000016f0: 2034 3a20 7573 6572 3440 656d 6169 6c2e   4: user4@email.
+00001700: 636f 6d0d 0a2e 2e2e 6574 630d 0a60 6060  com.....etc..```
+00001710: 0d0a 2323 2320 4765 7420 4375 7272 656e  ..### Get Curren
+00001720: 6369 6573 0d0a 6044 6561 6c43 6c6f 7564  cies..`DealCloud
+00001730: 2e67 6574 5f63 7572 7265 6e63 6965 7328  .get_currencies(
+00001740: 2960 2077 696c 6c20 7265 7475 726e 2074  )` will return t
+00001750: 6865 2063 7572 7265 6e63 7920 636f 6465  he currency code
+00001760: 7320 6f66 2061 6c6c 2065 6e61 626c 6564  s of all enabled
+00001770: 2063 7572 7265 6e63 6965 7320 696e 2074   currencies in t
+00001780: 6865 2073 6974 652e 0d0a 4578 616d 706c  he site...Exampl
+00001790: 653a 0d0a 0d0a 6060 6070 7974 686f 6e0d  e:....```python.
+000017a0: 0a66 726f 6d20 6465 616c 636c 6f75 645f  .from dealcloud_
+000017b0: 7364 6b20 696d 706f 7274 2044 6561 6c43  sdk import DealC
+000017c0: 6c6f 7564 0d0a 0d0a 6463 203d 2044 6561  loud....dc = Dea
+000017d0: 6c43 6c6f 7564 2e66 726f 6d5f 7961 6d6c  lCloud.from_yaml
+000017e0: 2822 7061 7468 2f74 6f2f 7961 6d6c 5f63  ("path/to/yaml_c
+000017f0: 6f6e 6669 675f 6669 6c65 2e6a 736f 6e22  onfig_file.json"
+00001800: 290d 0a0d 0a63 7572 7265 6e63 6965 7320  )....currencies 
+00001810: 3d20 6463 2e67 6574 5f63 7572 7265 6e63  = dc.get_currenc
+00001820: 6965 7328 290d 0a0d 0a66 6f72 2063 6379  ies()....for ccy
+00001830: 2069 6e20 6375 7272 656e 6369 6573 3a0d   in currencies:.
+00001840: 0a20 2020 2070 7269 6e74 2863 6379 290d  .    print(ccy).
+00001850: 0a60 6060 0d0a 5769 6c6c 206f 7574 7075  .```..Will outpu
+00001860: 743a 0d0a 6060 6062 6173 680d 0a47 4250  t:..```bash..GBP
+00001870: 0d0a 5553 440d 0a45 5552 0d0a 2e2e 2e65  ..USD..EUR.....e
+00001880: 7463 0d0a 6060 600d 0a0d 0a23 2323 2047  tc..```....### G
+00001890: 6574 204f 626a 6563 7473 0d0a 6044 6561  et Objects..`Dea
+000018a0: 6c43 6c6f 7564 2e67 6574 5f6f 626a 6563  lCloud.get_objec
+000018b0: 7428 2960 2077 696c 6c20 7265 7475 726e  t()` will return
+000018c0: 2061 6c6c 2063 6f6e 6669 6775 7265 6420   all configured 
+000018d0: 6f62 6a65 6374 7320 696e 2074 6865 2073  objects in the s
+000018e0: 6974 652e 2053 7065 6369 6669 6361 6c6c  ite. Specificall
+000018f0: 792c 2061 6e20 6172 7261 7920 6f66 2060  y, an array of `
+00001900: 4f62 6a65 6374 6020 6f62 6a65 6374 732e  Object` objects.
+00001910: 0d0a 4578 616d 706c 653a 0d0a 0d0a 6060  ..Example:....``
+00001920: 6070 7974 686f 6e0d 0a66 726f 6d20 6465  `python..from de
+00001930: 616c 636c 6f75 645f 7364 6b20 696d 706f  alcloud_sdk impo
+00001940: 7274 2044 6561 6c43 6c6f 7564 0d0a 0d0a  rt DealCloud....
+00001950: 6463 203d 2044 6561 6c43 6c6f 7564 2e66  dc = DealCloud.f
+00001960: 726f 6d5f 7961 6d6c 2822 7061 7468 2f74  rom_yaml("path/t
+00001970: 6f2f 7961 6d6c 5f63 6f6e 6669 675f 6669  o/yaml_config_fi
+00001980: 6c65 2e6a 736f 6e22 290d 0a0d 0a6f 626a  le.json")....obj
+00001990: 6563 7473 203d 2064 632e 6765 745f 6f62  ects = dc.get_ob
+000019a0: 6a65 6374 7328 290d 0a0d 0a66 6f72 206f  jects()....for o
+000019b0: 626a 2069 6e20 6f62 6a65 6374 733a 0d0a  bj in objects:..
+000019c0: 2020 2020 7072 696e 7428 6622 7b6f 626a      print(f"{obj
+000019d0: 2e61 7069 4e61 6d65 7d3a 207b 6f62 6a2e  .apiName}: {obj.
+000019e0: 706c 7572 616c 4e61 6d65 7d2c 207b 6f62  pluralName}, {ob
+000019f0: 6a2e 7369 6e67 756c 6172 4e61 6d65 7d22  j.singularName}"
+00001a00: 290d 0a60 6060 0d0a 5769 6c6c 206f 7574  )..```..Will out
+00001a10: 7075 743a 0d0a 6060 6062 6173 680d 0a43  put:..```bash..C
+00001a20: 6f6d 7061 6e79 3a20 436f 6d70 616e 6965  ompany: Companie
+00001a30: 732c 2043 6f6d 7061 6e79 0d0a 436f 6e74  s, Company..Cont
+00001a40: 6163 743a 2043 6f6e 7461 6374 732c 2043  act: Contacts, C
+00001a50: 6f6e 7461 6374 0d0a 436f 6d70 616e 7941  ontact..CompanyA
+00001a60: 6464 7265 7373 3a20 436f 6d70 616e 7920  ddress: Company 
+00001a70: 4164 6472 6573 7365 732c 2043 6f6d 7061  Addresses, Compa
+00001a80: 6e79 2041 6464 7265 7373 0d0a 2e2e 2e65  ny Address.....e
+00001a90: 7463 0d0a 6060 600d 0a0d 0a23 2320 4765  tc..```....## Ge
+00001aa0: 7420 4669 656c 6473 0d0a 6044 6561 6c43  t Fields..`DealC
+00001ab0: 6c6f 7564 2e67 6574 5f66 6965 6c64 7328  loud.get_fields(
+00001ac0: 2960 2070 726f 7669 6465 7320 7468 6520  )` provides the 
+00001ad0: 6162 696c 6974 7920 746f 2072 6574 7572  ability to retur
+00001ae0: 6e20 6669 656c 6473 2063 6f6e 6669 6775  n fields configu
+00001af0: 7265 6420 696e 2074 6865 2073 6974 652e  red in the site.
+00001b00: 2053 7065 6369 6669 6361 6c6c 792c 2061   Specifically, a
+00001b10: 6e20 6172 7261 7920 6f66 2060 4669 656c  n array of `Fiel
+00001b20: 6460 206f 626a 6563 7473 2e0d 0a0d 0a54  d` objects.....T
+00001b30: 6865 7265 2061 7265 2074 6872 6565 2077  here are three w
+00001b40: 6179 7320 746f 2071 7565 7279 2066 6f72  ays to query for
+00001b50: 2066 6965 6c64 733a 0d0a 312e 205f 5f41   fields:..1. __A
+00001b60: 6c6c 2046 6965 6c64 735f 5f3a 2063 616c  ll Fields__: cal
+00001b70: 6c20 6044 6561 6c43 6c6f 7564 2e67 6574  l `DealCloud.get
+00001b80: 5f66 6965 6c64 7328 2960 2077 6974 6820  _fields()` with 
+00001b90: 6e6f 2061 7267 756d 656e 7473 2074 6f20  no arguments to 
+00001ba0: 7265 7475 726e 2061 6c6c 2066 6965 6c64  return all field
+00001bb0: 732e 0d0a 0d0a 6060 6070 7974 686f 6e0d  s.....```python.
+00001bc0: 0a66 726f 6d20 6465 616c 636c 6f75 645f  .from dealcloud_
+00001bd0: 7364 6b20 696d 706f 7274 2044 6561 6c43  sdk import DealC
+00001be0: 6c6f 7564 0d0a 0d0a 6463 203d 2044 6561  loud....dc = Dea
+00001bf0: 6c43 6c6f 7564 2e66 726f 6d5f 7961 6d6c  lCloud.from_yaml
+00001c00: 2822 7061 7468 2f74 6f2f 7961 6d6c 5f63  ("path/to/yaml_c
+00001c10: 6f6e 6669 675f 6669 6c65 2e6a 736f 6e22  onfig_file.json"
+00001c20: 290d 0a0d 0a66 6965 6c64 7320 3d20 6463  )....fields = dc
+00001c30: 2e67 6574 5f66 6965 6c64 7328 290d 0a60  .get_fields()..`
+00001c40: 6060 0d0a 6066 6965 6c64 7360 2077 696c  ``..`fields` wil
+00001c50: 6c20 636f 6e74 6169 6e20 6120 6c69 7374  l contain a list
+00001c60: 206f 6620 6046 6965 6c64 6020 6f62 6a65   of `Field` obje
+00001c70: 6374 7320 636f 6e74 6169 6e69 6e67 2061  cts containing a
+00001c80: 6c6c 2063 6f6e 6669 6775 7265 6420 6669  ll configured fi
+00001c90: 656c 6473 2069 6e20 7468 6520 7369 7465  elds in the site
+00001ca0: 2e0d 0a0d 0a0d 0a32 2e20 5f5f 416c 6c20  .......2. __All 
+00001cb0: 4669 656c 6473 2066 6f72 2061 6e20 4f62  Fields for an Ob
+00001cc0: 6a65 6374 5f5f 3a20 6361 6c6c 2060 4465  ject__: call `De
+00001cd0: 616c 436c 6f75 642e 6765 745f 6669 656c  alCloud.get_fiel
+00001ce0: 6473 286f 626a 6563 745f 6964 3d22 4f62  ds(object_id="Ob
+00001cf0: 6a65 6374 4e61 6d65 2229 6020 7769 7468  jectName")` with
+00001d00: 2060 6f62 6a65 6374 5f69 6460 2073 6574   `object_id` set
+00001d10: 2074 6f20 7468 6520 6465 7369 7265 6420   to the desired 
+00001d20: 6f62 6a65 6374 2061 7069 206e 616d 652c  object api name,
+00001d30: 206f 7220 6f62 6a65 6374 2069 642c 2074   or object id, t
+00001d40: 6f20 7265 7475 726e 2061 6c6c 2066 6965  o return all fie
+00001d50: 6c64 7320 636f 6e66 6967 7572 6564 2066  lds configured f
+00001d60: 6f72 2074 6861 7420 6f62 6a65 6374 2e0d  or that object..
+00001d70: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
+00001d80: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
+00001d90: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
+00001da0: 640d 0a0d 0a64 6320 3d20 4465 616c 436c  d....dc = DealCl
+00001db0: 6f75 642e 6672 6f6d 5f79 616d 6c28 2270  oud.from_yaml("p
+00001dc0: 6174 682f 746f 2f79 616d 6c5f 636f 6e66  ath/to/yaml_conf
+00001dd0: 6967 5f66 696c 652e 6a73 6f6e 2229 0d0a  ig_file.json")..
+00001de0: 0d0a 6669 656c 6473 203d 2064 632e 6765  ..fields = dc.ge
+00001df0: 745f 6669 656c 6473 2822 436f 6d70 616e  t_fields("Compan
+00001e00: 7922 290d 0a60 6060 0d0a 6066 6965 6c64  y")..```..`field
+00001e10: 7360 2077 696c 6c20 636f 6e74 6169 6e20  s` will contain 
+00001e20: 6120 6c69 7374 206f 6620 6046 6965 6c64  a list of `Field
+00001e30: 6020 6f62 6a65 6374 732c 2063 6f6e 7461  ` objects, conta
+00001e40: 696e 696e 6720 616c 6c20 6669 656c 6473  ining all fields
+00001e50: 2063 6f6e 6669 6775 7265 6420 696e 2074   configured in t
+00001e60: 6865 2022 436f 6d70 616e 7922 206f 626a  he "Company" obj
+00001e70: 6563 742e 0d0a 0d0a 0d0a 332e 205f 5f41  ect.......3. __A
+00001e80: 2046 6965 6c64 2062 7920 4669 656c 6420   Field by Field 
+00001e90: 4944 5f5f 3a20 6361 6c6c 2060 4465 616c  ID__: call `Deal
+00001ea0: 436c 6f75 642e 6765 745f 6669 656c 6473  Cloud.get_fields
+00001eb0: 2866 6965 6c64 5f69 643d 3132 3334 2960  (field_id=1234)`
+00001ec0: 2077 6974 6820 6066 6965 6c64 5f69 6460   with `field_id`
+00001ed0: 2073 6574 2074 6f20 7468 6520 4944 206f   set to the ID o
+00001ee0: 6620 7468 6520 6465 7369 7265 6420 6669  f the desired fi
+00001ef0: 656c 642e 0d0a 0d0a 6060 6070 7974 686f  eld.....```pytho
+00001f00: 6e0d 0a66 726f 6d20 6465 616c 636c 6f75  n..from dealclou
+00001f10: 645f 7364 6b20 696d 706f 7274 2044 6561  d_sdk import Dea
+00001f20: 6c43 6c6f 7564 0d0a 0d0a 6463 203d 2044  lCloud....dc = D
+00001f30: 6561 6c43 6c6f 7564 2e66 726f 6d5f 7961  ealCloud.from_ya
+00001f40: 6d6c 2822 7061 7468 2f74 6f2f 7961 6d6c  ml("path/to/yaml
+00001f50: 5f63 6f6e 6669 675f 6669 6c65 2e6a 736f  _config_file.jso
+00001f60: 6e22 290d 0a0d 0a66 6965 6c64 203d 2064  n")....field = d
+00001f70: 632e 6765 745f 6669 656c 6473 2866 6965  c.get_fields(fie
+00001f80: 6c64 5f69 643d 3132 3334 290d 0a60 6060  ld_id=1234)..```
+00001f90: 0d0a 6066 6965 6c64 6020 7769 6c6c 2063  ..`field` will c
+00001fa0: 6f6e 7461 696e 2061 2073 696e 676c 6520  ontain a single 
+00001fb0: 6046 6965 6c64 6020 6f62 6a65 6374 2c20  `Field` object, 
+00001fc0: 6465 7363 7269 6269 6e67 2074 6865 2066  describing the f
+00001fd0: 6965 6c64 2077 6974 6820 4944 2060 3132  ield with ID `12
+00001fe0: 3334 602e 0d0a 0d0a 2323 2320 4765 7420  34`.....### Get 
+00001ff0: 5363 6865 6d61 0d0a 6044 6561 6c43 6c6f  Schema..`DealClo
+00002000: 7564 2e67 6574 5f73 6368 656d 6128 2960  ud.get_schema()`
+00002010: 2069 7320 6120 6d65 7468 6f64 2074 6861   is a method tha
+00002020: 7420 7769 6c6c 2072 6574 7572 6e20 7468  t will return th
+00002030: 6520 6675 6c6c 2044 6561 6c43 6c6f 7564  e full DealCloud
+00002040: 2073 6368 656d 6120 696e 2061 2073 696e   schema in a sin
+00002050: 676c 6520 6f62 6a65 6374 2e0d 0a54 6865  gle object...The
+00002060: 206d 6574 686f 6420 7461 6b65 7320 7468   method takes th
+00002070: 6520 6172 6775 6d65 6e74 3a20 606b 6579  e argument: `key
+00002080: 5f74 7970 6560 2c20 7768 6963 6820 6465  _type`, which de
+00002090: 7363 7269 6265 7320 7768 6963 6820 6669  scribes which fi
+000020a0: 656c 6420 7769 6c6c 2062 6520 7573 6564  eld will be used
+000020b0: 2061 7320 6b65 7973 2069 6e20 7468 6520   as keys in the 
+000020c0: 6e65 7374 6564 206f 626a 6563 7420 7374  nested object st
+000020d0: 7275 6374 7572 6520 6465 7363 7269 6269  ructure describi
+000020e0: 6e67 2074 6865 2073 6368 656d 612e 200d  ng the schema. .
+000020f0: 0a0d 0a54 6865 206f 7074 696f 6e73 2061  ...The options a
+00002100: 7265 3a0d 0a2d 2060 6170 6960 202d 2054  re:..- `api` - T
+00002110: 6865 2041 5049 206e 616d 650d 0a2d 2060  he API name..- `
+00002120: 6469 7370 6c61 7960 202d 2054 6865 2064  display` - The d
+00002130: 6973 706c 6179 206e 616d 650d 0a2d 2060  isplay name..- `
+00002140: 6964 6020 2d20 5468 6520 6f62 6a65 6374  id` - The object
+00002150: 2f66 6965 6c64 2049 440d 0a0d 0a55 7361  /field ID....Usa
+00002160: 6765 2045 7861 6d70 6c65 3a0d 0a0d 0a60  ge Example:....`
+00002170: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2064  ``python..from d
+00002180: 6561 6c63 6c6f 7564 5f73 646b 2069 6d70  ealcloud_sdk imp
+00002190: 6f72 7420 4465 616c 436c 6f75 640d 0a0d  ort DealCloud...
+000021a0: 0a64 6320 3d20 4465 616c 436c 6f75 642e  .dc = DealCloud.
+000021b0: 6672 6f6d 5f79 616d 6c28 2270 6174 682f  from_yaml("path/
+000021c0: 746f 2f79 616d 6c5f 636f 6e66 6967 5f66  to/yaml_config_f
+000021d0: 696c 652e 6a73 6f6e 2229 0d0a 0d0a 7363  ile.json")....sc
+000021e0: 6865 6d61 203d 2064 632e 6765 745f 7363  hema = dc.get_sc
+000021f0: 6865 6d61 2822 6170 6922 290d 0a60 6060  hema("api")..```
+00002200: 0d0a 6073 6368 656d 6160 2077 696c 6c20  ..`schema` will 
+00002210: 636f 6e74 6169 6e20 7468 6520 6120 6053  contain the a `S
+00002220: 6368 656d 6160 206f 626a 6563 7420 7769  chema` object wi
+00002230: 7468 2074 6865 2041 5049 206e 616d 6573  th the API names
+00002240: 2061 7320 6b65 7973 2c20 6173 2062 656c   as keys, as bel
+00002250: 6f77 3a20 0d0a 0d0a 6061 7069 6020 4578  ow: ....`api` Ex
+00002260: 616d 706c 653a 0d0a 6060 6070 7974 686f  ample:..```pytho
+00002270: 6e0d 0a7b 0d0a 2020 2243 6f6d 7061 6e79  n..{..  "Company
+00002280: 4150 494e 616d 6522 3a20 7b0d 0a20 2020  APIName": {..   
+00002290: 2022 436f 6d70 616e 794f 626a 6563 744d   "CompanyObjectM
+000022a0: 6574 6144 6174 6122 3a20 222e 2e2e 222c  etaData": "...",
+000022b0: 0d0a 2020 2020 2243 6f6d 7061 6e79 4f62  ..    "CompanyOb
+000022c0: 6a65 6374 4669 656c 6473 223a 207b 0d0a  jectFields": {..
+000022d0: 2020 2020 2020 2246 6965 6c64 3141 5049        "Field1API
+000022e0: 4e61 6d65 223a 207b 0d0a 2020 2020 2020  Name": {..      
+000022f0: 2020 2246 6965 6c64 314d 6574 6144 6174    "Field1MetaDat
+00002300: 6122 3a20 222e 2e2e 220d 0a20 2020 2020  a": "..."..     
+00002310: 207d 0d0a 2020 2020 7d0d 0a20 207d 0d0a   }..    }..  }..
+00002320: 7d0d 0a60 6060 0d0a 6064 6973 706c 6179  }..```..`display
+00002330: 6020 4578 616d 706c 653a 0d0a 6060 6070  ` Example:..```p
+00002340: 7974 686f 6e0d 0a7b 0d0a 2020 2243 6f6d  ython..{..  "Com
+00002350: 7061 6e79 2044 6973 706c 6179 204e 616d  pany Display Nam
+00002360: 6522 3a20 7b0d 0a20 2020 2022 436f 6d70  e": {..    "Comp
+00002370: 616e 794f 626a 6563 744d 6574 6144 6174  anyObjectMetaDat
+00002380: 6122 3a20 222e 2e2e 222c 0d0a 2020 2020  a": "...",..    
+00002390: 2243 6f6d 7061 6e79 4f62 6a65 6374 4669  "CompanyObjectFi
+000023a0: 656c 6473 223a 207b 0d0a 2020 2020 2020  elds": {..      
+000023b0: 2246 6965 6c64 2031 2044 6973 706c 6179  "Field 1 Display
+000023c0: 204e 616d 6522 3a20 7b0d 0a20 2020 2020   Name": {..     
+000023d0: 2020 2022 4669 656c 6431 4d65 7461 4461     "Field1MetaDa
+000023e0: 7461 223a 2022 2e2e 2e22 0d0a 2020 2020  ta": "..."..    
+000023f0: 2020 7d0d 0a20 2020 207d 0d0a 2020 7d0d    }..    }..  }.
+00002400: 0a7d 0d0a 6060 600d 0a60 6964 6020 4578  .}..```..`id` Ex
+00002410: 616d 706c 653a 0d0a 3e20 4e6f 7465 2074  ample:..> Note t
+00002420: 6865 2049 4420 6f66 2074 6865 2022 436f  he ID of the "Co
+00002430: 6d70 616e 7922 206f 626a 6563 7420 6973  mpany" object is
+00002440: 2031 3233 3435 2061 6e64 2074 6865 2049   12345 and the I
+00002450: 4420 6f66 2074 6865 2022 4669 656c 6420  D of the "Field 
+00002460: 3122 2066 6965 6c64 2069 7320 3132 3334  1" field is 1234
+00002470: 3536 200d 0a60 6060 7079 7468 6f6e 0d0a  56 ..```python..
+00002480: 7b0d 0a20 2031 3233 3435 3a20 7b0d 0a20  {..  12345: {.. 
+00002490: 2020 2022 436f 6d70 616e 794f 626a 6563     "CompanyObjec
+000024a0: 744d 6574 6144 6174 6122 3a20 222e 2e2e  tMetaData": "...
+000024b0: 222c 0d0a 2020 2020 2243 6f6d 7061 6e79  ",..    "Company
+000024c0: 4f62 6a65 6374 4669 656c 6473 223a 207b  ObjectFields": {
+000024d0: 0d0a 2020 2020 2020 3132 3334 3536 3a20  ..      123456: 
+000024e0: 7b0d 0a20 2020 2020 2020 2022 4669 656c  {..        "Fiel
+000024f0: 6431 4d65 7461 4461 7461 223a 2022 2e2e  d1MetaData": "..
+00002500: 2e22 0d0a 2020 2020 2020 7d0d 0a20 2020  ."..      }..   
+00002510: 207d 0d0a 2020 7d0d 0a7d 0d0a 6060 600d   }..  }..}..```.
+00002520: 0a0d 0a23 2320 4461 7461 204f 7065 7261  ...## Data Opera
+00002530: 7469 6f6e 730d 0a54 6865 2060 4465 616c  tions..The `Deal
+00002540: 436c 6f75 6460 206f 626a 6563 7420 7072  Cloud` object pr
+00002550: 6f76 6964 6573 206d 6574 686f 6473 2074  ovides methods t
+00002560: 6f20 4372 6561 7465 2c20 5265 6164 2c20  o Create, Read, 
+00002570: 5570 6461 7465 2061 6e64 2044 656c 6574  Update and Delet
+00002580: 6520 6461 7461 2069 6e20 6275 6c6b 2e20  e data in bulk. 
+00002590: 4173 2069 7473 2064 6566 6175 6c74 2062  As its default b
+000025a0: 6568 6176 696f 7572 2c20 7768 656e 2077  ehaviour, when w
+000025b0: 6f72 6b69 6e67 2077 6974 6820 7369 7465  orking with site
+000025c0: 2064 6174 612c 2074 6865 206c 6962 7261   data, the libra
+000025d0: 7279 2075 7365 7320 4461 7461 4672 616d  ry uses DataFram
+000025e0: 6573 2077 6974 680d 0a74 6865 205b 5061  es with..the [Pa
+000025f0: 6e64 6173 5d28 6874 7470 733a 2f2f 7061  ndas](https://pa
+00002600: 6e64 6173 2e70 7964 6174 612e 6f72 672f  ndas.pydata.org/
+00002610: 2920 6c69 6272 6172 792c 2068 6f77 6576  ) library, howev
+00002620: 6572 2074 6865 206f 7074 696f 6e20 6973  er the option is
+00002630: 2061 7661 696c 6162 6c65 2066 6f72 2069   available for i
+00002640: 7420 746f 2077 6f72 6b20 7769 7468 206a  t to work with j
+00002650: 7573 7420 7079 7468 6f6e 2073 7461 6e64  ust python stand
+00002660: 6172 6420 6461 7461 2074 7970 6573 2e0d  ard data types..
+00002670: 0a0d 0a23 2323 204c 6973 7420 436f 6e66  ...### List Conf
+00002680: 6967 7572 6564 2056 6965 7773 0d0a 6044  igured Views..`D
+00002690: 6561 6c43 6c6f 7564 2e6c 6973 745f 636f  ealCloud.list_co
+000026a0: 6e66 6967 7572 6564 5f76 6965 7773 2829  nfigured_views()
+000026b0: 6020 7265 7475 726e 7320 6120 6052 6f77  ` returns a `Row
+000026c0: 7360 206f 626a 6563 7420 636f 6e74 6169  s` object contai
+000026d0: 6e69 6e67 2061 6c6c 2063 6f6e 6669 6775  ning all configu
+000026e0: 7265 6420 7669 6577 7320 696e 2074 6865  red views in the
+000026f0: 2073 6974 652e 0d0a 5468 6520 6172 6775   site...The argu
+00002700: 6d65 6e74 2060 6973 5f70 7269 7661 7465  ment `is_private
+00002710: 6020 6361 6e20 6265 2070 6173 7365 6420  ` can be passed 
+00002720: 6173 2061 2062 6f6f 6c65 616e 2c20 7768  as a boolean, wh
+00002730: 6572 6520 6966 2074 7275 652c 206f 6e6c  ere if true, onl
+00002740: 7920 7072 6976 6174 6520 7669 6577 7320  y private views 
+00002750: 746f 2028 696e 636c 7564 696e 6720 7669  to (including vi
+00002760: 6577 7320 7368 6172 6564 2077 6974 6829  ews shared with)
+00002770: 2074 6865 2061 7574 6865 6e74 6963 6174   the authenticat
+00002780: 6564 2075 7365 7220 7769 6c6c 2062 6520  ed user will be 
+00002790: 7265 7475 726e 6564 2e0d 0a0d 0a45 7861  returned.....Exa
+000027a0: 6d70 6c65 3a0d 0a0d 0a60 6060 7079 7468  mple:....```pyth
+000027b0: 6f6e 0d0a 6672 6f6d 2064 6561 6c63 6c6f  on..from dealclo
+000027c0: 7564 5f73 646b 2069 6d70 6f72 7420 4465  ud_sdk import De
+000027d0: 616c 436c 6f75 640d 0a0d 0a64 6320 3d20  alCloud....dc = 
+000027e0: 4465 616c 436c 6f75 642e 6672 6f6d 5f79  DealCloud.from_y
+000027f0: 616d 6c28 2270 6174 682f 746f 2f79 616d  aml("path/to/yam
+00002800: 6c5f 636f 6e66 6967 5f66 696c 652e 6a73  l_config_file.js
+00002810: 6f6e 2229 0d0a 0d0a 7669 6577 7320 3d20  on")....views = 
+00002820: 6463 2e6c 6973 745f 636f 6e66 6967 7572  dc.list_configur
+00002830: 6564 5f76 6965 7773 2829 0d0a 6060 600d  ed_views()..```.
+00002840: 0a60 7669 6577 7360 2077 696c 6c20 636f  .`views` will co
+00002850: 6e74 6169 6e20 6120 7375 6d6d 6172 7920  ntain a summary 
+00002860: 6f66 2063 6f6e 6669 6775 7265 6420 7669  of configured vi
+00002870: 6577 732e 0d0a 0d0a 2323 2320 5265 6164  ews.....### Read
+00002880: 2044 6174 610d 0a60 4465 616c 436c 6f75   Data..`DealClou
+00002890: 642e 7265 6164 5f64 6174 6128 2960 2061  d.read_data()` a
+000028a0: 6c6c 6f77 7320 7573 6572 7320 746f 2072  llows users to r
+000028b0: 6561 6420 6461 7461 2066 726f 6d20 6120  ead data from a 
+000028c0: 4465 616c 436c 6f75 6420 6f62 6a65 6374  DealCloud object
+000028d0: 2069 6e74 6f20 6120 6070 616e 6461 732e   into a `pandas.
+000028e0: 4461 7461 4672 616d 6560 206f 7220 6120  DataFrame` or a 
+000028f0: 6c69 7374 206f 6620 7079 7468 6f6e 2064  list of python d
+00002900: 6963 7469 6f6e 6172 6965 732e 0d0a 3e20  ictionaries...> 
+00002910: 5b21 494d 504f 5254 414e 545d 200d 0a3e  [!IMPORTANT] ..>
+00002920: 204f 6e6c 7920 6f6e 6520 6f66 206f 626a   Only one of obj
+00002930: 6563 745f 6964 206f 7220 7669 6577 5f69  ect_id or view_i
+00002940: 6420 6361 6e20 6265 2070 6f70 756c 6174  d can be populat
+00002950: 6564 0d0a 2020 2020 2020 2020 0d0a 4172  ed..        ..Ar
+00002960: 6775 6d65 6e74 733a 0d0a 0d0a 2d20 6f62  guments:....- ob
+00002970: 6a65 6374 5f69 6420 6055 6e69 6f6e 5b69  ject_id `Union[i
+00002980: 6e74 2c20 7374 725d 603a 2074 6865 206f  nt, str]`: the o
+00002990: 626a 6563 7420 746f 2070 756c 6c20 6461  bject to pull da
+000029a0: 7461 2066 726f 6d0d 0a2d 2076 6965 775f  ta from..- view_
+000029b0: 6964 2060 556e 696f 6e5b 696e 742c 2073  id `Union[int, s
+000029c0: 7472 5d60 3a20 7468 6520 7669 6577 2074  tr]`: the view t
+000029d0: 6f20 7075 6c6c 2064 6174 6120 6672 6f6d  o pull data from
+000029e0: 0d0a 2d20 6f75 7470 7574 2060 7374 7260  ..- output `str`
+000029f0: 3a20 6070 616e 6461 7360 206f 7220 606c  : `pandas` or `l
+00002a00: 6973 7460 2c20 6465 6369 6465 7320 7468  ist`, decides th
+00002a10: 6520 6f75 7470 7574 2066 6f72 6d61 742c  e output format,
+00002a20: 2060 7061 6e64 6173 6020 6973 2064 6566   `pandas` is def
+00002a30: 6175 6c74 0d0a 2d20 7265 736f 6c76 6520  ault..- resolve 
+00002a40: 6073 7472 603a 2066 6f72 2070 616e 6461  `str`: for panda
+00002a50: 732c 2077 6865 7265 2066 6965 6c64 7320  s, where fields 
+00002a60: 636f 6e74 6169 6e20 616e 206f 626a 6563  contain an objec
+00002a70: 7420 2863 686f 6963 652c 2072 6566 6572  t (choice, refer
+00002a80: 656e 6365 2c20 7573 6572 292c 2072 6573  ence, user), res
+00002a90: 6f6c 7665 2074 6f20 7468 6520 6964 206f  olve to the id o
+00002aa0: 7220 6e61 6d65 0d0a 2d20 7669 6577 5f66  r name..- view_f
+00002ab0: 696c 7465 7220 606c 6973 745b 6469 6374  ilter `list[dict
+00002ac0: 5d60 3a20 636f 6c75 6d6e 2071 7565 7269  ]`: column queri
+00002ad0: 6573 2074 6f20 2273 7570 706c 7920 7661  es to "supply va
+00002ae0: 6c75 6520 6c61 7465 7222 2069 6e20 7669  lue later" in vi
+00002af0: 6577 732c 2073 6565 3a20 6874 7470 733a  ews, see: https:
+00002b00: 2f2f 6170 692e 646f 6373 2e64 6561 6c63  //api.docs.dealc
+00002b10: 6c6f 7564 2e63 6f6d 2f64 6f63 732f 6461  loud.com/docs/da
+00002b20: 7461 2f72 6f77 732f 7669 6577 5f64 6574  ta/rows/view_det
+00002b30: 6169 6c73 0d0a 2d20 6669 656c 6473 2060  ails..- fields `
+00002b40: 6c69 7374 5b73 7472 5d60 3a20 6966 206e  list[str]`: if n
+00002b50: 6f74 2060 4e6f 6e65 602c 2072 6574 7572  ot `None`, retur
+00002b60: 6e20 6f6e 6c79 2066 6965 6c64 7320 696e  n only fields in
+00002b70: 2074 6865 206c 6973 742e 200d 0a2d 2071   the list. ..- q
+00002b80: 7565 7279 2060 7374 7260 3a20 6120 4465  uery `str`: a De
+00002b90: 616c 436c 6f75 6420 726f 7773 2071 7565  alCloud rows que
+00002ba0: 7279 2073 7472 696e 6720 746f 2072 6571  ry string to req
+00002bb0: 7565 7374 2073 7065 6369 6669 6320 696e  uest specific in
+00002bc0: 666f 726d 6174 696f 6e2c 2073 6565 3a20  formation, see: 
+00002bd0: 6874 7470 733a 2f2f 6170 692e 646f 6373  https://api.docs
+00002be0: 2e64 6561 6c63 6c6f 7564 2e63 6f6d 2f64  .dealcloud.com/d
+00002bf0: 6f63 732f 6461 7461 2f72 6f77 732f 7175  ocs/data/rows/qu
+00002c00: 6572 790d 0a2d 2069 6e63 6c75 6465 5f6e  ery..- include_n
+00002c10: 756c 6c73 2060 626f 6f6c 603a 2069 6620  ulls `bool`: if 
+00002c20: 7472 7565 2c20 6e75 6c6c 2063 6f6c 756d  true, null colum
+00002c30: 6e73 2077 696c 6c20 616c 736f 2062 6520  ns will also be 
+00002c40: 7265 7475 726e 6564 0d0a 2d20 636f 6c75  returned..- colu
+00002c50: 6d6e 5f68 6561 6465 7273 2060 7374 7260  mn_headers `str`
+00002c60: 3a20 7370 6563 6966 6965 7320 7468 6520  : specifies the 
+00002c70: 7661 6c75 6520 7479 7065 206f 6620 7468  value type of th
+00002c80: 6520 7265 7475 726e 2066 6965 6c64 206b  e return field k
+00002c90: 6579 732f 636f 6c75 6d6e 206e 616d 6573  eys/column names
+00002ca0: 2e0d 0a20 202d 2060 6170 6960 203d 2046  ...  - `api` = F
+00002cb0: 6965 6c64 2041 5049 204e 616d 650d 0a20  ield API Name.. 
+00002cc0: 202d 2060 6e61 6d65 6020 3d20 4669 656c   - `name` = Fiel
+00002cd0: 6420 4469 7370 6c61 7920 4e61 6d65 0d0a  d Display Name..
+00002ce0: 2020 2d20 6069 6460 203d 2046 6965 6c64    - `id` = Field
+00002cf0: 2049 440d 0a0d 0a23 2323 2320 5265 6164   ID....#### Read
+00002d00: 696e 6720 4461 7461 2066 726f 6d20 616e  ing Data from an
+00002d10: 204f 626a 6563 740d 0a45 7861 6d70 6c65   Object..Example
+00002d20: 3a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  :....```python..
+00002d30: 6672 6f6d 2064 6561 6c63 6c6f 7564 5f73  from dealcloud_s
+00002d40: 646b 2069 6d70 6f72 7420 4465 616c 436c  dk import DealCl
+00002d50: 6f75 640d 0a0d 0a64 6320 3d20 4465 616c  oud....dc = Deal
+00002d60: 436c 6f75 642e 6672 6f6d 5f79 616d 6c28  Cloud.from_yaml(
+00002d70: 2270 6174 682f 746f 2f79 616d 6c5f 636f  "path/to/yaml_co
+00002d80: 6e66 6967 5f66 696c 652e 6a73 6f6e 2229  nfig_file.json")
+00002d90: 0d0a 0d0a 6461 7461 203d 2064 632e 7265  ....data = dc.re
+00002da0: 6164 5f64 6174 6128 2243 6f6d 7061 6e79  ad_data("Company
+00002db0: 2229 0d0a 6060 600d 0a60 6461 7461 6020  ")..```..`data` 
+00002dc0: 7769 6c6c 2062 6520 6120 6070 616e 6461  will be a `panda
+00002dd0: 732e 4461 7461 4672 616d 6560 2061 7320  s.DataFrame` as 
+00002de0: 6265 6c6f 773a 0d0a 0d0a 7c20 456e 7472  below:....| Entr
+00002df0: 7949 6420 7c20 436f 6d70 616e 794e 616d  yId | CompanyNam
+00002e00: 6520 7c20 436f 6d70 616e 7954 7970 6520  e | CompanyType 
+00002e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e60: 2020 2020 2020 2020 2020 207c 0d0a 7c2d             |..|-
+00002e70: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
+00002e80: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
+00002e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002ed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+00002ef0: 0d0a 7c20 3132 3334 3520 2020 7c20 436f  ..| 12345   | Co
+00002f00: 6d70 616e 7931 2020 2020 7c20 5b7b 2773  mpany1    | [{'s
+00002f10: 6571 4e75 6d62 6572 273a 2033 2c20 2769  eqNumber': 3, 'i
+00002f20: 7341 7574 6f50 6466 273a 2046 616c 7365  sAutoPdf': False
+00002f30: 2c20 2769 6427 3a20 3331 3937 3738 302c  , 'id': 3197780,
+00002f40: 2027 6e61 6d65 273a 2027 4c69 6d69 7465   'name': 'Limite
+00002f50: 6420 5061 7274 6e65 7227 2c20 2765 6e74  d Partner', 'ent
+00002f60: 7279 4c69 7374 4964 273a 202d 367d 5d20  ryListId': -6}] 
+00002f70: 2020 207c 0d0a 7c20 3132 3334 3620 2020     |..| 12346   
+00002f80: 7c20 436f 6d70 616e 7932 2020 2020 7c20  | Company2    | 
+00002f90: 5b7b 2773 6571 4e75 6d62 6572 273a 2031  [{'seqNumber': 1
+00002fa0: 2c20 2769 7341 7574 6f50 6466 273a 2046  , 'isAutoPdf': F
+00002fb0: 616c 7365 2c20 2769 6427 3a20 3331 3937  alse, 'id': 3197
+00002fc0: 3738 322c 2027 6e61 6d65 273a 2027 4f70  782, 'name': 'Op
+00002fd0: 6572 6174 696e 6720 436f 6d70 616e 7927  erating Company'
+00002fe0: 2c20 2765 6e74 7279 4c69 7374 4964 273a  , 'entryListId':
+00002ff0: 202d 367d 5d20 207c 0d0a 7c20 3132 3334   -6}]  |..| 1234
+00003000: 3720 2020 7c20 436f 6d70 616e 7933 2020  7   | Company3  
+00003010: 2020 7c20 5b7b 2773 6571 4e75 6d62 6572    | [{'seqNumber
+00003020: 273a 2033 2c20 2769 7341 7574 6f50 6466  ': 3, 'isAutoPdf
+00003030: 273a 2046 616c 7365 2c20 2769 6427 3a20  ': False, 'id': 
+00003040: 3331 3937 3738 302c 2027 6e61 6d65 273a  3197780, 'name':
+00003050: 2027 4c69 6d69 7465 6420 5061 7274 6e65   'Limited Partne
+00003060: 7227 2c20 2765 6e74 7279 4c69 7374 4964  r', 'entryListId
+00003070: 273a 202d 367d 5d20 2020 207c 0d0a 0d0a  ': -6}]    |....
+00003080: 546f 2072 6574 7572 6e20 6120 7079 7468  To return a pyth
+00003090: 6f6e 2060 6c69 7374 6020 696e 7374 6561  on `list` instea
+000030a0: 6420 6f66 2061 2060 7061 6e64 6173 2e44  d of a `pandas.D
+000030b0: 6174 6146 7261 6d65 603a 0d0a 0d0a 6060  ataFrame`:....``
+000030c0: 6070 7974 686f 6e0d 0a66 726f 6d20 6465  `python..from de
+000030d0: 616c 636c 6f75 645f 7364 6b20 696d 706f  alcloud_sdk impo
+000030e0: 7274 2044 6561 6c43 6c6f 7564 0d0a 0d0a  rt DealCloud....
+000030f0: 6463 203d 2044 6561 6c43 6c6f 7564 2e66  dc = DealCloud.f
+00003100: 726f 6d5f 7961 6d6c 2822 7061 7468 2f74  rom_yaml("path/t
+00003110: 6f2f 7961 6d6c 5f63 6f6e 6669 675f 6669  o/yaml_config_fi
+00003120: 6c65 2e6a 736f 6e22 290d 0a0d 0a64 6174  le.json")....dat
+00003130: 6120 3d20 6463 2e72 6561 645f 6461 7461  a = dc.read_data
+00003140: 2822 436f 6d70 616e 7922 2c20 6f75 7470  ("Company", outp
+00003150: 7574 3d22 6c69 7374 2229 0d0a 6060 600d  ut="list")..```.
+00003160: 0a60 6461 7461 6020 7769 6c6c 2062 6520  .`data` will be 
+00003170: 6120 606c 6973 7460 206f 6620 6064 6963  a `list` of `dic
+00003180: 7460 7320 6173 2062 656c 6f77 3a0d 0a60  t`s as below:..`
+00003190: 6060 7079 7468 6f6e 0d0a 5b0d 0a20 2020  ``python..[..   
+000031a0: 207b 0d0a 2020 2020 2020 2020 2745 6e74   {..        'Ent
+000031b0: 7279 4964 273a 2031 3233 3435 2c0d 0a20  ryId': 12345,.. 
+000031c0: 2020 2020 2020 2027 436f 6d70 616e 794e         'CompanyN
+000031d0: 616d 6527 3a20 2743 6f6d 7061 6e79 3127  ame': 'Company1'
+000031e0: 2c0d 0a20 2020 2020 2020 2027 436f 6d70  ,..        'Comp
+000031f0: 616e 7954 7970 6527 3a20 5b0d 0a20 2020  anyType': [..   
+00003200: 2020 2020 2020 2020 2020 7b0d 0a20 2020            {..   
+00003210: 2020 2020 2020 2020 2020 2020 2027 7365               'se
+00003220: 714e 756d 6265 7227 3a20 332c 0d0a 2020  qNumber': 3,..  
+00003230: 2020 2020 2020 2020 2020 2020 2020 2769                'i
+00003240: 7341 7574 6f50 6466 273a 2046 616c 7365  sAutoPdf': False
+00003250: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003260: 2020 2027 6964 273a 2033 3139 3737 3830     'id': 3197780
+00003270: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003280: 2020 2027 6e61 6d65 273a 2027 4c69 6d69     'name': 'Limi
+00003290: 7465 6420 5061 7274 6e65 7227 2c0d 0a20  ted Partner',.. 
+000032a0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000032b0: 656e 7472 794c 6973 7449 6427 3a20 2d36  entryListId': -6
+000032c0: 0d0a 2020 2020 2020 2020 2020 2020 207d  ..             }
+000032d0: 0d0a 2020 2020 2020 205d 2c0d 0a20 2020  ..       ],..   
+000032e0: 207d 2c0d 0a20 2020 207b 0d0a 2020 2020   },..    {..    
+000032f0: 2020 2745 6e74 7279 4964 273a 2031 3233    'EntryId': 123
+00003300: 3436 2c0d 0a20 2020 2020 2027 436f 6d70  46,..      'Comp
+00003310: 616e 794e 616d 6527 3a20 2743 6f6d 7061  anyName': 'Compa
+00003320: 6e79 3227 2c0d 0a20 2020 2020 2027 436f  ny2',..      'Co
+00003330: 6d70 616e 7954 7970 6527 3a20 5b0d 0a20  mpanyType': [.. 
+00003340: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
+00003350: 2020 2020 2020 2027 7365 714e 756d 6265         'seqNumbe
+00003360: 7227 3a20 312c 0d0a 2020 2020 2020 2020  r': 1,..        
+00003370: 2020 2020 2769 7341 7574 6f50 6466 273a      'isAutoPdf':
+00003380: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
+00003390: 2020 2020 2027 6964 273a 2033 3139 3737       'id': 31977
+000033a0: 3832 2c0d 0a20 2020 2020 2020 2020 2020  82,..           
+000033b0: 2027 6e61 6d65 273a 2027 4f70 6572 6174   'name': 'Operat
+000033c0: 696e 6720 436f 6d70 616e 7927 2c0d 0a20  ing Company',.. 
+000033d0: 2020 2020 2020 2020 2020 2027 656e 7472             'entr
+000033e0: 794c 6973 7449 6427 3a20 2d36 0d0a 2020  yListId': -6..  
+000033f0: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+00003400: 5d0d 0a20 2020 207d 2c0d 0a20 2020 207b  ]..    },..    {
+00003410: 0d0a 2020 2020 2020 2027 456e 7472 7949  ..       'EntryI
+00003420: 6427 3a20 3132 3334 372c 0d0a 2020 2020  d': 12347,..    
+00003430: 2020 2020 2743 6f6d 7061 6e79 4e61 6d65      'CompanyName
+00003440: 273a 2027 436f 6d70 616e 7933 272c 0d0a  ': 'Company3',..
+00003450: 2020 2020 2020 2020 2743 6f6d 7061 6e79          'Company
+00003460: 5479 7065 273a 205b 0d0a 2020 2020 2020  Type': [..      
+00003470: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+00003480: 2020 2020 2020 2020 2773 6571 4e75 6d62          'seqNumb
+00003490: 6572 273a 2034 2c0d 0a20 2020 2020 2020  er': 4,..       
+000034a0: 2020 2020 2020 2020 2027 6973 4175 746f           'isAuto
+000034b0: 5064 6627 3a20 4661 6c73 652c 0d0a 2020  Pdf': False,..  
+000034c0: 2020 2020 2020 2020 2020 2020 2020 2769                'i
+000034d0: 6427 3a20 3331 3937 3737 392c 0d0a 2020  d': 3197779,..  
+000034e0: 2020 2020 2020 2020 2020 2020 2020 276e                'n
+000034f0: 616d 6527 3a20 2753 6572 7669 6365 2050  ame': 'Service P
+00003500: 726f 7669 6465 7227 2c0d 0a20 2020 2020  rovider',..     
+00003510: 2020 2020 2020 2020 2020 2027 656e 7472             'entr
+00003520: 794c 6973 7449 6427 3a20 2d36 0d0a 2020  yListId': -6..  
+00003530: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
+00003540: 2020 2020 5d0d 0a20 2020 207d 2c0d 0a20      ]..    },.. 
+00003550: 5d0d 0a60 6060 0d0a 0d0a 2323 2323 2320  ]..```....##### 
+00003560: 5265 736f 6c76 696e 6720 746f 204e 616d  Resolving to Nam
+00003570: 6520 6f72 2074 6f20 4944 0d0a 3e20 5b21  e or to ID..> [!
+00003580: 4e4f 5445 5d0d 0a3e 2054 6865 2066 6f6c  NOTE]..> The fol
+00003590: 6c6f 7769 6e67 206d 6574 686f 6473 206f  lowing methods o
+000035a0: 6e6c 7920 6170 706c 7920 746f 2077 6865  nly apply to whe
+000035b0: 7265 2061 2060 7061 6e64 6173 2e44 6174  re a `pandas.Dat
+000035c0: 6146 7261 6d65 6020 6973 2072 6574 7572  aFrame` is retur
+000035d0: 6e65 642e 0d0a 0d0a 4368 6f69 6365 2c20  ned.....Choice, 
+000035e0: 5265 6665 7265 6e63 6520 616e 6420 5573  Reference and Us
+000035f0: 6572 2066 6965 6c64 7320 6170 7065 6172  er fields appear
+00003600: 2061 7320 6c69 7374 7320 6f66 2064 6963   as lists of dic
+00003610: 7469 6f6e 6172 6965 7320 6173 2073 6565  tionaries as see
+00003620: 6e20 696e 2074 6865 205b 6162 6f76 6520  n in the [above 
+00003630: 6578 616d 706c 655d 2823 7265 6164 696e  example](#readin
+00003640: 672d 6461 7461 2d66 726f 6d2d 616e 2d6f  g-data-from-an-o
+00003650: 626a 6563 7429 2062 7920 6465 6661 756c  bject) by defaul
+00003660: 742e 0d0a 0d0a 546f 2072 6573 6f6c 7665  t.....To resolve
+00003670: 2074 6865 7365 2066 6965 6c64 7320 746f   these fields to
+00003680: 2061 206d 6f72 6520 7265 6164 6162 6c65   a more readable
+00003690: 2060 6e61 6d65 6020 7661 6c75 653a 0d0a   `name` value:..
+000036a0: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
+000036b0: 6d20 6465 616c 636c 6f75 645f 7364 6b20  m dealcloud_sdk 
+000036c0: 696d 706f 7274 2044 6561 6c43 6c6f 7564  import DealCloud
+000036d0: 0d0a 0d0a 6463 203d 2044 6561 6c43 6c6f  ....dc = DealClo
+000036e0: 7564 2e66 726f 6d5f 7961 6d6c 2822 7061  ud.from_yaml("pa
+000036f0: 7468 2f74 6f2f 7961 6d6c 5f63 6f6e 6669  th/to/yaml_confi
+00003700: 675f 6669 6c65 2e6a 736f 6e22 290d 0a0d  g_file.json")...
+00003710: 0a64 6174 6120 3d20 6463 2e72 6561 645f  .data = dc.read_
+00003720: 6461 7461 2822 436f 6d70 616e 7922 2c20  data("Company", 
+00003730: 7265 736f 6c76 653d 226e 616d 6522 290d  resolve="name").
+00003740: 0a60 6060 0d0a 6064 6174 6160 2077 696c  .```..`data` wil
+00003750: 6c20 6265 2061 2060 7061 6e64 6173 2e44  l be a `pandas.D
+00003760: 6174 6146 7261 6d65 6020 6173 2062 656c  ataFrame` as bel
+00003770: 6f77 3a0d 0a0d 0a7c 2045 6e74 7279 4964  ow:....| EntryId
+00003780: 207c 2043 6f6d 7061 6e79 4e61 6d65 207c   | CompanyName |
+00003790: 2043 6f6d 7061 6e79 5479 7065 2020 2020   CompanyType    
+000037a0: 2020 2020 7c0d 0a7c 2d2d 2d2d 2d2d 2d2d      |..|--------
+000037b0: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  -|-------------|
+000037c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000037d0: 2d2d 2d2d 7c0d 0a7c 2031 3233 3435 2020  ----|..| 12345  
+000037e0: 207c 2043 6f6d 7061 6e79 3120 2020 207c   | Company1    |
+000037f0: 204c 696d 6974 6564 2050 6172 746e 6572   Limited Partner
+00003800: 2020 2020 7c0d 0a7c 2031 3233 3436 2020      |..| 12346  
+00003810: 207c 2043 6f6d 7061 6e79 3220 2020 207c   | Company2    |
+00003820: 204f 7065 7261 7469 6e67 2043 6f6d 7061   Operating Compa
+00003830: 6e79 2020 7c0d 0a7c 2031 3233 3437 2020  ny  |..| 12347  
+00003840: 207c 2043 6f6d 7061 6e79 3320 2020 207c   | Company3    |
+00003850: 204c 696d 6974 6564 2050 6172 746e 6572   Limited Partner
+00003860: 2020 2020 7c0d 0a0d 0a54 6f20 7265 736f      |....To reso
+00003870: 6c76 6520 7468 6520 6669 656c 6473 2074  lve the fields t
+00003880: 6f20 616e 2060 6964 6020 7661 6c75 653a  o an `id` value:
+00003890: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a66  ....```python..f
+000038a0: 726f 6d20 6465 616c 636c 6f75 645f 7364  rom dealcloud_sd
+000038b0: 6b20 696d 706f 7274 2044 6561 6c43 6c6f  k import DealClo
+000038c0: 7564 0d0a 0d0a 6463 203d 2044 6561 6c43  ud....dc = DealC
+000038d0: 6c6f 7564 2e66 726f 6d5f 7961 6d6c 2822  loud.from_yaml("
+000038e0: 7061 7468 2f74 6f2f 7961 6d6c 5f63 6f6e  path/to/yaml_con
+000038f0: 6669 675f 6669 6c65 2e6a 736f 6e22 290d  fig_file.json").
+00003900: 0a0d 0a64 6174 6120 3d20 6463 2e72 6561  ...data = dc.rea
+00003910: 645f 6461 7461 2822 436f 6d70 616e 7922  d_data("Company"
+00003920: 2c20 7265 736f 6c76 653d 2269 6422 290d  , resolve="id").
+00003930: 0a60 6060 0d0a 6064 6174 6160 2077 696c  .```..`data` wil
+00003940: 6c20 6265 2061 2060 7061 6e64 6173 2e44  l be a `pandas.D
+00003950: 6174 6146 7261 6d65 6020 6173 2062 656c  ataFrame` as bel
+00003960: 6f77 3a0d 0a0d 0a7c 2045 6e74 7279 4964  ow:....| EntryId
+00003970: 207c 2043 6f6d 7061 6e79 4e61 6d65 207c   | CompanyName |
+00003980: 2043 6f6d 7061 6e79 5479 7065 207c 0d0a   CompanyType |..
+00003990: 7c2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  |---------|-----
+000039a0: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
+000039b0: 2d2d 2d2d 2d2d 7c0d 0a7c 2031 3233 3435  ------|..| 12345
+000039c0: 2020 207c 2043 6f6d 7061 6e79 3120 2020     | Company1   
+000039d0: 207c 2033 3139 3737 3830 2020 2020 207c   | 3197780     |
+000039e0: 0d0a 7c20 3132 3334 3620 2020 7c20 436f  ..| 12346   | Co
+000039f0: 6d70 616e 7932 2020 2020 7c20 3331 3937  mpany2    | 3197
+00003a00: 3738 3220 2020 2020 7c0d 0a7c 2031 3233  782     |..| 123
+00003a10: 3437 2020 207c 2043 6f6d 7061 6e79 3320  47   | Company3 
+00003a20: 2020 207c 2033 3139 3737 3830 2020 2020     | 3197780    
+00003a30: 207c 0d0a 0d0a 2323 2323 2320 5265 6164   |....##### Read
+00003a40: 696e 6720 6120 5375 6273 6574 206f 6620  ing a Subset of 
+00003a50: 4669 656c 6473 0d0a 546f 2072 6561 6420  Fields..To read 
+00003a60: 6120 7370 6563 6966 6963 2073 6574 206f  a specific set o
+00003a70: 6620 6669 656c 6473 2066 726f 6d20 616e  f fields from an
+00003a80: 206f 626a 6563 742c 2070 6173 7320 6120   object, pass a 
+00003a90: 6c69 7374 206f 6620 4465 616c 436c 6f75  list of DealClou
+00003aa0: 6420 6669 656c 6420 4150 4920 6e61 6d65  d field API name
+00003ab0: 7320 746f 2074 6865 2061 7267 756d 656e  s to the argumen
+00003ac0: 7420 6066 6965 6c64 7360 3a0d 0a0d 0a60  t `fields`:....`
+00003ad0: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2064  ``python..from d
+00003ae0: 6561 6c63 6c6f 7564 5f73 646b 2069 6d70  ealcloud_sdk imp
+00003af0: 6f72 7420 4465 616c 436c 6f75 640d 0a0d  ort DealCloud...
+00003b00: 0a64 6320 3d20 4465 616c 436c 6f75 642e  .dc = DealCloud.
+00003b10: 6672 6f6d 5f79 616d 6c28 2270 6174 682f  from_yaml("path/
+00003b20: 746f 2f79 616d 6c5f 636f 6e66 6967 5f66  to/yaml_config_f
+00003b30: 696c 652e 6a73 6f6e 2229 0d0a 0d0a 6461  ile.json")....da
+00003b40: 7461 203d 2064 632e 7265 6164 5f64 6174  ta = dc.read_dat
+00003b50: 6128 2243 6f6d 7061 6e79 222c 2066 6965  a("Company", fie
+00003b60: 6c64 733d 5b22 436f 6d70 616e 794e 616d  lds=["CompanyNam
+00003b70: 6522 5d29 0d0a 6060 600d 0a60 6461 7461  e"])..```..`data
+00003b80: 6020 7769 6c6c 2062 6520 6120 6070 616e  ` will be a `pan
+00003b90: 6461 732e 4461 7461 4672 616d 6560 2061  das.DataFrame` a
+00003ba0: 7320 6265 6c6f 773a 0d0a 0d0a 7c20 456e  s below:....| En
+00003bb0: 7472 7949 6420 7c20 436f 6d70 616e 794e  tryId | CompanyN
+00003bc0: 616d 6520 7c0d 0a7c 2d2d 2d2d 2d2d 2d2d  ame |..|--------
+00003bd0: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  -|-------------|
+00003be0: 0d0a 7c20 3132 3334 3520 2020 7c20 436f  ..| 12345   | Co
+00003bf0: 6d70 616e 7931 2020 2020 7c0d 0a7c 2031  mpany1    |..| 1
+00003c00: 3233 3436 2020 207c 2043 6f6d 7061 6e79  2346   | Company
+00003c10: 3220 2020 207c 0d0a 7c20 3132 3334 3720  2    |..| 12347 
+00003c20: 2020 7c20 436f 6d70 616e 7933 2020 2020    | Company3    
+00003c30: 7c0d 0a0d 0a23 2323 2323 2055 7369 6e67  |....##### Using
+00003c40: 2051 7565 7269 6573 2074 6f20 5265 6164   Queries to Read
+00003c50: 2044 6174 610d 0a41 2071 7565 7279 2063   Data..A query c
+00003c60: 616e 2062 6520 7061 7373 6564 2074 6f20  an be passed to 
+00003c70: 7468 6520 4465 616c 436c 6f75 6420 7265  the DealCloud re
+00003c80: 7175 6573 7420 666f 7220 6461 7461 2074  quest for data t
+00003c90: 6f20 7265 7475 726e 206d 6f72 6520 7370  o return more sp
+00003ca0: 6563 6966 6963 2069 6e66 6f72 6d61 7469  ecific informati
+00003cb0: 6f6e 2c20 616e 6420 7265 6475 6365 2074  on, and reduce t
+00003cc0: 6865 2076 6f6c 756d 6520 6f66 2069 6e63  he volume of inc
+00003cd0: 6f6d 696e 6720 6461 7461 2e0d 0a54 6f20  oming data...To 
+00003ce0: 7573 6520 6120 7175 6572 792c 2070 6173  use a query, pas
+00003cf0: 7320 7468 6520 7175 6572 7920 7374 7269  s the query stri
+00003d00: 6e67 2074 6f20 7468 6520 6071 7565 7279  ng to the `query
+00003d10: 6020 6172 6775 6d65 6e74 2e0d 0a54 6865  ` argument...The
+00003d20: 2061 7661 696c 6162 6c65 2071 7565 7279   available query
+00003d30: 206f 7065 7261 7469 6f6e 7320 6172 6520   operations are 
+00003d40: 6265 6c6f 773a 0d0a 0d0a 7c20 4e61 6d65  below:....| Name
+00003d50: 2020 2020 2020 2020 2020 207c 2051 7565             | Que
+00003d60: 7279 204f 7065 7261 7469 6f6e 207c 0d0a  ry Operation |..
+00003d70: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
+00003d80: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
+00003d90: 2d2d 2d7c 0d0a 7c20 4571 7561 6c73 2020  ---|..| Equals  
+00003da0: 2020 2020 2020 207c 2024 6571 2020 2020         | $eq    
+00003db0: 2020 2020 2020 2020 207c 0d0a 7c20 436f           |..| Co
+00003dc0: 6e74 6169 6e73 2020 2020 2020 207c 2024  ntains       | $
+00003dd0: 636f 6e74 6169 6e73 2020 2020 2020 207c  contains       |
+00003de0: 0d0a 7c20 4772 6561 7465 7220 2020 2020  ..| Greater     
+00003df0: 2020 207c 2024 6774 2020 2020 2020 2020     | $gt        
+00003e00: 2020 2020 207c 0d0a 7c20 4772 6561 7465       |..| Greate
+00003e10: 724f 7245 7175 616c 207c 2024 6774 6520  rOrEqual | $gte 
+00003e20: 2020 2020 2020 2020 2020 207c 0d0a 7c20             |..| 
+00003e30: 4c65 7373 2020 2020 2020 2020 2020 207c  Less           |
+00003e40: 2024 6c74 2020 2020 2020 2020 2020 2020   $lt            
+00003e50: 207c 0d0a 7c20 4c65 7373 4f72 4571 7561   |..| LessOrEqua
+00003e60: 6c73 2020 207c 2024 6c74 6520 2020 2020  ls   | $lte     
+00003e70: 2020 2020 2020 207c 0d0a 7c20 5374 6172         |..| Star
+00003e80: 7473 5769 7468 2020 2020 207c 2024 7374  tsWith     | $st
+00003e90: 6172 7473 7769 7468 2020 2020 207c 0d0a  artswith     |..
+00003ea0: 7c20 496e 2020 2020 2020 2020 2020 2020  | In            
+00003eb0: 207c 2024 696e 2020 2020 2020 2020 2020   | $in          
+00003ec0: 2020 207c 0d0a 7c20 4265 7477 6565 6e20     |..| Between 
+00003ed0: 2020 2020 2020 207c 2024 6265 7477 6565         | $betwee
+00003ee0: 6e20 2020 2020 2020 207c 0d0a 7c20 4e6f  n        |..| No
+00003ef0: 7449 6e20 2020 2020 2020 2020 207c 2024  tIn          | $
+00003f00: 6e69 6e20 2020 2020 2020 2020 2020 207c  nin            |
+00003f10: 0d0a 7c20 4e6f 7445 7175 616c 546f 2020  ..| NotEqualTo  
+00003f20: 2020 207c 2024 6e6f 7420 2020 2020 2020     | $not       
+00003f30: 2020 2020 207c 0d0a 7c20 456e 6473 5769       |..| EndsWi
+00003f40: 7468 2020 2020 2020 207c 2024 656e 6473  th       | $ends
+00003f50: 7769 7468 2020 2020 2020 207c 0d0a 7c20  with       |..| 
+00003f60: 4f72 2020 2020 2020 2020 2020 2020 207c  Or             |
+00003f70: 2024 6f72 2020 2020 2020 2020 2020 2020   $or            
+00003f80: 207c 0d0a 7c20 416e 6420 2020 2020 2020   |..| And       
+00003f90: 2020 2020 207c 2024 616e 6420 2020 2020       | $and     
+00003fa0: 2020 2020 2020 207c 0d0a 0d0a 6060 6070         |....```p
+00003fb0: 7974 686f 6e0d 0a66 726f 6d20 6465 616c  ython..from deal
+00003fc0: 636c 6f75 645f 7364 6b20 696d 706f 7274  cloud_sdk import
+00003fd0: 2044 6561 6c43 6c6f 7564 0d0a 0d0a 6463   DealCloud....dc
+00003fe0: 203d 2044 6561 6c43 6c6f 7564 2e66 726f   = DealCloud.fro
+00003ff0: 6d5f 7961 6d6c 2822 7061 7468 2f74 6f2f  m_yaml("path/to/
+00004000: 7961 6d6c 5f63 6f6e 6669 675f 6669 6c65  yaml_config_file
+00004010: 2e6a 736f 6e22 290d 0a0d 0a64 632e 7265  .json")....dc.re
+00004020: 6164 5f64 6174 6128 2243 6f6d 7061 6e79  ad_data("Company
+00004030: 222c 2071 7565 7279 3d22 7b43 6f6d 7061  ", query="{Compa
+00004040: 6e79 4e61 6d65 3a20 7b24 636f 6e74 6169  nyName: {$contai
+00004050: 6e73 3a20 5c22 315c 227d 7d22 290d 0a60  ns: \"1\"}}")..`
+00004060: 6060 0d0a 6064 6174 6160 2077 696c 6c20  ``..`data` will 
+00004070: 6265 2061 2060 7061 6e64 6173 2e44 6174  be a `pandas.Dat
+00004080: 6146 7261 6d65 6020 6173 2062 656c 6f77  aFrame` as below
+00004090: 3a0d 0a0d 0a7c 2045 6e74 7279 4964 207c  :....| EntryId |
+000040a0: 2043 6f6d 7061 6e79 4e61 6d65 207c 2043   CompanyName | C
+000040b0: 6f6d 7061 6e79 5479 7065 207c 0d0a 7c2d  ompanyType |..|-
+000040c0: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
+000040d0: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
+000040e0: 2d2d 2d2d 7c0d 0a7c 2031 3233 3435 2020  ----|..| 12345  
+000040f0: 207c 2043 6f6d 7061 6e79 3120 2020 207c   | Company1    |
+00004100: 2033 3139 3737 3830 2020 2020 207c 0d0a   3197780     |..
+00004110: 0d0a 536f 6d65 206f 7468 6572 2065 7861  ..Some other exa
+00004120: 6d70 6c65 2071 7565 7279 2073 7472 696e  mple query strin
+00004130: 6773 2061 7265 2062 656c 6f77 3a0d 0a46  gs are below:..F
+00004140: 696c 7465 7220 6f6e 2065 7863 6c75 6469  ilter on excludi
+00004150: 6e67 2072 6563 6f72 6473 2077 6974 6820  ng records with 
+00004160: 6120 7370 6563 6966 6963 2072 6566 6572  a specific refer
+00004170: 656e 6365 2076 616c 7565 3a0d 0a0d 0a60  ence value:....`
+00004180: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2064  ``python..from d
+00004190: 6561 6c63 6c6f 7564 5f73 646b 2069 6d70  ealcloud_sdk imp
+000041a0: 6f72 7420 4465 616c 436c 6f75 640d 0a0d  ort DealCloud...
+000041b0: 0a64 6320 3d20 4465 616c 436c 6f75 642e  .dc = DealCloud.
+000041c0: 6672 6f6d 5f79 616d 6c28 2270 6174 682f  from_yaml("path/
+000041d0: 746f 2f79 616d 6c5f 636f 6e66 6967 5f66  to/yaml_config_f
+000041e0: 696c 652e 6a73 6f6e 2229 0d0a 0d0a 6463  ile.json")....dc
+000041f0: 2e72 6561 645f 6461 7461 2822 436f 6d70  .read_data("Comp
+00004200: 616e 7922 2c20 7175 6572 793d 227b 436f  any", query="{Co
+00004210: 7665 7261 6765 5065 7273 6f6e 3a20 7b24  veragePerson: {$
+00004220: 6e69 6e3a 205b 3537 3835 5d7d 2229 0d0a  nin: [5785]}")..
+00004230: 6060 600d 0a46 696c 7465 7220 7573 696e  ```..Filter usin
+00004240: 6720 4f72 3a0d 0a0d 0a60 6060 7079 7468  g Or:....```pyth
+00004250: 6f6e 0d0a 6672 6f6d 2064 6561 6c63 6c6f  on..from dealclo
+00004260: 7564 5f73 646b 2069 6d70 6f72 7420 4465  ud_sdk import De
+00004270: 616c 436c 6f75 640d 0a0d 0a64 6320 3d20  alCloud....dc = 
+00004280: 4465 616c 436c 6f75 642e 6672 6f6d 5f79  DealCloud.from_y
+00004290: 616d 6c28 2270 6174 682f 746f 2f79 616d  aml("path/to/yam
+000042a0: 6c5f 636f 6e66 6967 5f66 696c 652e 6a73  l_config_file.js
+000042b0: 6f6e 2229 0d0a 0d0a 6463 2e72 6561 645f  on")....dc.read_
+000042c0: 6461 7461 2822 436f 6d70 616e 7922 2c20  data("Company", 
+000042d0: 7175 6572 793d 227b 246f 723a 205b 7b43  query="{$or: [{C
+000042e0: 6f6d 7061 6e79 4e61 6d65 3a20 5c22 4465  ompanyName: \"De
+000042f0: 616c 436c 6f75 645c 227d 2c7b 436f 6d70  alCloud\"},{Comp
+00004300: 616e 794e 616d 653a 205c 2241 5049 2045  anyName: \"API E
+00004310: 6e74 7279 5c22 7d5d 7d22 290d 0a60 6060  ntry\"}]}")..```
+00004320: 0d0a 0d0a 2323 2323 2052 6561 6469 6e67  ....#### Reading
+00004330: 2044 6174 6120 6672 6f6d 2061 2056 6965   Data from a Vie
+00004340: 770d 0a54 6f20 7265 6164 2064 6174 6120  w..To read data 
+00004350: 6672 6f6d 2061 2076 6965 7720 7769 7468  from a view with
+00004360: 2049 443a 2060 3132 3334 3560 0d0a 0d0a   ID: `12345`....
+00004370: 4578 616d 706c 653a 0d0a 0d0a 6060 6070  Example:....```p
+00004380: 7974 686f 6e0d 0a66 726f 6d20 6465 616c  ython..from deal
+00004390: 636c 6f75 645f 7364 6b20 696d 706f 7274  cloud_sdk import
+000043a0: 2044 6561 6c43 6c6f 7564 0d0a 0d0a 6463   DealCloud....dc
+000043b0: 203d 2044 6561 6c43 6c6f 7564 2e66 726f   = DealCloud.fro
+000043c0: 6d5f 7961 6d6c 2822 7061 7468 2f74 6f2f  m_yaml("path/to/
+000043d0: 7961 6d6c 5f63 6f6e 6669 675f 6669 6c65  yaml_config_file
+000043e0: 2e6a 736f 6e22 290d 0a0d 0a64 6174 6120  .json")....data 
+000043f0: 3d20 6463 2e72 6561 645f 6461 7461 2876  = dc.read_data(v
+00004400: 6965 775f 6964 3d31 3233 3435 290d 0a60  iew_id=12345)..`
+00004410: 6060 0d0a 416c 7465 726e 6174 6976 656c  ``..Alternativel
+00004420: 792c 2069 6620 7468 6520 7669 6577 2069  y, if the view i
+00004430: 7320 6e61 6d65 643a 2022 4d79 2043 6f6d  s named: "My Com
+00004440: 7061 6e79 2056 6965 7722 3a0d 0a0d 0a60  pany View":....`
+00004450: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2064  ``python..from d
+00004460: 6561 6c63 6c6f 7564 5f73 646b 2069 6d70  ealcloud_sdk imp
+00004470: 6f72 7420 4465 616c 436c 6f75 640d 0a0d  ort DealCloud...
+00004480: 0a64 6320 3d20 4465 616c 436c 6f75 642e  .dc = DealCloud.
+00004490: 6672 6f6d 5f79 616d 6c28 2270 6174 682f  from_yaml("path/
+000044a0: 746f 2f79 616d 6c5f 636f 6e66 6967 5f66  to/yaml_config_f
+000044b0: 696c 652e 6a73 6f6e 2229 0d0a 0d0a 6461  ile.json")....da
+000044c0: 7461 203d 2064 632e 7265 6164 5f64 6174  ta = dc.read_dat
+000044d0: 6128 7669 6577 5f69 643d 224d 7920 436f  a(view_id="My Co
+000044e0: 6d70 616e 7920 5669 6577 2229 0d0a 6060  mpany View")..``
+000044f0: 600d 0a0d 0a60 6461 7461 6020 7769 6c6c  `....`data` will
+00004500: 2062 6520 6120 6070 616e 6461 732e 4461   be a `pandas.Da
+00004510: 7461 4672 616d 6560 2061 7320 6265 6c6f  taFrame` as belo
+00004520: 773a 0d0a 0d0a 7c20 456e 7472 7949 6420  w:....| EntryId 
+00004530: 7c20 436f 6d70 616e 794e 616d 6520 7c20  | CompanyName | 
+00004540: 436f 6d70 616e 7954 7970 6520 2020 2020  CompanyType     
+00004550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045a0: 2020 2020 2020 207c 0d0a 7c2d 2d2d 2d2d         |..|-----
+000045b0: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
+000045c0: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|-------------
+000045d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000045e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000045f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0d0a 7c20  -----------|..| 
+00004630: 3132 3334 3520 2020 7c20 436f 6d70 616e  12345   | Compan
+00004640: 7931 2020 2020 7c20 5b7b 2773 6571 4e75  y1    | [{'seqNu
+00004650: 6d62 6572 273a 2033 2c20 2769 7341 7574  mber': 3, 'isAut
+00004660: 6f50 6466 273a 2046 616c 7365 2c20 2769  oPdf': False, 'i
+00004670: 6427 3a20 3331 3937 3738 302c 2027 6e61  d': 3197780, 'na
+00004680: 6d65 273a 2027 4c69 6d69 7465 6420 5061  me': 'Limited Pa
+00004690: 7274 6e65 7227 2c20 2765 6e74 7279 4c69  rtner', 'entryLi
+000046a0: 7374 4964 273a 202d 367d 5d20 2020 207c  stId': -6}]    |
+000046b0: 0d0a 7c20 3132 3334 3620 2020 7c20 436f  ..| 12346   | Co
+000046c0: 6d70 616e 7932 2020 2020 7c20 5b7b 2773  mpany2    | [{'s
+000046d0: 6571 4e75 6d62 6572 273a 2031 2c20 2769  eqNumber': 1, 'i
+000046e0: 7341 7574 6f50 6466 273a 2046 616c 7365  sAutoPdf': False
+000046f0: 2c20 2769 6427 3a20 3331 3937 3738 322c  , 'id': 3197782,
+00004700: 2027 6e61 6d65 273a 2027 4f70 6572 6174   'name': 'Operat
+00004710: 696e 6720 436f 6d70 616e 7927 2c20 2765  ing Company', 'e
+00004720: 6e74 7279 4c69 7374 4964 273a 202d 367d  ntryListId': -6}
+00004730: 5d20 207c 0d0a 7c20 3132 3334 3720 2020  ]  |..| 12347   
+00004740: 7c20 436f 6d70 616e 7933 2020 2020 7c20  | Company3    | 
+00004750: 5b7b 2773 6571 4e75 6d62 6572 273a 2033  [{'seqNumber': 3
+00004760: 2c20 2769 7341 7574 6f50 6466 273a 2046  , 'isAutoPdf': F
+00004770: 616c 7365 2c20 2769 6427 3a20 3331 3937  alse, 'id': 3197
+00004780: 3738 302c 2027 6e61 6d65 273a 2027 4c69  780, 'name': 'Li
+00004790: 6d69 7465 6420 5061 7274 6e65 7227 2c20  mited Partner', 
+000047a0: 2765 6e74 7279 4c69 7374 4964 273a 202d  'entryListId': -
+000047b0: 367d 5d20 2020 207c 0d0a 0d0a 2323 2323  6}]    |....####
+000047c0: 2320 5573 696e 6720 6120 4669 6c74 6572  # Using a Filter
+000047d0: 2057 6865 6e20 5265 6164 696e 6720 5669   When Reading Vi
+000047e0: 6577 2044 6174 610d 0a57 6865 6e20 7265  ew Data..When re
+000047f0: 6164 696e 6720 6461 7461 2066 726f 6d20  ading data from 
+00004800: 6120 7669 6577 2c20 7768 6963 6820 6861  a view, which ha
+00004810: 7320 2253 7570 706c 7920 5661 6c75 6520  s "Supply Value 
+00004820: 4c61 7465 7222 2066 696c 7465 7273 2063  Later" filters c
+00004830: 6f6e 6669 6775 7265 642c 2074 6865 2066  onfigured, the f
+00004840: 696c 7465 7220 7661 6c75 6573 2063 616e  ilter values can
+00004850: 2062 6520 7072 6f76 6964 6564 2062 7920   be provided by 
+00004860: 7061 7373 696e 6720 7468 656d 2074 6f20  passing them to 
+00004870: 7468 6520 6076 6965 775f 6669 6c74 6572  the `view_filter
+00004880: 6020 6172 6775 6d65 6e74 2069 6e20 6120  ` argument in a 
+00004890: 606c 6973 7460 206f 6620 6064 6963 7460  `list` of `dict`
+000048a0: 732e 2046 6f72 206d 6f72 6520 696e 666f  s. For more info
+000048b0: 726d 6174 696f 6e20 6f6e 2074 6865 6972  rmation on their
+000048c0: 2066 6f72 6d61 742c 2070 6c65 6173 6520   format, please 
+000048d0: 7365 6520 7468 6520 5b41 5049 2044 6f63  see the [API Doc
+000048e0: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
+000048f0: 733a 2f2f 6170 692e 646f 6373 2e64 6561  s://api.docs.dea
+00004900: 6c63 6c6f 7564 2e63 6f6d 2f64 6f63 732f  lcloud.com/docs/
+00004910: 6461 7461 2f72 6f77 732f 7669 6577 5f64  data/rows/view_d
+00004920: 6574 6169 6c73 292e 0d0a 0d0a 466f 7220  etails).....For 
+00004930: 4578 616d 706c 652c 2073 7570 706c 7969  Example, supplyi
+00004940: 6e67 2061 2022 436f 6d70 616e 7954 7970  ng a "CompanyTyp
+00004950: 6522 2066 696c 7465 7220 7661 6c75 6520  e" filter value 
+00004960: 746f 2066 696c 7465 7220 666f 7220 6f6e  to filter for on
+00004970: 6c79 2022 4c69 6d69 7465 6420 5061 7274  ly "Limited Part
+00004980: 6e65 7222 2063 6f6d 7061 6e69 6573 3a0d  ner" companies:.
+00004990: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
+000049a0: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
+000049b0: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
+000049c0: 640d 0a0d 0a64 6320 3d20 4465 616c 436c  d....dc = DealCl
+000049d0: 6f75 642e 6672 6f6d 5f79 616d 6c28 2270  oud.from_yaml("p
+000049e0: 6174 682f 746f 2f79 616d 6c5f 636f 6e66  ath/to/yaml_conf
+000049f0: 6967 5f66 696c 652e 6a73 6f6e 2229 0d0a  ig_file.json")..
+00004a00: 0d0a 6461 7461 203d 2064 632e 7265 6164  ..data = dc.read
+00004a10: 5f64 6174 6128 0d0a 2020 2076 6965 775f  _data(..   view_
+00004a20: 6964 203d 2022 4d79 2043 6f6d 7061 6e79  id = "My Company
+00004a30: 2056 6965 7722 2c0d 0a20 2020 7669 6577   View",..   view
+00004a40: 5f66 696c 7465 7220 3d20 5b0d 0a20 2020  _filter = [..   
+00004a50: 2020 207b 0d0a 2020 2020 2020 2020 2022     {..         "
+00004a60: 636f 6c75 6d6e 223a 2243 6f6d 7061 6e79  column":"Company
+00004a70: 5479 7065 222c 0d0a 2020 2020 2020 2020  Type",..        
+00004a80: 2022 7661 6c75 6522 3a20 5b33 3139 3737   "value": [31977
+00004a90: 3830 5d0d 0a20 2020 2020 207d 0d0a 2020  80]..      }..  
+00004aa0: 205d 0d0a 290d 0a60 6060 0d0a 6064 6174   ]..)..```..`dat
+00004ab0: 6160 2077 696c 6c20 6265 2061 2060 7061  a` will be a `pa
+00004ac0: 6e64 6173 2e44 6174 6146 7261 6d65 6020  ndas.DataFrame` 
+00004ad0: 6173 2062 656c 6f77 3a0d 0a0d 0a7c 2045  as below:....| E
+00004ae0: 6e74 7279 4964 207c 2043 6f6d 7061 6e79  ntryId | Company
+00004af0: 4e61 6d65 207c 2043 6f6d 7061 6e79 5479  Name | CompanyTy
+00004b00: 7065 2020 2020 2020 2020 2020 2020 2020  pe              
+00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b50: 2020 2020 2020 2020 2020 2020 2020 7c0d                |.
+00004b60: 0a7c 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  .|---------|----
+00004b70: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
+00004b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004be0: 2d2d 7c0d 0a7c 2031 3233 3435 2020 207c  --|..| 12345   |
+00004bf0: 2043 6f6d 7061 6e79 3120 2020 207c 205b   Company1    | [
+00004c00: 7b27 7365 714e 756d 6265 7227 3a20 332c  {'seqNumber': 3,
+00004c10: 2027 6973 4175 746f 5064 6627 3a20 4661   'isAutoPdf': Fa
+00004c20: 6c73 652c 2027 6964 273a 2033 3139 3737  lse, 'id': 31977
+00004c30: 3830 2c20 276e 616d 6527 3a20 274c 696d  80, 'name': 'Lim
+00004c40: 6974 6564 2050 6172 746e 6572 272c 2027  ited Partner', '
+00004c50: 656e 7472 794c 6973 7449 6427 3a20 2d36  entryListId': -6
+00004c60: 7d5d 2020 2020 7c0d 0a7c 2031 3233 3437  }]    |..| 12347
+00004c70: 2020 207c 2043 6f6d 7061 6e79 3320 2020     | Company3   
+00004c80: 207c 205b 7b27 7365 714e 756d 6265 7227   | [{'seqNumber'
+00004c90: 3a20 332c 2027 6973 4175 746f 5064 6627  : 3, 'isAutoPdf'
+00004ca0: 3a20 4661 6c73 652c 2027 6964 273a 2033  : False, 'id': 3
+00004cb0: 3139 3737 3830 2c20 276e 616d 6527 3a20  197780, 'name': 
+00004cc0: 274c 696d 6974 6564 2050 6172 746e 6572  'Limited Partner
+00004cd0: 272c 2027 656e 7472 794c 6973 7449 6427  ', 'entryListId'
+00004ce0: 3a20 2d36 7d5d 2020 2020 7c0d 0a0d 0a0d  : -6}]    |.....
+00004cf0: 0a23 2323 2043 7265 6174 652c 2055 7064  .### Create, Upd
+00004d00: 6174 6520 616e 6420 5570 7365 7274 2044  ate and Upsert D
+00004d10: 6174 610d 0a60 4465 616c 436c 6f75 642e  ata..`DealCloud.
+00004d20: 696e 7365 7274 5f64 6174 6128 2960 2c20  insert_data()`, 
+00004d30: 6044 6561 6c43 6c6f 7564 2e75 7064 6174  `DealCloud.updat
+00004d40: 655f 6461 7461 2829 602c 2060 4465 616c  e_data()`, `Deal
+00004d50: 436c 6f75 642e 7570 7365 7274 5f64 6174  Cloud.upsert_dat
+00004d60: 6128 2960 2061 7265 206d 6574 686f 6473  a()` are methods
+00004d70: 2077 6869 6368 2070 726f 7669 6465 2074   which provide t
+00004d80: 6865 2061 6269 6c69 7479 2074 6f20 6372  he ability to cr
+00004d90: 6561 7465 2c20 7570 6461 7465 2061 6e64  eate, update and
+00004da0: 2075 7073 6572 7420 6461 7461 2072 6573   upsert data res
+00004db0: 7065 6374 6976 656c 792e 0d0a 5468 6573  pectively...Thes
+00004dc0: 6520 6d65 7468 6f64 7320 6861 7665 2074  e methods have t
+00004dd0: 6865 2073 616d 6520 6172 6775 6d65 6e74  he same argument
+00004de0: 2070 6174 7465 726e 3a0d 0a0d 0a41 7267   pattern:....Arg
+00004df0: 756d 656e 7473 3a0d 0a2d 206f 626a 6563  uments:..- objec
+00004e00: 745f 6170 695f 6e61 6d65 2060 7374 7260  t_api_name `str`
+00004e10: 3a20 7468 6520 6f62 6a65 6374 2041 5049  : the object API
+00004e20: 206e 616d 6520 746f 2077 7269 7465 2064   name to write d
+00004e30: 6174 6120 746f 0d0a 2d20 6461 7461 2060  ata to..- data `
+00004e40: 556e 696f 6e5b 6c69 7374 5b64 6963 745d  Union[list[dict]
+00004e50: 2c20 7064 2e44 6174 6146 7261 6d65 5d60  , pd.DataFrame]`
+00004e60: 3a20 7468 6520 6461 7461 2074 6f20 6265  : the data to be
+00004e70: 2073 656e 7420 746f 2044 6561 6c43 6c6f   sent to DealClo
+00004e80: 7564 2e0d 0a2d 2075 7365 5f64 6561 6c63  ud...- use_dealc
+00004e90: 6c6f 7564 5f69 6473 2060 626f 6f6c 603a  loud_ids `bool`:
+00004ea0: 2044 6566 6175 6c74 2069 7320 6054 7275   Default is `Tru
+00004eb0: 6560 2049 6620 6054 7275 6560 2c20 4465  e` If `True`, De
+00004ec0: 616c 436c 6f75 6420 456e 7472 7949 6473  alCloud EntryIds
+00004ed0: 206d 7573 7420 6265 2075 7365 6420 746f   must be used to
+00004ee0: 2072 6566 6572 656e 6365 2072 6563 6f72   reference recor
+00004ef0: 6473 2061 6e64 2063 686f 6963 6520 7661  ds and choice va
+00004f00: 6c75 6573 2e20 4966 2060 4661 6c73 6560  lues. If `False`
+00004f10: 2c20 7573 6520 6120 636f 6c75 6d6e 2061  , use a column a
+00004f20: 7320 6120 6c6f 6f6b 7570 2c20 6465 6669  s a lookup, defi
+00004f30: 6e65 6420 6279 2074 6865 206c 6f6f 6b75  ned by the looku
+00004f40: 705f 636f 6c75 6d6e 2061 7267 756d 656e  p_column argumen
+00004f50: 742e 0d0a 2d20 6c6f 6f6b 7570 5f63 6f6c  t...- lookup_col
+00004f60: 756d 6e20 6073 7472 603a 2069 6620 6075  umn `str`: if `u
+00004f70: 7365 5f64 6561 6c63 6c6f 7564 5f69 6473  se_dealcloud_ids
+00004f80: 6020 6973 2060 4661 6c73 6560 2c20 7468  ` is `False`, th
+00004f90: 6973 2064 6566 696e 6573 2074 6865 2063  is defines the c
+00004fa0: 6f6c 756d 6e20 746f 2062 6520 7573 6564  olumn to be used
+00004fb0: 2061 7320 6120 6c6f 6f6b 7570 2e0d 0a2d   as a lookup...-
+00004fc0: 206f 7574 7075 7460 7374 7260 3a20 606c   output`str`: `l
+00004fd0: 6973 7460 206f 7220 6070 616e 6461 7360  ist` or `pandas`
+00004fe0: 2c20 6465 6669 6e65 7320 7468 6520 6f75  , defines the ou
+00004ff0: 7470 7574 2066 6f72 6d61 7420 7265 7475  tput format retu
+00005000: 726e 6564 2066 726f 6d20 7468 6520 6675  rned from the fu
+00005010: 6e63 7469 6f6e 0d0a 0d0a 5265 7475 726e  nction....Return
+00005020: 733a 0d0a 2020 2060 556e 696f 6e5b 6c69  s:..   `Union[li
+00005030: 7374 5b64 6963 745d 2c20 7064 2e44 6174  st[dict], pd.Dat
+00005040: 6146 7261 6d65 5d60 3a20 7468 6520 6461  aFrame]`: the da
+00005050: 7461 2072 6574 7572 6e65 6420 6672 6f6d  ta returned from
+00005060: 2074 6865 2064 6174 6120 6f70 6572 6174   the data operat
+00005070: 696f 6e2e 0d0a 0d0a 3e20 5b21 494d 504f  ion.....> [!IMPO
+00005080: 5254 414e 545d 0d0a 3e20 5768 656e 206e  RTANT]..> When n
+00005090: 6f74 2075 7369 6e67 2060 7573 655f 6465  ot using `use_de
+000050a0: 616c 636c 6f75 645f 6964 7360 2c20 666f  alcloud_ids`, fo
+000050b0: 7220 5265 6665 7265 6e63 6520 6669 656c  r Reference fiel
+000050c0: 6473 2c20 7265 6665 7265 6e63 6520 6279  ds, reference by
+000050d0: 2072 6563 6f72 6420 456e 7472 7949 642e   record EntryId.
+000050e0: 2046 6f72 2063 686f 6963 6520 6669 656c   For choice fiel
+000050f0: 6473 2c20 7573 6520 7468 6520 6368 6f69  ds, use the choi
+00005100: 6365 2076 616c 7565 2049 442e 2046 6f72  ce value ID. For
+00005110: 2075 7365 7220 6669 656c 6473 2c20 7573   user fields, us
+00005120: 6520 7468 6520 7573 6572 2049 4420 2866  e the user ID (f
+00005130: 726f 6d20 6044 6561 6c43 6c6f 7564 2e67  rom `DealCloud.g
+00005140: 6574 5f75 7365 7273 2829 6029 2e20 0d0a  et_users()`). ..
+00005150: 3e20 5768 656e 2075 7369 6e67 2060 7573  > When using `us
+00005160: 655f 6465 616c 636c 6f75 645f 6964 7360  e_dealcloud_ids`
+00005170: 2c20 666f 7220 5265 6665 7265 6e63 6520  , for Reference 
+00005180: 6669 656c 6473 2c20 7265 6665 7265 6e63  fields, referenc
+00005190: 6520 6279 2074 6865 206c 6f6f 6b75 7020  e by the lookup 
+000051a0: 636f 6c75 6d6e 206f 6e20 7468 6520 7265  column on the re
+000051b0: 6665 7265 6e63 6564 206f 626a 6563 742e  ferenced object.
+000051c0: 2046 6f72 2063 686f 6963 6520 6669 656c   For choice fiel
+000051d0: 6473 2c20 7573 6520 7468 6520 6368 6f69  ds, use the choi
+000051e0: 6365 2066 6965 6c64 2064 6973 706c 6179  ce field display
+000051f0: 206e 616d 652e 2046 6f72 2075 7365 7220   name. For user 
+00005200: 6669 656c 6473 2c20 7573 6520 7468 6520  fields, use the 
+00005210: 7573 6572 2065 6d61 696c 2061 6464 7265  user email addre
+00005220: 7373 2e0d 0a0d 0a23 2323 2323 2046 6965  ss.....##### Fie
+00005230: 6c64 204d 6170 7069 6e67 0d0a 416c 6c20  ld Mapping..All 
+00005240: 636f 6c75 6d6e 7320 7061 7373 6564 2074  columns passed t
+00005250: 6f20 7468 6520 6372 6561 7465 2c20 7570  o the create, up
+00005260: 6461 7465 2061 6e64 2075 7073 6572 7420  date and upsert 
+00005270: 6d65 7468 6f64 7320 6d75 7374 206d 6174  methods must mat
+00005280: 6368 2062 7920 5f41 5049 204e 616d 655f  ch by _API Name_
+00005290: 2e20 4966 2061 2063 6f6c 756d 6e20 7061  . If a column pa
+000052a0: 7373 6564 2074 6f20 7468 6520 6d65 7468  ssed to the meth
+000052b0: 6f64 2064 6f65 7320 6e6f 7420 6578 6973  od does not exis
+000052c0: 7420 696e 2074 6865 2073 6974 6520 6279  t in the site by
+000052d0: 2041 5049 206e 616d 652c 2074 6865 6e20   API name, then 
+000052e0: 6120 604b 6579 4572 726f 7260 2077 696c  a `KeyError` wil
+000052f0: 6c20 6265 2072 6169 7365 643a 0d0a 0d0a  l be raised:....
+00005300: 6060 6070 7974 686f 6e0d 0a66 726f 6d20  ```python..from 
+00005310: 6465 616c 636c 6f75 645f 7364 6b20 696d  dealcloud_sdk im
+00005320: 706f 7274 2044 6561 6c43 6c6f 7564 0d0a  port DealCloud..
+00005330: 0d0a 6463 203d 2044 6561 6c43 6c6f 7564  ..dc = DealCloud
+00005340: 2e66 726f 6d5f 7961 6d6c 2822 7061 7468  .from_yaml("path
+00005350: 2f74 6f2f 7961 6d6c 5f63 6f6e 6669 675f  /to/yaml_config_
+00005360: 6669 6c65 2e6a 736f 6e22 290d 0a0d 0a74  file.json")....t
+00005370: 6f5f 7365 6e64 203d 205b 0d0a 2020 7b0d  o_send = [..  {.
+00005380: 0a20 2020 2020 2022 436f 6d70 616e 794e  .      "CompanyN
+00005390: 616d 6522 3a20 2254 6573 7420 436f 6d70  ame": "Test Comp
+000053a0: 616e 7920 3122 2c0d 0a20 2020 2020 2022  any 1",..      "
+000053b0: 556e 6d61 7070 6162 6c65 436f 6c75 6d6e  UnmappableColumn
+000053c0: 223a 2022 466f 6f22 2c0d 0a20 207d 0d0a  ": "Foo",..  }..
+000053d0: 5d0d 0a72 6573 706f 6e73 6573 203d 2064  ]..responses = d
+000053e0: 632e 696e 7365 7274 5f64 6174 6128 2243  c.insert_data("C
+000053f0: 6f6d 7061 6e79 222c 2074 6f5f 7365 6e64  ompany", to_send
+00005400: 290d 0a60 6060 0d0a 5769 6c6c 2052 6574  )..```..Will Ret
+00005410: 7572 6e0d 0a60 6060 6261 7368 0d0a 5472  urn..```bash..Tr
+00005420: 6163 6562 6163 6b2e 2e2e 0d0a 4b65 7945  aceback.....KeyE
+00005430: 7272 6f72 3a20 226d 6170 7069 6e67 2065  rror: "mapping e
+00005440: 7272 6f72 2c20 636f 756c 6420 6e6f 7420  rror, could not 
+00005450: 6d61 703a 205b 2755 6e6d 6170 7061 626c  map: ['Unmappabl
+00005460: 6543 6f6c 756d 6e27 5d22 0d0a 6060 600d  eColumn']"..```.
+00005470: 0a0d 0a23 2323 2320 4372 6561 7465 2044  ...#### Create D
+00005480: 6174 610d 0a45 7861 6d70 6c65 2c20 746f  ata..Example, to
+00005490: 2069 6e73 6572 7420 6461 7461 2069 6e74   insert data int
+000054a0: 6f20 7468 6520 2243 6f6d 7061 6e79 2220  o the "Company" 
+000054b0: 6f62 6a65 6374 2066 726f 6d20 6120 6c69  object from a li
+000054c0: 7374 3a0d 0a0d 0a60 6060 7079 7468 6f6e  st:....```python
+000054d0: 0d0a 6672 6f6d 2064 6561 6c63 6c6f 7564  ..from dealcloud
+000054e0: 5f73 646b 2069 6d70 6f72 7420 4465 616c  _sdk import Deal
+000054f0: 436c 6f75 640d 0a0d 0a64 6320 3d20 4465  Cloud....dc = De
+00005500: 616c 436c 6f75 642e 6672 6f6d 5f79 616d  alCloud.from_yam
+00005510: 6c28 2270 6174 682f 746f 2f79 616d 6c5f  l("path/to/yaml_
+00005520: 636f 6e66 6967 5f66 696c 652e 6a73 6f6e  config_file.json
+00005530: 2229 0d0a 0d0a 746f 5f73 656e 6420 3d20  ")....to_send = 
+00005540: 5b0d 0a20 207b 0d0a 2020 2020 2020 2243  [..  {..      "C
+00005550: 6f6d 7061 6e79 4e61 6d65 223a 2022 5465  ompanyName": "Te
+00005560: 7374 2043 6f6d 7061 6e79 2031 222c 0d0a  st Company 1",..
+00005570: 2020 2020 2020 2243 6f6d 7061 6e79 5479        "CompanyTy
+00005580: 7065 223a 2031 3233 3435 2c0d 0a20 2020  pe": 12345,..   
+00005590: 2020 2022 4275 7369 6e65 7373 4465 7363     "BusinessDesc
+000055a0: 7269 7074 696f 6e22 3a20 2248 6572 6520  ription": "Here 
+000055b0: 6973 2061 2062 7573 696e 6573 7320 6465  is a business de
+000055c0: 7363 7269 7074 696f 6e22 2c0d 0a20 2020  scription",..   
+000055d0: 2020 2022 5365 6374 6f72 223a 2031 3433     "Sector": 143
+000055e0: 3231 2c0d 0a20 207d 0d0a 5d0d 0a72 6573  21,..  }..]..res
+000055f0: 706f 6e73 6573 203d 2064 632e 696e 7365  ponses = dc.inse
+00005600: 7274 5f64 6174 6128 2243 6f6d 7061 6e79  rt_data("Company
+00005610: 222c 2074 6f5f 7365 6e64 290d 0a60 6060  ", to_send)..```
+00005620: 0d0a 4966 2073 7563 6365 7373 6675 6c2c  ..If successful,
+00005630: 2060 7265 7370 6f6e 7365 7360 2077 696c   `responses` wil
+00005640: 6c20 636f 6e74 6169 6e20 7468 6520 6265  l contain the be
+00005650: 6c6f 7720 2d20 6e6f 7465 2074 6861 7420  low - note that 
+00005660: 6045 6e74 7279 4964 6020 6973 206e 6f77  `EntryId` is now
+00005670: 2069 6e63 6c75 6465 643a 0d0a 6060 6070   included:..```p
+00005680: 7974 686f 6e0d 0a5b 0d0a 2020 2020 7b0d  ython..[..    {.
+00005690: 0a20 2020 2020 2020 2022 456e 7472 7949  .        "EntryI
+000056a0: 6422 3a20 3233 3435 3637 2c0d 0a20 2020  d": 234567,..   
+000056b0: 2020 2020 2022 436f 6d70 616e 794e 616d       "CompanyNam
+000056c0: 6522 3a20 2254 6573 7420 436f 6d70 616e  e": "Test Compan
+000056d0: 7920 3122 2c0d 0a20 2020 2020 2020 2022  y 1",..        "
+000056e0: 436f 6d70 616e 7954 7970 6522 3a20 3132  CompanyType": 12
+000056f0: 3334 352c 0d0a 2020 2020 2020 2020 2242  345,..        "B
+00005700: 7573 696e 6573 7344 6573 6372 6970 7469  usinessDescripti
+00005710: 6f6e 223a 2022 4865 7265 2069 7320 6120  on": "Here is a 
+00005720: 6275 7369 6e65 7373 2064 6573 6372 6970  business descrip
+00005730: 7469 6f6e 222c 0d0a 2020 2020 2020 2020  tion",..        
+00005740: 2253 6563 746f 7222 3a20 3134 3332 312c  "Sector": 14321,
+00005750: 0d0a 2020 2020 7d0d 0a5d 0d0a 6060 600d  ..    }..]..```.
+00005760: 0a45 7861 6d70 6c65 2c20 746f 2069 6e73  .Example, to ins
+00005770: 6572 7420 6461 7461 2069 6e74 6f20 7468  ert data into th
+00005780: 6520 2243 6f6d 7061 6e79 2220 6f62 6a65  e "Company" obje
+00005790: 6374 2066 726f 6d20 6120 4353 562c 2075  ct from a CSV, u
+000057a0: 7369 6e67 2060 7061 6e64 6173 603a 0d0a  sing `pandas`:..
+000057b0: 0d0a 4353 5620 4669 6c65 2028 6063 6f6d  ..CSV File (`com
+000057c0: 7061 6e79 2e63 7376 6029 3a0d 0a0d 0a7c  pany.csv`):....|
+000057d0: 2043 6f6d 7061 6e79 4e61 6d65 207c 2043   CompanyName | C
+000057e0: 6f6d 7061 6e79 5479 7065 207c 0d0a 7c2d  ompanyType |..|-
+000057f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ------------|---
+00005800: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0d 0a7c 2043  ----------|..| C
+00005810: 6f6d 7061 6e79 3120 2020 207c 2033 3139  ompany1    | 319
+00005820: 3737 3830 2020 2020 207c 0d0a 7c20 436f  7780     |..| Co
+00005830: 6d70 616e 7932 2020 2020 7c20 3331 3937  mpany2    | 3197
+00005840: 3738 3220 2020 2020 7c0d 0a7c 2043 6f6d  782     |..| Com
+00005850: 7061 6e79 3320 2020 207c 2033 3139 3737  pany3    | 31977
+00005860: 3830 2020 2020 207c 0d0a 0d0a 6060 6070  80     |....```p
+00005870: 7974 686f 6e0d 0a69 6d70 6f72 7420 7061  ython..import pa
+00005880: 6e64 6173 2061 7320 7064 0d0a 6672 6f6d  ndas as pd..from
+00005890: 2064 6561 6c63 6c6f 7564 5f73 646b 2069   dealcloud_sdk i
+000058a0: 6d70 6f72 7420 4465 616c 436c 6f75 640d  mport DealCloud.
+000058b0: 0a0d 0a64 6320 3d20 4465 616c 436c 6f75  ...dc = DealClou
+000058c0: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
+000058d0: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
+000058e0: 5f66 696c 652e 6a73 6f6e 2229 0d0a 0d0a  _file.json")....
+000058f0: 746f 5f73 656e 6420 3d20 7064 2e72 6561  to_send = pd.rea
+00005900: 645f 6373 7628 2263 6f6d 7061 6e79 2e63  d_csv("company.c
+00005910: 7376 2229 0d0a 7265 7370 6f6e 7365 7320  sv")..responses 
+00005920: 3d20 6463 2e69 6e73 6572 745f 6461 7461  = dc.insert_data
+00005930: 2822 436f 6d70 616e 7922 2c20 746f 5f73  ("Company", to_s
+00005940: 656e 6429 0d0a 6060 600d 0a45 7861 6d70  end)..```..Examp
+00005950: 6c65 2c20 746f 2069 6e73 6572 7420 6461  le, to insert da
+00005960: 7461 2069 6e74 6f20 7468 6520 2243 6f6d  ta into the "Com
+00005970: 7061 6e79 2220 6f62 6a65 6374 2075 7369  pany" object usi
+00005980: 6e67 2022 4578 7465 726e 616c 5379 7374  ng "ExternalSyst
+00005990: 656d 4944 2220 6173 2061 206c 6f6f 6b75  emID" as a looku
+000059a0: 7020 636f 6c75 6d6e 3a0d 0a0d 0a60 6060  p column:....```
+000059b0: 7079 7468 6f6e 0d0a 6672 6f6d 2064 6561  python..from dea
+000059c0: 6c63 6c6f 7564 5f73 646b 2069 6d70 6f72  lcloud_sdk impor
+000059d0: 7420 4465 616c 436c 6f75 640d 0a0d 0a64  t DealCloud....d
+000059e0: 6320 3d20 4465 616c 436c 6f75 642e 6672  c = DealCloud.fr
+000059f0: 6f6d 5f79 616d 6c28 2270 6174 682f 746f  om_yaml("path/to
+00005a00: 2f79 616d 6c5f 636f 6e66 6967 5f66 696c  /yaml_config_fil
+00005a10: 652e 6a73 6f6e 2229 0d0a 0d0a 746f 5f73  e.json")....to_s
+00005a20: 656e 6420 3d20 5b0d 0a20 207b 0d0a 2020  end = [..  {..  
+00005a30: 2020 2020 2243 6f6d 7061 6e79 4e61 6d65      "CompanyName
+00005a40: 223a 2022 5465 7374 2043 6f6d 7061 6e79  ": "Test Company
+00005a50: 2031 222c 0d0a 2020 2020 2020 2243 6f6d   1",..      "Com
+00005a60: 7061 6e79 5479 7065 223a 2022 4f70 6572  panyType": "Oper
+00005a70: 6174 696e 6720 436f 6d70 616e 7922 2c0d  ating Company",.
+00005a80: 0a20 2020 2020 2022 4275 7369 6e65 7373  .      "Business
+00005a90: 4465 7363 7269 7074 696f 6e22 3a20 2248  Description": "H
+00005aa0: 6572 6520 6973 2061 2062 7573 696e 6573  ere is a busines
+00005ab0: 7320 6465 7363 7269 7074 696f 6e22 2c0d  s description",.
+00005ac0: 0a20 2020 2020 2022 5365 6374 6f72 223a  .      "Sector":
+00005ad0: 2022 3631 3245 3946 4634 2d31 4438 432d   "612E9FF4-1D8C-
+00005ae0: 3431 4237 2d42 3845 442d 3244 3143 3135  41B7-B8ED-2D1C15
+00005af0: 3234 3034 3334 222c 0d0a 2020 7d0d 0a5d  240434",..  }..]
+00005b00: 0d0a 0d0a 7265 7370 6f6e 7365 7320 3d20  ....responses = 
+00005b10: 6463 2e69 6e73 6572 745f 6461 7461 280d  dc.insert_data(.
+00005b20: 0a20 2020 6f62 6a65 6374 5f61 7069 5f6e  .   object_api_n
+00005b30: 616d 6520 3d20 2243 6f6d 7061 6e79 222c  ame = "Company",
+00005b40: 0d0a 2020 2064 6174 6120 3d20 746f 5f73  ..   data = to_s
+00005b50: 656e 642c 0d0a 2020 2075 7365 5f64 6561  end,..   use_dea
+00005b60: 6c63 6c6f 7564 5f69 6473 203d 2046 616c  lcloud_ids = Fal
+00005b70: 7365 2c0d 0a20 2020 6c6f 6f6b 7570 5f63  se,..   lookup_c
+00005b80: 6f6c 756d 6e20 3d20 2245 7874 6572 6e61  olumn = "Externa
+00005b90: 6c53 7973 7465 6d49 4422 0d0a 290d 0a60  lSystemID"..)..`
+00005ba0: 6060 0d0a 2323 2323 2055 7064 6174 6520  ``..#### Update 
+00005bb0: 4461 7461 0d0a 546f 2075 7064 6174 6520  Data..To update 
+00005bc0: 6578 6973 7469 6e67 2073 6974 6520 6461  existing site da
+00005bd0: 7461 2c20 7468 6520 7072 6f63 6573 7320  ta, the process 
+00005be0: 6973 2073 696d 696c 6172 2c20 6578 6365  is similar, exce
+00005bf0: 7074 206f 626a 6563 7473 206d 7573 7420  pt objects must 
+00005c00: 696e 636c 7564 6520 6045 6e74 7279 4964  include `EntryId
+00005c10: 602c 206f 7220 6120 7661 6c69 6420 7072  `, or a valid pr
+00005c20: 696d 6172 7920 6b65 7920 6279 2060 6c6f  imary key by `lo
+00005c30: 6f6b 7570 5f63 6f6c 756d 6e60 2e0d 0a0d  okup_column`....
+00005c40: 0a45 7861 6d70 6c65 2c20 746f 2075 7064  .Example, to upd
+00005c50: 6174 6520 6461 7461 2069 6e20 7468 6520  ate data in the 
+00005c60: 2243 6f6d 7061 6e79 2220 6f62 6a65 6374  "Company" object
+00005c70: 2066 726f 6d20 6120 6c69 7374 3a0d 0a0d   from a list:...
+00005c80: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
+00005c90: 2064 6561 6c63 6c6f 7564 5f73 646b 2069   dealcloud_sdk i
+00005ca0: 6d70 6f72 7420 4465 616c 436c 6f75 640d  mport DealCloud.
+00005cb0: 0a0d 0a64 6320 3d20 4465 616c 436c 6f75  ...dc = DealClou
+00005cc0: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
+00005cd0: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
+00005ce0: 5f66 696c 652e 6a73 6f6e 2229 0d0a 0d0a  _file.json")....
+00005cf0: 746f 5f73 656e 6420 3d20 5b0d 0a20 207b  to_send = [..  {
+00005d00: 0d0a 2020 2020 2020 2245 6e74 7279 4964  ..      "EntryId
+00005d10: 223a 2032 3334 3536 372c 0d0a 2020 2020  ": 234567,..    
+00005d20: 2020 2242 7573 696e 6573 7344 6573 6372    "BusinessDescr
+00005d30: 6970 7469 6f6e 223a 2022 4865 7265 2069  iption": "Here i
+00005d40: 7320 616e 2075 7064 6174 6564 2062 7573  s an updated bus
+00005d50: 696e 6573 7320 6465 7363 7269 7074 696f  iness descriptio
+00005d60: 6e21 222c 0d0a 2020 7d0d 0a5d 0d0a 7265  n!",..  }..]..re
+00005d70: 7370 6f6e 7365 7320 3d20 6463 2e69 6e73  sponses = dc.ins
+00005d80: 6572 745f 6461 7461 2822 436f 6d70 616e  ert_data("Compan
+00005d90: 7922 2c20 746f 5f73 656e 6429 0d0a 6060  y", to_send)..``
+00005da0: 600d 0a49 6620 7375 6363 6573 7366 756c  `..If successful
+00005db0: 2c20 6072 6573 706f 6e73 6573 6020 7769  , `responses` wi
+00005dc0: 6c6c 2063 6f6e 7461 696e 2074 6865 2062  ll contain the b
+00005dd0: 656c 6f77 3a0d 0a60 6060 7079 7468 6f6e  elow:..```python
+00005de0: 0d0a 5b0d 0a20 2020 207b 0d0a 2020 2020  ..[..    {..    
+00005df0: 2020 2020 2245 6e74 7279 4964 223a 2032      "EntryId": 2
+00005e00: 3334 3536 372c 0d0a 2020 2020 2020 2020  34567,..        
+00005e10: 2243 6f6d 7061 6e79 4e61 6d65 223a 2022  "CompanyName": "
+00005e20: 5465 7374 2043 6f6d 7061 6e79 2031 222c  Test Company 1",
+00005e30: 0d0a 2020 2020 2020 2020 2243 6f6d 7061  ..        "Compa
+00005e40: 6e79 5479 7065 223a 2031 3233 3435 2c0d  nyType": 12345,.
+00005e50: 0a20 2020 2020 2020 2022 4275 7369 6e65  .        "Busine
+00005e60: 7373 4465 7363 7269 7074 696f 6e22 3a20  ssDescription": 
+00005e70: 2248 6572 6520 6973 2061 6e20 7570 6461  "Here is an upda
+00005e80: 7465 6420 6275 7369 6e65 7373 2064 6573  ted business des
+00005e90: 6372 6970 7469 6f6e 2122 2c0d 0a20 2020  cription!",..   
+00005ea0: 2020 2020 2022 5365 6374 6f72 223a 2031       "Sector": 1
+00005eb0: 3433 3231 2c0d 0a20 2020 207d 0d0a 5d0d  4321,..    }..].
+00005ec0: 0a60 6060 0d0a 4578 616d 706c 652c 2074  .```..Example, t
+00005ed0: 6f20 7570 6461 7465 2064 6174 6120 696e  o update data in
+00005ee0: 2074 6865 2022 436f 6d70 616e 7922 206f   the "Company" o
+00005ef0: 626a 6563 7420 6672 6f6d 2061 206c 6973  bject from a lis
+00005f00: 742c 2075 7369 6e67 2074 6865 2060 6c6f  t, using the `lo
+00005f10: 6f6b 7570 5f63 6f6c 756d 6e60 2c20 6045  okup_column`, `E
+00005f20: 7874 6572 6e61 6c53 7973 7465 6d49 6460  xternalSystemId`
+00005f30: 3a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  :....```python..
+00005f40: 6672 6f6d 2064 6561 6c63 6c6f 7564 5f73  from dealcloud_s
+00005f50: 646b 2069 6d70 6f72 7420 4465 616c 436c  dk import DealCl
+00005f60: 6f75 640d 0a0d 0a64 6320 3d20 4465 616c  oud....dc = Deal
+00005f70: 436c 6f75 642e 6672 6f6d 5f79 616d 6c28  Cloud.from_yaml(
+00005f80: 2270 6174 682f 746f 2f79 616d 6c5f 636f  "path/to/yaml_co
+00005f90: 6e66 6967 5f66 696c 652e 6a73 6f6e 2229  nfig_file.json")
+00005fa0: 0d0a 0d0a 746f 5f73 656e 6420 3d20 5b0d  ....to_send = [.
+00005fb0: 0a20 207b 0d0a 2020 2020 2020 2245 7874  .  {..      "Ext
+00005fc0: 6572 6e61 6c53 7973 7465 6d49 6422 3a20  ernalSystemId": 
+00005fd0: 2246 3632 3841 4643 382d 3533 3243 2d34  "F628AFC8-532C-4
+00005fe0: 3036 432d 4244 4536 2d41 3738 3246 3033  06C-BDE6-A782F03
+00005ff0: 3530 3844 3522 2c0d 0a20 2020 2020 2022  508D5",..      "
+00006000: 4275 7369 6e65 7373 4465 7363 7269 7074  BusinessDescript
+00006010: 696f 6e22 3a20 2248 6572 6520 6973 2061  ion": "Here is a
+00006020: 6e20 7570 6461 7465 6420 6275 7369 6e65  n updated busine
+00006030: 7373 2064 6573 6372 6970 7469 6f6e 2122  ss description!"
+00006040: 2c0d 0a20 207d 0d0a 5d0d 0a72 6573 706f  ,..  }..]..respo
+00006050: 6e73 6573 203d 2064 632e 696e 7365 7274  nses = dc.insert
+00006060: 5f64 6174 6128 0d0a 2020 206f 626a 6563  _data(..   objec
+00006070: 745f 6170 695f 6e61 6d65 203d 2022 436f  t_api_name = "Co
+00006080: 6d70 616e 7922 2c0d 0a20 2020 6461 7461  mpany",..   data
+00006090: 203d 2074 6f5f 7365 6e64 2c0d 0a20 2020   = to_send,..   
+000060a0: 7573 655f 6465 616c 636c 6f75 645f 6964  use_dealcloud_id
+000060b0: 7320 3d20 4661 6c73 652c 0d0a 2020 206c  s = False,..   l
+000060c0: 6f6f 6b75 705f 636f 6c75 6d6e 203d 2022  ookup_column = "
+000060d0: 4578 7465 726e 616c 5379 7374 656d 4964  ExternalSystemId
+000060e0: 220d 0a29 0d0a 6060 600d 0a0d 0a23 2323  "..)..```....###
+000060f0: 2320 5570 7365 7274 2044 6174 610d 0a55  # Upsert Data..U
+00006100: 7073 6572 7469 6e67 2064 6174 6120 6973  pserting data is
+00006110: 2061 206d 6574 686f 6420 7468 6174 2063   a method that c
+00006120: 6f6d 6269 6e65 7320 696e 7365 7274 2061  ombines insert a
+00006130: 6e64 2075 7064 6174 652e 2049 6620 6120  nd update. If a 
+00006140: 7265 636f 7264 2065 7869 7374 7320 616e  record exists an
+00006150: 6420 6361 6e20 6265 2066 6f75 6e64 2062  d can be found b
+00006160: 7920 6045 6e74 7279 4964 6020 6f72 2061  y `EntryId` or a
+00006170: 2060 6c6f 6f6b 7570 5f63 6f6c 756d 6e60   `lookup_column`
+00006180: 2074 6865 6e20 6974 2077 696c 6c20 6265   then it will be
+00006190: 2075 7064 6174 6564 2c20 6966 206e 6f74   updated, if not
+000061a0: 2c20 6974 2077 696c 6c20 6265 2063 7265  , it will be cre
+000061b0: 6174 6564 206e 6577 2e0d 0a0d 0a45 7861  ated new.....Exa
+000061c0: 6d70 6c65 2c20 746f 2075 7073 6572 7420  mple, to upsert 
+000061d0: 6461 7461 2069 6e20 7468 6520 2243 6f6d  data in the "Com
+000061e0: 7061 6e79 2220 6f62 6a65 6374 2066 726f  pany" object fro
+000061f0: 6d20 6120 6c69 7374 3a0d 0a0d 0a60 6060  m a list:....```
+00006200: 7079 7468 6f6e 0d0a 6672 6f6d 2064 6561  python..from dea
+00006210: 6c63 6c6f 7564 5f73 646b 2069 6d70 6f72  lcloud_sdk impor
+00006220: 7420 4465 616c 436c 6f75 640d 0a0d 0a64  t DealCloud....d
+00006230: 6320 3d20 4465 616c 436c 6f75 642e 6672  c = DealCloud.fr
+00006240: 6f6d 5f79 616d 6c28 2270 6174 682f 746f  om_yaml("path/to
+00006250: 2f79 616d 6c5f 636f 6e66 6967 5f66 696c  /yaml_config_fil
+00006260: 652e 6a73 6f6e 2229 0d0a 0d0a 746f 5f73  e.json")....to_s
+00006270: 656e 6420 3d20 5b0d 0a20 2020 7b0d 0a20  end = [..   {.. 
+00006280: 2020 2022 456e 7472 7949 6422 3a20 3233     "EntryId": 23
+00006290: 3435 3637 2c20 200d 0a20 2020 2022 436f  4567,  ..    "Co
+000062a0: 6d70 616e 794e 616d 6522 3a20 2254 6573  mpanyName": "Tes
+000062b0: 7420 436f 6d70 616e 7920 3122 2c0d 0a20  t Company 1",.. 
+000062c0: 2020 2022 436f 6d70 616e 7954 7970 6522     "CompanyType"
+000062d0: 3a20 3132 3334 352c 0d0a 2020 2020 2242  : 12345,..    "B
+000062e0: 7573 696e 6573 7344 6573 6372 6970 7469  usinessDescripti
+000062f0: 6f6e 223a 2022 4865 7265 2069 7320 616e  on": "Here is an
+00006300: 2075 7064 6174 6564 2062 7573 696e 6573   updated busines
+00006310: 7320 6465 7363 7269 7074 696f 6e22 2c0d  s description",.
+00006320: 0a20 2020 2022 5365 6374 6f72 223a 2031  .    "Sector": 1
+00006330: 3433 3231 2c0d 0a20 2020 7d2c 0d0a 2020  4321,..   },..  
+00006340: 207b 0d0a 2020 2020 2243 6f6d 7061 6e79   {..    "Company
+00006350: 4e61 6d65 223a 2022 5465 7374 2043 6f6d  Name": "Test Com
+00006360: 7061 6e79 2032 222c 0d0a 2020 2020 2243  pany 2",..    "C
+00006370: 6f6d 7061 6e79 5479 7065 223a 2031 3233  ompanyType": 123
+00006380: 3435 2c0d 0a20 2020 2022 4275 7369 6e65  45,..    "Busine
+00006390: 7373 4465 7363 7269 7074 696f 6e22 3a20  ssDescription": 
+000063a0: 2248 6572 6520 6973 2061 2062 7573 696e  "Here is a busin
+000063b0: 6573 7320 6465 7363 7269 7074 696f 6e20  ess description 
+000063c0: 666f 7220 6120 6e65 7720 636f 6d70 616e  for a new compan
+000063d0: 7922 2c0d 0a20 2020 2022 5365 6374 6f72  y",..    "Sector
+000063e0: 223a 2031 3433 3231 2c0d 0a20 2020 7d2c  ": 14321,..   },
+000063f0: 0d0a 5d0d 0a72 6573 706f 6e73 6573 203d  ..]..responses =
+00006400: 2064 632e 696e 7365 7274 5f64 6174 6128   dc.insert_data(
+00006410: 2243 6f6d 7061 6e79 222c 2074 6f5f 7365  "Company", to_se
+00006420: 6e64 290d 0a60 6060 0d0a 4966 2073 7563  nd)..```..If suc
+00006430: 6365 7373 6675 6c2c 2060 7265 7370 6f6e  cessful, `respon
+00006440: 7365 7360 2077 696c 6c20 636f 6e74 6169  ses` will contai
+00006450: 6e20 7468 6520 6265 6c6f 772c 206e 6f74  n the below, not
+00006460: 6520 7468 6174 2074 6865 2022 5465 7374  e that the "Test
+00006470: 2043 6f6d 7061 6e79 2032 2220 6e6f 7720   Company 2" now 
+00006480: 6861 7320 616e 2060 456e 7472 7949 6460  has an `EntryId`
+00006490: 2061 7320 6974 2068 6173 2062 6565 6e20   as it has been 
+000064a0: 6372 6561 7465 643a 0d0a 6060 6070 7974  created:..```pyt
+000064b0: 686f 6e0d 0a5b 0d0a 2020 207b 0d0a 2020  hon..[..   {..  
+000064c0: 2020 2245 6e74 7279 4964 223a 2032 3334    "EntryId": 234
+000064d0: 3536 372c 2020 0d0a 2020 2020 2243 6f6d  567,  ..    "Com
+000064e0: 7061 6e79 4e61 6d65 223a 2022 5465 7374  panyName": "Test
+000064f0: 2043 6f6d 7061 6e79 2031 222c 0d0a 2020   Company 1",..  
+00006500: 2020 2243 6f6d 7061 6e79 5479 7065 223a    "CompanyType":
+00006510: 2031 3233 3435 2c0d 0a20 2020 2022 4275   12345,..    "Bu
+00006520: 7369 6e65 7373 4465 7363 7269 7074 696f  sinessDescriptio
+00006530: 6e22 3a20 2248 6572 6520 6973 2061 6e20  n": "Here is an 
+00006540: 7570 6461 7465 6420 6275 7369 6e65 7373  updated business
+00006550: 2064 6573 6372 6970 7469 6f6e 222c 0d0a   description",..
+00006560: 2020 2020 2253 6563 746f 7222 3a20 3134      "Sector": 14
+00006570: 3332 312c 0d0a 2020 207d 2c0d 0a20 2020  321,..   },..   
+00006580: 7b0d 0a20 2020 2022 456e 7472 7949 6422  {..    "EntryId"
+00006590: 3a20 3233 3435 3638 2c0d 0a20 2020 2022  : 234568,..    "
+000065a0: 436f 6d70 616e 794e 616d 6522 3a20 2254  CompanyName": "T
+000065b0: 6573 7420 436f 6d70 616e 7920 3222 2c0d  est Company 2",.
+000065c0: 0a20 2020 2022 436f 6d70 616e 7954 7970  .    "CompanyTyp
+000065d0: 6522 3a20 3132 3334 352c 0d0a 2020 2020  e": 12345,..    
+000065e0: 2242 7573 696e 6573 7344 6573 6372 6970  "BusinessDescrip
+000065f0: 7469 6f6e 223a 2022 4865 7265 2069 7320  tion": "Here is 
+00006600: 6120 6275 7369 6e65 7373 2064 6573 6372  a business descr
+00006610: 6970 7469 6f6e 2066 6f72 2061 206e 6577  iption for a new
+00006620: 2063 6f6d 7061 6e79 222c 0d0a 2020 2020   company",..    
+00006630: 2253 6563 746f 7222 3a20 3134 3332 312c  "Sector": 14321,
+00006640: 0d0a 2020 207d 2c0d 0a5d 0d0a 6060 600d  ..   },..]..```.
+00006650: 0a23 2323 2320 556e 6465 7273 7461 6e64  .#### Understand
+00006660: 696e 6720 4572 726f 7273 0d0a 5468 6520  ing Errors..The 
+00006670: 6461 7461 206f 7065 7261 7469 6f6e 206d  data operation m
+00006680: 6574 686f 6473 2072 6169 7365 2065 7272  ethods raise err
+00006690: 6f72 7320 696e 2061 206e 756d 6265 7220  ors in a number 
+000066a0: 6f66 2077 6179 732c 2077 6865 6e20 6075  of ways, when `u
+000066b0: 7365 5f64 6561 6c63 6c6f 7564 5f69 6473  se_dealcloud_ids
+000066c0: 6020 6973 2060 4661 6c73 6560 2c20 6572  ` is `False`, er
+000066d0: 726f 7273 2061 7265 2066 6564 2062 6163  rors are fed bac
+000066e0: 6b20 6672 6f6d 2074 6865 2041 5049 2069  k from the API i
+000066f0: 6e74 6f20 7468 6520 6461 7461 2072 6574  nto the data ret
+00006700: 7572 6e65 6420 6672 6f6d 2074 6865 2066  urned from the f
+00006710: 756e 6374 696f 6e2e 0d0a 4578 616d 706c  unction...Exampl
+00006720: 652c 2069 6620 7468 6520 7365 6374 6f72  e, if the sector
+00006730: 2031 3233 3435 2064 6f65 7320 6e6f 7420   12345 does not 
+00006740: 6578 6973 743a 0d0a 0d0a 6060 6070 7974  exist:....```pyt
+00006750: 686f 6e0d 0a66 726f 6d20 6465 616c 636c  hon..from dealcl
+00006760: 6f75 645f 7364 6b20 696d 706f 7274 2044  oud_sdk import D
+00006770: 6561 6c43 6c6f 7564 0d0a 0d0a 6463 203d  ealCloud....dc =
+00006780: 2044 6561 6c43 6c6f 7564 2e66 726f 6d5f   DealCloud.from_
+00006790: 7961 6d6c 2822 7061 7468 2f74 6f2f 7961  yaml("path/to/ya
+000067a0: 6d6c 5f63 6f6e 6669 675f 6669 6c65 2e6a  ml_config_file.j
+000067b0: 736f 6e22 290d 0a0d 0a74 6f5f 7365 6e64  son")....to_send
+000067c0: 203d 205b 0d0a 2020 2020 7b27 436f 6d70   = [..    {'Comp
+000067d0: 616e 794e 616d 6527 3a20 2754 4553 545f  anyName': 'TEST_
+000067e0: 5550 4441 5445 4427 2c20 2253 6563 746f  UPDATED', "Secto
+000067f0: 7222 3a20 3132 3334 357d 0d0a 5d0d 0a72  r": 12345}..]..r
+00006800: 6573 706f 6e73 6573 203d 2064 632e 696e  esponses = dc.in
+00006810: 7365 7274 5f64 6174 6128 2257 4a5f 436f  sert_data("WJ_Co
+00006820: 6d70 616e 7922 2c20 746f 5f73 656e 6429  mpany", to_send)
+00006830: 0d0a 6060 600d 0a60 7265 7370 6f6e 7365  ..```..`response
+00006840: 7360 2077 696c 6c20 636f 6e74 6169 6e2e  s` will contain.
+00006850: 0d0a 6060 6070 7974 686f 6e0d 0a5b 7b27  ..```python..[{'
+00006860: 456e 7472 7949 6427 3a20 2d31 2c0d 0a20  EntryId': -1,.. 
+00006870: 2027 436f 6d70 616e 794e 616d 6527 3a20   'CompanyName': 
+00006880: 2754 4553 545f 5550 4441 5445 4427 2c0d  'TEST_UPDATED',.
+00006890: 0a20 2027 5365 6374 6f72 273a 204e 6f6e  .  'Sector': Non
+000068a0: 652c 0d0a 2020 2745 7272 6f72 7327 3a20  e,..  'Errors': 
+000068b0: 5b7b 2766 6965 6c64 273a 2027 5365 6374  [{'field': 'Sect
+000068c0: 6f72 272c 0d0a 2020 2020 2763 6f64 6527  or',..    'code'
+000068d0: 3a20 3530 3036 2c0d 0a20 2020 2027 6465  : 5006,..    'de
+000068e0: 7363 7269 7074 696f 6e27 3a20 274f 6e65  scription': 'One
+000068f0: 206f 7220 6d6f 7265 2072 6566 6572 656e   or more referen
+00006900: 6365 6420 656e 7472 6965 7320 6172 6520  ced entries are 
+00006910: 6e6f 7420 7661 6c69 6420 666f 7220 7468  not valid for th
+00006920: 6973 2066 6965 6c64 2e27 7d5d 7d5d 0d0a  is field.'}]}]..
+00006930: 6060 600d 0a3e 205b 214e 4f54 455d 0d0a  ```..> [!NOTE]..
+00006940: 3e20 496e 2074 6869 7320 6361 7365 2c20  > In this case, 
+00006950: 7468 6520 7265 636f 7264 2068 6173 206e  the record has n
+00006960: 6f74 2062 6565 6e20 6372 6561 7465 6420  ot been created 
+00006970: 696e 2074 6865 2073 6974 652e 2057 6865  in the site. Whe
+00006980: 6e20 6d75 6c74 6970 6c65 2072 6563 6f72  n multiple recor
+00006990: 6473 2061 7265 2074 7279 696e 6720 746f  ds are trying to
+000069a0: 2062 6520 6d61 6465 2061 6e64 2061 6e79   be made and any
+000069b0: 206f 6e65 2066 6169 6c73 2069 6e20 7468   one fails in th
+000069c0: 6973 2077 6179 2c20 6e6f 6e65 206f 6620  is way, none of 
+000069d0: 7468 6520 7265 636f 7264 7320 696e 2074  the records in t
+000069e0: 6861 7420 6772 6f75 7020 7769 6c6c 2062  hat group will b
+000069f0: 6520 6372 6561 7465 642e 2057 6865 6e20  e created. When 
+00006a00: 6120 6c61 7267 6520 766f 6c75 6d65 206f  a large volume o
+00006a10: 6620 7265 636f 7264 7320 6172 6520 6265  f records are be
+00006a20: 696e 6720 6372 6561 7465 642c 2060 4465  ing created, `De
+00006a30: 616c 436c 6f75 6460 2068 616e 646c 6573  alCloud` handles
+00006a40: 2062 7265 616b 696e 6720 7468 6520 6c61   breaking the la
+00006a50: 7267 6520 766f 6c75 6d65 206f 6620 6461  rge volume of da
+00006a60: 7461 2069 6e74 6f20 6d75 6c74 6970 6c65  ta into multiple
+00006a70: 2070 6167 6573 2e20 496e 2074 6869 7320   pages. In this 
+00006a80: 6361 7365 2c20 7768 6572 6520 7468 6572  case, where ther
+00006a90: 6520 6973 2061 6e20 6572 726f 7220 6f6e  e is an error on
+00006aa0: 2061 2072 6563 6f72 6420 696e 2061 2070   a record in a p
+00006ab0: 6167 652c 2061 6c6c 206f 6620 7468 6520  age, all of the 
+00006ac0: 7265 636f 7264 7320 696e 2074 6861 7420  records in that 
+00006ad0: 7061 6765 2077 696c 6c20 6e6f 7420 6265  page will not be
+00006ae0: 2063 7265 6174 6564 2f75 7064 6174 6564   created/updated
+00006af0: 2e0d 0a0d 0a57 6865 6e20 6075 7365 5f64  .....When `use_d
+00006b00: 6561 6c63 6c6f 7564 5f69 6473 6020 6973  ealcloud_ids` is
+00006b10: 2060 5472 7565 602c 2061 6e64 206c 6f6f   `True`, and loo
+00006b20: 6b75 7020 7661 6c75 6573 2061 7265 2075  kup values are u
+00006b30: 7365 642c 2074 6865 2063 7265 6174 652f  sed, the create/
+00006b40: 7570 6461 7465 2f75 7073 6572 7420 6d65  update/upsert me
+00006b50: 7468 6f64 7320 6172 6520 6c65 7373 2070  thods are less p
+00006b60: 726f 6e65 2074 6f20 2266 6169 6c69 6e67  rone to "failing
+00006b70: 2220 6572 726f 7273 2e20 5468 6973 2069  " errors. This i
+00006b80: 7320 6265 6361 7573 652c 2077 6865 6e20  s because, when 
+00006b90: 6120 7661 6c75 6520 6973 2062 6569 6e67  a value is being
+00006ba0: 2072 6573 6f6c 7665 6420 7468 726f 7567   resolved throug
+00006bb0: 6820 6120 606c 6f6f 6b75 705f 636f 6c75  h a `lookup_colu
+00006bc0: 6d6e 602c 2061 2076 616c 7565 2074 6861  mn`, a value tha
+00006bd0: 7420 6361 6e6e 6f74 2062 6520 666f 756e  t cannot be foun
+00006be0: 6420 7769 6c6c 2072 6573 756c 7420 696e  d will result in
+00006bf0: 2061 6e20 6572 726f 7220 6265 696e 6720   an error being 
+00006c00: 6c6f 6767 6564 2074 6f20 7468 6520 636f  logged to the co
+00006c10: 6e66 6967 7572 6564 206c 6f67 6765 722e  nfigured logger.
+00006c20: 2048 6f77 6576 6572 2c20 6173 2074 6865   However, as the
+00006c30: 2072 6563 6f72 6420 7072 6f67 7265 7373   record progress
+00006c40: 6573 2c20 7468 6520 756e 2d72 6573 6f6c  es, the un-resol
+00006c50: 7661 626c 6520 7661 6c75 6520 7769 6c6c  vable value will
+00006c60: 2073 696d 706c 7920 6265 2062 6c61 6e6b   simply be blank
+00006c70: 2e20 5468 6520 6c6f 6773 2061 7070 6561  . The logs appea
+00006c80: 7220 6173 2062 656c 6f77 3a0d 0a0d 0a46  r as below:....F
+00006c90: 6f72 2063 686f 6963 6520 6669 656c 6473  or choice fields
+00006ca0: 3a0d 0a60 6060 6261 7368 0d0a 4552 524f  :..```bash..ERRO
+00006cb0: 523a 2043 686f 6963 6520 6d61 7070 696e  R: Choice mappin
+00006cc0: 6720 6572 726f 7220 6f6e 3a20 7b6f 626a  g error on: {obj
+00006cd0: 6563 747d 2c20 7b66 6965 6c64 7d2c 2063  ect}, {field}, c
+00006ce0: 6f75 6c64 206e 6f74 2066 696e 6420 7661  ould not find va
+00006cf0: 6c75 653a 207b 7661 6c75 657d 0d0a 6060  lue: {value}..``
+00006d00: 600d 0a46 6f72 2072 6566 6572 656e 6365  `..For reference
+00006d10: 2066 6965 6c64 733a 0d0a 6060 6062 6173   fields:..```bas
+00006d20: 680d 0a45 5252 4f52 3a20 5265 6665 7265  h..ERROR: Refere
+00006d30: 6e63 6520 6d61 7070 696e 6720 6572 726f  nce mapping erro
+00006d40: 7220 6f6e 3a20 7b6f 626a 6563 747d 2c20  r on: {object}, 
+00006d50: 7b66 6965 6c64 7d2c 2063 6f75 6c64 206e  {field}, could n
+00006d60: 6f74 2066 696e 6420 7661 6c75 653a 207b  ot find value: {
+00006d70: 7661 6c75 657d 0d0a 6060 600d 0a46 6f72  value}..```..For
+00006d80: 2075 7365 7220 6669 656c 6473 3a0d 0a60   user fields:..`
+00006d90: 6060 6261 7368 0d0a 4552 524f 523a 2055  ``bash..ERROR: U
+00006da0: 7365 7220 6d61 7070 696e 6720 6572 726f  ser mapping erro
+00006db0: 7220 6f6e 3a20 7b6f 626a 6563 747d 2c20  r on: {object}, 
+00006dc0: 7b66 6965 6c64 7d2c 2063 6f75 6c64 206e  {field}, could n
+00006dd0: 6f74 2066 696e 6420 7661 6c75 653a 207b  ot find value: {
+00006de0: 7661 6c75 657d 0d0a 6060 600d 0a0d 0a57  value}..```....W
+00006df0: 6865 6e20 7573 696e 6720 6044 6561 6c43  hen using `DealC
+00006e00: 6c6f 7564 2e75 7064 6174 655f 6461 7461  loud.update_data
+00006e10: 2829 602c 2069 6620 616e 2060 456e 7472  ()`, if an `Entr
+00006e20: 7949 6460 2063 616e 6e6f 7420 6265 206c  yId` cannot be l
+00006e30: 6f63 6174 6564 2c20 796f 7520 7769 6c6c  ocated, you will
+00006e40: 2073 6565 2074 6865 2066 6f6c 6c6f 7769   see the followi
+00006e50: 6e67 2065 7272 6f72 3a0d 0a60 6060 6261  ng error:..```ba
+00006e60: 7368 0d0a 4552 524f 523a 2050 7269 6d61  sh..ERROR: Prima
+00006e70: 7279 204b 6579 2065 7272 6f72 206f 6e20  ry Key error on 
+00006e80: 6f62 6a65 6374 3a20 7b6f 626a 6563 747d  object: {object}
+00006e90: 2c20 7265 636f 7264 2066 6f75 6e64 2077  , record found w
+00006ea0: 6974 686f 7574 2027 456e 7472 7949 6427  ithout 'EntryId'
+00006eb0: 2066 6965 6c64 2e0d 0a60 6060 0d0a 0d0a   field...```....
+00006ec0: 2323 2320 4465 6c65 7465 2044 6174 610d  ### Delete Data.
+00006ed0: 0a60 4465 616c 436c 6f75 642e 6465 6c65  .`DealCloud.dele
+00006ee0: 7465 5f64 6174 6128 2960 2070 726f 7669  te_data()` provi
+00006ef0: 6465 7320 7468 6520 6162 696c 6974 7920  des the ability 
+00006f00: 746f 2064 656c 6574 6520 6461 7461 2066  to delete data f
+00006f10: 726f 6d20 616e 206f 626a 6563 7420 6279  rom an object by
+00006f20: 2074 6865 2060 456e 7472 7949 6460 2e20   the `EntryId`. 
+00006f30: 546f 2075 7365 2069 742c 2073 696d 706c  To use it, simpl
+00006f40: 7920 7061 7373 2074 6865 206f 626a 6563  y pass the objec
+00006f50: 7420 6170 6920 6e61 6d65 2074 6f20 7468  t api name to th
+00006f60: 6520 606f 626a 6563 745f 6170 695f 6e61  e `object_api_na
+00006f70: 6d65 6020 6172 6775 6d65 6e74 0d0a 616e  me` argument..an
+00006f80: 6420 6120 606c 6973 7460 206f 6620 6045  d a `list` of `E
+00006f90: 6e74 7279 4964 6073 2074 6f20 7468 6520  ntryId`s to the 
+00006fa0: 6072 6563 6f72 6473 6020 6172 6775 6d65  `records` argume
+00006fb0: 6e74 2e0d 0a0d 0a45 7861 6d70 6c65 2074  nt.....Example t
+00006fc0: 6f20 6465 6c65 7465 2074 776f 2072 6563  o delete two rec
+00006fd0: 6f72 6473 2077 6974 6820 7468 6520 456e  ords with the En
+00006fe0: 7472 7949 6473 2060 3132 3334 3531 6020  tryIds `123451` 
+00006ff0: 616e 6420 6031 3233 3436 603a 0d0a 0d0a  and `12346`:....
+00007000: 6060 6070 7974 686f 6e0d 0a66 726f 6d20  ```python..from 
+00007010: 6465 616c 636c 6f75 645f 7364 6b20 696d  dealcloud_sdk im
+00007020: 706f 7274 2044 6561 6c43 6c6f 7564 0d0a  port DealCloud..
+00007030: 0d0a 6463 203d 2044 6561 6c43 6c6f 7564  ..dc = DealCloud
+00007040: 2e66 726f 6d5f 7961 6d6c 2822 7061 7468  .from_yaml("path
+00007050: 2f74 6f2f 7961 6d6c 5f63 6f6e 6669 675f  /to/yaml_config_
+00007060: 6669 6c65 2e6a 736f 6e22 290d 0a0d 0a72  file.json")....r
+00007070: 6573 706f 6e73 6520 3d20 6463 2e64 656c  esponse = dc.del
+00007080: 6574 655f 6461 7461 280d 0a20 2020 6f62  ete_data(..   ob
+00007090: 6a65 6374 5f61 7069 5f6e 616d 653d 2243  ject_api_name="C
+000070a0: 6f6d 7061 6e79 222c 0d0a 2020 2072 6563  ompany",..   rec
+000070b0: 6f72 6473 3d5b 3132 3334 352c 2031 3233  ords=[12345, 123
+000070c0: 3436 5d0d 0a29 0d0a 6060 600d 0a60 7265  46]..)..```..`re
+000070d0: 7370 6f6e 7365 6020 7769 6c6c 2063 6f6e  sponse` will con
+000070e0: 7461 696e 3a0d 0a60 6060 7079 7468 6f6e  tain:..```python
+000070f0: 0d0a 5b0d 0a20 2020 7b27 656e 7472 7949  ..[..   {'entryI
+00007100: 6427 3a20 3132 3334 352c 2027 6669 656c  d': 12345, 'fiel
+00007110: 6449 6427 3a20 302c 2027 726f 7749 6427  dId': 0, 'rowId'
+00007120: 3a20 3439 3335 3635 302c 2027 6973 4e6f  : 4935650, 'isNo
+00007130: 4461 7461 273a 2046 616c 7365 7d2c 0d0a  Data': False},..
+00007140: 2020 207b 2765 6e74 7279 4964 273a 2031     {'entryId': 1
+00007150: 3233 3436 2c20 2766 6965 6c64 4964 273a  2346, 'fieldId':
+00007160: 2030 2c20 2772 6f77 4964 273a 2034 3933   0, 'rowId': 493
+00007170: 3536 3530 2c20 2769 734e 6f44 6174 6127  5650, 'isNoData'
+00007180: 3a20 4661 6c73 657d 2c0d 0a5d 0d0a 6060  : False},..]..``
+00007190: 600d 0a                                  `..
```

### Comparing `dealcloud_sdk-0.1.0/PKG-INFO` & `dealcloud_sdk-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6465 616c  : 2.1.Name: deal
 00000020: 636c 6f75 642d 7364 6b0a 5665 7273 696f  cloud-sdk.Versio
-00000030: 6e3a 2030 2e31 2e30 0a53 756d 6d61 7279  n: 0.1.0.Summary
+00000030: 6e3a 2030 2e31 2e31 0a53 756d 6d61 7279  n: 0.1.1.Summary
 00000040: 3a20 4465 616c 436c 6f75 6420 5344 4b20  : DealCloud SDK 
 00000050: 6973 2061 2077 7261 7070 6572 2061 726f  is a wrapper aro
 00000060: 756e 6420 7468 6520 4465 616c 436c 6f75  und the DealClou
 00000070: 6420 4150 492c 2064 6573 6967 6e65 6420  d API, designed 
 00000080: 746f 2061 7373 6973 7420 636c 6965 6e74  to assist client
 00000090: 7320 616e 6420 7061 7274 6e65 7273 2074  s and partners t
 000000a0: 6f20 6275 696c 6420 6f6e 2074 6f70 206f  o build on top o
@@ -49,1824 +49,1770 @@
 00000300: 6973 743a 2072 6571 7565 7374 7320 283e  ist: requests (>
 00000310: 3d32 2e33 312e 302c 3c33 2e30 2e30 290a  =2.31.0,<3.0.0).
 00000320: 5265 7175 6972 6573 2d44 6973 743a 2072  Requires-Dist: r
 00000330: 6571 7565 7374 732d 6675 7475 7265 7320  equests-futures 
 00000340: 283e 3d31 2e30 2e31 2c3c 322e 302e 3029  (>=1.0.1,<2.0.0)
 00000350: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
 00000360: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-00000370: 6d61 726b 646f 776e 0a0a 215b 4465 616c  markdown..![Deal
-00000380: 436c 6f75 645d 282f 6465 616c 636c 6f75  Cloud](/dealclou
-00000390: 642e 6a70 6729 0a3c 6831 3e64 6561 6c63  d.jpg).<h1>dealc
-000003a0: 6c6f 7564 5f73 646b 3c2f 6831 3e0a 3c70  loud_sdk</h1>.<p
-000003b0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-000003c0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-000003d0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7366  //github.com/psf
-000003e0: 2f62 6c61 636b 223e 3c69 6d67 2061 6c74  /black"><img alt
-000003f0: 3d22 436f 6465 2073 7479 6c65 3a20 626c  ="Code style: bl
-00000400: 6163 6b22 2073 7263 3d22 6874 7470 733a  ack" src="https:
-00000410: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000420: 2f62 6164 6765 2f63 6f64 6525 3230 7374  /badge/code%20st
-00000430: 796c 652d 626c 6163 6b2d 3030 3030 3030  yle-black-000000
-00000440: 2e73 7667 223e 3c2f 613e 0a3c 696d 6720  .svg"></a>.<img 
-00000450: 7372 633d 2263 6f76 6572 6167 652e 7376  src="coverage.sv
-00000460: 6722 3e0a 3c2f 703e 0a0a 4120 7772 6170  g">.</p>..A wrap
-00000470: 7065 7220 6172 6f75 6e64 2074 6865 2044  per around the D
-00000480: 6561 6c43 6c6f 7564 2041 5049 2c20 6465  ealCloud API, de
-00000490: 7369 676e 6564 2074 6f20 6173 7369 7374  signed to assist
-000004a0: 2075 7365 7273 2c20 636c 6965 6e74 7320   users, clients 
-000004b0: 616e 6420 7061 7274 6e65 7273 2074 6f20  and partners to 
-000004c0: 6275 696c 6420 6f6e 2074 6f70 206f 6620  build on top of 
-000004d0: 6f75 7220 706c 6174 666f 726d 2773 2041  our platform's A
-000004e0: 5049 2e0a 0a23 2043 6f6e 7465 6e74 730a  PI...# Contents.
-000004f0: 312e 205b 496e 7374 616c 6c61 7469 6f6e  1. [Installation
-00000500: 5d28 2369 6e73 7461 6c6c 6174 696f 6e29  ](#installation)
-00000510: 0a20 2020 312e 205b 5769 7468 2070 6970  .   1. [With pip
-00000520: 5d28 2370 6970 290a 2020 2032 2e20 5b4c  ](#pip).   2. [L
-00000530: 6f63 616c 6c79 5d28 2362 7569 6c64 2d61  ocally](#build-a
-00000540: 6e64 2d69 6e73 7461 6c6c 2d6c 6f63 616c  nd-install-local
-00000550: 6c79 290a 322e 205b 5573 6167 655d 2823  ly).2. [Usage](#
-00000560: 7573 6167 6529 0a20 2020 312e 205b 4372  usage).   1. [Cr
-00000570: 6561 7469 6e67 2061 2063 6c69 656e 7420  eating a client 
-00000580: 616e 6420 6175 7468 656e 7469 6361 7469  and authenticati
-00000590: 6e67 5d28 2363 7265 6174 696e 672d 612d  ng](#creating-a-
-000005a0: 636c 6965 6e74 2d61 6e64 2d61 7574 6865  client-and-authe
-000005b0: 6e74 6963 6174 696e 6729 0a20 2020 322e  nticating).   2.
-000005c0: 205b 5365 6375 7265 6c79 206c 6f61 6469   [Securely loadi
-000005d0: 6e67 2063 7265 6465 6e74 6961 6c73 5d28  ng credentials](
-000005e0: 2373 6563 7572 656c 792d 6c6f 6164 696e  #securely-loadin
-000005f0: 672d 6372 6564 656e 7469 616c 7329 0a20  g-credentials). 
-00000600: 2020 2020 2031 2e20 5b55 7369 6e67 2045       1. [Using E
-00000610: 6e76 6972 6f6e 6d65 6e74 2056 6172 6961  nvironment Varia
-00000620: 626c 6573 5d28 2375 7369 6e67 2d65 6e76  bles](#using-env
-00000630: 6972 6f6e 6d65 6e74 2d76 6172 6961 626c  ironment-variabl
-00000640: 6573 290a 2020 2020 2020 322e 205b 5573  es).      2. [Us
-00000650: 696e 6720 4a53 4f4e 2043 6f6e 6669 6720  ing JSON Config 
-00000660: 4669 6c65 5d28 2375 7369 6e67 2d6a 736f  File](#using-jso
-00000670: 6e2d 636f 6e66 6967 2d66 696c 6529 0a20  n-config-file). 
-00000680: 2020 2020 2033 2e20 5b55 7369 6e67 2059       3. [Using Y
-00000690: 414d 4c20 436f 6e66 6967 2046 696c 655d  AML Config File]
-000006a0: 2823 7573 696e 672d 7961 6d6c 2d63 6f6e  (#using-yaml-con
-000006b0: 6669 672d 6669 6c65 290a 2020 2033 2e20  fig-file).   3. 
-000006c0: 5b53 6368 656d 6120 5175 6572 7969 6e67  [Schema Querying
-000006d0: 5d28 2373 6368 656d 612d 7175 6572 7969  ](#schema-queryi
-000006e0: 6e67 290a 2020 2020 2020 312e 205b 4765  ng).      1. [Ge
-000006f0: 7420 5573 6572 735d 2823 6765 742d 7573  t Users](#get-us
-00000700: 6572 7329 0a20 2020 2020 2032 2e20 5b47  ers).      2. [G
-00000710: 6574 2043 7572 7265 6e63 6965 735d 2823  et Currencies](#
-00000720: 6765 742d 6375 7272 656e 6369 6573 290a  get-currencies).
-00000730: 2020 2020 2020 332e 205b 4765 7420 4f62        3. [Get Ob
-00000740: 6a65 6374 735d 2823 6765 742d 6f62 6a65  jects](#get-obje
-00000750: 6374 7329 0a20 2020 2020 2034 2e20 5b47  cts).      4. [G
-00000760: 6574 2046 6965 6c64 735d 2823 6765 742d  et Fields](#get-
-00000770: 6669 656c 6473 290a 2020 2020 2020 352e  fields).      5.
-00000780: 205b 4765 7420 5363 6865 6d61 5d28 2367   [Get Schema](#g
-00000790: 6574 2d73 6368 656d 6129 0a20 2020 342e  et-schema).   4.
-000007a0: 205b 4461 7461 204f 7065 7261 7469 6f6e   [Data Operation
-000007b0: 735d 2823 6461 7461 2d6f 7065 7261 7469  s](#data-operati
-000007c0: 6f6e 7329 0a20 2020 2020 2031 2e20 5b4c  ons).      1. [L
-000007d0: 6973 7420 436f 6e66 6967 7572 6564 2056  ist Configured V
-000007e0: 6965 7773 5d28 236c 6973 742d 636f 6e66  iews](#list-conf
-000007f0: 6967 7572 6564 2d76 6965 7773 290a 2020  igured-views).  
-00000800: 2020 2020 322e 205b 5265 6164 2044 6174      2. [Read Dat
-00000810: 615d 2823 7265 6164 2d64 6174 6129 0a20  a](#read-data). 
-00000820: 2020 2020 2020 2020 312e 205b 5265 6164          1. [Read
-00000830: 696e 6720 4461 7461 2066 726f 6d20 616e  ing Data from an
-00000840: 204f 626a 6563 745d 2823 7265 6164 696e   Object](#readin
-00000850: 672d 6461 7461 2d66 726f 6d2d 616e 2d6f  g-data-from-an-o
-00000860: 626a 6563 7429 0a20 2020 2020 2020 2020  bject).         
-00000870: 2020 2031 2e20 5b52 6573 6f6c 7669 6e67     1. [Resolving
-00000880: 2074 6f20 4e61 6d65 206f 7220 746f 2049   to Name or to I
-00000890: 445d 2823 7265 736f 6c76 696e 672d 746f  D](#resolving-to
-000008a0: 2d6e 616d 652d 6f72 2d74 6f2d 6964 290a  -name-or-to-id).
-000008b0: 2020 2020 2020 2020 2020 2020 322e 205b              2. [
-000008c0: 5265 6164 696e 6720 6120 5375 6273 6574  Reading a Subset
-000008d0: 206f 6620 4669 656c 6473 5d28 2372 6561   of Fields](#rea
-000008e0: 6469 6e67 2d61 2d73 7562 7365 742d 6f66  ding-a-subset-of
-000008f0: 2d66 6965 6c64 7329 0a20 2020 2020 2020  -fields).       
-00000900: 2020 322e 205b 5265 6164 696e 6720 4461    2. [Reading Da
-00000910: 7461 2066 726f 6d20 6120 5669 6577 5d28  ta from a View](
-00000920: 2372 6561 6469 6e67 2d64 6174 612d 6672  #reading-data-fr
-00000930: 6f6d 2d61 2d76 6965 7729 200a 2020 2020  om-a-view) .    
-00000940: 2020 2020 2020 2020 312e 205b 5573 696e          1. [Usin
-00000950: 6720 6120 4669 6c74 6572 2057 6865 6e20  g a Filter When 
-00000960: 5265 6164 696e 6720 5669 6577 2044 6174  Reading View Dat
-00000970: 615d 2823 7573 696e 672d 612d 6669 6c74  a](#using-a-filt
-00000980: 6572 2d77 6865 6e2d 7265 6164 696e 672d  er-when-reading-
-00000990: 7669 6577 2d64 6174 6129 200a 2020 2020  view-data) .    
-000009a0: 2020 332e 205b 4372 6561 7465 2c20 5570    3. [Create, Up
-000009b0: 6461 7465 2c20 5570 7365 7274 2044 6174  date, Upsert Dat
-000009c0: 615d 2823 6372 6561 7465 2d75 7064 6174  a](#create-updat
-000009d0: 652d 616e 642d 7570 7365 7274 2d64 6174  e-and-upsert-dat
-000009e0: 6129 0a20 2020 2020 2020 2020 312e 205b  a).         1. [
-000009f0: 4669 656c 6420 4d61 7070 696e 675d 2823  Field Mapping](#
-00000a00: 6669 656c 642d 6d61 7070 696e 6729 0a20  field-mapping). 
-00000a10: 2020 2020 2020 2020 322e 205b 4372 6561          2. [Crea
-00000a20: 7465 2044 6174 615d 2823 6372 6561 7465  te Data](#create
-00000a30: 2d64 6174 6129 0a20 2020 2020 2020 2020  -data).         
-00000a40: 332e 205b 5570 6461 7465 2044 6174 615d  3. [Update Data]
-00000a50: 2823 7570 6461 7465 2d64 6174 6129 0a20  (#update-data). 
-00000a60: 2020 2020 2020 2020 342e 205b 5570 7365          4. [Upse
-00000a70: 7274 2044 6174 615d 2823 7570 7365 7274  rt Data](#upsert
-00000a80: 2d64 6174 6129 0a20 2020 2020 2020 2020  -data).         
-00000a90: 352e 205b 556e 6465 7273 7461 6e64 696e  5. [Understandin
-00000aa0: 6720 4572 726f 7273 5d28 2375 6e64 6572  g Errors](#under
-00000ab0: 7374 616e 6469 6e67 2d65 7272 6f72 7329  standing-errors)
-00000ac0: 0a20 2020 2020 2034 2e20 5b44 656c 6574  .      4. [Delet
-00000ad0: 6520 4461 7461 5d28 2364 656c 6574 652d  e Data](#delete-
-00000ae0: 6461 7461 2920 0a0a 2320 496e 7374 616c  data) ..# Instal
-00000af0: 6c61 7469 6f6e 0a23 2320 7069 700a 496e  lation.## pip.In
-00000b00: 7374 616c 6c20 7573 696e 6720 7069 7020  stall using pip 
-00000b10: 7769 7468 3a0a 6060 6062 6173 680a 7069  with:.```bash.pi
-00000b20: 7020 696e 7374 616c 6c20 6465 616c 636c  p install dealcl
-00000b30: 6f75 645f 7364 6b0a 6060 600a 2323 2042  oud_sdk.```.## B
-00000b40: 7569 6c64 2061 6e64 2069 6e73 7461 6c6c  uild and install
-00000b50: 206c 6f63 616c 6c79 0a60 6465 616c 636c   locally.`dealcl
-00000b60: 6f75 645f 7364 6b60 2069 7320 6275 696c  oud_sdk` is buil
-00000b70: 7420 7573 696e 6720 5b70 6f65 7472 795d  t using [poetry]
-00000b80: 2868 7474 7073 3a2f 2f70 7974 686f 6e2d  (https://python-
-00000b90: 706f 6574 7279 2e6f 7267 2f29 2c20 656e  poetry.org/), en
-00000ba0: 7375 7265 2074 6861 7420 6974 2069 7320  sure that it is 
-00000bb0: 696e 7374 616c 6c65 6420 6f6e 2079 6f75  installed on you
-00000bc0: 7220 6d61 6368 696e 652e 0a60 6060 6261  r machine..```ba
-00000bd0: 7368 0a67 6974 2063 6c6f 6e65 2068 7474  sh.git clone htt
-00000be0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000bf0: 7763 742d 6a61 6d65 732f 6465 616c 636c  wct-james/dealcl
-00000c00: 6f75 645f 7364 6b2e 6769 740a 0a63 6420  oud_sdk.git..cd 
-00000c10: 6465 616c 636c 6f75 645f 7364 6b0a 0a70  dealcloud_sdk..p
-00000c20: 6f65 7472 7920 696e 7374 616c 6c0a 0a70  oetry install..p
-00000c30: 6f65 7472 7920 6275 696c 640a 6060 600a  oetry build.```.
-00000c40: 5468 6973 2077 696c 6c20 7072 6f64 7563  This will produc
-00000c50: 6520 6120 7768 6565 6c20 282e 7768 6c29  e a wheel (.whl)
-00000c60: 2066 696c 6520 696e 2074 6865 2060 6465   file in the `de
-00000c70: 616c 636c 6f75 645f 7364 6b2f 6469 7374  alcloud_sdk/dist
-00000c80: 6020 6469 7265 6374 6f72 792e 0a54 6f20  ` directory..To 
-00000c90: 696e 7374 616c 6c20 7468 6520 7061 636b  install the pack
-00000ca0: 6167 6520 6672 6f6d 2074 6865 2077 6865  age from the whe
-00000cb0: 656c 2c20 696e 2061 6e6f 7468 6572 2070  el, in another p
-00000cc0: 7974 686f 6e20 7072 6f6a 6563 743a 0a60  ython project:.`
-00000cd0: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
-00000ce0: 6c6c 2022 7061 7468 2f74 6f2f 6465 616c  ll "path/to/deal
-00000cf0: 636c 6f75 645f 7364 6b2f 6469 7374 2f64  cloud_sdk/dist/d
-00000d00: 6561 6c63 6c6f 7564 5f73 646b 2d58 2e59  ealcloud_sdk-X.Y
-00000d10: 2e5a 2d6e 6f6e 652d 616e 792e 7768 6c22  .Z-none-any.whl"
-00000d20: 0a60 6060 0a77 6865 7265 2074 6865 2070  .```.where the p
-00000d30: 6174 6820 6973 2074 6865 2061 6273 6f6c  ath is the absol
-00000d40: 7574 6520 7061 7468 2074 6f20 796f 7572  ute path to your
-00000d50: 202e 7768 6c20 6669 6c65 2e0a 0a0a 2320   .whl file....# 
-00000d60: 5573 6167 650a 0a23 2320 4372 6561 7469  Usage..## Creati
-00000d70: 6e67 2061 2063 6c69 656e 7420 616e 6420  ng a client and 
-00000d80: 6175 7468 656e 7469 6361 7469 6e67 0a60  authenticating.`
-00000d90: 6465 616c 636c 6f75 645f 7364 6b60 2773  dealcloud_sdk`'s
-00000da0: 206d 6169 6e20 656e 7472 7970 6f69 6e74   main entrypoint
-00000db0: 2069 7320 7468 6520 6044 6561 6c43 6c6f   is the `DealClo
-00000dc0: 7564 6020 636c 6173 732e 2057 6865 6e20  ud` class. When 
-00000dd0: 6974 2069 7320 696e 7374 616e 7469 6174  it is instantiat
-00000de0: 6564 2c20 7468 6520 6f62 6a65 6374 2069  ed, the object i
-00000df0: 7320 7363 6f70 6564 2074 6f20 6120 6769  s scoped to a gi
-00000e00: 7665 6e20 4465 616c 436c 6f75 6420 656e  ven DealCloud en
-00000e10: 7669 726f 6e6d 656e 742c 2062 7920 7061  vironment, by pa
-00000e20: 7373 696e 6720 7468 6520 7369 7465 2055  ssing the site U
-00000e30: 524c 2061 6e64 2041 5049 2063 7265 6465  RL and API crede
-00000e40: 6e74 6961 6c73 2061 7320 6172 6775 6d65  ntials as argume
-00000e50: 6e74 733a 0a0a 6060 6070 7974 686f 6e0a  nts:..```python.
-00000e60: 6672 6f6d 2064 6561 6c63 6c6f 7564 5f73  from dealcloud_s
-00000e70: 646b 2069 6d70 6f72 7420 4465 616c 436c  dk import DealCl
-00000e80: 6f75 640a 0a64 6320 3d20 4465 616c 436c  oud..dc = DealCl
-00000e90: 6f75 6428 0a20 2020 7369 7465 5f75 726c  oud(.   site_url
-00000ea0: 3d22 636c 6965 6e74 2e64 6561 6c63 6c6f  ="client.dealclo
-00000eb0: 7564 2e63 6f6d 222c 0a20 2020 636c 6965  ud.com",.   clie
-00000ec0: 6e74 5f69 643d 2231 3233 3435 222c 0a20  nt_id="12345",. 
-00000ed0: 2020 636c 6965 6e74 5f73 6563 7265 743d    client_secret=
-00000ee0: 2279 6f75 725f 636c 6965 6e74 5f73 6563  "your_client_sec
-00000ef0: 7265 7422 2c0a 290a 6060 600a 0a3e 205b  ret",.).```..> [
-00000f00: 2157 4152 4e49 4e47 5d0a 3e20 5768 696c  !WARNING].> Whil
-00000f10: 7374 2073 7569 7461 626c 6520 666f 7220  st suitable for 
-00000f20: 6c6f 6361 6c20 6465 7665 6c6f 706d 656e  local developmen
-00000f30: 742c 2074 6865 2061 626f 7665 2069 6d70  t, the above imp
-00000f40: 6c65 6d65 6e74 6174 696f 6e20 6973 2069  lementation is i
-00000f50: 6e73 6563 7572 6520 6966 2079 6f75 206b  nsecure if you k
-00000f60: 6565 7020 636f 6465 2069 6e20 6f6e 6c69  eep code in onli
-00000f70: 6e65 2072 6570 6f73 6974 6f72 6965 7320  ne repositories 
-00000f80: 7375 6368 2061 7320 4769 7448 7562 2e20  such as GitHub. 
-00000f90: 506c 6561 7365 2073 6565 2074 6865 2062  Please see the b
-00000fa0: 656c 6f77 2065 7861 6d70 6c65 7320 666f  elow examples fo
-00000fb0: 7220 6d6f 7265 2073 6563 7572 6520 696d  r more secure im
-00000fc0: 706c 656d 656e 7461 7469 6f6e 732e 2020  plementations.  
-00000fd0: 0a0a 2323 2053 6563 7572 656c 7920 6c6f  ..## Securely lo
-00000fe0: 6164 696e 6720 6372 6564 656e 7469 616c  ading credential
-00000ff0: 730a 2323 2320 5573 696e 6720 456e 7669  s.### Using Envi
-00001000: 726f 6e6d 656e 7420 5661 7269 6162 6c65  ronment Variable
-00001010: 730a 5768 6572 6520 7468 6520 656e 7669  s.Where the envi
-00001020: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-00001030: 7320 636f 6e74 6169 6e20 7468 6520 7265  s contain the re
-00001040: 6c65 7661 6e74 2076 616c 7565 732e 2054  levant values. T
-00001050: 6865 7365 2063 616e 2062 6520 6c6f 6164  hese can be load
-00001060: 6564 2066 726f 6d20 6120 2e65 6e76 2066  ed from a .env f
-00001070: 696c 6520 7573 696e 6720 7468 6520 6070  ile using the `p
-00001080: 7974 686f 6e2d 646f 7465 6e76 6020 5b50  ython-dotenv` [P
-00001090: 7950 6920 7061 636b 6167 655d 2868 7474  yPi package](htt
-000010a0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-000010b0: 6f6a 6563 742f 7079 7468 6f6e 2d64 6f74  oject/python-dot
-000010c0: 656e 762f 292e 0a0a 6060 6070 7974 686f  env/)...```pytho
-000010d0: 6e0a 6672 6f6d 2064 6561 6c63 6c6f 7564  n.from dealcloud
-000010e0: 5f73 646b 2069 6d70 6f72 7420 4465 616c  _sdk import Deal
-000010f0: 436c 6f75 640a 6672 6f6d 206f 7320 696d  Cloud.from os im
-00001100: 706f 7274 2067 6574 656e 760a 0a64 6320  port getenv..dc 
-00001110: 3d20 4465 616c 436c 6f75 6428 0a20 2020  = DealCloud(.   
-00001120: 2073 6974 655f 7572 6c3d 6765 7465 6e76   site_url=getenv
-00001130: 2822 4443 5f45 544c 5f53 4954 455f 5552  ("DC_ETL_SITE_UR
-00001140: 4c22 292c 0a20 2020 2063 6c69 656e 745f  L"),.    client_
-00001150: 6964 3d67 6574 656e 7628 2244 435f 4554  id=getenv("DC_ET
-00001160: 4c5f 434c 4945 4e54 5f49 4422 292c 0a20  L_CLIENT_ID"),. 
-00001170: 2020 2063 6c69 656e 745f 7365 6372 6574     client_secret
-00001180: 3d67 6574 656e 7628 2244 435f 4554 4c5f  =getenv("DC_ETL_
-00001190: 4150 495f 4b45 5922 292c 0a29 0a60 6060  API_KEY"),.).```
-000011a0: 0a23 2323 2055 7369 6e67 204a 534f 4e20  .### Using JSON 
-000011b0: 436f 6e66 6967 2046 696c 650a 4769 7665  Config File.Give
-000011c0: 6e20 6120 4a53 4f4e 2066 696c 6520 696e  n a JSON file in
-000011d0: 2074 6865 2062 656c 6f77 2066 6f72 6d61   the below forma
-000011e0: 743a 0a60 6060 6a73 6f6e 0a7b 0a20 2022  t:.```json.{.  "
-000011f0: 7369 7465 5f75 726c 223a 2022 636c 6965  site_url": "clie
-00001200: 6e74 2e64 6561 6c63 6c6f 7564 2e63 6f6d  nt.dealcloud.com
-00001210: 222c 0a20 2022 636c 6965 6e74 5f69 6422  ",.  "client_id"
-00001220: 3a20 3132 3334 352c 0a20 2022 636c 6965  : 12345,.  "clie
-00001230: 6e74 5f73 6563 7265 7422 3a20 2279 6f75  nt_secret": "you
-00001240: 725f 636c 6965 6e74 5f73 6563 7265 7422  r_client_secret"
-00001250: 0a7d 0a60 6060 0a54 6865 2044 6561 6c43  .}.```.The DealC
-00001260: 6c6f 7564 206f 626a 6563 7420 6361 6e20  loud object can 
-00001270: 6265 2063 7265 6174 6564 2061 7320 6265  be created as be
-00001280: 6c6f 773a 0a0a 6060 6070 7974 686f 6e0a  low:..```python.
-00001290: 6672 6f6d 2064 6561 6c63 6c6f 7564 5f73  from dealcloud_s
-000012a0: 646b 2069 6d70 6f72 7420 4465 616c 436c  dk import DealCl
-000012b0: 6f75 640a 0a64 6320 3d20 4465 616c 436c  oud..dc = DealCl
-000012c0: 6f75 642e 6672 6f6d 5f6a 736f 6e28 2270  oud.from_json("p
-000012d0: 6174 682f 746f 2f6a 736f 6e5f 636f 6e66  ath/to/json_conf
-000012e0: 6967 5f66 696c 652e 6a73 6f6e 2229 0a60  ig_file.json").`
-000012f0: 6060 0a53 696d 696c 6172 6c79 2c20 6966  ``.Similarly, if
-00001300: 2074 6865 2063 7265 6465 6e74 6961 6c73   the credentials
-00001310: 2061 7265 2073 746f 7265 6420 6173 2070   are stored as p
-00001320: 6172 7420 6f66 2061 206c 6172 6765 7220  art of a larger 
-00001330: 4a53 4f4e 2063 6f6e 6669 6720 6669 6c65  JSON config file
-00001340: 2c20 6120 6b65 7920 7061 7468 2063 616e  , a key path can
-00001350: 2062 6520 7061 7373 6564 2061 7320 7468   be passed as th
-00001360: 6520 7365 636f 6e64 2061 7267 756d 656e  e second argumen
-00001370: 742c 2064 6972 6563 7469 6e67 2020 6044  t, directing  `D
-00001380: 6561 6c43 6c6f 7564 6020 746f 2074 6865  ealCloud` to the
-00001390: 2070 6174 6820 6f66 2074 6865 2063 7265   path of the cre
-000013a0: 6465 6e74 6961 6c73 2069 6e20 7468 6520  dentials in the 
-000013b0: 7769 6465 7220 4a53 4f4e 2e20 466f 7220  wider JSON. For 
-000013c0: 6578 616d 706c 653a 0a60 6060 6a73 6f6e  example:.```json
-000013d0: 0a7b 0a20 2020 2022 6f74 6865 7222 3a20  .{.    "other": 
-000013e0: 5b31 2c32 2c33 5d2c 0a20 2020 2022 6372  [1,2,3],.    "cr
-000013f0: 6564 7322 3a7b 0a20 2020 2020 2020 2022  eds":{.        "
-00001400: 6463 223a 7b0a 2020 2020 2020 2020 2020  dc":{.          
-00001410: 2273 6974 655f 7572 6c22 3a20 2263 6c69  "site_url": "cli
-00001420: 656e 742e 6465 616c 636c 6f75 642e 636f  ent.dealcloud.co
-00001430: 6d22 2c0a 2020 2020 2020 2020 2020 2263  m",.          "c
-00001440: 6c69 656e 745f 6964 223a 2031 3233 3435  lient_id": 12345
-00001450: 2c0a 2020 2020 2020 2020 2020 2263 6c69  ,.          "cli
-00001460: 656e 745f 7365 6372 6574 223a 2022 796f  ent_secret": "yo
-00001470: 7572 5f63 6c69 656e 745f 7365 6372 6574  ur_client_secret
-00001480: 220a 2020 2020 2020 2020 7d0a 2020 2020  ".        }.    
-00001490: 7d0a 7d0a 6060 600a 0a60 6060 7079 7468  }.}.```..```pyth
-000014a0: 6f6e 0a66 726f 6d20 6465 616c 636c 6f75  on.from dealclou
-000014b0: 645f 7364 6b20 696d 706f 7274 2044 6561  d_sdk import Dea
-000014c0: 6c43 6c6f 7564 0a0a 6463 203d 2044 6561  lCloud..dc = Dea
-000014d0: 6c43 6c6f 7564 2e66 726f 6d5f 6a73 6f6e  lCloud.from_json
-000014e0: 2822 7061 7468 2f74 6f2f 6a73 6f6e 5f63  ("path/to/json_c
-000014f0: 6f6e 6669 675f 6669 6c65 2e6a 736f 6e22  onfig_file.json"
-00001500: 2c20 2263 7265 6473 2e64 6322 290a 6060  , "creds.dc").``
-00001510: 600a 2323 2320 5573 696e 6720 5941 4d4c  `.### Using YAML
-00001520: 2043 6f6e 6669 6720 4669 6c65 0a47 6976   Config File.Giv
-00001530: 656e 2061 2059 414d 4c20 6669 6c65 2069  en a YAML file i
-00001540: 6e20 7468 6520 6265 6c6f 7720 666f 726d  n the below form
-00001550: 6174 3a0a 6060 6079 616d 6c0a 7369 7465  at:.```yaml.site
-00001560: 5f75 726c 3a20 2263 6c69 656e 742e 6465  _url: "client.de
-00001570: 616c 636c 6f75 642e 636f 6d22 0a63 6c69  alcloud.com".cli
-00001580: 656e 745f 6964 3a20 3132 3334 350a 636c  ent_id: 12345.cl
-00001590: 6965 6e74 5f73 6563 7265 743a 2022 796f  ient_secret: "yo
-000015a0: 7572 5f63 6c69 656e 745f 7365 6372 6574  ur_client_secret
-000015b0: 220a 6060 600a 5468 6520 4465 616c 436c  ".```.The DealCl
-000015c0: 6f75 6420 6f62 6a65 6374 2063 616e 2062  oud object can b
-000015d0: 6520 6372 6561 7465 6420 6173 2062 656c  e created as bel
-000015e0: 6f77 3a0a 0a60 6060 7079 7468 6f6e 0a66  ow:..```python.f
-000015f0: 726f 6d20 6465 616c 636c 6f75 645f 7364  rom dealcloud_sd
-00001600: 6b20 696d 706f 7274 2044 6561 6c43 6c6f  k import DealClo
-00001610: 7564 0a0a 6463 203d 2044 6561 6c43 6c6f  ud..dc = DealClo
-00001620: 7564 2e66 726f 6d5f 7961 6d6c 2822 7061  ud.from_yaml("pa
-00001630: 7468 2f74 6f2f 7961 6d6c 5f63 6f6e 6669  th/to/yaml_confi
-00001640: 675f 6669 6c65 2e6a 736f 6e22 290a 6060  g_file.json").``
-00001650: 600a 5369 6d69 6c61 726c 792c 2069 6620  `.Similarly, if 
-00001660: 7468 6520 6372 6564 656e 7469 616c 7320  the credentials 
-00001670: 6172 6520 7374 6f72 6564 2061 7320 7061  are stored as pa
-00001680: 7274 206f 6620 6120 6c61 7267 6572 2059  rt of a larger Y
-00001690: 414d 4c20 636f 6e66 6967 2066 696c 652c  AML config file,
-000016a0: 2061 206b 6579 2070 6174 6820 6361 6e20   a key path can 
-000016b0: 6265 2070 6173 7365 6420 6173 2074 6865  be passed as the
-000016c0: 2073 6563 6f6e 6420 6172 6775 6d65 6e74   second argument
-000016d0: 2c20 6469 7265 6374 696e 6720 2060 4465  , directing  `De
-000016e0: 616c 436c 6f75 6460 2074 6f20 7468 6520  alCloud` to the 
-000016f0: 7061 7468 206f 6620 7468 6520 6372 6564  path of the cred
-00001700: 656e 7469 616c 7320 696e 2074 6865 2077  entials in the w
-00001710: 6964 6572 2059 414d 4c2e 2046 6f72 2065  ider YAML. For e
-00001720: 7861 6d70 6c65 3a0a 6060 6079 616d 6c0a  xample:.```yaml.
-00001730: 6f74 6865 723a 0a20 202d 2031 0a20 202d  other:.  - 1.  -
-00001740: 2032 0a20 202d 2033 0a63 7265 6473 3a0a   2.  - 3.creds:.
-00001750: 2020 6463 3a0a 2020 2020 7369 7465 5f75    dc:.    site_u
-00001760: 726c 3a20 2263 6c69 656e 742e 6465 616c  rl: "client.deal
-00001770: 636c 6f75 642e 636f 6d22 0a20 2020 2063  cloud.com".    c
-00001780: 6c69 656e 745f 6964 3a20 3132 3334 350a  lient_id: 12345.
-00001790: 2020 2020 636c 6965 6e74 5f73 6563 7265      client_secre
-000017a0: 743a 2022 796f 7572 5f63 6c69 656e 745f  t: "your_client_
-000017b0: 7365 6372 6574 220a 6060 600a 0a60 6060  secret".```..```
-000017c0: 7079 7468 6f6e 0a66 726f 6d20 6465 616c  python.from deal
-000017d0: 636c 6f75 645f 7364 6b20 696d 706f 7274  cloud_sdk import
-000017e0: 2044 6561 6c43 6c6f 7564 0a0a 6463 203d   DealCloud..dc =
-000017f0: 2044 6561 6c43 6c6f 7564 2e66 726f 6d5f   DealCloud.from_
-00001800: 7961 6d6c 2822 7061 7468 2f74 6f2f 7961  yaml("path/to/ya
-00001810: 6d6c 5f63 6f6e 6669 675f 6669 6c65 2e6a  ml_config_file.j
-00001820: 736f 6e22 2c20 2263 7265 6473 2e64 6322  son", "creds.dc"
-00001830: 290a 6060 600a 0a23 2320 5363 6865 6d61  ).```..## Schema
-00001840: 2051 7565 7279 696e 670a 5468 6520 4465   Querying.The De
-00001850: 616c 436c 6f75 6420 4150 4920 616c 6c6f  alCloud API allo
-00001860: 7773 2079 6f75 2074 6f20 7175 6572 7920  ws you to query 
-00001870: 7468 6520 7363 6865 6d61 206f 6620 6120  the schema of a 
-00001880: 6769 7665 6e20 7369 7465 2e20 5468 6520  given site. The 
-00001890: 6044 6561 6c43 6c6f 7564 6020 636c 6173  `DealCloud` clas
-000018a0: 7320 7072 6f76 6964 6573 2061 6363 6573  s provides acces
-000018b0: 7320 746f 2074 6865 2073 6368 656d 6120  s to the schema 
-000018c0: 656e 6470 6f69 6e74 7320 7468 726f 7567  endpoints throug
-000018d0: 6820 7468 6520 666f 6c6c 6f77 696e 6720  h the following 
-000018e0: 6d65 7468 6f64 733a 0a3e 2054 6865 2073  methods:.> The s
-000018f0: 6368 656d 6120 6d6f 6465 6c73 2061 7265  chema models are
-00001900: 2064 6566 696e 6564 2075 7369 6e67 205b   defined using [
-00001910: 5079 6461 6e74 6963 5d28 6874 7470 733a  Pydantic](https:
-00001920: 2f2f 7079 6461 6e74 6963 2e64 6576 2f29  //pydantic.dev/)
-00001930: 2c20 666f 7220 636c 6561 7220 7661 6c69  , for clear vali
-00001940: 6461 7469 6f6e 2c20 7374 7261 6967 6874  dation, straight
-00001950: 666f 7277 6172 6420 6174 7472 6962 7574  forward attribut
-00001960: 6520 6163 6365 7373 2061 6e64 2049 4445  e access and IDE
-00001970: 2061 7373 6973 7461 6e63 652e 0a3e 2054   assistance..> T
-00001980: 6865 7365 206d 6f64 656c 7320 6361 6e20  hese models can 
-00001990: 6265 2066 6f75 6e64 2069 6e20 7468 6520  be found in the 
-000019a0: 5b6d 6f64 656c 735d 282f 6465 616c 636c  [models](/dealcl
-000019b0: 6f75 645f 7364 6b2f 6d6f 6465 6c73 2920  oud_sdk/models) 
-000019c0: 6469 7265 6374 6f72 792e 0a0a 2323 2320  directory...### 
-000019d0: 4765 7420 5573 6572 730a 0a60 4465 616c  Get Users..`Deal
-000019e0: 436c 6f75 642e 6765 745f 7573 6572 7328  Cloud.get_users(
-000019f0: 2960 2077 696c 6c20 7265 7475 726e 2061  )` will return a
-00001a00: 6c6c 2075 7365 7273 2069 6e20 7468 6520  ll users in the 
-00001a10: 7369 7465 2e20 5370 6563 6966 6963 616c  site. Specifical
-00001a20: 6c79 2c20 616e 2061 7272 6179 206f 6620  ly, an array of 
-00001a30: 6055 7365 7260 206f 626a 6563 7473 2028  `User` objects (
-00001a40: 7365 6520 5b74 6865 2055 7365 7220 6f62  see [the User ob
-00001a50: 6a65 6374 5d28 2f64 6561 6c63 6c6f 7564  ject](/dealcloud
-00001a60: 5f73 646b 2f6d 6f64 656c 732f 7363 6865  _sdk/models/sche
-00001a70: 6d61 2e70 7923 4c36 392d 4c37 3529 292e  ma.py#L69-L75)).
-00001a80: 2054 6865 2061 7267 756d 656e 743a 2060   The argument: `
-00001a90: 6163 7469 7665 5f6f 6e6c 7960 2069 7320  active_only` is 
-00001aa0: 6120 626f 6f6c 6561 6e20 7468 6174 2063  a boolean that c
-00001ab0: 616e 2062 6520 7061 7373 6564 2c20 6966  an be passed, if
-00001ac0: 2074 7275 652c 2074 6865 2066 756e 6374   true, the funct
-00001ad0: 696f 6e20 7769 6c6c 206f 6e6c 7920 7265  ion will only re
-00001ae0: 7475 726e 2061 6374 6976 6520 7573 6572  turn active user
-00001af0: 732e 0a0a 4578 616d 706c 653a 0a0a 6060  s...Example:..``
-00001b00: 6070 7974 686f 6e0a 6672 6f6d 2064 6561  `python.from dea
-00001b10: 6c63 6c6f 7564 5f73 646b 2069 6d70 6f72  lcloud_sdk impor
-00001b20: 7420 4465 616c 436c 6f75 640a 0a64 6320  t DealCloud..dc 
-00001b30: 3d20 4465 616c 436c 6f75 642e 6672 6f6d  = DealCloud.from
-00001b40: 5f79 616d 6c28 2270 6174 682f 746f 2f79  _yaml("path/to/y
-00001b50: 616d 6c5f 636f 6e66 6967 5f66 696c 652e  aml_config_file.
-00001b60: 6a73 6f6e 2229 0a0a 7573 6572 7320 3d20  json")..users = 
-00001b70: 6463 2e67 6574 5f75 7365 7273 2829 0a0a  dc.get_users()..
-00001b80: 666f 7220 7573 6572 2069 6e20 7573 6572  for user in user
-00001b90: 733a 0a20 2020 2070 7269 6e74 2866 227b  s:.    print(f"{
-00001ba0: 7573 6572 2e6e 616d 657d 3a20 7b75 7365  user.name}: {use
-00001bb0: 722e 656d 6169 6c7d 2229 0a60 6060 0a57  r.email}").```.W
-00001bc0: 696c 6c20 6f75 7470 7574 3a0a 6060 6062  ill output:.```b
-00001bd0: 6173 680a 5573 6572 2031 3a20 7573 6572  ash.User 1: user
-00001be0: 3140 656d 6169 6c2e 636f 6d0a 5573 6572  1@email.com.User
-00001bf0: 2032 3a20 7573 6572 3240 656d 6169 6c2e   2: user2@email.
-00001c00: 636f 6d0a 5573 6572 2033 3a20 7573 6572  com.User 3: user
-00001c10: 3340 656d 6169 6c2e 636f 6d0a 5573 6572  3@email.com.User
-00001c20: 2034 3a20 7573 6572 3440 656d 6169 6c2e   4: user4@email.
-00001c30: 636f 6d0a 2e2e 2e65 7463 0a60 6060 0a23  com....etc.```.#
-00001c40: 2323 2047 6574 2043 7572 7265 6e63 6965  ## Get Currencie
-00001c50: 730a 6044 6561 6c43 6c6f 7564 2e67 6574  s.`DealCloud.get
-00001c60: 5f63 7572 7265 6e63 6965 7328 2960 2077  _currencies()` w
-00001c70: 696c 6c20 7265 7475 726e 2074 6865 2063  ill return the c
-00001c80: 7572 7265 6e63 7920 636f 6465 7320 6f66  urrency codes of
-00001c90: 2061 6c6c 2065 6e61 626c 6564 2063 7572   all enabled cur
-00001ca0: 7265 6e63 6965 7320 696e 2074 6865 2073  rencies in the s
-00001cb0: 6974 652e 0a45 7861 6d70 6c65 3a0a 0a60  ite..Example:..`
-00001cc0: 6060 7079 7468 6f6e 0a66 726f 6d20 6465  ``python.from de
-00001cd0: 616c 636c 6f75 645f 7364 6b20 696d 706f  alcloud_sdk impo
-00001ce0: 7274 2044 6561 6c43 6c6f 7564 0a0a 6463  rt DealCloud..dc
-00001cf0: 203d 2044 6561 6c43 6c6f 7564 2e66 726f   = DealCloud.fro
-00001d00: 6d5f 7961 6d6c 2822 7061 7468 2f74 6f2f  m_yaml("path/to/
-00001d10: 7961 6d6c 5f63 6f6e 6669 675f 6669 6c65  yaml_config_file
-00001d20: 2e6a 736f 6e22 290a 0a63 7572 7265 6e63  .json")..currenc
-00001d30: 6965 7320 3d20 6463 2e67 6574 5f63 7572  ies = dc.get_cur
-00001d40: 7265 6e63 6965 7328 290a 0a66 6f72 2063  rencies()..for c
-00001d50: 6379 2069 6e20 6375 7272 656e 6369 6573  cy in currencies
-00001d60: 3a0a 2020 2020 7072 696e 7428 6363 7929  :.    print(ccy)
-00001d70: 0a60 6060 0a57 696c 6c20 6f75 7470 7574  .```.Will output
-00001d80: 3a0a 6060 6062 6173 680a 4742 500a 5553  :.```bash.GBP.US
-00001d90: 440a 4555 520a 2e2e 2e65 7463 0a60 6060  D.EUR....etc.```
-00001da0: 0a0a 2323 2320 4765 7420 4f62 6a65 6374  ..### Get Object
-00001db0: 730a 6044 6561 6c43 6c6f 7564 2e67 6574  s.`DealCloud.get
-00001dc0: 5f6f 626a 6563 7428 2960 2077 696c 6c20  _object()` will 
-00001dd0: 7265 7475 726e 2061 6c6c 2063 6f6e 6669  return all confi
-00001de0: 6775 7265 6420 6f62 6a65 6374 7320 696e  gured objects in
-00001df0: 2074 6865 2073 6974 652e 2053 7065 6369   the site. Speci
-00001e00: 6669 6361 6c6c 792c 2061 6e20 6172 7261  fically, an arra
-00001e10: 7920 6f66 2060 4f62 6a65 6374 6020 6f62  y of `Object` ob
-00001e20: 6a65 6374 7320 2873 6565 205b 7468 6520  jects (see [the 
-00001e30: 4f62 6a65 6374 206f 626a 6563 745d 282f  Object object](/
-00001e40: 6465 616c 636c 6f75 645f 7364 6b2f 6d6f  dealcloud_sdk/mo
-00001e50: 6465 6c73 2f73 6368 656d 612e 7079 234c  dels/schema.py#L
-00001e60: 362d 4c31 3629 292e 0a45 7861 6d70 6c65  6-L16))..Example
-00001e70: 3a0a 0a60 6060 7079 7468 6f6e 0a66 726f  :..```python.fro
-00001e80: 6d20 6465 616c 636c 6f75 645f 7364 6b20  m dealcloud_sdk 
-00001e90: 696d 706f 7274 2044 6561 6c43 6c6f 7564  import DealCloud
-00001ea0: 0a0a 6463 203d 2044 6561 6c43 6c6f 7564  ..dc = DealCloud
-00001eb0: 2e66 726f 6d5f 7961 6d6c 2822 7061 7468  .from_yaml("path
-00001ec0: 2f74 6f2f 7961 6d6c 5f63 6f6e 6669 675f  /to/yaml_config_
-00001ed0: 6669 6c65 2e6a 736f 6e22 290a 0a6f 626a  file.json")..obj
-00001ee0: 6563 7473 203d 2064 632e 6765 745f 6f62  ects = dc.get_ob
-00001ef0: 6a65 6374 7328 290a 0a66 6f72 206f 626a  jects()..for obj
-00001f00: 2069 6e20 6f62 6a65 6374 733a 0a20 2020   in objects:.   
-00001f10: 2070 7269 6e74 2866 227b 6f62 6a2e 6170   print(f"{obj.ap
-00001f20: 694e 616d 657d 3a20 7b6f 626a 2e70 6c75  iName}: {obj.plu
-00001f30: 7261 6c4e 616d 657d 2c20 7b6f 626a 2e73  ralName}, {obj.s
-00001f40: 696e 6775 6c61 724e 616d 657d 2229 0a60  ingularName}").`
-00001f50: 6060 0a57 696c 6c20 6f75 7470 7574 3a0a  ``.Will output:.
-00001f60: 6060 6062 6173 680a 436f 6d70 616e 793a  ```bash.Company:
-00001f70: 2043 6f6d 7061 6e69 6573 2c20 436f 6d70   Companies, Comp
-00001f80: 616e 790a 436f 6e74 6163 743a 2043 6f6e  any.Contact: Con
-00001f90: 7461 6374 732c 2043 6f6e 7461 6374 0a43  tacts, Contact.C
-00001fa0: 6f6d 7061 6e79 4164 6472 6573 733a 2043  ompanyAddress: C
-00001fb0: 6f6d 7061 6e79 2041 6464 7265 7373 6573  ompany Addresses
-00001fc0: 2c20 436f 6d70 616e 7920 4164 6472 6573  , Company Addres
-00001fd0: 730a 2e2e 2e65 7463 0a60 6060 0a0a 2323  s....etc.```..##
-00001fe0: 2047 6574 2046 6965 6c64 730a 6044 6561   Get Fields.`Dea
-00001ff0: 6c43 6c6f 7564 2e67 6574 5f66 6965 6c64  lCloud.get_field
-00002000: 7328 2960 2070 726f 7669 6465 7320 7468  s()` provides th
-00002010: 6520 6162 696c 6974 7920 746f 2072 6574  e ability to ret
-00002020: 7572 6e20 6669 656c 6473 2063 6f6e 6669  urn fields confi
-00002030: 6775 7265 6420 696e 2074 6865 2073 6974  gured in the sit
-00002040: 652e 2053 7065 6369 6669 6361 6c6c 792c  e. Specifically,
-00002050: 2061 6e20 6172 7261 7920 6f66 2060 4669   an array of `Fi
-00002060: 656c 6460 206f 626a 6563 7473 2028 7365  eld` objects (se
-00002070: 6520 5b74 6865 2046 6965 6c64 206f 626a  e [the Field obj
-00002080: 6563 745d 282f 6465 616c 636c 6f75 645f  ect](/dealcloud_
-00002090: 7364 6b2f 6d6f 6465 6c73 2f73 6368 656d  sdk/models/schem
-000020a0: 612e 7079 234c 3239 2d4c 3533 2929 2e0a  a.py#L29-L53))..
-000020b0: 0a54 6865 7265 2061 7265 2074 6872 6565  .There are three
-000020c0: 2077 6179 7320 746f 2071 7565 7279 2066   ways to query f
-000020d0: 6f72 2066 6965 6c64 733a 0a31 2e20 5f5f  or fields:.1. __
-000020e0: 416c 6c20 4669 656c 6473 5f5f 3a20 6361  All Fields__: ca
-000020f0: 6c6c 2060 4465 616c 436c 6f75 642e 6765  ll `DealCloud.ge
-00002100: 745f 6669 656c 6473 2829 6020 7769 7468  t_fields()` with
-00002110: 206e 6f20 6172 6775 6d65 6e74 7320 746f   no arguments to
-00002120: 2072 6574 7572 6e20 616c 6c20 6669 656c   return all fiel
-00002130: 6473 2e0a 0a60 6060 7079 7468 6f6e 0a66  ds...```python.f
-00002140: 726f 6d20 6465 616c 636c 6f75 645f 7364  rom dealcloud_sd
-00002150: 6b20 696d 706f 7274 2044 6561 6c43 6c6f  k import DealClo
-00002160: 7564 0a0a 6463 203d 2044 6561 6c43 6c6f  ud..dc = DealClo
-00002170: 7564 2e66 726f 6d5f 7961 6d6c 2822 7061  ud.from_yaml("pa
-00002180: 7468 2f74 6f2f 7961 6d6c 5f63 6f6e 6669  th/to/yaml_confi
-00002190: 675f 6669 6c65 2e6a 736f 6e22 290a 0a66  g_file.json")..f
-000021a0: 6965 6c64 7320 3d20 6463 2e67 6574 5f66  ields = dc.get_f
-000021b0: 6965 6c64 7328 290a 6060 600a 6066 6965  ields().```.`fie
-000021c0: 6c64 7360 2077 696c 6c20 636f 6e74 6169  lds` will contai
-000021d0: 6e20 6120 6c69 7374 206f 6620 6046 6965  n a list of `Fie
-000021e0: 6c64 6020 6f62 6a65 6374 7320 636f 6e74  ld` objects cont
-000021f0: 6169 6e69 6e67 2061 6c6c 2063 6f6e 6669  aining all confi
-00002200: 6775 7265 6420 6669 656c 6473 2069 6e20  gured fields in 
-00002210: 7468 6520 7369 7465 2e0a 0a0a 322e 205f  the site....2. _
-00002220: 5f41 6c6c 2046 6965 6c64 7320 666f 7220  _All Fields for 
-00002230: 616e 204f 626a 6563 745f 5f3a 2063 616c  an Object__: cal
-00002240: 6c20 6044 6561 6c43 6c6f 7564 2e67 6574  l `DealCloud.get
-00002250: 5f66 6965 6c64 7328 6f62 6a65 6374 5f69  _fields(object_i
-00002260: 643d 224f 626a 6563 744e 616d 6522 2960  d="ObjectName")`
-00002270: 2077 6974 6820 606f 626a 6563 745f 6964   with `object_id
-00002280: 6020 7365 7420 746f 2074 6865 2064 6573  ` set to the des
-00002290: 6972 6564 206f 626a 6563 7420 6170 6920  ired object api 
-000022a0: 6e61 6d65 2c20 6f72 206f 626a 6563 7420  name, or object 
-000022b0: 6964 2c20 746f 2072 6574 7572 6e20 616c  id, to return al
-000022c0: 6c20 6669 656c 6473 2063 6f6e 6669 6775  l fields configu
-000022d0: 7265 6420 666f 7220 7468 6174 206f 626a  red for that obj
-000022e0: 6563 742e 0a0a 6060 6070 7974 686f 6e0a  ect...```python.
-000022f0: 6672 6f6d 2064 6561 6c63 6c6f 7564 5f73  from dealcloud_s
-00002300: 646b 2069 6d70 6f72 7420 4465 616c 436c  dk import DealCl
-00002310: 6f75 640a 0a64 6320 3d20 4465 616c 436c  oud..dc = DealCl
-00002320: 6f75 642e 6672 6f6d 5f79 616d 6c28 2270  oud.from_yaml("p
-00002330: 6174 682f 746f 2f79 616d 6c5f 636f 6e66  ath/to/yaml_conf
-00002340: 6967 5f66 696c 652e 6a73 6f6e 2229 0a0a  ig_file.json")..
-00002350: 6669 656c 6473 203d 2064 632e 6765 745f  fields = dc.get_
-00002360: 6669 656c 6473 2822 436f 6d70 616e 7922  fields("Company"
-00002370: 290a 6060 600a 6066 6965 6c64 7360 2077  ).```.`fields` w
-00002380: 696c 6c20 636f 6e74 6169 6e20 6120 6c69  ill contain a li
-00002390: 7374 206f 6620 6046 6965 6c64 6020 6f62  st of `Field` ob
-000023a0: 6a65 6374 732c 2063 6f6e 7461 696e 696e  jects, containin
-000023b0: 6720 616c 6c20 6669 656c 6473 2063 6f6e  g all fields con
-000023c0: 6669 6775 7265 6420 696e 2074 6865 2022  figured in the "
-000023d0: 436f 6d70 616e 7922 206f 626a 6563 742e  Company" object.
-000023e0: 0a0a 0a33 2e20 5f5f 4120 4669 656c 6420  ...3. __A Field 
-000023f0: 6279 2046 6965 6c64 2049 445f 5f3a 2063  by Field ID__: c
-00002400: 616c 6c20 6044 6561 6c43 6c6f 7564 2e67  all `DealCloud.g
-00002410: 6574 5f66 6965 6c64 7328 6669 656c 645f  et_fields(field_
-00002420: 6964 3d31 3233 3429 6020 7769 7468 2060  id=1234)` with `
-00002430: 6669 656c 645f 6964 6020 7365 7420 746f  field_id` set to
-00002440: 2074 6865 2049 4420 6f66 2074 6865 2064   the ID of the d
-00002450: 6573 6972 6564 2066 6965 6c64 2e0a 0a60  esired field...`
-00002460: 6060 7079 7468 6f6e 0a66 726f 6d20 6465  ``python.from de
-00002470: 616c 636c 6f75 645f 7364 6b20 696d 706f  alcloud_sdk impo
-00002480: 7274 2044 6561 6c43 6c6f 7564 0a0a 6463  rt DealCloud..dc
-00002490: 203d 2044 6561 6c43 6c6f 7564 2e66 726f   = DealCloud.fro
-000024a0: 6d5f 7961 6d6c 2822 7061 7468 2f74 6f2f  m_yaml("path/to/
-000024b0: 7961 6d6c 5f63 6f6e 6669 675f 6669 6c65  yaml_config_file
-000024c0: 2e6a 736f 6e22 290a 0a66 6965 6c64 203d  .json")..field =
-000024d0: 2064 632e 6765 745f 6669 656c 6473 2866   dc.get_fields(f
-000024e0: 6965 6c64 5f69 643d 3132 3334 290a 6060  ield_id=1234).``
-000024f0: 600a 6066 6965 6c64 6020 7769 6c6c 2063  `.`field` will c
-00002500: 6f6e 7461 696e 2061 2073 696e 676c 6520  ontain a single 
-00002510: 6046 6965 6c64 6020 6f62 6a65 6374 2c20  `Field` object, 
-00002520: 6465 7363 7269 6269 6e67 2074 6865 2066  describing the f
-00002530: 6965 6c64 2077 6974 6820 4944 2060 3132  ield with ID `12
-00002540: 3334 602e 0a0a 2323 2320 4765 7420 5363  34`...### Get Sc
-00002550: 6865 6d61 0a60 4465 616c 436c 6f75 642e  hema.`DealCloud.
-00002560: 6765 745f 7363 6865 6d61 2829 6020 6973  get_schema()` is
-00002570: 2061 206d 6574 686f 6420 7468 6174 2077   a method that w
-00002580: 696c 6c20 7265 7475 726e 2074 6865 2066  ill return the f
-00002590: 756c 6c20 4465 616c 436c 6f75 6420 7363  ull DealCloud sc
-000025a0: 6865 6d61 2069 6e20 6120 7369 6e67 6c65  hema in a single
-000025b0: 206f 626a 6563 7420 2873 6565 205b 7468   object (see [th
-000025c0: 6520 5363 6865 6d61 206f 626a 6563 745d  e Schema object]
-000025d0: 2864 6561 6c63 6c6f 7564 5f73 646b 2f6d  (dealcloud_sdk/m
-000025e0: 6f64 656c 732f 7363 6865 6d61 2e70 7923  odels/schema.py#
-000025f0: 4c36 332d 4c36 3629 292e 0a54 6865 206d  L63-L66))..The m
-00002600: 6574 686f 6420 7461 6b65 7320 7468 6520  ethod takes the 
-00002610: 6172 6775 6d65 6e74 3a20 606b 6579 5f74  argument: `key_t
-00002620: 7970 6560 2c20 7768 6963 6820 6465 7363  ype`, which desc
-00002630: 7269 6265 7320 7768 6963 6820 6669 656c  ribes which fiel
-00002640: 6420 7769 6c6c 2062 6520 7573 6564 2061  d will be used a
-00002650: 7320 6b65 7973 2069 6e20 7468 6520 6e65  s keys in the ne
-00002660: 7374 6564 206f 626a 6563 7420 7374 7275  sted object stru
-00002670: 6374 7572 6520 6465 7363 7269 6269 6e67  cture describing
-00002680: 2074 6865 2073 6368 656d 612e 200a 0a54   the schema. ..T
-00002690: 6865 206f 7074 696f 6e73 2061 7265 3a0a  he options are:.
-000026a0: 2d20 6061 7069 6020 2d20 5468 6520 4150  - `api` - The AP
-000026b0: 4920 6e61 6d65 0a2d 2060 6469 7370 6c61  I name.- `displa
-000026c0: 7960 202d 2054 6865 2064 6973 706c 6179  y` - The display
-000026d0: 206e 616d 650a 2d20 6069 6460 202d 2054   name.- `id` - T
-000026e0: 6865 206f 626a 6563 742f 6669 656c 6420  he object/field 
-000026f0: 4944 0a0a 5573 6167 6520 4578 616d 706c  ID..Usage Exampl
-00002700: 653a 0a0a 6060 6070 7974 686f 6e0a 6672  e:..```python.fr
-00002710: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
-00002720: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
-00002730: 640a 0a64 6320 3d20 4465 616c 436c 6f75  d..dc = DealClou
-00002740: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
-00002750: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
-00002760: 5f66 696c 652e 6a73 6f6e 2229 0a0a 7363  _file.json")..sc
-00002770: 6865 6d61 203d 2064 632e 6765 745f 7363  hema = dc.get_sc
-00002780: 6865 6d61 2822 6170 6922 290a 6060 600a  hema("api").```.
-00002790: 6073 6368 656d 6160 2077 696c 6c20 636f  `schema` will co
-000027a0: 6e74 6169 6e20 7468 6520 6120 6053 6368  ntain the a `Sch
-000027b0: 656d 6160 206f 626a 6563 7420 7769 7468  ema` object with
-000027c0: 2074 6865 2041 5049 206e 616d 6573 2061   the API names a
-000027d0: 7320 6b65 7973 2c20 6173 2062 656c 6f77  s keys, as below
-000027e0: 3a20 0a0a 6061 7069 6020 4578 616d 706c  : ..`api` Exampl
-000027f0: 653a 0a60 6060 7079 7468 6f6e 0a7b 0a20  e:.```python.{. 
-00002800: 2022 436f 6d70 616e 7941 5049 4e61 6d65   "CompanyAPIName
-00002810: 223a 207b 0a20 2020 2022 436f 6d70 616e  ": {.    "Compan
-00002820: 794f 626a 6563 744d 6574 6144 6174 6122  yObjectMetaData"
-00002830: 3a20 222e 2e2e 222c 0a20 2020 2022 436f  : "...",.    "Co
-00002840: 6d70 616e 794f 626a 6563 7446 6965 6c64  mpanyObjectField
-00002850: 7322 3a20 7b0a 2020 2020 2020 2246 6965  s": {.      "Fie
-00002860: 6c64 3141 5049 4e61 6d65 223a 207b 0a20  ld1APIName": {. 
-00002870: 2020 2020 2020 2022 4669 656c 6431 4d65         "Field1Me
-00002880: 7461 4461 7461 223a 2022 2e2e 2e22 0a20  taData": "...". 
-00002890: 2020 2020 207d 0a20 2020 207d 0a20 207d       }.    }.  }
-000028a0: 0a7d 0a60 6060 0a60 6469 7370 6c61 7960  .}.```.`display`
-000028b0: 2045 7861 6d70 6c65 3a0a 6060 6070 7974   Example:.```pyt
-000028c0: 686f 6e0a 7b0a 2020 2243 6f6d 7061 6e79  hon.{.  "Company
-000028d0: 2044 6973 706c 6179 204e 616d 6522 3a20   Display Name": 
-000028e0: 7b0a 2020 2020 2243 6f6d 7061 6e79 4f62  {.    "CompanyOb
-000028f0: 6a65 6374 4d65 7461 4461 7461 223a 2022  jectMetaData": "
-00002900: 2e2e 2e22 2c0a 2020 2020 2243 6f6d 7061  ...",.    "Compa
-00002910: 6e79 4f62 6a65 6374 4669 656c 6473 223a  nyObjectFields":
-00002920: 207b 0a20 2020 2020 2022 4669 656c 6420   {.      "Field 
-00002930: 3120 4469 7370 6c61 7920 4e61 6d65 223a  1 Display Name":
-00002940: 207b 0a20 2020 2020 2020 2022 4669 656c   {.        "Fiel
-00002950: 6431 4d65 7461 4461 7461 223a 2022 2e2e  d1MetaData": "..
-00002960: 2e22 0a20 2020 2020 207d 0a20 2020 207d  .".      }.    }
-00002970: 0a20 207d 0a7d 0a60 6060 0a60 6964 6020  .  }.}.```.`id` 
-00002980: 4578 616d 706c 653a 0a3e 204e 6f74 6520  Example:.> Note 
-00002990: 7468 6520 4944 206f 6620 7468 6520 2243  the ID of the "C
-000029a0: 6f6d 7061 6e79 2220 6f62 6a65 6374 2069  ompany" object i
-000029b0: 7320 3132 3334 3520 616e 6420 7468 6520  s 12345 and the 
-000029c0: 4944 206f 6620 7468 6520 2246 6965 6c64  ID of the "Field
-000029d0: 2031 2220 6669 656c 6420 6973 2031 3233   1" field is 123
-000029e0: 3435 3620 0a60 6060 7079 7468 6f6e 0a7b  456 .```python.{
-000029f0: 0a20 2031 3233 3435 3a20 7b0a 2020 2020  .  12345: {.    
-00002a00: 2243 6f6d 7061 6e79 4f62 6a65 6374 4d65  "CompanyObjectMe
-00002a10: 7461 4461 7461 223a 2022 2e2e 2e22 2c0a  taData": "...",.
-00002a20: 2020 2020 2243 6f6d 7061 6e79 4f62 6a65      "CompanyObje
-00002a30: 6374 4669 656c 6473 223a 207b 0a20 2020  ctFields": {.   
-00002a40: 2020 2031 3233 3435 363a 207b 0a20 2020     123456: {.   
-00002a50: 2020 2020 2022 4669 656c 6431 4d65 7461       "Field1Meta
-00002a60: 4461 7461 223a 2022 2e2e 2e22 0a20 2020  Data": "...".   
-00002a70: 2020 207d 0a20 2020 207d 0a20 207d 0a7d     }.    }.  }.}
-00002a80: 0a60 6060 0a0a 2323 2044 6174 6120 4f70  .```..## Data Op
-00002a90: 6572 6174 696f 6e73 0a54 6865 2060 4465  erations.The `De
-00002aa0: 616c 436c 6f75 6460 206f 626a 6563 7420  alCloud` object 
-00002ab0: 7072 6f76 6964 6573 206d 6574 686f 6473  provides methods
-00002ac0: 2074 6f20 4372 6561 7465 2c20 5265 6164   to Create, Read
-00002ad0: 2c20 5570 6461 7465 2061 6e64 2044 656c  , Update and Del
-00002ae0: 6574 6520 6461 7461 2069 6e20 6275 6c6b  ete data in bulk
-00002af0: 2e20 4173 2069 7473 2064 6566 6175 6c74  . As its default
-00002b00: 2062 6568 6176 696f 7572 2c20 7768 656e   behaviour, when
-00002b10: 2077 6f72 6b69 6e67 2077 6974 6820 7369   working with si
-00002b20: 7465 2064 6174 612c 2074 6865 206c 6962  te data, the lib
-00002b30: 7261 7279 2075 7365 7320 4461 7461 4672  rary uses DataFr
-00002b40: 616d 6573 2077 6974 680a 7468 6520 5b50  ames with.the [P
-00002b50: 616e 6461 735d 2868 7474 7073 3a2f 2f70  andas](https://p
-00002b60: 616e 6461 732e 7079 6461 7461 2e6f 7267  andas.pydata.org
-00002b70: 2f29 206c 6962 7261 7279 2c20 686f 7765  /) library, howe
-00002b80: 7665 7220 7468 6520 6f70 7469 6f6e 2069  ver the option i
-00002b90: 7320 6176 6169 6c61 626c 6520 666f 7220  s available for 
-00002ba0: 6974 2074 6f20 776f 726b 2077 6974 6820  it to work with 
-00002bb0: 6a75 7374 2070 7974 686f 6e20 7374 616e  just python stan
-00002bc0: 6461 7264 2064 6174 6120 7479 7065 732e  dard data types.
-00002bd0: 0a0a 2323 2320 4c69 7374 2043 6f6e 6669  ..### List Confi
-00002be0: 6775 7265 6420 5669 6577 730a 6044 6561  gured Views.`Dea
-00002bf0: 6c43 6c6f 7564 2e6c 6973 745f 636f 6e66  lCloud.list_conf
-00002c00: 6967 7572 6564 5f76 6965 7773 2829 6020  igured_views()` 
-00002c10: 7265 7475 726e 7320 6120 6052 6f77 7360  returns a `Rows`
-00002c20: 2028 7365 6520 5b74 6865 2052 6f77 7320   (see [the Rows 
-00002c30: 6f62 6a65 6374 5d28 2f64 6561 6c63 6c6f  object](/dealclo
-00002c40: 7564 5f73 646b 2f6d 6f64 656c 732f 6461  ud_sdk/models/da
-00002c50: 7461 2e70 7923 4c34 2d4c 3829 2920 636f  ta.py#L4-L8)) co
-00002c60: 6e74 6169 6e69 6e67 2061 6c6c 2063 6f6e  ntaining all con
-00002c70: 6669 6775 7265 6420 7669 6577 7320 696e  figured views in
-00002c80: 2074 6865 2073 6974 652e 0a54 6865 2061   the site..The a
-00002c90: 7267 756d 656e 7420 6069 735f 7072 6976  rgument `is_priv
-00002ca0: 6174 6560 2063 616e 2062 6520 7061 7373  ate` can be pass
-00002cb0: 6564 2061 7320 6120 626f 6f6c 6561 6e2c  ed as a boolean,
-00002cc0: 2077 6865 7265 2069 6620 7472 7565 2c20   where if true, 
-00002cd0: 6f6e 6c79 2070 7269 7661 7465 2076 6965  only private vie
-00002ce0: 7773 2074 6f20 2869 6e63 6c75 6469 6e67  ws to (including
-00002cf0: 2076 6965 7773 2073 6861 7265 6420 7769   views shared wi
-00002d00: 7468 2920 7468 6520 6175 7468 656e 7469  th) the authenti
-00002d10: 6361 7465 6420 7573 6572 2077 696c 6c20  cated user will 
-00002d20: 6265 2072 6574 7572 6e65 642e 0a0a 4578  be returned...Ex
-00002d30: 616d 706c 653a 0a0a 6060 6070 7974 686f  ample:..```pytho
-00002d40: 6e0a 6672 6f6d 2064 6561 6c63 6c6f 7564  n.from dealcloud
-00002d50: 5f73 646b 2069 6d70 6f72 7420 4465 616c  _sdk import Deal
-00002d60: 436c 6f75 640a 0a64 6320 3d20 4465 616c  Cloud..dc = Deal
-00002d70: 436c 6f75 642e 6672 6f6d 5f79 616d 6c28  Cloud.from_yaml(
-00002d80: 2270 6174 682f 746f 2f79 616d 6c5f 636f  "path/to/yaml_co
-00002d90: 6e66 6967 5f66 696c 652e 6a73 6f6e 2229  nfig_file.json")
-00002da0: 0a0a 7669 6577 7320 3d20 6463 2e6c 6973  ..views = dc.lis
-00002db0: 745f 636f 6e66 6967 7572 6564 5f76 6965  t_configured_vie
-00002dc0: 7773 2829 0a60 6060 0a60 7669 6577 7360  ws().```.`views`
-00002dd0: 2077 696c 6c20 636f 6e74 6169 6e20 6120   will contain a 
-00002de0: 7375 6d6d 6172 7920 6f66 2063 6f6e 6669  summary of confi
-00002df0: 6775 7265 6420 7669 6577 732e 0a0a 2323  gured views...##
-00002e00: 2320 5265 6164 2044 6174 610a 6044 6561  # Read Data.`Dea
-00002e10: 6c43 6c6f 7564 2e72 6561 645f 6461 7461  lCloud.read_data
-00002e20: 2829 6020 616c 6c6f 7773 2075 7365 7273  ()` allows users
-00002e30: 2074 6f20 7265 6164 2064 6174 6120 6672   to read data fr
-00002e40: 6f6d 2061 2044 6561 6c43 6c6f 7564 206f  om a DealCloud o
-00002e50: 626a 6563 7420 696e 746f 2061 2060 7061  bject into a `pa
-00002e60: 6e64 6173 2e44 6174 6146 7261 6d65 6020  ndas.DataFrame` 
-00002e70: 6f72 2061 206c 6973 7420 6f66 2070 7974  or a list of pyt
-00002e80: 686f 6e20 6469 6374 696f 6e61 7269 6573  hon dictionaries
-00002e90: 2e0a 3e20 5b21 494d 504f 5254 414e 545d  ..> [!IMPORTANT]
-00002ea0: 200a 3e20 4f6e 6c79 206f 6e65 206f 6620   .> Only one of 
-00002eb0: 6f62 6a65 6374 5f69 6420 6f72 2076 6965  object_id or vie
-00002ec0: 775f 6964 2063 616e 2062 6520 706f 7075  w_id can be popu
-00002ed0: 6c61 7465 640a 2020 2020 2020 2020 0a41  lated.        .A
-00002ee0: 7267 756d 656e 7473 3a0a 0a2d 206f 626a  rguments:..- obj
-00002ef0: 6563 745f 6964 2060 556e 696f 6e5b 696e  ect_id `Union[in
-00002f00: 742c 2073 7472 5d60 3a20 7468 6520 6f62  t, str]`: the ob
-00002f10: 6a65 6374 2074 6f20 7075 6c6c 2064 6174  ject to pull dat
-00002f20: 6120 6672 6f6d 0a2d 2076 6965 775f 6964  a from.- view_id
-00002f30: 2060 556e 696f 6e5b 696e 742c 2073 7472   `Union[int, str
-00002f40: 5d60 3a20 7468 6520 7669 6577 2074 6f20  ]`: the view to 
-00002f50: 7075 6c6c 2064 6174 6120 6672 6f6d 0a2d  pull data from.-
-00002f60: 206f 7574 7075 7420 6073 7472 603a 2060   output `str`: `
-00002f70: 7061 6e64 6173 6020 6f72 2060 6c69 7374  pandas` or `list
-00002f80: 602c 2064 6563 6964 6573 2074 6865 206f  `, decides the o
-00002f90: 7574 7075 7420 666f 726d 6174 2c20 6070  utput format, `p
-00002fa0: 616e 6461 7360 2069 7320 6465 6661 756c  andas` is defaul
-00002fb0: 740a 2d20 7265 736f 6c76 6520 6073 7472  t.- resolve `str
-00002fc0: 603a 2066 6f72 2070 616e 6461 732c 2077  `: for pandas, w
-00002fd0: 6865 7265 2066 6965 6c64 7320 636f 6e74  here fields cont
-00002fe0: 6169 6e20 616e 206f 626a 6563 7420 2863  ain an object (c
-00002ff0: 686f 6963 652c 2072 6566 6572 656e 6365  hoice, reference
-00003000: 2c20 7573 6572 292c 2072 6573 6f6c 7665  , user), resolve
-00003010: 2074 6f20 7468 6520 6964 206f 7220 6e61   to the id or na
-00003020: 6d65 0a2d 2076 6965 775f 6669 6c74 6572  me.- view_filter
-00003030: 2060 6c69 7374 5b64 6963 745d 603a 2063   `list[dict]`: c
-00003040: 6f6c 756d 6e20 7175 6572 6965 7320 746f  olumn queries to
-00003050: 2022 7375 7070 6c79 2076 616c 7565 206c   "supply value l
-00003060: 6174 6572 2220 696e 2076 6965 7773 2c20  ater" in views, 
-00003070: 7365 653a 2068 7474 7073 3a2f 2f61 7069  see: https://api
-00003080: 2e64 6f63 732e 6465 616c 636c 6f75 642e  .docs.dealcloud.
-00003090: 636f 6d2f 646f 6373 2f64 6174 612f 726f  com/docs/data/ro
-000030a0: 7773 2f76 6965 775f 6465 7461 696c 730a  ws/view_details.
-000030b0: 2d20 6669 656c 6473 2060 6c69 7374 5b73  - fields `list[s
-000030c0: 7472 5d60 3a20 6966 206e 6f74 2060 4e6f  tr]`: if not `No
-000030d0: 6e65 602c 2072 6574 7572 6e20 6f6e 6c79  ne`, return only
-000030e0: 2066 6965 6c64 7320 696e 2074 6865 206c   fields in the l
-000030f0: 6973 742e 200a 2d20 7175 6572 7920 6073  ist. .- query `s
-00003100: 7472 603a 2061 2044 6561 6c43 6c6f 7564  tr`: a DealCloud
-00003110: 2072 6f77 7320 7175 6572 7920 7374 7269   rows query stri
-00003120: 6e67 2074 6f20 7265 7175 6573 7420 7370  ng to request sp
-00003130: 6563 6966 6963 2069 6e66 6f72 6d61 7469  ecific informati
-00003140: 6f6e 2c20 7365 653a 2068 7474 7073 3a2f  on, see: https:/
-00003150: 2f61 7069 2e64 6f63 732e 6465 616c 636c  /api.docs.dealcl
-00003160: 6f75 642e 636f 6d2f 646f 6373 2f64 6174  oud.com/docs/dat
-00003170: 612f 726f 7773 2f71 7565 7279 0a2d 2069  a/rows/query.- i
-00003180: 6e63 6c75 6465 5f6e 756c 6c73 2060 626f  nclude_nulls `bo
-00003190: 6f6c 603a 2069 6620 7472 7565 2c20 6e75  ol`: if true, nu
-000031a0: 6c6c 2063 6f6c 756d 6e73 2077 696c 6c20  ll columns will 
-000031b0: 616c 736f 2062 6520 7265 7475 726e 6564  also be returned
-000031c0: 0a2d 2063 6f6c 756d 6e5f 6865 6164 6572  .- column_header
-000031d0: 7320 6073 7472 603a 2073 7065 6369 6669  s `str`: specifi
-000031e0: 6573 2074 6865 2076 616c 7565 2074 7970  es the value typ
-000031f0: 6520 6f66 2074 6865 2072 6574 7572 6e20  e of the return 
-00003200: 6669 656c 6420 6b65 7973 2f63 6f6c 756d  field keys/colum
-00003210: 6e20 6e61 6d65 732e 0a20 202d 2060 6170  n names..  - `ap
-00003220: 6960 203d 2046 6965 6c64 2041 5049 204e  i` = Field API N
-00003230: 616d 650a 2020 2d20 606e 616d 6560 203d  ame.  - `name` =
-00003240: 2046 6965 6c64 2044 6973 706c 6179 204e   Field Display N
-00003250: 616d 650a 2020 2d20 6069 6460 203d 2046  ame.  - `id` = F
-00003260: 6965 6c64 2049 440a 0a23 2323 2320 5265  ield ID..#### Re
-00003270: 6164 696e 6720 4461 7461 2066 726f 6d20  ading Data from 
-00003280: 616e 204f 626a 6563 740a 4578 616d 706c  an Object.Exampl
-00003290: 653a 0a0a 6060 6070 7974 686f 6e0a 6672  e:..```python.fr
-000032a0: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
-000032b0: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
-000032c0: 640a 0a64 6320 3d20 4465 616c 436c 6f75  d..dc = DealClou
-000032d0: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
-000032e0: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
-000032f0: 5f66 696c 652e 6a73 6f6e 2229 0a0a 6461  _file.json")..da
-00003300: 7461 203d 2064 632e 7265 6164 5f64 6174  ta = dc.read_dat
-00003310: 6128 2243 6f6d 7061 6e79 2229 0a60 6060  a("Company").```
-00003320: 0a60 6461 7461 6020 7769 6c6c 2062 6520  .`data` will be 
-00003330: 6120 6070 616e 6461 732e 4461 7461 4672  a `pandas.DataFr
-00003340: 616d 6560 2061 7320 6265 6c6f 773a 0a0a  ame` as below:..
-00003350: 7c20 456e 7472 7949 6420 7c20 436f 6d70  | EntryId | Comp
-00003360: 616e 794e 616d 6520 7c20 436f 6d70 616e  anyName | Compan
-00003370: 7954 7970 6520 2020 2020 2020 2020 2020  yType           
-00003380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033d0: 207c 0a7c 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d   |.|---------|--
-000033e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
-000033f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003450: 2d2d 2d2d 7c0a 7c20 3132 3334 3520 2020  ----|.| 12345   
-00003460: 7c20 436f 6d70 616e 7931 2020 2020 7c20  | Company1    | 
-00003470: 5b7b 2773 6571 4e75 6d62 6572 273a 2033  [{'seqNumber': 3
-00003480: 2c20 2769 7341 7574 6f50 6466 273a 2046  , 'isAutoPdf': F
-00003490: 616c 7365 2c20 2769 6427 3a20 3331 3937  alse, 'id': 3197
-000034a0: 3738 302c 2027 6e61 6d65 273a 2027 4c69  780, 'name': 'Li
-000034b0: 6d69 7465 6420 5061 7274 6e65 7227 2c20  mited Partner', 
-000034c0: 2765 6e74 7279 4c69 7374 4964 273a 202d  'entryListId': -
-000034d0: 367d 5d20 2020 207c 0a7c 2031 3233 3436  6}]    |.| 12346
-000034e0: 2020 207c 2043 6f6d 7061 6e79 3220 2020     | Company2   
-000034f0: 207c 205b 7b27 7365 714e 756d 6265 7227   | [{'seqNumber'
-00003500: 3a20 312c 2027 6973 4175 746f 5064 6627  : 1, 'isAutoPdf'
-00003510: 3a20 4661 6c73 652c 2027 6964 273a 2033  : False, 'id': 3
-00003520: 3139 3737 3832 2c20 276e 616d 6527 3a20  197782, 'name': 
-00003530: 274f 7065 7261 7469 6e67 2043 6f6d 7061  'Operating Compa
-00003540: 6e79 272c 2027 656e 7472 794c 6973 7449  ny', 'entryListI
-00003550: 6427 3a20 2d36 7d5d 2020 7c0a 7c20 3132  d': -6}]  |.| 12
-00003560: 3334 3720 2020 7c20 436f 6d70 616e 7933  347   | Company3
-00003570: 2020 2020 7c20 5b7b 2773 6571 4e75 6d62      | [{'seqNumb
-00003580: 6572 273a 2033 2c20 2769 7341 7574 6f50  er': 3, 'isAutoP
-00003590: 6466 273a 2046 616c 7365 2c20 2769 6427  df': False, 'id'
-000035a0: 3a20 3331 3937 3738 302c 2027 6e61 6d65  : 3197780, 'name
-000035b0: 273a 2027 4c69 6d69 7465 6420 5061 7274  ': 'Limited Part
-000035c0: 6e65 7227 2c20 2765 6e74 7279 4c69 7374  ner', 'entryList
-000035d0: 4964 273a 202d 367d 5d20 2020 207c 0a0a  Id': -6}]    |..
-000035e0: 546f 2072 6574 7572 6e20 6120 7079 7468  To return a pyth
-000035f0: 6f6e 2060 6c69 7374 6020 696e 7374 6561  on `list` instea
-00003600: 6420 6f66 2061 2060 7061 6e64 6173 2e44  d of a `pandas.D
-00003610: 6174 6146 7261 6d65 603a 0a0a 6060 6070  ataFrame`:..```p
-00003620: 7974 686f 6e0a 6672 6f6d 2064 6561 6c63  ython.from dealc
-00003630: 6c6f 7564 5f73 646b 2069 6d70 6f72 7420  loud_sdk import 
-00003640: 4465 616c 436c 6f75 640a 0a64 6320 3d20  DealCloud..dc = 
-00003650: 4465 616c 436c 6f75 642e 6672 6f6d 5f79  DealCloud.from_y
-00003660: 616d 6c28 2270 6174 682f 746f 2f79 616d  aml("path/to/yam
-00003670: 6c5f 636f 6e66 6967 5f66 696c 652e 6a73  l_config_file.js
-00003680: 6f6e 2229 0a0a 6461 7461 203d 2064 632e  on")..data = dc.
-00003690: 7265 6164 5f64 6174 6128 2243 6f6d 7061  read_data("Compa
-000036a0: 6e79 222c 206f 7574 7075 743d 226c 6973  ny", output="lis
-000036b0: 7422 290a 6060 600a 6064 6174 6160 2077  t").```.`data` w
-000036c0: 696c 6c20 6265 2061 2060 6c69 7374 6020  ill be a `list` 
-000036d0: 6f66 2060 6469 6374 6073 2061 7320 6265  of `dict`s as be
-000036e0: 6c6f 773a 0a60 6060 7079 7468 6f6e 0a5b  low:.```python.[
-000036f0: 0a20 2020 207b 0a20 2020 2020 2020 2027  .    {.        '
-00003700: 456e 7472 7949 6427 3a20 3132 3334 352c  EntryId': 12345,
-00003710: 0a20 2020 2020 2020 2027 436f 6d70 616e  .        'Compan
-00003720: 794e 616d 6527 3a20 2743 6f6d 7061 6e79  yName': 'Company
-00003730: 3127 2c0a 2020 2020 2020 2020 2743 6f6d  1',.        'Com
-00003740: 7061 6e79 5479 7065 273a 205b 0a20 2020  panyType': [.   
-00003750: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00003760: 2020 2020 2020 2020 2020 2020 2773 6571              'seq
-00003770: 4e75 6d62 6572 273a 2033 2c0a 2020 2020  Number': 3,.    
-00003780: 2020 2020 2020 2020 2020 2020 2769 7341              'isA
-00003790: 7574 6f50 6466 273a 2046 616c 7365 2c0a  utoPdf': False,.
-000037a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037b0: 2769 6427 3a20 3331 3937 3738 302c 0a20  'id': 3197780,. 
-000037c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000037d0: 6e61 6d65 273a 2027 4c69 6d69 7465 6420  name': 'Limited 
-000037e0: 5061 7274 6e65 7227 2c0a 2020 2020 2020  Partner',.      
-000037f0: 2020 2020 2020 2020 2020 2765 6e74 7279            'entry
-00003800: 4c69 7374 4964 273a 202d 360a 2020 2020  ListId': -6.    
-00003810: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00003820: 2020 5d2c 0a20 2020 207d 2c0a 2020 2020    ],.    },.    
-00003830: 7b0a 2020 2020 2020 2745 6e74 7279 4964  {.      'EntryId
-00003840: 273a 2031 3233 3436 2c0a 2020 2020 2020  ': 12346,.      
-00003850: 2743 6f6d 7061 6e79 4e61 6d65 273a 2027  'CompanyName': '
-00003860: 436f 6d70 616e 7932 272c 0a20 2020 2020  Company2',.     
-00003870: 2027 436f 6d70 616e 7954 7970 6527 3a20   'CompanyType': 
-00003880: 5b0a 2020 2020 2020 2020 207b 0a20 2020  [.         {.   
-00003890: 2020 2020 2020 2020 2027 7365 714e 756d           'seqNum
-000038a0: 6265 7227 3a20 312c 0a20 2020 2020 2020  ber': 1,.       
-000038b0: 2020 2020 2027 6973 4175 746f 5064 6627       'isAutoPdf'
-000038c0: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
-000038d0: 2020 2020 2027 6964 273a 2033 3139 3737       'id': 31977
-000038e0: 3832 2c0a 2020 2020 2020 2020 2020 2020  82,.            
-000038f0: 276e 616d 6527 3a20 274f 7065 7261 7469  'name': 'Operati
-00003900: 6e67 2043 6f6d 7061 6e79 272c 0a20 2020  ng Company',.   
-00003910: 2020 2020 2020 2020 2027 656e 7472 794c           'entryL
-00003920: 6973 7449 6427 3a20 2d36 0a20 2020 2020  istId': -6.     
-00003930: 2020 2020 7d0a 2020 2020 2020 5d0a 2020      }.      ].  
-00003940: 2020 7d2c 0a20 2020 207b 0a20 2020 2020    },.    {.     
-00003950: 2020 2745 6e74 7279 4964 273a 2031 3233    'EntryId': 123
-00003960: 3437 2c0a 2020 2020 2020 2020 2743 6f6d  47,.        'Com
-00003970: 7061 6e79 4e61 6d65 273a 2027 436f 6d70  panyName': 'Comp
-00003980: 616e 7933 272c 0a20 2020 2020 2020 2027  any3',.        '
-00003990: 436f 6d70 616e 7954 7970 6527 3a20 5b0a  CompanyType': [.
-000039a0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
-000039b0: 2020 2020 2020 2020 2020 2020 2027 7365               'se
-000039c0: 714e 756d 6265 7227 3a20 342c 0a20 2020  qNumber': 4,.   
-000039d0: 2020 2020 2020 2020 2020 2020 2027 6973               'is
-000039e0: 4175 746f 5064 6627 3a20 4661 6c73 652c  AutoPdf': False,
-000039f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003a00: 2027 6964 273a 2033 3139 3737 3739 2c0a   'id': 3197779,.
-00003a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a20: 276e 616d 6527 3a20 2753 6572 7669 6365  'name': 'Service
-00003a30: 2050 726f 7669 6465 7227 2c0a 2020 2020   Provider',.    
-00003a40: 2020 2020 2020 2020 2020 2020 2765 6e74              'ent
-00003a50: 7279 4c69 7374 4964 273a 202d 360a 2020  ryListId': -6.  
-00003a60: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00003a70: 2020 205d 0a20 2020 207d 2c0a 205d 0a60     ].    },. ].`
-00003a80: 6060 0a0a 2323 2323 2320 5265 736f 6c76  ``..##### Resolv
-00003a90: 696e 6720 746f 204e 616d 6520 6f72 2074  ing to Name or t
-00003aa0: 6f20 4944 0a3e 205b 214e 4f54 455d 0a3e  o ID.> [!NOTE].>
-00003ab0: 2054 6865 2066 6f6c 6c6f 7769 6e67 206d   The following m
-00003ac0: 6574 686f 6473 206f 6e6c 7920 6170 706c  ethods only appl
-00003ad0: 7920 746f 2077 6865 7265 2061 2060 7061  y to where a `pa
-00003ae0: 6e64 6173 2e44 6174 6146 7261 6d65 6020  ndas.DataFrame` 
-00003af0: 6973 2072 6574 7572 6e65 642e 0a0a 4368  is returned...Ch
-00003b00: 6f69 6365 2c20 5265 6665 7265 6e63 6520  oice, Reference 
-00003b10: 616e 6420 5573 6572 2066 6965 6c64 7320  and User fields 
-00003b20: 6170 7065 6172 2061 7320 6c69 7374 7320  appear as lists 
-00003b30: 6f66 2064 6963 7469 6f6e 6172 6965 7320  of dictionaries 
-00003b40: 6173 2073 6565 6e20 696e 2074 6865 205b  as seen in the [
-00003b50: 6162 6f76 6520 6578 616d 706c 655d 2823  above example](#
-00003b60: 7265 6164 696e 672d 6461 7461 2d66 726f  reading-data-fro
-00003b70: 6d2d 616e 2d6f 626a 6563 7429 2062 7920  m-an-object) by 
-00003b80: 6465 6661 756c 742e 0a0a 546f 2072 6573  default...To res
-00003b90: 6f6c 7665 2074 6865 7365 2066 6965 6c64  olve these field
-00003ba0: 7320 746f 2061 206d 6f72 6520 7265 6164  s to a more read
-00003bb0: 6162 6c65 2060 6e61 6d65 6020 7661 6c75  able `name` valu
-00003bc0: 653a 0a0a 6060 6070 7974 686f 6e0a 6672  e:..```python.fr
-00003bd0: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
-00003be0: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
-00003bf0: 640a 0a64 6320 3d20 4465 616c 436c 6f75  d..dc = DealClou
-00003c00: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
-00003c10: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
-00003c20: 5f66 696c 652e 6a73 6f6e 2229 0a0a 6461  _file.json")..da
-00003c30: 7461 203d 2064 632e 7265 6164 5f64 6174  ta = dc.read_dat
-00003c40: 6128 2243 6f6d 7061 6e79 222c 2072 6573  a("Company", res
-00003c50: 6f6c 7665 3d22 6e61 6d65 2229 0a60 6060  olve="name").```
-00003c60: 0a60 6461 7461 6020 7769 6c6c 2062 6520  .`data` will be 
-00003c70: 6120 6070 616e 6461 732e 4461 7461 4672  a `pandas.DataFr
-00003c80: 616d 6560 2061 7320 6265 6c6f 773a 0a0a  ame` as below:..
-00003c90: 7c20 456e 7472 7949 6420 7c20 436f 6d70  | EntryId | Comp
-00003ca0: 616e 794e 616d 6520 7c20 436f 6d70 616e  anyName | Compan
-00003cb0: 7954 7970 6520 2020 2020 2020 207c 0a7c  yType        |.|
-00003cc0: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
-00003cd0: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00003ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20  ------------|.| 
-00003cf0: 3132 3334 3520 2020 7c20 436f 6d70 616e  12345   | Compan
-00003d00: 7931 2020 2020 7c20 4c69 6d69 7465 6420  y1    | Limited 
-00003d10: 5061 7274 6e65 7220 2020 207c 0a7c 2031  Partner    |.| 1
-00003d20: 3233 3436 2020 207c 2043 6f6d 7061 6e79  2346   | Company
-00003d30: 3220 2020 207c 204f 7065 7261 7469 6e67  2    | Operating
-00003d40: 2043 6f6d 7061 6e79 2020 7c0a 7c20 3132   Company  |.| 12
-00003d50: 3334 3720 2020 7c20 436f 6d70 616e 7933  347   | Company3
-00003d60: 2020 2020 7c20 4c69 6d69 7465 6420 5061      | Limited Pa
-00003d70: 7274 6e65 7220 2020 207c 0a0a 546f 2072  rtner    |..To r
-00003d80: 6573 6f6c 7665 2074 6865 2066 6965 6c64  esolve the field
-00003d90: 7320 746f 2061 6e20 6069 6460 2076 616c  s to an `id` val
-00003da0: 7565 3a0a 0a60 6060 7079 7468 6f6e 0a66  ue:..```python.f
-00003db0: 726f 6d20 6465 616c 636c 6f75 645f 7364  rom dealcloud_sd
-00003dc0: 6b20 696d 706f 7274 2044 6561 6c43 6c6f  k import DealClo
-00003dd0: 7564 0a0a 6463 203d 2044 6561 6c43 6c6f  ud..dc = DealClo
-00003de0: 7564 2e66 726f 6d5f 7961 6d6c 2822 7061  ud.from_yaml("pa
-00003df0: 7468 2f74 6f2f 7961 6d6c 5f63 6f6e 6669  th/to/yaml_confi
-00003e00: 675f 6669 6c65 2e6a 736f 6e22 290a 0a64  g_file.json")..d
-00003e10: 6174 6120 3d20 6463 2e72 6561 645f 6461  ata = dc.read_da
-00003e20: 7461 2822 436f 6d70 616e 7922 2c20 7265  ta("Company", re
-00003e30: 736f 6c76 653d 2269 6422 290a 6060 600a  solve="id").```.
-00003e40: 6064 6174 6160 2077 696c 6c20 6265 2061  `data` will be a
-00003e50: 2060 7061 6e64 6173 2e44 6174 6146 7261   `pandas.DataFra
-00003e60: 6d65 6020 6173 2062 656c 6f77 3a0a 0a7c  me` as below:..|
-00003e70: 2045 6e74 7279 4964 207c 2043 6f6d 7061   EntryId | Compa
-00003e80: 6e79 4e61 6d65 207c 2043 6f6d 7061 6e79  nyName | Company
-00003e90: 5479 7065 207c 0a7c 2d2d 2d2d 2d2d 2d2d  Type |.|--------
-00003ea0: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  -|-------------|
-00003eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c  -------------|.|
-00003ec0: 2031 3233 3435 2020 207c 2043 6f6d 7061   12345   | Compa
-00003ed0: 6e79 3120 2020 207c 2033 3139 3737 3830  ny1    | 3197780
-00003ee0: 2020 2020 207c 0a7c 2031 3233 3436 2020       |.| 12346  
-00003ef0: 207c 2043 6f6d 7061 6e79 3220 2020 207c   | Company2    |
-00003f00: 2033 3139 3737 3832 2020 2020 207c 0a7c   3197782     |.|
-00003f10: 2031 3233 3437 2020 207c 2043 6f6d 7061   12347   | Compa
-00003f20: 6e79 3320 2020 207c 2033 3139 3737 3830  ny3    | 3197780
-00003f30: 2020 2020 207c 0a0a 2323 2323 2320 5265       |..##### Re
-00003f40: 6164 696e 6720 6120 5375 6273 6574 206f  ading a Subset o
-00003f50: 6620 4669 656c 6473 0a54 6f20 7265 6164  f Fields.To read
-00003f60: 2061 2073 7065 6369 6669 6320 7365 7420   a specific set 
-00003f70: 6f66 2066 6965 6c64 7320 6672 6f6d 2061  of fields from a
-00003f80: 6e20 6f62 6a65 6374 2c20 7061 7373 2061  n object, pass a
-00003f90: 206c 6973 7420 6f66 2044 6561 6c43 6c6f   list of DealClo
-00003fa0: 7564 2066 6965 6c64 2041 5049 206e 616d  ud field API nam
-00003fb0: 6573 2074 6f20 7468 6520 6172 6775 6d65  es to the argume
-00003fc0: 6e74 2060 6669 656c 6473 603a 0a0a 6060  nt `fields`:..``
-00003fd0: 6070 7974 686f 6e0a 6672 6f6d 2064 6561  `python.from dea
-00003fe0: 6c63 6c6f 7564 5f73 646b 2069 6d70 6f72  lcloud_sdk impor
-00003ff0: 7420 4465 616c 436c 6f75 640a 0a64 6320  t DealCloud..dc 
-00004000: 3d20 4465 616c 436c 6f75 642e 6672 6f6d  = DealCloud.from
-00004010: 5f79 616d 6c28 2270 6174 682f 746f 2f79  _yaml("path/to/y
-00004020: 616d 6c5f 636f 6e66 6967 5f66 696c 652e  aml_config_file.
-00004030: 6a73 6f6e 2229 0a0a 6461 7461 203d 2064  json")..data = d
-00004040: 632e 7265 6164 5f64 6174 6128 2243 6f6d  c.read_data("Com
-00004050: 7061 6e79 222c 2066 6965 6c64 733d 5b22  pany", fields=["
-00004060: 436f 6d70 616e 794e 616d 6522 5d29 0a60  CompanyName"]).`
-00004070: 6060 0a60 6461 7461 6020 7769 6c6c 2062  ``.`data` will b
-00004080: 6520 6120 6070 616e 6461 732e 4461 7461  e a `pandas.Data
-00004090: 4672 616d 6560 2061 7320 6265 6c6f 773a  Frame` as below:
-000040a0: 0a0a 7c20 456e 7472 7949 6420 7c20 436f  ..| EntryId | Co
-000040b0: 6d70 616e 794e 616d 6520 7c0a 7c2d 2d2d  mpanyName |.|---
-000040c0: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-000040d0: 2d2d 2d2d 7c0a 7c20 3132 3334 3520 2020  ----|.| 12345   
-000040e0: 7c20 436f 6d70 616e 7931 2020 2020 7c0a  | Company1    |.
-000040f0: 7c20 3132 3334 3620 2020 7c20 436f 6d70  | 12346   | Comp
-00004100: 616e 7932 2020 2020 7c0a 7c20 3132 3334  any2    |.| 1234
-00004110: 3720 2020 7c20 436f 6d70 616e 7933 2020  7   | Company3  
-00004120: 2020 7c0a 0a23 2323 2323 2055 7369 6e67    |..##### Using
-00004130: 2051 7565 7269 6573 2074 6f20 5265 6164   Queries to Read
-00004140: 2044 6174 610a 4120 7175 6572 7920 6361   Data.A query ca
-00004150: 6e20 6265 2070 6173 7365 6420 746f 2074  n be passed to t
-00004160: 6865 2044 6561 6c43 6c6f 7564 2072 6571  he DealCloud req
-00004170: 7565 7374 2066 6f72 2064 6174 6120 746f  uest for data to
-00004180: 2072 6574 7572 6e20 6d6f 7265 2073 7065   return more spe
-00004190: 6369 6669 6320 696e 666f 726d 6174 696f  cific informatio
-000041a0: 6e2c 2061 6e64 2072 6564 7563 6520 7468  n, and reduce th
-000041b0: 6520 766f 6c75 6d65 206f 6620 696e 636f  e volume of inco
-000041c0: 6d69 6e67 2064 6174 612e 0a54 6f20 7573  ming data..To us
-000041d0: 6520 6120 7175 6572 792c 2070 6173 7320  e a query, pass 
-000041e0: 7468 6520 7175 6572 7920 7374 7269 6e67  the query string
-000041f0: 2074 6f20 7468 6520 6071 7565 7279 6020   to the `query` 
-00004200: 6172 6775 6d65 6e74 2e0a 5468 6520 6176  argument..The av
-00004210: 6169 6c61 626c 6520 7175 6572 7920 6f70  ailable query op
-00004220: 6572 6174 696f 6e73 2061 7265 2062 656c  erations are bel
-00004230: 6f77 3a0a 0a7c 204e 616d 6520 2020 2020  ow:..| Name     
-00004240: 2020 2020 2020 7c20 5175 6572 7920 4f70        | Query Op
-00004250: 6572 6174 696f 6e20 7c0a 7c2d 2d2d 2d2d  eration |.|-----
-00004260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  -----------|----
-00004270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c  -------------|.|
-00004280: 2045 7175 616c 7320 2020 2020 2020 2020   Equals         
-00004290: 7c20 2465 7120 2020 2020 2020 2020 2020  | $eq           
-000042a0: 2020 7c0a 7c20 436f 6e74 6169 6e73 2020    |.| Contains  
-000042b0: 2020 2020 207c 2024 636f 6e74 6169 6e73       | $contains
-000042c0: 2020 2020 2020 207c 0a7c 2047 7265 6174         |.| Great
-000042d0: 6572 2020 2020 2020 2020 7c20 2467 7420  er        | $gt 
-000042e0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-000042f0: 4772 6561 7465 724f 7245 7175 616c 207c  GreaterOrEqual |
-00004300: 2024 6774 6520 2020 2020 2020 2020 2020   $gte           
-00004310: 207c 0a7c 204c 6573 7320 2020 2020 2020   |.| Less       
-00004320: 2020 2020 7c20 246c 7420 2020 2020 2020      | $lt       
-00004330: 2020 2020 2020 7c0a 7c20 4c65 7373 4f72        |.| LessOr
-00004340: 4571 7561 6c73 2020 207c 2024 6c74 6520  Equals   | $lte 
-00004350: 2020 2020 2020 2020 2020 207c 0a7c 2053             |.| S
-00004360: 7461 7274 7357 6974 6820 2020 2020 7c20  tartsWith     | 
-00004370: 2473 7461 7274 7377 6974 6820 2020 2020  $startswith     
-00004380: 7c0a 7c20 496e 2020 2020 2020 2020 2020  |.| In          
-00004390: 2020 207c 2024 696e 2020 2020 2020 2020     | $in        
-000043a0: 2020 2020 207c 0a7c 2042 6574 7765 656e       |.| Between
-000043b0: 2020 2020 2020 2020 7c20 2462 6574 7765          | $betwe
-000043c0: 656e 2020 2020 2020 2020 7c0a 7c20 4e6f  en        |.| No
-000043d0: 7449 6e20 2020 2020 2020 2020 207c 2024  tIn          | $
-000043e0: 6e69 6e20 2020 2020 2020 2020 2020 207c  nin            |
-000043f0: 0a7c 204e 6f74 4571 7561 6c54 6f20 2020  .| NotEqualTo   
-00004400: 2020 7c20 246e 6f74 2020 2020 2020 2020    | $not        
-00004410: 2020 2020 7c0a 7c20 456e 6473 5769 7468      |.| EndsWith
-00004420: 2020 2020 2020 207c 2024 656e 6473 7769         | $endswi
-00004430: 7468 2020 2020 2020 207c 0a7c 204f 7220  th       |.| Or 
-00004440: 2020 2020 2020 2020 2020 2020 7c20 246f              | $o
-00004450: 7220 2020 2020 2020 2020 2020 2020 7c0a  r             |.
-00004460: 7c20 416e 6420 2020 2020 2020 2020 2020  | And           
-00004470: 207c 2024 616e 6420 2020 2020 2020 2020   | $and         
-00004480: 2020 207c 0a0a 6060 6070 7974 686f 6e0a     |..```python.
-00004490: 6672 6f6d 2064 6561 6c63 6c6f 7564 5f73  from dealcloud_s
-000044a0: 646b 2069 6d70 6f72 7420 4465 616c 436c  dk import DealCl
-000044b0: 6f75 640a 0a64 6320 3d20 4465 616c 436c  oud..dc = DealCl
-000044c0: 6f75 642e 6672 6f6d 5f79 616d 6c28 2270  oud.from_yaml("p
-000044d0: 6174 682f 746f 2f79 616d 6c5f 636f 6e66  ath/to/yaml_conf
-000044e0: 6967 5f66 696c 652e 6a73 6f6e 2229 0a0a  ig_file.json")..
-000044f0: 6463 2e72 6561 645f 6461 7461 2822 436f  dc.read_data("Co
-00004500: 6d70 616e 7922 2c20 7175 6572 793d 227b  mpany", query="{
-00004510: 436f 6d70 616e 794e 616d 653a 207b 2463  CompanyName: {$c
-00004520: 6f6e 7461 696e 733a 205c 2231 5c22 7d7d  ontains: \"1\"}}
-00004530: 2229 0a60 6060 0a60 6461 7461 6020 7769  ").```.`data` wi
-00004540: 6c6c 2062 6520 6120 6070 616e 6461 732e  ll be a `pandas.
-00004550: 4461 7461 4672 616d 6560 2061 7320 6265  DataFrame` as be
-00004560: 6c6f 773a 0a0a 7c20 456e 7472 7949 6420  low:..| EntryId 
-00004570: 7c20 436f 6d70 616e 794e 616d 6520 7c20  | CompanyName | 
-00004580: 436f 6d70 616e 7954 7970 6520 7c0a 7c2d  CompanyType |.|-
-00004590: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
-000045a0: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-000045b0: 2d2d 2d2d 7c0a 7c20 3132 3334 3520 2020  ----|.| 12345   
-000045c0: 7c20 436f 6d70 616e 7931 2020 2020 7c20  | Company1    | 
-000045d0: 3331 3937 3738 3020 2020 2020 7c0a 0a53  3197780     |..S
-000045e0: 6f6d 6520 6f74 6865 7220 6578 616d 706c  ome other exampl
-000045f0: 6520 7175 6572 7920 7374 7269 6e67 7320  e query strings 
-00004600: 6172 6520 6265 6c6f 773a 0a46 696c 7465  are below:.Filte
-00004610: 7220 6f6e 2065 7863 6c75 6469 6e67 2072  r on excluding r
-00004620: 6563 6f72 6473 2077 6974 6820 6120 7370  ecords with a sp
-00004630: 6563 6966 6963 2072 6566 6572 656e 6365  ecific reference
-00004640: 2076 616c 7565 3a0a 0a60 6060 7079 7468   value:..```pyth
-00004650: 6f6e 0a66 726f 6d20 6465 616c 636c 6f75  on.from dealclou
-00004660: 645f 7364 6b20 696d 706f 7274 2044 6561  d_sdk import Dea
-00004670: 6c43 6c6f 7564 0a0a 6463 203d 2044 6561  lCloud..dc = Dea
-00004680: 6c43 6c6f 7564 2e66 726f 6d5f 7961 6d6c  lCloud.from_yaml
-00004690: 2822 7061 7468 2f74 6f2f 7961 6d6c 5f63  ("path/to/yaml_c
-000046a0: 6f6e 6669 675f 6669 6c65 2e6a 736f 6e22  onfig_file.json"
-000046b0: 290a 0a64 632e 7265 6164 5f64 6174 6128  )..dc.read_data(
-000046c0: 2243 6f6d 7061 6e79 222c 2071 7565 7279  "Company", query
-000046d0: 3d22 7b43 6f76 6572 6167 6550 6572 736f  ="{CoveragePerso
-000046e0: 6e3a 207b 246e 696e 3a20 5b35 3738 355d  n: {$nin: [5785]
-000046f0: 7d22 290a 6060 600a 4669 6c74 6572 2075  }").```.Filter u
-00004700: 7369 6e67 204f 723a 0a0a 6060 6070 7974  sing Or:..```pyt
-00004710: 686f 6e0a 6672 6f6d 2064 6561 6c63 6c6f  hon.from dealclo
-00004720: 7564 5f73 646b 2069 6d70 6f72 7420 4465  ud_sdk import De
-00004730: 616c 436c 6f75 640a 0a64 6320 3d20 4465  alCloud..dc = De
-00004740: 616c 436c 6f75 642e 6672 6f6d 5f79 616d  alCloud.from_yam
-00004750: 6c28 2270 6174 682f 746f 2f79 616d 6c5f  l("path/to/yaml_
-00004760: 636f 6e66 6967 5f66 696c 652e 6a73 6f6e  config_file.json
-00004770: 2229 0a0a 6463 2e72 6561 645f 6461 7461  ")..dc.read_data
-00004780: 2822 436f 6d70 616e 7922 2c20 7175 6572  ("Company", quer
-00004790: 793d 227b 246f 723a 205b 7b43 6f6d 7061  y="{$or: [{Compa
-000047a0: 6e79 4e61 6d65 3a20 5c22 4465 616c 436c  nyName: \"DealCl
-000047b0: 6f75 645c 227d 2c7b 436f 6d70 616e 794e  oud\"},{CompanyN
-000047c0: 616d 653a 205c 2241 5049 2045 6e74 7279  ame: \"API Entry
-000047d0: 5c22 7d5d 7d22 290a 6060 600a 0a23 2323  \"}]}").```..###
-000047e0: 2320 5265 6164 696e 6720 4461 7461 2066  # Reading Data f
-000047f0: 726f 6d20 6120 5669 6577 0a54 6f20 7265  rom a View.To re
-00004800: 6164 2064 6174 6120 6672 6f6d 2061 2076  ad data from a v
-00004810: 6965 7720 7769 7468 2049 443a 2060 3132  iew with ID: `12
-00004820: 3334 3560 0a0a 4578 616d 706c 653a 0a0a  345`..Example:..
-00004830: 6060 6070 7974 686f 6e0a 6672 6f6d 2064  ```python.from d
-00004840: 6561 6c63 6c6f 7564 5f73 646b 2069 6d70  ealcloud_sdk imp
-00004850: 6f72 7420 4465 616c 436c 6f75 640a 0a64  ort DealCloud..d
-00004860: 6320 3d20 4465 616c 436c 6f75 642e 6672  c = DealCloud.fr
-00004870: 6f6d 5f79 616d 6c28 2270 6174 682f 746f  om_yaml("path/to
-00004880: 2f79 616d 6c5f 636f 6e66 6967 5f66 696c  /yaml_config_fil
-00004890: 652e 6a73 6f6e 2229 0a0a 6461 7461 203d  e.json")..data =
-000048a0: 2064 632e 7265 6164 5f64 6174 6128 7669   dc.read_data(vi
-000048b0: 6577 5f69 643d 3132 3334 3529 0a60 6060  ew_id=12345).```
-000048c0: 0a41 6c74 6572 6e61 7469 7665 6c79 2c20  .Alternatively, 
-000048d0: 6966 2074 6865 2076 6965 7720 6973 206e  if the view is n
-000048e0: 616d 6564 3a20 224d 7920 436f 6d70 616e  amed: "My Compan
-000048f0: 7920 5669 6577 223a 0a0a 6060 6070 7974  y View":..```pyt
-00004900: 686f 6e0a 6672 6f6d 2064 6561 6c63 6c6f  hon.from dealclo
-00004910: 7564 5f73 646b 2069 6d70 6f72 7420 4465  ud_sdk import De
-00004920: 616c 436c 6f75 640a 0a64 6320 3d20 4465  alCloud..dc = De
-00004930: 616c 436c 6f75 642e 6672 6f6d 5f79 616d  alCloud.from_yam
-00004940: 6c28 2270 6174 682f 746f 2f79 616d 6c5f  l("path/to/yaml_
-00004950: 636f 6e66 6967 5f66 696c 652e 6a73 6f6e  config_file.json
-00004960: 2229 0a0a 6461 7461 203d 2064 632e 7265  ")..data = dc.re
-00004970: 6164 5f64 6174 6128 7669 6577 5f69 643d  ad_data(view_id=
-00004980: 224d 7920 436f 6d70 616e 7920 5669 6577  "My Company View
-00004990: 2229 0a60 6060 0a0a 6064 6174 6160 2077  ").```..`data` w
-000049a0: 696c 6c20 6265 2061 2060 7061 6e64 6173  ill be a `pandas
-000049b0: 2e44 6174 6146 7261 6d65 6020 6173 2062  .DataFrame` as b
-000049c0: 656c 6f77 3a0a 0a7c 2045 6e74 7279 4964  elow:..| EntryId
-000049d0: 207c 2043 6f6d 7061 6e79 4e61 6d65 207c   | CompanyName |
-000049e0: 2043 6f6d 7061 6e79 5479 7065 2020 2020   CompanyType    
-000049f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a40: 2020 2020 2020 2020 7c0a 7c2d 2d2d 2d2d          |.|-----
-00004a50: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
-00004a60: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|-------------
-00004a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2031  -----------|.| 1
-00004ad0: 3233 3435 2020 207c 2043 6f6d 7061 6e79  2345   | Company
-00004ae0: 3120 2020 207c 205b 7b27 7365 714e 756d  1    | [{'seqNum
-00004af0: 6265 7227 3a20 332c 2027 6973 4175 746f  ber': 3, 'isAuto
-00004b00: 5064 6627 3a20 4661 6c73 652c 2027 6964  Pdf': False, 'id
-00004b10: 273a 2033 3139 3737 3830 2c20 276e 616d  ': 3197780, 'nam
-00004b20: 6527 3a20 274c 696d 6974 6564 2050 6172  e': 'Limited Par
-00004b30: 746e 6572 272c 2027 656e 7472 794c 6973  tner', 'entryLis
-00004b40: 7449 6427 3a20 2d36 7d5d 2020 2020 7c0a  tId': -6}]    |.
-00004b50: 7c20 3132 3334 3620 2020 7c20 436f 6d70  | 12346   | Comp
-00004b60: 616e 7932 2020 2020 7c20 5b7b 2773 6571  any2    | [{'seq
-00004b70: 4e75 6d62 6572 273a 2031 2c20 2769 7341  Number': 1, 'isA
-00004b80: 7574 6f50 6466 273a 2046 616c 7365 2c20  utoPdf': False, 
-00004b90: 2769 6427 3a20 3331 3937 3738 322c 2027  'id': 3197782, '
-00004ba0: 6e61 6d65 273a 2027 4f70 6572 6174 696e  name': 'Operatin
-00004bb0: 6720 436f 6d70 616e 7927 2c20 2765 6e74  g Company', 'ent
-00004bc0: 7279 4c69 7374 4964 273a 202d 367d 5d20  ryListId': -6}] 
-00004bd0: 207c 0a7c 2031 3233 3437 2020 207c 2043   |.| 12347   | C
-00004be0: 6f6d 7061 6e79 3320 2020 207c 205b 7b27  ompany3    | [{'
-00004bf0: 7365 714e 756d 6265 7227 3a20 332c 2027  seqNumber': 3, '
-00004c00: 6973 4175 746f 5064 6627 3a20 4661 6c73  isAutoPdf': Fals
-00004c10: 652c 2027 6964 273a 2033 3139 3737 3830  e, 'id': 3197780
-00004c20: 2c20 276e 616d 6527 3a20 274c 696d 6974  , 'name': 'Limit
-00004c30: 6564 2050 6172 746e 6572 272c 2027 656e  ed Partner', 'en
-00004c40: 7472 794c 6973 7449 6427 3a20 2d36 7d5d  tryListId': -6}]
-00004c50: 2020 2020 7c0a 0a23 2323 2323 2055 7369      |..##### Usi
-00004c60: 6e67 2061 2046 696c 7465 7220 5768 656e  ng a Filter When
-00004c70: 2052 6561 6469 6e67 2056 6965 7720 4461   Reading View Da
-00004c80: 7461 0a57 6865 6e20 7265 6164 696e 6720  ta.When reading 
-00004c90: 6461 7461 2066 726f 6d20 6120 7669 6577  data from a view
-00004ca0: 2c20 7768 6963 6820 6861 7320 2253 7570  , which has "Sup
-00004cb0: 706c 7920 5661 6c75 6520 4c61 7465 7222  ply Value Later"
-00004cc0: 2066 696c 7465 7273 2063 6f6e 6669 6775   filters configu
-00004cd0: 7265 642c 2074 6865 2066 696c 7465 7220  red, the filter 
-00004ce0: 7661 6c75 6573 2063 616e 2062 6520 7072  values can be pr
-00004cf0: 6f76 6964 6564 2062 7920 7061 7373 696e  ovided by passin
-00004d00: 6720 7468 656d 2074 6f20 7468 6520 6076  g them to the `v
-00004d10: 6965 775f 6669 6c74 6572 6020 6172 6775  iew_filter` argu
-00004d20: 6d65 6e74 2069 6e20 6120 606c 6973 7460  ment in a `list`
-00004d30: 206f 6620 6064 6963 7460 732e 2046 6f72   of `dict`s. For
-00004d40: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-00004d50: 6e20 6f6e 2074 6865 6972 2066 6f72 6d61  n on their forma
-00004d60: 742c 2070 6c65 6173 6520 7365 6520 7468  t, please see th
-00004d70: 6520 5b41 5049 2044 6f63 756d 656e 7461  e [API Documenta
-00004d80: 7469 6f6e 5d28 6874 7470 733a 2f2f 6170  tion](https://ap
-00004d90: 692e 646f 6373 2e64 6561 6c63 6c6f 7564  i.docs.dealcloud
-00004da0: 2e63 6f6d 2f64 6f63 732f 6461 7461 2f72  .com/docs/data/r
-00004db0: 6f77 732f 7669 6577 5f64 6574 6169 6c73  ows/view_details
-00004dc0: 292e 0a0a 466f 7220 4578 616d 706c 652c  )...For Example,
-00004dd0: 2073 7570 706c 7969 6e67 2061 2022 436f   supplying a "Co
-00004de0: 6d70 616e 7954 7970 6522 2066 696c 7465  mpanyType" filte
-00004df0: 7220 7661 6c75 6520 746f 2066 696c 7465  r value to filte
-00004e00: 7220 666f 7220 6f6e 6c79 2022 4c69 6d69  r for only "Limi
-00004e10: 7465 6420 5061 7274 6e65 7222 2063 6f6d  ted Partner" com
-00004e20: 7061 6e69 6573 3a0a 0a60 6060 7079 7468  panies:..```pyth
-00004e30: 6f6e 0a66 726f 6d20 6465 616c 636c 6f75  on.from dealclou
-00004e40: 645f 7364 6b20 696d 706f 7274 2044 6561  d_sdk import Dea
-00004e50: 6c43 6c6f 7564 0a0a 6463 203d 2044 6561  lCloud..dc = Dea
-00004e60: 6c43 6c6f 7564 2e66 726f 6d5f 7961 6d6c  lCloud.from_yaml
-00004e70: 2822 7061 7468 2f74 6f2f 7961 6d6c 5f63  ("path/to/yaml_c
-00004e80: 6f6e 6669 675f 6669 6c65 2e6a 736f 6e22  onfig_file.json"
-00004e90: 290a 0a64 6174 6120 3d20 6463 2e72 6561  )..data = dc.rea
-00004ea0: 645f 6461 7461 280a 2020 2076 6965 775f  d_data(.   view_
-00004eb0: 6964 203d 2022 4d79 2043 6f6d 7061 6e79  id = "My Company
-00004ec0: 2056 6965 7722 2c0a 2020 2076 6965 775f   View",.   view_
-00004ed0: 6669 6c74 6572 203d 205b 0a20 2020 2020  filter = [.     
-00004ee0: 207b 0a20 2020 2020 2020 2020 2263 6f6c   {.         "col
-00004ef0: 756d 6e22 3a22 436f 6d70 616e 7954 7970  umn":"CompanyTyp
-00004f00: 6522 2c0a 2020 2020 2020 2020 2022 7661  e",.         "va
-00004f10: 6c75 6522 3a20 5b33 3139 3737 3830 5d0a  lue": [3197780].
-00004f20: 2020 2020 2020 7d0a 2020 205d 0a29 0a60        }.   ].).`
-00004f30: 6060 0a60 6461 7461 6020 7769 6c6c 2062  ``.`data` will b
-00004f40: 6520 6120 6070 616e 6461 732e 4461 7461  e a `pandas.Data
-00004f50: 4672 616d 6560 2061 7320 6265 6c6f 773a  Frame` as below:
-00004f60: 0a0a 7c20 456e 7472 7949 6420 7c20 436f  ..| EntryId | Co
-00004f70: 6d70 616e 794e 616d 6520 7c20 436f 6d70  mpanyName | Comp
-00004f80: 616e 7954 7970 6520 2020 2020 2020 2020  anyType         
-00004f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fe0: 2020 207c 0a7c 2d2d 2d2d 2d2d 2d2d 2d7c     |.|---------|
-00004ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -------------|--
-00005000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005060: 2d2d 2d2d 2d2d 7c0a 7c20 3132 3334 3520  ------|.| 12345 
-00005070: 2020 7c20 436f 6d70 616e 7931 2020 2020    | Company1    
-00005080: 7c20 5b7b 2773 6571 4e75 6d62 6572 273a  | [{'seqNumber':
-00005090: 2033 2c20 2769 7341 7574 6f50 6466 273a   3, 'isAutoPdf':
-000050a0: 2046 616c 7365 2c20 2769 6427 3a20 3331   False, 'id': 31
-000050b0: 3937 3738 302c 2027 6e61 6d65 273a 2027  97780, 'name': '
-000050c0: 4c69 6d69 7465 6420 5061 7274 6e65 7227  Limited Partner'
-000050d0: 2c20 2765 6e74 7279 4c69 7374 4964 273a  , 'entryListId':
-000050e0: 202d 367d 5d20 2020 207c 0a7c 2031 3233   -6}]    |.| 123
-000050f0: 3437 2020 207c 2043 6f6d 7061 6e79 3320  47   | Company3 
-00005100: 2020 207c 205b 7b27 7365 714e 756d 6265     | [{'seqNumbe
-00005110: 7227 3a20 332c 2027 6973 4175 746f 5064  r': 3, 'isAutoPd
-00005120: 6627 3a20 4661 6c73 652c 2027 6964 273a  f': False, 'id':
-00005130: 2033 3139 3737 3830 2c20 276e 616d 6527   3197780, 'name'
-00005140: 3a20 274c 696d 6974 6564 2050 6172 746e  : 'Limited Partn
-00005150: 6572 272c 2027 656e 7472 794c 6973 7449  er', 'entryListI
-00005160: 6427 3a20 2d36 7d5d 2020 2020 7c0a 0a0a  d': -6}]    |...
-00005170: 2323 2320 4372 6561 7465 2c20 5570 6461  ### Create, Upda
-00005180: 7465 2061 6e64 2055 7073 6572 7420 4461  te and Upsert Da
-00005190: 7461 0a60 4465 616c 436c 6f75 642e 696e  ta.`DealCloud.in
-000051a0: 7365 7274 5f64 6174 6128 2960 2c20 6044  sert_data()`, `D
-000051b0: 6561 6c43 6c6f 7564 2e75 7064 6174 655f  ealCloud.update_
-000051c0: 6461 7461 2829 602c 2060 4465 616c 436c  data()`, `DealCl
-000051d0: 6f75 642e 7570 7365 7274 5f64 6174 6128  oud.upsert_data(
-000051e0: 2960 2061 7265 206d 6574 686f 6473 2077  )` are methods w
-000051f0: 6869 6368 2070 726f 7669 6465 2074 6865  hich provide the
-00005200: 2061 6269 6c69 7479 2074 6f20 6372 6561   ability to crea
-00005210: 7465 2c20 7570 6461 7465 2061 6e64 2075  te, update and u
-00005220: 7073 6572 7420 6461 7461 2072 6573 7065  psert data respe
-00005230: 6374 6976 656c 792e 0a54 6865 7365 206d  ctively..These m
-00005240: 6574 686f 6473 2068 6176 6520 7468 6520  ethods have the 
-00005250: 7361 6d65 2061 7267 756d 656e 7420 7061  same argument pa
-00005260: 7474 6572 6e3a 0a0a 4172 6775 6d65 6e74  ttern:..Argument
-00005270: 733a 0a2d 206f 626a 6563 745f 6170 695f  s:.- object_api_
-00005280: 6e61 6d65 2060 7374 7260 3a20 7468 6520  name `str`: the 
-00005290: 6f62 6a65 6374 2041 5049 206e 616d 6520  object API name 
-000052a0: 746f 2077 7269 7465 2064 6174 6120 746f  to write data to
-000052b0: 0a2d 2064 6174 6120 6055 6e69 6f6e 5b6c  .- data `Union[l
-000052c0: 6973 745b 6469 6374 5d2c 2070 642e 4461  ist[dict], pd.Da
-000052d0: 7461 4672 616d 655d 603a 2074 6865 2064  taFrame]`: the d
-000052e0: 6174 6120 746f 2062 6520 7365 6e74 2074  ata to be sent t
-000052f0: 6f20 4465 616c 436c 6f75 642e 0a2d 2075  o DealCloud..- u
-00005300: 7365 5f64 6561 6c63 6c6f 7564 5f69 6473  se_dealcloud_ids
-00005310: 2060 626f 6f6c 603a 2044 6566 6175 6c74   `bool`: Default
-00005320: 2069 7320 6054 7275 6560 2049 6620 6054   is `True` If `T
-00005330: 7275 6560 2c20 4465 616c 436c 6f75 6420  rue`, DealCloud 
-00005340: 456e 7472 7949 6473 206d 7573 7420 6265  EntryIds must be
-00005350: 2075 7365 6420 746f 2072 6566 6572 656e   used to referen
-00005360: 6365 2072 6563 6f72 6473 2061 6e64 2063  ce records and c
-00005370: 686f 6963 6520 7661 6c75 6573 2e20 4966  hoice values. If
-00005380: 2060 4661 6c73 6560 2c20 7573 6520 6120   `False`, use a 
-00005390: 636f 6c75 6d6e 2061 7320 6120 6c6f 6f6b  column as a look
-000053a0: 7570 2c20 6465 6669 6e65 6420 6279 2074  up, defined by t
-000053b0: 6865 206c 6f6f 6b75 705f 636f 6c75 6d6e  he lookup_column
-000053c0: 2061 7267 756d 656e 742e 0a2d 206c 6f6f   argument..- loo
-000053d0: 6b75 705f 636f 6c75 6d6e 2060 7374 7260  kup_column `str`
-000053e0: 3a20 6966 2060 7573 655f 6465 616c 636c  : if `use_dealcl
-000053f0: 6f75 645f 6964 7360 2069 7320 6046 616c  oud_ids` is `Fal
-00005400: 7365 602c 2074 6869 7320 6465 6669 6e65  se`, this define
-00005410: 7320 7468 6520 636f 6c75 6d6e 2074 6f20  s the column to 
-00005420: 6265 2075 7365 6420 6173 2061 206c 6f6f  be used as a loo
-00005430: 6b75 702e 0a2d 206f 7574 7075 7460 7374  kup..- output`st
-00005440: 7260 3a20 606c 6973 7460 206f 7220 6070  r`: `list` or `p
-00005450: 616e 6461 7360 2c20 6465 6669 6e65 7320  andas`, defines 
-00005460: 7468 6520 6f75 7470 7574 2066 6f72 6d61  the output forma
-00005470: 7420 7265 7475 726e 6564 2066 726f 6d20  t returned from 
-00005480: 7468 6520 6675 6e63 7469 6f6e 0a0a 5265  the function..Re
-00005490: 7475 726e 733a 0a20 2020 6055 6e69 6f6e  turns:.   `Union
-000054a0: 5b6c 6973 745b 6469 6374 5d2c 2070 642e  [list[dict], pd.
-000054b0: 4461 7461 4672 616d 655d 603a 2074 6865  DataFrame]`: the
-000054c0: 2064 6174 6120 7265 7475 726e 6564 2066   data returned f
-000054d0: 726f 6d20 7468 6520 6461 7461 206f 7065  rom the data ope
-000054e0: 7261 7469 6f6e 2e0a 0a3e 205b 2149 4d50  ration...> [!IMP
-000054f0: 4f52 5441 4e54 5d0a 3e20 5768 656e 206e  ORTANT].> When n
-00005500: 6f74 2075 7369 6e67 2060 7573 655f 6465  ot using `use_de
-00005510: 616c 636c 6f75 645f 6964 7360 2c20 666f  alcloud_ids`, fo
-00005520: 7220 5265 6665 7265 6e63 6520 6669 656c  r Reference fiel
-00005530: 6473 2c20 7265 6665 7265 6e63 6520 6279  ds, reference by
-00005540: 2072 6563 6f72 6420 456e 7472 7949 642e   record EntryId.
-00005550: 2046 6f72 2063 686f 6963 6520 6669 656c   For choice fiel
-00005560: 6473 2c20 7573 6520 7468 6520 6368 6f69  ds, use the choi
-00005570: 6365 2076 616c 7565 2049 442e 2046 6f72  ce value ID. For
-00005580: 2075 7365 7220 6669 656c 6473 2c20 7573   user fields, us
-00005590: 6520 7468 6520 7573 6572 2049 4420 2866  e the user ID (f
-000055a0: 726f 6d20 6044 6561 6c43 6c6f 7564 2e67  rom `DealCloud.g
-000055b0: 6574 5f75 7365 7273 2829 6029 2e20 0a3e  et_users()`). .>
-000055c0: 2057 6865 6e20 7573 696e 6720 6075 7365   When using `use
-000055d0: 5f64 6561 6c63 6c6f 7564 5f69 6473 602c  _dealcloud_ids`,
-000055e0: 2066 6f72 2052 6566 6572 656e 6365 2066   for Reference f
-000055f0: 6965 6c64 732c 2072 6566 6572 656e 6365  ields, reference
-00005600: 2062 7920 7468 6520 6c6f 6f6b 7570 2063   by the lookup c
-00005610: 6f6c 756d 6e20 6f6e 2074 6865 2072 6566  olumn on the ref
-00005620: 6572 656e 6365 6420 6f62 6a65 6374 2e20  erenced object. 
-00005630: 466f 7220 6368 6f69 6365 2066 6965 6c64  For choice field
-00005640: 732c 2075 7365 2074 6865 2063 686f 6963  s, use the choic
-00005650: 6520 6669 656c 6420 6469 7370 6c61 7920  e field display 
-00005660: 6e61 6d65 2e20 466f 7220 7573 6572 2066  name. For user f
-00005670: 6965 6c64 732c 2075 7365 2074 6865 2075  ields, use the u
-00005680: 7365 7220 656d 6169 6c20 6164 6472 6573  ser email addres
-00005690: 732e 0a0a 2323 2323 2320 4669 656c 6420  s...##### Field 
-000056a0: 4d61 7070 696e 670a 416c 6c20 636f 6c75  Mapping.All colu
-000056b0: 6d6e 7320 7061 7373 6564 2074 6f20 7468  mns passed to th
-000056c0: 6520 6372 6561 7465 2c20 7570 6461 7465  e create, update
-000056d0: 2061 6e64 2075 7073 6572 7420 6d65 7468   and upsert meth
-000056e0: 6f64 7320 6d75 7374 206d 6174 6368 2062  ods must match b
-000056f0: 7920 5f41 5049 204e 616d 655f 2e20 4966  y _API Name_. If
-00005700: 2061 2063 6f6c 756d 6e20 7061 7373 6564   a column passed
-00005710: 2074 6f20 7468 6520 6d65 7468 6f64 2064   to the method d
-00005720: 6f65 7320 6e6f 7420 6578 6973 7420 696e  oes not exist in
-00005730: 2074 6865 2073 6974 6520 6279 2041 5049   the site by API
-00005740: 206e 616d 652c 2074 6865 6e20 6120 604b   name, then a `K
-00005750: 6579 4572 726f 7260 2077 696c 6c20 6265  eyError` will be
-00005760: 2072 6169 7365 643a 0a0a 6060 6070 7974   raised:..```pyt
-00005770: 686f 6e0a 6672 6f6d 2064 6561 6c63 6c6f  hon.from dealclo
-00005780: 7564 5f73 646b 2069 6d70 6f72 7420 4465  ud_sdk import De
-00005790: 616c 436c 6f75 640a 0a64 6320 3d20 4465  alCloud..dc = De
-000057a0: 616c 436c 6f75 642e 6672 6f6d 5f79 616d  alCloud.from_yam
-000057b0: 6c28 2270 6174 682f 746f 2f79 616d 6c5f  l("path/to/yaml_
-000057c0: 636f 6e66 6967 5f66 696c 652e 6a73 6f6e  config_file.json
-000057d0: 2229 0a0a 746f 5f73 656e 6420 3d20 5b0a  ")..to_send = [.
-000057e0: 2020 7b0a 2020 2020 2020 2243 6f6d 7061    {.      "Compa
-000057f0: 6e79 4e61 6d65 223a 2022 5465 7374 2043  nyName": "Test C
-00005800: 6f6d 7061 6e79 2031 222c 0a20 2020 2020  ompany 1",.     
-00005810: 2022 556e 6d61 7070 6162 6c65 436f 6c75   "UnmappableColu
-00005820: 6d6e 223a 2022 466f 6f22 2c0a 2020 7d0a  mn": "Foo",.  }.
-00005830: 5d0a 7265 7370 6f6e 7365 7320 3d20 6463  ].responses = dc
-00005840: 2e69 6e73 6572 745f 6461 7461 2822 436f  .insert_data("Co
-00005850: 6d70 616e 7922 2c20 746f 5f73 656e 6429  mpany", to_send)
-00005860: 0a60 6060 0a57 696c 6c20 5265 7475 726e  .```.Will Return
-00005870: 0a60 6060 6261 7368 0a54 7261 6365 6261  .```bash.Traceba
-00005880: 636b 2e2e 2e0a 4b65 7945 7272 6f72 3a20  ck....KeyError: 
-00005890: 226d 6170 7069 6e67 2065 7272 6f72 2c20  "mapping error, 
-000058a0: 636f 756c 6420 6e6f 7420 6d61 703a 205b  could not map: [
-000058b0: 2755 6e6d 6170 7061 626c 6543 6f6c 756d  'UnmappableColum
-000058c0: 6e27 5d22 0a60 6060 0a0a 2323 2323 2043  n']".```..#### C
-000058d0: 7265 6174 6520 4461 7461 0a45 7861 6d70  reate Data.Examp
-000058e0: 6c65 2c20 746f 2069 6e73 6572 7420 6461  le, to insert da
-000058f0: 7461 2069 6e74 6f20 7468 6520 2243 6f6d  ta into the "Com
-00005900: 7061 6e79 2220 6f62 6a65 6374 2066 726f  pany" object fro
-00005910: 6d20 6120 6c69 7374 3a0a 0a60 6060 7079  m a list:..```py
-00005920: 7468 6f6e 0a66 726f 6d20 6465 616c 636c  thon.from dealcl
-00005930: 6f75 645f 7364 6b20 696d 706f 7274 2044  oud_sdk import D
-00005940: 6561 6c43 6c6f 7564 0a0a 6463 203d 2044  ealCloud..dc = D
-00005950: 6561 6c43 6c6f 7564 2e66 726f 6d5f 7961  ealCloud.from_ya
-00005960: 6d6c 2822 7061 7468 2f74 6f2f 7961 6d6c  ml("path/to/yaml
-00005970: 5f63 6f6e 6669 675f 6669 6c65 2e6a 736f  _config_file.jso
-00005980: 6e22 290a 0a74 6f5f 7365 6e64 203d 205b  n")..to_send = [
-00005990: 0a20 207b 0a20 2020 2020 2022 436f 6d70  .  {.      "Comp
-000059a0: 616e 794e 616d 6522 3a20 2254 6573 7420  anyName": "Test 
-000059b0: 436f 6d70 616e 7920 3122 2c0a 2020 2020  Company 1",.    
-000059c0: 2020 2243 6f6d 7061 6e79 5479 7065 223a    "CompanyType":
-000059d0: 2031 3233 3435 2c0a 2020 2020 2020 2242   12345,.      "B
-000059e0: 7573 696e 6573 7344 6573 6372 6970 7469  usinessDescripti
-000059f0: 6f6e 223a 2022 4865 7265 2069 7320 6120  on": "Here is a 
-00005a00: 6275 7369 6e65 7373 2064 6573 6372 6970  business descrip
-00005a10: 7469 6f6e 222c 0a20 2020 2020 2022 5365  tion",.      "Se
-00005a20: 6374 6f72 223a 2031 3433 3231 2c0a 2020  ctor": 14321,.  
-00005a30: 7d0a 5d0a 7265 7370 6f6e 7365 7320 3d20  }.].responses = 
-00005a40: 6463 2e69 6e73 6572 745f 6461 7461 2822  dc.insert_data("
-00005a50: 436f 6d70 616e 7922 2c20 746f 5f73 656e  Company", to_sen
-00005a60: 6429 0a60 6060 0a49 6620 7375 6363 6573  d).```.If succes
-00005a70: 7366 756c 2c20 6072 6573 706f 6e73 6573  sful, `responses
-00005a80: 6020 7769 6c6c 2063 6f6e 7461 696e 2074  ` will contain t
-00005a90: 6865 2062 656c 6f77 202d 206e 6f74 6520  he below - note 
-00005aa0: 7468 6174 2060 456e 7472 7949 6460 2069  that `EntryId` i
-00005ab0: 7320 6e6f 7720 696e 636c 7564 6564 3a0a  s now included:.
-00005ac0: 6060 6070 7974 686f 6e0a 5b0a 2020 2020  ```python.[.    
-00005ad0: 7b0a 2020 2020 2020 2020 2245 6e74 7279  {.        "Entry
-00005ae0: 4964 223a 2032 3334 3536 372c 0a20 2020  Id": 234567,.   
-00005af0: 2020 2020 2022 436f 6d70 616e 794e 616d       "CompanyNam
-00005b00: 6522 3a20 2254 6573 7420 436f 6d70 616e  e": "Test Compan
-00005b10: 7920 3122 2c0a 2020 2020 2020 2020 2243  y 1",.        "C
-00005b20: 6f6d 7061 6e79 5479 7065 223a 2031 3233  ompanyType": 123
-00005b30: 3435 2c0a 2020 2020 2020 2020 2242 7573  45,.        "Bus
+00000370: 6d61 726b 646f 776e 0a0a 3c68 313e 6465  markdown..<h1>de
+00000380: 616c 636c 6f75 645f 7364 6b3c 2f68 313e  alcloud_sdk</h1>
+00000390: 0a0a 4120 7772 6170 7065 7220 6172 6f75  ..A wrapper arou
+000003a0: 6e64 2074 6865 2044 6561 6c43 6c6f 7564  nd the DealCloud
+000003b0: 2041 5049 2c20 6465 7369 676e 6564 2074   API, designed t
+000003c0: 6f20 6173 7369 7374 2075 7365 7273 2c20  o assist users, 
+000003d0: 636c 6965 6e74 7320 616e 6420 7061 7274  clients and part
+000003e0: 6e65 7273 2074 6f20 6275 696c 6420 6f6e  ners to build on
+000003f0: 2074 6f70 206f 6620 6f75 7220 706c 6174   top of our plat
+00000400: 666f 726d 2773 2041 5049 2e0a 0a23 2043  form's API...# C
+00000410: 6f6e 7465 6e74 730a 312e 205b 496e 7374  ontents.1. [Inst
+00000420: 616c 6c61 7469 6f6e 5d28 2369 6e73 7461  allation](#insta
+00000430: 6c6c 6174 696f 6e29 0a20 2020 312e 205b  llation).   1. [
+00000440: 5769 7468 2070 6970 5d28 2370 6970 290a  With pip](#pip).
+00000450: 2020 2032 2e20 5b4c 6f63 616c 6c79 5d28     2. [Locally](
+00000460: 2362 7569 6c64 2d61 6e64 2d69 6e73 7461  #build-and-insta
+00000470: 6c6c 2d6c 6f63 616c 6c79 290a 322e 205b  ll-locally).2. [
+00000480: 5573 6167 655d 2823 7573 6167 6529 0a20  Usage](#usage). 
+00000490: 2020 312e 205b 4372 6561 7469 6e67 2061    1. [Creating a
+000004a0: 2063 6c69 656e 7420 616e 6420 6175 7468   client and auth
+000004b0: 656e 7469 6361 7469 6e67 5d28 2363 7265  enticating](#cre
+000004c0: 6174 696e 672d 612d 636c 6965 6e74 2d61  ating-a-client-a
+000004d0: 6e64 2d61 7574 6865 6e74 6963 6174 696e  nd-authenticatin
+000004e0: 6729 0a20 2020 322e 205b 5365 6375 7265  g).   2. [Secure
+000004f0: 6c79 206c 6f61 6469 6e67 2063 7265 6465  ly loading crede
+00000500: 6e74 6961 6c73 5d28 2373 6563 7572 656c  ntials](#securel
+00000510: 792d 6c6f 6164 696e 672d 6372 6564 656e  y-loading-creden
+00000520: 7469 616c 7329 0a20 2020 2020 2031 2e20  tials).      1. 
+00000530: 5b55 7369 6e67 2045 6e76 6972 6f6e 6d65  [Using Environme
+00000540: 6e74 2056 6172 6961 626c 6573 5d28 2375  nt Variables](#u
+00000550: 7369 6e67 2d65 6e76 6972 6f6e 6d65 6e74  sing-environment
+00000560: 2d76 6172 6961 626c 6573 290a 2020 2020  -variables).    
+00000570: 2020 322e 205b 5573 696e 6720 4a53 4f4e    2. [Using JSON
+00000580: 2043 6f6e 6669 6720 4669 6c65 5d28 2375   Config File](#u
+00000590: 7369 6e67 2d6a 736f 6e2d 636f 6e66 6967  sing-json-config
+000005a0: 2d66 696c 6529 0a20 2020 2020 2033 2e20  -file).      3. 
+000005b0: 5b55 7369 6e67 2059 414d 4c20 436f 6e66  [Using YAML Conf
+000005c0: 6967 2046 696c 655d 2823 7573 696e 672d  ig File](#using-
+000005d0: 7961 6d6c 2d63 6f6e 6669 672d 6669 6c65  yaml-config-file
+000005e0: 290a 2020 2033 2e20 5b53 6368 656d 6120  ).   3. [Schema 
+000005f0: 5175 6572 7969 6e67 5d28 2373 6368 656d  Querying](#schem
+00000600: 612d 7175 6572 7969 6e67 290a 2020 2020  a-querying).    
+00000610: 2020 312e 205b 4765 7420 5573 6572 735d    1. [Get Users]
+00000620: 2823 6765 742d 7573 6572 7329 0a20 2020  (#get-users).   
+00000630: 2020 2032 2e20 5b47 6574 2043 7572 7265     2. [Get Curre
+00000640: 6e63 6965 735d 2823 6765 742d 6375 7272  ncies](#get-curr
+00000650: 656e 6369 6573 290a 2020 2020 2020 332e  encies).      3.
+00000660: 205b 4765 7420 4f62 6a65 6374 735d 2823   [Get Objects](#
+00000670: 6765 742d 6f62 6a65 6374 7329 0a20 2020  get-objects).   
+00000680: 2020 2034 2e20 5b47 6574 2046 6965 6c64     4. [Get Field
+00000690: 735d 2823 6765 742d 6669 656c 6473 290a  s](#get-fields).
+000006a0: 2020 2020 2020 352e 205b 4765 7420 5363        5. [Get Sc
+000006b0: 6865 6d61 5d28 2367 6574 2d73 6368 656d  hema](#get-schem
+000006c0: 6129 0a20 2020 342e 205b 4461 7461 204f  a).   4. [Data O
+000006d0: 7065 7261 7469 6f6e 735d 2823 6461 7461  perations](#data
+000006e0: 2d6f 7065 7261 7469 6f6e 7329 0a20 2020  -operations).   
+000006f0: 2020 2031 2e20 5b4c 6973 7420 436f 6e66     1. [List Conf
+00000700: 6967 7572 6564 2056 6965 7773 5d28 236c  igured Views](#l
+00000710: 6973 742d 636f 6e66 6967 7572 6564 2d76  ist-configured-v
+00000720: 6965 7773 290a 2020 2020 2020 322e 205b  iews).      2. [
+00000730: 5265 6164 2044 6174 615d 2823 7265 6164  Read Data](#read
+00000740: 2d64 6174 6129 0a20 2020 2020 2020 2020  -data).         
+00000750: 312e 205b 5265 6164 696e 6720 4461 7461  1. [Reading Data
+00000760: 2066 726f 6d20 616e 204f 626a 6563 745d   from an Object]
+00000770: 2823 7265 6164 696e 672d 6461 7461 2d66  (#reading-data-f
+00000780: 726f 6d2d 616e 2d6f 626a 6563 7429 0a20  rom-an-object). 
+00000790: 2020 2020 2020 2020 2020 2031 2e20 5b52             1. [R
+000007a0: 6573 6f6c 7669 6e67 2074 6f20 4e61 6d65  esolving to Name
+000007b0: 206f 7220 746f 2049 445d 2823 7265 736f   or to ID](#reso
+000007c0: 6c76 696e 672d 746f 2d6e 616d 652d 6f72  lving-to-name-or
+000007d0: 2d74 6f2d 6964 290a 2020 2020 2020 2020  -to-id).        
+000007e0: 2020 2020 322e 205b 5265 6164 696e 6720      2. [Reading 
+000007f0: 6120 5375 6273 6574 206f 6620 4669 656c  a Subset of Fiel
+00000800: 6473 5d28 2372 6561 6469 6e67 2d61 2d73  ds](#reading-a-s
+00000810: 7562 7365 742d 6f66 2d66 6965 6c64 7329  ubset-of-fields)
+00000820: 0a20 2020 2020 2020 2020 322e 205b 5265  .         2. [Re
+00000830: 6164 696e 6720 4461 7461 2066 726f 6d20  ading Data from 
+00000840: 6120 5669 6577 5d28 2372 6561 6469 6e67  a View](#reading
+00000850: 2d64 6174 612d 6672 6f6d 2d61 2d76 6965  -data-from-a-vie
+00000860: 7729 200a 2020 2020 2020 2020 2020 2020  w) .            
+00000870: 312e 205b 5573 696e 6720 6120 4669 6c74  1. [Using a Filt
+00000880: 6572 2057 6865 6e20 5265 6164 696e 6720  er When Reading 
+00000890: 5669 6577 2044 6174 615d 2823 7573 696e  View Data](#usin
+000008a0: 672d 612d 6669 6c74 6572 2d77 6865 6e2d  g-a-filter-when-
+000008b0: 7265 6164 696e 672d 7669 6577 2d64 6174  reading-view-dat
+000008c0: 6129 200a 2020 2020 2020 332e 205b 4372  a) .      3. [Cr
+000008d0: 6561 7465 2c20 5570 6461 7465 2c20 5570  eate, Update, Up
+000008e0: 7365 7274 2044 6174 615d 2823 6372 6561  sert Data](#crea
+000008f0: 7465 2d75 7064 6174 652d 616e 642d 7570  te-update-and-up
+00000900: 7365 7274 2d64 6174 6129 0a20 2020 2020  sert-data).     
+00000910: 2020 2020 312e 205b 4669 656c 6420 4d61      1. [Field Ma
+00000920: 7070 696e 675d 2823 6669 656c 642d 6d61  pping](#field-ma
+00000930: 7070 696e 6729 0a20 2020 2020 2020 2020  pping).         
+00000940: 322e 205b 4372 6561 7465 2044 6174 615d  2. [Create Data]
+00000950: 2823 6372 6561 7465 2d64 6174 6129 0a20  (#create-data). 
+00000960: 2020 2020 2020 2020 332e 205b 5570 6461          3. [Upda
+00000970: 7465 2044 6174 615d 2823 7570 6461 7465  te Data](#update
+00000980: 2d64 6174 6129 0a20 2020 2020 2020 2020  -data).         
+00000990: 342e 205b 5570 7365 7274 2044 6174 615d  4. [Upsert Data]
+000009a0: 2823 7570 7365 7274 2d64 6174 6129 0a20  (#upsert-data). 
+000009b0: 2020 2020 2020 2020 352e 205b 556e 6465          5. [Unde
+000009c0: 7273 7461 6e64 696e 6720 4572 726f 7273  rstanding Errors
+000009d0: 5d28 2375 6e64 6572 7374 616e 6469 6e67  ](#understanding
+000009e0: 2d65 7272 6f72 7329 0a20 2020 2020 2034  -errors).      4
+000009f0: 2e20 5b44 656c 6574 6520 4461 7461 5d28  . [Delete Data](
+00000a00: 2364 656c 6574 652d 6461 7461 2920 0a0a  #delete-data) ..
+00000a10: 2320 496e 7374 616c 6c61 7469 6f6e 0a23  # Installation.#
+00000a20: 2320 7069 700a 496e 7374 616c 6c20 7573  # pip.Install us
+00000a30: 696e 6720 7069 7020 7769 7468 3a0a 6060  ing pip with:.``
+00000a40: 6062 6173 680a 7069 7020 696e 7374 616c  `bash.pip instal
+00000a50: 6c20 6465 616c 636c 6f75 645f 7364 6b0a  l dealcloud_sdk.
+00000a60: 6060 600a 2320 5573 6167 650a 0a23 2320  ```.# Usage..## 
+00000a70: 4372 6561 7469 6e67 2061 2063 6c69 656e  Creating a clien
+00000a80: 7420 616e 6420 6175 7468 656e 7469 6361  t and authentica
+00000a90: 7469 6e67 0a60 6465 616c 636c 6f75 645f  ting.`dealcloud_
+00000aa0: 7364 6b60 2773 206d 6169 6e20 656e 7472  sdk`'s main entr
+00000ab0: 7970 6f69 6e74 2069 7320 7468 6520 6044  ypoint is the `D
+00000ac0: 6561 6c43 6c6f 7564 6020 636c 6173 732e  ealCloud` class.
+00000ad0: 2057 6865 6e20 6974 2069 7320 696e 7374   When it is inst
+00000ae0: 616e 7469 6174 6564 2c20 7468 6520 6f62  antiated, the ob
+00000af0: 6a65 6374 2069 7320 7363 6f70 6564 2074  ject is scoped t
+00000b00: 6f20 6120 6769 7665 6e20 4465 616c 436c  o a given DealCl
+00000b10: 6f75 6420 656e 7669 726f 6e6d 656e 742c  oud environment,
+00000b20: 2062 7920 7061 7373 696e 6720 7468 6520   by passing the 
+00000b30: 7369 7465 2055 524c 2061 6e64 2041 5049  site URL and API
+00000b40: 2063 7265 6465 6e74 6961 6c73 2061 7320   credentials as 
+00000b50: 6172 6775 6d65 6e74 733a 0a0a 6060 6070  arguments:..```p
+00000b60: 7974 686f 6e0a 6672 6f6d 2064 6561 6c63  ython.from dealc
+00000b70: 6c6f 7564 5f73 646b 2069 6d70 6f72 7420  loud_sdk import 
+00000b80: 4465 616c 436c 6f75 640a 0a64 6320 3d20  DealCloud..dc = 
+00000b90: 4465 616c 436c 6f75 6428 0a20 2020 7369  DealCloud(.   si
+00000ba0: 7465 5f75 726c 3d22 636c 6965 6e74 2e64  te_url="client.d
+00000bb0: 6561 6c63 6c6f 7564 2e63 6f6d 222c 0a20  ealcloud.com",. 
+00000bc0: 2020 636c 6965 6e74 5f69 643d 2231 3233    client_id="123
+00000bd0: 3435 222c 0a20 2020 636c 6965 6e74 5f73  45",.   client_s
+00000be0: 6563 7265 743d 2279 6f75 725f 636c 6965  ecret="your_clie
+00000bf0: 6e74 5f73 6563 7265 7422 2c0a 290a 6060  nt_secret",.).``
+00000c00: 600a 0a3e 205b 2157 4152 4e49 4e47 5d0a  `..> [!WARNING].
+00000c10: 3e20 5768 696c 7374 2073 7569 7461 626c  > Whilst suitabl
+00000c20: 6520 666f 7220 6c6f 6361 6c20 6465 7665  e for local deve
+00000c30: 6c6f 706d 656e 742c 2074 6865 2061 626f  lopment, the abo
+00000c40: 7665 2069 6d70 6c65 6d65 6e74 6174 696f  ve implementatio
+00000c50: 6e20 6973 2069 6e73 6563 7572 6520 6966  n is insecure if
+00000c60: 2079 6f75 206b 6565 7020 636f 6465 2069   you keep code i
+00000c70: 6e20 6f6e 6c69 6e65 2072 6570 6f73 6974  n online reposit
+00000c80: 6f72 6965 7320 7375 6368 2061 7320 4769  ories such as Gi
+00000c90: 7448 7562 2e20 506c 6561 7365 2073 6565  tHub. Please see
+00000ca0: 2074 6865 2062 656c 6f77 2065 7861 6d70   the below examp
+00000cb0: 6c65 7320 666f 7220 6d6f 7265 2073 6563  les for more sec
+00000cc0: 7572 6520 696d 706c 656d 656e 7461 7469  ure implementati
+00000cd0: 6f6e 732e 2020 0a0a 2323 2053 6563 7572  ons.  ..## Secur
+00000ce0: 656c 7920 6c6f 6164 696e 6720 6372 6564  ely loading cred
+00000cf0: 656e 7469 616c 730a 2323 2320 5573 696e  entials.### Usin
+00000d00: 6720 456e 7669 726f 6e6d 656e 7420 5661  g Environment Va
+00000d10: 7269 6162 6c65 730a 0a57 6865 7265 2074  riables..Where t
+00000d20: 6865 2065 6e76 6972 6f6e 6d65 6e74 2076  he environment v
+00000d30: 6172 6961 626c 6573 2063 6f6e 7461 696e  ariables contain
+00000d40: 2074 6865 2072 656c 6576 616e 7420 7661   the relevant va
+00000d50: 6c75 6573 2e20 5468 6573 6520 6361 6e20  lues. These can 
+00000d60: 6265 206c 6f61 6465 6420 6672 6f6d 2061  be loaded from a
+00000d70: 202e 656e 7620 6669 6c65 2075 7369 6e67   .env file using
+00000d80: 2074 6865 2060 7079 7468 6f6e 2d64 6f74   the `python-dot
+00000d90: 656e 7660 205b 5079 5069 2070 6163 6b61  env` [PyPi packa
+00000da0: 6765 5d28 6874 7470 733a 2f2f 7079 7069  ge](https://pypi
+00000db0: 2e6f 7267 2f70 726f 6a65 6374 2f70 7974  .org/project/pyt
+00000dc0: 686f 6e2d 646f 7465 6e76 2f29 2e0a 0a54  hon-dotenv/)...T
+00000dd0: 6865 2064 6566 6175 6c74 2065 6e76 6972  he default envir
+00000de0: 6f6e 6d65 6e74 2076 6172 6961 626c 6520  onment variable 
+00000df0: 6e61 6d65 7320 6172 652c 2074 6865 7365  names are, these
+00000e00: 2063 616e 2062 6520 6f76 6572 7269 6464   can be overridd
+00000e10: 656e 2069 6620 6465 7369 7265 643a 0a60  en if desired:.`
+00000e20: 6060 0a44 435f 5344 4b5f 5349 5445 5f55  ``.DC_SDK_SITE_U
+00000e30: 524c 0a44 435f 5344 4b5f 434c 4945 4e54  RL.DC_SDK_CLIENT
+00000e40: 5f49 440a 4443 5f53 444b 5f43 4c49 454e  _ID.DC_SDK_CLIEN
+00000e50: 545f 5345 4352 4554 0a60 6060 0a0a 6060  T_SECRET.```..``
+00000e60: 6070 7974 686f 6e0a 6672 6f6d 2064 6561  `python.from dea
+00000e70: 6c63 6c6f 7564 5f73 646b 2069 6d70 6f72  lcloud_sdk impor
+00000e80: 7420 4465 616c 436c 6f75 640a 0a64 6320  t DealCloud..dc 
+00000e90: 3d20 4465 616c 436c 6f75 6428 292e 6672  = DealCloud().fr
+00000ea0: 6f6d 5f65 6e76 2829 0a60 6060 0a54 6f20  om_env().```.To 
+00000eb0: 6f76 6572 7269 6465 2074 6865 2064 6566  override the def
+00000ec0: 6175 6c74 2065 6e76 6972 6f6e 6d65 6e74  ault environment
+00000ed0: 2076 6172 6961 626c 6520 6e61 6d65 733a   variable names:
+00000ee0: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00000ef0: 6465 616c 636c 6f75 645f 7364 6b20 696d  dealcloud_sdk im
+00000f00: 706f 7274 2044 6561 6c43 6c6f 7564 0a0a  port DealCloud..
+00000f10: 6463 203d 2044 6561 6c43 6c6f 7564 2829  dc = DealCloud()
+00000f20: 2e66 726f 6d5f 656e 7628 0a20 2073 6974  .from_env(.  sit
+00000f30: 655f 7572 6c5f 656e 765f 6e61 6d65 3d22  e_url_env_name="
+00000f40: 4f56 4552 5249 4444 454e 5f53 4954 455f  OVERRIDDEN_SITE_
+00000f50: 4b45 5922 2c0a 2020 636c 6965 6e74 5f69  KEY",.  client_i
+00000f60: 645f 656e 765f 6e61 6d65 3d22 4f56 4552  d_env_name="OVER
+00000f70: 5249 4444 454e 5f43 4c49 454e 545f 4944  RIDDEN_CLIENT_ID
+00000f80: 5f4b 4559 222c 0a20 2063 6c69 656e 745f  _KEY",.  client_
+00000f90: 7365 6372 6574 5f65 6e76 5f6e 616d 653d  secret_env_name=
+00000fa0: 224f 5645 5252 4944 4445 4e5f 434c 4945  "OVERRIDDEN_CLIE
+00000fb0: 4e54 5f53 4543 5245 545f 4b45 5922 2c0a  NT_SECRET_KEY",.
+00000fc0: 290a 6060 600a 2323 2320 5573 696e 6720  ).```.### Using 
+00000fd0: 4a53 4f4e 2043 6f6e 6669 6720 4669 6c65  JSON Config File
+00000fe0: 0a47 6976 656e 2061 204a 534f 4e20 6669  .Given a JSON fi
+00000ff0: 6c65 2069 6e20 7468 6520 6265 6c6f 7720  le in the below 
+00001000: 666f 726d 6174 3a0a 6060 606a 736f 6e0a  format:.```json.
+00001010: 7b0a 2020 2273 6974 655f 7572 6c22 3a20  {.  "site_url": 
+00001020: 2263 6c69 656e 742e 6465 616c 636c 6f75  "client.dealclou
+00001030: 642e 636f 6d22 2c0a 2020 2263 6c69 656e  d.com",.  "clien
+00001040: 745f 6964 223a 2031 3233 3435 2c0a 2020  t_id": 12345,.  
+00001050: 2263 6c69 656e 745f 7365 6372 6574 223a  "client_secret":
+00001060: 2022 796f 7572 5f63 6c69 656e 745f 7365   "your_client_se
+00001070: 6372 6574 220a 7d0a 6060 600a 5468 6520  cret".}.```.The 
+00001080: 4465 616c 436c 6f75 6420 6f62 6a65 6374  DealCloud object
+00001090: 2063 616e 2062 6520 6372 6561 7465 6420   can be created 
+000010a0: 6173 2062 656c 6f77 3a0a 0a60 6060 7079  as below:..```py
+000010b0: 7468 6f6e 0a66 726f 6d20 6465 616c 636c  thon.from dealcl
+000010c0: 6f75 645f 7364 6b20 696d 706f 7274 2044  oud_sdk import D
+000010d0: 6561 6c43 6c6f 7564 0a0a 6463 203d 2044  ealCloud..dc = D
+000010e0: 6561 6c43 6c6f 7564 2e66 726f 6d5f 6a73  ealCloud.from_js
+000010f0: 6f6e 2822 7061 7468 2f74 6f2f 6a73 6f6e  on("path/to/json
+00001100: 5f63 6f6e 6669 675f 6669 6c65 2e6a 736f  _config_file.jso
+00001110: 6e22 290a 6060 600a 5369 6d69 6c61 726c  n").```.Similarl
+00001120: 792c 2069 6620 7468 6520 6372 6564 656e  y, if the creden
+00001130: 7469 616c 7320 6172 6520 7374 6f72 6564  tials are stored
+00001140: 2061 7320 7061 7274 206f 6620 6120 6c61   as part of a la
+00001150: 7267 6572 204a 534f 4e20 636f 6e66 6967  rger JSON config
+00001160: 2066 696c 652c 2061 206b 6579 2070 6174   file, a key pat
+00001170: 6820 6361 6e20 6265 2070 6173 7365 6420  h can be passed 
+00001180: 6173 2074 6865 2073 6563 6f6e 6420 6172  as the second ar
+00001190: 6775 6d65 6e74 2c20 6469 7265 6374 696e  gument, directin
+000011a0: 6720 2060 4465 616c 436c 6f75 6460 2074  g  `DealCloud` t
+000011b0: 6f20 7468 6520 7061 7468 206f 6620 7468  o the path of th
+000011c0: 6520 6372 6564 656e 7469 616c 7320 696e  e credentials in
+000011d0: 2074 6865 2077 6964 6572 204a 534f 4e2e   the wider JSON.
+000011e0: 2046 6f72 2065 7861 6d70 6c65 3a0a 6060   For example:.``
+000011f0: 606a 736f 6e0a 7b0a 2020 2020 226f 7468  `json.{.    "oth
+00001200: 6572 223a 205b 312c 322c 335d 2c0a 2020  er": [1,2,3],.  
+00001210: 2020 2263 7265 6473 223a 7b0a 2020 2020    "creds":{.    
+00001220: 2020 2020 2264 6322 3a7b 0a20 2020 2020      "dc":{.     
+00001230: 2020 2020 2022 7369 7465 5f75 726c 223a       "site_url":
+00001240: 2022 636c 6965 6e74 2e64 6561 6c63 6c6f   "client.dealclo
+00001250: 7564 2e63 6f6d 222c 0a20 2020 2020 2020  ud.com",.       
+00001260: 2020 2022 636c 6965 6e74 5f69 6422 3a20     "client_id": 
+00001270: 3132 3334 352c 0a20 2020 2020 2020 2020  12345,.         
+00001280: 2022 636c 6965 6e74 5f73 6563 7265 7422   "client_secret"
+00001290: 3a20 2279 6f75 725f 636c 6965 6e74 5f73  : "your_client_s
+000012a0: 6563 7265 7422 0a20 2020 2020 2020 207d  ecret".        }
+000012b0: 0a20 2020 207d 0a7d 0a60 6060 0a0a 6060  .    }.}.```..``
+000012c0: 6070 7974 686f 6e0a 6672 6f6d 2064 6561  `python.from dea
+000012d0: 6c63 6c6f 7564 5f73 646b 2069 6d70 6f72  lcloud_sdk impor
+000012e0: 7420 4465 616c 436c 6f75 640a 0a64 6320  t DealCloud..dc 
+000012f0: 3d20 4465 616c 436c 6f75 642e 6672 6f6d  = DealCloud.from
+00001300: 5f6a 736f 6e28 2270 6174 682f 746f 2f6a  _json("path/to/j
+00001310: 736f 6e5f 636f 6e66 6967 5f66 696c 652e  son_config_file.
+00001320: 6a73 6f6e 222c 2022 6372 6564 732e 6463  json", "creds.dc
+00001330: 2229 0a60 6060 0a23 2323 2055 7369 6e67  ").```.### Using
+00001340: 2059 414d 4c20 436f 6e66 6967 2046 696c   YAML Config Fil
+00001350: 650a 4769 7665 6e20 6120 5941 4d4c 2066  e.Given a YAML f
+00001360: 696c 6520 696e 2074 6865 2062 656c 6f77  ile in the below
+00001370: 2066 6f72 6d61 743a 0a60 6060 7961 6d6c   format:.```yaml
+00001380: 0a73 6974 655f 7572 6c3a 2022 636c 6965  .site_url: "clie
+00001390: 6e74 2e64 6561 6c63 6c6f 7564 2e63 6f6d  nt.dealcloud.com
+000013a0: 220a 636c 6965 6e74 5f69 643a 2031 3233  ".client_id: 123
+000013b0: 3435 0a63 6c69 656e 745f 7365 6372 6574  45.client_secret
+000013c0: 3a20 2279 6f75 725f 636c 6965 6e74 5f73  : "your_client_s
+000013d0: 6563 7265 7422 0a60 6060 0a54 6865 2044  ecret".```.The D
+000013e0: 6561 6c43 6c6f 7564 206f 626a 6563 7420  ealCloud object 
+000013f0: 6361 6e20 6265 2063 7265 6174 6564 2061  can be created a
+00001400: 7320 6265 6c6f 773a 0a0a 6060 6070 7974  s below:..```pyt
+00001410: 686f 6e0a 6672 6f6d 2064 6561 6c63 6c6f  hon.from dealclo
+00001420: 7564 5f73 646b 2069 6d70 6f72 7420 4465  ud_sdk import De
+00001430: 616c 436c 6f75 640a 0a64 6320 3d20 4465  alCloud..dc = De
+00001440: 616c 436c 6f75 642e 6672 6f6d 5f79 616d  alCloud.from_yam
+00001450: 6c28 2270 6174 682f 746f 2f79 616d 6c5f  l("path/to/yaml_
+00001460: 636f 6e66 6967 5f66 696c 652e 6a73 6f6e  config_file.json
+00001470: 2229 0a60 6060 0a53 696d 696c 6172 6c79  ").```.Similarly
+00001480: 2c20 6966 2074 6865 2063 7265 6465 6e74  , if the credent
+00001490: 6961 6c73 2061 7265 2073 746f 7265 6420  ials are stored 
+000014a0: 6173 2070 6172 7420 6f66 2061 206c 6172  as part of a lar
+000014b0: 6765 7220 5941 4d4c 2063 6f6e 6669 6720  ger YAML config 
+000014c0: 6669 6c65 2c20 6120 6b65 7920 7061 7468  file, a key path
+000014d0: 2063 616e 2062 6520 7061 7373 6564 2061   can be passed a
+000014e0: 7320 7468 6520 7365 636f 6e64 2061 7267  s the second arg
+000014f0: 756d 656e 742c 2064 6972 6563 7469 6e67  ument, directing
+00001500: 2020 6044 6561 6c43 6c6f 7564 6020 746f    `DealCloud` to
+00001510: 2074 6865 2070 6174 6820 6f66 2074 6865   the path of the
+00001520: 2063 7265 6465 6e74 6961 6c73 2069 6e20   credentials in 
+00001530: 7468 6520 7769 6465 7220 5941 4d4c 2e20  the wider YAML. 
+00001540: 466f 7220 6578 616d 706c 653a 0a60 6060  For example:.```
+00001550: 7961 6d6c 0a6f 7468 6572 3a0a 2020 2d20  yaml.other:.  - 
+00001560: 310a 2020 2d20 320a 2020 2d20 330a 6372  1.  - 2.  - 3.cr
+00001570: 6564 733a 0a20 2064 633a 0a20 2020 2073  eds:.  dc:.    s
+00001580: 6974 655f 7572 6c3a 2022 636c 6965 6e74  ite_url: "client
+00001590: 2e64 6561 6c63 6c6f 7564 2e63 6f6d 220a  .dealcloud.com".
+000015a0: 2020 2020 636c 6965 6e74 5f69 643a 2031      client_id: 1
+000015b0: 3233 3435 0a20 2020 2063 6c69 656e 745f  2345.    client_
+000015c0: 7365 6372 6574 3a20 2279 6f75 725f 636c  secret: "your_cl
+000015d0: 6965 6e74 5f73 6563 7265 7422 0a60 6060  ient_secret".```
+000015e0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+000015f0: 2064 6561 6c63 6c6f 7564 5f73 646b 2069   dealcloud_sdk i
+00001600: 6d70 6f72 7420 4465 616c 436c 6f75 640a  mport DealCloud.
+00001610: 0a64 6320 3d20 4465 616c 436c 6f75 642e  .dc = DealCloud.
+00001620: 6672 6f6d 5f79 616d 6c28 2270 6174 682f  from_yaml("path/
+00001630: 746f 2f79 616d 6c5f 636f 6e66 6967 5f66  to/yaml_config_f
+00001640: 696c 652e 6a73 6f6e 222c 2022 6372 6564  ile.json", "cred
+00001650: 732e 6463 2229 0a60 6060 0a0a 2323 2053  s.dc").```..## S
+00001660: 6368 656d 6120 5175 6572 7969 6e67 0a54  chema Querying.T
+00001670: 6865 2044 6561 6c43 6c6f 7564 2041 5049  he DealCloud API
+00001680: 2061 6c6c 6f77 7320 796f 7520 746f 2071   allows you to q
+00001690: 7565 7279 2074 6865 2073 6368 656d 6120  uery the schema 
+000016a0: 6f66 2061 2067 6976 656e 2073 6974 652e  of a given site.
+000016b0: 2054 6865 2060 4465 616c 436c 6f75 6460   The `DealCloud`
+000016c0: 2063 6c61 7373 2070 726f 7669 6465 7320   class provides 
+000016d0: 6163 6365 7373 2074 6f20 7468 6520 7363  access to the sc
+000016e0: 6865 6d61 2065 6e64 706f 696e 7473 2074  hema endpoints t
+000016f0: 6872 6f75 6768 2074 6865 2066 6f6c 6c6f  hrough the follo
+00001700: 7769 6e67 206d 6574 686f 6473 3a0a 3e20  wing methods:.> 
+00001710: 5468 6520 7363 6865 6d61 206d 6f64 656c  The schema model
+00001720: 7320 6172 6520 6465 6669 6e65 6420 7573  s are defined us
+00001730: 696e 6720 5b50 7964 616e 7469 635d 2868  ing [Pydantic](h
+00001740: 7474 7073 3a2f 2f70 7964 616e 7469 632e  ttps://pydantic.
+00001750: 6465 762f 292c 2066 6f72 2063 6c65 6172  dev/), for clear
+00001760: 2076 616c 6964 6174 696f 6e2c 2073 7472   validation, str
+00001770: 6169 6768 7466 6f72 7761 7264 2061 7474  aightforward att
+00001780: 7269 6275 7465 2061 6363 6573 7320 616e  ribute access an
+00001790: 6420 4944 4520 6173 7369 7374 616e 6365  d IDE assistance
+000017a0: 2e0a 0a23 2323 2047 6574 2055 7365 7273  ...### Get Users
+000017b0: 0a0a 6044 6561 6c43 6c6f 7564 2e67 6574  ..`DealCloud.get
+000017c0: 5f75 7365 7273 2829 6020 7769 6c6c 2072  _users()` will r
+000017d0: 6574 7572 6e20 616c 6c20 7573 6572 7320  eturn all users 
+000017e0: 696e 2074 6865 2073 6974 652e 2053 7065  in the site. Spe
+000017f0: 6369 6669 6361 6c6c 792c 2061 6e20 6172  cifically, an ar
+00001800: 7261 7920 6f66 2060 5573 6572 6020 6f62  ray of `User` ob
+00001810: 6a65 6374 732e 2054 6865 2061 7267 756d  jects. The argum
+00001820: 656e 743a 2060 6163 7469 7665 5f6f 6e6c  ent: `active_onl
+00001830: 7960 2069 7320 6120 626f 6f6c 6561 6e20  y` is a boolean 
+00001840: 7468 6174 2063 616e 2062 6520 7061 7373  that can be pass
+00001850: 6564 2c20 6966 2074 7275 652c 2074 6865  ed, if true, the
+00001860: 2066 756e 6374 696f 6e20 7769 6c6c 206f   function will o
+00001870: 6e6c 7920 7265 7475 726e 2061 6374 6976  nly return activ
+00001880: 6520 7573 6572 732e 0a0a 4578 616d 706c  e users...Exampl
+00001890: 653a 0a0a 6060 6070 7974 686f 6e0a 6672  e:..```python.fr
+000018a0: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
+000018b0: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
+000018c0: 640a 0a64 6320 3d20 4465 616c 436c 6f75  d..dc = DealClou
+000018d0: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
+000018e0: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
+000018f0: 5f66 696c 652e 6a73 6f6e 2229 0a0a 7573  _file.json")..us
+00001900: 6572 7320 3d20 6463 2e67 6574 5f75 7365  ers = dc.get_use
+00001910: 7273 2829 0a0a 666f 7220 7573 6572 2069  rs()..for user i
+00001920: 6e20 7573 6572 733a 0a20 2020 2070 7269  n users:.    pri
+00001930: 6e74 2866 227b 7573 6572 2e6e 616d 657d  nt(f"{user.name}
+00001940: 3a20 7b75 7365 722e 656d 6169 6c7d 2229  : {user.email}")
+00001950: 0a60 6060 0a57 696c 6c20 6f75 7470 7574  .```.Will output
+00001960: 3a0a 6060 6062 6173 680a 5573 6572 2031  :.```bash.User 1
+00001970: 3a20 7573 6572 3140 656d 6169 6c2e 636f  : user1@email.co
+00001980: 6d0a 5573 6572 2032 3a20 7573 6572 3240  m.User 2: user2@
+00001990: 656d 6169 6c2e 636f 6d0a 5573 6572 2033  email.com.User 3
+000019a0: 3a20 7573 6572 3340 656d 6169 6c2e 636f  : user3@email.co
+000019b0: 6d0a 5573 6572 2034 3a20 7573 6572 3440  m.User 4: user4@
+000019c0: 656d 6169 6c2e 636f 6d0a 2e2e 2e65 7463  email.com....etc
+000019d0: 0a60 6060 0a23 2323 2047 6574 2043 7572  .```.### Get Cur
+000019e0: 7265 6e63 6965 730a 6044 6561 6c43 6c6f  rencies.`DealClo
+000019f0: 7564 2e67 6574 5f63 7572 7265 6e63 6965  ud.get_currencie
+00001a00: 7328 2960 2077 696c 6c20 7265 7475 726e  s()` will return
+00001a10: 2074 6865 2063 7572 7265 6e63 7920 636f   the currency co
+00001a20: 6465 7320 6f66 2061 6c6c 2065 6e61 626c  des of all enabl
+00001a30: 6564 2063 7572 7265 6e63 6965 7320 696e  ed currencies in
+00001a40: 2074 6865 2073 6974 652e 0a45 7861 6d70   the site..Examp
+00001a50: 6c65 3a0a 0a60 6060 7079 7468 6f6e 0a66  le:..```python.f
+00001a60: 726f 6d20 6465 616c 636c 6f75 645f 7364  rom dealcloud_sd
+00001a70: 6b20 696d 706f 7274 2044 6561 6c43 6c6f  k import DealClo
+00001a80: 7564 0a0a 6463 203d 2044 6561 6c43 6c6f  ud..dc = DealClo
+00001a90: 7564 2e66 726f 6d5f 7961 6d6c 2822 7061  ud.from_yaml("pa
+00001aa0: 7468 2f74 6f2f 7961 6d6c 5f63 6f6e 6669  th/to/yaml_confi
+00001ab0: 675f 6669 6c65 2e6a 736f 6e22 290a 0a63  g_file.json")..c
+00001ac0: 7572 7265 6e63 6965 7320 3d20 6463 2e67  urrencies = dc.g
+00001ad0: 6574 5f63 7572 7265 6e63 6965 7328 290a  et_currencies().
+00001ae0: 0a66 6f72 2063 6379 2069 6e20 6375 7272  .for ccy in curr
+00001af0: 656e 6369 6573 3a0a 2020 2020 7072 696e  encies:.    prin
+00001b00: 7428 6363 7929 0a60 6060 0a57 696c 6c20  t(ccy).```.Will 
+00001b10: 6f75 7470 7574 3a0a 6060 6062 6173 680a  output:.```bash.
+00001b20: 4742 500a 5553 440a 4555 520a 2e2e 2e65  GBP.USD.EUR....e
+00001b30: 7463 0a60 6060 0a0a 2323 2320 4765 7420  tc.```..### Get 
+00001b40: 4f62 6a65 6374 730a 6044 6561 6c43 6c6f  Objects.`DealClo
+00001b50: 7564 2e67 6574 5f6f 626a 6563 7428 2960  ud.get_object()`
+00001b60: 2077 696c 6c20 7265 7475 726e 2061 6c6c   will return all
+00001b70: 2063 6f6e 6669 6775 7265 6420 6f62 6a65   configured obje
+00001b80: 6374 7320 696e 2074 6865 2073 6974 652e  cts in the site.
+00001b90: 2053 7065 6369 6669 6361 6c6c 792c 2061   Specifically, a
+00001ba0: 6e20 6172 7261 7920 6f66 2060 4f62 6a65  n array of `Obje
+00001bb0: 6374 6020 6f62 6a65 6374 732e 0a45 7861  ct` objects..Exa
+00001bc0: 6d70 6c65 3a0a 0a60 6060 7079 7468 6f6e  mple:..```python
+00001bd0: 0a66 726f 6d20 6465 616c 636c 6f75 645f  .from dealcloud_
+00001be0: 7364 6b20 696d 706f 7274 2044 6561 6c43  sdk import DealC
+00001bf0: 6c6f 7564 0a0a 6463 203d 2044 6561 6c43  loud..dc = DealC
+00001c00: 6c6f 7564 2e66 726f 6d5f 7961 6d6c 2822  loud.from_yaml("
+00001c10: 7061 7468 2f74 6f2f 7961 6d6c 5f63 6f6e  path/to/yaml_con
+00001c20: 6669 675f 6669 6c65 2e6a 736f 6e22 290a  fig_file.json").
+00001c30: 0a6f 626a 6563 7473 203d 2064 632e 6765  .objects = dc.ge
+00001c40: 745f 6f62 6a65 6374 7328 290a 0a66 6f72  t_objects()..for
+00001c50: 206f 626a 2069 6e20 6f62 6a65 6374 733a   obj in objects:
+00001c60: 0a20 2020 2070 7269 6e74 2866 227b 6f62  .    print(f"{ob
+00001c70: 6a2e 6170 694e 616d 657d 3a20 7b6f 626a  j.apiName}: {obj
+00001c80: 2e70 6c75 7261 6c4e 616d 657d 2c20 7b6f  .pluralName}, {o
+00001c90: 626a 2e73 696e 6775 6c61 724e 616d 657d  bj.singularName}
+00001ca0: 2229 0a60 6060 0a57 696c 6c20 6f75 7470  ").```.Will outp
+00001cb0: 7574 3a0a 6060 6062 6173 680a 436f 6d70  ut:.```bash.Comp
+00001cc0: 616e 793a 2043 6f6d 7061 6e69 6573 2c20  any: Companies, 
+00001cd0: 436f 6d70 616e 790a 436f 6e74 6163 743a  Company.Contact:
+00001ce0: 2043 6f6e 7461 6374 732c 2043 6f6e 7461   Contacts, Conta
+00001cf0: 6374 0a43 6f6d 7061 6e79 4164 6472 6573  ct.CompanyAddres
+00001d00: 733a 2043 6f6d 7061 6e79 2041 6464 7265  s: Company Addre
+00001d10: 7373 6573 2c20 436f 6d70 616e 7920 4164  sses, Company Ad
+00001d20: 6472 6573 730a 2e2e 2e65 7463 0a60 6060  dress....etc.```
+00001d30: 0a0a 2323 2047 6574 2046 6965 6c64 730a  ..## Get Fields.
+00001d40: 6044 6561 6c43 6c6f 7564 2e67 6574 5f66  `DealCloud.get_f
+00001d50: 6965 6c64 7328 2960 2070 726f 7669 6465  ields()` provide
+00001d60: 7320 7468 6520 6162 696c 6974 7920 746f  s the ability to
+00001d70: 2072 6574 7572 6e20 6669 656c 6473 2063   return fields c
+00001d80: 6f6e 6669 6775 7265 6420 696e 2074 6865  onfigured in the
+00001d90: 2073 6974 652e 2053 7065 6369 6669 6361   site. Specifica
+00001da0: 6c6c 792c 2061 6e20 6172 7261 7920 6f66  lly, an array of
+00001db0: 2060 4669 656c 6460 206f 626a 6563 7473   `Field` objects
+00001dc0: 2e0a 0a54 6865 7265 2061 7265 2074 6872  ...There are thr
+00001dd0: 6565 2077 6179 7320 746f 2071 7565 7279  ee ways to query
+00001de0: 2066 6f72 2066 6965 6c64 733a 0a31 2e20   for fields:.1. 
+00001df0: 5f5f 416c 6c20 4669 656c 6473 5f5f 3a20  __All Fields__: 
+00001e00: 6361 6c6c 2060 4465 616c 436c 6f75 642e  call `DealCloud.
+00001e10: 6765 745f 6669 656c 6473 2829 6020 7769  get_fields()` wi
+00001e20: 7468 206e 6f20 6172 6775 6d65 6e74 7320  th no arguments 
+00001e30: 746f 2072 6574 7572 6e20 616c 6c20 6669  to return all fi
+00001e40: 656c 6473 2e0a 0a60 6060 7079 7468 6f6e  elds...```python
+00001e50: 0a66 726f 6d20 6465 616c 636c 6f75 645f  .from dealcloud_
+00001e60: 7364 6b20 696d 706f 7274 2044 6561 6c43  sdk import DealC
+00001e70: 6c6f 7564 0a0a 6463 203d 2044 6561 6c43  loud..dc = DealC
+00001e80: 6c6f 7564 2e66 726f 6d5f 7961 6d6c 2822  loud.from_yaml("
+00001e90: 7061 7468 2f74 6f2f 7961 6d6c 5f63 6f6e  path/to/yaml_con
+00001ea0: 6669 675f 6669 6c65 2e6a 736f 6e22 290a  fig_file.json").
+00001eb0: 0a66 6965 6c64 7320 3d20 6463 2e67 6574  .fields = dc.get
+00001ec0: 5f66 6965 6c64 7328 290a 6060 600a 6066  _fields().```.`f
+00001ed0: 6965 6c64 7360 2077 696c 6c20 636f 6e74  ields` will cont
+00001ee0: 6169 6e20 6120 6c69 7374 206f 6620 6046  ain a list of `F
+00001ef0: 6965 6c64 6020 6f62 6a65 6374 7320 636f  ield` objects co
+00001f00: 6e74 6169 6e69 6e67 2061 6c6c 2063 6f6e  ntaining all con
+00001f10: 6669 6775 7265 6420 6669 656c 6473 2069  figured fields i
+00001f20: 6e20 7468 6520 7369 7465 2e0a 0a0a 322e  n the site....2.
+00001f30: 205f 5f41 6c6c 2046 6965 6c64 7320 666f   __All Fields fo
+00001f40: 7220 616e 204f 626a 6563 745f 5f3a 2063  r an Object__: c
+00001f50: 616c 6c20 6044 6561 6c43 6c6f 7564 2e67  all `DealCloud.g
+00001f60: 6574 5f66 6965 6c64 7328 6f62 6a65 6374  et_fields(object
+00001f70: 5f69 643d 224f 626a 6563 744e 616d 6522  _id="ObjectName"
+00001f80: 2960 2077 6974 6820 606f 626a 6563 745f  )` with `object_
+00001f90: 6964 6020 7365 7420 746f 2074 6865 2064  id` set to the d
+00001fa0: 6573 6972 6564 206f 626a 6563 7420 6170  esired object ap
+00001fb0: 6920 6e61 6d65 2c20 6f72 206f 626a 6563  i name, or objec
+00001fc0: 7420 6964 2c20 746f 2072 6574 7572 6e20  t id, to return 
+00001fd0: 616c 6c20 6669 656c 6473 2063 6f6e 6669  all fields confi
+00001fe0: 6775 7265 6420 666f 7220 7468 6174 206f  gured for that o
+00001ff0: 626a 6563 742e 0a0a 6060 6070 7974 686f  bject...```pytho
+00002000: 6e0a 6672 6f6d 2064 6561 6c63 6c6f 7564  n.from dealcloud
+00002010: 5f73 646b 2069 6d70 6f72 7420 4465 616c  _sdk import Deal
+00002020: 436c 6f75 640a 0a64 6320 3d20 4465 616c  Cloud..dc = Deal
+00002030: 436c 6f75 642e 6672 6f6d 5f79 616d 6c28  Cloud.from_yaml(
+00002040: 2270 6174 682f 746f 2f79 616d 6c5f 636f  "path/to/yaml_co
+00002050: 6e66 6967 5f66 696c 652e 6a73 6f6e 2229  nfig_file.json")
+00002060: 0a0a 6669 656c 6473 203d 2064 632e 6765  ..fields = dc.ge
+00002070: 745f 6669 656c 6473 2822 436f 6d70 616e  t_fields("Compan
+00002080: 7922 290a 6060 600a 6066 6965 6c64 7360  y").```.`fields`
+00002090: 2077 696c 6c20 636f 6e74 6169 6e20 6120   will contain a 
+000020a0: 6c69 7374 206f 6620 6046 6965 6c64 6020  list of `Field` 
+000020b0: 6f62 6a65 6374 732c 2063 6f6e 7461 696e  objects, contain
+000020c0: 696e 6720 616c 6c20 6669 656c 6473 2063  ing all fields c
+000020d0: 6f6e 6669 6775 7265 6420 696e 2074 6865  onfigured in the
+000020e0: 2022 436f 6d70 616e 7922 206f 626a 6563   "Company" objec
+000020f0: 742e 0a0a 0a33 2e20 5f5f 4120 4669 656c  t....3. __A Fiel
+00002100: 6420 6279 2046 6965 6c64 2049 445f 5f3a  d by Field ID__:
+00002110: 2063 616c 6c20 6044 6561 6c43 6c6f 7564   call `DealCloud
+00002120: 2e67 6574 5f66 6965 6c64 7328 6669 656c  .get_fields(fiel
+00002130: 645f 6964 3d31 3233 3429 6020 7769 7468  d_id=1234)` with
+00002140: 2060 6669 656c 645f 6964 6020 7365 7420   `field_id` set 
+00002150: 746f 2074 6865 2049 4420 6f66 2074 6865  to the ID of the
+00002160: 2064 6573 6972 6564 2066 6965 6c64 2e0a   desired field..
+00002170: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00002180: 6465 616c 636c 6f75 645f 7364 6b20 696d  dealcloud_sdk im
+00002190: 706f 7274 2044 6561 6c43 6c6f 7564 0a0a  port DealCloud..
+000021a0: 6463 203d 2044 6561 6c43 6c6f 7564 2e66  dc = DealCloud.f
+000021b0: 726f 6d5f 7961 6d6c 2822 7061 7468 2f74  rom_yaml("path/t
+000021c0: 6f2f 7961 6d6c 5f63 6f6e 6669 675f 6669  o/yaml_config_fi
+000021d0: 6c65 2e6a 736f 6e22 290a 0a66 6965 6c64  le.json")..field
+000021e0: 203d 2064 632e 6765 745f 6669 656c 6473   = dc.get_fields
+000021f0: 2866 6965 6c64 5f69 643d 3132 3334 290a  (field_id=1234).
+00002200: 6060 600a 6066 6965 6c64 6020 7769 6c6c  ```.`field` will
+00002210: 2063 6f6e 7461 696e 2061 2073 696e 676c   contain a singl
+00002220: 6520 6046 6965 6c64 6020 6f62 6a65 6374  e `Field` object
+00002230: 2c20 6465 7363 7269 6269 6e67 2074 6865  , describing the
+00002240: 2066 6965 6c64 2077 6974 6820 4944 2060   field with ID `
+00002250: 3132 3334 602e 0a0a 2323 2320 4765 7420  1234`...### Get 
+00002260: 5363 6865 6d61 0a60 4465 616c 436c 6f75  Schema.`DealClou
+00002270: 642e 6765 745f 7363 6865 6d61 2829 6020  d.get_schema()` 
+00002280: 6973 2061 206d 6574 686f 6420 7468 6174  is a method that
+00002290: 2077 696c 6c20 7265 7475 726e 2074 6865   will return the
+000022a0: 2066 756c 6c20 4465 616c 436c 6f75 6420   full DealCloud 
+000022b0: 7363 6865 6d61 2069 6e20 6120 7369 6e67  schema in a sing
+000022c0: 6c65 206f 626a 6563 742e 0a54 6865 206d  le object..The m
+000022d0: 6574 686f 6420 7461 6b65 7320 7468 6520  ethod takes the 
+000022e0: 6172 6775 6d65 6e74 3a20 606b 6579 5f74  argument: `key_t
+000022f0: 7970 6560 2c20 7768 6963 6820 6465 7363  ype`, which desc
+00002300: 7269 6265 7320 7768 6963 6820 6669 656c  ribes which fiel
+00002310: 6420 7769 6c6c 2062 6520 7573 6564 2061  d will be used a
+00002320: 7320 6b65 7973 2069 6e20 7468 6520 6e65  s keys in the ne
+00002330: 7374 6564 206f 626a 6563 7420 7374 7275  sted object stru
+00002340: 6374 7572 6520 6465 7363 7269 6269 6e67  cture describing
+00002350: 2074 6865 2073 6368 656d 612e 200a 0a54   the schema. ..T
+00002360: 6865 206f 7074 696f 6e73 2061 7265 3a0a  he options are:.
+00002370: 2d20 6061 7069 6020 2d20 5468 6520 4150  - `api` - The AP
+00002380: 4920 6e61 6d65 0a2d 2060 6469 7370 6c61  I name.- `displa
+00002390: 7960 202d 2054 6865 2064 6973 706c 6179  y` - The display
+000023a0: 206e 616d 650a 2d20 6069 6460 202d 2054   name.- `id` - T
+000023b0: 6865 206f 626a 6563 742f 6669 656c 6420  he object/field 
+000023c0: 4944 0a0a 5573 6167 6520 4578 616d 706c  ID..Usage Exampl
+000023d0: 653a 0a0a 6060 6070 7974 686f 6e0a 6672  e:..```python.fr
+000023e0: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
+000023f0: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
+00002400: 640a 0a64 6320 3d20 4465 616c 436c 6f75  d..dc = DealClou
+00002410: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
+00002420: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
+00002430: 5f66 696c 652e 6a73 6f6e 2229 0a0a 7363  _file.json")..sc
+00002440: 6865 6d61 203d 2064 632e 6765 745f 7363  hema = dc.get_sc
+00002450: 6865 6d61 2822 6170 6922 290a 6060 600a  hema("api").```.
+00002460: 6073 6368 656d 6160 2077 696c 6c20 636f  `schema` will co
+00002470: 6e74 6169 6e20 7468 6520 6120 6053 6368  ntain the a `Sch
+00002480: 656d 6160 206f 626a 6563 7420 7769 7468  ema` object with
+00002490: 2074 6865 2041 5049 206e 616d 6573 2061   the API names a
+000024a0: 7320 6b65 7973 2c20 6173 2062 656c 6f77  s keys, as below
+000024b0: 3a20 0a0a 6061 7069 6020 4578 616d 706c  : ..`api` Exampl
+000024c0: 653a 0a60 6060 7079 7468 6f6e 0a7b 0a20  e:.```python.{. 
+000024d0: 2022 436f 6d70 616e 7941 5049 4e61 6d65   "CompanyAPIName
+000024e0: 223a 207b 0a20 2020 2022 436f 6d70 616e  ": {.    "Compan
+000024f0: 794f 626a 6563 744d 6574 6144 6174 6122  yObjectMetaData"
+00002500: 3a20 222e 2e2e 222c 0a20 2020 2022 436f  : "...",.    "Co
+00002510: 6d70 616e 794f 626a 6563 7446 6965 6c64  mpanyObjectField
+00002520: 7322 3a20 7b0a 2020 2020 2020 2246 6965  s": {.      "Fie
+00002530: 6c64 3141 5049 4e61 6d65 223a 207b 0a20  ld1APIName": {. 
+00002540: 2020 2020 2020 2022 4669 656c 6431 4d65         "Field1Me
+00002550: 7461 4461 7461 223a 2022 2e2e 2e22 0a20  taData": "...". 
+00002560: 2020 2020 207d 0a20 2020 207d 0a20 207d       }.    }.  }
+00002570: 0a7d 0a60 6060 0a60 6469 7370 6c61 7960  .}.```.`display`
+00002580: 2045 7861 6d70 6c65 3a0a 6060 6070 7974   Example:.```pyt
+00002590: 686f 6e0a 7b0a 2020 2243 6f6d 7061 6e79  hon.{.  "Company
+000025a0: 2044 6973 706c 6179 204e 616d 6522 3a20   Display Name": 
+000025b0: 7b0a 2020 2020 2243 6f6d 7061 6e79 4f62  {.    "CompanyOb
+000025c0: 6a65 6374 4d65 7461 4461 7461 223a 2022  jectMetaData": "
+000025d0: 2e2e 2e22 2c0a 2020 2020 2243 6f6d 7061  ...",.    "Compa
+000025e0: 6e79 4f62 6a65 6374 4669 656c 6473 223a  nyObjectFields":
+000025f0: 207b 0a20 2020 2020 2022 4669 656c 6420   {.      "Field 
+00002600: 3120 4469 7370 6c61 7920 4e61 6d65 223a  1 Display Name":
+00002610: 207b 0a20 2020 2020 2020 2022 4669 656c   {.        "Fiel
+00002620: 6431 4d65 7461 4461 7461 223a 2022 2e2e  d1MetaData": "..
+00002630: 2e22 0a20 2020 2020 207d 0a20 2020 207d  .".      }.    }
+00002640: 0a20 207d 0a7d 0a60 6060 0a60 6964 6020  .  }.}.```.`id` 
+00002650: 4578 616d 706c 653a 0a3e 204e 6f74 6520  Example:.> Note 
+00002660: 7468 6520 4944 206f 6620 7468 6520 2243  the ID of the "C
+00002670: 6f6d 7061 6e79 2220 6f62 6a65 6374 2069  ompany" object i
+00002680: 7320 3132 3334 3520 616e 6420 7468 6520  s 12345 and the 
+00002690: 4944 206f 6620 7468 6520 2246 6965 6c64  ID of the "Field
+000026a0: 2031 2220 6669 656c 6420 6973 2031 3233   1" field is 123
+000026b0: 3435 3620 0a60 6060 7079 7468 6f6e 0a7b  456 .```python.{
+000026c0: 0a20 2031 3233 3435 3a20 7b0a 2020 2020  .  12345: {.    
+000026d0: 2243 6f6d 7061 6e79 4f62 6a65 6374 4d65  "CompanyObjectMe
+000026e0: 7461 4461 7461 223a 2022 2e2e 2e22 2c0a  taData": "...",.
+000026f0: 2020 2020 2243 6f6d 7061 6e79 4f62 6a65      "CompanyObje
+00002700: 6374 4669 656c 6473 223a 207b 0a20 2020  ctFields": {.   
+00002710: 2020 2031 3233 3435 363a 207b 0a20 2020     123456: {.   
+00002720: 2020 2020 2022 4669 656c 6431 4d65 7461       "Field1Meta
+00002730: 4461 7461 223a 2022 2e2e 2e22 0a20 2020  Data": "...".   
+00002740: 2020 207d 0a20 2020 207d 0a20 207d 0a7d     }.    }.  }.}
+00002750: 0a60 6060 0a0a 2323 2044 6174 6120 4f70  .```..## Data Op
+00002760: 6572 6174 696f 6e73 0a54 6865 2060 4465  erations.The `De
+00002770: 616c 436c 6f75 6460 206f 626a 6563 7420  alCloud` object 
+00002780: 7072 6f76 6964 6573 206d 6574 686f 6473  provides methods
+00002790: 2074 6f20 4372 6561 7465 2c20 5265 6164   to Create, Read
+000027a0: 2c20 5570 6461 7465 2061 6e64 2044 656c  , Update and Del
+000027b0: 6574 6520 6461 7461 2069 6e20 6275 6c6b  ete data in bulk
+000027c0: 2e20 4173 2069 7473 2064 6566 6175 6c74  . As its default
+000027d0: 2062 6568 6176 696f 7572 2c20 7768 656e   behaviour, when
+000027e0: 2077 6f72 6b69 6e67 2077 6974 6820 7369   working with si
+000027f0: 7465 2064 6174 612c 2074 6865 206c 6962  te data, the lib
+00002800: 7261 7279 2075 7365 7320 4461 7461 4672  rary uses DataFr
+00002810: 616d 6573 2077 6974 680a 7468 6520 5b50  ames with.the [P
+00002820: 616e 6461 735d 2868 7474 7073 3a2f 2f70  andas](https://p
+00002830: 616e 6461 732e 7079 6461 7461 2e6f 7267  andas.pydata.org
+00002840: 2f29 206c 6962 7261 7279 2c20 686f 7765  /) library, howe
+00002850: 7665 7220 7468 6520 6f70 7469 6f6e 2069  ver the option i
+00002860: 7320 6176 6169 6c61 626c 6520 666f 7220  s available for 
+00002870: 6974 2074 6f20 776f 726b 2077 6974 6820  it to work with 
+00002880: 6a75 7374 2070 7974 686f 6e20 7374 616e  just python stan
+00002890: 6461 7264 2064 6174 6120 7479 7065 732e  dard data types.
+000028a0: 0a0a 2323 2320 4c69 7374 2043 6f6e 6669  ..### List Confi
+000028b0: 6775 7265 6420 5669 6577 730a 6044 6561  gured Views.`Dea
+000028c0: 6c43 6c6f 7564 2e6c 6973 745f 636f 6e66  lCloud.list_conf
+000028d0: 6967 7572 6564 5f76 6965 7773 2829 6020  igured_views()` 
+000028e0: 7265 7475 726e 7320 6120 6052 6f77 7360  returns a `Rows`
+000028f0: 206f 626a 6563 7420 636f 6e74 6169 6e69   object containi
+00002900: 6e67 2061 6c6c 2063 6f6e 6669 6775 7265  ng all configure
+00002910: 6420 7669 6577 7320 696e 2074 6865 2073  d views in the s
+00002920: 6974 652e 0a54 6865 2061 7267 756d 656e  ite..The argumen
+00002930: 7420 6069 735f 7072 6976 6174 6560 2063  t `is_private` c
+00002940: 616e 2062 6520 7061 7373 6564 2061 7320  an be passed as 
+00002950: 6120 626f 6f6c 6561 6e2c 2077 6865 7265  a boolean, where
+00002960: 2069 6620 7472 7565 2c20 6f6e 6c79 2070   if true, only p
+00002970: 7269 7661 7465 2076 6965 7773 2074 6f20  rivate views to 
+00002980: 2869 6e63 6c75 6469 6e67 2076 6965 7773  (including views
+00002990: 2073 6861 7265 6420 7769 7468 2920 7468   shared with) th
+000029a0: 6520 6175 7468 656e 7469 6361 7465 6420  e authenticated 
+000029b0: 7573 6572 2077 696c 6c20 6265 2072 6574  user will be ret
+000029c0: 7572 6e65 642e 0a0a 4578 616d 706c 653a  urned...Example:
+000029d0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+000029e0: 2064 6561 6c63 6c6f 7564 5f73 646b 2069   dealcloud_sdk i
+000029f0: 6d70 6f72 7420 4465 616c 436c 6f75 640a  mport DealCloud.
+00002a00: 0a64 6320 3d20 4465 616c 436c 6f75 642e  .dc = DealCloud.
+00002a10: 6672 6f6d 5f79 616d 6c28 2270 6174 682f  from_yaml("path/
+00002a20: 746f 2f79 616d 6c5f 636f 6e66 6967 5f66  to/yaml_config_f
+00002a30: 696c 652e 6a73 6f6e 2229 0a0a 7669 6577  ile.json")..view
+00002a40: 7320 3d20 6463 2e6c 6973 745f 636f 6e66  s = dc.list_conf
+00002a50: 6967 7572 6564 5f76 6965 7773 2829 0a60  igured_views().`
+00002a60: 6060 0a60 7669 6577 7360 2077 696c 6c20  ``.`views` will 
+00002a70: 636f 6e74 6169 6e20 6120 7375 6d6d 6172  contain a summar
+00002a80: 7920 6f66 2063 6f6e 6669 6775 7265 6420  y of configured 
+00002a90: 7669 6577 732e 0a0a 2323 2320 5265 6164  views...### Read
+00002aa0: 2044 6174 610a 6044 6561 6c43 6c6f 7564   Data.`DealCloud
+00002ab0: 2e72 6561 645f 6461 7461 2829 6020 616c  .read_data()` al
+00002ac0: 6c6f 7773 2075 7365 7273 2074 6f20 7265  lows users to re
+00002ad0: 6164 2064 6174 6120 6672 6f6d 2061 2044  ad data from a D
+00002ae0: 6561 6c43 6c6f 7564 206f 626a 6563 7420  ealCloud object 
+00002af0: 696e 746f 2061 2060 7061 6e64 6173 2e44  into a `pandas.D
+00002b00: 6174 6146 7261 6d65 6020 6f72 2061 206c  ataFrame` or a l
+00002b10: 6973 7420 6f66 2070 7974 686f 6e20 6469  ist of python di
+00002b20: 6374 696f 6e61 7269 6573 2e0a 3e20 5b21  ctionaries..> [!
+00002b30: 494d 504f 5254 414e 545d 200a 3e20 4f6e  IMPORTANT] .> On
+00002b40: 6c79 206f 6e65 206f 6620 6f62 6a65 6374  ly one of object
+00002b50: 5f69 6420 6f72 2076 6965 775f 6964 2063  _id or view_id c
+00002b60: 616e 2062 6520 706f 7075 6c61 7465 640a  an be populated.
+00002b70: 2020 2020 2020 2020 0a41 7267 756d 656e          .Argumen
+00002b80: 7473 3a0a 0a2d 206f 626a 6563 745f 6964  ts:..- object_id
+00002b90: 2060 556e 696f 6e5b 696e 742c 2073 7472   `Union[int, str
+00002ba0: 5d60 3a20 7468 6520 6f62 6a65 6374 2074  ]`: the object t
+00002bb0: 6f20 7075 6c6c 2064 6174 6120 6672 6f6d  o pull data from
+00002bc0: 0a2d 2076 6965 775f 6964 2060 556e 696f  .- view_id `Unio
+00002bd0: 6e5b 696e 742c 2073 7472 5d60 3a20 7468  n[int, str]`: th
+00002be0: 6520 7669 6577 2074 6f20 7075 6c6c 2064  e view to pull d
+00002bf0: 6174 6120 6672 6f6d 0a2d 206f 7574 7075  ata from.- outpu
+00002c00: 7420 6073 7472 603a 2060 7061 6e64 6173  t `str`: `pandas
+00002c10: 6020 6f72 2060 6c69 7374 602c 2064 6563  ` or `list`, dec
+00002c20: 6964 6573 2074 6865 206f 7574 7075 7420  ides the output 
+00002c30: 666f 726d 6174 2c20 6070 616e 6461 7360  format, `pandas`
+00002c40: 2069 7320 6465 6661 756c 740a 2d20 7265   is default.- re
+00002c50: 736f 6c76 6520 6073 7472 603a 2066 6f72  solve `str`: for
+00002c60: 2070 616e 6461 732c 2077 6865 7265 2066   pandas, where f
+00002c70: 6965 6c64 7320 636f 6e74 6169 6e20 616e  ields contain an
+00002c80: 206f 626a 6563 7420 2863 686f 6963 652c   object (choice,
+00002c90: 2072 6566 6572 656e 6365 2c20 7573 6572   reference, user
+00002ca0: 292c 2072 6573 6f6c 7665 2074 6f20 7468  ), resolve to th
+00002cb0: 6520 6964 206f 7220 6e61 6d65 0a2d 2076  e id or name.- v
+00002cc0: 6965 775f 6669 6c74 6572 2060 6c69 7374  iew_filter `list
+00002cd0: 5b64 6963 745d 603a 2063 6f6c 756d 6e20  [dict]`: column 
+00002ce0: 7175 6572 6965 7320 746f 2022 7375 7070  queries to "supp
+00002cf0: 6c79 2076 616c 7565 206c 6174 6572 2220  ly value later" 
+00002d00: 696e 2076 6965 7773 2c20 7365 653a 2068  in views, see: h
+00002d10: 7474 7073 3a2f 2f61 7069 2e64 6f63 732e  ttps://api.docs.
+00002d20: 6465 616c 636c 6f75 642e 636f 6d2f 646f  dealcloud.com/do
+00002d30: 6373 2f64 6174 612f 726f 7773 2f76 6965  cs/data/rows/vie
+00002d40: 775f 6465 7461 696c 730a 2d20 6669 656c  w_details.- fiel
+00002d50: 6473 2060 6c69 7374 5b73 7472 5d60 3a20  ds `list[str]`: 
+00002d60: 6966 206e 6f74 2060 4e6f 6e65 602c 2072  if not `None`, r
+00002d70: 6574 7572 6e20 6f6e 6c79 2066 6965 6c64  eturn only field
+00002d80: 7320 696e 2074 6865 206c 6973 742e 200a  s in the list. .
+00002d90: 2d20 7175 6572 7920 6073 7472 603a 2061  - query `str`: a
+00002da0: 2044 6561 6c43 6c6f 7564 2072 6f77 7320   DealCloud rows 
+00002db0: 7175 6572 7920 7374 7269 6e67 2074 6f20  query string to 
+00002dc0: 7265 7175 6573 7420 7370 6563 6966 6963  request specific
+00002dd0: 2069 6e66 6f72 6d61 7469 6f6e 2c20 7365   information, se
+00002de0: 653a 2068 7474 7073 3a2f 2f61 7069 2e64  e: https://api.d
+00002df0: 6f63 732e 6465 616c 636c 6f75 642e 636f  ocs.dealcloud.co
+00002e00: 6d2f 646f 6373 2f64 6174 612f 726f 7773  m/docs/data/rows
+00002e10: 2f71 7565 7279 0a2d 2069 6e63 6c75 6465  /query.- include
+00002e20: 5f6e 756c 6c73 2060 626f 6f6c 603a 2069  _nulls `bool`: i
+00002e30: 6620 7472 7565 2c20 6e75 6c6c 2063 6f6c  f true, null col
+00002e40: 756d 6e73 2077 696c 6c20 616c 736f 2062  umns will also b
+00002e50: 6520 7265 7475 726e 6564 0a2d 2063 6f6c  e returned.- col
+00002e60: 756d 6e5f 6865 6164 6572 7320 6073 7472  umn_headers `str
+00002e70: 603a 2073 7065 6369 6669 6573 2074 6865  `: specifies the
+00002e80: 2076 616c 7565 2074 7970 6520 6f66 2074   value type of t
+00002e90: 6865 2072 6574 7572 6e20 6669 656c 6420  he return field 
+00002ea0: 6b65 7973 2f63 6f6c 756d 6e20 6e61 6d65  keys/column name
+00002eb0: 732e 0a20 202d 2060 6170 6960 203d 2046  s..  - `api` = F
+00002ec0: 6965 6c64 2041 5049 204e 616d 650a 2020  ield API Name.  
+00002ed0: 2d20 606e 616d 6560 203d 2046 6965 6c64  - `name` = Field
+00002ee0: 2044 6973 706c 6179 204e 616d 650a 2020   Display Name.  
+00002ef0: 2d20 6069 6460 203d 2046 6965 6c64 2049  - `id` = Field I
+00002f00: 440a 0a23 2323 2320 5265 6164 696e 6720  D..#### Reading 
+00002f10: 4461 7461 2066 726f 6d20 616e 204f 626a  Data from an Obj
+00002f20: 6563 740a 4578 616d 706c 653a 0a0a 6060  ect.Example:..``
+00002f30: 6070 7974 686f 6e0a 6672 6f6d 2064 6561  `python.from dea
+00002f40: 6c63 6c6f 7564 5f73 646b 2069 6d70 6f72  lcloud_sdk impor
+00002f50: 7420 4465 616c 436c 6f75 640a 0a64 6320  t DealCloud..dc 
+00002f60: 3d20 4465 616c 436c 6f75 642e 6672 6f6d  = DealCloud.from
+00002f70: 5f79 616d 6c28 2270 6174 682f 746f 2f79  _yaml("path/to/y
+00002f80: 616d 6c5f 636f 6e66 6967 5f66 696c 652e  aml_config_file.
+00002f90: 6a73 6f6e 2229 0a0a 6461 7461 203d 2064  json")..data = d
+00002fa0: 632e 7265 6164 5f64 6174 6128 2243 6f6d  c.read_data("Com
+00002fb0: 7061 6e79 2229 0a60 6060 0a60 6461 7461  pany").```.`data
+00002fc0: 6020 7769 6c6c 2062 6520 6120 6070 616e  ` will be a `pan
+00002fd0: 6461 732e 4461 7461 4672 616d 6560 2061  das.DataFrame` a
+00002fe0: 7320 6265 6c6f 773a 0a0a 7c20 456e 7472  s below:..| Entr
+00002ff0: 7949 6420 7c20 436f 6d70 616e 794e 616d  yId | CompanyNam
+00003000: 6520 7c20 436f 6d70 616e 7954 7970 6520  e | CompanyType 
+00003010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003060: 2020 2020 2020 2020 2020 207c 0a7c 2d2d             |.|--
+00003070: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
+00003080: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
+00003090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000030a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000030b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000030c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000030d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000030e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  --------------|.
+000030f0: 7c20 3132 3334 3520 2020 7c20 436f 6d70  | 12345   | Comp
+00003100: 616e 7931 2020 2020 7c20 5b7b 2773 6571  any1    | [{'seq
+00003110: 4e75 6d62 6572 273a 2033 2c20 2769 7341  Number': 3, 'isA
+00003120: 7574 6f50 6466 273a 2046 616c 7365 2c20  utoPdf': False, 
+00003130: 2769 6427 3a20 3331 3937 3738 302c 2027  'id': 3197780, '
+00003140: 6e61 6d65 273a 2027 4c69 6d69 7465 6420  name': 'Limited 
+00003150: 5061 7274 6e65 7227 2c20 2765 6e74 7279  Partner', 'entry
+00003160: 4c69 7374 4964 273a 202d 367d 5d20 2020  ListId': -6}]   
+00003170: 207c 0a7c 2031 3233 3436 2020 207c 2043   |.| 12346   | C
+00003180: 6f6d 7061 6e79 3220 2020 207c 205b 7b27  ompany2    | [{'
+00003190: 7365 714e 756d 6265 7227 3a20 312c 2027  seqNumber': 1, '
+000031a0: 6973 4175 746f 5064 6627 3a20 4661 6c73  isAutoPdf': Fals
+000031b0: 652c 2027 6964 273a 2033 3139 3737 3832  e, 'id': 3197782
+000031c0: 2c20 276e 616d 6527 3a20 274f 7065 7261  , 'name': 'Opera
+000031d0: 7469 6e67 2043 6f6d 7061 6e79 272c 2027  ting Company', '
+000031e0: 656e 7472 794c 6973 7449 6427 3a20 2d36  entryListId': -6
+000031f0: 7d5d 2020 7c0a 7c20 3132 3334 3720 2020  }]  |.| 12347   
+00003200: 7c20 436f 6d70 616e 7933 2020 2020 7c20  | Company3    | 
+00003210: 5b7b 2773 6571 4e75 6d62 6572 273a 2033  [{'seqNumber': 3
+00003220: 2c20 2769 7341 7574 6f50 6466 273a 2046  , 'isAutoPdf': F
+00003230: 616c 7365 2c20 2769 6427 3a20 3331 3937  alse, 'id': 3197
+00003240: 3738 302c 2027 6e61 6d65 273a 2027 4c69  780, 'name': 'Li
+00003250: 6d69 7465 6420 5061 7274 6e65 7227 2c20  mited Partner', 
+00003260: 2765 6e74 7279 4c69 7374 4964 273a 202d  'entryListId': -
+00003270: 367d 5d20 2020 207c 0a0a 546f 2072 6574  6}]    |..To ret
+00003280: 7572 6e20 6120 7079 7468 6f6e 2060 6c69  urn a python `li
+00003290: 7374 6020 696e 7374 6561 6420 6f66 2061  st` instead of a
+000032a0: 2060 7061 6e64 6173 2e44 6174 6146 7261   `pandas.DataFra
+000032b0: 6d65 603a 0a0a 6060 6070 7974 686f 6e0a  me`:..```python.
+000032c0: 6672 6f6d 2064 6561 6c63 6c6f 7564 5f73  from dealcloud_s
+000032d0: 646b 2069 6d70 6f72 7420 4465 616c 436c  dk import DealCl
+000032e0: 6f75 640a 0a64 6320 3d20 4465 616c 436c  oud..dc = DealCl
+000032f0: 6f75 642e 6672 6f6d 5f79 616d 6c28 2270  oud.from_yaml("p
+00003300: 6174 682f 746f 2f79 616d 6c5f 636f 6e66  ath/to/yaml_conf
+00003310: 6967 5f66 696c 652e 6a73 6f6e 2229 0a0a  ig_file.json")..
+00003320: 6461 7461 203d 2064 632e 7265 6164 5f64  data = dc.read_d
+00003330: 6174 6128 2243 6f6d 7061 6e79 222c 206f  ata("Company", o
+00003340: 7574 7075 743d 226c 6973 7422 290a 6060  utput="list").``
+00003350: 600a 6064 6174 6160 2077 696c 6c20 6265  `.`data` will be
+00003360: 2061 2060 6c69 7374 6020 6f66 2060 6469   a `list` of `di
+00003370: 6374 6073 2061 7320 6265 6c6f 773a 0a60  ct`s as below:.`
+00003380: 6060 7079 7468 6f6e 0a5b 0a20 2020 207b  ``python.[.    {
+00003390: 0a20 2020 2020 2020 2027 456e 7472 7949  .        'EntryI
+000033a0: 6427 3a20 3132 3334 352c 0a20 2020 2020  d': 12345,.     
+000033b0: 2020 2027 436f 6d70 616e 794e 616d 6527     'CompanyName'
+000033c0: 3a20 2743 6f6d 7061 6e79 3127 2c0a 2020  : 'Company1',.  
+000033d0: 2020 2020 2020 2743 6f6d 7061 6e79 5479        'CompanyTy
+000033e0: 7065 273a 205b 0a20 2020 2020 2020 2020  pe': [.         
+000033f0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00003400: 2020 2020 2020 2773 6571 4e75 6d62 6572        'seqNumber
+00003410: 273a 2033 2c0a 2020 2020 2020 2020 2020  ': 3,.          
+00003420: 2020 2020 2020 2769 7341 7574 6f50 6466        'isAutoPdf
+00003430: 273a 2046 616c 7365 2c0a 2020 2020 2020  ': False,.      
+00003440: 2020 2020 2020 2020 2020 2769 6427 3a20            'id': 
+00003450: 3331 3937 3738 302c 0a20 2020 2020 2020  3197780,.       
+00003460: 2020 2020 2020 2020 2027 6e61 6d65 273a           'name':
+00003470: 2027 4c69 6d69 7465 6420 5061 7274 6e65   'Limited Partne
+00003480: 7227 2c0a 2020 2020 2020 2020 2020 2020  r',.            
+00003490: 2020 2020 2765 6e74 7279 4c69 7374 4964      'entryListId
+000034a0: 273a 202d 360a 2020 2020 2020 2020 2020  ': -6.          
+000034b0: 2020 207d 0a20 2020 2020 2020 5d2c 0a20     }.       ],. 
+000034c0: 2020 207d 2c0a 2020 2020 7b0a 2020 2020     },.    {.    
+000034d0: 2020 2745 6e74 7279 4964 273a 2031 3233    'EntryId': 123
+000034e0: 3436 2c0a 2020 2020 2020 2743 6f6d 7061  46,.      'Compa
+000034f0: 6e79 4e61 6d65 273a 2027 436f 6d70 616e  nyName': 'Compan
+00003500: 7932 272c 0a20 2020 2020 2027 436f 6d70  y2',.      'Comp
+00003510: 616e 7954 7970 6527 3a20 5b0a 2020 2020  anyType': [.    
+00003520: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00003530: 2020 2027 7365 714e 756d 6265 7227 3a20     'seqNumber': 
+00003540: 312c 0a20 2020 2020 2020 2020 2020 2027  1,.            '
+00003550: 6973 4175 746f 5064 6627 3a20 4661 6c73  isAutoPdf': Fals
+00003560: 652c 0a20 2020 2020 2020 2020 2020 2027  e,.            '
+00003570: 6964 273a 2033 3139 3737 3832 2c0a 2020  id': 3197782,.  
+00003580: 2020 2020 2020 2020 2020 276e 616d 6527            'name'
+00003590: 3a20 274f 7065 7261 7469 6e67 2043 6f6d  : 'Operating Com
+000035a0: 7061 6e79 272c 0a20 2020 2020 2020 2020  pany',.         
+000035b0: 2020 2027 656e 7472 794c 6973 7449 6427     'entryListId'
+000035c0: 3a20 2d36 0a20 2020 2020 2020 2020 7d0a  : -6.         }.
+000035d0: 2020 2020 2020 5d0a 2020 2020 7d2c 0a20        ].    },. 
+000035e0: 2020 207b 0a20 2020 2020 2020 2745 6e74     {.       'Ent
+000035f0: 7279 4964 273a 2031 3233 3437 2c0a 2020  ryId': 12347,.  
+00003600: 2020 2020 2020 2743 6f6d 7061 6e79 4e61        'CompanyNa
+00003610: 6d65 273a 2027 436f 6d70 616e 7933 272c  me': 'Company3',
+00003620: 0a20 2020 2020 2020 2027 436f 6d70 616e  .        'Compan
+00003630: 7954 7970 6527 3a20 5b0a 2020 2020 2020  yType': [.      
+00003640: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00003650: 2020 2020 2020 2027 7365 714e 756d 6265         'seqNumbe
+00003660: 7227 3a20 342c 0a20 2020 2020 2020 2020  r': 4,.         
+00003670: 2020 2020 2020 2027 6973 4175 746f 5064         'isAutoPd
+00003680: 6627 3a20 4661 6c73 652c 0a20 2020 2020  f': False,.     
+00003690: 2020 2020 2020 2020 2020 2027 6964 273a             'id':
+000036a0: 2033 3139 3737 3739 2c0a 2020 2020 2020   3197779,.      
+000036b0: 2020 2020 2020 2020 2020 276e 616d 6527            'name'
+000036c0: 3a20 2753 6572 7669 6365 2050 726f 7669  : 'Service Provi
+000036d0: 6465 7227 2c0a 2020 2020 2020 2020 2020  der',.          
+000036e0: 2020 2020 2020 2765 6e74 7279 4c69 7374        'entryList
+000036f0: 4964 273a 202d 360a 2020 2020 2020 2020  Id': -6.        
+00003700: 2020 207d 0a20 2020 2020 2020 205d 0a20     }.        ]. 
+00003710: 2020 207d 2c0a 205d 0a60 6060 0a0a 2323     },. ].```..##
+00003720: 2323 2320 5265 736f 6c76 696e 6720 746f  ### Resolving to
+00003730: 204e 616d 6520 6f72 2074 6f20 4944 0a3e   Name or to ID.>
+00003740: 205b 214e 4f54 455d 0a3e 2054 6865 2066   [!NOTE].> The f
+00003750: 6f6c 6c6f 7769 6e67 206d 6574 686f 6473  ollowing methods
+00003760: 206f 6e6c 7920 6170 706c 7920 746f 2077   only apply to w
+00003770: 6865 7265 2061 2060 7061 6e64 6173 2e44  here a `pandas.D
+00003780: 6174 6146 7261 6d65 6020 6973 2072 6574  ataFrame` is ret
+00003790: 7572 6e65 642e 0a0a 4368 6f69 6365 2c20  urned...Choice, 
+000037a0: 5265 6665 7265 6e63 6520 616e 6420 5573  Reference and Us
+000037b0: 6572 2066 6965 6c64 7320 6170 7065 6172  er fields appear
+000037c0: 2061 7320 6c69 7374 7320 6f66 2064 6963   as lists of dic
+000037d0: 7469 6f6e 6172 6965 7320 6173 2073 6565  tionaries as see
+000037e0: 6e20 696e 2074 6865 205b 6162 6f76 6520  n in the [above 
+000037f0: 6578 616d 706c 655d 2823 7265 6164 696e  example](#readin
+00003800: 672d 6461 7461 2d66 726f 6d2d 616e 2d6f  g-data-from-an-o
+00003810: 626a 6563 7429 2062 7920 6465 6661 756c  bject) by defaul
+00003820: 742e 0a0a 546f 2072 6573 6f6c 7665 2074  t...To resolve t
+00003830: 6865 7365 2066 6965 6c64 7320 746f 2061  hese fields to a
+00003840: 206d 6f72 6520 7265 6164 6162 6c65 2060   more readable `
+00003850: 6e61 6d65 6020 7661 6c75 653a 0a0a 6060  name` value:..``
+00003860: 6070 7974 686f 6e0a 6672 6f6d 2064 6561  `python.from dea
+00003870: 6c63 6c6f 7564 5f73 646b 2069 6d70 6f72  lcloud_sdk impor
+00003880: 7420 4465 616c 436c 6f75 640a 0a64 6320  t DealCloud..dc 
+00003890: 3d20 4465 616c 436c 6f75 642e 6672 6f6d  = DealCloud.from
+000038a0: 5f79 616d 6c28 2270 6174 682f 746f 2f79  _yaml("path/to/y
+000038b0: 616d 6c5f 636f 6e66 6967 5f66 696c 652e  aml_config_file.
+000038c0: 6a73 6f6e 2229 0a0a 6461 7461 203d 2064  json")..data = d
+000038d0: 632e 7265 6164 5f64 6174 6128 2243 6f6d  c.read_data("Com
+000038e0: 7061 6e79 222c 2072 6573 6f6c 7665 3d22  pany", resolve="
+000038f0: 6e61 6d65 2229 0a60 6060 0a60 6461 7461  name").```.`data
+00003900: 6020 7769 6c6c 2062 6520 6120 6070 616e  ` will be a `pan
+00003910: 6461 732e 4461 7461 4672 616d 6560 2061  das.DataFrame` a
+00003920: 7320 6265 6c6f 773a 0a0a 7c20 456e 7472  s below:..| Entr
+00003930: 7949 6420 7c20 436f 6d70 616e 794e 616d  yId | CompanyNam
+00003940: 6520 7c20 436f 6d70 616e 7954 7970 6520  e | CompanyType 
+00003950: 2020 2020 2020 207c 0a7c 2d2d 2d2d 2d2d         |.|------
+00003960: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
+00003970: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
+00003980: 2d2d 2d2d 2d2d 7c0a 7c20 3132 3334 3520  ------|.| 12345 
+00003990: 2020 7c20 436f 6d70 616e 7931 2020 2020    | Company1    
+000039a0: 7c20 4c69 6d69 7465 6420 5061 7274 6e65  | Limited Partne
+000039b0: 7220 2020 207c 0a7c 2031 3233 3436 2020  r    |.| 12346  
+000039c0: 207c 2043 6f6d 7061 6e79 3220 2020 207c   | Company2    |
+000039d0: 204f 7065 7261 7469 6e67 2043 6f6d 7061   Operating Compa
+000039e0: 6e79 2020 7c0a 7c20 3132 3334 3720 2020  ny  |.| 12347   
+000039f0: 7c20 436f 6d70 616e 7933 2020 2020 7c20  | Company3    | 
+00003a00: 4c69 6d69 7465 6420 5061 7274 6e65 7220  Limited Partner 
+00003a10: 2020 207c 0a0a 546f 2072 6573 6f6c 7665     |..To resolve
+00003a20: 2074 6865 2066 6965 6c64 7320 746f 2061   the fields to a
+00003a30: 6e20 6069 6460 2076 616c 7565 3a0a 0a60  n `id` value:..`
+00003a40: 6060 7079 7468 6f6e 0a66 726f 6d20 6465  ``python.from de
+00003a50: 616c 636c 6f75 645f 7364 6b20 696d 706f  alcloud_sdk impo
+00003a60: 7274 2044 6561 6c43 6c6f 7564 0a0a 6463  rt DealCloud..dc
+00003a70: 203d 2044 6561 6c43 6c6f 7564 2e66 726f   = DealCloud.fro
+00003a80: 6d5f 7961 6d6c 2822 7061 7468 2f74 6f2f  m_yaml("path/to/
+00003a90: 7961 6d6c 5f63 6f6e 6669 675f 6669 6c65  yaml_config_file
+00003aa0: 2e6a 736f 6e22 290a 0a64 6174 6120 3d20  .json")..data = 
+00003ab0: 6463 2e72 6561 645f 6461 7461 2822 436f  dc.read_data("Co
+00003ac0: 6d70 616e 7922 2c20 7265 736f 6c76 653d  mpany", resolve=
+00003ad0: 2269 6422 290a 6060 600a 6064 6174 6160  "id").```.`data`
+00003ae0: 2077 696c 6c20 6265 2061 2060 7061 6e64   will be a `pand
+00003af0: 6173 2e44 6174 6146 7261 6d65 6020 6173  as.DataFrame` as
+00003b00: 2062 656c 6f77 3a0a 0a7c 2045 6e74 7279   below:..| Entry
+00003b10: 4964 207c 2043 6f6d 7061 6e79 4e61 6d65  Id | CompanyName
+00003b20: 207c 2043 6f6d 7061 6e79 5479 7065 207c   | CompanyType |
+00003b30: 0a7c 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  .|---------|----
+00003b40: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
+00003b50: 2d2d 2d2d 2d2d 2d7c 0a7c 2031 3233 3435  -------|.| 12345
+00003b60: 2020 207c 2043 6f6d 7061 6e79 3120 2020     | Company1   
+00003b70: 207c 2033 3139 3737 3830 2020 2020 207c   | 3197780     |
+00003b80: 0a7c 2031 3233 3436 2020 207c 2043 6f6d  .| 12346   | Com
+00003b90: 7061 6e79 3220 2020 207c 2033 3139 3737  pany2    | 31977
+00003ba0: 3832 2020 2020 207c 0a7c 2031 3233 3437  82     |.| 12347
+00003bb0: 2020 207c 2043 6f6d 7061 6e79 3320 2020     | Company3   
+00003bc0: 207c 2033 3139 3737 3830 2020 2020 207c   | 3197780     |
+00003bd0: 0a0a 2323 2323 2320 5265 6164 696e 6720  ..##### Reading 
+00003be0: 6120 5375 6273 6574 206f 6620 4669 656c  a Subset of Fiel
+00003bf0: 6473 0a54 6f20 7265 6164 2061 2073 7065  ds.To read a spe
+00003c00: 6369 6669 6320 7365 7420 6f66 2066 6965  cific set of fie
+00003c10: 6c64 7320 6672 6f6d 2061 6e20 6f62 6a65  lds from an obje
+00003c20: 6374 2c20 7061 7373 2061 206c 6973 7420  ct, pass a list 
+00003c30: 6f66 2044 6561 6c43 6c6f 7564 2066 6965  of DealCloud fie
+00003c40: 6c64 2041 5049 206e 616d 6573 2074 6f20  ld API names to 
+00003c50: 7468 6520 6172 6775 6d65 6e74 2060 6669  the argument `fi
+00003c60: 656c 6473 603a 0a0a 6060 6070 7974 686f  elds`:..```pytho
+00003c70: 6e0a 6672 6f6d 2064 6561 6c63 6c6f 7564  n.from dealcloud
+00003c80: 5f73 646b 2069 6d70 6f72 7420 4465 616c  _sdk import Deal
+00003c90: 436c 6f75 640a 0a64 6320 3d20 4465 616c  Cloud..dc = Deal
+00003ca0: 436c 6f75 642e 6672 6f6d 5f79 616d 6c28  Cloud.from_yaml(
+00003cb0: 2270 6174 682f 746f 2f79 616d 6c5f 636f  "path/to/yaml_co
+00003cc0: 6e66 6967 5f66 696c 652e 6a73 6f6e 2229  nfig_file.json")
+00003cd0: 0a0a 6461 7461 203d 2064 632e 7265 6164  ..data = dc.read
+00003ce0: 5f64 6174 6128 2243 6f6d 7061 6e79 222c  _data("Company",
+00003cf0: 2066 6965 6c64 733d 5b22 436f 6d70 616e   fields=["Compan
+00003d00: 794e 616d 6522 5d29 0a60 6060 0a60 6461  yName"]).```.`da
+00003d10: 7461 6020 7769 6c6c 2062 6520 6120 6070  ta` will be a `p
+00003d20: 616e 6461 732e 4461 7461 4672 616d 6560  andas.DataFrame`
+00003d30: 2061 7320 6265 6c6f 773a 0a0a 7c20 456e   as below:..| En
+00003d40: 7472 7949 6420 7c20 436f 6d70 616e 794e  tryId | CompanyN
+00003d50: 616d 6520 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d  ame |.|---------
+00003d60: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  |-------------|.
+00003d70: 7c20 3132 3334 3520 2020 7c20 436f 6d70  | 12345   | Comp
+00003d80: 616e 7931 2020 2020 7c0a 7c20 3132 3334  any1    |.| 1234
+00003d90: 3620 2020 7c20 436f 6d70 616e 7932 2020  6   | Company2  
+00003da0: 2020 7c0a 7c20 3132 3334 3720 2020 7c20    |.| 12347   | 
+00003db0: 436f 6d70 616e 7933 2020 2020 7c0a 0a23  Company3    |..#
+00003dc0: 2323 2323 2055 7369 6e67 2051 7565 7269  #### Using Queri
+00003dd0: 6573 2074 6f20 5265 6164 2044 6174 610a  es to Read Data.
+00003de0: 4120 7175 6572 7920 6361 6e20 6265 2070  A query can be p
+00003df0: 6173 7365 6420 746f 2074 6865 2044 6561  assed to the Dea
+00003e00: 6c43 6c6f 7564 2072 6571 7565 7374 2066  lCloud request f
+00003e10: 6f72 2064 6174 6120 746f 2072 6574 7572  or data to retur
+00003e20: 6e20 6d6f 7265 2073 7065 6369 6669 6320  n more specific 
+00003e30: 696e 666f 726d 6174 696f 6e2c 2061 6e64  information, and
+00003e40: 2072 6564 7563 6520 7468 6520 766f 6c75   reduce the volu
+00003e50: 6d65 206f 6620 696e 636f 6d69 6e67 2064  me of incoming d
+00003e60: 6174 612e 0a54 6f20 7573 6520 6120 7175  ata..To use a qu
+00003e70: 6572 792c 2070 6173 7320 7468 6520 7175  ery, pass the qu
+00003e80: 6572 7920 7374 7269 6e67 2074 6f20 7468  ery string to th
+00003e90: 6520 6071 7565 7279 6020 6172 6775 6d65  e `query` argume
+00003ea0: 6e74 2e0a 5468 6520 6176 6169 6c61 626c  nt..The availabl
+00003eb0: 6520 7175 6572 7920 6f70 6572 6174 696f  e query operatio
+00003ec0: 6e73 2061 7265 2062 656c 6f77 3a0a 0a7c  ns are below:..|
+00003ed0: 204e 616d 6520 2020 2020 2020 2020 2020   Name           
+00003ee0: 7c20 5175 6572 7920 4f70 6572 6174 696f  | Query Operatio
+00003ef0: 6e20 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  n |.|-----------
+00003f00: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
+00003f10: 2d2d 2d2d 2d2d 2d7c 0a7c 2045 7175 616c  -------|.| Equal
+00003f20: 7320 2020 2020 2020 2020 7c20 2465 7120  s         | $eq 
+00003f30: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00003f40: 436f 6e74 6169 6e73 2020 2020 2020 207c  Contains       |
+00003f50: 2024 636f 6e74 6169 6e73 2020 2020 2020   $contains      
+00003f60: 207c 0a7c 2047 7265 6174 6572 2020 2020   |.| Greater    
+00003f70: 2020 2020 7c20 2467 7420 2020 2020 2020      | $gt       
+00003f80: 2020 2020 2020 7c0a 7c20 4772 6561 7465        |.| Greate
+00003f90: 724f 7245 7175 616c 207c 2024 6774 6520  rOrEqual | $gte 
+00003fa0: 2020 2020 2020 2020 2020 207c 0a7c 204c             |.| L
+00003fb0: 6573 7320 2020 2020 2020 2020 2020 7c20  ess           | 
+00003fc0: 246c 7420 2020 2020 2020 2020 2020 2020  $lt             
+00003fd0: 7c0a 7c20 4c65 7373 4f72 4571 7561 6c73  |.| LessOrEquals
+00003fe0: 2020 207c 2024 6c74 6520 2020 2020 2020     | $lte       
+00003ff0: 2020 2020 207c 0a7c 2053 7461 7274 7357       |.| StartsW
+00004000: 6974 6820 2020 2020 7c20 2473 7461 7274  ith     | $start
+00004010: 7377 6974 6820 2020 2020 7c0a 7c20 496e  swith     |.| In
+00004020: 2020 2020 2020 2020 2020 2020 207c 2024               | $
+00004030: 696e 2020 2020 2020 2020 2020 2020 207c  in             |
+00004040: 0a7c 2042 6574 7765 656e 2020 2020 2020  .| Between      
+00004050: 2020 7c20 2462 6574 7765 656e 2020 2020    | $between    
+00004060: 2020 2020 7c0a 7c20 4e6f 7449 6e20 2020      |.| NotIn   
+00004070: 2020 2020 2020 207c 2024 6e69 6e20 2020         | $nin   
+00004080: 2020 2020 2020 2020 207c 0a7c 204e 6f74           |.| Not
+00004090: 4571 7561 6c54 6f20 2020 2020 7c20 246e  EqualTo     | $n
+000040a0: 6f74 2020 2020 2020 2020 2020 2020 7c0a  ot            |.
+000040b0: 7c20 456e 6473 5769 7468 2020 2020 2020  | EndsWith      
+000040c0: 207c 2024 656e 6473 7769 7468 2020 2020   | $endswith    
+000040d0: 2020 207c 0a7c 204f 7220 2020 2020 2020     |.| Or       
+000040e0: 2020 2020 2020 7c20 246f 7220 2020 2020        | $or     
+000040f0: 2020 2020 2020 2020 7c0a 7c20 416e 6420          |.| And 
+00004100: 2020 2020 2020 2020 2020 207c 2024 616e             | $an
+00004110: 6420 2020 2020 2020 2020 2020 207c 0a0a  d            |..
+00004120: 6060 6070 7974 686f 6e0a 6672 6f6d 2064  ```python.from d
+00004130: 6561 6c63 6c6f 7564 5f73 646b 2069 6d70  ealcloud_sdk imp
+00004140: 6f72 7420 4465 616c 436c 6f75 640a 0a64  ort DealCloud..d
+00004150: 6320 3d20 4465 616c 436c 6f75 642e 6672  c = DealCloud.fr
+00004160: 6f6d 5f79 616d 6c28 2270 6174 682f 746f  om_yaml("path/to
+00004170: 2f79 616d 6c5f 636f 6e66 6967 5f66 696c  /yaml_config_fil
+00004180: 652e 6a73 6f6e 2229 0a0a 6463 2e72 6561  e.json")..dc.rea
+00004190: 645f 6461 7461 2822 436f 6d70 616e 7922  d_data("Company"
+000041a0: 2c20 7175 6572 793d 227b 436f 6d70 616e  , query="{Compan
+000041b0: 794e 616d 653a 207b 2463 6f6e 7461 696e  yName: {$contain
+000041c0: 733a 205c 2231 5c22 7d7d 2229 0a60 6060  s: \"1\"}}").```
+000041d0: 0a60 6461 7461 6020 7769 6c6c 2062 6520  .`data` will be 
+000041e0: 6120 6070 616e 6461 732e 4461 7461 4672  a `pandas.DataFr
+000041f0: 616d 6560 2061 7320 6265 6c6f 773a 0a0a  ame` as below:..
+00004200: 7c20 456e 7472 7949 6420 7c20 436f 6d70  | EntryId | Comp
+00004210: 616e 794e 616d 6520 7c20 436f 6d70 616e  anyName | Compan
+00004220: 7954 7970 6520 7c0a 7c2d 2d2d 2d2d 2d2d  yType |.|-------
+00004230: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|-------------
+00004240: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  |-------------|.
+00004250: 7c20 3132 3334 3520 2020 7c20 436f 6d70  | 12345   | Comp
+00004260: 616e 7931 2020 2020 7c20 3331 3937 3738  any1    | 319778
+00004270: 3020 2020 2020 7c0a 0a53 6f6d 6520 6f74  0     |..Some ot
+00004280: 6865 7220 6578 616d 706c 6520 7175 6572  her example quer
+00004290: 7920 7374 7269 6e67 7320 6172 6520 6265  y strings are be
+000042a0: 6c6f 773a 0a46 696c 7465 7220 6f6e 2065  low:.Filter on e
+000042b0: 7863 6c75 6469 6e67 2072 6563 6f72 6473  xcluding records
+000042c0: 2077 6974 6820 6120 7370 6563 6966 6963   with a specific
+000042d0: 2072 6566 6572 656e 6365 2076 616c 7565   reference value
+000042e0: 3a0a 0a60 6060 7079 7468 6f6e 0a66 726f  :..```python.fro
+000042f0: 6d20 6465 616c 636c 6f75 645f 7364 6b20  m dealcloud_sdk 
+00004300: 696d 706f 7274 2044 6561 6c43 6c6f 7564  import DealCloud
+00004310: 0a0a 6463 203d 2044 6561 6c43 6c6f 7564  ..dc = DealCloud
+00004320: 2e66 726f 6d5f 7961 6d6c 2822 7061 7468  .from_yaml("path
+00004330: 2f74 6f2f 7961 6d6c 5f63 6f6e 6669 675f  /to/yaml_config_
+00004340: 6669 6c65 2e6a 736f 6e22 290a 0a64 632e  file.json")..dc.
+00004350: 7265 6164 5f64 6174 6128 2243 6f6d 7061  read_data("Compa
+00004360: 6e79 222c 2071 7565 7279 3d22 7b43 6f76  ny", query="{Cov
+00004370: 6572 6167 6550 6572 736f 6e3a 207b 246e  eragePerson: {$n
+00004380: 696e 3a20 5b35 3738 355d 7d22 290a 6060  in: [5785]}").``
+00004390: 600a 4669 6c74 6572 2075 7369 6e67 204f  `.Filter using O
+000043a0: 723a 0a0a 6060 6070 7974 686f 6e0a 6672  r:..```python.fr
+000043b0: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
+000043c0: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
+000043d0: 640a 0a64 6320 3d20 4465 616c 436c 6f75  d..dc = DealClou
+000043e0: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
+000043f0: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
+00004400: 5f66 696c 652e 6a73 6f6e 2229 0a0a 6463  _file.json")..dc
+00004410: 2e72 6561 645f 6461 7461 2822 436f 6d70  .read_data("Comp
+00004420: 616e 7922 2c20 7175 6572 793d 227b 246f  any", query="{$o
+00004430: 723a 205b 7b43 6f6d 7061 6e79 4e61 6d65  r: [{CompanyName
+00004440: 3a20 5c22 4465 616c 436c 6f75 645c 227d  : \"DealCloud\"}
+00004450: 2c7b 436f 6d70 616e 794e 616d 653a 205c  ,{CompanyName: \
+00004460: 2241 5049 2045 6e74 7279 5c22 7d5d 7d22  "API Entry\"}]}"
+00004470: 290a 6060 600a 0a23 2323 2320 5265 6164  ).```..#### Read
+00004480: 696e 6720 4461 7461 2066 726f 6d20 6120  ing Data from a 
+00004490: 5669 6577 0a54 6f20 7265 6164 2064 6174  View.To read dat
+000044a0: 6120 6672 6f6d 2061 2076 6965 7720 7769  a from a view wi
+000044b0: 7468 2049 443a 2060 3132 3334 3560 0a0a  th ID: `12345`..
+000044c0: 4578 616d 706c 653a 0a0a 6060 6070 7974  Example:..```pyt
+000044d0: 686f 6e0a 6672 6f6d 2064 6561 6c63 6c6f  hon.from dealclo
+000044e0: 7564 5f73 646b 2069 6d70 6f72 7420 4465  ud_sdk import De
+000044f0: 616c 436c 6f75 640a 0a64 6320 3d20 4465  alCloud..dc = De
+00004500: 616c 436c 6f75 642e 6672 6f6d 5f79 616d  alCloud.from_yam
+00004510: 6c28 2270 6174 682f 746f 2f79 616d 6c5f  l("path/to/yaml_
+00004520: 636f 6e66 6967 5f66 696c 652e 6a73 6f6e  config_file.json
+00004530: 2229 0a0a 6461 7461 203d 2064 632e 7265  ")..data = dc.re
+00004540: 6164 5f64 6174 6128 7669 6577 5f69 643d  ad_data(view_id=
+00004550: 3132 3334 3529 0a60 6060 0a41 6c74 6572  12345).```.Alter
+00004560: 6e61 7469 7665 6c79 2c20 6966 2074 6865  natively, if the
+00004570: 2076 6965 7720 6973 206e 616d 6564 3a20   view is named: 
+00004580: 224d 7920 436f 6d70 616e 7920 5669 6577  "My Company View
+00004590: 223a 0a0a 6060 6070 7974 686f 6e0a 6672  ":..```python.fr
+000045a0: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
+000045b0: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
+000045c0: 640a 0a64 6320 3d20 4465 616c 436c 6f75  d..dc = DealClou
+000045d0: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
+000045e0: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
+000045f0: 5f66 696c 652e 6a73 6f6e 2229 0a0a 6461  _file.json")..da
+00004600: 7461 203d 2064 632e 7265 6164 5f64 6174  ta = dc.read_dat
+00004610: 6128 7669 6577 5f69 643d 224d 7920 436f  a(view_id="My Co
+00004620: 6d70 616e 7920 5669 6577 2229 0a60 6060  mpany View").```
+00004630: 0a0a 6064 6174 6160 2077 696c 6c20 6265  ..`data` will be
+00004640: 2061 2060 7061 6e64 6173 2e44 6174 6146   a `pandas.DataF
+00004650: 7261 6d65 6020 6173 2062 656c 6f77 3a0a  rame` as below:.
+00004660: 0a7c 2045 6e74 7279 4964 207c 2043 6f6d  .| EntryId | Com
+00004670: 7061 6e79 4e61 6d65 207c 2043 6f6d 7061  panyName | Compa
+00004680: 6e79 5479 7065 2020 2020 2020 2020 2020  nyType          
+00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046e0: 2020 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d 7c2d    |.|---------|-
+000046f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ------------|---
+00004700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004760: 2d2d 2d2d 2d7c 0a7c 2031 3233 3435 2020  -----|.| 12345  
+00004770: 207c 2043 6f6d 7061 6e79 3120 2020 207c   | Company1    |
+00004780: 205b 7b27 7365 714e 756d 6265 7227 3a20   [{'seqNumber': 
+00004790: 332c 2027 6973 4175 746f 5064 6627 3a20  3, 'isAutoPdf': 
+000047a0: 4661 6c73 652c 2027 6964 273a 2033 3139  False, 'id': 319
+000047b0: 3737 3830 2c20 276e 616d 6527 3a20 274c  7780, 'name': 'L
+000047c0: 696d 6974 6564 2050 6172 746e 6572 272c  imited Partner',
+000047d0: 2027 656e 7472 794c 6973 7449 6427 3a20   'entryListId': 
+000047e0: 2d36 7d5d 2020 2020 7c0a 7c20 3132 3334  -6}]    |.| 1234
+000047f0: 3620 2020 7c20 436f 6d70 616e 7932 2020  6   | Company2  
+00004800: 2020 7c20 5b7b 2773 6571 4e75 6d62 6572    | [{'seqNumber
+00004810: 273a 2031 2c20 2769 7341 7574 6f50 6466  ': 1, 'isAutoPdf
+00004820: 273a 2046 616c 7365 2c20 2769 6427 3a20  ': False, 'id': 
+00004830: 3331 3937 3738 322c 2027 6e61 6d65 273a  3197782, 'name':
+00004840: 2027 4f70 6572 6174 696e 6720 436f 6d70   'Operating Comp
+00004850: 616e 7927 2c20 2765 6e74 7279 4c69 7374  any', 'entryList
+00004860: 4964 273a 202d 367d 5d20 207c 0a7c 2031  Id': -6}]  |.| 1
+00004870: 3233 3437 2020 207c 2043 6f6d 7061 6e79  2347   | Company
+00004880: 3320 2020 207c 205b 7b27 7365 714e 756d  3    | [{'seqNum
+00004890: 6265 7227 3a20 332c 2027 6973 4175 746f  ber': 3, 'isAuto
+000048a0: 5064 6627 3a20 4661 6c73 652c 2027 6964  Pdf': False, 'id
+000048b0: 273a 2033 3139 3737 3830 2c20 276e 616d  ': 3197780, 'nam
+000048c0: 6527 3a20 274c 696d 6974 6564 2050 6172  e': 'Limited Par
+000048d0: 746e 6572 272c 2027 656e 7472 794c 6973  tner', 'entryLis
+000048e0: 7449 6427 3a20 2d36 7d5d 2020 2020 7c0a  tId': -6}]    |.
+000048f0: 0a23 2323 2323 2055 7369 6e67 2061 2046  .##### Using a F
+00004900: 696c 7465 7220 5768 656e 2052 6561 6469  ilter When Readi
+00004910: 6e67 2056 6965 7720 4461 7461 0a57 6865  ng View Data.Whe
+00004920: 6e20 7265 6164 696e 6720 6461 7461 2066  n reading data f
+00004930: 726f 6d20 6120 7669 6577 2c20 7768 6963  rom a view, whic
+00004940: 6820 6861 7320 2253 7570 706c 7920 5661  h has "Supply Va
+00004950: 6c75 6520 4c61 7465 7222 2066 696c 7465  lue Later" filte
+00004960: 7273 2063 6f6e 6669 6775 7265 642c 2074  rs configured, t
+00004970: 6865 2066 696c 7465 7220 7661 6c75 6573  he filter values
+00004980: 2063 616e 2062 6520 7072 6f76 6964 6564   can be provided
+00004990: 2062 7920 7061 7373 696e 6720 7468 656d   by passing them
+000049a0: 2074 6f20 7468 6520 6076 6965 775f 6669   to the `view_fi
+000049b0: 6c74 6572 6020 6172 6775 6d65 6e74 2069  lter` argument i
+000049c0: 6e20 6120 606c 6973 7460 206f 6620 6064  n a `list` of `d
+000049d0: 6963 7460 732e 2046 6f72 206d 6f72 6520  ict`s. For more 
+000049e0: 696e 666f 726d 6174 696f 6e20 6f6e 2074  information on t
+000049f0: 6865 6972 2066 6f72 6d61 742c 2070 6c65  heir format, ple
+00004a00: 6173 6520 7365 6520 7468 6520 5b41 5049  ase see the [API
+00004a10: 2044 6f63 756d 656e 7461 7469 6f6e 5d28   Documentation](
+00004a20: 6874 7470 733a 2f2f 6170 692e 646f 6373  https://api.docs
+00004a30: 2e64 6561 6c63 6c6f 7564 2e63 6f6d 2f64  .dealcloud.com/d
+00004a40: 6f63 732f 6461 7461 2f72 6f77 732f 7669  ocs/data/rows/vi
+00004a50: 6577 5f64 6574 6169 6c73 292e 0a0a 466f  ew_details)...Fo
+00004a60: 7220 4578 616d 706c 652c 2073 7570 706c  r Example, suppl
+00004a70: 7969 6e67 2061 2022 436f 6d70 616e 7954  ying a "CompanyT
+00004a80: 7970 6522 2066 696c 7465 7220 7661 6c75  ype" filter valu
+00004a90: 6520 746f 2066 696c 7465 7220 666f 7220  e to filter for 
+00004aa0: 6f6e 6c79 2022 4c69 6d69 7465 6420 5061  only "Limited Pa
+00004ab0: 7274 6e65 7222 2063 6f6d 7061 6e69 6573  rtner" companies
+00004ac0: 3a0a 0a60 6060 7079 7468 6f6e 0a66 726f  :..```python.fro
+00004ad0: 6d20 6465 616c 636c 6f75 645f 7364 6b20  m dealcloud_sdk 
+00004ae0: 696d 706f 7274 2044 6561 6c43 6c6f 7564  import DealCloud
+00004af0: 0a0a 6463 203d 2044 6561 6c43 6c6f 7564  ..dc = DealCloud
+00004b00: 2e66 726f 6d5f 7961 6d6c 2822 7061 7468  .from_yaml("path
+00004b10: 2f74 6f2f 7961 6d6c 5f63 6f6e 6669 675f  /to/yaml_config_
+00004b20: 6669 6c65 2e6a 736f 6e22 290a 0a64 6174  file.json")..dat
+00004b30: 6120 3d20 6463 2e72 6561 645f 6461 7461  a = dc.read_data
+00004b40: 280a 2020 2076 6965 775f 6964 203d 2022  (.   view_id = "
+00004b50: 4d79 2043 6f6d 7061 6e79 2056 6965 7722  My Company View"
+00004b60: 2c0a 2020 2076 6965 775f 6669 6c74 6572  ,.   view_filter
+00004b70: 203d 205b 0a20 2020 2020 207b 0a20 2020   = [.      {.   
+00004b80: 2020 2020 2020 2263 6f6c 756d 6e22 3a22        "column":"
+00004b90: 436f 6d70 616e 7954 7970 6522 2c0a 2020  CompanyType",.  
+00004ba0: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+00004bb0: 5b33 3139 3737 3830 5d0a 2020 2020 2020  [3197780].      
+00004bc0: 7d0a 2020 205d 0a29 0a60 6060 0a60 6461  }.   ].).```.`da
+00004bd0: 7461 6020 7769 6c6c 2062 6520 6120 6070  ta` will be a `p
+00004be0: 616e 6461 732e 4461 7461 4672 616d 6560  andas.DataFrame`
+00004bf0: 2061 7320 6265 6c6f 773a 0a0a 7c20 456e   as below:..| En
+00004c00: 7472 7949 6420 7c20 436f 6d70 616e 794e  tryId | CompanyN
+00004c10: 616d 6520 7c20 436f 6d70 616e 7954 7970  ame | CompanyTyp
+00004c20: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+00004c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c70: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00004c80: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
+00004c90: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
+00004ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004d00: 7c0a 7c20 3132 3334 3520 2020 7c20 436f  |.| 12345   | Co
+00004d10: 6d70 616e 7931 2020 2020 7c20 5b7b 2773  mpany1    | [{'s
+00004d20: 6571 4e75 6d62 6572 273a 2033 2c20 2769  eqNumber': 3, 'i
+00004d30: 7341 7574 6f50 6466 273a 2046 616c 7365  sAutoPdf': False
+00004d40: 2c20 2769 6427 3a20 3331 3937 3738 302c  , 'id': 3197780,
+00004d50: 2027 6e61 6d65 273a 2027 4c69 6d69 7465   'name': 'Limite
+00004d60: 6420 5061 7274 6e65 7227 2c20 2765 6e74  d Partner', 'ent
+00004d70: 7279 4c69 7374 4964 273a 202d 367d 5d20  ryListId': -6}] 
+00004d80: 2020 207c 0a7c 2031 3233 3437 2020 207c     |.| 12347   |
+00004d90: 2043 6f6d 7061 6e79 3320 2020 207c 205b   Company3    | [
+00004da0: 7b27 7365 714e 756d 6265 7227 3a20 332c  {'seqNumber': 3,
+00004db0: 2027 6973 4175 746f 5064 6627 3a20 4661   'isAutoPdf': Fa
+00004dc0: 6c73 652c 2027 6964 273a 2033 3139 3737  lse, 'id': 31977
+00004dd0: 3830 2c20 276e 616d 6527 3a20 274c 696d  80, 'name': 'Lim
+00004de0: 6974 6564 2050 6172 746e 6572 272c 2027  ited Partner', '
+00004df0: 656e 7472 794c 6973 7449 6427 3a20 2d36  entryListId': -6
+00004e00: 7d5d 2020 2020 7c0a 0a0a 2323 2320 4372  }]    |...### Cr
+00004e10: 6561 7465 2c20 5570 6461 7465 2061 6e64  eate, Update and
+00004e20: 2055 7073 6572 7420 4461 7461 0a60 4465   Upsert Data.`De
+00004e30: 616c 436c 6f75 642e 696e 7365 7274 5f64  alCloud.insert_d
+00004e40: 6174 6128 2960 2c20 6044 6561 6c43 6c6f  ata()`, `DealClo
+00004e50: 7564 2e75 7064 6174 655f 6461 7461 2829  ud.update_data()
+00004e60: 602c 2060 4465 616c 436c 6f75 642e 7570  `, `DealCloud.up
+00004e70: 7365 7274 5f64 6174 6128 2960 2061 7265  sert_data()` are
+00004e80: 206d 6574 686f 6473 2077 6869 6368 2070   methods which p
+00004e90: 726f 7669 6465 2074 6865 2061 6269 6c69  rovide the abili
+00004ea0: 7479 2074 6f20 6372 6561 7465 2c20 7570  ty to create, up
+00004eb0: 6461 7465 2061 6e64 2075 7073 6572 7420  date and upsert 
+00004ec0: 6461 7461 2072 6573 7065 6374 6976 656c  data respectivel
+00004ed0: 792e 0a54 6865 7365 206d 6574 686f 6473  y..These methods
+00004ee0: 2068 6176 6520 7468 6520 7361 6d65 2061   have the same a
+00004ef0: 7267 756d 656e 7420 7061 7474 6572 6e3a  rgument pattern:
+00004f00: 0a0a 4172 6775 6d65 6e74 733a 0a2d 206f  ..Arguments:.- o
+00004f10: 626a 6563 745f 6170 695f 6e61 6d65 2060  bject_api_name `
+00004f20: 7374 7260 3a20 7468 6520 6f62 6a65 6374  str`: the object
+00004f30: 2041 5049 206e 616d 6520 746f 2077 7269   API name to wri
+00004f40: 7465 2064 6174 6120 746f 0a2d 2064 6174  te data to.- dat
+00004f50: 6120 6055 6e69 6f6e 5b6c 6973 745b 6469  a `Union[list[di
+00004f60: 6374 5d2c 2070 642e 4461 7461 4672 616d  ct], pd.DataFram
+00004f70: 655d 603a 2074 6865 2064 6174 6120 746f  e]`: the data to
+00004f80: 2062 6520 7365 6e74 2074 6f20 4465 616c   be sent to Deal
+00004f90: 436c 6f75 642e 0a2d 2075 7365 5f64 6561  Cloud..- use_dea
+00004fa0: 6c63 6c6f 7564 5f69 6473 2060 626f 6f6c  lcloud_ids `bool
+00004fb0: 603a 2044 6566 6175 6c74 2069 7320 6054  `: Default is `T
+00004fc0: 7275 6560 2049 6620 6054 7275 6560 2c20  rue` If `True`, 
+00004fd0: 4465 616c 436c 6f75 6420 456e 7472 7949  DealCloud EntryI
+00004fe0: 6473 206d 7573 7420 6265 2075 7365 6420  ds must be used 
+00004ff0: 746f 2072 6566 6572 656e 6365 2072 6563  to reference rec
+00005000: 6f72 6473 2061 6e64 2063 686f 6963 6520  ords and choice 
+00005010: 7661 6c75 6573 2e20 4966 2060 4661 6c73  values. If `Fals
+00005020: 6560 2c20 7573 6520 6120 636f 6c75 6d6e  e`, use a column
+00005030: 2061 7320 6120 6c6f 6f6b 7570 2c20 6465   as a lookup, de
+00005040: 6669 6e65 6420 6279 2074 6865 206c 6f6f  fined by the loo
+00005050: 6b75 705f 636f 6c75 6d6e 2061 7267 756d  kup_column argum
+00005060: 656e 742e 0a2d 206c 6f6f 6b75 705f 636f  ent..- lookup_co
+00005070: 6c75 6d6e 2060 7374 7260 3a20 6966 2060  lumn `str`: if `
+00005080: 7573 655f 6465 616c 636c 6f75 645f 6964  use_dealcloud_id
+00005090: 7360 2069 7320 6046 616c 7365 602c 2074  s` is `False`, t
+000050a0: 6869 7320 6465 6669 6e65 7320 7468 6520  his defines the 
+000050b0: 636f 6c75 6d6e 2074 6f20 6265 2075 7365  column to be use
+000050c0: 6420 6173 2061 206c 6f6f 6b75 702e 0a2d  d as a lookup..-
+000050d0: 206f 7574 7075 7460 7374 7260 3a20 606c   output`str`: `l
+000050e0: 6973 7460 206f 7220 6070 616e 6461 7360  ist` or `pandas`
+000050f0: 2c20 6465 6669 6e65 7320 7468 6520 6f75  , defines the ou
+00005100: 7470 7574 2066 6f72 6d61 7420 7265 7475  tput format retu
+00005110: 726e 6564 2066 726f 6d20 7468 6520 6675  rned from the fu
+00005120: 6e63 7469 6f6e 0a0a 5265 7475 726e 733a  nction..Returns:
+00005130: 0a20 2020 6055 6e69 6f6e 5b6c 6973 745b  .   `Union[list[
+00005140: 6469 6374 5d2c 2070 642e 4461 7461 4672  dict], pd.DataFr
+00005150: 616d 655d 603a 2074 6865 2064 6174 6120  ame]`: the data 
+00005160: 7265 7475 726e 6564 2066 726f 6d20 7468  returned from th
+00005170: 6520 6461 7461 206f 7065 7261 7469 6f6e  e data operation
+00005180: 2e0a 0a3e 205b 2149 4d50 4f52 5441 4e54  ...> [!IMPORTANT
+00005190: 5d0a 3e20 5768 656e 206e 6f74 2075 7369  ].> When not usi
+000051a0: 6e67 2060 7573 655f 6465 616c 636c 6f75  ng `use_dealclou
+000051b0: 645f 6964 7360 2c20 666f 7220 5265 6665  d_ids`, for Refe
+000051c0: 7265 6e63 6520 6669 656c 6473 2c20 7265  rence fields, re
+000051d0: 6665 7265 6e63 6520 6279 2072 6563 6f72  ference by recor
+000051e0: 6420 456e 7472 7949 642e 2046 6f72 2063  d EntryId. For c
+000051f0: 686f 6963 6520 6669 656c 6473 2c20 7573  hoice fields, us
+00005200: 6520 7468 6520 6368 6f69 6365 2076 616c  e the choice val
+00005210: 7565 2049 442e 2046 6f72 2075 7365 7220  ue ID. For user 
+00005220: 6669 656c 6473 2c20 7573 6520 7468 6520  fields, use the 
+00005230: 7573 6572 2049 4420 2866 726f 6d20 6044  user ID (from `D
+00005240: 6561 6c43 6c6f 7564 2e67 6574 5f75 7365  ealCloud.get_use
+00005250: 7273 2829 6029 2e20 0a3e 2057 6865 6e20  rs()`). .> When 
+00005260: 7573 696e 6720 6075 7365 5f64 6561 6c63  using `use_dealc
+00005270: 6c6f 7564 5f69 6473 602c 2066 6f72 2052  loud_ids`, for R
+00005280: 6566 6572 656e 6365 2066 6965 6c64 732c  eference fields,
+00005290: 2072 6566 6572 656e 6365 2062 7920 7468   reference by th
+000052a0: 6520 6c6f 6f6b 7570 2063 6f6c 756d 6e20  e lookup column 
+000052b0: 6f6e 2074 6865 2072 6566 6572 656e 6365  on the reference
+000052c0: 6420 6f62 6a65 6374 2e20 466f 7220 6368  d object. For ch
+000052d0: 6f69 6365 2066 6965 6c64 732c 2075 7365  oice fields, use
+000052e0: 2074 6865 2063 686f 6963 6520 6669 656c   the choice fiel
+000052f0: 6420 6469 7370 6c61 7920 6e61 6d65 2e20  d display name. 
+00005300: 466f 7220 7573 6572 2066 6965 6c64 732c  For user fields,
+00005310: 2075 7365 2074 6865 2075 7365 7220 656d   use the user em
+00005320: 6169 6c20 6164 6472 6573 732e 0a0a 2323  ail address...##
+00005330: 2323 2320 4669 656c 6420 4d61 7070 696e  ### Field Mappin
+00005340: 670a 416c 6c20 636f 6c75 6d6e 7320 7061  g.All columns pa
+00005350: 7373 6564 2074 6f20 7468 6520 6372 6561  ssed to the crea
+00005360: 7465 2c20 7570 6461 7465 2061 6e64 2075  te, update and u
+00005370: 7073 6572 7420 6d65 7468 6f64 7320 6d75  psert methods mu
+00005380: 7374 206d 6174 6368 2062 7920 5f41 5049  st match by _API
+00005390: 204e 616d 655f 2e20 4966 2061 2063 6f6c   Name_. If a col
+000053a0: 756d 6e20 7061 7373 6564 2074 6f20 7468  umn passed to th
+000053b0: 6520 6d65 7468 6f64 2064 6f65 7320 6e6f  e method does no
+000053c0: 7420 6578 6973 7420 696e 2074 6865 2073  t exist in the s
+000053d0: 6974 6520 6279 2041 5049 206e 616d 652c  ite by API name,
+000053e0: 2074 6865 6e20 6120 604b 6579 4572 726f   then a `KeyErro
+000053f0: 7260 2077 696c 6c20 6265 2072 6169 7365  r` will be raise
+00005400: 643a 0a0a 6060 6070 7974 686f 6e0a 6672  d:..```python.fr
+00005410: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
+00005420: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
+00005430: 640a 0a64 6320 3d20 4465 616c 436c 6f75  d..dc = DealClou
+00005440: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
+00005450: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
+00005460: 5f66 696c 652e 6a73 6f6e 2229 0a0a 746f  _file.json")..to
+00005470: 5f73 656e 6420 3d20 5b0a 2020 7b0a 2020  _send = [.  {.  
+00005480: 2020 2020 2243 6f6d 7061 6e79 4e61 6d65      "CompanyName
+00005490: 223a 2022 5465 7374 2043 6f6d 7061 6e79  ": "Test Company
+000054a0: 2031 222c 0a20 2020 2020 2022 556e 6d61   1",.      "Unma
+000054b0: 7070 6162 6c65 436f 6c75 6d6e 223a 2022  ppableColumn": "
+000054c0: 466f 6f22 2c0a 2020 7d0a 5d0a 7265 7370  Foo",.  }.].resp
+000054d0: 6f6e 7365 7320 3d20 6463 2e69 6e73 6572  onses = dc.inser
+000054e0: 745f 6461 7461 2822 436f 6d70 616e 7922  t_data("Company"
+000054f0: 2c20 746f 5f73 656e 6429 0a60 6060 0a57  , to_send).```.W
+00005500: 696c 6c20 5265 7475 726e 0a60 6060 6261  ill Return.```ba
+00005510: 7368 0a54 7261 6365 6261 636b 2e2e 2e0a  sh.Traceback....
+00005520: 4b65 7945 7272 6f72 3a20 226d 6170 7069  KeyError: "mappi
+00005530: 6e67 2065 7272 6f72 2c20 636f 756c 6420  ng error, could 
+00005540: 6e6f 7420 6d61 703a 205b 2755 6e6d 6170  not map: ['Unmap
+00005550: 7061 626c 6543 6f6c 756d 6e27 5d22 0a60  pableColumn']".`
+00005560: 6060 0a0a 2323 2323 2043 7265 6174 6520  ``..#### Create 
+00005570: 4461 7461 0a45 7861 6d70 6c65 2c20 746f  Data.Example, to
+00005580: 2069 6e73 6572 7420 6461 7461 2069 6e74   insert data int
+00005590: 6f20 7468 6520 2243 6f6d 7061 6e79 2220  o the "Company" 
+000055a0: 6f62 6a65 6374 2066 726f 6d20 6120 6c69  object from a li
+000055b0: 7374 3a0a 0a60 6060 7079 7468 6f6e 0a66  st:..```python.f
+000055c0: 726f 6d20 6465 616c 636c 6f75 645f 7364  rom dealcloud_sd
+000055d0: 6b20 696d 706f 7274 2044 6561 6c43 6c6f  k import DealClo
+000055e0: 7564 0a0a 6463 203d 2044 6561 6c43 6c6f  ud..dc = DealClo
+000055f0: 7564 2e66 726f 6d5f 7961 6d6c 2822 7061  ud.from_yaml("pa
+00005600: 7468 2f74 6f2f 7961 6d6c 5f63 6f6e 6669  th/to/yaml_confi
+00005610: 675f 6669 6c65 2e6a 736f 6e22 290a 0a74  g_file.json")..t
+00005620: 6f5f 7365 6e64 203d 205b 0a20 207b 0a20  o_send = [.  {. 
+00005630: 2020 2020 2022 436f 6d70 616e 794e 616d       "CompanyNam
+00005640: 6522 3a20 2254 6573 7420 436f 6d70 616e  e": "Test Compan
+00005650: 7920 3122 2c0a 2020 2020 2020 2243 6f6d  y 1",.      "Com
+00005660: 7061 6e79 5479 7065 223a 2031 3233 3435  panyType": 12345
+00005670: 2c0a 2020 2020 2020 2242 7573 696e 6573  ,.      "Busines
+00005680: 7344 6573 6372 6970 7469 6f6e 223a 2022  sDescription": "
+00005690: 4865 7265 2069 7320 6120 6275 7369 6e65  Here is a busine
+000056a0: 7373 2064 6573 6372 6970 7469 6f6e 222c  ss description",
+000056b0: 0a20 2020 2020 2022 5365 6374 6f72 223a  .      "Sector":
+000056c0: 2031 3433 3231 2c0a 2020 7d0a 5d0a 7265   14321,.  }.].re
+000056d0: 7370 6f6e 7365 7320 3d20 6463 2e69 6e73  sponses = dc.ins
+000056e0: 6572 745f 6461 7461 2822 436f 6d70 616e  ert_data("Compan
+000056f0: 7922 2c20 746f 5f73 656e 6429 0a60 6060  y", to_send).```
+00005700: 0a49 6620 7375 6363 6573 7366 756c 2c20  .If successful, 
+00005710: 6072 6573 706f 6e73 6573 6020 7769 6c6c  `responses` will
+00005720: 2063 6f6e 7461 696e 2074 6865 2062 656c   contain the bel
+00005730: 6f77 202d 206e 6f74 6520 7468 6174 2060  ow - note that `
+00005740: 456e 7472 7949 6460 2069 7320 6e6f 7720  EntryId` is now 
+00005750: 696e 636c 7564 6564 3a0a 6060 6070 7974  included:.```pyt
+00005760: 686f 6e0a 5b0a 2020 2020 7b0a 2020 2020  hon.[.    {.    
+00005770: 2020 2020 2245 6e74 7279 4964 223a 2032      "EntryId": 2
+00005780: 3334 3536 372c 0a20 2020 2020 2020 2022  34567,.        "
+00005790: 436f 6d70 616e 794e 616d 6522 3a20 2254  CompanyName": "T
+000057a0: 6573 7420 436f 6d70 616e 7920 3122 2c0a  est Company 1",.
+000057b0: 2020 2020 2020 2020 2243 6f6d 7061 6e79          "Company
+000057c0: 5479 7065 223a 2031 3233 3435 2c0a 2020  Type": 12345,.  
+000057d0: 2020 2020 2020 2242 7573 696e 6573 7344        "BusinessD
+000057e0: 6573 6372 6970 7469 6f6e 223a 2022 4865  escription": "He
+000057f0: 7265 2069 7320 6120 6275 7369 6e65 7373  re is a business
+00005800: 2064 6573 6372 6970 7469 6f6e 222c 0a20   description",. 
+00005810: 2020 2020 2020 2022 5365 6374 6f72 223a         "Sector":
+00005820: 2031 3433 3231 2c0a 2020 2020 7d0a 5d0a   14321,.    }.].
+00005830: 6060 600a 4578 616d 706c 652c 2074 6f20  ```.Example, to 
+00005840: 696e 7365 7274 2064 6174 6120 696e 746f  insert data into
+00005850: 2074 6865 2022 436f 6d70 616e 7922 206f   the "Company" o
+00005860: 626a 6563 7420 6672 6f6d 2061 2043 5356  bject from a CSV
+00005870: 2c20 7573 696e 6720 6070 616e 6461 7360  , using `pandas`
+00005880: 3a0a 0a43 5356 2046 696c 6520 2860 636f  :..CSV File (`co
+00005890: 6d70 616e 792e 6373 7660 293a 0a0a 7c20  mpany.csv`):..| 
+000058a0: 436f 6d70 616e 794e 616d 6520 7c20 436f  CompanyName | Co
+000058b0: 6d70 616e 7954 7970 6520 7c0a 7c2d 2d2d  mpanyType |.|---
+000058c0: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
+000058d0: 2d2d 2d2d 2d2d 2d2d 7c0a 7c20 436f 6d70  --------|.| Comp
+000058e0: 616e 7931 2020 2020 7c20 3331 3937 3738  any1    | 319778
+000058f0: 3020 2020 2020 7c0a 7c20 436f 6d70 616e  0     |.| Compan
+00005900: 7932 2020 2020 7c20 3331 3937 3738 3220  y2    | 3197782 
+00005910: 2020 2020 7c0a 7c20 436f 6d70 616e 7933      |.| Company3
+00005920: 2020 2020 7c20 3331 3937 3738 3020 2020      | 3197780   
+00005930: 2020 7c0a 0a60 6060 7079 7468 6f6e 0a69    |..```python.i
+00005940: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
+00005950: 7064 0a66 726f 6d20 6465 616c 636c 6f75  pd.from dealclou
+00005960: 645f 7364 6b20 696d 706f 7274 2044 6561  d_sdk import Dea
+00005970: 6c43 6c6f 7564 0a0a 6463 203d 2044 6561  lCloud..dc = Dea
+00005980: 6c43 6c6f 7564 2e66 726f 6d5f 7961 6d6c  lCloud.from_yaml
+00005990: 2822 7061 7468 2f74 6f2f 7961 6d6c 5f63  ("path/to/yaml_c
+000059a0: 6f6e 6669 675f 6669 6c65 2e6a 736f 6e22  onfig_file.json"
+000059b0: 290a 0a74 6f5f 7365 6e64 203d 2070 642e  )..to_send = pd.
+000059c0: 7265 6164 5f63 7376 2822 636f 6d70 616e  read_csv("compan
+000059d0: 792e 6373 7622 290a 7265 7370 6f6e 7365  y.csv").response
+000059e0: 7320 3d20 6463 2e69 6e73 6572 745f 6461  s = dc.insert_da
+000059f0: 7461 2822 436f 6d70 616e 7922 2c20 746f  ta("Company", to
+00005a00: 5f73 656e 6429 0a60 6060 0a45 7861 6d70  _send).```.Examp
+00005a10: 6c65 2c20 746f 2069 6e73 6572 7420 6461  le, to insert da
+00005a20: 7461 2069 6e74 6f20 7468 6520 2243 6f6d  ta into the "Com
+00005a30: 7061 6e79 2220 6f62 6a65 6374 2075 7369  pany" object usi
+00005a40: 6e67 2022 4578 7465 726e 616c 5379 7374  ng "ExternalSyst
+00005a50: 656d 4944 2220 6173 2061 206c 6f6f 6b75  emID" as a looku
+00005a60: 7020 636f 6c75 6d6e 3a0a 0a60 6060 7079  p column:..```py
+00005a70: 7468 6f6e 0a66 726f 6d20 6465 616c 636c  thon.from dealcl
+00005a80: 6f75 645f 7364 6b20 696d 706f 7274 2044  oud_sdk import D
+00005a90: 6561 6c43 6c6f 7564 0a0a 6463 203d 2044  ealCloud..dc = D
+00005aa0: 6561 6c43 6c6f 7564 2e66 726f 6d5f 7961  ealCloud.from_ya
+00005ab0: 6d6c 2822 7061 7468 2f74 6f2f 7961 6d6c  ml("path/to/yaml
+00005ac0: 5f63 6f6e 6669 675f 6669 6c65 2e6a 736f  _config_file.jso
+00005ad0: 6e22 290a 0a74 6f5f 7365 6e64 203d 205b  n")..to_send = [
+00005ae0: 0a20 207b 0a20 2020 2020 2022 436f 6d70  .  {.      "Comp
+00005af0: 616e 794e 616d 6522 3a20 2254 6573 7420  anyName": "Test 
+00005b00: 436f 6d70 616e 7920 3122 2c0a 2020 2020  Company 1",.    
+00005b10: 2020 2243 6f6d 7061 6e79 5479 7065 223a    "CompanyType":
+00005b20: 2022 4f70 6572 6174 696e 6720 436f 6d70   "Operating Comp
+00005b30: 616e 7922 2c0a 2020 2020 2020 2242 7573  any",.      "Bus
 00005b40: 696e 6573 7344 6573 6372 6970 7469 6f6e  inessDescription
 00005b50: 223a 2022 4865 7265 2069 7320 6120 6275  ": "Here is a bu
 00005b60: 7369 6e65 7373 2064 6573 6372 6970 7469  siness descripti
-00005b70: 6f6e 222c 0a20 2020 2020 2020 2022 5365  on",.        "Se
-00005b80: 6374 6f72 223a 2031 3433 3231 2c0a 2020  ctor": 14321,.  
-00005b90: 2020 7d0a 5d0a 6060 600a 4578 616d 706c    }.].```.Exampl
-00005ba0: 652c 2074 6f20 696e 7365 7274 2064 6174  e, to insert dat
-00005bb0: 6120 696e 746f 2074 6865 2022 436f 6d70  a into the "Comp
-00005bc0: 616e 7922 206f 626a 6563 7420 6672 6f6d  any" object from
-00005bd0: 2061 2043 5356 2c20 7573 696e 6720 6070   a CSV, using `p
-00005be0: 616e 6461 7360 3a0a 0a43 5356 2046 696c  andas`:..CSV Fil
-00005bf0: 6520 2860 636f 6d70 616e 792e 6373 7660  e (`company.csv`
-00005c00: 293a 0a0a 7c20 436f 6d70 616e 794e 616d  ):..| CompanyNam
-00005c10: 6520 7c20 436f 6d70 616e 7954 7970 6520  e | CompanyType 
-00005c20: 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.|-------------
-00005c30: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  |-------------|.
-00005c40: 7c20 436f 6d70 616e 7931 2020 2020 7c20  | Company1    | 
-00005c50: 3331 3937 3738 3020 2020 2020 7c0a 7c20  3197780     |.| 
-00005c60: 436f 6d70 616e 7932 2020 2020 7c20 3331  Company2    | 31
-00005c70: 3937 3738 3220 2020 2020 7c0a 7c20 436f  97782     |.| Co
-00005c80: 6d70 616e 7933 2020 2020 7c20 3331 3937  mpany3    | 3197
-00005c90: 3738 3020 2020 2020 7c0a 0a60 6060 7079  780     |..```py
-00005ca0: 7468 6f6e 0a69 6d70 6f72 7420 7061 6e64  thon.import pand
-00005cb0: 6173 2061 7320 7064 0a66 726f 6d20 6465  as as pd.from de
-00005cc0: 616c 636c 6f75 645f 7364 6b20 696d 706f  alcloud_sdk impo
-00005cd0: 7274 2044 6561 6c43 6c6f 7564 0a0a 6463  rt DealCloud..dc
-00005ce0: 203d 2044 6561 6c43 6c6f 7564 2e66 726f   = DealCloud.fro
-00005cf0: 6d5f 7961 6d6c 2822 7061 7468 2f74 6f2f  m_yaml("path/to/
-00005d00: 7961 6d6c 5f63 6f6e 6669 675f 6669 6c65  yaml_config_file
-00005d10: 2e6a 736f 6e22 290a 0a74 6f5f 7365 6e64  .json")..to_send
-00005d20: 203d 2070 642e 7265 6164 5f63 7376 2822   = pd.read_csv("
-00005d30: 636f 6d70 616e 792e 6373 7622 290a 7265  company.csv").re
-00005d40: 7370 6f6e 7365 7320 3d20 6463 2e69 6e73  sponses = dc.ins
-00005d50: 6572 745f 6461 7461 2822 436f 6d70 616e  ert_data("Compan
-00005d60: 7922 2c20 746f 5f73 656e 6429 0a60 6060  y", to_send).```
-00005d70: 0a45 7861 6d70 6c65 2c20 746f 2069 6e73  .Example, to ins
-00005d80: 6572 7420 6461 7461 2069 6e74 6f20 7468  ert data into th
-00005d90: 6520 2243 6f6d 7061 6e79 2220 6f62 6a65  e "Company" obje
-00005da0: 6374 2075 7369 6e67 2022 4578 7465 726e  ct using "Extern
-00005db0: 616c 5379 7374 656d 4944 2220 6173 2061  alSystemID" as a
-00005dc0: 206c 6f6f 6b75 7020 636f 6c75 6d6e 3a0a   lookup column:.
-00005dd0: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
-00005de0: 6465 616c 636c 6f75 645f 7364 6b20 696d  dealcloud_sdk im
-00005df0: 706f 7274 2044 6561 6c43 6c6f 7564 0a0a  port DealCloud..
-00005e00: 6463 203d 2044 6561 6c43 6c6f 7564 2e66  dc = DealCloud.f
-00005e10: 726f 6d5f 7961 6d6c 2822 7061 7468 2f74  rom_yaml("path/t
-00005e20: 6f2f 7961 6d6c 5f63 6f6e 6669 675f 6669  o/yaml_config_fi
-00005e30: 6c65 2e6a 736f 6e22 290a 0a74 6f5f 7365  le.json")..to_se
-00005e40: 6e64 203d 205b 0a20 207b 0a20 2020 2020  nd = [.  {.     
-00005e50: 2022 436f 6d70 616e 794e 616d 6522 3a20   "CompanyName": 
-00005e60: 2254 6573 7420 436f 6d70 616e 7920 3122  "Test Company 1"
-00005e70: 2c0a 2020 2020 2020 2243 6f6d 7061 6e79  ,.      "Company
-00005e80: 5479 7065 223a 2022 4f70 6572 6174 696e  Type": "Operatin
-00005e90: 6720 436f 6d70 616e 7922 2c0a 2020 2020  g Company",.    
-00005ea0: 2020 2242 7573 696e 6573 7344 6573 6372    "BusinessDescr
-00005eb0: 6970 7469 6f6e 223a 2022 4865 7265 2069  iption": "Here i
-00005ec0: 7320 6120 6275 7369 6e65 7373 2064 6573  s a business des
-00005ed0: 6372 6970 7469 6f6e 222c 0a20 2020 2020  cription",.     
-00005ee0: 2022 5365 6374 6f72 223a 2022 3631 3245   "Sector": "612E
-00005ef0: 3946 4634 2d31 4438 432d 3431 4237 2d42  9FF4-1D8C-41B7-B
-00005f00: 3845 442d 3244 3143 3135 3234 3034 3334  8ED-2D1C15240434
-00005f10: 222c 0a20 207d 0a5d 0a0a 7265 7370 6f6e  ",.  }.]..respon
-00005f20: 7365 7320 3d20 6463 2e69 6e73 6572 745f  ses = dc.insert_
-00005f30: 6461 7461 280a 2020 206f 626a 6563 745f  data(.   object_
-00005f40: 6170 695f 6e61 6d65 203d 2022 436f 6d70  api_name = "Comp
-00005f50: 616e 7922 2c0a 2020 2064 6174 6120 3d20  any",.   data = 
-00005f60: 746f 5f73 656e 642c 0a20 2020 7573 655f  to_send,.   use_
-00005f70: 6465 616c 636c 6f75 645f 6964 7320 3d20  dealcloud_ids = 
-00005f80: 4661 6c73 652c 0a20 2020 6c6f 6f6b 7570  False,.   lookup
-00005f90: 5f63 6f6c 756d 6e20 3d20 2245 7874 6572  _column = "Exter
-00005fa0: 6e61 6c53 7973 7465 6d49 4422 0a29 0a60  nalSystemID".).`
-00005fb0: 6060 0a23 2323 2320 5570 6461 7465 2044  ``.#### Update D
-00005fc0: 6174 610a 546f 2075 7064 6174 6520 6578  ata.To update ex
-00005fd0: 6973 7469 6e67 2073 6974 6520 6461 7461  isting site data
-00005fe0: 2c20 7468 6520 7072 6f63 6573 7320 6973  , the process is
-00005ff0: 2073 696d 696c 6172 2c20 6578 6365 7074   similar, except
-00006000: 206f 626a 6563 7473 206d 7573 7420 696e   objects must in
-00006010: 636c 7564 6520 6045 6e74 7279 4964 602c  clude `EntryId`,
-00006020: 206f 7220 6120 7661 6c69 6420 7072 696d   or a valid prim
-00006030: 6172 7920 6b65 7920 6279 2060 6c6f 6f6b  ary key by `look
-00006040: 7570 5f63 6f6c 756d 6e60 2e0a 0a45 7861  up_column`...Exa
-00006050: 6d70 6c65 2c20 746f 2075 7064 6174 6520  mple, to update 
-00006060: 6461 7461 2069 6e20 7468 6520 2243 6f6d  data in the "Com
-00006070: 7061 6e79 2220 6f62 6a65 6374 2066 726f  pany" object fro
-00006080: 6d20 6120 6c69 7374 3a0a 0a60 6060 7079  m a list:..```py
-00006090: 7468 6f6e 0a66 726f 6d20 6465 616c 636c  thon.from dealcl
-000060a0: 6f75 645f 7364 6b20 696d 706f 7274 2044  oud_sdk import D
-000060b0: 6561 6c43 6c6f 7564 0a0a 6463 203d 2044  ealCloud..dc = D
-000060c0: 6561 6c43 6c6f 7564 2e66 726f 6d5f 7961  ealCloud.from_ya
-000060d0: 6d6c 2822 7061 7468 2f74 6f2f 7961 6d6c  ml("path/to/yaml
-000060e0: 5f63 6f6e 6669 675f 6669 6c65 2e6a 736f  _config_file.jso
-000060f0: 6e22 290a 0a74 6f5f 7365 6e64 203d 205b  n")..to_send = [
-00006100: 0a20 207b 0a20 2020 2020 2022 456e 7472  .  {.      "Entr
-00006110: 7949 6422 3a20 3233 3435 3637 2c0a 2020  yId": 234567,.  
-00006120: 2020 2020 2242 7573 696e 6573 7344 6573      "BusinessDes
-00006130: 6372 6970 7469 6f6e 223a 2022 4865 7265  cription": "Here
-00006140: 2069 7320 616e 2075 7064 6174 6564 2062   is an updated b
-00006150: 7573 696e 6573 7320 6465 7363 7269 7074  usiness descript
-00006160: 696f 6e21 222c 0a20 207d 0a5d 0a72 6573  ion!",.  }.].res
-00006170: 706f 6e73 6573 203d 2064 632e 696e 7365  ponses = dc.inse
-00006180: 7274 5f64 6174 6128 2243 6f6d 7061 6e79  rt_data("Company
-00006190: 222c 2074 6f5f 7365 6e64 290a 6060 600a  ", to_send).```.
-000061a0: 4966 2073 7563 6365 7373 6675 6c2c 2060  If successful, `
-000061b0: 7265 7370 6f6e 7365 7360 2077 696c 6c20  responses` will 
-000061c0: 636f 6e74 6169 6e20 7468 6520 6265 6c6f  contain the belo
-000061d0: 773a 0a60 6060 7079 7468 6f6e 0a5b 0a20  w:.```python.[. 
-000061e0: 2020 207b 0a20 2020 2020 2020 2022 456e     {.        "En
-000061f0: 7472 7949 6422 3a20 3233 3435 3637 2c0a  tryId": 234567,.
-00006200: 2020 2020 2020 2020 2243 6f6d 7061 6e79          "Company
-00006210: 4e61 6d65 223a 2022 5465 7374 2043 6f6d  Name": "Test Com
-00006220: 7061 6e79 2031 222c 0a20 2020 2020 2020  pany 1",.       
-00006230: 2022 436f 6d70 616e 7954 7970 6522 3a20   "CompanyType": 
-00006240: 3132 3334 352c 0a20 2020 2020 2020 2022  12345,.        "
-00006250: 4275 7369 6e65 7373 4465 7363 7269 7074  BusinessDescript
-00006260: 696f 6e22 3a20 2248 6572 6520 6973 2061  ion": "Here is a
-00006270: 6e20 7570 6461 7465 6420 6275 7369 6e65  n updated busine
-00006280: 7373 2064 6573 6372 6970 7469 6f6e 2122  ss description!"
-00006290: 2c0a 2020 2020 2020 2020 2253 6563 746f  ,.        "Secto
-000062a0: 7222 3a20 3134 3332 312c 0a20 2020 207d  r": 14321,.    }
-000062b0: 0a5d 0a60 6060 0a45 7861 6d70 6c65 2c20  .].```.Example, 
-000062c0: 746f 2075 7064 6174 6520 6461 7461 2069  to update data i
-000062d0: 6e20 7468 6520 2243 6f6d 7061 6e79 2220  n the "Company" 
-000062e0: 6f62 6a65 6374 2066 726f 6d20 6120 6c69  object from a li
-000062f0: 7374 2c20 7573 696e 6720 7468 6520 606c  st, using the `l
-00006300: 6f6f 6b75 705f 636f 6c75 6d6e 602c 2060  ookup_column`, `
-00006310: 4578 7465 726e 616c 5379 7374 656d 4964  ExternalSystemId
-00006320: 603a 0a0a 6060 6070 7974 686f 6e0a 6672  `:..```python.fr
-00006330: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
-00006340: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
-00006350: 640a 0a64 6320 3d20 4465 616c 436c 6f75  d..dc = DealClou
-00006360: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
-00006370: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
-00006380: 5f66 696c 652e 6a73 6f6e 2229 0a0a 746f  _file.json")..to
-00006390: 5f73 656e 6420 3d20 5b0a 2020 7b0a 2020  _send = [.  {.  
-000063a0: 2020 2020 2245 7874 6572 6e61 6c53 7973      "ExternalSys
-000063b0: 7465 6d49 6422 3a20 2246 3632 3841 4643  temId": "F628AFC
-000063c0: 382d 3533 3243 2d34 3036 432d 4244 4536  8-532C-406C-BDE6
-000063d0: 2d41 3738 3246 3033 3530 3844 3522 2c0a  -A782F03508D5",.
-000063e0: 2020 2020 2020 2242 7573 696e 6573 7344        "BusinessD
-000063f0: 6573 6372 6970 7469 6f6e 223a 2022 4865  escription": "He
-00006400: 7265 2069 7320 616e 2075 7064 6174 6564  re is an updated
-00006410: 2062 7573 696e 6573 7320 6465 7363 7269   business descri
-00006420: 7074 696f 6e21 222c 0a20 207d 0a5d 0a72  ption!",.  }.].r
-00006430: 6573 706f 6e73 6573 203d 2064 632e 696e  esponses = dc.in
-00006440: 7365 7274 5f64 6174 6128 0a20 2020 6f62  sert_data(.   ob
-00006450: 6a65 6374 5f61 7069 5f6e 616d 6520 3d20  ject_api_name = 
-00006460: 2243 6f6d 7061 6e79 222c 0a20 2020 6461  "Company",.   da
-00006470: 7461 203d 2074 6f5f 7365 6e64 2c0a 2020  ta = to_send,.  
-00006480: 2075 7365 5f64 6561 6c63 6c6f 7564 5f69   use_dealcloud_i
-00006490: 6473 203d 2046 616c 7365 2c0a 2020 206c  ds = False,.   l
-000064a0: 6f6f 6b75 705f 636f 6c75 6d6e 203d 2022  ookup_column = "
-000064b0: 4578 7465 726e 616c 5379 7374 656d 4964  ExternalSystemId
-000064c0: 220a 290a 6060 600a 0a23 2323 2320 5570  ".).```..#### Up
-000064d0: 7365 7274 2044 6174 610a 5570 7365 7274  sert Data.Upsert
-000064e0: 696e 6720 6461 7461 2069 7320 6120 6d65  ing data is a me
-000064f0: 7468 6f64 2074 6861 7420 636f 6d62 696e  thod that combin
-00006500: 6573 2069 6e73 6572 7420 616e 6420 7570  es insert and up
-00006510: 6461 7465 2e20 4966 2061 2072 6563 6f72  date. If a recor
-00006520: 6420 6578 6973 7473 2061 6e64 2063 616e  d exists and can
-00006530: 2062 6520 666f 756e 6420 6279 2060 456e   be found by `En
-00006540: 7472 7949 6460 206f 7220 6120 606c 6f6f  tryId` or a `loo
-00006550: 6b75 705f 636f 6c75 6d6e 6020 7468 656e  kup_column` then
-00006560: 2069 7420 7769 6c6c 2062 6520 7570 6461   it will be upda
-00006570: 7465 642c 2069 6620 6e6f 742c 2069 7420  ted, if not, it 
-00006580: 7769 6c6c 2062 6520 6372 6561 7465 6420  will be created 
-00006590: 6e65 772e 0a0a 4578 616d 706c 652c 2074  new...Example, t
-000065a0: 6f20 7570 7365 7274 2064 6174 6120 696e  o upsert data in
-000065b0: 2074 6865 2022 436f 6d70 616e 7922 206f   the "Company" o
-000065c0: 626a 6563 7420 6672 6f6d 2061 206c 6973  bject from a lis
-000065d0: 743a 0a0a 6060 6070 7974 686f 6e0a 6672  t:..```python.fr
-000065e0: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
-000065f0: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
-00006600: 640a 0a64 6320 3d20 4465 616c 436c 6f75  d..dc = DealClou
-00006610: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
-00006620: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
-00006630: 5f66 696c 652e 6a73 6f6e 2229 0a0a 746f  _file.json")..to
-00006640: 5f73 656e 6420 3d20 5b0a 2020 207b 0a20  _send = [.   {. 
-00006650: 2020 2022 456e 7472 7949 6422 3a20 3233     "EntryId": 23
-00006660: 3435 3637 2c20 200a 2020 2020 2243 6f6d  4567,  .    "Com
-00006670: 7061 6e79 4e61 6d65 223a 2022 5465 7374  panyName": "Test
-00006680: 2043 6f6d 7061 6e79 2031 222c 0a20 2020   Company 1",.   
-00006690: 2022 436f 6d70 616e 7954 7970 6522 3a20   "CompanyType": 
-000066a0: 3132 3334 352c 0a20 2020 2022 4275 7369  12345,.    "Busi
-000066b0: 6e65 7373 4465 7363 7269 7074 696f 6e22  nessDescription"
-000066c0: 3a20 2248 6572 6520 6973 2061 6e20 7570  : "Here is an up
-000066d0: 6461 7465 6420 6275 7369 6e65 7373 2064  dated business d
-000066e0: 6573 6372 6970 7469 6f6e 222c 0a20 2020  escription",.   
-000066f0: 2022 5365 6374 6f72 223a 2031 3433 3231   "Sector": 14321
-00006700: 2c0a 2020 207d 2c0a 2020 207b 0a20 2020  ,.   },.   {.   
-00006710: 2022 436f 6d70 616e 794e 616d 6522 3a20   "CompanyName": 
-00006720: 2254 6573 7420 436f 6d70 616e 7920 3222  "Test Company 2"
-00006730: 2c0a 2020 2020 2243 6f6d 7061 6e79 5479  ,.    "CompanyTy
-00006740: 7065 223a 2031 3233 3435 2c0a 2020 2020  pe": 12345,.    
-00006750: 2242 7573 696e 6573 7344 6573 6372 6970  "BusinessDescrip
-00006760: 7469 6f6e 223a 2022 4865 7265 2069 7320  tion": "Here is 
-00006770: 6120 6275 7369 6e65 7373 2064 6573 6372  a business descr
-00006780: 6970 7469 6f6e 2066 6f72 2061 206e 6577  iption for a new
-00006790: 2063 6f6d 7061 6e79 222c 0a20 2020 2022   company",.    "
-000067a0: 5365 6374 6f72 223a 2031 3433 3231 2c0a  Sector": 14321,.
-000067b0: 2020 207d 2c0a 5d0a 7265 7370 6f6e 7365     },.].response
-000067c0: 7320 3d20 6463 2e69 6e73 6572 745f 6461  s = dc.insert_da
-000067d0: 7461 2822 436f 6d70 616e 7922 2c20 746f  ta("Company", to
-000067e0: 5f73 656e 6429 0a60 6060 0a49 6620 7375  _send).```.If su
-000067f0: 6363 6573 7366 756c 2c20 6072 6573 706f  ccessful, `respo
-00006800: 6e73 6573 6020 7769 6c6c 2063 6f6e 7461  nses` will conta
-00006810: 696e 2074 6865 2062 656c 6f77 2c20 6e6f  in the below, no
-00006820: 7465 2074 6861 7420 7468 6520 2254 6573  te that the "Tes
-00006830: 7420 436f 6d70 616e 7920 3222 206e 6f77  t Company 2" now
-00006840: 2068 6173 2061 6e20 6045 6e74 7279 4964   has an `EntryId
-00006850: 6020 6173 2069 7420 6861 7320 6265 656e  ` as it has been
-00006860: 2063 7265 6174 6564 3a0a 6060 6070 7974   created:.```pyt
-00006870: 686f 6e0a 5b0a 2020 207b 0a20 2020 2022  hon.[.   {.    "
-00006880: 456e 7472 7949 6422 3a20 3233 3435 3637  EntryId": 234567
-00006890: 2c20 200a 2020 2020 2243 6f6d 7061 6e79  ,  .    "Company
-000068a0: 4e61 6d65 223a 2022 5465 7374 2043 6f6d  Name": "Test Com
-000068b0: 7061 6e79 2031 222c 0a20 2020 2022 436f  pany 1",.    "Co
-000068c0: 6d70 616e 7954 7970 6522 3a20 3132 3334  mpanyType": 1234
-000068d0: 352c 0a20 2020 2022 4275 7369 6e65 7373  5,.    "Business
-000068e0: 4465 7363 7269 7074 696f 6e22 3a20 2248  Description": "H
-000068f0: 6572 6520 6973 2061 6e20 7570 6461 7465  ere is an update
-00006900: 6420 6275 7369 6e65 7373 2064 6573 6372  d business descr
-00006910: 6970 7469 6f6e 222c 0a20 2020 2022 5365  iption",.    "Se
-00006920: 6374 6f72 223a 2031 3433 3231 2c0a 2020  ctor": 14321,.  
-00006930: 207d 2c0a 2020 207b 0a20 2020 2022 456e   },.   {.    "En
-00006940: 7472 7949 6422 3a20 3233 3435 3638 2c0a  tryId": 234568,.
-00006950: 2020 2020 2243 6f6d 7061 6e79 4e61 6d65      "CompanyName
-00006960: 223a 2022 5465 7374 2043 6f6d 7061 6e79  ": "Test Company
-00006970: 2032 222c 0a20 2020 2022 436f 6d70 616e   2",.    "Compan
-00006980: 7954 7970 6522 3a20 3132 3334 352c 0a20  yType": 12345,. 
-00006990: 2020 2022 4275 7369 6e65 7373 4465 7363     "BusinessDesc
-000069a0: 7269 7074 696f 6e22 3a20 2248 6572 6520  ription": "Here 
-000069b0: 6973 2061 2062 7573 696e 6573 7320 6465  is a business de
-000069c0: 7363 7269 7074 696f 6e20 666f 7220 6120  scription for a 
-000069d0: 6e65 7720 636f 6d70 616e 7922 2c0a 2020  new company",.  
-000069e0: 2020 2253 6563 746f 7222 3a20 3134 3332    "Sector": 1432
-000069f0: 312c 0a20 2020 7d2c 0a5d 0a60 6060 0a23  1,.   },.].```.#
-00006a00: 2323 2320 556e 6465 7273 7461 6e64 696e  ### Understandin
-00006a10: 6720 4572 726f 7273 0a54 6865 2064 6174  g Errors.The dat
-00006a20: 6120 6f70 6572 6174 696f 6e20 6d65 7468  a operation meth
-00006a30: 6f64 7320 7261 6973 6520 6572 726f 7273  ods raise errors
-00006a40: 2069 6e20 6120 6e75 6d62 6572 206f 6620   in a number of 
-00006a50: 7761 7973 2c20 7768 656e 2060 7573 655f  ways, when `use_
-00006a60: 6465 616c 636c 6f75 645f 6964 7360 2069  dealcloud_ids` i
-00006a70: 7320 6046 616c 7365 602c 2065 7272 6f72  s `False`, error
-00006a80: 7320 6172 6520 6665 6420 6261 636b 2066  s are fed back f
-00006a90: 726f 6d20 7468 6520 4150 4920 696e 746f  rom the API into
-00006aa0: 2074 6865 2064 6174 6120 7265 7475 726e   the data return
-00006ab0: 6564 2066 726f 6d20 7468 6520 6675 6e63  ed from the func
-00006ac0: 7469 6f6e 2e0a 4578 616d 706c 652c 2069  tion..Example, i
-00006ad0: 6620 7468 6520 7365 6374 6f72 2031 3233  f the sector 123
-00006ae0: 3435 2064 6f65 7320 6e6f 7420 6578 6973  45 does not exis
-00006af0: 743a 0a0a 6060 6070 7974 686f 6e0a 6672  t:..```python.fr
-00006b00: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
-00006b10: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
-00006b20: 640a 0a64 6320 3d20 4465 616c 436c 6f75  d..dc = DealClou
-00006b30: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
-00006b40: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
-00006b50: 5f66 696c 652e 6a73 6f6e 2229 0a0a 746f  _file.json")..to
-00006b60: 5f73 656e 6420 3d20 5b0a 2020 2020 7b27  _send = [.    {'
-00006b70: 436f 6d70 616e 794e 616d 6527 3a20 2754  CompanyName': 'T
-00006b80: 4553 545f 5550 4441 5445 4427 2c20 2253  EST_UPDATED', "S
-00006b90: 6563 746f 7222 3a20 3132 3334 357d 0a5d  ector": 12345}.]
-00006ba0: 0a72 6573 706f 6e73 6573 203d 2064 632e  .responses = dc.
-00006bb0: 696e 7365 7274 5f64 6174 6128 2257 4a5f  insert_data("WJ_
-00006bc0: 436f 6d70 616e 7922 2c20 746f 5f73 656e  Company", to_sen
-00006bd0: 6429 0a60 6060 0a60 7265 7370 6f6e 7365  d).```.`response
-00006be0: 7360 2077 696c 6c20 636f 6e74 6169 6e2e  s` will contain.
-00006bf0: 0a60 6060 7079 7468 6f6e 0a5b 7b27 456e  .```python.[{'En
-00006c00: 7472 7949 6427 3a20 2d31 2c0a 2020 2743  tryId': -1,.  'C
-00006c10: 6f6d 7061 6e79 4e61 6d65 273a 2027 5445  ompanyName': 'TE
-00006c20: 5354 5f55 5044 4154 4544 272c 0a20 2027  ST_UPDATED',.  '
-00006c30: 5365 6374 6f72 273a 204e 6f6e 652c 0a20  Sector': None,. 
-00006c40: 2027 4572 726f 7273 273a 205b 7b27 6669   'Errors': [{'fi
-00006c50: 656c 6427 3a20 2753 6563 746f 7227 2c0a  eld': 'Sector',.
-00006c60: 2020 2020 2763 6f64 6527 3a20 3530 3036      'code': 5006
-00006c70: 2c0a 2020 2020 2764 6573 6372 6970 7469  ,.    'descripti
-00006c80: 6f6e 273a 2027 4f6e 6520 6f72 206d 6f72  on': 'One or mor
-00006c90: 6520 7265 6665 7265 6e63 6564 2065 6e74  e referenced ent
-00006ca0: 7269 6573 2061 7265 206e 6f74 2076 616c  ries are not val
-00006cb0: 6964 2066 6f72 2074 6869 7320 6669 656c  id for this fiel
-00006cc0: 642e 277d 5d7d 5d0a 6060 600a 3e20 5b21  d.'}]}].```.> [!
-00006cd0: 4e4f 5445 5d0a 3e20 496e 2074 6869 7320  NOTE].> In this 
-00006ce0: 6361 7365 2c20 7468 6520 7265 636f 7264  case, the record
-00006cf0: 2068 6173 206e 6f74 2062 6565 6e20 6372   has not been cr
-00006d00: 6561 7465 6420 696e 2074 6865 2073 6974  eated in the sit
-00006d10: 652e 2057 6865 6e20 6d75 6c74 6970 6c65  e. When multiple
-00006d20: 2072 6563 6f72 6473 2061 7265 2074 7279   records are try
-00006d30: 696e 6720 746f 2062 6520 6d61 6465 2061  ing to be made a
-00006d40: 6e64 2061 6e79 206f 6e65 2066 6169 6c73  nd any one fails
-00006d50: 2069 6e20 7468 6973 2077 6179 2c20 6e6f   in this way, no
-00006d60: 6e65 206f 6620 7468 6520 7265 636f 7264  ne of the record
-00006d70: 7320 696e 2074 6861 7420 6772 6f75 7020  s in that group 
-00006d80: 7769 6c6c 2062 6520 6372 6561 7465 642e  will be created.
-00006d90: 2057 6865 6e20 6120 6c61 7267 6520 766f   When a large vo
-00006da0: 6c75 6d65 206f 6620 7265 636f 7264 7320  lume of records 
-00006db0: 6172 6520 6265 696e 6720 6372 6561 7465  are being create
-00006dc0: 642c 2060 4465 616c 436c 6f75 6460 2068  d, `DealCloud` h
-00006dd0: 616e 646c 6573 2062 7265 616b 696e 6720  andles breaking 
-00006de0: 7468 6520 6c61 7267 6520 766f 6c75 6d65  the large volume
-00006df0: 206f 6620 6461 7461 2069 6e74 6f20 6d75   of data into mu
-00006e00: 6c74 6970 6c65 2070 6167 6573 2e20 496e  ltiple pages. In
-00006e10: 2074 6869 7320 6361 7365 2c20 7768 6572   this case, wher
-00006e20: 6520 7468 6572 6520 6973 2061 6e20 6572  e there is an er
-00006e30: 726f 7220 6f6e 2061 2072 6563 6f72 6420  ror on a record 
-00006e40: 696e 2061 2070 6167 652c 2061 6c6c 206f  in a page, all o
-00006e50: 6620 7468 6520 7265 636f 7264 7320 696e  f the records in
-00006e60: 2074 6861 7420 7061 6765 2077 696c 6c20   that page will 
-00006e70: 6e6f 7420 6265 2063 7265 6174 6564 2f75  not be created/u
-00006e80: 7064 6174 6564 2e0a 0a57 6865 6e20 6075  pdated...When `u
-00006e90: 7365 5f64 6561 6c63 6c6f 7564 5f69 6473  se_dealcloud_ids
-00006ea0: 6020 6973 2060 5472 7565 602c 2061 6e64  ` is `True`, and
-00006eb0: 206c 6f6f 6b75 7020 7661 6c75 6573 2061   lookup values a
-00006ec0: 7265 2075 7365 642c 2074 6865 2063 7265  re used, the cre
-00006ed0: 6174 652f 7570 6461 7465 2f75 7073 6572  ate/update/upser
-00006ee0: 7420 6d65 7468 6f64 7320 6172 6520 6c65  t methods are le
-00006ef0: 7373 2070 726f 6e65 2074 6f20 2266 6169  ss prone to "fai
-00006f00: 6c69 6e67 2220 6572 726f 7273 2e20 5468  ling" errors. Th
-00006f10: 6973 2069 7320 6265 6361 7573 652c 2077  is is because, w
-00006f20: 6865 6e20 6120 7661 6c75 6520 6973 2062  hen a value is b
-00006f30: 6569 6e67 2072 6573 6f6c 7665 6420 7468  eing resolved th
-00006f40: 726f 7567 6820 6120 606c 6f6f 6b75 705f  rough a `lookup_
-00006f50: 636f 6c75 6d6e 602c 2061 2076 616c 7565  column`, a value
-00006f60: 2074 6861 7420 6361 6e6e 6f74 2062 6520   that cannot be 
-00006f70: 666f 756e 6420 7769 6c6c 2072 6573 756c  found will resul
-00006f80: 7420 696e 2061 6e20 6572 726f 7220 6265  t in an error be
-00006f90: 696e 6720 6c6f 6767 6564 2074 6f20 7468  ing logged to th
-00006fa0: 6520 636f 6e66 6967 7572 6564 206c 6f67  e configured log
-00006fb0: 6765 722e 2048 6f77 6576 6572 2c20 6173  ger. However, as
-00006fc0: 2074 6865 2072 6563 6f72 6420 7072 6f67   the record prog
-00006fd0: 7265 7373 6573 2c20 7468 6520 756e 2d72  resses, the un-r
-00006fe0: 6573 6f6c 7661 626c 6520 7661 6c75 6520  esolvable value 
-00006ff0: 7769 6c6c 2073 696d 706c 7920 6265 2062  will simply be b
-00007000: 6c61 6e6b 2e20 5468 6520 6c6f 6773 2061  lank. The logs a
-00007010: 7070 6561 7220 6173 2062 656c 6f77 3a0a  ppear as below:.
-00007020: 0a46 6f72 2063 686f 6963 6520 6669 656c  .For choice fiel
-00007030: 6473 3a0a 6060 6062 6173 680a 4552 524f  ds:.```bash.ERRO
-00007040: 523a 2043 686f 6963 6520 6d61 7070 696e  R: Choice mappin
-00007050: 6720 6572 726f 7220 6f6e 3a20 7b6f 626a  g error on: {obj
-00007060: 6563 747d 2c20 7b66 6965 6c64 7d2c 2063  ect}, {field}, c
-00007070: 6f75 6c64 206e 6f74 2066 696e 6420 7661  ould not find va
-00007080: 6c75 653a 207b 7661 6c75 657d 0a60 6060  lue: {value}.```
-00007090: 0a46 6f72 2072 6566 6572 656e 6365 2066  .For reference f
-000070a0: 6965 6c64 733a 0a60 6060 6261 7368 0a45  ields:.```bash.E
-000070b0: 5252 4f52 3a20 5265 6665 7265 6e63 6520  RROR: Reference 
-000070c0: 6d61 7070 696e 6720 6572 726f 7220 6f6e  mapping error on
-000070d0: 3a20 7b6f 626a 6563 747d 2c20 7b66 6965  : {object}, {fie
-000070e0: 6c64 7d2c 2063 6f75 6c64 206e 6f74 2066  ld}, could not f
-000070f0: 696e 6420 7661 6c75 653a 207b 7661 6c75  ind value: {valu
-00007100: 657d 0a60 6060 0a46 6f72 2075 7365 7220  e}.```.For user 
-00007110: 6669 656c 6473 3a0a 6060 6062 6173 680a  fields:.```bash.
-00007120: 4552 524f 523a 2055 7365 7220 6d61 7070  ERROR: User mapp
-00007130: 696e 6720 6572 726f 7220 6f6e 3a20 7b6f  ing error on: {o
-00007140: 626a 6563 747d 2c20 7b66 6965 6c64 7d2c  bject}, {field},
-00007150: 2063 6f75 6c64 206e 6f74 2066 696e 6420   could not find 
-00007160: 7661 6c75 653a 207b 7661 6c75 657d 0a60  value: {value}.`
-00007170: 6060 0a0a 5768 656e 2075 7369 6e67 2060  ``..When using `
-00007180: 4465 616c 436c 6f75 642e 7570 6461 7465  DealCloud.update
-00007190: 5f64 6174 6128 2960 2c20 6966 2061 6e20  _data()`, if an 
-000071a0: 6045 6e74 7279 4964 6020 6361 6e6e 6f74  `EntryId` cannot
-000071b0: 2062 6520 6c6f 6361 7465 642c 2079 6f75   be located, you
-000071c0: 2077 696c 6c20 7365 6520 7468 6520 666f   will see the fo
-000071d0: 6c6c 6f77 696e 6720 6572 726f 723a 0a60  llowing error:.`
-000071e0: 6060 6261 7368 0a45 5252 4f52 3a20 5072  ``bash.ERROR: Pr
-000071f0: 696d 6172 7920 4b65 7920 6572 726f 7220  imary Key error 
-00007200: 6f6e 206f 626a 6563 743a 207b 6f62 6a65  on object: {obje
-00007210: 6374 7d2c 2072 6563 6f72 6420 666f 756e  ct}, record foun
-00007220: 6420 7769 7468 6f75 7420 2745 6e74 7279  d without 'Entry
-00007230: 4964 2720 6669 656c 642e 0a60 6060 0a0a  Id' field..```..
-00007240: 2323 2320 4465 6c65 7465 2044 6174 610a  ### Delete Data.
-00007250: 6044 6561 6c43 6c6f 7564 2e64 656c 6574  `DealCloud.delet
-00007260: 655f 6461 7461 2829 6020 7072 6f76 6964  e_data()` provid
-00007270: 6573 2074 6865 2061 6269 6c69 7479 2074  es the ability t
-00007280: 6f20 6465 6c65 7465 2064 6174 6120 6672  o delete data fr
-00007290: 6f6d 2061 6e20 6f62 6a65 6374 2062 7920  om an object by 
-000072a0: 7468 6520 6045 6e74 7279 4964 602e 2054  the `EntryId`. T
-000072b0: 6f20 7573 6520 6974 2c20 7369 6d70 6c79  o use it, simply
-000072c0: 2070 6173 7320 7468 6520 6f62 6a65 6374   pass the object
-000072d0: 2061 7069 206e 616d 6520 746f 2074 6865   api name to the
-000072e0: 2060 6f62 6a65 6374 5f61 7069 5f6e 616d   `object_api_nam
-000072f0: 6560 2061 7267 756d 656e 740a 616e 6420  e` argument.and 
-00007300: 6120 606c 6973 7460 206f 6620 6045 6e74  a `list` of `Ent
-00007310: 7279 4964 6073 2074 6f20 7468 6520 6072  ryId`s to the `r
-00007320: 6563 6f72 6473 6020 6172 6775 6d65 6e74  ecords` argument
-00007330: 2e0a 0a45 7861 6d70 6c65 2074 6f20 6465  ...Example to de
-00007340: 6c65 7465 2074 776f 2072 6563 6f72 6473  lete two records
-00007350: 2077 6974 6820 7468 6520 456e 7472 7949   with the EntryI
-00007360: 6473 2060 3132 3334 3531 6020 616e 6420  ds `123451` and 
-00007370: 6031 3233 3436 603a 0a0a 6060 6070 7974  `12346`:..```pyt
-00007380: 686f 6e0a 6672 6f6d 2064 6561 6c63 6c6f  hon.from dealclo
-00007390: 7564 5f73 646b 2069 6d70 6f72 7420 4465  ud_sdk import De
-000073a0: 616c 436c 6f75 640a 0a64 6320 3d20 4465  alCloud..dc = De
-000073b0: 616c 436c 6f75 642e 6672 6f6d 5f79 616d  alCloud.from_yam
-000073c0: 6c28 2270 6174 682f 746f 2f79 616d 6c5f  l("path/to/yaml_
-000073d0: 636f 6e66 6967 5f66 696c 652e 6a73 6f6e  config_file.json
-000073e0: 2229 0a0a 7265 7370 6f6e 7365 203d 2064  ")..response = d
-000073f0: 632e 6465 6c65 7465 5f64 6174 6128 0a20  c.delete_data(. 
-00007400: 2020 6f62 6a65 6374 5f61 7069 5f6e 616d    object_api_nam
-00007410: 653d 2243 6f6d 7061 6e79 222c 0a20 2020  e="Company",.   
-00007420: 7265 636f 7264 733d 5b31 3233 3435 2c20  records=[12345, 
-00007430: 3132 3334 365d 0a29 0a60 6060 0a60 7265  12346].).```.`re
-00007440: 7370 6f6e 7365 6020 7769 6c6c 2063 6f6e  sponse` will con
-00007450: 7461 696e 3a0a 6060 6070 7974 686f 6e0a  tain:.```python.
-00007460: 5b0a 2020 207b 2765 6e74 7279 4964 273a  [.   {'entryId':
-00007470: 2031 3233 3435 2c20 2766 6965 6c64 4964   12345, 'fieldId
-00007480: 273a 2030 2c20 2772 6f77 4964 273a 2034  ': 0, 'rowId': 4
-00007490: 3933 3536 3530 2c20 2769 734e 6f44 6174  935650, 'isNoDat
-000074a0: 6127 3a20 4661 6c73 657d 2c0a 2020 207b  a': False},.   {
-000074b0: 2765 6e74 7279 4964 273a 2031 3233 3436  'entryId': 12346
-000074c0: 2c20 2766 6965 6c64 4964 273a 2030 2c20  , 'fieldId': 0, 
-000074d0: 2772 6f77 4964 273a 2034 3933 3536 3530  'rowId': 4935650
-000074e0: 2c20 2769 734e 6f44 6174 6127 3a20 4661  , 'isNoData': Fa
-000074f0: 6c73 657d 2c0a 5d0a 6060 600a            lse},.].```.
+00005b70: 6f6e 222c 0a20 2020 2020 2022 5365 6374  on",.      "Sect
+00005b80: 6f72 223a 2022 3631 3245 3946 4634 2d31  or": "612E9FF4-1
+00005b90: 4438 432d 3431 4237 2d42 3845 442d 3244  D8C-41B7-B8ED-2D
+00005ba0: 3143 3135 3234 3034 3334 222c 0a20 207d  1C15240434",.  }
+00005bb0: 0a5d 0a0a 7265 7370 6f6e 7365 7320 3d20  .]..responses = 
+00005bc0: 6463 2e69 6e73 6572 745f 6461 7461 280a  dc.insert_data(.
+00005bd0: 2020 206f 626a 6563 745f 6170 695f 6e61     object_api_na
+00005be0: 6d65 203d 2022 436f 6d70 616e 7922 2c0a  me = "Company",.
+00005bf0: 2020 2064 6174 6120 3d20 746f 5f73 656e     data = to_sen
+00005c00: 642c 0a20 2020 7573 655f 6465 616c 636c  d,.   use_dealcl
+00005c10: 6f75 645f 6964 7320 3d20 4661 6c73 652c  oud_ids = False,
+00005c20: 0a20 2020 6c6f 6f6b 7570 5f63 6f6c 756d  .   lookup_colum
+00005c30: 6e20 3d20 2245 7874 6572 6e61 6c53 7973  n = "ExternalSys
+00005c40: 7465 6d49 4422 0a29 0a60 6060 0a23 2323  temID".).```.###
+00005c50: 2320 5570 6461 7465 2044 6174 610a 546f  # Update Data.To
+00005c60: 2075 7064 6174 6520 6578 6973 7469 6e67   update existing
+00005c70: 2073 6974 6520 6461 7461 2c20 7468 6520   site data, the 
+00005c80: 7072 6f63 6573 7320 6973 2073 696d 696c  process is simil
+00005c90: 6172 2c20 6578 6365 7074 206f 626a 6563  ar, except objec
+00005ca0: 7473 206d 7573 7420 696e 636c 7564 6520  ts must include 
+00005cb0: 6045 6e74 7279 4964 602c 206f 7220 6120  `EntryId`, or a 
+00005cc0: 7661 6c69 6420 7072 696d 6172 7920 6b65  valid primary ke
+00005cd0: 7920 6279 2060 6c6f 6f6b 7570 5f63 6f6c  y by `lookup_col
+00005ce0: 756d 6e60 2e0a 0a45 7861 6d70 6c65 2c20  umn`...Example, 
+00005cf0: 746f 2075 7064 6174 6520 6461 7461 2069  to update data i
+00005d00: 6e20 7468 6520 2243 6f6d 7061 6e79 2220  n the "Company" 
+00005d10: 6f62 6a65 6374 2066 726f 6d20 6120 6c69  object from a li
+00005d20: 7374 3a0a 0a60 6060 7079 7468 6f6e 0a66  st:..```python.f
+00005d30: 726f 6d20 6465 616c 636c 6f75 645f 7364  rom dealcloud_sd
+00005d40: 6b20 696d 706f 7274 2044 6561 6c43 6c6f  k import DealClo
+00005d50: 7564 0a0a 6463 203d 2044 6561 6c43 6c6f  ud..dc = DealClo
+00005d60: 7564 2e66 726f 6d5f 7961 6d6c 2822 7061  ud.from_yaml("pa
+00005d70: 7468 2f74 6f2f 7961 6d6c 5f63 6f6e 6669  th/to/yaml_confi
+00005d80: 675f 6669 6c65 2e6a 736f 6e22 290a 0a74  g_file.json")..t
+00005d90: 6f5f 7365 6e64 203d 205b 0a20 207b 0a20  o_send = [.  {. 
+00005da0: 2020 2020 2022 456e 7472 7949 6422 3a20       "EntryId": 
+00005db0: 3233 3435 3637 2c0a 2020 2020 2020 2242  234567,.      "B
+00005dc0: 7573 696e 6573 7344 6573 6372 6970 7469  usinessDescripti
+00005dd0: 6f6e 223a 2022 4865 7265 2069 7320 616e  on": "Here is an
+00005de0: 2075 7064 6174 6564 2062 7573 696e 6573   updated busines
+00005df0: 7320 6465 7363 7269 7074 696f 6e21 222c  s description!",
+00005e00: 0a20 207d 0a5d 0a72 6573 706f 6e73 6573  .  }.].responses
+00005e10: 203d 2064 632e 696e 7365 7274 5f64 6174   = dc.insert_dat
+00005e20: 6128 2243 6f6d 7061 6e79 222c 2074 6f5f  a("Company", to_
+00005e30: 7365 6e64 290a 6060 600a 4966 2073 7563  send).```.If suc
+00005e40: 6365 7373 6675 6c2c 2060 7265 7370 6f6e  cessful, `respon
+00005e50: 7365 7360 2077 696c 6c20 636f 6e74 6169  ses` will contai
+00005e60: 6e20 7468 6520 6265 6c6f 773a 0a60 6060  n the below:.```
+00005e70: 7079 7468 6f6e 0a5b 0a20 2020 207b 0a20  python.[.    {. 
+00005e80: 2020 2020 2020 2022 456e 7472 7949 6422         "EntryId"
+00005e90: 3a20 3233 3435 3637 2c0a 2020 2020 2020  : 234567,.      
+00005ea0: 2020 2243 6f6d 7061 6e79 4e61 6d65 223a    "CompanyName":
+00005eb0: 2022 5465 7374 2043 6f6d 7061 6e79 2031   "Test Company 1
+00005ec0: 222c 0a20 2020 2020 2020 2022 436f 6d70  ",.        "Comp
+00005ed0: 616e 7954 7970 6522 3a20 3132 3334 352c  anyType": 12345,
+00005ee0: 0a20 2020 2020 2020 2022 4275 7369 6e65  .        "Busine
+00005ef0: 7373 4465 7363 7269 7074 696f 6e22 3a20  ssDescription": 
+00005f00: 2248 6572 6520 6973 2061 6e20 7570 6461  "Here is an upda
+00005f10: 7465 6420 6275 7369 6e65 7373 2064 6573  ted business des
+00005f20: 6372 6970 7469 6f6e 2122 2c0a 2020 2020  cription!",.    
+00005f30: 2020 2020 2253 6563 746f 7222 3a20 3134      "Sector": 14
+00005f40: 3332 312c 0a20 2020 207d 0a5d 0a60 6060  321,.    }.].```
+00005f50: 0a45 7861 6d70 6c65 2c20 746f 2075 7064  .Example, to upd
+00005f60: 6174 6520 6461 7461 2069 6e20 7468 6520  ate data in the 
+00005f70: 2243 6f6d 7061 6e79 2220 6f62 6a65 6374  "Company" object
+00005f80: 2066 726f 6d20 6120 6c69 7374 2c20 7573   from a list, us
+00005f90: 696e 6720 7468 6520 606c 6f6f 6b75 705f  ing the `lookup_
+00005fa0: 636f 6c75 6d6e 602c 2060 4578 7465 726e  column`, `Extern
+00005fb0: 616c 5379 7374 656d 4964 603a 0a0a 6060  alSystemId`:..``
+00005fc0: 6070 7974 686f 6e0a 6672 6f6d 2064 6561  `python.from dea
+00005fd0: 6c63 6c6f 7564 5f73 646b 2069 6d70 6f72  lcloud_sdk impor
+00005fe0: 7420 4465 616c 436c 6f75 640a 0a64 6320  t DealCloud..dc 
+00005ff0: 3d20 4465 616c 436c 6f75 642e 6672 6f6d  = DealCloud.from
+00006000: 5f79 616d 6c28 2270 6174 682f 746f 2f79  _yaml("path/to/y
+00006010: 616d 6c5f 636f 6e66 6967 5f66 696c 652e  aml_config_file.
+00006020: 6a73 6f6e 2229 0a0a 746f 5f73 656e 6420  json")..to_send 
+00006030: 3d20 5b0a 2020 7b0a 2020 2020 2020 2245  = [.  {.      "E
+00006040: 7874 6572 6e61 6c53 7973 7465 6d49 6422  xternalSystemId"
+00006050: 3a20 2246 3632 3841 4643 382d 3533 3243  : "F628AFC8-532C
+00006060: 2d34 3036 432d 4244 4536 2d41 3738 3246  -406C-BDE6-A782F
+00006070: 3033 3530 3844 3522 2c0a 2020 2020 2020  03508D5",.      
+00006080: 2242 7573 696e 6573 7344 6573 6372 6970  "BusinessDescrip
+00006090: 7469 6f6e 223a 2022 4865 7265 2069 7320  tion": "Here is 
+000060a0: 616e 2075 7064 6174 6564 2062 7573 696e  an updated busin
+000060b0: 6573 7320 6465 7363 7269 7074 696f 6e21  ess description!
+000060c0: 222c 0a20 207d 0a5d 0a72 6573 706f 6e73  ",.  }.].respons
+000060d0: 6573 203d 2064 632e 696e 7365 7274 5f64  es = dc.insert_d
+000060e0: 6174 6128 0a20 2020 6f62 6a65 6374 5f61  ata(.   object_a
+000060f0: 7069 5f6e 616d 6520 3d20 2243 6f6d 7061  pi_name = "Compa
+00006100: 6e79 222c 0a20 2020 6461 7461 203d 2074  ny",.   data = t
+00006110: 6f5f 7365 6e64 2c0a 2020 2075 7365 5f64  o_send,.   use_d
+00006120: 6561 6c63 6c6f 7564 5f69 6473 203d 2046  ealcloud_ids = F
+00006130: 616c 7365 2c0a 2020 206c 6f6f 6b75 705f  alse,.   lookup_
+00006140: 636f 6c75 6d6e 203d 2022 4578 7465 726e  column = "Extern
+00006150: 616c 5379 7374 656d 4964 220a 290a 6060  alSystemId".).``
+00006160: 600a 0a23 2323 2320 5570 7365 7274 2044  `..#### Upsert D
+00006170: 6174 610a 5570 7365 7274 696e 6720 6461  ata.Upserting da
+00006180: 7461 2069 7320 6120 6d65 7468 6f64 2074  ta is a method t
+00006190: 6861 7420 636f 6d62 696e 6573 2069 6e73  hat combines ins
+000061a0: 6572 7420 616e 6420 7570 6461 7465 2e20  ert and update. 
+000061b0: 4966 2061 2072 6563 6f72 6420 6578 6973  If a record exis
+000061c0: 7473 2061 6e64 2063 616e 2062 6520 666f  ts and can be fo
+000061d0: 756e 6420 6279 2060 456e 7472 7949 6460  und by `EntryId`
+000061e0: 206f 7220 6120 606c 6f6f 6b75 705f 636f   or a `lookup_co
+000061f0: 6c75 6d6e 6020 7468 656e 2069 7420 7769  lumn` then it wi
+00006200: 6c6c 2062 6520 7570 6461 7465 642c 2069  ll be updated, i
+00006210: 6620 6e6f 742c 2069 7420 7769 6c6c 2062  f not, it will b
+00006220: 6520 6372 6561 7465 6420 6e65 772e 0a0a  e created new...
+00006230: 4578 616d 706c 652c 2074 6f20 7570 7365  Example, to upse
+00006240: 7274 2064 6174 6120 696e 2074 6865 2022  rt data in the "
+00006250: 436f 6d70 616e 7922 206f 626a 6563 7420  Company" object 
+00006260: 6672 6f6d 2061 206c 6973 743a 0a0a 6060  from a list:..``
+00006270: 6070 7974 686f 6e0a 6672 6f6d 2064 6561  `python.from dea
+00006280: 6c63 6c6f 7564 5f73 646b 2069 6d70 6f72  lcloud_sdk impor
+00006290: 7420 4465 616c 436c 6f75 640a 0a64 6320  t DealCloud..dc 
+000062a0: 3d20 4465 616c 436c 6f75 642e 6672 6f6d  = DealCloud.from
+000062b0: 5f79 616d 6c28 2270 6174 682f 746f 2f79  _yaml("path/to/y
+000062c0: 616d 6c5f 636f 6e66 6967 5f66 696c 652e  aml_config_file.
+000062d0: 6a73 6f6e 2229 0a0a 746f 5f73 656e 6420  json")..to_send 
+000062e0: 3d20 5b0a 2020 207b 0a20 2020 2022 456e  = [.   {.    "En
+000062f0: 7472 7949 6422 3a20 3233 3435 3637 2c20  tryId": 234567, 
+00006300: 200a 2020 2020 2243 6f6d 7061 6e79 4e61   .    "CompanyNa
+00006310: 6d65 223a 2022 5465 7374 2043 6f6d 7061  me": "Test Compa
+00006320: 6e79 2031 222c 0a20 2020 2022 436f 6d70  ny 1",.    "Comp
+00006330: 616e 7954 7970 6522 3a20 3132 3334 352c  anyType": 12345,
+00006340: 0a20 2020 2022 4275 7369 6e65 7373 4465  .    "BusinessDe
+00006350: 7363 7269 7074 696f 6e22 3a20 2248 6572  scription": "Her
+00006360: 6520 6973 2061 6e20 7570 6461 7465 6420  e is an updated 
+00006370: 6275 7369 6e65 7373 2064 6573 6372 6970  business descrip
+00006380: 7469 6f6e 222c 0a20 2020 2022 5365 6374  tion",.    "Sect
+00006390: 6f72 223a 2031 3433 3231 2c0a 2020 207d  or": 14321,.   }
+000063a0: 2c0a 2020 207b 0a20 2020 2022 436f 6d70  ,.   {.    "Comp
+000063b0: 616e 794e 616d 6522 3a20 2254 6573 7420  anyName": "Test 
+000063c0: 436f 6d70 616e 7920 3222 2c0a 2020 2020  Company 2",.    
+000063d0: 2243 6f6d 7061 6e79 5479 7065 223a 2031  "CompanyType": 1
+000063e0: 3233 3435 2c0a 2020 2020 2242 7573 696e  2345,.    "Busin
+000063f0: 6573 7344 6573 6372 6970 7469 6f6e 223a  essDescription":
+00006400: 2022 4865 7265 2069 7320 6120 6275 7369   "Here is a busi
+00006410: 6e65 7373 2064 6573 6372 6970 7469 6f6e  ness description
+00006420: 2066 6f72 2061 206e 6577 2063 6f6d 7061   for a new compa
+00006430: 6e79 222c 0a20 2020 2022 5365 6374 6f72  ny",.    "Sector
+00006440: 223a 2031 3433 3231 2c0a 2020 207d 2c0a  ": 14321,.   },.
+00006450: 5d0a 7265 7370 6f6e 7365 7320 3d20 6463  ].responses = dc
+00006460: 2e69 6e73 6572 745f 6461 7461 2822 436f  .insert_data("Co
+00006470: 6d70 616e 7922 2c20 746f 5f73 656e 6429  mpany", to_send)
+00006480: 0a60 6060 0a49 6620 7375 6363 6573 7366  .```.If successf
+00006490: 756c 2c20 6072 6573 706f 6e73 6573 6020  ul, `responses` 
+000064a0: 7769 6c6c 2063 6f6e 7461 696e 2074 6865  will contain the
+000064b0: 2062 656c 6f77 2c20 6e6f 7465 2074 6861   below, note tha
+000064c0: 7420 7468 6520 2254 6573 7420 436f 6d70  t the "Test Comp
+000064d0: 616e 7920 3222 206e 6f77 2068 6173 2061  any 2" now has a
+000064e0: 6e20 6045 6e74 7279 4964 6020 6173 2069  n `EntryId` as i
+000064f0: 7420 6861 7320 6265 656e 2063 7265 6174  t has been creat
+00006500: 6564 3a0a 6060 6070 7974 686f 6e0a 5b0a  ed:.```python.[.
+00006510: 2020 207b 0a20 2020 2022 456e 7472 7949     {.    "EntryI
+00006520: 6422 3a20 3233 3435 3637 2c20 200a 2020  d": 234567,  .  
+00006530: 2020 2243 6f6d 7061 6e79 4e61 6d65 223a    "CompanyName":
+00006540: 2022 5465 7374 2043 6f6d 7061 6e79 2031   "Test Company 1
+00006550: 222c 0a20 2020 2022 436f 6d70 616e 7954  ",.    "CompanyT
+00006560: 7970 6522 3a20 3132 3334 352c 0a20 2020  ype": 12345,.   
+00006570: 2022 4275 7369 6e65 7373 4465 7363 7269   "BusinessDescri
+00006580: 7074 696f 6e22 3a20 2248 6572 6520 6973  ption": "Here is
+00006590: 2061 6e20 7570 6461 7465 6420 6275 7369   an updated busi
+000065a0: 6e65 7373 2064 6573 6372 6970 7469 6f6e  ness description
+000065b0: 222c 0a20 2020 2022 5365 6374 6f72 223a  ",.    "Sector":
+000065c0: 2031 3433 3231 2c0a 2020 207d 2c0a 2020   14321,.   },.  
+000065d0: 207b 0a20 2020 2022 456e 7472 7949 6422   {.    "EntryId"
+000065e0: 3a20 3233 3435 3638 2c0a 2020 2020 2243  : 234568,.    "C
+000065f0: 6f6d 7061 6e79 4e61 6d65 223a 2022 5465  ompanyName": "Te
+00006600: 7374 2043 6f6d 7061 6e79 2032 222c 0a20  st Company 2",. 
+00006610: 2020 2022 436f 6d70 616e 7954 7970 6522     "CompanyType"
+00006620: 3a20 3132 3334 352c 0a20 2020 2022 4275  : 12345,.    "Bu
+00006630: 7369 6e65 7373 4465 7363 7269 7074 696f  sinessDescriptio
+00006640: 6e22 3a20 2248 6572 6520 6973 2061 2062  n": "Here is a b
+00006650: 7573 696e 6573 7320 6465 7363 7269 7074  usiness descript
+00006660: 696f 6e20 666f 7220 6120 6e65 7720 636f  ion for a new co
+00006670: 6d70 616e 7922 2c0a 2020 2020 2253 6563  mpany",.    "Sec
+00006680: 746f 7222 3a20 3134 3332 312c 0a20 2020  tor": 14321,.   
+00006690: 7d2c 0a5d 0a60 6060 0a23 2323 2320 556e  },.].```.#### Un
+000066a0: 6465 7273 7461 6e64 696e 6720 4572 726f  derstanding Erro
+000066b0: 7273 0a54 6865 2064 6174 6120 6f70 6572  rs.The data oper
+000066c0: 6174 696f 6e20 6d65 7468 6f64 7320 7261  ation methods ra
+000066d0: 6973 6520 6572 726f 7273 2069 6e20 6120  ise errors in a 
+000066e0: 6e75 6d62 6572 206f 6620 7761 7973 2c20  number of ways, 
+000066f0: 7768 656e 2060 7573 655f 6465 616c 636c  when `use_dealcl
+00006700: 6f75 645f 6964 7360 2069 7320 6046 616c  oud_ids` is `Fal
+00006710: 7365 602c 2065 7272 6f72 7320 6172 6520  se`, errors are 
+00006720: 6665 6420 6261 636b 2066 726f 6d20 7468  fed back from th
+00006730: 6520 4150 4920 696e 746f 2074 6865 2064  e API into the d
+00006740: 6174 6120 7265 7475 726e 6564 2066 726f  ata returned fro
+00006750: 6d20 7468 6520 6675 6e63 7469 6f6e 2e0a  m the function..
+00006760: 4578 616d 706c 652c 2069 6620 7468 6520  Example, if the 
+00006770: 7365 6374 6f72 2031 3233 3435 2064 6f65  sector 12345 doe
+00006780: 7320 6e6f 7420 6578 6973 743a 0a0a 6060  s not exist:..``
+00006790: 6070 7974 686f 6e0a 6672 6f6d 2064 6561  `python.from dea
+000067a0: 6c63 6c6f 7564 5f73 646b 2069 6d70 6f72  lcloud_sdk impor
+000067b0: 7420 4465 616c 436c 6f75 640a 0a64 6320  t DealCloud..dc 
+000067c0: 3d20 4465 616c 436c 6f75 642e 6672 6f6d  = DealCloud.from
+000067d0: 5f79 616d 6c28 2270 6174 682f 746f 2f79  _yaml("path/to/y
+000067e0: 616d 6c5f 636f 6e66 6967 5f66 696c 652e  aml_config_file.
+000067f0: 6a73 6f6e 2229 0a0a 746f 5f73 656e 6420  json")..to_send 
+00006800: 3d20 5b0a 2020 2020 7b27 436f 6d70 616e  = [.    {'Compan
+00006810: 794e 616d 6527 3a20 2754 4553 545f 5550  yName': 'TEST_UP
+00006820: 4441 5445 4427 2c20 2253 6563 746f 7222  DATED', "Sector"
+00006830: 3a20 3132 3334 357d 0a5d 0a72 6573 706f  : 12345}.].respo
+00006840: 6e73 6573 203d 2064 632e 696e 7365 7274  nses = dc.insert
+00006850: 5f64 6174 6128 2257 4a5f 436f 6d70 616e  _data("WJ_Compan
+00006860: 7922 2c20 746f 5f73 656e 6429 0a60 6060  y", to_send).```
+00006870: 0a60 7265 7370 6f6e 7365 7360 2077 696c  .`responses` wil
+00006880: 6c20 636f 6e74 6169 6e2e 0a60 6060 7079  l contain..```py
+00006890: 7468 6f6e 0a5b 7b27 456e 7472 7949 6427  thon.[{'EntryId'
+000068a0: 3a20 2d31 2c0a 2020 2743 6f6d 7061 6e79  : -1,.  'Company
+000068b0: 4e61 6d65 273a 2027 5445 5354 5f55 5044  Name': 'TEST_UPD
+000068c0: 4154 4544 272c 0a20 2027 5365 6374 6f72  ATED',.  'Sector
+000068d0: 273a 204e 6f6e 652c 0a20 2027 4572 726f  ': None,.  'Erro
+000068e0: 7273 273a 205b 7b27 6669 656c 6427 3a20  rs': [{'field': 
+000068f0: 2753 6563 746f 7227 2c0a 2020 2020 2763  'Sector',.    'c
+00006900: 6f64 6527 3a20 3530 3036 2c0a 2020 2020  ode': 5006,.    
+00006910: 2764 6573 6372 6970 7469 6f6e 273a 2027  'description': '
+00006920: 4f6e 6520 6f72 206d 6f72 6520 7265 6665  One or more refe
+00006930: 7265 6e63 6564 2065 6e74 7269 6573 2061  renced entries a
+00006940: 7265 206e 6f74 2076 616c 6964 2066 6f72  re not valid for
+00006950: 2074 6869 7320 6669 656c 642e 277d 5d7d   this field.'}]}
+00006960: 5d0a 6060 600a 3e20 5b21 4e4f 5445 5d0a  ].```.> [!NOTE].
+00006970: 3e20 496e 2074 6869 7320 6361 7365 2c20  > In this case, 
+00006980: 7468 6520 7265 636f 7264 2068 6173 206e  the record has n
+00006990: 6f74 2062 6565 6e20 6372 6561 7465 6420  ot been created 
+000069a0: 696e 2074 6865 2073 6974 652e 2057 6865  in the site. Whe
+000069b0: 6e20 6d75 6c74 6970 6c65 2072 6563 6f72  n multiple recor
+000069c0: 6473 2061 7265 2074 7279 696e 6720 746f  ds are trying to
+000069d0: 2062 6520 6d61 6465 2061 6e64 2061 6e79   be made and any
+000069e0: 206f 6e65 2066 6169 6c73 2069 6e20 7468   one fails in th
+000069f0: 6973 2077 6179 2c20 6e6f 6e65 206f 6620  is way, none of 
+00006a00: 7468 6520 7265 636f 7264 7320 696e 2074  the records in t
+00006a10: 6861 7420 6772 6f75 7020 7769 6c6c 2062  hat group will b
+00006a20: 6520 6372 6561 7465 642e 2057 6865 6e20  e created. When 
+00006a30: 6120 6c61 7267 6520 766f 6c75 6d65 206f  a large volume o
+00006a40: 6620 7265 636f 7264 7320 6172 6520 6265  f records are be
+00006a50: 696e 6720 6372 6561 7465 642c 2060 4465  ing created, `De
+00006a60: 616c 436c 6f75 6460 2068 616e 646c 6573  alCloud` handles
+00006a70: 2062 7265 616b 696e 6720 7468 6520 6c61   breaking the la
+00006a80: 7267 6520 766f 6c75 6d65 206f 6620 6461  rge volume of da
+00006a90: 7461 2069 6e74 6f20 6d75 6c74 6970 6c65  ta into multiple
+00006aa0: 2070 6167 6573 2e20 496e 2074 6869 7320   pages. In this 
+00006ab0: 6361 7365 2c20 7768 6572 6520 7468 6572  case, where ther
+00006ac0: 6520 6973 2061 6e20 6572 726f 7220 6f6e  e is an error on
+00006ad0: 2061 2072 6563 6f72 6420 696e 2061 2070   a record in a p
+00006ae0: 6167 652c 2061 6c6c 206f 6620 7468 6520  age, all of the 
+00006af0: 7265 636f 7264 7320 696e 2074 6861 7420  records in that 
+00006b00: 7061 6765 2077 696c 6c20 6e6f 7420 6265  page will not be
+00006b10: 2063 7265 6174 6564 2f75 7064 6174 6564   created/updated
+00006b20: 2e0a 0a57 6865 6e20 6075 7365 5f64 6561  ...When `use_dea
+00006b30: 6c63 6c6f 7564 5f69 6473 6020 6973 2060  lcloud_ids` is `
+00006b40: 5472 7565 602c 2061 6e64 206c 6f6f 6b75  True`, and looku
+00006b50: 7020 7661 6c75 6573 2061 7265 2075 7365  p values are use
+00006b60: 642c 2074 6865 2063 7265 6174 652f 7570  d, the create/up
+00006b70: 6461 7465 2f75 7073 6572 7420 6d65 7468  date/upsert meth
+00006b80: 6f64 7320 6172 6520 6c65 7373 2070 726f  ods are less pro
+00006b90: 6e65 2074 6f20 2266 6169 6c69 6e67 2220  ne to "failing" 
+00006ba0: 6572 726f 7273 2e20 5468 6973 2069 7320  errors. This is 
+00006bb0: 6265 6361 7573 652c 2077 6865 6e20 6120  because, when a 
+00006bc0: 7661 6c75 6520 6973 2062 6569 6e67 2072  value is being r
+00006bd0: 6573 6f6c 7665 6420 7468 726f 7567 6820  esolved through 
+00006be0: 6120 606c 6f6f 6b75 705f 636f 6c75 6d6e  a `lookup_column
+00006bf0: 602c 2061 2076 616c 7565 2074 6861 7420  `, a value that 
+00006c00: 6361 6e6e 6f74 2062 6520 666f 756e 6420  cannot be found 
+00006c10: 7769 6c6c 2072 6573 756c 7420 696e 2061  will result in a
+00006c20: 6e20 6572 726f 7220 6265 696e 6720 6c6f  n error being lo
+00006c30: 6767 6564 2074 6f20 7468 6520 636f 6e66  gged to the conf
+00006c40: 6967 7572 6564 206c 6f67 6765 722e 2048  igured logger. H
+00006c50: 6f77 6576 6572 2c20 6173 2074 6865 2072  owever, as the r
+00006c60: 6563 6f72 6420 7072 6f67 7265 7373 6573  ecord progresses
+00006c70: 2c20 7468 6520 756e 2d72 6573 6f6c 7661  , the un-resolva
+00006c80: 626c 6520 7661 6c75 6520 7769 6c6c 2073  ble value will s
+00006c90: 696d 706c 7920 6265 2062 6c61 6e6b 2e20  imply be blank. 
+00006ca0: 5468 6520 6c6f 6773 2061 7070 6561 7220  The logs appear 
+00006cb0: 6173 2062 656c 6f77 3a0a 0a46 6f72 2063  as below:..For c
+00006cc0: 686f 6963 6520 6669 656c 6473 3a0a 6060  hoice fields:.``
+00006cd0: 6062 6173 680a 4552 524f 523a 2043 686f  `bash.ERROR: Cho
+00006ce0: 6963 6520 6d61 7070 696e 6720 6572 726f  ice mapping erro
+00006cf0: 7220 6f6e 3a20 7b6f 626a 6563 747d 2c20  r on: {object}, 
+00006d00: 7b66 6965 6c64 7d2c 2063 6f75 6c64 206e  {field}, could n
+00006d10: 6f74 2066 696e 6420 7661 6c75 653a 207b  ot find value: {
+00006d20: 7661 6c75 657d 0a60 6060 0a46 6f72 2072  value}.```.For r
+00006d30: 6566 6572 656e 6365 2066 6965 6c64 733a  eference fields:
+00006d40: 0a60 6060 6261 7368 0a45 5252 4f52 3a20  .```bash.ERROR: 
+00006d50: 5265 6665 7265 6e63 6520 6d61 7070 696e  Reference mappin
+00006d60: 6720 6572 726f 7220 6f6e 3a20 7b6f 626a  g error on: {obj
+00006d70: 6563 747d 2c20 7b66 6965 6c64 7d2c 2063  ect}, {field}, c
+00006d80: 6f75 6c64 206e 6f74 2066 696e 6420 7661  ould not find va
+00006d90: 6c75 653a 207b 7661 6c75 657d 0a60 6060  lue: {value}.```
+00006da0: 0a46 6f72 2075 7365 7220 6669 656c 6473  .For user fields
+00006db0: 3a0a 6060 6062 6173 680a 4552 524f 523a  :.```bash.ERROR:
+00006dc0: 2055 7365 7220 6d61 7070 696e 6720 6572   User mapping er
+00006dd0: 726f 7220 6f6e 3a20 7b6f 626a 6563 747d  ror on: {object}
+00006de0: 2c20 7b66 6965 6c64 7d2c 2063 6f75 6c64  , {field}, could
+00006df0: 206e 6f74 2066 696e 6420 7661 6c75 653a   not find value:
+00006e00: 207b 7661 6c75 657d 0a60 6060 0a0a 5768   {value}.```..Wh
+00006e10: 656e 2075 7369 6e67 2060 4465 616c 436c  en using `DealCl
+00006e20: 6f75 642e 7570 6461 7465 5f64 6174 6128  oud.update_data(
+00006e30: 2960 2c20 6966 2061 6e20 6045 6e74 7279  )`, if an `Entry
+00006e40: 4964 6020 6361 6e6e 6f74 2062 6520 6c6f  Id` cannot be lo
+00006e50: 6361 7465 642c 2079 6f75 2077 696c 6c20  cated, you will 
+00006e60: 7365 6520 7468 6520 666f 6c6c 6f77 696e  see the followin
+00006e70: 6720 6572 726f 723a 0a60 6060 6261 7368  g error:.```bash
+00006e80: 0a45 5252 4f52 3a20 5072 696d 6172 7920  .ERROR: Primary 
+00006e90: 4b65 7920 6572 726f 7220 6f6e 206f 626a  Key error on obj
+00006ea0: 6563 743a 207b 6f62 6a65 6374 7d2c 2072  ect: {object}, r
+00006eb0: 6563 6f72 6420 666f 756e 6420 7769 7468  ecord found with
+00006ec0: 6f75 7420 2745 6e74 7279 4964 2720 6669  out 'EntryId' fi
+00006ed0: 656c 642e 0a60 6060 0a0a 2323 2320 4465  eld..```..### De
+00006ee0: 6c65 7465 2044 6174 610a 6044 6561 6c43  lete Data.`DealC
+00006ef0: 6c6f 7564 2e64 656c 6574 655f 6461 7461  loud.delete_data
+00006f00: 2829 6020 7072 6f76 6964 6573 2074 6865  ()` provides the
+00006f10: 2061 6269 6c69 7479 2074 6f20 6465 6c65   ability to dele
+00006f20: 7465 2064 6174 6120 6672 6f6d 2061 6e20  te data from an 
+00006f30: 6f62 6a65 6374 2062 7920 7468 6520 6045  object by the `E
+00006f40: 6e74 7279 4964 602e 2054 6f20 7573 6520  ntryId`. To use 
+00006f50: 6974 2c20 7369 6d70 6c79 2070 6173 7320  it, simply pass 
+00006f60: 7468 6520 6f62 6a65 6374 2061 7069 206e  the object api n
+00006f70: 616d 6520 746f 2074 6865 2060 6f62 6a65  ame to the `obje
+00006f80: 6374 5f61 7069 5f6e 616d 6560 2061 7267  ct_api_name` arg
+00006f90: 756d 656e 740a 616e 6420 6120 606c 6973  ument.and a `lis
+00006fa0: 7460 206f 6620 6045 6e74 7279 4964 6073  t` of `EntryId`s
+00006fb0: 2074 6f20 7468 6520 6072 6563 6f72 6473   to the `records
+00006fc0: 6020 6172 6775 6d65 6e74 2e0a 0a45 7861  ` argument...Exa
+00006fd0: 6d70 6c65 2074 6f20 6465 6c65 7465 2074  mple to delete t
+00006fe0: 776f 2072 6563 6f72 6473 2077 6974 6820  wo records with 
+00006ff0: 7468 6520 456e 7472 7949 6473 2060 3132  the EntryIds `12
+00007000: 3334 3531 6020 616e 6420 6031 3233 3436  3451` and `12346
+00007010: 603a 0a0a 6060 6070 7974 686f 6e0a 6672  `:..```python.fr
+00007020: 6f6d 2064 6561 6c63 6c6f 7564 5f73 646b  om dealcloud_sdk
+00007030: 2069 6d70 6f72 7420 4465 616c 436c 6f75   import DealClou
+00007040: 640a 0a64 6320 3d20 4465 616c 436c 6f75  d..dc = DealClou
+00007050: 642e 6672 6f6d 5f79 616d 6c28 2270 6174  d.from_yaml("pat
+00007060: 682f 746f 2f79 616d 6c5f 636f 6e66 6967  h/to/yaml_config
+00007070: 5f66 696c 652e 6a73 6f6e 2229 0a0a 7265  _file.json")..re
+00007080: 7370 6f6e 7365 203d 2064 632e 6465 6c65  sponse = dc.dele
+00007090: 7465 5f64 6174 6128 0a20 2020 6f62 6a65  te_data(.   obje
+000070a0: 6374 5f61 7069 5f6e 616d 653d 2243 6f6d  ct_api_name="Com
+000070b0: 7061 6e79 222c 0a20 2020 7265 636f 7264  pany",.   record
+000070c0: 733d 5b31 3233 3435 2c20 3132 3334 365d  s=[12345, 12346]
+000070d0: 0a29 0a60 6060 0a60 7265 7370 6f6e 7365  .).```.`response
+000070e0: 6020 7769 6c6c 2063 6f6e 7461 696e 3a0a  ` will contain:.
+000070f0: 6060 6070 7974 686f 6e0a 5b0a 2020 207b  ```python.[.   {
+00007100: 2765 6e74 7279 4964 273a 2031 3233 3435  'entryId': 12345
+00007110: 2c20 2766 6965 6c64 4964 273a 2030 2c20  , 'fieldId': 0, 
+00007120: 2772 6f77 4964 273a 2034 3933 3536 3530  'rowId': 4935650
+00007130: 2c20 2769 734e 6f44 6174 6127 3a20 4661  , 'isNoData': Fa
+00007140: 6c73 657d 2c0a 2020 207b 2765 6e74 7279  lse},.   {'entry
+00007150: 4964 273a 2031 3233 3436 2c20 2766 6965  Id': 12346, 'fie
+00007160: 6c64 4964 273a 2030 2c20 2772 6f77 4964  ldId': 0, 'rowId
+00007170: 273a 2034 3933 3536 3530 2c20 2769 734e  ': 4935650, 'isN
+00007180: 6f44 6174 6127 3a20 4661 6c73 657d 2c0a  oData': False},.
+00007190: 5d0a 6060 600a 0a                        ].```..
```

