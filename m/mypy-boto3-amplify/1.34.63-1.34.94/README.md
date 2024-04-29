# Comparing `tmp/mypy-boto3-amplify-1.34.63.tar.gz` & `tmp/mypy_boto3_amplify-1.34.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplify-1.34.63.tar", last modified: Thu Mar 14 19:19:06 2024, max compression
+gzip compressed data, was "mypy_boto3_amplify-1.34.94.tar", last modified: Mon Apr 29 19:32:08 2024, max compression
```

## Comparing `mypy-boto3-amplify-1.34.63.tar` & `mypy_boto3_amplify-1.34.94.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:19:06.242532 mypy-boto3-amplify-1.34.63/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-14 19:18:37.000000 mypy-boto3-amplify-1.34.63/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-03-14 19:19:06.242532 mypy-boto3-amplify-1.34.63/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-03-14 19:18:37.000000 mypy-boto3-amplify-1.34.63/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:19:06.242532 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-14 19:18:37.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-14 19:18:37.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-14 19:18:37.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28198 2024-03-14 19:18:37.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-03-14 19:18:37.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-03-14 19:18:37.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-03-14 19:18:37.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-03-14 19:18:37.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-03-14 19:18:37.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 19:18:37.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    31724 2024-03-14 19:18:38.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    31724 2024-03-14 19:18:38.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-14 19:18:37.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:19:06.242532 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-03-14 19:19:06.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-14 19:19:06.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 19:19:06.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 19:19:06.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-14 19:19:06.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-14 19:19:06.000000 mypy-boto3-amplify-1.34.63/mypy_boto3_amplify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 19:19:06.242532 mypy-boto3-amplify-1.34.63/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-03-14 19:18:37.000000 mypy-boto3-amplify-1.34.63/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:08.314775 mypy_boto3_amplify-1.34.94/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 19:31:46.000000 mypy_boto3_amplify-1.34.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13061 2024-04-29 19:32:08.314775 mypy_boto3_amplify-1.34.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-04-29 19:31:46.000000 mypy_boto3_amplify-1.34.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:08.310775 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-29 19:31:46.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-29 19:31:46.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-29 19:31:46.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28213 2024-04-29 19:31:46.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28210 2024-04-29 19:31:46.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-29 19:31:46.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-29 19:31:46.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-29 19:31:46.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-29 19:31:46.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:31:46.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    31128 2024-04-29 19:31:47.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31128 2024-04-29 19:31:47.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 19:31:46.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:08.314775 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13061 2024-04-29 19:32:08.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-29 19:32:08.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:08.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:08.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 19:32:08.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 19:32:08.000000 mypy_boto3_amplify-1.34.94/mypy_boto3_amplify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:32:08.314775 mypy_boto3_amplify-1.34.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-29 19:31:46.000000 mypy_boto3_amplify-1.34.94/setup.py
```

### Comparing `mypy-boto3-amplify-1.34.63/LICENSE` & `mypy_boto3_amplify-1.34.94/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.34.63/PKG-INFO` & `mypy_boto3_amplify-1.34.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplify
-Version: 1.34.63
-Summary: Type annotations for boto3.Amplify 1.34.63 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.94
+Summary: Type annotations for boto3.Amplify 1.34.94 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplify)](https://pepy.tech/project/mypy-boto3-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Amplify 1.34.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[boto3.Amplify 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,18 +326,18 @@
 `mypy_boto3_amplify.type_defs` module contains structures and shapes assembled
 to typed dictionaries and unions for additional type checking.
 
 Full list of `Amplify` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/type_defs/).
 
 ```python
-from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigPaginatorTypeDef
+from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigOutputTypeDef
 
 
-def get_value() -> AutoBranchCreationConfigPaginatorTypeDef:
+def get_value() -> AutoBranchCreationConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplify-1.34.63/README.md` & `mypy_boto3_amplify-1.34.94/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplify)](https://pepy.tech/project/mypy-boto3-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Amplify 1.34.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[boto3.Amplify 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,18 +293,18 @@
 `mypy_boto3_amplify.type_defs` module contains structures and shapes assembled
 to typed dictionaries and unions for additional type checking.
 
 Full list of `Amplify` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/type_defs/).
 
 ```python
-from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigPaginatorTypeDef
+from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigOutputTypeDef
 
 
-def get_value() -> AutoBranchCreationConfigPaginatorTypeDef:
+def get_value() -> AutoBranchCreationConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/__init__.py` & `mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/__init__.pyi` & `mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/__main__.py` & `mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Amplify 1.34.63\n"
-        "Version:         1.34.63\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.Amplify 1.34.94\n"
+        "Version:         1.34.94\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.63")
+    print("1.34.94")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/client.py` & `mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .paginator import (
     ListAppsPaginator,
     ListBranchesPaginator,
     ListDomainAssociationsPaginator,
     ListJobsPaginator,
 )
 from .type_defs import (
-    AutoBranchCreationConfigTypeDef,
+    AutoBranchCreationConfigUnionTypeDef,
     BackendTypeDef,
     CertificateSettingsTypeDef,
     CreateAppResultTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateDomainAssociationResultTypeDef,
@@ -147,15 +147,15 @@
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...,
+        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...,
     ) -> CreateAppResultTypeDef:
         """
         Creates a new Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/client/#create_app)
         """
@@ -533,15 +533,15 @@
         enableBasicAuth: bool = ...,
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...,
+        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...,
         repository: str = ...,
         oauthToken: str = ...,
         accessToken: str = ...,
     ) -> UpdateAppResultTypeDef:
         """
         Updates an existing Amplify app.
```

### Comparing `mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/client.pyi` & `mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .paginator import (
     ListAppsPaginator,
     ListBranchesPaginator,
     ListDomainAssociationsPaginator,
     ListJobsPaginator,
 )
 from .type_defs import (
-    AutoBranchCreationConfigTypeDef,
+    AutoBranchCreationConfigUnionTypeDef,
     BackendTypeDef,
     CertificateSettingsTypeDef,
     CreateAppResultTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateDomainAssociationResultTypeDef,
@@ -144,15 +144,15 @@
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...,
+        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...,
     ) -> CreateAppResultTypeDef:
         """
         Creates a new Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/client/#create_app)
         """
@@ -530,15 +530,15 @@
         enableBasicAuth: bool = ...,
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...,
+        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...,
         repository: str = ...,
         oauthToken: str = ...,
         accessToken: str = ...,
     ) -> UpdateAppResultTypeDef:
         """
         Updates an existing Amplify app.
```

### Comparing `mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/literals.py` & `mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
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
@@ -160,24 +161,26 @@
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
@@ -374,14 +377,15 @@
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
@@ -467,14 +471,15 @@
     "sqs",
 ]
 PaginatorName = Literal["list_apps", "list_branches", "list_domain_associations", "list_jobs"]
 RegionName = Literal[
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
```

### Comparing `mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/literals.pyi` & `mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
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
@@ -160,24 +161,26 @@
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
@@ -374,14 +377,15 @@
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
@@ -467,14 +471,15 @@
     "sqs",
 ]
 PaginatorName = Literal["list_apps", "list_branches", "list_domain_associations", "list_jobs"]
 RegionName = Literal[
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
```

### Comparing `mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/paginator.py` & `mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    ListAppsResultPaginatorTypeDef,
+    ListAppsResultTypeDef,
     ListBranchesResultTypeDef,
     ListDomainAssociationsResultTypeDef,
     ListJobsResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
@@ -59,15 +59,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Paginator.ListApps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/paginators/#listappspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListAppsResultPaginatorTypeDef]:
+    ) -> _PageIterator[ListAppsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Paginator.ListApps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/paginators/#listappspaginator)
         """
 
 
 class ListBranchesPaginator(Paginator):
```

### Comparing `mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/paginator.pyi` & `mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    ListAppsResultPaginatorTypeDef,
+    ListAppsResultTypeDef,
     ListBranchesResultTypeDef,
     ListDomainAssociationsResultTypeDef,
     ListJobsResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
@@ -57,15 +57,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Paginator.ListApps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/paginators/#listappspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListAppsResultPaginatorTypeDef]:
+    ) -> _PageIterator[ListAppsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Paginator.ListApps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/paginators/#listappspaginator)
         """
 
 class ListBranchesPaginator(Paginator):
     """
```

### Comparing `mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/type_defs.py` & `mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplify service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigPaginatorTypeDef
+    from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigOutputTypeDef
 
-    data: AutoBranchCreationConfigPaginatorTypeDef = ...
+    data: AutoBranchCreationConfigOutputTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
@@ -33,19 +33,20 @@
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AutoBranchCreationConfigPaginatorTypeDef",
+    "AutoBranchCreationConfigOutputTypeDef",
     "CustomRuleTypeDef",
     "ProductionBranchTypeDef",
-    "AutoBranchCreationConfigTypeDef",
     "ArtifactTypeDef",
+    "AutoBranchCreationConfigExtraOutputTypeDef",
+    "AutoBranchCreationConfigTypeDef",
     "BackendEnvironmentTypeDef",
     "BackendTypeDef",
     "CertificateSettingsTypeDef",
     "CertificateTypeDef",
     "ResponseMetadataTypeDef",
     "CreateBackendEnvironmentRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
@@ -78,16 +79,16 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebhooksRequestRequestTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StopJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWebhookRequestRequestTypeDef",
-    "AppPaginatorTypeDef",
     "AppTypeDef",
+    "AutoBranchCreationConfigUnionTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "BranchTypeDef",
     "CreateBranchRequestRequestTypeDef",
     "UpdateBranchRequestRequestTypeDef",
     "CreateBackendEnvironmentResultTypeDef",
     "CreateDeploymentResultTypeDef",
@@ -114,15 +115,14 @@
     "GenerateAccessLogsRequestRequestTypeDef",
     "StartJobRequestRequestTypeDef",
     "JobTypeDef",
     "ListAppsRequestListAppsPaginateTypeDef",
     "ListBranchesRequestListBranchesPaginateTypeDef",
     "ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
-    "ListAppsResultPaginatorTypeDef",
     "CreateAppResultTypeDef",
     "DeleteAppResultTypeDef",
     "GetAppResultTypeDef",
     "ListAppsResultTypeDef",
     "UpdateAppResultTypeDef",
     "CreateBranchResultTypeDef",
     "DeleteBranchResultTypeDef",
@@ -134,16 +134,16 @@
     "CreateDomainAssociationResultTypeDef",
     "DeleteDomainAssociationResultTypeDef",
     "GetDomainAssociationResultTypeDef",
     "ListDomainAssociationsResultTypeDef",
     "UpdateDomainAssociationResultTypeDef",
 )
 
-AutoBranchCreationConfigPaginatorTypeDef = TypedDict(
-    "AutoBranchCreationConfigPaginatorTypeDef",
+AutoBranchCreationConfigOutputTypeDef = TypedDict(
+    "AutoBranchCreationConfigOutputTypeDef",
     {
         "stage": NotRequired[StageType],
         "framework": NotRequired[str],
         "enableAutoBuild": NotRequired[bool],
         "environmentVariables": NotRequired[Dict[str, str]],
         "basicAuthCredentials": NotRequired[str],
         "enableBasicAuth": NotRequired[bool],
@@ -167,34 +167,49 @@
     {
         "lastDeployTime": NotRequired[datetime],
         "status": NotRequired[str],
         "thumbnailUrl": NotRequired[str],
         "branchName": NotRequired[str],
     },
 )
-AutoBranchCreationConfigTypeDef = TypedDict(
-    "AutoBranchCreationConfigTypeDef",
+ArtifactTypeDef = TypedDict(
+    "ArtifactTypeDef",
+    {
+        "artifactFileName": str,
+        "artifactId": str,
+    },
+)
+AutoBranchCreationConfigExtraOutputTypeDef = TypedDict(
+    "AutoBranchCreationConfigExtraOutputTypeDef",
     {
         "stage": NotRequired[StageType],
         "framework": NotRequired[str],
         "enableAutoBuild": NotRequired[bool],
-        "environmentVariables": NotRequired[Mapping[str, str]],
+        "environmentVariables": NotRequired[Dict[str, str]],
         "basicAuthCredentials": NotRequired[str],
         "enableBasicAuth": NotRequired[bool],
         "enablePerformanceMode": NotRequired[bool],
         "buildSpec": NotRequired[str],
         "enablePullRequestPreview": NotRequired[bool],
         "pullRequestEnvironmentName": NotRequired[str],
     },
 )
-ArtifactTypeDef = TypedDict(
-    "ArtifactTypeDef",
+AutoBranchCreationConfigTypeDef = TypedDict(
+    "AutoBranchCreationConfigTypeDef",
     {
-        "artifactFileName": str,
-        "artifactId": str,
+        "stage": NotRequired[StageType],
+        "framework": NotRequired[str],
+        "enableAutoBuild": NotRequired[bool],
+        "environmentVariables": NotRequired[Mapping[str, str]],
+        "basicAuthCredentials": NotRequired[str],
+        "enableBasicAuth": NotRequired[bool],
+        "enablePerformanceMode": NotRequired[bool],
+        "buildSpec": NotRequired[str],
+        "enablePullRequestPreview": NotRequired[bool],
+        "pullRequestEnvironmentName": NotRequired[str],
     },
 )
 BackendEnvironmentTypeDef = TypedDict(
     "BackendEnvironmentTypeDef",
     {
         "backendEnvironmentArn": str,
         "environmentName": str,
@@ -506,43 +521,14 @@
     "UpdateWebhookRequestRequestTypeDef",
     {
         "webhookId": str,
         "branchName": NotRequired[str],
         "description": NotRequired[str],
     },
 )
-AppPaginatorTypeDef = TypedDict(
-    "AppPaginatorTypeDef",
-    {
-        "appId": str,
-        "appArn": str,
-        "name": str,
-        "description": str,
-        "repository": str,
-        "platform": PlatformType,
-        "createTime": datetime,
-        "updateTime": datetime,
-        "environmentVariables": Dict[str, str],
-        "defaultDomain": str,
-        "enableBranchAutoBuild": bool,
-        "enableBasicAuth": bool,
-        "tags": NotRequired[Dict[str, str]],
-        "iamServiceRoleArn": NotRequired[str],
-        "enableBranchAutoDeletion": NotRequired[bool],
-        "basicAuthCredentials": NotRequired[str],
-        "customRules": NotRequired[List[CustomRuleTypeDef]],
-        "productionBranch": NotRequired[ProductionBranchTypeDef],
-        "buildSpec": NotRequired[str],
-        "customHeaders": NotRequired[str],
-        "enableAutoBranchCreation": NotRequired[bool],
-        "autoBranchCreationPatterns": NotRequired[List[str]],
-        "autoBranchCreationConfig": NotRequired[AutoBranchCreationConfigPaginatorTypeDef],
-        "repositoryCloneMethod": NotRequired[RepositoryCloneMethodType],
-    },
-)
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "appId": str,
         "appArn": str,
         "name": str,
         "description": str,
@@ -560,18 +546,21 @@
         "basicAuthCredentials": NotRequired[str],
         "customRules": NotRequired[List[CustomRuleTypeDef]],
         "productionBranch": NotRequired[ProductionBranchTypeDef],
         "buildSpec": NotRequired[str],
         "customHeaders": NotRequired[str],
         "enableAutoBranchCreation": NotRequired[bool],
         "autoBranchCreationPatterns": NotRequired[List[str]],
-        "autoBranchCreationConfig": NotRequired[AutoBranchCreationConfigTypeDef],
+        "autoBranchCreationConfig": NotRequired[AutoBranchCreationConfigOutputTypeDef],
         "repositoryCloneMethod": NotRequired[RepositoryCloneMethodType],
     },
 )
+AutoBranchCreationConfigUnionTypeDef = Union[
+    AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigExtraOutputTypeDef
+]
 CreateAppRequestRequestTypeDef = TypedDict(
     "CreateAppRequestRequestTypeDef",
     {
         "name": str,
         "description": NotRequired[str],
         "repository": NotRequired[str],
         "platform": NotRequired[PlatformType],
@@ -921,22 +910,14 @@
     "ListJobsRequestListJobsPaginateTypeDef",
     {
         "appId": str,
         "branchName": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-ListAppsResultPaginatorTypeDef = TypedDict(
-    "ListAppsResultPaginatorTypeDef",
-    {
-        "apps": List[AppPaginatorTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CreateAppResultTypeDef = TypedDict(
     "CreateAppResultTypeDef",
     {
         "app": AppTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-amplify-1.34.63/mypy_boto3_amplify/type_defs.pyi` & `mypy_boto3_amplify-1.34.94/mypy_boto3_amplify/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplify service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigPaginatorTypeDef
+    from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigOutputTypeDef
 
-    data: AutoBranchCreationConfigPaginatorTypeDef = ...
+    data: AutoBranchCreationConfigOutputTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
@@ -33,19 +33,20 @@
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AutoBranchCreationConfigPaginatorTypeDef",
+    "AutoBranchCreationConfigOutputTypeDef",
     "CustomRuleTypeDef",
     "ProductionBranchTypeDef",
-    "AutoBranchCreationConfigTypeDef",
     "ArtifactTypeDef",
+    "AutoBranchCreationConfigExtraOutputTypeDef",
+    "AutoBranchCreationConfigTypeDef",
     "BackendEnvironmentTypeDef",
     "BackendTypeDef",
     "CertificateSettingsTypeDef",
     "CertificateTypeDef",
     "ResponseMetadataTypeDef",
     "CreateBackendEnvironmentRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
@@ -78,16 +79,16 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebhooksRequestRequestTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StopJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWebhookRequestRequestTypeDef",
-    "AppPaginatorTypeDef",
     "AppTypeDef",
+    "AutoBranchCreationConfigUnionTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "BranchTypeDef",
     "CreateBranchRequestRequestTypeDef",
     "UpdateBranchRequestRequestTypeDef",
     "CreateBackendEnvironmentResultTypeDef",
     "CreateDeploymentResultTypeDef",
@@ -114,15 +115,14 @@
     "GenerateAccessLogsRequestRequestTypeDef",
     "StartJobRequestRequestTypeDef",
     "JobTypeDef",
     "ListAppsRequestListAppsPaginateTypeDef",
     "ListBranchesRequestListBranchesPaginateTypeDef",
     "ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
-    "ListAppsResultPaginatorTypeDef",
     "CreateAppResultTypeDef",
     "DeleteAppResultTypeDef",
     "GetAppResultTypeDef",
     "ListAppsResultTypeDef",
     "UpdateAppResultTypeDef",
     "CreateBranchResultTypeDef",
     "DeleteBranchResultTypeDef",
@@ -134,16 +134,16 @@
     "CreateDomainAssociationResultTypeDef",
     "DeleteDomainAssociationResultTypeDef",
     "GetDomainAssociationResultTypeDef",
     "ListDomainAssociationsResultTypeDef",
     "UpdateDomainAssociationResultTypeDef",
 )
 
-AutoBranchCreationConfigPaginatorTypeDef = TypedDict(
-    "AutoBranchCreationConfigPaginatorTypeDef",
+AutoBranchCreationConfigOutputTypeDef = TypedDict(
+    "AutoBranchCreationConfigOutputTypeDef",
     {
         "stage": NotRequired[StageType],
         "framework": NotRequired[str],
         "enableAutoBuild": NotRequired[bool],
         "environmentVariables": NotRequired[Dict[str, str]],
         "basicAuthCredentials": NotRequired[str],
         "enableBasicAuth": NotRequired[bool],
@@ -167,34 +167,49 @@
     {
         "lastDeployTime": NotRequired[datetime],
         "status": NotRequired[str],
         "thumbnailUrl": NotRequired[str],
         "branchName": NotRequired[str],
     },
 )
-AutoBranchCreationConfigTypeDef = TypedDict(
-    "AutoBranchCreationConfigTypeDef",
+ArtifactTypeDef = TypedDict(
+    "ArtifactTypeDef",
+    {
+        "artifactFileName": str,
+        "artifactId": str,
+    },
+)
+AutoBranchCreationConfigExtraOutputTypeDef = TypedDict(
+    "AutoBranchCreationConfigExtraOutputTypeDef",
     {
         "stage": NotRequired[StageType],
         "framework": NotRequired[str],
         "enableAutoBuild": NotRequired[bool],
-        "environmentVariables": NotRequired[Mapping[str, str]],
+        "environmentVariables": NotRequired[Dict[str, str]],
         "basicAuthCredentials": NotRequired[str],
         "enableBasicAuth": NotRequired[bool],
         "enablePerformanceMode": NotRequired[bool],
         "buildSpec": NotRequired[str],
         "enablePullRequestPreview": NotRequired[bool],
         "pullRequestEnvironmentName": NotRequired[str],
     },
 )
-ArtifactTypeDef = TypedDict(
-    "ArtifactTypeDef",
+AutoBranchCreationConfigTypeDef = TypedDict(
+    "AutoBranchCreationConfigTypeDef",
     {
-        "artifactFileName": str,
-        "artifactId": str,
+        "stage": NotRequired[StageType],
+        "framework": NotRequired[str],
+        "enableAutoBuild": NotRequired[bool],
+        "environmentVariables": NotRequired[Mapping[str, str]],
+        "basicAuthCredentials": NotRequired[str],
+        "enableBasicAuth": NotRequired[bool],
+        "enablePerformanceMode": NotRequired[bool],
+        "buildSpec": NotRequired[str],
+        "enablePullRequestPreview": NotRequired[bool],
+        "pullRequestEnvironmentName": NotRequired[str],
     },
 )
 BackendEnvironmentTypeDef = TypedDict(
     "BackendEnvironmentTypeDef",
     {
         "backendEnvironmentArn": str,
         "environmentName": str,
@@ -506,43 +521,14 @@
     "UpdateWebhookRequestRequestTypeDef",
     {
         "webhookId": str,
         "branchName": NotRequired[str],
         "description": NotRequired[str],
     },
 )
-AppPaginatorTypeDef = TypedDict(
-    "AppPaginatorTypeDef",
-    {
-        "appId": str,
-        "appArn": str,
-        "name": str,
-        "description": str,
-        "repository": str,
-        "platform": PlatformType,
-        "createTime": datetime,
-        "updateTime": datetime,
-        "environmentVariables": Dict[str, str],
-        "defaultDomain": str,
-        "enableBranchAutoBuild": bool,
-        "enableBasicAuth": bool,
-        "tags": NotRequired[Dict[str, str]],
-        "iamServiceRoleArn": NotRequired[str],
-        "enableBranchAutoDeletion": NotRequired[bool],
-        "basicAuthCredentials": NotRequired[str],
-        "customRules": NotRequired[List[CustomRuleTypeDef]],
-        "productionBranch": NotRequired[ProductionBranchTypeDef],
-        "buildSpec": NotRequired[str],
-        "customHeaders": NotRequired[str],
-        "enableAutoBranchCreation": NotRequired[bool],
-        "autoBranchCreationPatterns": NotRequired[List[str]],
-        "autoBranchCreationConfig": NotRequired[AutoBranchCreationConfigPaginatorTypeDef],
-        "repositoryCloneMethod": NotRequired[RepositoryCloneMethodType],
-    },
-)
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "appId": str,
         "appArn": str,
         "name": str,
         "description": str,
@@ -560,18 +546,21 @@
         "basicAuthCredentials": NotRequired[str],
         "customRules": NotRequired[List[CustomRuleTypeDef]],
         "productionBranch": NotRequired[ProductionBranchTypeDef],
         "buildSpec": NotRequired[str],
         "customHeaders": NotRequired[str],
         "enableAutoBranchCreation": NotRequired[bool],
         "autoBranchCreationPatterns": NotRequired[List[str]],
-        "autoBranchCreationConfig": NotRequired[AutoBranchCreationConfigTypeDef],
+        "autoBranchCreationConfig": NotRequired[AutoBranchCreationConfigOutputTypeDef],
         "repositoryCloneMethod": NotRequired[RepositoryCloneMethodType],
     },
 )
+AutoBranchCreationConfigUnionTypeDef = Union[
+    AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigExtraOutputTypeDef
+]
 CreateAppRequestRequestTypeDef = TypedDict(
     "CreateAppRequestRequestTypeDef",
     {
         "name": str,
         "description": NotRequired[str],
         "repository": NotRequired[str],
         "platform": NotRequired[PlatformType],
@@ -921,22 +910,14 @@
     "ListJobsRequestListJobsPaginateTypeDef",
     {
         "appId": str,
         "branchName": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-ListAppsResultPaginatorTypeDef = TypedDict(
-    "ListAppsResultPaginatorTypeDef",
-    {
-        "apps": List[AppPaginatorTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CreateAppResultTypeDef = TypedDict(
     "CreateAppResultTypeDef",
     {
         "app": AppTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-amplify-1.34.63/mypy_boto3_amplify.egg-info/PKG-INFO` & `mypy_boto3_amplify-1.34.94/mypy_boto3_amplify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplify
-Version: 1.34.63
-Summary: Type annotations for boto3.Amplify 1.34.63 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.94
+Summary: Type annotations for boto3.Amplify 1.34.94 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplify)](https://pepy.tech/project/mypy-boto3-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Amplify 1.34.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[boto3.Amplify 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,18 +326,18 @@
 `mypy_boto3_amplify.type_defs` module contains structures and shapes assembled
 to typed dictionaries and unions for additional type checking.
 
 Full list of `Amplify` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/type_defs/).
 
 ```python
-from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigPaginatorTypeDef
+from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigOutputTypeDef
 
 
-def get_value() -> AutoBranchCreationConfigPaginatorTypeDef:
+def get_value() -> AutoBranchCreationConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplify-1.34.63/mypy_boto3_amplify.egg-info/SOURCES.txt` & `mypy_boto3_amplify-1.34.94/mypy_boto3_amplify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.34.63/setup.py` & `mypy_boto3_amplify-1.34.94/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplify",
-    version="1.34.63",
+    version="1.34.94",
     packages=["mypy_boto3_amplify"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Amplify 1.34.63 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.Amplify 1.34.94 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

