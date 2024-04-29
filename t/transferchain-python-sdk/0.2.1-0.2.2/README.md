# Comparing `tmp/transferchain-python-sdk-0.2.1.tar.gz` & `tmp/transferchain-python-sdk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transferchain-python-sdk-0.2.1.tar", last modified: Wed Feb 21 21:14:49 2024, max compression
+gzip compressed data, was "transferchain-python-sdk-0.2.2.tar", last modified: Mon Apr 29 14:53:45 2024, max compression
```

## Comparing `transferchain-python-sdk-0.2.1.tar` & `transferchain-python-sdk-0.2.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 ghroo2    (1000) ghroo-2   (1000)        0 2024-02-21 21:14:49.979608 transferchain-python-sdk-0.2.1/
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1073 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/LICENSE
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     3545 2024-02-21 21:14:49.979608 transferchain-python-sdk-0.2.1/PKG-INFO
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     3193 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/README.md
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)       38 2024-02-21 21:14:49.979608 transferchain-python-sdk-0.2.1/setup.cfg
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      799 2024-02-21 21:14:43.000000 transferchain-python-sdk-0.2.1/setup.py
-drwxr-xr-x   0 ghroo2    (1000) ghroo-2   (1000)        0 2024-02-21 21:14:49.975608 transferchain-python-sdk-0.2.1/tests/
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)        0 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/__init__.py
-drwxr-xr-x   0 ghroo2    (1000) ghroo-2   (1000)        0 2024-02-21 21:14:49.975608 transferchain-python-sdk-0.2.1/tests/crypt/
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)        0 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/crypt/__init__.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1039 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/crypt/test_address.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      748 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/crypt/test_bip39.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     2294 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/crypt/test_crypt.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1171 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/crypt/test_keys.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1585 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/test_addresses.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      966 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/test_blockchain.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     6411 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/test_client.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      511 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/test_config.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      530 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/test_db.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      332 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/test_grpc_client.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     3547 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/test_restore.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     3756 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/test_storage.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     6941 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/test_transfer.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      758 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/tests/test_utils.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1617 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.1/tests/test_wallet.py
-drwxr-xr-x   0 ghroo2    (1000) ghroo-2   (1000)        0 2024-02-21 21:14:49.979608 transferchain-python-sdk-0.2.1/transferchain/
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     2073 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.1/transferchain/__init__.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     6642 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/addresses.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1581 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/blockchain.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1784 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/cert.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    19901 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/client.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     2680 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.1/transferchain/config.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      742 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/constants.py
-drwxr-xr-x   0 ghroo2    (1000) ghroo-2   (1000)        0 2024-02-21 21:14:49.979608 transferchain-python-sdk-0.2.1/transferchain/crypt/
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)       85 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/crypt/__init__.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     2391 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/crypt/address.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     2514 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/crypt/bip39.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    15124 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/crypt/crypt.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     7569 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/crypt/keys.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    19465 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/crypt/words.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     4357 2023-11-21 12:47:20.000000 transferchain-python-sdk-0.2.1/transferchain/datastructures.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      791 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/db.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)       81 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/exceptions.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      626 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.1/transferchain/grpc_client.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      350 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/logger.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      617 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/mixins.py
-drwxr-xr-x   0 ghroo2    (1000) ghroo-2   (1000)        0 2024-02-21 21:14:49.979608 transferchain-python-sdk-0.2.1/transferchain/protobuf/
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)        0 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/protobuf/__init__.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    30448 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.1/transferchain/protobuf/service_pb2.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    63296 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.1/transferchain/protobuf/service_pb2_grpc.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    12266 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/restore.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      921 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.1/transferchain/settings.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    22444 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/storage.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     2676 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/transaction.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    28372 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/transfer.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1481 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.1/transferchain/utils.py
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     3670 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.1/transferchain/wallet.py
-drwxr-xr-x   0 ghroo2    (1000) ghroo-2   (1000)        0 2024-02-21 21:14:49.979608 transferchain-python-sdk-0.2.1/transferchain_python_sdk.egg-info/
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     3545 2024-02-21 21:14:49.000000 transferchain-python-sdk-0.2.1/transferchain_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1461 2024-02-21 21:14:49.000000 transferchain-python-sdk-0.2.1/transferchain_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)        1 2024-02-21 21:14:49.000000 transferchain-python-sdk-0.2.1/transferchain_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      164 2024-02-21 21:14:49.000000 transferchain-python-sdk-0.2.1/transferchain_python_sdk.egg-info/requires.txt
--rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)       20 2024-02-21 21:14:49.000000 transferchain-python-sdk-0.2.1/transferchain_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 ghroo2    (1000) ghroo-2   (1000)        0 2024-04-29 14:53:45.325987 transferchain-python-sdk-0.2.2/
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1073 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/LICENSE
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     3545 2024-04-29 14:53:45.325987 transferchain-python-sdk-0.2.2/PKG-INFO
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     3193 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/README.md
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)       38 2024-04-29 14:53:45.325987 transferchain-python-sdk-0.2.2/setup.cfg
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      799 2024-04-29 14:53:00.000000 transferchain-python-sdk-0.2.2/setup.py
+drwxr-xr-x   0 ghroo2    (1000) ghroo-2   (1000)        0 2024-04-29 14:53:45.325987 transferchain-python-sdk-0.2.2/tests/
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)        0 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/__init__.py
+drwxr-xr-x   0 ghroo2    (1000) ghroo-2   (1000)        0 2024-04-29 14:53:45.325987 transferchain-python-sdk-0.2.2/tests/crypt/
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)        0 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/crypt/__init__.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1039 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/crypt/test_address.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      748 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/crypt/test_bip39.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     2294 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/crypt/test_crypt.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1171 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/crypt/test_keys.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1585 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/test_addresses.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      966 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/test_blockchain.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     6411 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/test_client.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      511 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/test_config.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      530 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/test_db.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      332 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/test_grpc_client.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     3547 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/test_restore.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     3756 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/test_storage.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     6941 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/test_transfer.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      758 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/tests/test_utils.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1617 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.2/tests/test_wallet.py
+drwxr-xr-x   0 ghroo2    (1000) ghroo-2   (1000)        0 2024-04-29 14:53:45.325987 transferchain-python-sdk-0.2.2/transferchain/
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     2073 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.2/transferchain/__init__.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     6642 2024-04-29 14:53:00.000000 transferchain-python-sdk-0.2.2/transferchain/addresses.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1581 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/blockchain.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1784 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/cert.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    19901 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/client.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     2680 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.2/transferchain/config.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      742 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/constants.py
+drwxr-xr-x   0 ghroo2    (1000) ghroo-2   (1000)        0 2024-04-29 14:53:45.325987 transferchain-python-sdk-0.2.2/transferchain/crypt/
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)       85 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/crypt/__init__.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     2391 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/crypt/address.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     2514 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/crypt/bip39.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    15124 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/crypt/crypt.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     7569 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/crypt/keys.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    19465 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/crypt/words.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     4357 2023-11-21 12:47:20.000000 transferchain-python-sdk-0.2.2/transferchain/datastructures.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      791 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/db.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)       81 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/exceptions.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      626 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.2/transferchain/grpc_client.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      350 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/logger.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      617 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/mixins.py
+drwxr-xr-x   0 ghroo2    (1000) ghroo-2   (1000)        0 2024-04-29 14:53:45.325987 transferchain-python-sdk-0.2.2/transferchain/protobuf/
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)        0 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/protobuf/__init__.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    30448 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.2/transferchain/protobuf/service_pb2.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    63296 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.2/transferchain/protobuf/service_pb2_grpc.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    12266 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/restore.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      921 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.2/transferchain/settings.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    22444 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/storage.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     2676 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/transaction.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)    28372 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/transfer.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1481 2023-11-20 11:08:23.000000 transferchain-python-sdk-0.2.2/transferchain/utils.py
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     3670 2024-01-18 12:38:20.000000 transferchain-python-sdk-0.2.2/transferchain/wallet.py
+drwxr-xr-x   0 ghroo2    (1000) ghroo-2   (1000)        0 2024-04-29 14:53:45.325987 transferchain-python-sdk-0.2.2/transferchain_python_sdk.egg-info/
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     3545 2024-04-29 14:53:45.000000 transferchain-python-sdk-0.2.2/transferchain_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)     1461 2024-04-29 14:53:45.000000 transferchain-python-sdk-0.2.2/transferchain_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)        1 2024-04-29 14:53:45.000000 transferchain-python-sdk-0.2.2/transferchain_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)      164 2024-04-29 14:53:45.000000 transferchain-python-sdk-0.2.2/transferchain_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 ghroo2    (1000) ghroo-2   (1000)       20 2024-04-29 14:53:45.000000 transferchain-python-sdk-0.2.2/transferchain_python_sdk.egg-info/top_level.txt
```

### Comparing `transferchain-python-sdk-0.2.1/LICENSE` & `transferchain-python-sdk-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/PKG-INFO` & `transferchain-python-sdk-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transferchain-python-sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: TransferChain Python SDK
 Home-page: https://github.com/TransferChain/transferchain-python-sdk
 Author: TransferChain
 Author-email: info@transferchain.io
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `transferchain-python-sdk-0.2.1/README.md` & `transferchain-python-sdk-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/setup.py` & `transferchain-python-sdk-0.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     'grpcio==1.59.0',
     'grpcio-tools==1.59.0',
     'tcabci-read-client'
 ]
 
 setup(
     name="transferchain-python-sdk",
-    version="0.2.1",
+    version="0.2.2",
     author="TransferChain",
     author_email="info@transferchain.io",
     description="TransferChain Python SDK",
     long_description=page_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TransferChain/transferchain-python-sdk",
     packages=find_packages(),
```

### Comparing `transferchain-python-sdk-0.2.1/tests/crypt/test_address.py` & `transferchain-python-sdk-0.2.2/tests/crypt/test_address.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/tests/crypt/test_bip39.py` & `transferchain-python-sdk-0.2.2/tests/crypt/test_bip39.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/tests/crypt/test_crypt.py` & `transferchain-python-sdk-0.2.2/tests/crypt/test_crypt.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/tests/crypt/test_keys.py` & `transferchain-python-sdk-0.2.2/tests/crypt/test_keys.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/tests/test_addresses.py` & `transferchain-python-sdk-0.2.2/tests/test_addresses.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/tests/test_blockchain.py` & `transferchain-python-sdk-0.2.2/tests/test_blockchain.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/tests/test_client.py` & `transferchain-python-sdk-0.2.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/tests/test_db.py` & `transferchain-python-sdk-0.2.2/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/tests/test_restore.py` & `transferchain-python-sdk-0.2.2/tests/test_restore.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/tests/test_storage.py` & `transferchain-python-sdk-0.2.2/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/tests/test_transfer.py` & `transferchain-python-sdk-0.2.2/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/tests/test_utils.py` & `transferchain-python-sdk-0.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/tests/test_wallet.py` & `transferchain-python-sdk-0.2.2/tests/test_wallet.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/__init__.py` & `transferchain-python-sdk-0.2.2/transferchain/__init__.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/addresses.py` & `transferchain-python-sdk-0.2.2/transferchain/addresses.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     result = blockchain.broadcast(tx)
     if result.success is False:
         return Result(
             success=False,
             error_message='The master address is not published on the blockchain.') # noqa
 
     addresses_payload = []
-    for i in range(0, 250):
+    for i in range(0, 100):
         user_pass = "{}-{}".format(
             get_user_password(user_id, sub_user_id), i)
         user_sub_keys = keys.create_keys_with_mnemonic(mnemonics, user_pass)
         address = Address(
             Master=False,
             Key=user_sub_keys,
             UserID=user_id,
@@ -181,15 +181,15 @@
     if result.success is False:
         return Result(
             success=False,
             error_message='The master address is not published on the blockchain.') # noqa
 
     addresses_payload = []
 
-    for i in range(0, 250):
+    for i in range(0, 100):
         user_pass = "{}-{}".format(get_user_password(user_id), i)
         user_sub_keys = keys.create_keys_with_mnemonic(mnemonics, user_pass)
         address = Address(
             Master=False,
             Key=user_sub_keys,
             UserID=user_id,
             Mnemonics=mnemonics,
```

### Comparing `transferchain-python-sdk-0.2.1/transferchain/blockchain.py` & `transferchain-python-sdk-0.2.2/transferchain/blockchain.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/cert.py` & `transferchain-python-sdk-0.2.2/transferchain/cert.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/client.py` & `transferchain-python-sdk-0.2.2/transferchain/client.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/config.py` & `transferchain-python-sdk-0.2.2/transferchain/config.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/constants.py` & `transferchain-python-sdk-0.2.2/transferchain/constants.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/crypt/address.py` & `transferchain-python-sdk-0.2.2/transferchain/crypt/address.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/crypt/bip39.py` & `transferchain-python-sdk-0.2.2/transferchain/crypt/bip39.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/crypt/crypt.py` & `transferchain-python-sdk-0.2.2/transferchain/crypt/crypt.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/crypt/keys.py` & `transferchain-python-sdk-0.2.2/transferchain/crypt/keys.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/crypt/words.py` & `transferchain-python-sdk-0.2.2/transferchain/crypt/words.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/datastructures.py` & `transferchain-python-sdk-0.2.2/transferchain/datastructures.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/db.py` & `transferchain-python-sdk-0.2.2/transferchain/db.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/grpc_client.py` & `transferchain-python-sdk-0.2.2/transferchain/grpc_client.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/mixins.py` & `transferchain-python-sdk-0.2.2/transferchain/mixins.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/protobuf/service_pb2.py` & `transferchain-python-sdk-0.2.2/transferchain/protobuf/service_pb2.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/protobuf/service_pb2_grpc.py` & `transferchain-python-sdk-0.2.2/transferchain/protobuf/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/restore.py` & `transferchain-python-sdk-0.2.2/transferchain/restore.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/settings.py` & `transferchain-python-sdk-0.2.2/transferchain/settings.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/storage.py` & `transferchain-python-sdk-0.2.2/transferchain/storage.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/transaction.py` & `transferchain-python-sdk-0.2.2/transferchain/transaction.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/transfer.py` & `transferchain-python-sdk-0.2.2/transferchain/transfer.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/utils.py` & `transferchain-python-sdk-0.2.2/transferchain/utils.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain/wallet.py` & `transferchain-python-sdk-0.2.2/transferchain/wallet.py`

 * *Files identical despite different names*

### Comparing `transferchain-python-sdk-0.2.1/transferchain_python_sdk.egg-info/PKG-INFO` & `transferchain-python-sdk-0.2.2/transferchain_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transferchain-python-sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: TransferChain Python SDK
 Home-page: https://github.com/TransferChain/transferchain-python-sdk
 Author: TransferChain
 Author-email: info@transferchain.io
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `transferchain-python-sdk-0.2.1/transferchain_python_sdk.egg-info/SOURCES.txt` & `transferchain-python-sdk-0.2.2/transferchain_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

