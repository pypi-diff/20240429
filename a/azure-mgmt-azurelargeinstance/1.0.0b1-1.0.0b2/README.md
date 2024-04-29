# Comparing `tmp/azure-mgmt-azurelargeinstance-1.0.0b1.tar.gz` & `tmp/azure-mgmt-azurelargeinstance-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-mgmt-azurelargeinstance-1.0.0b1.tar", last modified: Mon Mar  4 02:48:26 2024, max compression
+gzip compressed data, was "azure-mgmt-azurelargeinstance-1.0.0b2.tar", last modified: Mon Apr 29 02:05:26 2024, max compression
```

## Comparing `azure-mgmt-azurelargeinstance-1.0.0b1.tar` & `azure-mgmt-azurelargeinstance-1.0.0b2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-04 02:48:26.902700 azure-mgmt-azurelargeinstance-1.0.0b1/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       62 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      224 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/MANIFEST.in
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     3140 2024-03-04 02:48:26.902700 azure-mgmt-azurelargeinstance-1.0.0b1/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2051 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      644 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/_meta.json
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-04 02:48:26.894700 azure-mgmt-azurelargeinstance-1.0.0b1/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-04 02:48:26.894700 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-04 02:48:26.894700 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      910 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3543 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4857 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/_large_instance_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    79289 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-04 02:48:26.894700 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      857 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3591 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5001 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/_large_instance_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-04 02:48:26.898700 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1005 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    45396 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/operations/_azure_large_instance_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20743 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/operations/_azure_large_storage_instance_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5796 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-04 02:48:26.898700 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3663 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11911 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/models/_large_instance_mgmt_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48217 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-04 02:48:26.898700 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1005 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    54881 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/operations/_azure_large_instance_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26087 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/operations/_azure_large_storage_instance_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6505 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-04 02:48:26.898700 azure-mgmt-azurelargeinstance-1.0.0b1/azure_mgmt_azurelargeinstance.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     3140 2024-03-04 02:48:26.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure_mgmt_azurelargeinstance.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1873 2024-03-04 02:48:26.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure_mgmt_azurelargeinstance.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-04 02:48:26.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure_mgmt_azurelargeinstance.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-04 02:48:26.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure_mgmt_azurelargeinstance.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       70 2024-03-04 02:48:26.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure_mgmt_azurelargeinstance.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-03-04 02:48:26.000000 azure-mgmt-azurelargeinstance-1.0.0b1/azure_mgmt_azurelargeinstance.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-03-04 02:48:26.902700 azure-mgmt-azurelargeinstance-1.0.0b1/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2803 2024-03-04 02:47:36.000000 azure-mgmt-azurelargeinstance-1.0.0b1/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-29 02:05:26.308921 azure-mgmt-azurelargeinstance-1.0.0b2/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      285 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      224 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1410 2024-04-29 02:05:26.308921 azure-mgmt-azurelargeinstance-1.0.0b2/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      209 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      644 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/_meta.json
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-29 02:05:26.300921 azure-mgmt-azurelargeinstance-1.0.0b2/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-29 02:05:26.300921 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-29 02:05:26.300921 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      910 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3543 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4857 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/_large_instance_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    79289 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-29 02:05:26.304921 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      857 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3591 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5001 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/_large_instance_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-29 02:05:26.304921 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1005 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    45396 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/operations/_azure_large_instance_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20743 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/operations/_azure_large_storage_instance_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5796 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-29 02:05:26.304921 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3663 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11911 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/models/_large_instance_mgmt_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48217 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-29 02:05:26.304921 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1005 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    54881 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/operations/_azure_large_instance_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26087 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/operations/_azure_large_storage_instance_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6505 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-29 02:05:26.308921 azure-mgmt-azurelargeinstance-1.0.0b2/azure_mgmt_azurelargeinstance.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1410 2024-04-29 02:05:26.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure_mgmt_azurelargeinstance.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1888 2024-04-29 02:05:26.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure_mgmt_azurelargeinstance.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-29 02:05:26.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure_mgmt_azurelargeinstance.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-29 02:05:26.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure_mgmt_azurelargeinstance.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       70 2024-04-29 02:05:26.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure_mgmt_azurelargeinstance.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-29 02:05:26.000000 azure-mgmt-azurelargeinstance-1.0.0b2/azure_mgmt_azurelargeinstance.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       44 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/pyproject.toml
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-29 02:05:26.308921 azure-mgmt-azurelargeinstance-1.0.0b2/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2807 2024-04-29 02:03:50.000000 azure-mgmt-azurelargeinstance-1.0.0b2/setup.py
```

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/LICENSE` & `azure-mgmt-azurelargeinstance-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/_meta.json` & `azure-mgmt-azurelargeinstance-1.0.0b2/_meta.json`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/__init__.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/_configuration.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/_large_instance_mgmt_client.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/_large_instance_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/_patch.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/_serialization.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/_vendor.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/__init__.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/_configuration.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/_large_instance_mgmt_client.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/_large_instance_mgmt_client.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/_patch.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/operations/__init__.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/operations/_azure_large_instance_operations.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/operations/_azure_large_instance_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/operations/_azure_large_storage_instance_operations.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/operations/_azure_large_storage_instance_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/operations/_operations.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/aio/operations/_patch.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/models/__init__.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/models/_large_instance_mgmt_client_enums.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/models/_large_instance_mgmt_client_enums.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/models/_models_py3.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/models/_models_py3.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/models/_patch.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/operations/__init__.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/operations/_azure_large_instance_operations.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/operations/_azure_large_instance_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/operations/_azure_large_storage_instance_operations.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/operations/_azure_large_storage_instance_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/operations/_operations.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure/mgmt/azurelargeinstance/operations/_patch.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure/mgmt/azurelargeinstance/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/azure_mgmt_azurelargeinstance.egg-info/SOURCES.txt` & `azure-mgmt-azurelargeinstance-1.0.0b2/azure_mgmt_azurelargeinstance.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 _meta.json
+pyproject.toml
 setup.py
 azure/__init__.py
 azure/mgmt/__init__.py
 azure/mgmt/azurelargeinstance/__init__.py
 azure/mgmt/azurelargeinstance/_configuration.py
 azure/mgmt/azurelargeinstance/_large_instance_mgmt_client.py
 azure/mgmt/azurelargeinstance/_patch.py
```

### Comparing `azure-mgmt-azurelargeinstance-1.0.0b1/setup.py` & `azure-mgmt-azurelargeinstance-1.0.0b2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     long_description_content_type="text/markdown",
     license="MIT License",
     author="Microsoft Corporation",
     author_email="azpysdkhelp@microsoft.com",
     url="https://github.com/Azure/azure-sdk-for-python",
     keywords="azure, azure sdk",  # update with search keywords relevant to the azure service / product
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 7 - Inactive",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

