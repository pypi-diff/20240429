# Comparing `tmp/mypy-boto3-trustedadvisor-1.34.0.tar.gz` & `tmp/mypy_boto3_trustedadvisor-1.34.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-trustedadvisor-1.34.0.tar", last modified: Wed Dec 13 21:24:03 2023, max compression
+gzip compressed data, was "mypy_boto3_trustedadvisor-1.34.94.tar", last modified: Mon Apr 29 19:32:10 2024, max compression
```

## Comparing `mypy-boto3-trustedadvisor-1.34.0.tar` & `mypy_boto3_trustedadvisor-1.34.94.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:03.719408 mypy-boto3-trustedadvisor-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:20:50.000000 mypy-boto3-trustedadvisor-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14220 2023-12-13 21:24:03.719408 mypy-boto3-trustedadvisor-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12650 2023-12-13 21:20:50.000000 mypy-boto3-trustedadvisor-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:03.715408 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 21:20:50.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2023-12-13 21:20:50.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2023-12-13 21:20:50.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15594 2023-12-13 21:20:50.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15590 2023-12-13 21:20:50.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10724 2023-12-13 21:20:50.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10722 2023-12-13 21:20:50.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2023-12-13 21:20:50.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9870 2023-12-13 21:20:50.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:20:50.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18905 2023-12-13 21:20:51.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18904 2023-12-13 21:20:50.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:20:50.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:03.715408 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14220 2023-12-13 21:24:03.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-13 21:24:03.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:24:03.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:24:03.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:24:03.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 21:24:03.000000 mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:24:03.719408 mypy-boto3-trustedadvisor-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2023-12-13 21:20:50.000000 mypy-boto3-trustedadvisor-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:10.078770 mypy_boto3_trustedadvisor-1.34.94/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 19:31:56.000000 mypy_boto3_trustedadvisor-1.34.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14235 2024-04-29 19:32:10.078770 mypy_boto3_trustedadvisor-1.34.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-29 19:31:56.000000 mypy_boto3_trustedadvisor-1.34.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:10.074770 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-29 19:31:56.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-29 19:31:56.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-29 19:31:56.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16717 2024-04-29 19:31:56.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16714 2024-04-29 19:31:56.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-04-29 19:31:56.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-04-29 19:31:56.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-04-29 19:31:56.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-04-29 19:31:56.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:31:56.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20567 2024-04-29 19:31:57.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20567 2024-04-29 19:31:57.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 19:31:56.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:10.078770 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14235 2024-04-29 19:32:10.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-29 19:32:10.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:10.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:10.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 19:32:10.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 19:32:10.000000 mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:32:10.078770 mypy_boto3_trustedadvisor-1.34.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-29 19:31:56.000000 mypy_boto3_trustedadvisor-1.34.94/setup.py
```

### Comparing `mypy-boto3-trustedadvisor-1.34.0/LICENSE` & `mypy_boto3_trustedadvisor-1.34.94/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-trustedadvisor-1.34.0/PKG-INFO` & `mypy_boto3_trustedadvisor-1.34.94/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-trustedadvisor
-Version: 1.34.0
-Summary: Type annotations for boto3.TrustedAdvisorPublicAPI 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.94
+Summary: Type annotations for boto3.TrustedAdvisorPublicAPI 1.34.94 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-trustedadvisor"></a>
 
 # mypy-boto3-trustedadvisor
 
 [![PyPI - mypy-boto3-trustedadvisor](https://img.shields.io/pypi/v/mypy-boto3-trustedadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-trustedadvisor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-trustedadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-trustedadvisor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-trustedadvisor)](https://pepy.tech/project/mypy-boto3-trustedadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TrustedAdvisorPublicAPI 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI)
+[boto3.TrustedAdvisorPublicAPI 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-trustedadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,18 +323,18 @@
 `mypy_boto3_trustedadvisor.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `TrustedAdvisorPublicAPI` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/literals/).
 
 ```python
-from mypy_boto3_trustedadvisor.literals import ListChecksPaginatorName
+from mypy_boto3_trustedadvisor.literals import ExclusionStatusType
 
 
-def check_value(value: ListChecksPaginatorName) -> bool: ...
+def check_value(value: ExclusionStatusType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_trustedadvisor.type_defs` module contains structures and shapes
```

### Comparing `mypy-boto3-trustedadvisor-1.34.0/README.md` & `mypy_boto3_trustedadvisor-1.34.94/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-trustedadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-trustedadvisor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-trustedadvisor)](https://pepy.tech/project/mypy-boto3-trustedadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TrustedAdvisorPublicAPI 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI)
+[boto3.TrustedAdvisorPublicAPI 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-trustedadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,18 +290,18 @@
 `mypy_boto3_trustedadvisor.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `TrustedAdvisorPublicAPI` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/literals/).
 
 ```python
-from mypy_boto3_trustedadvisor.literals import ListChecksPaginatorName
+from mypy_boto3_trustedadvisor.literals import ExclusionStatusType
 
 
-def check_value(value: ListChecksPaginatorName) -> bool: ...
+def check_value(value: ExclusionStatusType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_trustedadvisor.type_defs` module contains structures and shapes
```

### Comparing `mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/__init__.py` & `mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListOrganizationRecommendationsPaginator,
     ListRecommendationResourcesPaginator,
     ListRecommendationsPaginator,
 )
 
 Client = TrustedAdvisorPublicAPIClient
 
-
 __all__ = (
     "Client",
     "ListChecksPaginator",
     "ListOrganizationRecommendationAccountsPaginator",
     "ListOrganizationRecommendationResourcesPaginator",
     "ListOrganizationRecommendationsPaginator",
     "ListRecommendationResourcesPaginator",
```

### Comparing `mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/__init__.pyi` & `mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/__main__.py` & `mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TrustedAdvisorPublicAPI 1.34.0\nVersion:        "
-        " 1.34.0\nBuilder version: 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.TrustedAdvisorPublicAPI 1.34.94\n"
+        "Version:         1.34.94\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.94")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/client.py` & `mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 
     session = Session()
     client: TrustedAdvisorPublicAPIClient = session.client("trustedadvisor")
     ```
 """
 
 import sys
-from typing import Any, Dict, Mapping, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    ExclusionStatusType,
     RecommendationLanguageType,
     RecommendationPillarType,
     RecommendationSourceType,
     RecommendationStatusType,
     RecommendationTypeType,
     ResourceStatusType,
     UpdateRecommendationLifecycleStageReasonCodeType,
@@ -34,32 +35,33 @@
     ListOrganizationRecommendationAccountsPaginator,
     ListOrganizationRecommendationResourcesPaginator,
     ListOrganizationRecommendationsPaginator,
     ListRecommendationResourcesPaginator,
     ListRecommendationsPaginator,
 )
 from .type_defs import (
+    BatchUpdateRecommendationResourceExclusionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetOrganizationRecommendationResponseTypeDef,
     GetRecommendationResponseTypeDef,
     ListChecksResponseTypeDef,
     ListOrganizationRecommendationAccountsResponseTypeDef,
     ListOrganizationRecommendationResourcesResponseTypeDef,
     ListOrganizationRecommendationsResponseTypeDef,
     ListRecommendationResourcesResponseTypeDef,
     ListRecommendationsResponseTypeDef,
+    RecommendationResourceExclusionTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("TrustedAdvisorPublicAPIClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -90,14 +92,26 @@
         """
         TrustedAdvisorPublicAPIClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#exceptions)
         """
 
+    def batch_update_recommendation_resource_exclusion(
+        self, *, recommendationResourceExclusions: Sequence[RecommendationResourceExclusionTypeDef]
+    ) -> BatchUpdateRecommendationResourceExclusionResponseTypeDef:
+        """
+        Update one or more exclusion status for a list of recommendation resources See
+        also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/trustedadvisor-2022-09-15/BatchUpdateRecommendationResourceExclusion).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.batch_update_recommendation_resource_exclusion)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#batch_update_recommendation_resource_exclusion)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#can_paginate)
         """
@@ -149,15 +163,15 @@
         self,
         *,
         awsService: str = ...,
         language: RecommendationLanguageType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         pillar: RecommendationPillarType = ...,
-        source: RecommendationSourceType = ...
+        source: RecommendationSourceType = ...,
     ) -> ListChecksResponseTypeDef:
         """
         List a filterable set of Checks See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/trustedadvisor-2022-09-15/ListChecks).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_checks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#list_checks)
@@ -165,33 +179,34 @@
 
     def list_organization_recommendation_accounts(
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListOrganizationRecommendationAccountsResponseTypeDef:
         """
         Lists the accounts that own the resources for an organization aggregate
         recommendation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_organization_recommendation_accounts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#list_organization_recommendation_accounts)
         """
 
     def list_organization_recommendation_resources(
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
+        exclusionStatus: ExclusionStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         regionCode: str = ...,
-        status: ResourceStatusType = ...
+        status: ResourceStatusType = ...,
     ) -> ListOrganizationRecommendationResourcesResponseTypeDef:
         """
         List Resources of a Recommendation within an Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_organization_recommendation_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#list_organization_recommendation_resources)
         """
@@ -204,31 +219,32 @@
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
-        type: RecommendationTypeType = ...
+        type: RecommendationTypeType = ...,
     ) -> ListOrganizationRecommendationsResponseTypeDef:
         """
         List a filterable set of Recommendations within an Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_organization_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#list_organization_recommendations)
         """
 
     def list_recommendation_resources(
         self,
         *,
         recommendationIdentifier: str,
+        exclusionStatus: ExclusionStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         regionCode: str = ...,
-        status: ResourceStatusType = ...
+        status: ResourceStatusType = ...,
     ) -> ListRecommendationResourcesResponseTypeDef:
         """
         List Resources of a Recommendation See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/trustedadvisor-2022-09-15/ListRecommendationResources).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_recommendation_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#list_recommendation_resources)
@@ -242,15 +258,15 @@
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
-        type: RecommendationTypeType = ...
+        type: RecommendationTypeType = ...,
     ) -> ListRecommendationsResponseTypeDef:
         """
         List a filterable set of Recommendations See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/trustedadvisor-2022-09-15/ListRecommendations).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#list_recommendations)
@@ -258,30 +274,30 @@
 
     def update_organization_recommendation_lifecycle(
         self,
         *,
         lifecycleStage: UpdateRecommendationLifecycleStageType,
         organizationRecommendationIdentifier: str,
         updateReason: str = ...,
-        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...
+        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Update the lifecyle of a Recommendation within an Organization.
+        Update the lifecycle of a Recommendation within an Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.update_organization_recommendation_lifecycle)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#update_organization_recommendation_lifecycle)
         """
 
     def update_recommendation_lifecycle(
         self,
         *,
         lifecycleStage: UpdateRecommendationLifecycleStageType,
         recommendationIdentifier: str,
         updateReason: str = ...,
-        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...
+        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Update the lifecyle of a Recommendation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.update_recommendation_lifecycle)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#update_recommendation_lifecycle)
         """
```

### Comparing `mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/client.pyi` & `mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 
     session = Session()
     client: TrustedAdvisorPublicAPIClient = session.client("trustedadvisor")
     ```
 """
 
 import sys
-from typing import Any, Dict, Mapping, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    ExclusionStatusType,
     RecommendationLanguageType,
     RecommendationPillarType,
     RecommendationSourceType,
     RecommendationStatusType,
     RecommendationTypeType,
     ResourceStatusType,
     UpdateRecommendationLifecycleStageReasonCodeType,
@@ -34,23 +35,25 @@
     ListOrganizationRecommendationAccountsPaginator,
     ListOrganizationRecommendationResourcesPaginator,
     ListOrganizationRecommendationsPaginator,
     ListRecommendationResourcesPaginator,
     ListRecommendationsPaginator,
 )
 from .type_defs import (
+    BatchUpdateRecommendationResourceExclusionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetOrganizationRecommendationResponseTypeDef,
     GetRecommendationResponseTypeDef,
     ListChecksResponseTypeDef,
     ListOrganizationRecommendationAccountsResponseTypeDef,
     ListOrganizationRecommendationResourcesResponseTypeDef,
     ListOrganizationRecommendationsResponseTypeDef,
     ListRecommendationResourcesResponseTypeDef,
     ListRecommendationsResponseTypeDef,
+    RecommendationResourceExclusionTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -86,14 +89,26 @@
         """
         TrustedAdvisorPublicAPIClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#exceptions)
         """
 
+    def batch_update_recommendation_resource_exclusion(
+        self, *, recommendationResourceExclusions: Sequence[RecommendationResourceExclusionTypeDef]
+    ) -> BatchUpdateRecommendationResourceExclusionResponseTypeDef:
+        """
+        Update one or more exclusion status for a list of recommendation resources See
+        also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/trustedadvisor-2022-09-15/BatchUpdateRecommendationResourceExclusion).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.batch_update_recommendation_resource_exclusion)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#batch_update_recommendation_resource_exclusion)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#can_paginate)
         """
@@ -145,15 +160,15 @@
         self,
         *,
         awsService: str = ...,
         language: RecommendationLanguageType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         pillar: RecommendationPillarType = ...,
-        source: RecommendationSourceType = ...
+        source: RecommendationSourceType = ...,
     ) -> ListChecksResponseTypeDef:
         """
         List a filterable set of Checks See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/trustedadvisor-2022-09-15/ListChecks).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_checks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#list_checks)
@@ -161,33 +176,34 @@
 
     def list_organization_recommendation_accounts(
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListOrganizationRecommendationAccountsResponseTypeDef:
         """
         Lists the accounts that own the resources for an organization aggregate
         recommendation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_organization_recommendation_accounts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#list_organization_recommendation_accounts)
         """
 
     def list_organization_recommendation_resources(
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
+        exclusionStatus: ExclusionStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         regionCode: str = ...,
-        status: ResourceStatusType = ...
+        status: ResourceStatusType = ...,
     ) -> ListOrganizationRecommendationResourcesResponseTypeDef:
         """
         List Resources of a Recommendation within an Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_organization_recommendation_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#list_organization_recommendation_resources)
         """
@@ -200,31 +216,32 @@
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
-        type: RecommendationTypeType = ...
+        type: RecommendationTypeType = ...,
     ) -> ListOrganizationRecommendationsResponseTypeDef:
         """
         List a filterable set of Recommendations within an Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_organization_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#list_organization_recommendations)
         """
 
     def list_recommendation_resources(
         self,
         *,
         recommendationIdentifier: str,
+        exclusionStatus: ExclusionStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         regionCode: str = ...,
-        status: ResourceStatusType = ...
+        status: ResourceStatusType = ...,
     ) -> ListRecommendationResourcesResponseTypeDef:
         """
         List Resources of a Recommendation See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/trustedadvisor-2022-09-15/ListRecommendationResources).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_recommendation_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#list_recommendation_resources)
@@ -238,15 +255,15 @@
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
-        type: RecommendationTypeType = ...
+        type: RecommendationTypeType = ...,
     ) -> ListRecommendationsResponseTypeDef:
         """
         List a filterable set of Recommendations See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/trustedadvisor-2022-09-15/ListRecommendations).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.list_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#list_recommendations)
@@ -254,30 +271,30 @@
 
     def update_organization_recommendation_lifecycle(
         self,
         *,
         lifecycleStage: UpdateRecommendationLifecycleStageType,
         organizationRecommendationIdentifier: str,
         updateReason: str = ...,
-        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...
+        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Update the lifecyle of a Recommendation within an Organization.
+        Update the lifecycle of a Recommendation within an Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.update_organization_recommendation_lifecycle)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#update_organization_recommendation_lifecycle)
         """
 
     def update_recommendation_lifecycle(
         self,
         *,
         lifecycleStage: UpdateRecommendationLifecycleStageType,
         recommendationIdentifier: str,
         updateReason: str = ...,
-        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...
+        updateReasonCode: UpdateRecommendationLifecycleStageReasonCodeType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Update the lifecyle of a Recommendation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Client.update_recommendation_lifecycle)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/client/#update_recommendation_lifecycle)
         """
```

### Comparing `mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/literals.py` & `mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 Type annotations for trustedadvisor service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_trustedadvisor.literals import ListChecksPaginatorName
+    from mypy_boto3_trustedadvisor.literals import ExclusionStatusType
 
-    data: ListChecksPaginatorName = "list_checks"
+    data: ExclusionStatusType = "excluded"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
+    "ExclusionStatusType",
     "ListChecksPaginatorName",
     "ListOrganizationRecommendationAccountsPaginatorName",
     "ListOrganizationRecommendationResourcesPaginatorName",
     "ListOrganizationRecommendationsPaginatorName",
     "ListRecommendationResourcesPaginatorName",
     "ListRecommendationsPaginatorName",
     "RecommendationLanguageType",
@@ -38,15 +38,15 @@
     "UpdateRecommendationLifecycleStageType",
     "TrustedAdvisorPublicAPIServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
+ExclusionStatusType = Literal["excluded", "included"]
 ListChecksPaginatorName = Literal["list_checks"]
 ListOrganizationRecommendationAccountsPaginatorName = Literal[
     "list_organization_recommendation_accounts"
 ]
 ListOrganizationRecommendationResourcesPaginatorName = Literal[
     "list_organization_recommendation_resources"
 ]
@@ -120,14 +120,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -138,14 +139,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -163,14 +165,15 @@
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
@@ -183,24 +186,26 @@
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
@@ -261,15 +266,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -341,17 +345,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -396,14 +402,15 @@
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
@@ -441,19 +448,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/literals.pyi` & `mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 Type annotations for trustedadvisor service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_trustedadvisor.literals import ListChecksPaginatorName
+    from mypy_boto3_trustedadvisor.literals import ExclusionStatusType
 
-    data: ListChecksPaginatorName = "list_checks"
+    data: ExclusionStatusType = "excluded"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "ExclusionStatusType",
     "ListChecksPaginatorName",
     "ListOrganizationRecommendationAccountsPaginatorName",
     "ListOrganizationRecommendationResourcesPaginatorName",
     "ListOrganizationRecommendationsPaginatorName",
     "ListRecommendationResourcesPaginatorName",
     "ListRecommendationsPaginatorName",
     "RecommendationLanguageType",
@@ -37,14 +38,15 @@
     "UpdateRecommendationLifecycleStageType",
     "TrustedAdvisorPublicAPIServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+ExclusionStatusType = Literal["excluded", "included"]
 ListChecksPaginatorName = Literal["list_checks"]
 ListOrganizationRecommendationAccountsPaginatorName = Literal[
     "list_organization_recommendation_accounts"
 ]
 ListOrganizationRecommendationResourcesPaginatorName = Literal[
     "list_organization_recommendation_resources"
 ]
@@ -118,14 +120,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -136,14 +139,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -161,14 +165,15 @@
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
@@ -181,24 +186,26 @@
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
@@ -259,15 +266,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -339,17 +345,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -394,14 +402,15 @@
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
@@ -439,19 +448,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/paginator.py` & `mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/paginator.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
+    ExclusionStatusType,
     RecommendationLanguageType,
     RecommendationPillarType,
     RecommendationSourceType,
     RecommendationStatusType,
     RecommendationTypeType,
     ResourceStatusType,
 )
@@ -58,86 +59,81 @@
     "ListOrganizationRecommendationAccountsPaginator",
     "ListOrganizationRecommendationResourcesPaginator",
     "ListOrganizationRecommendationsPaginator",
     "ListRecommendationResourcesPaginator",
     "ListRecommendationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListChecksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListChecks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listcheckspaginator)
     """
 
     def paginate(
         self,
         *,
         awsService: str = ...,
         language: RecommendationLanguageType = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListChecks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listcheckspaginator)
         """
 
-
 class ListOrganizationRecommendationAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendationAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listorganizationrecommendationaccountspaginator)
     """
 
     def paginate(
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListOrganizationRecommendationAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendationAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listorganizationrecommendationaccountspaginator)
         """
 
-
 class ListOrganizationRecommendationResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendationResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listorganizationrecommendationresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
+        exclusionStatus: ExclusionStatusType = ...,
         regionCode: str = ...,
         status: ResourceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListOrganizationRecommendationResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendationResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listorganizationrecommendationresourcespaginator)
         """
 
-
 class ListOrganizationRecommendationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listorganizationrecommendationspaginator)
     """
 
     def paginate(
@@ -147,42 +143,41 @@
         awsService: str = ...,
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
         type: RecommendationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListOrganizationRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listorganizationrecommendationspaginator)
         """
 
-
 class ListRecommendationResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListRecommendationResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listrecommendationresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         recommendationIdentifier: str,
+        exclusionStatus: ExclusionStatusType = ...,
         regionCode: str = ...,
         status: ResourceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListRecommendationResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListRecommendationResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listrecommendationresourcespaginator)
         """
 
-
 class ListRecommendationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListRecommendations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listrecommendationspaginator)
     """
 
     def paginate(
@@ -192,13 +187,13 @@
         awsService: str = ...,
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
         type: RecommendationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListRecommendations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listrecommendationspaginator)
         """
```

### Comparing `mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/paginator.pyi` & `mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/paginator.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
+    ExclusionStatusType,
     RecommendationLanguageType,
     RecommendationPillarType,
     RecommendationSourceType,
     RecommendationStatusType,
     RecommendationTypeType,
     ResourceStatusType,
 )
@@ -60,78 +61,84 @@
     "ListOrganizationRecommendationsPaginator",
     "ListRecommendationResourcesPaginator",
     "ListRecommendationsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListChecksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListChecks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listcheckspaginator)
     """
 
     def paginate(
         self,
         *,
         awsService: str = ...,
         language: RecommendationLanguageType = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListChecks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listcheckspaginator)
         """
 
+
 class ListOrganizationRecommendationAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendationAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listorganizationrecommendationaccountspaginator)
     """
 
     def paginate(
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListOrganizationRecommendationAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendationAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listorganizationrecommendationaccountspaginator)
         """
 
+
 class ListOrganizationRecommendationResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendationResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listorganizationrecommendationresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         organizationRecommendationIdentifier: str,
         affectedAccountId: str = ...,
+        exclusionStatus: ExclusionStatusType = ...,
         regionCode: str = ...,
         status: ResourceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListOrganizationRecommendationResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendationResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listorganizationrecommendationresourcespaginator)
         """
 
+
 class ListOrganizationRecommendationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listorganizationrecommendationspaginator)
     """
 
     def paginate(
@@ -141,40 +148,43 @@
         awsService: str = ...,
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
         type: RecommendationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListOrganizationRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listorganizationrecommendationspaginator)
         """
 
+
 class ListRecommendationResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListRecommendationResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listrecommendationresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         recommendationIdentifier: str,
+        exclusionStatus: ExclusionStatusType = ...,
         regionCode: str = ...,
         status: ResourceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListRecommendationResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListRecommendationResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listrecommendationresourcespaginator)
         """
 
+
 class ListRecommendationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListRecommendations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listrecommendationspaginator)
     """
 
     def paginate(
@@ -184,13 +194,13 @@
         awsService: str = ...,
         beforeLastUpdatedAt: TimestampTypeDef = ...,
         checkIdentifier: str = ...,
         pillar: RecommendationPillarType = ...,
         source: RecommendationSourceType = ...,
         status: RecommendationStatusType = ...,
         type: RecommendationTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI.Paginator.ListRecommendations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/paginators/#listrecommendationspaginator)
         """
```

### Comparing `mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/type_defs.py` & `mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 
     data: AccountRecommendationLifecycleSummaryTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Union
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
+    ExclusionStatusType,
     RecommendationLanguageType,
     RecommendationLifecycleStageType,
     RecommendationPillarType,
     RecommendationSourceType,
     RecommendationStatusType,
     RecommendationTypeType,
     ResourceStatusType,
@@ -33,36 +34,39 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountRecommendationLifecycleSummaryTypeDef",
-    "CheckSummaryTypeDef",
+    "RecommendationResourceExclusionTypeDef",
     "ResponseMetadataTypeDef",
+    "UpdateRecommendationResourceExclusionErrorTypeDef",
+    "CheckSummaryTypeDef",
     "GetOrganizationRecommendationRequestRequestTypeDef",
     "GetRecommendationRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListChecksRequestRequestTypeDef",
     "ListOrganizationRecommendationAccountsRequestRequestTypeDef",
     "ListOrganizationRecommendationResourcesRequestRequestTypeDef",
     "OrganizationRecommendationResourceSummaryTypeDef",
     "TimestampTypeDef",
     "ListRecommendationResourcesRequestRequestTypeDef",
     "RecommendationResourceSummaryTypeDef",
     "RecommendationResourcesAggregatesTypeDef",
     "RecommendationCostOptimizingAggregatesTypeDef",
     "UpdateOrganizationRecommendationLifecycleRequestRequestTypeDef",
     "UpdateRecommendationLifecycleRequestRequestTypeDef",
+    "BatchUpdateRecommendationResourceExclusionRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "ListChecksResponseTypeDef",
     "ListOrganizationRecommendationAccountsResponseTypeDef",
+    "BatchUpdateRecommendationResourceExclusionResponseTypeDef",
+    "ListChecksResponseTypeDef",
     "ListChecksRequestListChecksPaginateTypeDef",
     "ListOrganizationRecommendationAccountsRequestListOrganizationRecommendationAccountsPaginateTypeDef",
     "ListOrganizationRecommendationResourcesRequestListOrganizationRecommendationResourcesPaginateTypeDef",
     "ListRecommendationResourcesRequestListRecommendationResourcesPaginateTypeDef",
     "ListOrganizationRecommendationResourcesResponseTypeDef",
     "ListOrganizationRecommendationsRequestListOrganizationRecommendationsPaginateTypeDef",
     "ListOrganizationRecommendationsRequestRequestTypeDef",
@@ -89,35 +93,50 @@
         "lifecycleStage": NotRequired[RecommendationLifecycleStageType],
         "updateReason": NotRequired[str],
         "updateReasonCode": NotRequired[UpdateRecommendationLifecycleStageReasonCodeType],
         "updatedOnBehalfOf": NotRequired[str],
         "updatedOnBehalfOfJobTitle": NotRequired[str],
     },
 )
-CheckSummaryTypeDef = TypedDict(
-    "CheckSummaryTypeDef",
+RecommendationResourceExclusionTypeDef = TypedDict(
+    "RecommendationResourceExclusionTypeDef",
     {
         "arn": str,
-        "awsServices": List[str],
-        "description": str,
-        "id": str,
-        "metadata": Dict[str, str],
-        "name": str,
-        "pillars": List[RecommendationPillarType],
-        "source": RecommendationSourceType,
+        "isExcluded": bool,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
+    },
+)
+UpdateRecommendationResourceExclusionErrorTypeDef = TypedDict(
+    "UpdateRecommendationResourceExclusionErrorTypeDef",
+    {
+        "arn": NotRequired[str],
+        "errorCode": NotRequired[str],
+        "errorMessage": NotRequired[str],
+    },
+)
+CheckSummaryTypeDef = TypedDict(
+    "CheckSummaryTypeDef",
+    {
+        "arn": str,
+        "awsServices": List[str],
+        "description": str,
+        "id": str,
+        "metadata": Dict[str, str],
+        "name": str,
+        "pillars": List[RecommendationPillarType],
+        "source": RecommendationSourceType,
     },
 )
 GetOrganizationRecommendationRequestRequestTypeDef = TypedDict(
     "GetOrganizationRecommendationRequestRequestTypeDef",
     {
         "organizationRecommendationIdentifier": str,
     },
@@ -157,14 +176,15 @@
     },
 )
 ListOrganizationRecommendationResourcesRequestRequestTypeDef = TypedDict(
     "ListOrganizationRecommendationResourcesRequestRequestTypeDef",
     {
         "organizationRecommendationIdentifier": str,
         "affectedAccountId": NotRequired[str],
+        "exclusionStatus": NotRequired[ExclusionStatusType],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
         "regionCode": NotRequired[str],
         "status": NotRequired[ResourceStatusType],
     },
 )
 OrganizationRecommendationResourceSummaryTypeDef = TypedDict(
@@ -175,21 +195,23 @@
         "id": str,
         "lastUpdatedAt": datetime,
         "metadata": Dict[str, str],
         "recommendationArn": str,
         "regionCode": str,
         "status": ResourceStatusType,
         "accountId": NotRequired[str],
+        "exclusionStatus": NotRequired[ExclusionStatusType],
     },
 )
 TimestampTypeDef = Union[datetime, str]
 ListRecommendationResourcesRequestRequestTypeDef = TypedDict(
     "ListRecommendationResourcesRequestRequestTypeDef",
     {
         "recommendationIdentifier": str,
+        "exclusionStatus": NotRequired[ExclusionStatusType],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
         "regionCode": NotRequired[str],
         "status": NotRequired[ResourceStatusType],
     },
 )
 RecommendationResourceSummaryTypeDef = TypedDict(
@@ -199,14 +221,15 @@
         "awsResourceId": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "metadata": Dict[str, str],
         "recommendationArn": str,
         "regionCode": str,
         "status": ResourceStatusType,
+        "exclusionStatus": NotRequired[ExclusionStatusType],
     },
 )
 RecommendationResourcesAggregatesTypeDef = TypedDict(
     "RecommendationResourcesAggregatesTypeDef",
     {
         "errorCount": int,
         "okCount": int,
@@ -234,38 +257,53 @@
     {
         "lifecycleStage": UpdateRecommendationLifecycleStageType,
         "recommendationIdentifier": str,
         "updateReason": NotRequired[str],
         "updateReasonCode": NotRequired[UpdateRecommendationLifecycleStageReasonCodeType],
     },
 )
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+BatchUpdateRecommendationResourceExclusionRequestRequestTypeDef = TypedDict(
+    "BatchUpdateRecommendationResourceExclusionRequestRequestTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "recommendationResourceExclusions": Sequence[RecommendationResourceExclusionTypeDef],
     },
 )
-ListChecksResponseTypeDef = TypedDict(
-    "ListChecksResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "checkSummaries": List[CheckSummaryTypeDef],
-        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListOrganizationRecommendationAccountsResponseTypeDef = TypedDict(
     "ListOrganizationRecommendationAccountsResponseTypeDef",
     {
         "accountRecommendationLifecycleSummaries": List[
             AccountRecommendationLifecycleSummaryTypeDef
         ],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+BatchUpdateRecommendationResourceExclusionResponseTypeDef = TypedDict(
+    "BatchUpdateRecommendationResourceExclusionResponseTypeDef",
+    {
+        "batchUpdateRecommendationResourceExclusionErrors": List[
+            UpdateRecommendationResourceExclusionErrorTypeDef
+        ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListChecksResponseTypeDef = TypedDict(
+    "ListChecksResponseTypeDef",
+    {
+        "checkSummaries": List[CheckSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListChecksRequestListChecksPaginateTypeDef = TypedDict(
     "ListChecksRequestListChecksPaginateTypeDef",
     {
         "awsService": NotRequired[str],
         "language": NotRequired[RecommendationLanguageType],
         "pillar": NotRequired[RecommendationPillarType],
         "source": NotRequired[RecommendationSourceType],
@@ -281,23 +319,25 @@
     },
 )
 ListOrganizationRecommendationResourcesRequestListOrganizationRecommendationResourcesPaginateTypeDef = TypedDict(
     "ListOrganizationRecommendationResourcesRequestListOrganizationRecommendationResourcesPaginateTypeDef",
     {
         "organizationRecommendationIdentifier": str,
         "affectedAccountId": NotRequired[str],
+        "exclusionStatus": NotRequired[ExclusionStatusType],
         "regionCode": NotRequired[str],
         "status": NotRequired[ResourceStatusType],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListRecommendationResourcesRequestListRecommendationResourcesPaginateTypeDef = TypedDict(
     "ListRecommendationResourcesRequestListRecommendationResourcesPaginateTypeDef",
     {
         "recommendationIdentifier": str,
+        "exclusionStatus": NotRequired[ExclusionStatusType],
         "regionCode": NotRequired[str],
         "status": NotRequired[ResourceStatusType],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListOrganizationRecommendationResourcesResponseTypeDef = TypedDict(
     "ListOrganizationRecommendationResourcesResponseTypeDef",
```

### Comparing `mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor/type_defs.pyi` & `mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 
     data: AccountRecommendationLifecycleSummaryTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Union
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
+    ExclusionStatusType,
     RecommendationLanguageType,
     RecommendationLifecycleStageType,
     RecommendationPillarType,
     RecommendationSourceType,
     RecommendationStatusType,
     RecommendationTypeType,
     ResourceStatusType,
@@ -35,33 +36,37 @@
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountRecommendationLifecycleSummaryTypeDef",
-    "CheckSummaryTypeDef",
+    "RecommendationResourceExclusionTypeDef",
     "ResponseMetadataTypeDef",
+    "UpdateRecommendationResourceExclusionErrorTypeDef",
+    "CheckSummaryTypeDef",
     "GetOrganizationRecommendationRequestRequestTypeDef",
     "GetRecommendationRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListChecksRequestRequestTypeDef",
     "ListOrganizationRecommendationAccountsRequestRequestTypeDef",
     "ListOrganizationRecommendationResourcesRequestRequestTypeDef",
     "OrganizationRecommendationResourceSummaryTypeDef",
     "TimestampTypeDef",
     "ListRecommendationResourcesRequestRequestTypeDef",
     "RecommendationResourceSummaryTypeDef",
     "RecommendationResourcesAggregatesTypeDef",
     "RecommendationCostOptimizingAggregatesTypeDef",
     "UpdateOrganizationRecommendationLifecycleRequestRequestTypeDef",
     "UpdateRecommendationLifecycleRequestRequestTypeDef",
+    "BatchUpdateRecommendationResourceExclusionRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "ListChecksResponseTypeDef",
     "ListOrganizationRecommendationAccountsResponseTypeDef",
+    "BatchUpdateRecommendationResourceExclusionResponseTypeDef",
+    "ListChecksResponseTypeDef",
     "ListChecksRequestListChecksPaginateTypeDef",
     "ListOrganizationRecommendationAccountsRequestListOrganizationRecommendationAccountsPaginateTypeDef",
     "ListOrganizationRecommendationResourcesRequestListOrganizationRecommendationResourcesPaginateTypeDef",
     "ListRecommendationResourcesRequestListRecommendationResourcesPaginateTypeDef",
     "ListOrganizationRecommendationResourcesResponseTypeDef",
     "ListOrganizationRecommendationsRequestListOrganizationRecommendationsPaginateTypeDef",
     "ListOrganizationRecommendationsRequestRequestTypeDef",
@@ -88,35 +93,50 @@
         "lifecycleStage": NotRequired[RecommendationLifecycleStageType],
         "updateReason": NotRequired[str],
         "updateReasonCode": NotRequired[UpdateRecommendationLifecycleStageReasonCodeType],
         "updatedOnBehalfOf": NotRequired[str],
         "updatedOnBehalfOfJobTitle": NotRequired[str],
     },
 )
-CheckSummaryTypeDef = TypedDict(
-    "CheckSummaryTypeDef",
+RecommendationResourceExclusionTypeDef = TypedDict(
+    "RecommendationResourceExclusionTypeDef",
     {
         "arn": str,
-        "awsServices": List[str],
-        "description": str,
-        "id": str,
-        "metadata": Dict[str, str],
-        "name": str,
-        "pillars": List[RecommendationPillarType],
-        "source": RecommendationSourceType,
+        "isExcluded": bool,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
+    },
+)
+UpdateRecommendationResourceExclusionErrorTypeDef = TypedDict(
+    "UpdateRecommendationResourceExclusionErrorTypeDef",
+    {
+        "arn": NotRequired[str],
+        "errorCode": NotRequired[str],
+        "errorMessage": NotRequired[str],
+    },
+)
+CheckSummaryTypeDef = TypedDict(
+    "CheckSummaryTypeDef",
+    {
+        "arn": str,
+        "awsServices": List[str],
+        "description": str,
+        "id": str,
+        "metadata": Dict[str, str],
+        "name": str,
+        "pillars": List[RecommendationPillarType],
+        "source": RecommendationSourceType,
     },
 )
 GetOrganizationRecommendationRequestRequestTypeDef = TypedDict(
     "GetOrganizationRecommendationRequestRequestTypeDef",
     {
         "organizationRecommendationIdentifier": str,
     },
@@ -156,14 +176,15 @@
     },
 )
 ListOrganizationRecommendationResourcesRequestRequestTypeDef = TypedDict(
     "ListOrganizationRecommendationResourcesRequestRequestTypeDef",
     {
         "organizationRecommendationIdentifier": str,
         "affectedAccountId": NotRequired[str],
+        "exclusionStatus": NotRequired[ExclusionStatusType],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
         "regionCode": NotRequired[str],
         "status": NotRequired[ResourceStatusType],
     },
 )
 OrganizationRecommendationResourceSummaryTypeDef = TypedDict(
@@ -174,21 +195,23 @@
         "id": str,
         "lastUpdatedAt": datetime,
         "metadata": Dict[str, str],
         "recommendationArn": str,
         "regionCode": str,
         "status": ResourceStatusType,
         "accountId": NotRequired[str],
+        "exclusionStatus": NotRequired[ExclusionStatusType],
     },
 )
 TimestampTypeDef = Union[datetime, str]
 ListRecommendationResourcesRequestRequestTypeDef = TypedDict(
     "ListRecommendationResourcesRequestRequestTypeDef",
     {
         "recommendationIdentifier": str,
+        "exclusionStatus": NotRequired[ExclusionStatusType],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
         "regionCode": NotRequired[str],
         "status": NotRequired[ResourceStatusType],
     },
 )
 RecommendationResourceSummaryTypeDef = TypedDict(
@@ -198,14 +221,15 @@
         "awsResourceId": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "metadata": Dict[str, str],
         "recommendationArn": str,
         "regionCode": str,
         "status": ResourceStatusType,
+        "exclusionStatus": NotRequired[ExclusionStatusType],
     },
 )
 RecommendationResourcesAggregatesTypeDef = TypedDict(
     "RecommendationResourcesAggregatesTypeDef",
     {
         "errorCount": int,
         "okCount": int,
@@ -233,38 +257,53 @@
     {
         "lifecycleStage": UpdateRecommendationLifecycleStageType,
         "recommendationIdentifier": str,
         "updateReason": NotRequired[str],
         "updateReasonCode": NotRequired[UpdateRecommendationLifecycleStageReasonCodeType],
     },
 )
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+BatchUpdateRecommendationResourceExclusionRequestRequestTypeDef = TypedDict(
+    "BatchUpdateRecommendationResourceExclusionRequestRequestTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "recommendationResourceExclusions": Sequence[RecommendationResourceExclusionTypeDef],
     },
 )
-ListChecksResponseTypeDef = TypedDict(
-    "ListChecksResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "checkSummaries": List[CheckSummaryTypeDef],
-        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListOrganizationRecommendationAccountsResponseTypeDef = TypedDict(
     "ListOrganizationRecommendationAccountsResponseTypeDef",
     {
         "accountRecommendationLifecycleSummaries": List[
             AccountRecommendationLifecycleSummaryTypeDef
         ],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+BatchUpdateRecommendationResourceExclusionResponseTypeDef = TypedDict(
+    "BatchUpdateRecommendationResourceExclusionResponseTypeDef",
+    {
+        "batchUpdateRecommendationResourceExclusionErrors": List[
+            UpdateRecommendationResourceExclusionErrorTypeDef
+        ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListChecksResponseTypeDef = TypedDict(
+    "ListChecksResponseTypeDef",
+    {
+        "checkSummaries": List[CheckSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListChecksRequestListChecksPaginateTypeDef = TypedDict(
     "ListChecksRequestListChecksPaginateTypeDef",
     {
         "awsService": NotRequired[str],
         "language": NotRequired[RecommendationLanguageType],
         "pillar": NotRequired[RecommendationPillarType],
         "source": NotRequired[RecommendationSourceType],
@@ -280,23 +319,25 @@
     },
 )
 ListOrganizationRecommendationResourcesRequestListOrganizationRecommendationResourcesPaginateTypeDef = TypedDict(
     "ListOrganizationRecommendationResourcesRequestListOrganizationRecommendationResourcesPaginateTypeDef",
     {
         "organizationRecommendationIdentifier": str,
         "affectedAccountId": NotRequired[str],
+        "exclusionStatus": NotRequired[ExclusionStatusType],
         "regionCode": NotRequired[str],
         "status": NotRequired[ResourceStatusType],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListRecommendationResourcesRequestListRecommendationResourcesPaginateTypeDef = TypedDict(
     "ListRecommendationResourcesRequestListRecommendationResourcesPaginateTypeDef",
     {
         "recommendationIdentifier": str,
+        "exclusionStatus": NotRequired[ExclusionStatusType],
         "regionCode": NotRequired[str],
         "status": NotRequired[ResourceStatusType],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListOrganizationRecommendationResourcesResponseTypeDef = TypedDict(
     "ListOrganizationRecommendationResourcesResponseTypeDef",
```

### Comparing `mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor.egg-info/PKG-INFO` & `mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-trustedadvisor
-Version: 1.34.0
-Summary: Type annotations for boto3.TrustedAdvisorPublicAPI 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.94
+Summary: Type annotations for boto3.TrustedAdvisorPublicAPI 1.34.94 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-trustedadvisor"></a>
 
 # mypy-boto3-trustedadvisor
 
 [![PyPI - mypy-boto3-trustedadvisor](https://img.shields.io/pypi/v/mypy-boto3-trustedadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-trustedadvisor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-trustedadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-trustedadvisor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-trustedadvisor)](https://pepy.tech/project/mypy-boto3-trustedadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TrustedAdvisorPublicAPI 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI)
+[boto3.TrustedAdvisorPublicAPI 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#TrustedAdvisorPublicAPI)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-trustedadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,18 +323,18 @@
 `mypy_boto3_trustedadvisor.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `TrustedAdvisorPublicAPI` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/literals/).
 
 ```python
-from mypy_boto3_trustedadvisor.literals import ListChecksPaginatorName
+from mypy_boto3_trustedadvisor.literals import ExclusionStatusType
 
 
-def check_value(value: ListChecksPaginatorName) -> bool: ...
+def check_value(value: ExclusionStatusType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_trustedadvisor.type_defs` module contains structures and shapes
```

### Comparing `mypy-boto3-trustedadvisor-1.34.0/mypy_boto3_trustedadvisor.egg-info/SOURCES.txt` & `mypy_boto3_trustedadvisor-1.34.94/mypy_boto3_trustedadvisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-trustedadvisor-1.34.0/setup.py` & `mypy_boto3_trustedadvisor-1.34.94/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-trustedadvisor",
-    version="1.34.0",
+    version="1.34.94",
     packages=["mypy_boto3_trustedadvisor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.TrustedAdvisorPublicAPI 1.34.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.TrustedAdvisorPublicAPI 1.34.94 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 trustedadvisor type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_trustedadvisor": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_trustedadvisor/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

