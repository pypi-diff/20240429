# Comparing `tmp/PyPowerStore-3.1.0.0.tar.gz` & `tmp/PyPowerStore-3.2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyPowerStore-3.1.0.0.tar", last modified: Thu Feb 29 09:31:24 2024, max compression
+gzip compressed data, was "dist/PyPowerStore-3.2.0.0.tar", last modified: Mon Apr 29 12:11:23 2024, max compression
```

## Comparing `PyPowerStore-3.1.0.0.tar` & `PyPowerStore-3.2.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 09:31:24.000000 PyPowerStore-3.1.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 09:31:24.000000 PyPowerStore-3.1.0.0/PyPowerStore/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 09:31:24.000000 PyPowerStore-3.1.0.0/PyPowerStore/objects/
--rw-r--r--   0 root         (0) root         (0)      991 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/objects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5629 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/objects/file_dns.py
--rw-r--r--   0 root         (0) root         (0)     6357 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/objects/file_interface.py
--rw-r--r--   0 root         (0) root         (0)     5666 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/objects/file_nis.py
--rw-r--r--   0 root         (0) root         (0)     6005 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/objects/nfs_server.py
--rw-r--r--   0 root         (0) root         (0)     5882 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/objects/smb_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 09:31:24.000000 PyPowerStore-3.1.0.0/PyPowerStore/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37205 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/utils/constants.py
--rw-r--r--   0 root         (0) root         (0)      584 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/utils/exception.py
--rw-r--r--   0 root         (0) root         (0)     6934 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/utils/helpers.py
--rw-r--r--   0 root         (0) root         (0)      240 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16271 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/client.py
--rw-r--r--   0 root         (0) root         (0)    96987 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/configuration.py
--rw-r--r--   0 root         (0) root         (0)     2739 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/powerstore_conn.py
--rw-r--r--   0 root         (0) root         (0)    61608 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/protection.py
--rw-r--r--   0 root         (0) root         (0)   104905 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/PyPowerStore/provisioning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 09:31:24.000000 PyPowerStore-3.1.0.0/PyPowerStore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      339 2024-02-29 09:31:22.000000 PyPowerStore-3.1.0.0/PyPowerStore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      696 2024-02-29 09:31:23.000000 PyPowerStore-3.1.0.0/PyPowerStore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-29 09:31:22.000000 PyPowerStore-3.1.0.0/PyPowerStore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-02-29 09:31:22.000000 PyPowerStore-3.1.0.0/PyPowerStore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-02-29 09:31:22.000000 PyPowerStore-3.1.0.0/PyPowerStore.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1749 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)      729 2024-02-29 09:31:19.000000 PyPowerStore-3.1.0.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      339 2024-02-29 09:31:24.000000 PyPowerStore-3.1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-29 09:31:24.000000 PyPowerStore-3.1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/objects/
+-rw-r--r--   0 root         (0) root         (0)      991 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5629 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/objects/file_dns.py
+-rw-r--r--   0 root         (0) root         (0)     6357 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/objects/file_interface.py
+-rw-r--r--   0 root         (0) root         (0)     5666 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/objects/file_nis.py
+-rw-r--r--   0 root         (0) root         (0)     6005 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/objects/nfs_server.py
+-rw-r--r--   0 root         (0) root         (0)     5882 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/objects/smb_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37909 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/utils/constants.py
+-rw-r--r--   0 root         (0) root         (0)      584 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/utils/exception.py
+-rw-r--r--   0 root         (0) root         (0)     7269 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/utils/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      240 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16271 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/client.py
+-rw-r--r--   0 root         (0) root         (0)    96987 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/powerstore_conn.py
+-rw-r--r--   0 root         (0) root         (0)    61608 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/protection.py
+-rw-r--r--   0 root         (0) root         (0)   105129 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore/provisioning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      339 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      696 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PyPowerStore.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      729 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      339 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 12:11:23.000000 PyPowerStore-3.2.0.0/setup.cfg
```

### Comparing `PyPowerStore-3.1.0.0/PyPowerStore/objects/__init__.py` & `PyPowerStore-3.2.0.0/PyPowerStore/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.1.0.0/PyPowerStore/objects/file_dns.py` & `PyPowerStore-3.2.0.0/PyPowerStore/objects/file_dns.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.1.0.0/PyPowerStore/objects/file_interface.py` & `PyPowerStore-3.2.0.0/PyPowerStore/objects/file_interface.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.1.0.0/PyPowerStore/objects/file_nis.py` & `PyPowerStore-3.2.0.0/PyPowerStore/objects/file_nis.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.1.0.0/PyPowerStore/objects/nfs_server.py` & `PyPowerStore-3.2.0.0/PyPowerStore/objects/nfs_server.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.1.0.0/PyPowerStore/objects/smb_server.py` & `PyPowerStore-3.2.0.0/PyPowerStore/objects/smb_server.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.1.0.0/PyPowerStore/utils/constants.py` & `PyPowerStore-3.2.0.0/PyPowerStore/utils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,20 @@
 # Pagination Constants
 # offset is 0 and limit is 99 for first request
 # offset for second request
 OFFSET = 100
 # max number of items limit in a response
 MAX_LIMIT = 2000
 
-# Foot Hill Prime Plus Version
+# Platform Versions
+FOOTHILL_VERSION = '2.0.0.0'
+MALKA_VERSION = '2.1.0.0'
+FOOTHILL_PRIME_VERSION = '3.0.0.0'
 FOOTHILL_PRIME_PLUS_VERSION = '3.2.0.0'
+VICTORY_VERSION = '4.0.0.0'
 
 # Query params
 
 # Volume Query
 SELECT_ALL_VOLUME = {"select": "id,name,description,type,wwn,appliance_id,"
                                "state,size,creation_timestamp,"
                                "protection_policy_id,performance_policy_id,"
@@ -60,14 +64,24 @@
               "host_group(name,id),volume_groups(name,id),"
               "mapped_volumes(id,logical_unit_number),nsid,nguid,"
               "node_affinity,node_affinity_l10n,metro_replication_session_id,"
               "is_host_access_available,app_type,app_type_other,app_type_l10n,"
               "migration_session_id"
 }
 
+VICTORY_VOLUME_DETAILS_QUERY = {
+    "select": "id,name,description,type,wwn,nsid,nguid,appliance_id,state,"
+              "size,logical_used,node_affinity,creation_timestamp,"
+              "protection_policy_id,performance_policy_id,qos_performance_policy_id,"
+              "is_replication_destination,migration_session_id,metro_replication_session_id,"
+              "is_host_access_available,protection_data,location_history,"
+              "app_type,app_type_other,type_l10n,state_l10n,node_affinity_l10n,app_type_l10n,"
+              "volume_groups(name,id), protection_policy(name,id)"
+}
+
 # Host Query
 SELECT_ALL_HOST = {
     "select": "id,name,description,os_type,"
               "host_group_id,"
               "host_initiators,os_type_l10n,"
               "mapped_hosts(id,logical_unit_number,"
               "host_group(id,name),volume(id,name)),"
```

### Comparing `PyPowerStore-3.1.0.0/PyPowerStore/utils/exception.py` & `PyPowerStore-3.2.0.0/PyPowerStore/utils/exception.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.1.0.0/PyPowerStore/utils/helpers.py` & `PyPowerStore-3.2.0.0/PyPowerStore/utils/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
-# Copyright: (c) 2019, Dell Technologies
+# Copyright: (c) 2024, Dell Technologies
 
 """Helper module for PowerStore"""
 import logging
 from pkg_resources import parse_version
+from PyPowerStore.utils import constants
 
 provisioning_obj = None
 
 
 def set_provisioning_obj(val):
     global provisioning_obj
     provisioning_obj = val
@@ -48,44 +49,53 @@
 
 def is_foot_hill_or_higher():
     """Returns true if the array version is foot hill or higher.
 
     :return: True if foot hill or higher
     :rtype: bool
     """
-    foot_hill_version = '2.0.0.0'
     array_version = provisioning_obj.get_array_version()
     if array_version and (
-            parse_version(array_version[0:7]) >= parse_version(foot_hill_version)):
+            parse_version(array_version[0:7]) >= parse_version(constants.FOOTHILL_VERSION)):
         return True
     return False
 
 def is_malka_or_higher():
     """Returns true if the array version is Malka or higher.
 
     :return: True if array version is Malka or higher
     :rtype: bool
     """
-    malka_version = '2.1.0.0'
     array_version = provisioning_obj.get_array_version()
     if array_version and (
-            parse_version(array_version[0:7]) >= parse_version(malka_version)):
+            parse_version(array_version[0:7]) >= parse_version(constants.MALKA_VERSION)):
         return True
     return False
 
 def is_foot_hill_prime_or_higher():
     """Returns true if the array version is foothill prime or higher.
 
     :return: True if foothill prime or higher
     :rtype: bool
     """
-    foot_hill_prime_version = '3.0.0.0'
     array_version = provisioning_obj.get_array_version()
     if array_version and (
-            parse_version(array_version[0:7]) >= parse_version(foot_hill_prime_version)):
+            parse_version(array_version[0:7]) >= parse_version(constants.FOOTHILL_PRIME_VERSION)):
+        return True
+    return False
+
+def is_victory_or_higher():
+    """Returns true if the array version is victory or higher.
+
+    :return: True if victory or higher
+    :rtype: bool
+    """
+    array_version = provisioning_obj.get_array_version()
+    if array_version and (
+            parse_version(array_version[0:7]) >= parse_version(constants.VICTORY_VERSION)):
         return True
     return False
 
 
 def filtered_details(filterable_keys, filter_dict, resource_list,
                      resource_name):
     """
```

### Comparing `PyPowerStore-3.1.0.0/PyPowerStore/client.py` & `PyPowerStore-3.2.0.0/PyPowerStore/client.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.1.0.0/PyPowerStore/configuration.py` & `PyPowerStore-3.2.0.0/PyPowerStore/configuration.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.1.0.0/PyPowerStore/powerstore_conn.py` & `PyPowerStore-3.2.0.0/PyPowerStore/powerstore_conn.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.1.0.0/PyPowerStore/protection.py` & `PyPowerStore-3.2.0.0/PyPowerStore/protection.py`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.1.0.0/PyPowerStore/provisioning.py` & `PyPowerStore-3.2.0.0/PyPowerStore/provisioning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright: (c) 2019, Dell Technologies
+# Copyright: (c) 2024, Dell Technologies
 
 """Collection of provisioning related functions for PowerStore"""
 
 from PyPowerStore.client import Client
 from PyPowerStore.utils import constants, helpers
 
 # TODO: kept LOG as global for now will improve it to avoid overriding
@@ -638,15 +638,17 @@
         :param volume_id: The volume ID
         :type volume_id: str
         :return: Volume details
         :rtype: dict
         """
         LOG.info("Getting volume details by ID: '%s'" % volume_id)
         querystring = constants.SELECT_ALL_VOLUME
-        if helpers.is_foot_hill_prime_or_higher():
+        if helpers.is_victory_or_higher():
+            querystring = constants.VICTORY_VOLUME_DETAILS_QUERY
+        elif helpers.is_foot_hill_prime_or_higher():
             querystring = constants.FHP_VOLUME_DETAILS_QUERY
         elif helpers.is_foot_hill_or_higher():
             querystring = constants.FHC_VOLUME_DETAILS_QUERY
 
         resp = self.client.request(constants.GET,
                                    constants.GET_VOLUME_DETAILS_URL.format
                                    (self.server_ip, volume_id), payload=None,
@@ -664,15 +666,17 @@
         :param volume_name: The volume name
         :type volume_name: str
         :return: Volume details
         :rtype: dict
         """
         LOG.info("Getting volume details by name: '%s'" % volume_name)
         querystring = constants.SELECT_ALL_VOLUME
-        if helpers.is_foot_hill_prime_or_higher():
+        if helpers.is_victory_or_higher():
+            querystring = constants.VICTORY_VOLUME_DETAILS_QUERY
+        elif helpers.is_foot_hill_prime_or_higher():
             querystring = constants.FHP_VOLUME_DETAILS_QUERY
         elif helpers.is_foot_hill_or_higher():
             querystring = constants.FHC_VOLUME_DETAILS_QUERY
 
         resp = self.client.request(
             constants.GET,
             constants.GET_VOLUME_BY_NAME_URL.format(self.server_ip),
```

### Comparing `PyPowerStore-3.1.0.0/PyPowerStore.egg-info/SOURCES.txt` & `PyPowerStore-3.2.0.0/PyPowerStore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.1.0.0/README.md` & `PyPowerStore-3.2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `PyPowerStore-3.1.0.0/setup.py` & `PyPowerStore-3.2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 
 setup(name='PyPowerStore',
-      version='3.1.0.0',
+      version='3.2.0.0',
       description='Python Library for Dell PowerStore',
       author='Ansible Team at Dell',
       author_email='ansible.team@dell.com',
       install_requires=[
         'urllib3>=1.26.7',
         'requests>=2.23.0'
       ],
```

