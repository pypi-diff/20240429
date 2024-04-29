# Comparing `tmp/climb_onyx_client-4.3.0.tar.gz` & `tmp/climb_onyx_client-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climb_onyx_client-4.3.0.tar", last modified: Wed Apr 24 15:15:25 2024, max compression
+gzip compressed data, was "climb_onyx_client-4.4.0.tar", last modified: Mon Apr 29 14:42:58 2024, max compression
```

## Comparing `climb_onyx_client-4.3.0.tar` & `climb_onyx_client-4.4.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:25.332217 climb_onyx_client-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-24 15:15:25.332217 climb_onyx_client-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:25.332217 climb_onyx_client-4.3.0/climb_onyx_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-24 15:15:25.000000 climb_onyx_client-4.3.0/climb_onyx_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-24 15:15:25.000000 climb_onyx_client-4.3.0/climb_onyx_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:15:25.000000 climb_onyx_client-4.3.0/climb_onyx_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 15:15:25.000000 climb_onyx_client-4.3.0/climb_onyx_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 15:15:25.000000 climb_onyx_client-4.3.0/climb_onyx_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:15:25.000000 climb_onyx_client-4.3.0/climb_onyx_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:25.332217 climb_onyx_client-4.3.0/onyx/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/onyx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    76687 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/onyx/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    32879 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/onyx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/onyx/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/onyx/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/onyx/field.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/onyx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:15:25.332217 climb_onyx_client-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:25.332217 climb_onyx_client-4.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    50827 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/tests/test_field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:42:58.700443 climb_onyx_client-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-29 14:42:58.700443 climb_onyx_client-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:42:58.700443 climb_onyx_client-4.4.0/climb_onyx_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-29 14:42:58.000000 climb_onyx_client-4.4.0/climb_onyx_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-29 14:42:58.000000 climb_onyx_client-4.4.0/climb_onyx_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:42:58.000000 climb_onyx_client-4.4.0/climb_onyx_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 14:42:58.000000 climb_onyx_client-4.4.0/climb_onyx_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 14:42:58.000000 climb_onyx_client-4.4.0/climb_onyx_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 14:42:58.000000 climb_onyx_client-4.4.0/climb_onyx_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:42:58.700443 climb_onyx_client-4.4.0/onyx/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/onyx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77753 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/onyx/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32879 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/onyx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/onyx/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/onyx/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/onyx/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/onyx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:42:58.700443 climb_onyx_client-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:42:58.700443 climb_onyx_client-4.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    52657 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/tests/test_url_formation.py
```

### Comparing `climb_onyx_client-4.3.0/LICENSE` & `climb_onyx_client-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.3.0/PKG-INFO` & `climb_onyx_client-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climb-onyx-client
-Version: 4.3.0
+Version: 4.4.0
 Summary: Client program for interacting with Onyx.
 Home-page: https://github.com/CLIMB-TRE/onyx-client
 Author: Thomas Brier
 Author-email: t.brier@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `climb_onyx_client-4.3.0/README.md` & `climb_onyx_client-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.3.0/climb_onyx_client.egg-info/PKG-INFO` & `climb_onyx_client-4.4.0/climb_onyx_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climb-onyx-client
-Version: 4.3.0
+Version: 4.4.0
 Summary: Client program for interacting with Onyx.
 Home-page: https://github.com/CLIMB-TRE/onyx-client
 Author: Thomas Brier
 Author-email: t.brier@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `climb_onyx_client-4.3.0/onyx/api.py` & `climb_onyx_client-4.4.0/onyx/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os
+import posixpath
 import csv
 import inspect
 import requests
 from requests import HTTPError, RequestException
 from typing import Any, Generator, List, Dict, TextIO, Optional, Union
 from .config import OnyxConfig
 from .field import OnyxField
@@ -14,233 +14,233 @@
 )
 
 
 class OnyxClientBase:
     __slots__ = "config", "_request_handler", "_session"
     ENDPOINTS = {
         "projects": lambda domain: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "projects/",
             ),
             domain=domain,
         ),
         "types": lambda domain: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "projects/types/",
             ),
             domain=domain,
         ),
         "lookups": lambda domain: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "projects/lookups/",
             ),
             domain=domain,
         ),
         "fields": lambda domain, project: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "projects",
                 str(project),
                 "fields/",
             ),
             domain=domain,
             project=project,
         ),
         "choices": lambda domain, project, field: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "projects",
                 str(project),
                 "choices",
                 str(field),
                 "",
             ),
             domain=domain,
             project=project,
             field=field,
         ),
         "get": lambda domain, project, climb_id: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "projects",
                 str(project),
                 str(climb_id),
                 "",
             ),
             domain=domain,
             project=project,
             climb_id=climb_id,
         ),
         "filter": lambda domain, project: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "projects",
                 str(project),
                 "",
             ),
             domain=domain,
             project=project,
         ),
         "query": lambda domain, project: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "projects",
                 str(project),
                 "query/",
             ),
             domain=domain,
             project=project,
         ),
         "history": lambda domain, project, climb_id: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "projects",
                 str(project),
                 "history",
                 str(climb_id),
                 "",
             ),
             domain=domain,
             project=project,
             climb_id=climb_id,
         ),
         "identify": lambda domain, project, field: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "projects",
                 str(project),
                 "identify",
                 str(field),
                 "",
             ),
             domain=domain,
             project=project,
             field=field,
         ),
         "create": lambda domain, project: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "projects",
                 str(project),
                 "",
             ),
             domain=domain,
             project=project,
         ),
         "testcreate": lambda domain, project: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "projects",
                 str(project),
                 "test/",
             ),
             domain=domain,
             project=project,
         ),
         "update": lambda domain, project, climb_id: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "projects",
                 str(project),
                 str(climb_id),
                 "",
             ),
             domain=domain,
             project=project,
             climb_id=climb_id,
         ),
         "testupdate": lambda domain, project, climb_id: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "projects",
                 str(project),
                 "test",
                 str(climb_id),
                 "",
             ),
             domain=domain,
             project=project,
             climb_id=climb_id,
         ),
         "delete": lambda domain, project, climb_id: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "projects",
                 str(project),
                 str(climb_id),
                 "",
             ),
             domain=domain,
             project=project,
             climb_id=climb_id,
         ),
         "register": lambda domain: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "accounts/register/",
             ),
             domain=domain,
         ),
         "login": lambda domain: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "accounts/login/",
             ),
             domain=domain,
         ),
         "logout": lambda domain: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "accounts/logout/",
             ),
             domain=domain,
         ),
         "logoutall": lambda domain: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "accounts/logoutall/",
             ),
             domain=domain,
         ),
         "profile": lambda domain: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "accounts/profile/",
             ),
             domain=domain,
         ),
         "waiting": lambda domain: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "accounts/waiting/",
             ),
             domain=domain,
         ),
         "approve": lambda domain, username: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "accounts/approve",
                 str(username),
                 "",
             ),
             domain=domain,
             username=username,
         ),
         "siteusers": lambda domain: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "accounts/site/",
             ),
             domain=domain,
         ),
         "allusers": lambda domain: OnyxClient._handle_endpoint(
-            lambda: os.path.join(
+            lambda: posixpath.join(
                 str(domain),
                 "accounts/all/",
             ),
             domain=domain,
         ),
     }
 
@@ -472,23 +472,30 @@
     def filter(
         self,
         project: str,
         fields: Optional[Dict[str, Any]] = None,
         include: Union[List[str], str, None] = None,
         exclude: Union[List[str], str, None] = None,
         summarise: Union[List[str], str, None] = None,
+        **kwargs: Any,
     ) -> Generator[requests.Response, Any, None]:
         if fields is None:
             fields = {}
 
         fields = fields | {
             "include": include,
             "exclude": exclude,
             "summarise": summarise,
         }
+
+        for field, value in kwargs.items():
+            if type(value) in {list, tuple, set}:
+                value = ",".join(map(lambda x: str(x) if x is not None else "", value))
+            fields[field] = value
+
         _next = OnyxClient.ENDPOINTS["filter"](self.config.domain, project)
 
         while _next is not None:
             response = self._request(
                 method="get",
                 url=_next,
                 params=fields,
@@ -866,29 +873,29 @@
     """
 
     def __init__(self, config: OnyxConfig) -> None:
         """
         Initialise a client.
 
         Args:
-            config: Object that stores information for connecting and authenticating with Onyx.
+            config: `OnyxConfig` object that stores information for connecting and authenticating with Onyx.
 
         Examples:
             The recommended way to initialise a client (as a context manager):
             ```python
             import os
             from onyx import OnyxConfig, OnyxEnv, OnyxClient
 
             config = OnyxConfig(
                 domain=os.environ[OnyxEnv.DOMAIN],
                 token=os.environ[OnyxEnv.TOKEN],
             )
 
             with OnyxClient(config) as client:
-                pass # Do something with the client here
+                pass # Do something with the client here
             ```
 
             Alternatively, the client can be initialised as follows:
             ```python
             import os
             from onyx import OnyxConfig, OnyxEnv, OnyxClient
 
@@ -1239,15 +1246,15 @@
     ) -> Dict[str, Any]:
         """
         Get a record from a project.
 
         Args:
             project: Name of the project.
             climb_id: Unique identifier for the record in the project.
-            fields: Series of conditions on fields, used to filter the data.
+            fields: Dictionary of field filters used to uniquely identify the record.
             include: Fields to include in the output.
             exclude: Fields to exclude from the output.
 
         Returns:
             Dict containing the record.
 
         Examples:
@@ -1384,45 +1391,57 @@
     def filter(
         self,
         project: str,
         fields: Optional[Dict[str, Any]] = None,
         include: Union[List[str], str, None] = None,
         exclude: Union[List[str], str, None] = None,
         summarise: Union[List[str], str, None] = None,
+        **kwargs: Any,
     ) -> Generator[Dict[str, Any], Any, None]:
         """
         Filter records from a project.
 
         Args:
             project: Name of the project.
-            fields: Series of conditions on fields, used to filter the data.
+            fields: Dictionary of field filters.
             include: Fields to include in the output.
             exclude: Fields to exclude from the output.
             summarise: For a given field (or group of fields), return the frequency of each unique value (or unique group of values).
+            **kwargs: Additional keyword arguments are interpreted as field filters.
 
         Returns:
             Generator of records. If a summarise argument is provided, each record will be a dict containing values of the summary fields and a count for the frequency.
 
         Notes:
-            - The fields argument must be a dict of field conditions. Each of these specifies a requirement that the returned data must match.
-            - These conditions can be a simple match on a value (e.g. `"published_date" : "2023-01-01"`).
-            - Or, they can use a 'lookup' for more complex matching conditions (e.g. `"published_date__year" : "2023"`).
-            - Multi-value lookups must be provided as a comma-separated string of values (e.g. `"published_date__range" : "2023-01-01, 2023-01-02"`).
+            - Field filters specify requirements that the returned data must satisfy. They can be provided as keyword arguments, or as a dictionary to the `fields` argument.
+            - These filters can be a simple match on a value (e.g. `"published_date" : "2023-01-01"`), or they can use a 'lookup' for more complex matching conditions (e.g. `"published_date__iso_year" : "2023"`).
+            - Multi-value lookups (e.g. `in`, `range`) can also be used. For keyword arguments, multiple values can be provided as a Python list. For the `fields` dictionary, multiple values must be provided as a comma-separated string (see examples below).
 
         Examples:
             Retrieve all records that match a set of field requirements:
             ```python
             import os
             from onyx import OnyxConfig, OnyxEnv, OnyxClient
 
             config = OnyxConfig(
                 domain=os.environ[OnyxEnv.DOMAIN],
                 token=os.environ[OnyxEnv.TOKEN],
             )
 
+            # Field conditions can either be provided as keyword arguments:
+            with OnyxClient(config) as client:
+                records = list(
+                    client.filter(
+                        project="project",
+                        field1="abcd",
+                        published_date__range=["2023-01-01", "2023-01-02"],
+                    )
+                )
+
+            # Or as a dictionary to the 'fields' argument:
             with OnyxClient(config) as client:
                 records = list(
                     client.filter(
                         project="project",
                         fields={
                             "field1": "abcd",
                             "published_date__range" : "2023-01-01, 2023-01-02",
@@ -1458,29 +1477,25 @@
                 token=os.environ[OnyxEnv.TOKEN],
             )
 
             with OnyxClient(config) as client:
                 records_v1 = list(
                     client.filter(
                         project="project",
-                        fields={
-                            "field1": "abcd",
-                            "published_date__range" : "2023-01-01, 2023-01-02",
-                        },
+                        field1="abcd",
+                        published_date__range=["2023-01-01", "2023-01-02"],
                         summarise="published_date",
                     )
                 )
 
                 records_v2 = list(
                     client.filter(
                         project="project",
-                        fields={
-                            "field1": "abcd",
-                            "published_date__range" : "2023-01-01, 2023-01-02",
-                        },
+                        field1="abcd",
+                        published_date__range=["2023-01-01", "2023-01-02"],
                         summarise=["published_date", "field2"],
                     )
                 )
             ```
             ```python
             >>> records_v1
             [
@@ -1512,14 +1527,15 @@
 
         responses = super().filter(
             project,
             fields=fields,
             include=include,
             exclude=exclude,
             summarise=summarise,
+            **kwargs,
         )
         for response in responses:
             response.raise_for_status()
             for result in response.json()["data"]:
                 yield result
 
     @onyx_errors
@@ -1530,31 +1546,34 @@
         include: Union[List[str], str, None] = None,
         exclude: Union[List[str], str, None] = None,
         summarise: Union[List[str], str, None] = None,
     ) -> Generator[Dict[str, Any], Any, None]:
         """
         Query records from a project.
 
+        This method supports more complex filtering than the `OnyxClient.filter` method.
+        Here, filters can be combined using Python's bitwise operators, representing AND, OR, XOR and NOT operations.
+
         Args:
             project: Name of the project.
-            query: OnyxField object representing the query being made.
+            query: `OnyxField` object representing the query being made.
             include: Fields to include in the output.
             exclude: Fields to exclude from the output.
             summarise: For a given field (or group of fields), return the frequency of each unique value (or unique group of values).
 
         Returns:
             Generator of records. If a summarise argument is provided, each record will be a dict containing values of the summary fields and a count for the frequency.
 
         Notes:
-            - The query argument must be an instance of OnyxField.
-            - OnyxField instances can be combined into complex expressions using Python's bitwise operators: `&` (AND), `|` (OR), `^` (XOR), and `~` (NOT).
-            - Multi-value lookups (e.g. 'in', 'range') support passing a Python list as the value. These are coerced into comma-separated strings internally.
+            - The `query` argument must be an instance of `OnyxField`.
+            - `OnyxField` instances can be combined into complex expressions using Python's bitwise operators: `&` (AND), `|` (OR), `^` (XOR), and `~` (NOT).
+            - Multi-value lookups (e.g. `in`, `range`) support passing a Python list (see example below).
 
         Examples:
-            Retrieve all records that match the query provided by an OnyxField object:
+            Retrieve all records that match the query provided by an `OnyxField` object:
             ```python
             import os
             from onyx import OnyxConfig, OnyxEnv, OnyxClient, OnyxField
 
             config = OnyxConfig(
                 domain=os.environ[OnyxEnv.DOMAIN],
                 token=os.environ[OnyxEnv.TOKEN],
@@ -1612,15 +1631,15 @@
     ):
         """
         Write a set of records to a CSV file.
 
         Args:
             csv_file: File object for the CSV file being written to.
             data: The data being written to the CSV file. Must be either a list / generator of dict records.
-            delimiter: CSV delimiter. If not provided, defaults to ',' for CSVs. Set this to '\\t' to work with TSV files.
+            delimiter: CSV delimiter. If not provided, defaults to `","` for CSVs. Set this to `"\\t"` to work with TSV files.
 
         Examples:
             ```python
             import os
             from onyx import OnyxConfig, OnyxEnv, OnyxClient
 
             config = OnyxConfig(
@@ -1782,15 +1801,15 @@
     ) -> Dict[str, Any]:
         """
         Create a record in a project.
 
         Args:
             project: Name of the project.
             fields: Object representing the record to be created.
-            test: If True, runs the command as a test. Default: False
+            test: If `True`, runs the command as a test. Default: `False`
 
         Returns:
             Dict containing the CLIMB ID of the created record.
 
         Examples:
             ```python
             import os
@@ -1831,15 +1850,15 @@
         """
         Update a record in a project.
 
         Args:
             project: Name of the project.
             climb_id: Unique identifier for the record in the project.
             fields: Object representing the record to be updated.
-            test: If True, runs the command as a test. Default: False
+            test: If `True`, runs the command as a test. Default: `False`
 
         Returns:
             Dict containing the CLIMB ID of the updated record.
 
         Examples:
             ```python
             import os
@@ -1925,20 +1944,20 @@
         """
         Use a CSV file to create record(s) in a project.
 
         Args:
             project: Name of the project.
             csv_file: File object for the CSV file being used for record upload.
             fields: Additional fields provided for each record being uploaded. Takes precedence over fields in the CSV.
-            delimiter: CSV delimiter. If not provided, defaults to ',' for CSVs. Set this to '\\t' to work with TSV files.
-            multiline: If True, allows processing of CSV files with more than one record. Default: False
-            test: If True, runs the command as a test. Default: False
+            delimiter: CSV delimiter. If not provided, defaults to `","` for CSVs. Set this to `"\\t"` to work with TSV files.
+            multiline: If `True`, allows processing of CSV files with more than one record. Default: `False`
+            test: If `True`, runs the command as a test. Default: `False`
 
         Returns:
-            Dict containing the CLIMB ID of the created record. If multiline = True, returns a list of dicts containing the CLIMB ID of each created record.
+            Dict containing the CLIMB ID of the created record. If `multiline = True`, returns a list of dicts containing the CLIMB ID of each created record.
 
         Examples:
             Create a single record:
             ```python
             import os
             from onyx import OnyxConfig, OnyxEnv, OnyxClient
 
@@ -2008,20 +2027,20 @@
         """
         Use a CSV file to update record(s) in a project.
 
         Args:
             project: Name of the project.
             csv_file: File object for the CSV file being used for record upload.
             fields: Additional fields provided for each record being uploaded. Takes precedence over fields in the CSV.
-            delimiter: CSV delimiter. If not provided, defaults to ',' for CSVs. Set this to '\\t' to work with TSV files.
-            multiline: If True, allows processing of CSV files with more than one record. Default: False
-            test: If True, runs the command as a test. Default: False
+            delimiter: CSV delimiter. If not provided, defaults to `","` for CSVs. Set this to `"\\t"` to work with TSV files.
+            multiline: If `True`, allows processing of CSV files with more than one record. Default: `False`
+            test: If `True`, runs the command as a test. Default: `False`
 
         Returns:
-            Dict containing the CLIMB ID of the updated record. If multiline = True, returns a list of dicts containing the CLIMB ID of each updated record.
+            Dict containing the CLIMB ID of the updated record. If `multiline = True`, returns a list of dicts containing the CLIMB ID of each updated record.
 
         Examples:
             Update a single record:
             ```python
             import os
             from onyx import OnyxConfig, OnyxEnv, OnyxClient
 
@@ -2088,19 +2107,19 @@
     ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
         """
         Use a CSV file to delete record(s) in a project.
 
         Args:
             project: Name of the project.
             csv_file: File object for the CSV file being used for record upload.
-            delimiter: CSV delimiter. If not provided, defaults to ',' for CSVs. Set this to '\\t' to work with TSV files.
-            multiline: If True, allows processing of CSV files with more than one record. Default: False
+            delimiter: CSV delimiter. If not provided, defaults to `","` for CSVs. Set this to `"\\t"` to work with TSV files.
+            multiline: If `True`, allows processing of CSV files with more than one record. Default: `False`
 
         Returns:
-            Dict containing the CLIMB ID of the deleted record. If multiline = True, returns a list of dicts containing the CLIMB ID of each deleted record.
+            Dict containing the CLIMB ID of the deleted record. If `multiline = True`, returns a list of dicts containing the CLIMB ID of each deleted record.
 
         Examples:
             Delete a single record:
             ```python
             import os
             from onyx import OnyxConfig, OnyxEnv, OnyxClient
```

### Comparing `climb_onyx_client-4.3.0/onyx/cli.py` & `climb_onyx_client-4.4.0/onyx/cli.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.3.0/onyx/config.py` & `climb_onyx_client-4.4.0/onyx/config.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.3.0/onyx/exceptions.py` & `climb_onyx_client-4.4.0/onyx/exceptions.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.3.0/onyx/field.py` & `climb_onyx_client-4.4.0/onyx/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,19 +24,19 @@
         Args:
             **kwargs: Keyword arguments containing a single key-value pair.
 
         Notes:
             - Takes a single key-value argument as input.
             - The key corresponds to a field (and optional lookup) to use for filtering.
             - The value corresponds to the field value(s) that are being matched against.
-            - OnyxField instances can be combined into complex expressions using Python's bitwise operators: `&` (AND), `|` (OR), `^` (XOR), and `~` (NOT).
-            - Multi-value lookups (e.g. 'in', 'range') support passing a Python list as the value. These are coerced into comma-separated strings internally.
+            - `OnyxField` instances can be combined into complex expressions using Python's bitwise operators: `&` (AND), `|` (OR), `^` (XOR), and `~` (NOT).
+            - Multi-value lookups (e.g. `in`, `range`) support passing a Python list as the value. These are coerced into comma-separated strings internally.
 
         Examples:
-            Create OnyxField objects and combine them using Python bitwise operators:
+            Create `OnyxField` objects and combine them using Python bitwise operators:
             ```python
             from onyx import OnyxField
 
             field1 = OnyxField(field1="value1")
             field2 = OnyxField(field2__contains="value2")
 
             expression = (field1 | field2) & OnyxField(
```

### Comparing `climb_onyx_client-4.3.0/setup.py` & `climb_onyx_client-4.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.3.0/tests/test_api.py` & `climb_onyx_client-4.4.0/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,14 +220,15 @@
             "sample_id": "sample-123",
             "run_name": "run-456",
         },
     ],
 }
 SAMPLE_ID = "sample-abc"
 RUN_NAME = "run-def"
+PUBLISHED_DATE_RANGE = ["2023-01-01", "2024-01-01"]
 FILTER_SPECIFIC_DATA = {
     "status": "success",
     "code": 200,
     "next": None,
     "previous": None,
     "data": [
         {
@@ -683,14 +684,16 @@
 
         elif url == OnyxClient.ENDPOINTS["filter"](DOMAIN, PROJECT):
             if params.get(UNKNOWN_FIELD):
                 return MockResponse(FILTER_UNKNOWN_FIELD_DATA)
             elif (
                 params.get("sample_id") == SAMPLE_ID
                 and params.get("run_name") == RUN_NAME
+                and params.get("published_date__range")
+                == ",".join(PUBLISHED_DATE_RANGE)
             ):
                 if params.get("include") == INCLUDE_FIELDS:
                     return MockResponse(FILTER_SPECIFIC_INCLUDE_DATA)
                 elif params.get("exclude") == EXCLUDE_FIELDS:
                     return MockResponse(FILTER_SPECIFIC_EXCLUDE_DATA)
                 else:
                     return MockResponse(FILTER_SPECIFIC_DATA)
@@ -905,30 +908,43 @@
         """
         Test that the OnyxClient can retrieve a record from a project.
         """
 
         self.assertEqual(self.client.get(PROJECT, CLIMB_ID), GET_DATA["data"])
         self.assertEqual(
             self.client.get(
-                PROJECT, fields={"sample_id": SAMPLE_ID, "run_name": RUN_NAME}
+                PROJECT,
+                fields={
+                    "sample_id": SAMPLE_ID,
+                    "run_name": RUN_NAME,
+                    "published_date__range": ",".join(PUBLISHED_DATE_RANGE),
+                },
             ),
             FILTER_SPECIFIC_DATA["data"][0],
         )
         self.assertEqual(
             self.client.get(
                 PROJECT,
-                fields={"sample_id": SAMPLE_ID, "run_name": RUN_NAME},
+                fields={
+                    "sample_id": SAMPLE_ID,
+                    "run_name": RUN_NAME,
+                    "published_date__range": ",".join(PUBLISHED_DATE_RANGE),
+                },
                 include=INCLUDE_FIELDS,
             ),
             FILTER_SPECIFIC_INCLUDE_DATA["data"][0],
         )
         self.assertEqual(
             self.client.get(
                 PROJECT,
-                fields={"sample_id": SAMPLE_ID, "run_name": RUN_NAME},
+                fields={
+                    "sample_id": SAMPLE_ID,
+                    "run_name": RUN_NAME,
+                    "published_date__range": ",".join(PUBLISHED_DATE_RANGE),
+                },
                 exclude=EXCLUDE_FIELDS,
             ),
             FILTER_SPECIFIC_EXCLUDE_DATA["data"][0],
         )
         self.assertEqual(self.config.token, TOKEN)
 
         # Cannot provide both CLIMB_ID and fields
@@ -974,36 +990,73 @@
             [x for x in self.client.filter(PROJECT)],
             FILTER_PAGE_1_DATA["data"] + FILTER_PAGE_2_DATA["data"],
         )
         self.assertEqual(
             [
                 x
                 for x in self.client.filter(
-                    PROJECT, fields={"sample_id": SAMPLE_ID, "run_name": RUN_NAME}
+                    PROJECT,
+                    fields={
+                        "sample_id": SAMPLE_ID,
+                        "run_name": RUN_NAME,
+                        "published_date__range": ",".join(PUBLISHED_DATE_RANGE),
+                    },
+                )
+            ],
+            FILTER_SPECIFIC_DATA["data"],
+        )
+        self.assertEqual(
+            [
+                x
+                for x in self.client.filter(
+                    PROJECT,
+                    sample_id=SAMPLE_ID,
+                    run_name=RUN_NAME,
+                    published_date__range=PUBLISHED_DATE_RANGE,
+                )
+            ],
+            FILTER_SPECIFIC_DATA["data"],
+        )
+        self.assertEqual(
+            [
+                x
+                for x in self.client.filter(
+                    PROJECT,
+                    fields={"sample_id": "will-be-overwritten", "run_name": RUN_NAME},
+                    sample_id=SAMPLE_ID,
+                    published_date__range=PUBLISHED_DATE_RANGE,
                 )
             ],
             FILTER_SPECIFIC_DATA["data"],
         )
         self.assertEqual(
             [
                 x
                 for x in self.client.filter(
                     PROJECT,
-                    fields={"sample_id": SAMPLE_ID, "run_name": RUN_NAME},
+                    fields={
+                        "sample_id": SAMPLE_ID,
+                        "run_name": RUN_NAME,
+                        "published_date__range": ",".join(PUBLISHED_DATE_RANGE),
+                    },
                     include=INCLUDE_FIELDS,
                 )
             ],
             FILTER_SPECIFIC_INCLUDE_DATA["data"],
         )
         self.assertEqual(
             [
                 x
                 for x in self.client.filter(
                     PROJECT,
-                    fields={"sample_id": SAMPLE_ID, "run_name": RUN_NAME},
+                    fields={
+                        "sample_id": SAMPLE_ID,
+                        "run_name": RUN_NAME,
+                        "published_date__range": ",".join(PUBLISHED_DATE_RANGE),
+                    },
                     exclude=EXCLUDE_FIELDS,
                 )
             ],
             FILTER_SPECIFIC_EXCLUDE_DATA["data"],
         )
         self.assertEqual(self.config.token, TOKEN)
```

### Comparing `climb_onyx_client-4.3.0/tests/test_config.py` & `climb_onyx_client-4.4.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.3.0/tests/test_field.py` & `climb_onyx_client-4.4.0/tests/test_field.py`

 * *Files identical despite different names*

