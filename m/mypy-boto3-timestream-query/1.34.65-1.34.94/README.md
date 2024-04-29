# Comparing `tmp/mypy-boto3-timestream-query-1.34.65.tar.gz` & `tmp/mypy_boto3_timestream_query-1.34.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-timestream-query-1.34.65.tar", last modified: Mon Mar 18 20:47:31 2024, max compression
+gzip compressed data, was "mypy_boto3_timestream_query-1.34.94.tar", last modified: Mon Apr 29 19:32:09 2024, max compression
```

## Comparing `mypy-boto3-timestream-query-1.34.65.tar` & `mypy_boto3_timestream_query-1.34.94.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:31.594604 mypy-boto3-timestream-query-1.34.65/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-03-18 20:47:31.594604 mypy-boto3-timestream-query-1.34.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11915 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:31.594604 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13137 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13134 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15910 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15910 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:31.594604 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-03-18 20:47:31.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-18 20:47:31.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 20:47:31.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 20:47:31.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-18 20:47:31.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-18 20:47:31.000000 mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 20:47:31.594604 mypy-boto3-timestream-query-1.34.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-18 20:47:19.000000 mypy-boto3-timestream-query-1.34.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:09.370772 mypy_boto3_timestream_query-1.34.94/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 19:31:53.000000 mypy_boto3_timestream_query-1.34.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-29 19:32:09.370772 mypy_boto3_timestream_query-1.34.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11915 2024-04-29 19:31:53.000000 mypy_boto3_timestream_query-1.34.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:09.370772 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-29 19:31:53.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-29 19:31:53.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-29 19:31:53.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14539 2024-04-29 19:31:53.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14536 2024-04-29 19:31:53.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9706 2024-04-29 19:31:53.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9706 2024-04-29 19:31:53.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-29 19:31:53.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-29 19:31:53.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:31:53.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18455 2024-04-29 19:31:54.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18455 2024-04-29 19:31:54.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 19:31:53.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:09.370772 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-29 19:32:09.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-29 19:32:09.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:09.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:09.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 19:32:09.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 19:32:09.000000 mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:32:09.370772 mypy_boto3_timestream_query-1.34.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-29 19:31:53.000000 mypy_boto3_timestream_query-1.34.94/setup.py
```

### Comparing `mypy-boto3-timestream-query-1.34.65/LICENSE` & `mypy_boto3_timestream_query-1.34.94/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.34.65/PKG-INFO` & `mypy_boto3_timestream_query-1.34.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-query
-Version: 1.34.65
-Summary: Type annotations for boto3.TimestreamQuery 1.34.65 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.94
+Summary: Type annotations for boto3.TimestreamQuery 1.34.94 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-query)](https://pepy.tech/project/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.34.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-timestream-query-1.34.65/README.md` & `mypy_boto3_timestream_query-1.34.94/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-query)](https://pepy.tech/project/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.34.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/__init__.py` & `mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/__init__.pyi` & `mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/__main__.py` & `mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TimestreamQuery 1.34.65\n"
-        "Version:         1.34.65\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.TimestreamQuery 1.34.94\n"
+        "Version:         1.34.94\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.65")
+    print("1.34.94")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/client.py` & `mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,32 +15,34 @@
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import ScheduledQueryStateType
+from .literals import QueryPricingModelType, ScheduledQueryStateType
 from .paginator import ListScheduledQueriesPaginator, ListTagsForResourcePaginator, QueryPaginator
 from .type_defs import (
     CancelQueryResponseTypeDef,
     CreateScheduledQueryResponseTypeDef,
+    DescribeAccountSettingsResponseTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeScheduledQueryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ErrorReportConfigurationTypeDef,
     ListScheduledQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
-    TargetConfigurationTypeDef,
+    TargetConfigurationUnionTypeDef,
     TimestampTypeDef,
+    UpdateAccountSettingsResponseTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -114,15 +116,15 @@
         *,
         Name: str,
         QueryString: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         NotificationConfiguration: NotificationConfigurationTypeDef,
         ScheduledQueryExecutionRoleArn: str,
         ErrorReportConfiguration: ErrorReportConfigurationTypeDef,
-        TargetConfiguration: TargetConfigurationTypeDef = ...,
+        TargetConfiguration: TargetConfigurationUnionTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
     ) -> CreateScheduledQueryResponseTypeDef:
         """
         Create a scheduled query that will be run on your behalf at the configured
         schedule.
@@ -135,14 +137,24 @@
         """
         Deletes a given scheduled query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.delete_scheduled_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/client/#delete_scheduled_query)
         """
 
+    def describe_account_settings(self) -> DescribeAccountSettingsResponseTypeDef:
+        """
+        Describes the settings for your account that include the query pricing model
+        and the configured maximum TCUs the service can use for your query
+        workload.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.describe_account_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/client/#describe_account_settings)
+        """
+
     def describe_endpoints(self) -> DescribeEndpointsResponseTypeDef:
         """
         DescribeEndpoints returns a list of available endpoints to make Timestream API
         calls
         against.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.describe_endpoints)
@@ -239,14 +251,26 @@
         """
         Removes the association of tags from a Timestream query resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/client/#untag_resource)
         """
 
+    def update_account_settings(
+        self, *, MaxQueryTCU: int = ..., QueryPricingModel: QueryPricingModelType = ...
+    ) -> UpdateAccountSettingsResponseTypeDef:
+        """
+        Transitions your account to use TCUs for query pricing and modifies the maximum
+        query compute units that you've
+        configured.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.update_account_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/client/#update_account_settings)
+        """
+
     def update_scheduled_query(
         self, *, ScheduledQueryArn: str, State: ScheduledQueryStateType
     ) -> EmptyResponseMetadataTypeDef:
         """
         Update a scheduled query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.update_scheduled_query)
```

### Comparing `mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/client.pyi` & `mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -15,32 +15,34 @@
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import ScheduledQueryStateType
+from .literals import QueryPricingModelType, ScheduledQueryStateType
 from .paginator import ListScheduledQueriesPaginator, ListTagsForResourcePaginator, QueryPaginator
 from .type_defs import (
     CancelQueryResponseTypeDef,
     CreateScheduledQueryResponseTypeDef,
+    DescribeAccountSettingsResponseTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeScheduledQueryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ErrorReportConfigurationTypeDef,
     ListScheduledQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
-    TargetConfigurationTypeDef,
+    TargetConfigurationUnionTypeDef,
     TimestampTypeDef,
+    UpdateAccountSettingsResponseTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -111,15 +113,15 @@
         *,
         Name: str,
         QueryString: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         NotificationConfiguration: NotificationConfigurationTypeDef,
         ScheduledQueryExecutionRoleArn: str,
         ErrorReportConfiguration: ErrorReportConfigurationTypeDef,
-        TargetConfiguration: TargetConfigurationTypeDef = ...,
+        TargetConfiguration: TargetConfigurationUnionTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
     ) -> CreateScheduledQueryResponseTypeDef:
         """
         Create a scheduled query that will be run on your behalf at the configured
         schedule.
@@ -132,14 +134,24 @@
         """
         Deletes a given scheduled query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.delete_scheduled_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/client/#delete_scheduled_query)
         """
 
+    def describe_account_settings(self) -> DescribeAccountSettingsResponseTypeDef:
+        """
+        Describes the settings for your account that include the query pricing model
+        and the configured maximum TCUs the service can use for your query
+        workload.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.describe_account_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/client/#describe_account_settings)
+        """
+
     def describe_endpoints(self) -> DescribeEndpointsResponseTypeDef:
         """
         DescribeEndpoints returns a list of available endpoints to make Timestream API
         calls
         against.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.describe_endpoints)
@@ -236,14 +248,26 @@
         """
         Removes the association of tags from a Timestream query resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/client/#untag_resource)
         """
 
+    def update_account_settings(
+        self, *, MaxQueryTCU: int = ..., QueryPricingModel: QueryPricingModelType = ...
+    ) -> UpdateAccountSettingsResponseTypeDef:
+        """
+        Transitions your account to use TCUs for query pricing and modifies the maximum
+        query compute units that you've
+        configured.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.update_account_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/client/#update_account_settings)
+        """
+
     def update_scheduled_query(
         self, *, ScheduledQueryArn: str, State: ScheduledQueryStateType
     ) -> EmptyResponseMetadataTypeDef:
         """
         Update a scheduled query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.update_scheduled_query)
```

### Comparing `mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/literals.py` & `mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 __all__ = (
     "DimensionValueTypeType",
     "ListScheduledQueriesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "MeasureValueTypeType",
     "QueryPaginatorName",
+    "QueryPricingModelType",
     "S3EncryptionOptionType",
     "ScalarMeasureValueTypeType",
     "ScalarTypeType",
     "ScheduledQueryRunStatusType",
     "ScheduledQueryStateType",
     "TimestreamQueryServiceName",
     "ServiceName",
@@ -37,14 +38,15 @@
 )
 
 DimensionValueTypeType = Literal["VARCHAR"]
 ListScheduledQueriesPaginatorName = Literal["list_scheduled_queries"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 MeasureValueTypeType = Literal["BIGINT", "BOOLEAN", "DOUBLE", "MULTI", "VARCHAR"]
 QueryPaginatorName = Literal["query"]
+QueryPricingModelType = Literal["BYTES_SCANNED", "COMPUTE_UNITS"]
 S3EncryptionOptionType = Literal["SSE_KMS", "SSE_S3"]
 ScalarMeasureValueTypeType = Literal["BIGINT", "BOOLEAN", "DOUBLE", "TIMESTAMP", "VARCHAR"]
 ScalarTypeType = Literal[
     "BIGINT",
     "BOOLEAN",
     "DATE",
     "DOUBLE",
@@ -131,14 +133,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -151,24 +154,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -365,14 +370,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/literals.pyi` & `mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 __all__ = (
     "DimensionValueTypeType",
     "ListScheduledQueriesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "MeasureValueTypeType",
     "QueryPaginatorName",
+    "QueryPricingModelType",
     "S3EncryptionOptionType",
     "ScalarMeasureValueTypeType",
     "ScalarTypeType",
     "ScheduledQueryRunStatusType",
     "ScheduledQueryStateType",
     "TimestreamQueryServiceName",
     "ServiceName",
@@ -37,14 +38,15 @@
 )
 
 DimensionValueTypeType = Literal["VARCHAR"]
 ListScheduledQueriesPaginatorName = Literal["list_scheduled_queries"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 MeasureValueTypeType = Literal["BIGINT", "BOOLEAN", "DOUBLE", "MULTI", "VARCHAR"]
 QueryPaginatorName = Literal["query"]
+QueryPricingModelType = Literal["BYTES_SCANNED", "COMPUTE_UNITS"]
 S3EncryptionOptionType = Literal["SSE_KMS", "SSE_S3"]
 ScalarMeasureValueTypeType = Literal["BIGINT", "BOOLEAN", "DOUBLE", "TIMESTAMP", "VARCHAR"]
 ScalarTypeType = Literal[
     "BIGINT",
     "BOOLEAN",
     "DATE",
     "DOUBLE",
@@ -131,14 +133,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -151,24 +154,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -365,14 +370,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/paginator.py` & `mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/paginator.pyi` & `mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/type_defs.py` & `mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Sequence, Union
 
 from .literals import (
     MeasureValueTypeType,
+    QueryPricingModelType,
     S3EncryptionOptionType,
     ScalarMeasureValueTypeType,
     ScalarTypeType,
     ScheduledQueryRunStatusType,
     ScheduledQueryStateType,
 )
 
@@ -63,41 +64,49 @@
     "PrepareQueryRequestRequestTypeDef",
     "SelectColumnTypeDef",
     "QueryRequestRequestTypeDef",
     "QueryStatusTypeDef",
     "TimestreamDestinationTypeDef",
     "TypeTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateAccountSettingsRequestRequestTypeDef",
     "UpdateScheduledQueryRequestRequestTypeDef",
     "CancelQueryResponseTypeDef",
     "CreateScheduledQueryResponseTypeDef",
+    "DescribeAccountSettingsResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "UpdateAccountSettingsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatumTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "ErrorReportConfigurationTypeDef",
     "ErrorReportLocationTypeDef",
     "ExecuteScheduledQueryRequestRequestTypeDef",
     "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "QueryRequestQueryPaginateTypeDef",
+    "MixedMeasureMappingOutputTypeDef",
     "MixedMeasureMappingTypeDef",
+    "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
     "NotificationConfigurationTypeDef",
     "PrepareQueryResponseTypeDef",
     "QueryResponseTypeDef",
     "TargetDestinationTypeDef",
     "ScheduledQueryRunSummaryTypeDef",
+    "TimestreamConfigurationOutputTypeDef",
     "TimestreamConfigurationTypeDef",
     "ScheduledQueryTypeDef",
+    "TargetConfigurationOutputTypeDef",
     "TargetConfigurationTypeDef",
     "ListScheduledQueriesResponseTypeDef",
-    "CreateScheduledQueryRequestRequestTypeDef",
     "ScheduledQueryDescriptionTypeDef",
+    "CreateScheduledQueryRequestRequestTypeDef",
+    "TargetConfigurationUnionTypeDef",
     "DescribeScheduledQueryResponseTypeDef",
 )
 
 CancelQueryRequestRequestTypeDef = TypedDict(
     "CancelQueryRequestRequestTypeDef",
     {
         "QueryId": str,
@@ -190,14 +199,15 @@
 TimestampTypeDef = Union[datetime, str]
 ExecutionStatsTypeDef = TypedDict(
     "ExecutionStatsTypeDef",
     {
         "ExecutionTimeInMillis": NotRequired[int],
         "DataWrites": NotRequired[int],
         "BytesMetered": NotRequired[int],
+        "CumulativeBytesScanned": NotRequired[int],
         "RecordsIngested": NotRequired[int],
         "QueryResultRows": NotRequired[int],
     },
 )
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
@@ -295,14 +305,21 @@
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
+UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateAccountSettingsRequestRequestTypeDef",
+    {
+        "MaxQueryTCU": NotRequired[int],
+        "QueryPricingModel": NotRequired[QueryPricingModelType],
+    },
+)
 UpdateScheduledQueryRequestRequestTypeDef = TypedDict(
     "UpdateScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
         "State": ScheduledQueryStateType,
     },
 )
@@ -316,26 +333,42 @@
 CreateScheduledQueryResponseTypeDef = TypedDict(
     "CreateScheduledQueryResponseTypeDef",
     {
         "Arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeAccountSettingsResponseTypeDef = TypedDict(
+    "DescribeAccountSettingsResponseTypeDef",
+    {
+        "MaxQueryTCU": int,
+        "QueryPricingModel": QueryPricingModelType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateAccountSettingsResponseTypeDef = TypedDict(
+    "UpdateAccountSettingsResponseTypeDef",
+    {
+        "MaxQueryTCU": int,
+        "QueryPricingModel": QueryPricingModelType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
@@ -395,24 +428,41 @@
     "QueryRequestQueryPaginateTypeDef",
     {
         "QueryString": str,
         "ClientToken": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+MixedMeasureMappingOutputTypeDef = TypedDict(
+    "MixedMeasureMappingOutputTypeDef",
+    {
+        "MeasureValueType": MeasureValueTypeType,
+        "MeasureName": NotRequired[str],
+        "SourceColumn": NotRequired[str],
+        "TargetMeasureName": NotRequired[str],
+        "MultiMeasureAttributeMappings": NotRequired[List[MultiMeasureAttributeMappingTypeDef]],
+    },
+)
 MixedMeasureMappingTypeDef = TypedDict(
     "MixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
         "MeasureName": NotRequired[str],
         "SourceColumn": NotRequired[str],
         "TargetMeasureName": NotRequired[str],
         "MultiMeasureAttributeMappings": NotRequired[Sequence[MultiMeasureAttributeMappingTypeDef]],
     },
 )
+MultiMeasureMappingsOutputTypeDef = TypedDict(
+    "MultiMeasureMappingsOutputTypeDef",
+    {
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
+        "TargetMultiMeasureName": NotRequired[str],
+    },
+)
 MultiMeasureMappingsTypeDef = TypedDict(
     "MultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
         "TargetMultiMeasureName": NotRequired[str],
     },
 )
@@ -431,19 +481,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 QueryResponseTypeDef = TypedDict(
     "QueryResponseTypeDef",
     {
         "QueryId": str,
-        "NextToken": str,
         "Rows": List[RowTypeDef],
         "ColumnInfo": List["ColumnInfoTypeDef"],
         "QueryStatus": QueryStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 TargetDestinationTypeDef = TypedDict(
     "TargetDestinationTypeDef",
     {
         "TimestreamDestination": NotRequired[TimestreamDestinationTypeDef],
     },
@@ -455,14 +505,26 @@
         "TriggerTime": NotRequired[datetime],
         "RunStatus": NotRequired[ScheduledQueryRunStatusType],
         "ExecutionStats": NotRequired[ExecutionStatsTypeDef],
         "ErrorReportLocation": NotRequired[ErrorReportLocationTypeDef],
         "FailureReason": NotRequired[str],
     },
 )
+TimestreamConfigurationOutputTypeDef = TypedDict(
+    "TimestreamConfigurationOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "TimeColumn": str,
+        "DimensionMappings": List[DimensionMappingTypeDef],
+        "MultiMeasureMappings": NotRequired[MultiMeasureMappingsOutputTypeDef],
+        "MixedMeasureMappings": NotRequired[List[MixedMeasureMappingOutputTypeDef]],
+        "MeasureNameColumn": NotRequired[str],
+    },
+)
 TimestreamConfigurationTypeDef = TypedDict(
     "TimestreamConfigurationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "TimeColumn": str,
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
@@ -481,63 +543,72 @@
         "PreviousInvocationTime": NotRequired[datetime],
         "NextInvocationTime": NotRequired[datetime],
         "ErrorReportConfiguration": NotRequired[ErrorReportConfigurationTypeDef],
         "TargetDestination": NotRequired[TargetDestinationTypeDef],
         "LastRunStatus": NotRequired[ScheduledQueryRunStatusType],
     },
 )
+TargetConfigurationOutputTypeDef = TypedDict(
+    "TargetConfigurationOutputTypeDef",
+    {
+        "TimestreamConfiguration": TimestreamConfigurationOutputTypeDef,
+    },
+)
 TargetConfigurationTypeDef = TypedDict(
     "TargetConfigurationTypeDef",
     {
         "TimestreamConfiguration": TimestreamConfigurationTypeDef,
     },
 )
 ListScheduledQueriesResponseTypeDef = TypedDict(
     "ListScheduledQueriesResponseTypeDef",
     {
         "ScheduledQueries": List[ScheduledQueryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-CreateScheduledQueryRequestRequestTypeDef = TypedDict(
-    "CreateScheduledQueryRequestRequestTypeDef",
-    {
-        "Name": str,
-        "QueryString": str,
-        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
-        "NotificationConfiguration": NotificationConfigurationTypeDef,
-        "ScheduledQueryExecutionRoleArn": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
-        "TargetConfiguration": NotRequired[TargetConfigurationTypeDef],
-        "ClientToken": NotRequired[str],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "KmsKeyId": NotRequired[str],
+        "NextToken": NotRequired[str],
     },
 )
 ScheduledQueryDescriptionTypeDef = TypedDict(
     "ScheduledQueryDescriptionTypeDef",
     {
         "Arn": str,
         "Name": str,
         "QueryString": str,
         "State": ScheduledQueryStateType,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
         "CreationTime": NotRequired[datetime],
         "PreviousInvocationTime": NotRequired[datetime],
         "NextInvocationTime": NotRequired[datetime],
-        "TargetConfiguration": NotRequired[TargetConfigurationTypeDef],
+        "TargetConfiguration": NotRequired[TargetConfigurationOutputTypeDef],
         "ScheduledQueryExecutionRoleArn": NotRequired[str],
         "KmsKeyId": NotRequired[str],
         "ErrorReportConfiguration": NotRequired[ErrorReportConfigurationTypeDef],
         "LastRunSummary": NotRequired[ScheduledQueryRunSummaryTypeDef],
         "RecentlyFailedRuns": NotRequired[List[ScheduledQueryRunSummaryTypeDef]],
     },
 )
+CreateScheduledQueryRequestRequestTypeDef = TypedDict(
+    "CreateScheduledQueryRequestRequestTypeDef",
+    {
+        "Name": str,
+        "QueryString": str,
+        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
+        "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "ScheduledQueryExecutionRoleArn": str,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
+        "TargetConfiguration": NotRequired[TargetConfigurationTypeDef],
+        "ClientToken": NotRequired[str],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "KmsKeyId": NotRequired[str],
+    },
+)
+TargetConfigurationUnionTypeDef = Union[
+    TargetConfigurationTypeDef, TargetConfigurationOutputTypeDef
+]
 DescribeScheduledQueryResponseTypeDef = TypedDict(
     "DescribeScheduledQueryResponseTypeDef",
     {
         "ScheduledQuery": ScheduledQueryDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query/type_defs.pyi` & `mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Sequence, Union
 
 from .literals import (
     MeasureValueTypeType,
+    QueryPricingModelType,
     S3EncryptionOptionType,
     ScalarMeasureValueTypeType,
     ScalarTypeType,
     ScheduledQueryRunStatusType,
     ScheduledQueryStateType,
 )
 
@@ -63,41 +64,49 @@
     "PrepareQueryRequestRequestTypeDef",
     "SelectColumnTypeDef",
     "QueryRequestRequestTypeDef",
     "QueryStatusTypeDef",
     "TimestreamDestinationTypeDef",
     "TypeTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateAccountSettingsRequestRequestTypeDef",
     "UpdateScheduledQueryRequestRequestTypeDef",
     "CancelQueryResponseTypeDef",
     "CreateScheduledQueryResponseTypeDef",
+    "DescribeAccountSettingsResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "UpdateAccountSettingsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatumTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "ErrorReportConfigurationTypeDef",
     "ErrorReportLocationTypeDef",
     "ExecuteScheduledQueryRequestRequestTypeDef",
     "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "QueryRequestQueryPaginateTypeDef",
+    "MixedMeasureMappingOutputTypeDef",
     "MixedMeasureMappingTypeDef",
+    "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
     "NotificationConfigurationTypeDef",
     "PrepareQueryResponseTypeDef",
     "QueryResponseTypeDef",
     "TargetDestinationTypeDef",
     "ScheduledQueryRunSummaryTypeDef",
+    "TimestreamConfigurationOutputTypeDef",
     "TimestreamConfigurationTypeDef",
     "ScheduledQueryTypeDef",
+    "TargetConfigurationOutputTypeDef",
     "TargetConfigurationTypeDef",
     "ListScheduledQueriesResponseTypeDef",
-    "CreateScheduledQueryRequestRequestTypeDef",
     "ScheduledQueryDescriptionTypeDef",
+    "CreateScheduledQueryRequestRequestTypeDef",
+    "TargetConfigurationUnionTypeDef",
     "DescribeScheduledQueryResponseTypeDef",
 )
 
 CancelQueryRequestRequestTypeDef = TypedDict(
     "CancelQueryRequestRequestTypeDef",
     {
         "QueryId": str,
@@ -190,14 +199,15 @@
 TimestampTypeDef = Union[datetime, str]
 ExecutionStatsTypeDef = TypedDict(
     "ExecutionStatsTypeDef",
     {
         "ExecutionTimeInMillis": NotRequired[int],
         "DataWrites": NotRequired[int],
         "BytesMetered": NotRequired[int],
+        "CumulativeBytesScanned": NotRequired[int],
         "RecordsIngested": NotRequired[int],
         "QueryResultRows": NotRequired[int],
     },
 )
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
@@ -295,14 +305,21 @@
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
+UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateAccountSettingsRequestRequestTypeDef",
+    {
+        "MaxQueryTCU": NotRequired[int],
+        "QueryPricingModel": NotRequired[QueryPricingModelType],
+    },
+)
 UpdateScheduledQueryRequestRequestTypeDef = TypedDict(
     "UpdateScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
         "State": ScheduledQueryStateType,
     },
 )
@@ -316,26 +333,42 @@
 CreateScheduledQueryResponseTypeDef = TypedDict(
     "CreateScheduledQueryResponseTypeDef",
     {
         "Arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeAccountSettingsResponseTypeDef = TypedDict(
+    "DescribeAccountSettingsResponseTypeDef",
+    {
+        "MaxQueryTCU": int,
+        "QueryPricingModel": QueryPricingModelType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateAccountSettingsResponseTypeDef = TypedDict(
+    "UpdateAccountSettingsResponseTypeDef",
+    {
+        "MaxQueryTCU": int,
+        "QueryPricingModel": QueryPricingModelType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
@@ -395,24 +428,41 @@
     "QueryRequestQueryPaginateTypeDef",
     {
         "QueryString": str,
         "ClientToken": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+MixedMeasureMappingOutputTypeDef = TypedDict(
+    "MixedMeasureMappingOutputTypeDef",
+    {
+        "MeasureValueType": MeasureValueTypeType,
+        "MeasureName": NotRequired[str],
+        "SourceColumn": NotRequired[str],
+        "TargetMeasureName": NotRequired[str],
+        "MultiMeasureAttributeMappings": NotRequired[List[MultiMeasureAttributeMappingTypeDef]],
+    },
+)
 MixedMeasureMappingTypeDef = TypedDict(
     "MixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
         "MeasureName": NotRequired[str],
         "SourceColumn": NotRequired[str],
         "TargetMeasureName": NotRequired[str],
         "MultiMeasureAttributeMappings": NotRequired[Sequence[MultiMeasureAttributeMappingTypeDef]],
     },
 )
+MultiMeasureMappingsOutputTypeDef = TypedDict(
+    "MultiMeasureMappingsOutputTypeDef",
+    {
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
+        "TargetMultiMeasureName": NotRequired[str],
+    },
+)
 MultiMeasureMappingsTypeDef = TypedDict(
     "MultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
         "TargetMultiMeasureName": NotRequired[str],
     },
 )
@@ -431,19 +481,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 QueryResponseTypeDef = TypedDict(
     "QueryResponseTypeDef",
     {
         "QueryId": str,
-        "NextToken": str,
         "Rows": List[RowTypeDef],
         "ColumnInfo": List["ColumnInfoTypeDef"],
         "QueryStatus": QueryStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 TargetDestinationTypeDef = TypedDict(
     "TargetDestinationTypeDef",
     {
         "TimestreamDestination": NotRequired[TimestreamDestinationTypeDef],
     },
@@ -455,14 +505,26 @@
         "TriggerTime": NotRequired[datetime],
         "RunStatus": NotRequired[ScheduledQueryRunStatusType],
         "ExecutionStats": NotRequired[ExecutionStatsTypeDef],
         "ErrorReportLocation": NotRequired[ErrorReportLocationTypeDef],
         "FailureReason": NotRequired[str],
     },
 )
+TimestreamConfigurationOutputTypeDef = TypedDict(
+    "TimestreamConfigurationOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "TimeColumn": str,
+        "DimensionMappings": List[DimensionMappingTypeDef],
+        "MultiMeasureMappings": NotRequired[MultiMeasureMappingsOutputTypeDef],
+        "MixedMeasureMappings": NotRequired[List[MixedMeasureMappingOutputTypeDef]],
+        "MeasureNameColumn": NotRequired[str],
+    },
+)
 TimestreamConfigurationTypeDef = TypedDict(
     "TimestreamConfigurationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "TimeColumn": str,
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
@@ -481,63 +543,72 @@
         "PreviousInvocationTime": NotRequired[datetime],
         "NextInvocationTime": NotRequired[datetime],
         "ErrorReportConfiguration": NotRequired[ErrorReportConfigurationTypeDef],
         "TargetDestination": NotRequired[TargetDestinationTypeDef],
         "LastRunStatus": NotRequired[ScheduledQueryRunStatusType],
     },
 )
+TargetConfigurationOutputTypeDef = TypedDict(
+    "TargetConfigurationOutputTypeDef",
+    {
+        "TimestreamConfiguration": TimestreamConfigurationOutputTypeDef,
+    },
+)
 TargetConfigurationTypeDef = TypedDict(
     "TargetConfigurationTypeDef",
     {
         "TimestreamConfiguration": TimestreamConfigurationTypeDef,
     },
 )
 ListScheduledQueriesResponseTypeDef = TypedDict(
     "ListScheduledQueriesResponseTypeDef",
     {
         "ScheduledQueries": List[ScheduledQueryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-CreateScheduledQueryRequestRequestTypeDef = TypedDict(
-    "CreateScheduledQueryRequestRequestTypeDef",
-    {
-        "Name": str,
-        "QueryString": str,
-        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
-        "NotificationConfiguration": NotificationConfigurationTypeDef,
-        "ScheduledQueryExecutionRoleArn": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
-        "TargetConfiguration": NotRequired[TargetConfigurationTypeDef],
-        "ClientToken": NotRequired[str],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "KmsKeyId": NotRequired[str],
+        "NextToken": NotRequired[str],
     },
 )
 ScheduledQueryDescriptionTypeDef = TypedDict(
     "ScheduledQueryDescriptionTypeDef",
     {
         "Arn": str,
         "Name": str,
         "QueryString": str,
         "State": ScheduledQueryStateType,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
         "CreationTime": NotRequired[datetime],
         "PreviousInvocationTime": NotRequired[datetime],
         "NextInvocationTime": NotRequired[datetime],
-        "TargetConfiguration": NotRequired[TargetConfigurationTypeDef],
+        "TargetConfiguration": NotRequired[TargetConfigurationOutputTypeDef],
         "ScheduledQueryExecutionRoleArn": NotRequired[str],
         "KmsKeyId": NotRequired[str],
         "ErrorReportConfiguration": NotRequired[ErrorReportConfigurationTypeDef],
         "LastRunSummary": NotRequired[ScheduledQueryRunSummaryTypeDef],
         "RecentlyFailedRuns": NotRequired[List[ScheduledQueryRunSummaryTypeDef]],
     },
 )
+CreateScheduledQueryRequestRequestTypeDef = TypedDict(
+    "CreateScheduledQueryRequestRequestTypeDef",
+    {
+        "Name": str,
+        "QueryString": str,
+        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
+        "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "ScheduledQueryExecutionRoleArn": str,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
+        "TargetConfiguration": NotRequired[TargetConfigurationTypeDef],
+        "ClientToken": NotRequired[str],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "KmsKeyId": NotRequired[str],
+    },
+)
+TargetConfigurationUnionTypeDef = Union[
+    TargetConfigurationTypeDef, TargetConfigurationOutputTypeDef
+]
 DescribeScheduledQueryResponseTypeDef = TypedDict(
     "DescribeScheduledQueryResponseTypeDef",
     {
         "ScheduledQuery": ScheduledQueryDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query.egg-info/PKG-INFO` & `mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-query
-Version: 1.34.65
-Summary: Type annotations for boto3.TimestreamQuery 1.34.65 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.94
+Summary: Type annotations for boto3.TimestreamQuery 1.34.94 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-query)](https://pepy.tech/project/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.34.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-timestream-query-1.34.65/mypy_boto3_timestream_query.egg-info/SOURCES.txt` & `mypy_boto3_timestream_query-1.34.94/mypy_boto3_timestream_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.34.65/setup.py` & `mypy_boto3_timestream_query-1.34.94/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-timestream-query",
-    version="1.34.65",
+    version="1.34.94",
     packages=["mypy_boto3_timestream_query"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.TimestreamQuery 1.34.65 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.TimestreamQuery 1.34.94 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

