# Comparing `tmp/provena-interfaces-0.1.14.tar.gz` & `tmp/provena-interfaces-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "provena-interfaces-0.1.14.tar", last modified: Fri Apr 19 04:29:01 2024, max compression
+gzip compressed data, was "provena-interfaces-2.6.0.tar", last modified: Mon Apr 29 02:26:37 2024, max compression
```

## Comparing `provena-interfaces-0.1.14.tar` & `provena-interfaces-2.6.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:29:01.422510 provena-interfaces-0.1.14/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-19 04:29:01.422510 provena-interfaces-0.1.14/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:29:01.418510 provena-interfaces-0.1.14/ProvenaInterfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/APIResponses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/AsyncJobAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/AsyncJobModels.py
--rw-r--r--   0 runner    (1001) docker     (127)    17609 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/AuthAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/DataStoreAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/HandleAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/HandleModels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/ProvenanceAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/ProvenanceModels.py
--rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/RegistryAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)    64215 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/RegistryModels.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/SearchAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/SharedTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:29:01.418510 provena-interfaces-0.1.14/ProvenaInterfaces/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/helpers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/helpers/types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/ProvenaInterfaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:29:01.422510 provena-interfaces-0.1.14/provena_interfaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-19 04:29:01.000000 provena-interfaces-0.1.14/provena_interfaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-19 04:29:01.000000 provena-interfaces-0.1.14/provena_interfaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 04:29:01.000000 provena-interfaces-0.1.14/provena_interfaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 04:29:01.000000 provena-interfaces-0.1.14/provena_interfaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 04:29:01.000000 provena-interfaces-0.1.14/provena_interfaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 04:29:01.422510 provena-interfaces-0.1.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:29:01.422510 provena-interfaces-0.1.14/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/tests/test_registry_api_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-04-19 04:28:25.000000 provena-interfaces-0.1.14/tests/test_registry_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 02:26:37.218994 provena-interfaces-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-29 02:26:37.218994 provena-interfaces-2.6.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 02:26:37.214994 provena-interfaces-2.6.0/ProvenaInterfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/APIResponses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/AsyncJobAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/AsyncJobModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17609 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/AuthAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/DataStoreAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/HandleAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/HandleModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/ProvenanceAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/ProvenanceModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/RegistryAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64215 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/RegistryModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/SearchAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/SentryMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/SharedTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 02:26:37.214994 provena-interfaces-2.6.0/ProvenaInterfaces/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/helpers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/helpers/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/ProvenaInterfaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 02:26:37.218994 provena-interfaces-2.6.0/provena_interfaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-29 02:26:37.000000 provena-interfaces-2.6.0/provena_interfaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-29 02:26:37.000000 provena-interfaces-2.6.0/provena_interfaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 02:26:37.000000 provena-interfaces-2.6.0/provena_interfaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-29 02:26:37.000000 provena-interfaces-2.6.0/provena_interfaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 02:26:37.000000 provena-interfaces-2.6.0/provena_interfaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 02:26:37.218994 provena-interfaces-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 02:26:37.218994 provena-interfaces-2.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/tests/test_registry_api_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-04-29 02:25:56.000000 provena-interfaces-2.6.0/tests/test_registry_models.py
```

### Comparing `provena-interfaces-0.1.14/PKG-INFO` & `provena-interfaces-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: provena-interfaces
-Version: 0.1.14
+Version: 2.6.0
 Summary: Interfaces for Provena Application (see https://provena.io)
 Home-page: https://provena.io
 Maintainer-email: rrap-mds-is-support@csiro.au
 Description-Content-Type: text/markdown
 
 
 Provena-Interfaces is a Python package that provides interfaces for the Provena Application. It includes a set of interfaces that are used to interact with the Provena system. The interfaces are especially useful for parsing response payloads from the API, and for creating requests to the API. The interfaces will sit adjacent to (and be consumed by) a ProvenaClient library which is a work in progress.
```

### Comparing `provena-interfaces-0.1.14/ProvenaInterfaces/AsyncJobAPI.py` & `provena-interfaces-2.6.0/ProvenaInterfaces/AsyncJobAPI.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.14/ProvenaInterfaces/AsyncJobModels.py` & `provena-interfaces-2.6.0/ProvenaInterfaces/AsyncJobModels.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.14/ProvenaInterfaces/AuthAPI.py` & `provena-interfaces-2.6.0/ProvenaInterfaces/AuthAPI.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.14/ProvenaInterfaces/DataStoreAPI.py` & `provena-interfaces-2.6.0/ProvenaInterfaces/DataStoreAPI.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.14/ProvenaInterfaces/HandleAPI.py` & `provena-interfaces-2.6.0/ProvenaInterfaces/HandleAPI.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.14/ProvenaInterfaces/ProvenanceAPI.py` & `provena-interfaces-2.6.0/ProvenaInterfaces/ProvenanceAPI.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.14/ProvenaInterfaces/ProvenanceModels.py` & `provena-interfaces-2.6.0/ProvenaInterfaces/ProvenanceModels.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.14/ProvenaInterfaces/RegistryAPI.py` & `provena-interfaces-2.6.0/ProvenaInterfaces/RegistryAPI.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.14/ProvenaInterfaces/RegistryModels.py` & `provena-interfaces-2.6.0/ProvenaInterfaces/RegistryModels.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.14/ProvenaInterfaces/SearchAPI.py` & `provena-interfaces-2.6.0/ProvenaInterfaces/SearchAPI.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.14/ProvenaInterfaces/SharedTypes.py` & `provena-interfaces-2.6.0/ProvenaInterfaces/SharedTypes.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.14/ProvenaInterfaces/helpers/types.py` & `provena-interfaces-2.6.0/ProvenaInterfaces/helpers/types.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.14/README.md` & `provena-interfaces-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.14/provena_interfaces.egg-info/PKG-INFO` & `provena-interfaces-2.6.0/provena_interfaces.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: provena-interfaces
-Version: 0.1.14
+Version: 2.6.0
 Summary: Interfaces for Provena Application (see https://provena.io)
 Home-page: https://provena.io
 Maintainer-email: rrap-mds-is-support@csiro.au
 Description-Content-Type: text/markdown
 
 
 Provena-Interfaces is a Python package that provides interfaces for the Provena Application. It includes a set of interfaces that are used to interact with the Provena system. The interfaces are especially useful for parsing response payloads from the API, and for creating requests to the API. The interfaces will sit adjacent to (and be consumed by) a ProvenaClient library which is a work in progress.
```

### Comparing `provena-interfaces-0.1.14/provena_interfaces.egg-info/SOURCES.txt` & `provena-interfaces-2.6.0/provena_interfaces.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 ProvenaInterfaces/HandleAPI.py
 ProvenaInterfaces/HandleModels.py
 ProvenaInterfaces/ProvenanceAPI.py
 ProvenaInterfaces/ProvenanceModels.py
 ProvenaInterfaces/RegistryAPI.py
 ProvenaInterfaces/RegistryModels.py
 ProvenaInterfaces/SearchAPI.py
+ProvenaInterfaces/SentryMonitoring.py
 ProvenaInterfaces/SharedTypes.py
 ProvenaInterfaces/__init__.py
 ProvenaInterfaces/py.typed
 ProvenaInterfaces/helpers/__init__.py
 ProvenaInterfaces/helpers/helpers.py
 ProvenaInterfaces/helpers/types.py
 provena_interfaces.egg-info/PKG-INFO
```

### Comparing `provena-interfaces-0.1.14/setup.py` & `provena-interfaces-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.14/tests/test_registry_api_models.py` & `provena-interfaces-2.6.0/tests/test_registry_api_models.py`

 * *Files identical despite different names*

### Comparing `provena-interfaces-0.1.14/tests/test_registry_models.py` & `provena-interfaces-2.6.0/tests/test_registry_models.py`

 * *Files identical despite different names*

