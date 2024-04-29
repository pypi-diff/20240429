# Comparing `tmp/zenlayercloud-sdk-python-2.0.5.tar.gz` & `tmp/zenlayercloud_sdk_python-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenlayercloud-sdk-python-2.0.5.tar", last modified: Mon Oct 30 06:29:27 2023, max compression
+gzip compressed data, was "zenlayercloud_sdk_python-2.0.7.tar", last modified: Mon Apr 29 13:09:58 2024, max compression
```

## Comparing `zenlayercloud-sdk-python-2.0.5.tar` & `zenlayercloud_sdk_python-2.0.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2023-10-30 06:29:27.403641 zenlayercloud-sdk-python-2.0.5/
--rw-r--r--   0 wolfgang   (501) staff       (20)    11356 2023-07-08 09:12:39.000000 zenlayercloud-sdk-python-2.0.5/LICENSE
--rw-r--r--   0 wolfgang   (501) staff       (20)     1423 2023-10-30 06:29:27.402549 zenlayercloud-sdk-python-2.0.5/PKG-INFO
--rw-r--r--   0 wolfgang   (501) staff       (20)      664 2023-07-08 09:24:35.000000 zenlayercloud-sdk-python-2.0.5/README.rst
--rw-r--r--   0 wolfgang   (501) staff       (20)       38 2023-10-30 06:29:27.403954 zenlayercloud-sdk-python-2.0.5/setup.cfg
--rw-r--r--   0 wolfgang   (501) staff       (20)     1137 2023-07-08 09:12:39.000000 zenlayercloud-sdk-python-2.0.5/setup.py
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2023-10-30 06:29:27.212493 zenlayercloud-sdk-python-2.0.5/zenlayercloud/
--rw-r--r--   0 wolfgang   (501) staff       (20)       94 2023-10-30 06:27:12.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/__init__.py
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2023-10-30 06:29:27.219034 zenlayercloud-sdk-python-2.0.5/zenlayercloud/bmc/
--rw-r--r--   0 wolfgang   (501) staff       (20)       69 2023-07-08 09:07:36.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/bmc/__init__.py
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2023-10-30 06:29:27.228557 zenlayercloud-sdk-python-2.0.5/zenlayercloud/bmc/v20221120/
--rw-r--r--   0 wolfgang   (501) staff       (20)       69 2023-07-08 09:07:36.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/bmc/v20221120/__init__.py
--rw-r--r--   0 wolfgang   (501) staff       (20)    15150 2023-10-30 02:16:18.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/bmc/v20221120/bmc_client.py
--rw-r--r--   0 wolfgang   (501) staff       (20)    72982 2023-10-30 02:16:18.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/bmc/v20221120/models.py
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2023-10-30 06:29:27.314932 zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/
--rw-r--r--   0 wolfgang   (501) staff       (20)        0 2023-07-08 09:07:36.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/__init__.py
--rw-r--r--   0 wolfgang   (501) staff       (20)     5228 2023-07-08 09:12:39.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/abstract_client.py
--rw-r--r--   0 wolfgang   (501) staff       (20)     1626 2023-07-08 09:07:36.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/abstract_model.py
--rw-r--r--   0 wolfgang   (501) staff       (20)     1094 2023-07-08 09:12:39.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/config.py
--rw-r--r--   0 wolfgang   (501) staff       (20)     1180 2023-07-08 09:07:36.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/credential.py
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2023-10-30 06:29:27.339831 zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/excpetion/
--rw-r--r--   0 wolfgang   (501) staff       (20)       69 2023-07-08 09:07:36.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/excpetion/__init__.py
--rw-r--r--   0 wolfgang   (501) staff       (20)      170 2023-07-08 09:07:36.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/excpetion/error_code.py
--rw-r--r--   0 wolfgang   (501) staff       (20)      866 2023-07-08 09:07:36.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/excpetion/zenlayer_cloud_sdk_exception.py
--rw-r--r--   0 wolfgang   (501) staff       (20)     2925 2023-07-08 09:07:36.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/request.py
--rw-r--r--   0 wolfgang   (501) staff       (20)      497 2023-07-08 09:07:36.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/response.py
--rw-r--r--   0 wolfgang   (501) staff       (20)      354 2023-07-08 09:07:36.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/utils.py
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2023-10-30 06:29:27.342132 zenlayercloud-sdk-python-2.0.5/zenlayercloud/sdn/
--rw-r--r--   0 wolfgang   (501) staff       (20)       69 2023-10-30 02:16:18.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/sdn/__init__.py
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2023-10-30 06:29:27.350947 zenlayercloud-sdk-python-2.0.5/zenlayercloud/sdn/v20230830/
--rw-r--r--   0 wolfgang   (501) staff       (20)       69 2023-10-30 02:16:18.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/sdn/v20230830/__init__.py
--rw-r--r--   0 wolfgang   (501) staff       (20)    39623 2023-10-30 06:27:12.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/sdn/v20230830/models.py
--rw-r--r--   0 wolfgang   (501) staff       (20)     8030 2023-10-30 06:27:12.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/sdn/v20230830/sdn_client.py
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2023-10-30 06:29:27.363134 zenlayercloud-sdk-python-2.0.5/zenlayercloud/vm/
--rw-r--r--   0 wolfgang   (501) staff       (20)       69 2023-07-08 09:17:28.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/vm/__init__.py
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2023-10-30 06:29:27.376948 zenlayercloud-sdk-python-2.0.5/zenlayercloud/vm/v20230313/
--rw-r--r--   0 wolfgang   (501) staff       (20)       69 2023-07-08 09:12:39.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/vm/v20230313/__init__.py
--rw-r--r--   0 wolfgang   (501) staff       (20)    69251 2023-10-30 02:16:18.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/vm/v20230313/models.py
--rw-r--r--   0 wolfgang   (501) staff       (20)    16335 2023-10-30 02:16:18.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/vm/v20230313/vm_client.py
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2023-10-30 06:29:27.379412 zenlayercloud-sdk-python-2.0.5/zenlayercloud/zls/
--rw-r--r--   0 wolfgang   (501) staff       (20)       69 2023-10-30 02:16:18.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/zls/__init__.py
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2023-10-30 06:29:27.389568 zenlayercloud-sdk-python-2.0.5/zenlayercloud/zls/v20230804/
--rw-r--r--   0 wolfgang   (501) staff       (20)       69 2023-10-30 02:16:18.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/zls/v20230804/__init__.py
--rw-r--r--   0 wolfgang   (501) staff       (20)     2518 2023-10-30 02:16:18.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/zls/v20230804/models.py
--rw-r--r--   0 wolfgang   (501) staff       (20)      471 2023-10-30 02:16:18.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud/zls/v20230804/zls_client.py
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2023-10-30 06:29:27.399278 zenlayercloud-sdk-python-2.0.5/zenlayercloud_sdk_python.egg-info/
--rw-r--r--   0 wolfgang   (501) staff       (20)     1423 2023-10-30 06:29:27.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 wolfgang   (501) staff       (20)     1311 2023-10-30 06:29:27.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 wolfgang   (501) staff       (20)        1 2023-10-30 06:29:27.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 wolfgang   (501) staff       (20)       17 2023-10-30 06:29:27.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud_sdk_python.egg-info/requires.txt
--rw-r--r--   0 wolfgang   (501) staff       (20)       14 2023-10-30 06:29:27.000000 zenlayercloud-sdk-python-2.0.5/zenlayercloud_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:09:57.995213 zenlayercloud_sdk_python-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-29 13:09:57.995213 zenlayercloud_sdk_python-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:09:57.995213 zenlayercloud_sdk_python-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:09:57.987213 zenlayercloud_sdk_python-2.0.7/zenlayercloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:09:57.987213 zenlayercloud_sdk_python-2.0.7/zenlayercloud/bmc/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/bmc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:09:57.987213 zenlayercloud_sdk_python-2.0.7/zenlayercloud/bmc/v20221120/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/bmc/v20221120/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15150 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/bmc/v20221120/bmc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73044 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/bmc/v20221120/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:09:57.991213 zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:09:57.991213 zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/excpetion/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/excpetion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/excpetion/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/excpetion/zenlayer_cloud_sdk_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:09:57.991213 zenlayercloud_sdk_python-2.0.7/zenlayercloud/sdn/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/sdn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:09:57.991213 zenlayercloud_sdk_python-2.0.7/zenlayercloud/sdn/v20230830/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/sdn/v20230830/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45512 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/sdn/v20230830/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/sdn/v20230830/sdn_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:09:57.991213 zenlayercloud_sdk_python-2.0.7/zenlayercloud/vm/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/vm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:09:57.991213 zenlayercloud_sdk_python-2.0.7/zenlayercloud/vm/v20230313/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/vm/v20230313/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69251 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/vm/v20230313/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16335 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/vm/v20230313/vm_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:09:57.991213 zenlayercloud_sdk_python-2.0.7/zenlayercloud/zls/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/zls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:09:57.995213 zenlayercloud_sdk_python-2.0.7/zenlayercloud/zls/v20230804/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/zls/v20230804/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/zls/v20230804/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-29 13:09:54.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud/zls/v20230804/zls_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:09:57.995213 zenlayercloud_sdk_python-2.0.7/zenlayercloud_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-29 13:09:57.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-29 13:09:57.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:09:57.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 13:09:57.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 13:09:57.000000 zenlayercloud_sdk_python-2.0.7/zenlayercloud_sdk_python.egg-info/top_level.txt
```

### Comparing `zenlayercloud-sdk-python-2.0.5/LICENSE` & `zenlayercloud_sdk_python-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zenlayercloud-sdk-python-2.0.5/PKG-INFO` & `zenlayercloud_sdk_python-2.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenlayercloud-sdk-python
-Version: 2.0.5
+Version: 2.0.7
 Summary: Zenlayer Cloud SDK for Python
 Home-page: https://github.com/zenlayer/zenlayercloud-sdk-python
 Author: Zenlayer Cloud
 Maintainer-email: console_api@zenlayer.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
+Requires-Dist: requests>=2.27.0
 
 =============================
 Zenlayer Cloud SDK for Python
 =============================
 
 Zenlayer Cloud Python SDK is the official software development kit, which allows Python developers to write software that makes use of Zenlayer Cloud services like BMC and VM.
 
@@ -39,9 +40,7 @@
 or download source code from github and install:
 
 .. code-block:: sh
 
     $ git clone https://github.com/zenlayer/zenlayercloud-sdk-python.git
     $ cd zenlayercloud-sdk-python
     $ python setup.py install
-
-
```

### Comparing `zenlayercloud-sdk-python-2.0.5/README.rst` & `zenlayercloud_sdk_python-2.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `zenlayercloud-sdk-python-2.0.5/setup.py` & `zenlayercloud_sdk_python-2.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `zenlayercloud-sdk-python-2.0.5/zenlayercloud/bmc/v20221120/bmc_client.py` & `zenlayercloud_sdk_python-2.0.7/zenlayercloud/bmc/v20221120/bmc_client.py`

 * *Files identical despite different names*

### Comparing `zenlayercloud-sdk-python-2.0.5/zenlayercloud/bmc/v20221120/models.py` & `zenlayercloud_sdk_python-2.0.7/zenlayercloud/bmc/v20221120/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,15 +435,15 @@
         if params.get("partitions") is not None:
             self.partitions = []
             for item in params.get("partitions"):
                 obj = Partition(item)
                 self.partitions.append(obj)
         if params.get("nic") is not None:
             self.nic = Nic(params.get("nic"))
-        self.autoRenew =  params.get("autoRenew")
+        self.autoRenew = params.get("autoRenew")
 
 
 class StartInstancesRequest(AbstractModel):
 
     def __init__(self):
         self.instanceIds = None
 
@@ -855,23 +855,25 @@
         self.zoneId = None
         self.sellStatus = None
         self.internetChargeTypes = None
         self.instanceTypeId = None
         self.maximumBandwidthOut = None
         self.defaultBandwidthOut = None
         self.defaultTrafficPackageSize = None
+        self.qty = None
 
     def _deserialize(self, params):
         self.zoneId = params.get("zoneId")
         self.sellStatus = params.get("sellStatus")
         self.internetChargeTypes = params.get("internetChargeTypes")
         self.instanceTypeId = params.get("instanceTypeId")
         self.maximumBandwidthOut = params.get("maximumBandwidthOut")
         self.defaultBandwidthOut = params.get("defaultBandwidthOut")
         self.defaultTrafficPackageSize = params.get("defaultTrafficPackageSize")
+        self.qty = params.get("qty")
 
 
 class ModifyInstanceBandwidthRequest(AbstractModel):
 
     def __init__(self):
         self.instanceId = None
         self.bandwidthOutMbps = None
@@ -1151,14 +1153,15 @@
         self.requestId = params.get("requestId")
         if params.get("monitorHealthList") is not None:
             self.monitorHealthList = []
             for item in params.get("monitorHealthList"):
                 obj = InstanceHealth(item)
                 self.monitorHealthList.append(obj)
 
+
 class InstanceHealth(AbstractModel):
 
     def __init__(self, params=None):
         if params is None:
             params = {}
         if len(params) > 0:
             self._deserialize(params)
@@ -1182,14 +1185,15 @@
         self.ipmiStatus = params.get("ipmiStatus")
         self.memoryStatus = params.get("memoryStatus")
         self.psuStatus = params.get("psuStatus")
         self.wanPortStatus = params.get("wanPortStatus")
         self.serverBrand = params.get("serverBrand")
         self.serverModel = params.get("serverModel")
 
+
 class DescribeEipAddressesRequest(AbstractModel):
 
     def __init__(self):
         self.eipChargeType = None
         self.eipIds = None
         self.eipStatus = None
         self.instanceId = None
```

### Comparing `zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/abstract_client.py` & `zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/abstract_model.py` & `zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/config.py` & `zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/config.py`

 * *Files identical despite different names*

### Comparing `zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/credential.py` & `zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/excpetion/zenlayer_cloud_sdk_exception.py` & `zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/excpetion/zenlayer_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `zenlayercloud-sdk-python-2.0.5/zenlayercloud/common/request.py` & `zenlayercloud_sdk_python-2.0.7/zenlayercloud/common/request.py`

 * *Files identical despite different names*

### Comparing `zenlayercloud-sdk-python-2.0.5/zenlayercloud/sdn/v20230830/models.py` & `zenlayercloud_sdk_python-2.0.7/zenlayercloud/sdn/v20230830/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #  Zenlayer.com Inc.
 #  Copyright (c) 2014-2023 All Rights Reserved.
 from zenlayercloud.common.abstract_model import AbstractModel
 
+
 class DescribeDatacentersRequest(AbstractModel):
     def __init__(self):
         self.dcIds = None
         self.isPortAvailable = None
 
     def _deserialize(self, params):
         self.dcIds = params.get("dcIds")
         self.isPortAvailable = params.get("isPortAvailable")
 
+
 class DescribeDatacentersResponse(AbstractModel):
 
     def __init__(self):
         self.requestId = None
         self.dcSet = None
 
     def _deserialize(self, params):
@@ -71,31 +73,31 @@
         self.requestId = params.get("requestId")
         if params.get("portPriceSet") is not None:
             self.portPriceSet = []
             for item in params.get("portPriceSet"):
                 obj = PortPrice(item)
                 self.portPriceSet.append(obj)
 
+
 class PortPrice(AbstractModel):
     def __init__(self, params=None):
         if params is None:
             params = {}
         if len(params) > 0:
             self._deserialize(params)
             return
         self.dcId = None
         self.portType = None
-        self.portDailyPrice = None
-        self.portMonthlyPrice = None
+        self.portPrice = None
 
     def _deserialize(self, params):
         self.dcId = params.get("dcId")
         self.portType = params.get("portType")
-        self.portDailyPrice = params.get("portDailyPrice")
-        self.portMonthlyPrice = params.get("portMonthlyPrice")
+        self.portPrice = Price(params.get("portPrice"))
+
 
 class DescribePortsRequest(AbstractModel):
     def __init__(self):
         self.portIds = None
         self.dcId = None
         self.portName = None
         self.portRemarks = None
@@ -247,15 +249,14 @@
 
     def __init__(self):
         self.requestId = None
         self.start = None
         self.end = None
         self.inuseVlanList = None
 
-
     def _deserialize(self, params):
         self.requestId = params.get("requestId")
         self.start = params.get("start")
         self.end = params.get("end")
         self.inuseVlanList = params.get("inuseVlanList")
 
 
@@ -268,15 +269,14 @@
 
 
 class DestroyPortResponse(AbstractModel):
 
     def __init__(self):
         self.requestId = None
 
-
     def _deserialize(self, params):
         self.requestId = params.get("requestId")
 
 
 class ModifyPortAttributeRequest(AbstractModel):
     def __init__(self):
         self.portId = None
@@ -292,15 +292,14 @@
 
 
 class ModifyPortAttributeResponse(AbstractModel):
 
     def __init__(self):
         self.requestId = None
 
-
     def _deserialize(self, params):
         self.requestId = params.get("requestId")
 
 
 class TerminatePortRequest(AbstractModel):
     def __init__(self):
         self.portId = None
@@ -310,15 +309,14 @@
 
 
 class TerminatePortResponse(AbstractModel):
 
     def __init__(self):
         self.requestId = None
 
-
     def _deserialize(self, params):
         self.requestId = params.get("requestId")
 
 
 class RenewPortRequest(AbstractModel):
     def __init__(self):
         self.portId = None
@@ -328,15 +326,14 @@
 
 
 class RenewPortResponse(AbstractModel):
 
     def __init__(self):
         self.requestId = None
 
-
     def _deserialize(self, params):
         self.requestId = params.get("requestId")
 
 
 class DescribePrivateConnectsRequest(AbstractModel):
     def __init__(self):
         self.privateConnectIds = None
@@ -354,22 +351,22 @@
         self.connectivityStatus = params.get("connectivityStatus")
         self.privateConnectStatus = params.get("privateConnectStatus")
         self.endpointTypes = params.get("endpointTypes")
         self.resourceGroupId = params.get("resourceGroupId")
         self.pageNum = params.get("pageNum")
         self.pageSize = params.get("pageSize")
 
+
 class DescribePrivateConnectsResponse(AbstractModel):
 
     def __init__(self):
         self.requestId = None
         self.totalCount = None
         self.dataSet = None
 
-
     def _deserialize(self, params):
         self.requestId = params.get("requestId")
         self.totalCount = params.get("totalCount")
         if params.get("dataSet") is not None:
             self.dataSet = []
             for item in params.get("dataSet"):
                 obj = PrivateConnect(item)
@@ -418,82 +415,120 @@
         if params is None:
             params = {}
         if len(params) > 0:
             self._deserialize(params)
             return
         self.endpointId = None
         self.endpointName = None
+        self.cloudRegionId = None
+        self.cloudAccountId = None
         self.endpointType = None
         self.dataCenter = None
         self.vlanId = None
         self.connectivityStatus = None
 
     def _deserialize(self, params):
         self.endpointId = params.get("endpointId")
         self.endpointName = params.get("endpointName")
+        self.cloudRegionId = params.get("cloudRegionId")
+        self.cloudAccountId = params.get("cloudAccountId")
         self.endpointType = params.get("endpointType")
         if params.get("dataCenter") is not None:
             self.dataCenter = DatacenterInfo(params.get("dataCenter"))
         self.vlanId = params.get("vlanId")
         self.connectivityStatus = params.get("connectivityStatus")
 
 
-
 class DatacenterInfo(AbstractModel):
     def __init__(self, params=None):
         if params is None:
             params = {}
         if len(params) > 0:
             self._deserialize(params)
             return
         self.dcId = None
         self.dcName = None
         self.dcAddress = None
         self.cityName = None
         self.countryName = None
         self.areaName = None
+        self.latitude = None
+        self.longitude = None
 
     def _deserialize(self, params):
         self.dcId = params.get("dcId")
         self.dcName = params.get("dcName")
         self.dcAddress = params.get("dcAddress")
         self.cityName = params.get("cityName")
         self.countryName = params.get("countryName")
         self.areaName = params.get("areaName")
+        self.areaName = params.get("latitude")
+        self.areaName = params.get("longitude")
 
 
 class DescribeCreatePrivateConnectAvailableSubnetsRequest(AbstractModel):
     def __init__(self):
         self.dcId = None
         self.pageNum = None
         self.pageSize = None
 
     def _deserialize(self, params):
         self.dcId = params.get("dcId")
         self.pageNum = params.get("pageNum")
         self.pageSize = params.get("pageSize")
 
+
 class DescribeCreatePrivateConnectAvailableSubnetsResponse(AbstractModel):
 
     def __init__(self):
         self.requestId = None
         self.totalCount = None
         self.dataSet = None
 
-
     def _deserialize(self, params):
         self.requestId = params.get("requestId")
         self.totalCount = params.get("totalCount")
         if params.get("dataSet") is not None:
             self.dataSet = []
             for item in params.get("dataSet"):
                 obj = PrivateConnectAvailableSubnet(item)
                 self.dataSet.append(obj)
 
 
+class DescribePrivateConnectAvailablePortsRequest(AbstractModel):
+    def __init__(self):
+        self.portIds = None
+        self.dcId = None
+        self.pageNum = None
+        self.pageSize = None
+
+    def _deserialize(self, params):
+        self.portIds = params.get("portIds")
+        self.dcId = params.get("dcId")
+        self.pageNum = params.get("pageNum")
+        self.pageSize = params.get("pageSize")
+
+
+class DescribePrivateConnectAvailablePortsResponse(AbstractModel):
+
+    def __init__(self):
+        self.requestId = None
+        self.totalCount = None
+        self.dataSet = None
+
+    def _deserialize(self, params):
+        self.requestId = params.get("requestId")
+        self.totalCount = params.get("totalCount")
+        if params.get("dataSet") is not None:
+            self.dataSet = []
+            for item in params.get("dataSet"):
+                obj = PortInfo(item)
+                self.dataSet.append(obj)
+
+
 class PrivateConnectAvailableSubnet(AbstractModel):
     def __init__(self, params=None):
         if params is None:
             params = {}
         if len(params) > 0:
             self._deserialize(params)
             return
@@ -525,14 +560,15 @@
         if params.get("endpointA") is not None:
             self.endpointA = CreateEndpointParam(params.get("endpointA"))
         if params.get("endpointZ") is not None:
             self.endpointZ = CreateEndpointParam(params.get("endpointZ"))
         self.bandwidthMbps = params.get("bandwidthMbps")
         self.resourceGroupId = params.get("resourceGroupId")
 
+
 class CreatePrivateConnectResponse(AbstractModel):
 
     def __init__(self):
         self.requestId = None
         self.privateConnectId = None
 
     def _deserialize(self, params):
@@ -543,24 +579,28 @@
 class CreateEndpointParam(AbstractModel):
     def __init__(self, params=None):
         if params is None:
             params = {}
         if len(params) > 0:
             self._deserialize(params)
             return
-        self.subnetId = None
         self.portId = None
         self.vlanId = None
-
+        self.cloudAccountId = None
+        self.cloudType = None
+        self.cloudRegionId = None
+        self.dcId = None
 
     def _deserialize(self, params):
-        self.subnetId = params.get("subnetId")
         self.portId = params.get("portId")
         self.vlanId = params.get("vlanId")
-
+        self.cloudAccountId = params.get("cloudAccountId")
+        self.cloudType = params.get("cloudType")
+        self.cloudRegionId = params.get("cloudRegionId")
+        self.dcId = params.get("dcId")
 
 
 class ModifyPrivateConnectsAttributeRequest(AbstractModel):
     def __init__(self):
         self.privateConnectIds = None
         self.privateConnectName = None
 
@@ -649,15 +689,14 @@
     def _deserialize(self, params):
         self.stepStart = params.get("stepStart")
         self.stepEnd = params.get("stepEnd")
         self.unitPrice = params.get("unitPrice")
         self.discountUnitPrice = params.get("discountUnitPrice")
 
 
-
 class DeletePrivateConnectRequest(AbstractModel):
     def __init__(self):
         self.privateConnectId = None
 
     def _deserialize(self, params):
         self.privateConnectId = params.get("privateConnectId")
 
@@ -701,15 +740,14 @@
     def __init__(self):
         self.requestId = None
 
     def _deserialize(self, params):
         self.requestId = params.get("requestId")
 
 
-
 class DescribePrivateConnectTrafficRequest(AbstractModel):
     def __init__(self):
         self.privateConnectId = None
         self.startTime = None
         self.endTime = None
 
     def _deserialize(self, params):
@@ -749,15 +787,14 @@
         self.out95 = params.get("out95")
         self.outAvg = params.get("outAvg")
         self.outMax = params.get("outMax")
         self.outMin = params.get("outMin")
         self.unit = params.get("unit")
 
 
-
 class ModifyPrivateConnectBandwidthRequest(AbstractModel):
     def __init__(self):
         self.privateConnectId = None
         self.bandwidthMbps = None
 
     def _deserialize(self, params):
         self.privateConnectId = params.get("privateConnectId")
@@ -774,28 +811,29 @@
 
 
 class DescribeCloudRoutersRequest(AbstractModel):
     def __init__(self):
         self.cloudRouterIds = None
         self.cloudRouterName = None
         self.cloudRouterStatus = None
-        self.egdePointId = None
+        self.edgePointId = None
         self.resourceGroupId = None
         self.pageNum = None
         self.pageSize = None
 
     def _deserialize(self, params):
         self.cloudRouterIds = params.get("cloudRouterIds")
         self.cloudRouterName = params.get("cloudRouterName")
         self.cloudRouterStatus = params.get("cloudRouterStatus")
-        self.egdePointId = params.get("egdePointId")
+        self.edgePointId = params.get("edgePointId")
         self.resourceGroupId = params.get("resourceGroupId")
         self.pageNum = params.get("pageNum")
         self.pageSize = params.get("pageSize")
 
+
 class DescribeCloudRoutersResponse(AbstractModel):
 
     def __init__(self):
         self.requestId = None
         self.dataSet = None
         self.totalCount = None
 
@@ -861,14 +899,16 @@
         self.edgePointName = None
         self.connectivityStatus = None
         self.dataCenter = None
         self.ipAddress = None
         self.edgePointType = None
         self.vpcId = None
         self.portId = None
+        self.cloudRegionId = None
+        self.cloudAccountId = None
         self.vlanId = None
         self.bandwidthMbps = None
         self.bgpConnection = None
         self.staticRoutes = None
         self.createTime = None
 
     def _deserialize(self, params):
@@ -877,14 +917,16 @@
         self.connectivityStatus = params.get("connectivityStatus")
         if params.get("dataCenter") is not None:
             self.dataCenter = DatacenterInfo(params.get("dataCenter"))
         self.ipAddress = params.get("ipAddress")
         self.edgePointType = params.get("edgePointType")
         self.vpcId = params.get("vpcId")
         self.portId = params.get("portId")
+        self.cloudRegionId = params.get("cloudRegionId")
+        self.cloudAccountId = params.get("cloudAccountId")
         self.vlanId = params.get("vlanId")
         self.bandwidthMbps = params.get("bandwidthMbps")
         if params.get("bgpConnection") is not None:
             self.bgpConnection = BGPConnection(params.get("bgpConnection"))
         if params.get("staticRoutes") is not None:
             self.staticRoutes = []
             for item in params.get("staticRoutes"):
@@ -923,26 +965,26 @@
         self.nextHop = None
 
     def _deserialize(self, params):
         self.prefix = params.get("prefix")
         self.nextHop = params.get("nextHop")
 
 
-
 class DescribeCloudRouterAvailableVpcsRequest(AbstractModel):
     def __init__(self):
         self.vpcId = None
         self.pageNum = None
         self.pageSize = None
 
     def _deserialize(self, params):
         self.vpcId = params.get("vpcId")
         self.pageNum = params.get("pageNum")
         self.pageSize = params.get("pageSize")
 
+
 class DescribeCloudRouterAvailableVpcsResponse(AbstractModel):
 
     def __init__(self):
         self.requestId = None
         self.dataSet = None
         self.totalCount = None
 
@@ -971,14 +1013,15 @@
     def _deserialize(self, params):
         self.vpcId = params.get("vpcId")
         self.vpcName = params.get("vpcName")
         if params.get("dataCenter") is not None:
             self.dataCenter = DatacenterInfo(params.get("dataCenter"))
         self.cidrBlock = params.get("cidrBlock")
 
+
 class DescribeCloudRouterAvailablePortsRequest(AbstractModel):
     def __init__(self):
         self.portIds = None
         self.dcId = None
         self.pageNum = None
         self.pageSize = None
 
@@ -1126,23 +1169,23 @@
     def __init__(self):
         self.requestId = None
 
     def _deserialize(self, params):
         self.requestId = params.get("requestId")
 
 
-class DeleteCloudRouterEdgePointRequest(AbstractModel):
+class DeleteCloudRouterRequest(AbstractModel):
     def __init__(self):
         self.cloudRouterId = None
 
     def _deserialize(self, params):
         self.cloudRouterId = params.get("cloudRouterId")
 
 
-class DeleteCloudRouterEdgePointResponse(AbstractModel):
+class DeleteCloudRouterResponse(AbstractModel):
 
     def __init__(self):
         self.requestId = None
 
     def _deserialize(self, params):
         self.requestId = params.get("requestId")
 
@@ -1275,7 +1318,165 @@
 class ModifyCloudRouterEdgePointResponse(AbstractModel):
 
     def __init__(self):
         self.requestId = None
 
     def _deserialize(self, params):
         self.requestId = params.get("requestId")
+
+
+class DescribeAWSRegionsRequest(AbstractModel):
+    def __init__(self):
+        self.product = None
+
+    def _deserialize(self, params):
+        self.product = params.get("product")
+
+
+class DescribeAWSRegionsResponse(AbstractModel):
+
+    def __init__(self):
+        self.requestId = None
+        self.cloudRegions = None
+
+    def _deserialize(self, params):
+        self.requestId = params.get("requestId")
+        if params.get("cloudRegions") is not None:
+            self.cloudRegions = []
+            for item in params.get("cloudRegions"):
+                obj = CloudRegion(item)
+                self.cloudRegions.append(obj)
+
+
+class CloudRegion(AbstractModel):
+    def __init__(self, params=None):
+        if params is None:
+            params = {}
+        if len(params) > 0:
+            self._deserialize(params)
+            return
+        self.cloudRegionId = None
+        self.dataCenter = None
+        self.products = None
+
+    def _deserialize(self, params):
+        self.cloudRegionId = params.get("cloudRegionId")
+        if params.get("dataCenter") is not None:
+            self.dataCenter = DatacenterInfo(params.get("dataCenter"))
+        self.products = params.get("products")
+
+
+class DescribeAWSVlanUsageRequest(AbstractModel):
+    def __init__(self):
+        self.dcId = None
+
+    def _deserialize(self, params):
+        self.dcId = params.get("dcId")
+
+
+class DescribeAWSVlanUsageResponse(AbstractModel):
+
+    def __init__(self):
+        self.requestId = None
+        self.start = None
+        self.end = None
+        self.usedVlans = None
+
+    def _deserialize(self, params):
+        self.requestId = params.get("requestId")
+        self.start = params.get("start")
+        self.end = params.get("end")
+        self.usedVlans = params.get("usedVlans")
+
+
+class DescribeTencentRegionsRequest(AbstractModel):
+    def __init__(self):
+        self.product = None
+
+    def _deserialize(self, params):
+        self.product = params.get("product")
+
+
+class DescribeTencentRegionsResponse(AbstractModel):
+
+    def __init__(self):
+        self.requestId = None
+        self.cloudRegions = None
+
+    def _deserialize(self, params):
+        self.requestId = params.get("requestId")
+        if params.get("cloudRegions") is not None:
+            self.cloudRegions = []
+            for item in params.get("cloudRegions"):
+                obj = CloudRegion(item)
+                self.cloudRegions.append(obj)
+
+
+class DescribeTencentVlanUsageRequest(AbstractModel):
+    def __init__(self):
+        self.dcId = None
+
+    def _deserialize(self, params):
+        self.dcId = params.get("dcId")
+
+
+class DescribeTencentVlanUsageResponse(AbstractModel):
+
+    def __init__(self):
+        self.requestId = None
+        self.start = None
+        self.end = None
+        self.usedVlans = None
+
+    def _deserialize(self, params):
+        self.requestId = params.get("requestId")
+        self.start = params.get("start")
+        self.end = params.get("end")
+        self.usedVlans = params.get("usedVlans")
+
+
+class DescribeGoogleRegionsRequest(AbstractModel):
+    def __init__(self):
+        self.pairingKey = None
+        self.product = None
+
+    def _deserialize(self, params):
+        self.pairingKey = params.get("pairingKey")
+        self.product = params.get("product")
+
+
+class DescribeGoogleRegionsResponse(AbstractModel):
+
+    def __init__(self):
+        self.requestId = None
+        self.cloudRegions = None
+
+    def _deserialize(self, params):
+        self.requestId = params.get("requestId")
+        if params.get("cloudRegions") is not None:
+            self.cloudRegions = []
+            for item in params.get("cloudRegions"):
+                obj = CloudRegion(item)
+                self.cloudRegions.append(obj)
+
+
+class DescribeGoogleVlanUsageRequest(AbstractModel):
+    def __init__(self):
+        self.dcId = None
+
+    def _deserialize(self, params):
+        self.dcId = params.get("dcId")
+
+
+class DescribeGoogleVlanUsageResponse(AbstractModel):
+
+    def __init__(self):
+        self.requestId = None
+        self.start = None
+        self.end = None
+        self.usedVlans = None
+
+    def _deserialize(self, params):
+        self.requestId = params.get("requestId")
+        self.start = params.get("start")
+        self.end = params.get("end")
+        self.usedVlans = params.get("usedVlans")
```

### Comparing `zenlayercloud-sdk-python-2.0.5/zenlayercloud/sdn/v20230830/sdn_client.py` & `zenlayercloud_sdk_python-2.0.7/zenlayercloud/sdn/v20230830/sdn_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,54 +25,49 @@
     def DescribeDataCenterPortPrice(self, request):
         response = self._api_call("DescribeDataCenterPortPrice", request)
 
         model = models.DescribeDataCenterPortPriceResponse()
         model._deserialize(response)
         return model
 
-
     def DescribePorts(self, request):
         response = self._api_call("DescribePorts", request)
 
         model = models.DescribePortsResponse()
         model._deserialize(response)
         return model
 
-
     def DescribePortTraffic(self, request):
         response = self._api_call("DescribePortTraffic", request)
 
         model = models.DescribePortTrafficResponse()
         model._deserialize(response)
         return model
 
-
     def DescribePortUsableVlan(self, request):
         response = self._api_call("DescribePortUsableVlan", request)
 
         model = models.DescribePortUsableVlanResponse()
         model._deserialize(response)
         return model
 
-
     def DestroyPort(self, request):
         response = self._api_call("DestroyPort", request)
 
         model = models.DestroyPortResponse()
         model._deserialize(response)
         return model
 
     def ModifyPortAttribute(self, request):
         response = self._api_call("ModifyPortAttribute", request)
 
         model = models.ModifyPortAttributeResponse()
         model._deserialize(response)
         return model
 
-
     def TerminatePort(self, request):
         response = self._api_call("TerminatePort", request)
 
         model = models.TerminatePortResponse()
         model._deserialize(response)
         return model
 
@@ -86,146 +81,140 @@
     def DescribePrivateConnects(self, request):
         response = self._api_call("DescribePrivateConnects", request)
 
         model = models.DescribePrivateConnectsResponse()
         model._deserialize(response)
         return model
 
-
     def DescribeCreatePrivateConnectAvailableSubnets(self, request):
         response = self._api_call("DescribeCreatePrivateConnectAvailableSubnets", request)
 
         model = models.DescribeCreatePrivateConnectAvailableSubnetsResponse()
         model._deserialize(response)
         return model
 
+    def DescribePrivateConnectAvailablePorts(self, request):
+        response = self._api_call("DescribePrivateConnectAvailablePorts", request)
+
+        model = models.DescribePrivateConnectAvailablePortsResponse()
+        model._deserialize(response)
+        return model
+
     def CreatePrivateConnect(self, request):
         response = self._api_call("CreatePrivateConnect", request)
 
         model = models.CreatePrivateConnectResponse()
         model._deserialize(response)
         return model
 
-
     def ModifyPrivateConnectsAttribute(self, request):
         response = self._api_call("ModifyPrivateConnectsAttribute", request)
 
         model = models.ModifyPrivateConnectsAttributeResponse()
         model._deserialize(response)
         return model
 
-
     def InquiryCreatePrivateConnectPrice(self, request):
         response = self._api_call("InquiryCreatePrivateConnectPrice", request)
 
         model = models.InquiryCreatePrivateConnectPriceResponse()
         model._deserialize(response)
         return model
 
-
     def DeletePrivateConnect(self, request):
         response = self._api_call("DeletePrivateConnect", request)
 
         model = models.DeletePrivateConnectResponse()
         model._deserialize(response)
         return model
 
-
     def DestroyPrivateConnect(self, request):
         response = self._api_call("DestroyPrivateConnect", request)
 
         model = models.DestroyPrivateConnectResponse()
         model._deserialize(response)
         return model
 
-
     def RenewPrivateConnect(self, request):
         response = self._api_call("RenewPrivateConnect", request)
 
         model = models.RenewPrivateConnectResponse()
         model._deserialize(response)
         return model
 
-
     def DescribePrivateConnectTraffic(self, request):
         response = self._api_call("DescribePrivateConnectTraffic", request)
 
         model = models.DescribePrivateConnectTrafficResponse()
         model._deserialize(response)
         return model
 
     def ModifyPrivateConnectBandwidth(self, request):
         response = self._api_call("ModifyPrivateConnectBandwidth", request)
 
         model = models.ModifyPrivateConnectBandwidthResponse()
         model._deserialize(response)
         return model
 
-
     def DescribeCloudRouters(self, request):
         response = self._api_call("DescribeCloudRouters", request)
 
         model = models.DescribeCloudRoutersResponse()
         model._deserialize(response)
         return model
 
     def DescribeCloudRouterAvailableVpcs(self, request):
         response = self._api_call("DescribeCloudRouterAvailableVpcs", request)
 
         model = models.DescribeCloudRouterAvailableVpcsResponse()
         model._deserialize(response)
         return model
 
-
     def DescribeCloudRouterAvailablePorts(self, request):
         response = self._api_call("DescribeCloudRouterAvailablePorts", request)
 
         model = models.DescribeCloudRouterAvailablePortsResponse()
         model._deserialize(response)
         return model
 
-
     def CreateCloudRouter(self, request):
         response = self._api_call("CreateCloudRouter", request)
 
         model = models.CreateCloudRouterResponse()
         model._deserialize(response)
         return model
 
-
     def ModifyCloudRoutersAttribute(self, request):
         response = self._api_call("ModifyCloudRoutersAttribute", request)
 
         model = models.ModifyCloudRoutersAttributeResponse()
         model._deserialize(response)
         return model
 
     def AddCloudRouterEdgePoints(self, request):
         response = self._api_call("AddCloudRouterEdgePoints", request)
 
         model = models.AddCloudRouterEdgePointsResponse()
         model._deserialize(response)
         return model
 
-
     def DeleteCloudRouterEdgePoint(self, request):
         response = self._api_call("DeleteCloudRouterEdgePoint", request)
 
         model = models.DeleteCloudRouterEdgePointResponse()
         model._deserialize(response)
         return model
 
     def DeleteCloudRouter(self, request):
         response = self._api_call("DeleteCloudRouter", request)
 
         model = models.DeleteCloudRouterResponse()
         model._deserialize(response)
         return model
 
-
     def DestroyCloudRouter(self, request):
         response = self._api_call("DestroyCloudRouter", request)
 
         model = models.DestroyCloudRouterResponse()
         model._deserialize(response)
         return model
 
@@ -239,21 +228,62 @@
     def ModifyCloudRouterEdgePointBandwidth(self, request):
         response = self._api_call("ModifyCloudRouterEdgePointBandwidth", request)
 
         model = models.ModifyCloudRouterEdgePointBandwidthResponse()
         model._deserialize(response)
         return model
 
-
     def DescribeCloudRouterEdgePointTraffic(self, request):
         response = self._api_call("DescribeCloudRouterEdgePointTraffic", request)
 
         model = models.DescribeCloudRouterEdgePointTrafficResponse()
         model._deserialize(response)
         return model
 
     def ModifyCloudRouterEdgePoint(self, request):
         response = self._api_call("ModifyCloudRouterEdgePoint", request)
 
         model = models.ModifyCloudRouterEdgePointResponse()
         model._deserialize(response)
         return model
+
+    def DescribeAWSRegions(self, request):
+        response = self._api_call("DescribeAWSRegions", request)
+
+        model = models.DescribeAWSRegionsResponse()
+        model._deserialize(response)
+        return model
+
+    def DescribeAWSVlanUsage(self, request):
+        response = self._api_call("DescribeAWSVlanUsage", request)
+
+        model = models.DescribeAWSVlanUsageResponse()
+        model._deserialize(response)
+        return model
+
+    def DescribeTencentRegions(self, request):
+        response = self._api_call("DescribeTencentRegions", request)
+
+        model = models.DescribeTencentRegionsResponse()
+        model._deserialize(response)
+        return model
+
+    def DescribeTencentVlanUsage(self, request):
+        response = self._api_call("DescribeTencentVlanUsage", request)
+
+        model = models.DescribeTencentVlanUsageResponse()
+        model._deserialize(response)
+        return model
+
+    def DescribeGoogleRegions(self, request):
+        response = self._api_call("DescribeGoogleRegions", request)
+
+        model = models.DescribeGoogleRegionsResponse()
+        model._deserialize(response)
+        return model
+
+    def DescribeGoogleVlanUsage(self, request):
+        response = self._api_call("DescribeGoogleVlanUsage", request)
+
+        model = models.DescribeGoogleVlanUsageResponse()
+        model._deserialize(response)
+        return model
```

### Comparing `zenlayercloud-sdk-python-2.0.5/zenlayercloud/vm/v20230313/models.py` & `zenlayercloud_sdk_python-2.0.7/zenlayercloud/vm/v20230313/models.py`

 * *Files identical despite different names*

### Comparing `zenlayercloud-sdk-python-2.0.5/zenlayercloud/vm/v20230313/vm_client.py` & `zenlayercloud_sdk_python-2.0.7/zenlayercloud/vm/v20230313/vm_client.py`

 * *Files identical despite different names*

### Comparing `zenlayercloud-sdk-python-2.0.5/zenlayercloud/zls/v20230804/models.py` & `zenlayercloud_sdk_python-2.0.7/zenlayercloud/zls/v20230804/models.py`

 * *Files identical despite different names*

### Comparing `zenlayercloud-sdk-python-2.0.5/zenlayercloud_sdk_python.egg-info/PKG-INFO` & `zenlayercloud_sdk_python-2.0.7/zenlayercloud_sdk_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenlayercloud-sdk-python
-Version: 2.0.5
+Version: 2.0.7
 Summary: Zenlayer Cloud SDK for Python
 Home-page: https://github.com/zenlayer/zenlayercloud-sdk-python
 Author: Zenlayer Cloud
 Maintainer-email: console_api@zenlayer.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
+Requires-Dist: requests>=2.27.0
 
 =============================
 Zenlayer Cloud SDK for Python
 =============================
 
 Zenlayer Cloud Python SDK is the official software development kit, which allows Python developers to write software that makes use of Zenlayer Cloud services like BMC and VM.
 
@@ -39,9 +40,7 @@
 or download source code from github and install:
 
 .. code-block:: sh
 
     $ git clone https://github.com/zenlayer/zenlayercloud-sdk-python.git
     $ cd zenlayercloud-sdk-python
     $ python setup.py install
-
-
```

### Comparing `zenlayercloud-sdk-python-2.0.5/zenlayercloud_sdk_python.egg-info/SOURCES.txt` & `zenlayercloud_sdk_python-2.0.7/zenlayercloud_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

