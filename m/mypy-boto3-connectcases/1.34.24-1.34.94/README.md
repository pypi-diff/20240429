# Comparing `tmp/mypy-boto3-connectcases-1.34.24.tar.gz` & `tmp/mypy_boto3_connectcases-1.34.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connectcases-1.34.24.tar", last modified: Mon Jan 22 20:33:19 2024, max compression
+gzip compressed data, was "mypy_boto3_connectcases-1.34.94.tar", last modified: Mon Apr 29 19:32:08 2024, max compression
```

## Comparing `mypy-boto3-connectcases-1.34.24.tar` & `mypy_boto3_connectcases-1.34.94.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 20:33:19.719051 mypy-boto3-connectcases-1.34.24/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-22 20:32:04.000000 mypy-boto3-connectcases-1.34.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-01-22 20:33:19.719051 mypy-boto3-connectcases-1.34.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11547 2024-01-22 20:32:04.000000 mypy-boto3-connectcases-1.34.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 20:33:19.715051 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-01-22 20:32:04.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-01-22 20:32:04.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-01-22 20:32:04.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22695 2024-01-22 20:32:04.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-01-22 20:32:04.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-01-22 20:32:04.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-01-22 20:32:04.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-01-22 20:32:04.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-01-22 20:32:04.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 20:32:04.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    25935 2024-01-22 20:32:05.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25935 2024-01-22 20:32:05.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-22 20:32:04.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 20:33:19.715051 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-01-22 20:33:19.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-22 20:33:19.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 20:33:19.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 20:33:19.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-22 20:33:19.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-22 20:33:19.000000 mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 20:33:19.719051 mypy-boto3-connectcases-1.34.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-01-22 20:32:04.000000 mypy-boto3-connectcases-1.34.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:08.658774 mypy_boto3_connectcases-1.34.94/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-04-29 19:32:08.658774 mypy_boto3_connectcases-1.34.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11547 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:08.658774 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24124 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24121 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-04-29 19:31:48.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-04-29 19:31:48.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    30101 2024-04-29 19:31:49.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30101 2024-04-29 19:31:48.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:08.658774 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-04-29 19:32:08.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-29 19:32:08.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:08.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:08.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 19:32:08.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 19:32:08.000000 mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:32:08.658774 mypy_boto3_connectcases-1.34.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-29 19:31:47.000000 mypy_boto3_connectcases-1.34.94/setup.py
```

### Comparing `mypy-boto3-connectcases-1.34.24/LICENSE` & `mypy_boto3_connectcases-1.34.94/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.34.24/PKG-INFO` & `mypy_boto3_connectcases-1.34.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.34.24
-Summary: Type annotations for boto3.ConnectCases 1.34.24 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.94
+Summary: Type annotations for boto3.ConnectCases 1.34.94 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcases)](https://pepy.tech/project/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.34.24](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-connectcases-1.34.24/README.md` & `mypy_boto3_connectcases-1.34.94/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcases)](https://pepy.tech/project/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.34.24](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/__init__.py` & `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/__init__.pyi` & `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/__main__.py` & `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectCases 1.34.24\nVersion:         1.34.24\nBuilder"
-        " version: 7.23.1\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.ConnectCases 1.34.94\n"
+        "Version:         1.34.94\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.24")
+    print("1.34.94")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/client.py` & `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,26 +28,26 @@
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventBridgeConfigurationTypeDef,
+    EventBridgeConfigurationUnionTypeDef,
     FieldIdentifierTypeDef,
     FieldOptionTypeDef,
-    FieldValueTypeDef,
+    FieldValueExtraUnionTypeDef,
     GetCaseAuditEventsResponseTypeDef,
     GetCaseEventConfigurationResponseTypeDef,
     GetCaseResponseTypeDef,
     GetDomainResponseTypeDef,
     GetLayoutResponseTypeDef,
     GetTemplateResponseTypeDef,
     LayoutConfigurationTypeDef,
-    LayoutContentTypeDef,
+    LayoutContentUnionTypeDef,
     ListCasesForContactResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplatesResponseTypeDef,
@@ -141,15 +141,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#close)
         """
 
     def create_case(
         self,
         *,
         domainId: str,
-        fields: Sequence[FieldValueTypeDef],
+        fields: Sequence[FieldValueExtraUnionTypeDef],
         templateId: str,
         clientToken: str = ...,
         performedBy: UserUnionTypeDef = ...,
     ) -> CreateCaseResponseTypeDef:
         """
         .
 
@@ -174,15 +174,15 @@
         Creates a field in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_field)
         """
 
     def create_layout(
-        self, *, content: LayoutContentTypeDef, domainId: str, name: str
+        self, *, content: LayoutContentUnionTypeDef, domainId: str, name: str
     ) -> CreateLayoutResponseTypeDef:
         """
         Creates a layout in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_layout)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_layout)
         """
@@ -225,14 +225,38 @@
         """
         Deletes a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#delete_domain)
         """
 
+    def delete_field(self, *, domainId: str, fieldId: str) -> Dict[str, Any]:
+        """
+        Deletes a field from a cases template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_field)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#delete_field)
+        """
+
+    def delete_layout(self, *, domainId: str, layoutId: str) -> Dict[str, Any]:
+        """
+        Deletes a layout from a cases template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_layout)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#delete_layout)
+        """
+
+    def delete_template(self, *, domainId: str, templateId: str) -> Dict[str, Any]:
+        """
+        Deletes a cases template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#delete_template)
+        """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -378,15 +402,15 @@
         Lists all of the templates in a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_templates)
         """
 
     def put_case_event_configuration(
-        self, *, domainId: str, eventBridge: EventBridgeConfigurationTypeDef
+        self, *, domainId: str, eventBridge: EventBridgeConfigurationUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Adds case event publishing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.put_case_event_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#put_case_event_configuration)
         """
@@ -442,15 +466,15 @@
         """
 
     def update_case(
         self,
         *,
         caseId: str,
         domainId: str,
-        fields: Sequence[FieldValueTypeDef],
+        fields: Sequence[FieldValueExtraUnionTypeDef],
         performedBy: UserUnionTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_case)
@@ -463,15 +487,20 @@
         Updates the properties of an existing field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_field)
         """
 
     def update_layout(
-        self, *, domainId: str, layoutId: str, content: LayoutContentTypeDef = ..., name: str = ...
+        self,
+        *,
+        domainId: str,
+        layoutId: str,
+        content: LayoutContentUnionTypeDef = ...,
+        name: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the attributes of an existing layout.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_layout)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_layout)
         """
```

### Comparing `mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/client.pyi` & `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -28,26 +28,26 @@
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventBridgeConfigurationTypeDef,
+    EventBridgeConfigurationUnionTypeDef,
     FieldIdentifierTypeDef,
     FieldOptionTypeDef,
-    FieldValueTypeDef,
+    FieldValueExtraUnionTypeDef,
     GetCaseAuditEventsResponseTypeDef,
     GetCaseEventConfigurationResponseTypeDef,
     GetCaseResponseTypeDef,
     GetDomainResponseTypeDef,
     GetLayoutResponseTypeDef,
     GetTemplateResponseTypeDef,
     LayoutConfigurationTypeDef,
-    LayoutContentTypeDef,
+    LayoutContentUnionTypeDef,
     ListCasesForContactResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplatesResponseTypeDef,
@@ -138,15 +138,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#close)
         """
 
     def create_case(
         self,
         *,
         domainId: str,
-        fields: Sequence[FieldValueTypeDef],
+        fields: Sequence[FieldValueExtraUnionTypeDef],
         templateId: str,
         clientToken: str = ...,
         performedBy: UserUnionTypeDef = ...,
     ) -> CreateCaseResponseTypeDef:
         """
         .
 
@@ -171,15 +171,15 @@
         Creates a field in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_field)
         """
 
     def create_layout(
-        self, *, content: LayoutContentTypeDef, domainId: str, name: str
+        self, *, content: LayoutContentUnionTypeDef, domainId: str, name: str
     ) -> CreateLayoutResponseTypeDef:
         """
         Creates a layout in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_layout)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_layout)
         """
@@ -222,14 +222,38 @@
         """
         Deletes a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#delete_domain)
         """
 
+    def delete_field(self, *, domainId: str, fieldId: str) -> Dict[str, Any]:
+        """
+        Deletes a field from a cases template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_field)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#delete_field)
+        """
+
+    def delete_layout(self, *, domainId: str, layoutId: str) -> Dict[str, Any]:
+        """
+        Deletes a layout from a cases template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_layout)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#delete_layout)
+        """
+
+    def delete_template(self, *, domainId: str, templateId: str) -> Dict[str, Any]:
+        """
+        Deletes a cases template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_template)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#delete_template)
+        """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -375,15 +399,15 @@
         Lists all of the templates in a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_templates)
         """
 
     def put_case_event_configuration(
-        self, *, domainId: str, eventBridge: EventBridgeConfigurationTypeDef
+        self, *, domainId: str, eventBridge: EventBridgeConfigurationUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Adds case event publishing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.put_case_event_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#put_case_event_configuration)
         """
@@ -439,15 +463,15 @@
         """
 
     def update_case(
         self,
         *,
         caseId: str,
         domainId: str,
-        fields: Sequence[FieldValueTypeDef],
+        fields: Sequence[FieldValueExtraUnionTypeDef],
         performedBy: UserUnionTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_case)
@@ -460,15 +484,20 @@
         Updates the properties of an existing field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_field)
         """
 
     def update_layout(
-        self, *, domainId: str, layoutId: str, content: LayoutContentTypeDef = ..., name: str = ...
+        self,
+        *,
+        domainId: str,
+        layoutId: str,
+        content: LayoutContentUnionTypeDef = ...,
+        name: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the attributes of an existing layout.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_layout)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_layout)
         """
```

### Comparing `mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/literals.py` & `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
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
@@ -88,14 +89,15 @@
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
@@ -113,14 +115,15 @@
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
@@ -133,24 +136,26 @@
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
@@ -211,15 +216,14 @@
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
@@ -348,14 +352,15 @@
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
@@ -399,14 +404,15 @@
     "sts",
     "supplychain",
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

### Comparing `mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/literals.pyi` & `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
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
@@ -88,14 +89,15 @@
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
@@ -113,14 +115,15 @@
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
@@ -133,24 +136,26 @@
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
@@ -211,15 +216,14 @@
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
@@ -348,14 +352,15 @@
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
@@ -399,14 +404,15 @@
     "sts",
     "supplychain",
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

### Comparing `mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/paginator.py` & `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/paginator.pyi` & `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/type_defs.py` & `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AuditEventFieldValueUnionTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AuditEventTypeType,
     DomainStatusType,
     FieldNamespaceType,
     FieldTypeType,
     OrderType,
@@ -54,18 +54,23 @@
     "ContactFilterTypeDef",
     "ContactTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "CreateFieldRequestRequestTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
     "DeleteDomainRequestRequestTypeDef",
+    "DeleteFieldRequestRequestTypeDef",
+    "DeleteLayoutRequestRequestTypeDef",
+    "DeleteTemplateRequestRequestTypeDef",
     "DomainSummaryTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
     "FieldItemTypeDef",
     "FieldSummaryTypeDef",
+    "FieldValueUnionExtraOutputTypeDef",
+    "FieldValueUnionOutputTypeDef",
     "FieldValueUnionTypeDef",
     "GetCaseAuditEventsRequestRequestTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
     "LayoutSummaryTypeDef",
@@ -81,14 +86,15 @@
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "AuditEventFieldTypeDef",
     "AuditEventPerformedByTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
+    "CaseEventIncludedDataOutputTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
     "CreateCaseResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "CreateFieldResponseTypeDef",
     "CreateLayoutResponseTypeDef",
@@ -104,45 +110,57 @@
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
     "CreateTemplateRequestRequestTypeDef",
     "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
+    "FieldGroupOutputTypeDef",
     "FieldGroupTypeDef",
     "ListFieldsResponseTypeDef",
+    "FieldValueExtraOutputTypeDef",
+    "FieldValueOutputTypeDef",
     "FieldValueTypeDef",
     "ListLayoutsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "SearchCasesRequestRequestTypeDef",
     "AuditEventTypeDef",
+    "EventIncludedDataOutputTypeDef",
     "EventIncludedDataTypeDef",
     "SearchRelatedItemsResponseItemTypeDef",
     "SearchRelatedItemsRequestRequestTypeDef",
     "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     "CreateRelatedItemRequestRequestTypeDef",
+    "SectionOutputTypeDef",
     "SectionTypeDef",
-    "CreateCaseRequestRequestTypeDef",
-    "FieldFilterTypeDef",
     "GetCaseResponseTypeDef",
     "SearchCasesResponseItemTypeDef",
-    "UpdateCaseRequestRequestTypeDef",
+    "FieldFilterTypeDef",
+    "FieldValueExtraUnionTypeDef",
     "GetCaseAuditEventsResponseTypeDef",
+    "EventBridgeConfigurationOutputTypeDef",
     "EventBridgeConfigurationTypeDef",
     "SearchRelatedItemsResponseTypeDef",
+    "LayoutSectionsOutputTypeDef",
     "LayoutSectionsTypeDef",
-    "CaseFilterTypeDef",
     "SearchCasesResponseTypeDef",
+    "CaseFilterTypeDef",
+    "CreateCaseRequestRequestTypeDef",
+    "UpdateCaseRequestRequestTypeDef",
     "GetCaseEventConfigurationResponseTypeDef",
+    "EventBridgeConfigurationUnionTypeDef",
     "PutCaseEventConfigurationRequestRequestTypeDef",
+    "BasicLayoutOutputTypeDef",
     "BasicLayoutTypeDef",
     "SearchCasesRequestSearchCasesPaginateTypeDef",
+    "LayoutContentOutputTypeDef",
     "LayoutContentTypeDef",
-    "CreateLayoutRequestRequestTypeDef",
     "GetLayoutResponseTypeDef",
+    "CreateLayoutRequestRequestTypeDef",
+    "LayoutContentUnionTypeDef",
     "UpdateLayoutRequestRequestTypeDef",
 )
 
 AuditEventFieldValueUnionTypeDef = TypedDict(
     "AuditEventFieldValueUnionTypeDef",
     {
         "booleanValue": NotRequired[bool],
@@ -176,26 +194,29 @@
     "GetFieldResponseTypeDef",
     {
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
         "type": FieldTypeType,
+        "createdTime": NotRequired[datetime],
+        "deleted": NotRequired[bool],
         "description": NotRequired[str],
+        "lastModifiedTime": NotRequired[datetime],
         "tags": NotRequired[Dict[str, str]],
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
     },
 )
 FieldOptionTypeDef = TypedDict(
     "FieldOptionTypeDef",
     {
         "active": bool,
         "name": str,
@@ -274,14 +295,35 @@
 )
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
+DeleteFieldRequestRequestTypeDef = TypedDict(
+    "DeleteFieldRequestRequestTypeDef",
+    {
+        "domainId": str,
+        "fieldId": str,
+    },
+)
+DeleteLayoutRequestRequestTypeDef = TypedDict(
+    "DeleteLayoutRequestRequestTypeDef",
+    {
+        "domainId": str,
+        "layoutId": str,
+    },
+)
+DeleteTemplateRequestRequestTypeDef = TypedDict(
+    "DeleteTemplateRequestRequestTypeDef",
+    {
+        "domainId": str,
+        "templateId": str,
+    },
+)
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
@@ -304,14 +346,34 @@
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
         "type": FieldTypeType,
     },
 )
+FieldValueUnionExtraOutputTypeDef = TypedDict(
+    "FieldValueUnionExtraOutputTypeDef",
+    {
+        "booleanValue": NotRequired[bool],
+        "doubleValue": NotRequired[float],
+        "emptyValue": NotRequired[Dict[str, Any]],
+        "stringValue": NotRequired[str],
+        "userArnValue": NotRequired[str],
+    },
+)
+FieldValueUnionOutputTypeDef = TypedDict(
+    "FieldValueUnionOutputTypeDef",
+    {
+        "booleanValue": NotRequired[bool],
+        "doubleValue": NotRequired[float],
+        "emptyValue": NotRequired[Dict[str, Any]],
+        "stringValue": NotRequired[str],
+        "userArnValue": NotRequired[str],
+    },
+)
 FieldValueUnionTypeDef = TypedDict(
     "FieldValueUnionTypeDef",
     {
         "booleanValue": NotRequired[bool],
         "doubleValue": NotRequired[float],
         "emptyValue": NotRequired[Mapping[str, Any]],
         "stringValue": NotRequired[str],
@@ -483,18 +545,24 @@
 BatchGetFieldRequestRequestTypeDef = TypedDict(
     "BatchGetFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
+CaseEventIncludedDataOutputTypeDef = TypedDict(
+    "CaseEventIncludedDataOutputTypeDef",
+    {
+        "fields": List[FieldIdentifierTypeDef],
+    },
+)
 CaseEventIncludedDataTypeDef = TypedDict(
     "CaseEventIncludedDataTypeDef",
     {
-        "fields": List[FieldIdentifierTypeDef],
+        "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 GetCaseRequestRequestTypeDef = TypedDict(
     "GetCaseRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
@@ -646,15 +714,18 @@
         "requiredFields": NotRequired[Sequence[RequiredFieldTypeDef]],
         "status": NotRequired[TemplateStatusType],
     },
 )
 GetTemplateResponseTypeDef = TypedDict(
     "GetTemplateResponseTypeDef",
     {
+        "createdTime": datetime,
+        "deleted": bool,
         "description": str,
+        "lastModifiedTime": datetime,
         "layoutConfiguration": LayoutConfigurationTypeDef,
         "name": str,
         "requiredFields": List[RequiredFieldTypeDef],
         "status": TemplateStatusType,
         "tags": Dict[str, str],
         "templateArn": str,
         "templateId": str,
@@ -677,14 +748,21 @@
     "ListDomainsResponseTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+FieldGroupOutputTypeDef = TypedDict(
+    "FieldGroupOutputTypeDef",
+    {
+        "fields": List[FieldItemTypeDef],
+        "name": NotRequired[str],
+    },
+)
 FieldGroupTypeDef = TypedDict(
     "FieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
         "name": NotRequired[str],
     },
 )
@@ -692,14 +770,28 @@
     "ListFieldsResponseTypeDef",
     {
         "fields": List[FieldSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+FieldValueExtraOutputTypeDef = TypedDict(
+    "FieldValueExtraOutputTypeDef",
+    {
+        "id": str,
+        "value": FieldValueUnionExtraOutputTypeDef,
+    },
+)
+FieldValueOutputTypeDef = TypedDict(
+    "FieldValueOutputTypeDef",
+    {
+        "id": str,
+        "value": FieldValueUnionOutputTypeDef,
+    },
+)
 FieldValueTypeDef = TypedDict(
     "FieldValueTypeDef",
     {
         "id": str,
         "value": FieldValueUnionTypeDef,
     },
 )
@@ -738,14 +830,21 @@
         "fields": List[AuditEventFieldTypeDef],
         "performedTime": datetime,
         "type": AuditEventTypeType,
         "performedBy": NotRequired[AuditEventPerformedByTypeDef],
         "relatedItemType": NotRequired[RelatedItemTypeType],
     },
 )
+EventIncludedDataOutputTypeDef = TypedDict(
+    "EventIncludedDataOutputTypeDef",
+    {
+        "caseData": NotRequired[CaseEventIncludedDataOutputTypeDef],
+        "relatedItemData": NotRequired[RelatedItemEventIncludedDataTypeDef],
+    },
+)
 EventIncludedDataTypeDef = TypedDict(
     "EventIncludedDataTypeDef",
     {
         "caseData": NotRequired[CaseEventIncludedDataTypeDef],
         "relatedItemData": NotRequired[RelatedItemEventIncludedDataTypeDef],
     },
 )
@@ -785,77 +884,72 @@
         "caseId": str,
         "content": RelatedItemInputContentTypeDef,
         "domainId": str,
         "type": RelatedItemTypeType,
         "performedBy": NotRequired[UserUnionTypeDef],
     },
 )
-SectionTypeDef = TypedDict(
-    "SectionTypeDef",
-    {
-        "fieldGroup": NotRequired[FieldGroupTypeDef],
-    },
-)
-CreateCaseRequestRequestTypeDef = TypedDict(
-    "CreateCaseRequestRequestTypeDef",
+SectionOutputTypeDef = TypedDict(
+    "SectionOutputTypeDef",
     {
-        "domainId": str,
-        "fields": Sequence[FieldValueTypeDef],
-        "templateId": str,
-        "clientToken": NotRequired[str],
-        "performedBy": NotRequired[UserUnionTypeDef],
+        "fieldGroup": NotRequired[FieldGroupOutputTypeDef],
     },
 )
-FieldFilterTypeDef = TypedDict(
-    "FieldFilterTypeDef",
+SectionTypeDef = TypedDict(
+    "SectionTypeDef",
     {
-        "contains": NotRequired[FieldValueTypeDef],
-        "equalTo": NotRequired[FieldValueTypeDef],
-        "greaterThan": NotRequired[FieldValueTypeDef],
-        "greaterThanOrEqualTo": NotRequired[FieldValueTypeDef],
-        "lessThan": NotRequired[FieldValueTypeDef],
-        "lessThanOrEqualTo": NotRequired[FieldValueTypeDef],
+        "fieldGroup": NotRequired[FieldGroupTypeDef],
     },
 )
 GetCaseResponseTypeDef = TypedDict(
     "GetCaseResponseTypeDef",
     {
-        "fields": List[FieldValueTypeDef],
+        "fields": List[FieldValueOutputTypeDef],
         "nextToken": str,
         "tags": Dict[str, str],
         "templateId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchCasesResponseItemTypeDef = TypedDict(
     "SearchCasesResponseItemTypeDef",
     {
         "caseId": str,
-        "fields": List[FieldValueTypeDef],
+        "fields": List[FieldValueOutputTypeDef],
         "templateId": str,
         "tags": NotRequired[Dict[str, str]],
     },
 )
-UpdateCaseRequestRequestTypeDef = TypedDict(
-    "UpdateCaseRequestRequestTypeDef",
+FieldFilterTypeDef = TypedDict(
+    "FieldFilterTypeDef",
     {
-        "caseId": str,
-        "domainId": str,
-        "fields": Sequence[FieldValueTypeDef],
-        "performedBy": NotRequired[UserUnionTypeDef],
+        "contains": NotRequired[FieldValueTypeDef],
+        "equalTo": NotRequired[FieldValueTypeDef],
+        "greaterThan": NotRequired[FieldValueTypeDef],
+        "greaterThanOrEqualTo": NotRequired[FieldValueTypeDef],
+        "lessThan": NotRequired[FieldValueTypeDef],
+        "lessThanOrEqualTo": NotRequired[FieldValueTypeDef],
     },
 )
+FieldValueExtraUnionTypeDef = Union[FieldValueTypeDef, FieldValueExtraOutputTypeDef]
 GetCaseAuditEventsResponseTypeDef = TypedDict(
     "GetCaseAuditEventsResponseTypeDef",
     {
         "auditEvents": List[AuditEventTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+EventBridgeConfigurationOutputTypeDef = TypedDict(
+    "EventBridgeConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "includedData": NotRequired[EventIncludedDataOutputTypeDef],
+    },
+)
 EventBridgeConfigurationTypeDef = TypedDict(
     "EventBridgeConfigurationTypeDef",
     {
         "enabled": bool,
         "includedData": NotRequired[EventIncludedDataTypeDef],
     },
 )
@@ -863,51 +957,86 @@
     "SearchRelatedItemsResponseTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+LayoutSectionsOutputTypeDef = TypedDict(
+    "LayoutSectionsOutputTypeDef",
+    {
+        "sections": NotRequired[List[SectionOutputTypeDef]],
+    },
+)
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": NotRequired[Sequence[SectionTypeDef]],
     },
 )
+SearchCasesResponseTypeDef = TypedDict(
+    "SearchCasesResponseTypeDef",
+    {
+        "cases": List[SearchCasesResponseItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CaseFilterTypeDef = TypedDict(
     "CaseFilterTypeDef",
     {
         "andAll": NotRequired[Sequence[Dict[str, Any]]],
         "field": NotRequired[FieldFilterTypeDef],
         "not": NotRequired[Dict[str, Any]],
         "orAll": NotRequired[Sequence[Dict[str, Any]]],
     },
 )
-SearchCasesResponseTypeDef = TypedDict(
-    "SearchCasesResponseTypeDef",
+CreateCaseRequestRequestTypeDef = TypedDict(
+    "CreateCaseRequestRequestTypeDef",
     {
-        "cases": List[SearchCasesResponseItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "domainId": str,
+        "fields": Sequence[FieldValueExtraUnionTypeDef],
+        "templateId": str,
+        "clientToken": NotRequired[str],
+        "performedBy": NotRequired[UserUnionTypeDef],
+    },
+)
+UpdateCaseRequestRequestTypeDef = TypedDict(
+    "UpdateCaseRequestRequestTypeDef",
+    {
+        "caseId": str,
+        "domainId": str,
+        "fields": Sequence[FieldValueExtraUnionTypeDef],
+        "performedBy": NotRequired[UserUnionTypeDef],
     },
 )
 GetCaseEventConfigurationResponseTypeDef = TypedDict(
     "GetCaseEventConfigurationResponseTypeDef",
     {
-        "eventBridge": EventBridgeConfigurationTypeDef,
+        "eventBridge": EventBridgeConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+EventBridgeConfigurationUnionTypeDef = Union[
+    EventBridgeConfigurationTypeDef, EventBridgeConfigurationOutputTypeDef
+]
 PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "PutCaseEventConfigurationRequestRequestTypeDef",
     {
         "domainId": str,
         "eventBridge": EventBridgeConfigurationTypeDef,
     },
 )
+BasicLayoutOutputTypeDef = TypedDict(
+    "BasicLayoutOutputTypeDef",
+    {
+        "moreInfo": NotRequired[LayoutSectionsOutputTypeDef],
+        "topPanel": NotRequired[LayoutSectionsOutputTypeDef],
+    },
+)
 BasicLayoutTypeDef = TypedDict(
     "BasicLayoutTypeDef",
     {
         "moreInfo": NotRequired[LayoutSectionsTypeDef],
         "topPanel": NotRequired[LayoutSectionsTypeDef],
     },
 )
@@ -918,39 +1047,49 @@
         "fields": NotRequired[Sequence[FieldIdentifierTypeDef]],
         "filter": NotRequired[CaseFilterTypeDef],
         "searchTerm": NotRequired[str],
         "sorts": NotRequired[Sequence[SortTypeDef]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-LayoutContentTypeDef = TypedDict(
-    "LayoutContentTypeDef",
+LayoutContentOutputTypeDef = TypedDict(
+    "LayoutContentOutputTypeDef",
     {
-        "basic": NotRequired[BasicLayoutTypeDef],
+        "basic": NotRequired[BasicLayoutOutputTypeDef],
     },
 )
-CreateLayoutRequestRequestTypeDef = TypedDict(
-    "CreateLayoutRequestRequestTypeDef",
+LayoutContentTypeDef = TypedDict(
+    "LayoutContentTypeDef",
     {
-        "content": LayoutContentTypeDef,
-        "domainId": str,
-        "name": str,
+        "basic": NotRequired[BasicLayoutTypeDef],
     },
 )
 GetLayoutResponseTypeDef = TypedDict(
     "GetLayoutResponseTypeDef",
     {
-        "content": LayoutContentTypeDef,
+        "content": LayoutContentOutputTypeDef,
+        "createdTime": datetime,
+        "deleted": bool,
+        "lastModifiedTime": datetime,
         "layoutArn": str,
         "layoutId": str,
         "name": str,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateLayoutRequestRequestTypeDef = TypedDict(
+    "CreateLayoutRequestRequestTypeDef",
+    {
+        "content": LayoutContentTypeDef,
+        "domainId": str,
+        "name": str,
+    },
+)
+LayoutContentUnionTypeDef = Union[LayoutContentTypeDef, LayoutContentOutputTypeDef]
 UpdateLayoutRequestRequestTypeDef = TypedDict(
     "UpdateLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
         "content": NotRequired[LayoutContentTypeDef],
         "name": NotRequired[str],
```

### Comparing `mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases/type_defs.pyi` & `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AuditEventFieldValueUnionTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AuditEventTypeType,
     DomainStatusType,
     FieldNamespaceType,
     FieldTypeType,
     OrderType,
@@ -54,18 +54,23 @@
     "ContactFilterTypeDef",
     "ContactTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "CreateFieldRequestRequestTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
     "DeleteDomainRequestRequestTypeDef",
+    "DeleteFieldRequestRequestTypeDef",
+    "DeleteLayoutRequestRequestTypeDef",
+    "DeleteTemplateRequestRequestTypeDef",
     "DomainSummaryTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
     "FieldItemTypeDef",
     "FieldSummaryTypeDef",
+    "FieldValueUnionExtraOutputTypeDef",
+    "FieldValueUnionOutputTypeDef",
     "FieldValueUnionTypeDef",
     "GetCaseAuditEventsRequestRequestTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
     "LayoutSummaryTypeDef",
@@ -81,14 +86,15 @@
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "AuditEventFieldTypeDef",
     "AuditEventPerformedByTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
+    "CaseEventIncludedDataOutputTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
     "CreateCaseResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "CreateFieldResponseTypeDef",
     "CreateLayoutResponseTypeDef",
@@ -104,45 +110,57 @@
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
     "CreateTemplateRequestRequestTypeDef",
     "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
+    "FieldGroupOutputTypeDef",
     "FieldGroupTypeDef",
     "ListFieldsResponseTypeDef",
+    "FieldValueExtraOutputTypeDef",
+    "FieldValueOutputTypeDef",
     "FieldValueTypeDef",
     "ListLayoutsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "SearchCasesRequestRequestTypeDef",
     "AuditEventTypeDef",
+    "EventIncludedDataOutputTypeDef",
     "EventIncludedDataTypeDef",
     "SearchRelatedItemsResponseItemTypeDef",
     "SearchRelatedItemsRequestRequestTypeDef",
     "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     "CreateRelatedItemRequestRequestTypeDef",
+    "SectionOutputTypeDef",
     "SectionTypeDef",
-    "CreateCaseRequestRequestTypeDef",
-    "FieldFilterTypeDef",
     "GetCaseResponseTypeDef",
     "SearchCasesResponseItemTypeDef",
-    "UpdateCaseRequestRequestTypeDef",
+    "FieldFilterTypeDef",
+    "FieldValueExtraUnionTypeDef",
     "GetCaseAuditEventsResponseTypeDef",
+    "EventBridgeConfigurationOutputTypeDef",
     "EventBridgeConfigurationTypeDef",
     "SearchRelatedItemsResponseTypeDef",
+    "LayoutSectionsOutputTypeDef",
     "LayoutSectionsTypeDef",
-    "CaseFilterTypeDef",
     "SearchCasesResponseTypeDef",
+    "CaseFilterTypeDef",
+    "CreateCaseRequestRequestTypeDef",
+    "UpdateCaseRequestRequestTypeDef",
     "GetCaseEventConfigurationResponseTypeDef",
+    "EventBridgeConfigurationUnionTypeDef",
     "PutCaseEventConfigurationRequestRequestTypeDef",
+    "BasicLayoutOutputTypeDef",
     "BasicLayoutTypeDef",
     "SearchCasesRequestSearchCasesPaginateTypeDef",
+    "LayoutContentOutputTypeDef",
     "LayoutContentTypeDef",
-    "CreateLayoutRequestRequestTypeDef",
     "GetLayoutResponseTypeDef",
+    "CreateLayoutRequestRequestTypeDef",
+    "LayoutContentUnionTypeDef",
     "UpdateLayoutRequestRequestTypeDef",
 )
 
 AuditEventFieldValueUnionTypeDef = TypedDict(
     "AuditEventFieldValueUnionTypeDef",
     {
         "booleanValue": NotRequired[bool],
@@ -176,26 +194,29 @@
     "GetFieldResponseTypeDef",
     {
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
         "type": FieldTypeType,
+        "createdTime": NotRequired[datetime],
+        "deleted": NotRequired[bool],
         "description": NotRequired[str],
+        "lastModifiedTime": NotRequired[datetime],
         "tags": NotRequired[Dict[str, str]],
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
     },
 )
 FieldOptionTypeDef = TypedDict(
     "FieldOptionTypeDef",
     {
         "active": bool,
         "name": str,
@@ -274,14 +295,35 @@
 )
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
+DeleteFieldRequestRequestTypeDef = TypedDict(
+    "DeleteFieldRequestRequestTypeDef",
+    {
+        "domainId": str,
+        "fieldId": str,
+    },
+)
+DeleteLayoutRequestRequestTypeDef = TypedDict(
+    "DeleteLayoutRequestRequestTypeDef",
+    {
+        "domainId": str,
+        "layoutId": str,
+    },
+)
+DeleteTemplateRequestRequestTypeDef = TypedDict(
+    "DeleteTemplateRequestRequestTypeDef",
+    {
+        "domainId": str,
+        "templateId": str,
+    },
+)
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
@@ -304,14 +346,34 @@
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
         "type": FieldTypeType,
     },
 )
+FieldValueUnionExtraOutputTypeDef = TypedDict(
+    "FieldValueUnionExtraOutputTypeDef",
+    {
+        "booleanValue": NotRequired[bool],
+        "doubleValue": NotRequired[float],
+        "emptyValue": NotRequired[Dict[str, Any]],
+        "stringValue": NotRequired[str],
+        "userArnValue": NotRequired[str],
+    },
+)
+FieldValueUnionOutputTypeDef = TypedDict(
+    "FieldValueUnionOutputTypeDef",
+    {
+        "booleanValue": NotRequired[bool],
+        "doubleValue": NotRequired[float],
+        "emptyValue": NotRequired[Dict[str, Any]],
+        "stringValue": NotRequired[str],
+        "userArnValue": NotRequired[str],
+    },
+)
 FieldValueUnionTypeDef = TypedDict(
     "FieldValueUnionTypeDef",
     {
         "booleanValue": NotRequired[bool],
         "doubleValue": NotRequired[float],
         "emptyValue": NotRequired[Mapping[str, Any]],
         "stringValue": NotRequired[str],
@@ -483,18 +545,24 @@
 BatchGetFieldRequestRequestTypeDef = TypedDict(
     "BatchGetFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
+CaseEventIncludedDataOutputTypeDef = TypedDict(
+    "CaseEventIncludedDataOutputTypeDef",
+    {
+        "fields": List[FieldIdentifierTypeDef],
+    },
+)
 CaseEventIncludedDataTypeDef = TypedDict(
     "CaseEventIncludedDataTypeDef",
     {
-        "fields": List[FieldIdentifierTypeDef],
+        "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 GetCaseRequestRequestTypeDef = TypedDict(
     "GetCaseRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
@@ -646,15 +714,18 @@
         "requiredFields": NotRequired[Sequence[RequiredFieldTypeDef]],
         "status": NotRequired[TemplateStatusType],
     },
 )
 GetTemplateResponseTypeDef = TypedDict(
     "GetTemplateResponseTypeDef",
     {
+        "createdTime": datetime,
+        "deleted": bool,
         "description": str,
+        "lastModifiedTime": datetime,
         "layoutConfiguration": LayoutConfigurationTypeDef,
         "name": str,
         "requiredFields": List[RequiredFieldTypeDef],
         "status": TemplateStatusType,
         "tags": Dict[str, str],
         "templateArn": str,
         "templateId": str,
@@ -677,14 +748,21 @@
     "ListDomainsResponseTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+FieldGroupOutputTypeDef = TypedDict(
+    "FieldGroupOutputTypeDef",
+    {
+        "fields": List[FieldItemTypeDef],
+        "name": NotRequired[str],
+    },
+)
 FieldGroupTypeDef = TypedDict(
     "FieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
         "name": NotRequired[str],
     },
 )
@@ -692,14 +770,28 @@
     "ListFieldsResponseTypeDef",
     {
         "fields": List[FieldSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+FieldValueExtraOutputTypeDef = TypedDict(
+    "FieldValueExtraOutputTypeDef",
+    {
+        "id": str,
+        "value": FieldValueUnionExtraOutputTypeDef,
+    },
+)
+FieldValueOutputTypeDef = TypedDict(
+    "FieldValueOutputTypeDef",
+    {
+        "id": str,
+        "value": FieldValueUnionOutputTypeDef,
+    },
+)
 FieldValueTypeDef = TypedDict(
     "FieldValueTypeDef",
     {
         "id": str,
         "value": FieldValueUnionTypeDef,
     },
 )
@@ -738,14 +830,21 @@
         "fields": List[AuditEventFieldTypeDef],
         "performedTime": datetime,
         "type": AuditEventTypeType,
         "performedBy": NotRequired[AuditEventPerformedByTypeDef],
         "relatedItemType": NotRequired[RelatedItemTypeType],
     },
 )
+EventIncludedDataOutputTypeDef = TypedDict(
+    "EventIncludedDataOutputTypeDef",
+    {
+        "caseData": NotRequired[CaseEventIncludedDataOutputTypeDef],
+        "relatedItemData": NotRequired[RelatedItemEventIncludedDataTypeDef],
+    },
+)
 EventIncludedDataTypeDef = TypedDict(
     "EventIncludedDataTypeDef",
     {
         "caseData": NotRequired[CaseEventIncludedDataTypeDef],
         "relatedItemData": NotRequired[RelatedItemEventIncludedDataTypeDef],
     },
 )
@@ -785,77 +884,72 @@
         "caseId": str,
         "content": RelatedItemInputContentTypeDef,
         "domainId": str,
         "type": RelatedItemTypeType,
         "performedBy": NotRequired[UserUnionTypeDef],
     },
 )
-SectionTypeDef = TypedDict(
-    "SectionTypeDef",
-    {
-        "fieldGroup": NotRequired[FieldGroupTypeDef],
-    },
-)
-CreateCaseRequestRequestTypeDef = TypedDict(
-    "CreateCaseRequestRequestTypeDef",
+SectionOutputTypeDef = TypedDict(
+    "SectionOutputTypeDef",
     {
-        "domainId": str,
-        "fields": Sequence[FieldValueTypeDef],
-        "templateId": str,
-        "clientToken": NotRequired[str],
-        "performedBy": NotRequired[UserUnionTypeDef],
+        "fieldGroup": NotRequired[FieldGroupOutputTypeDef],
     },
 )
-FieldFilterTypeDef = TypedDict(
-    "FieldFilterTypeDef",
+SectionTypeDef = TypedDict(
+    "SectionTypeDef",
     {
-        "contains": NotRequired[FieldValueTypeDef],
-        "equalTo": NotRequired[FieldValueTypeDef],
-        "greaterThan": NotRequired[FieldValueTypeDef],
-        "greaterThanOrEqualTo": NotRequired[FieldValueTypeDef],
-        "lessThan": NotRequired[FieldValueTypeDef],
-        "lessThanOrEqualTo": NotRequired[FieldValueTypeDef],
+        "fieldGroup": NotRequired[FieldGroupTypeDef],
     },
 )
 GetCaseResponseTypeDef = TypedDict(
     "GetCaseResponseTypeDef",
     {
-        "fields": List[FieldValueTypeDef],
+        "fields": List[FieldValueOutputTypeDef],
         "nextToken": str,
         "tags": Dict[str, str],
         "templateId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchCasesResponseItemTypeDef = TypedDict(
     "SearchCasesResponseItemTypeDef",
     {
         "caseId": str,
-        "fields": List[FieldValueTypeDef],
+        "fields": List[FieldValueOutputTypeDef],
         "templateId": str,
         "tags": NotRequired[Dict[str, str]],
     },
 )
-UpdateCaseRequestRequestTypeDef = TypedDict(
-    "UpdateCaseRequestRequestTypeDef",
+FieldFilterTypeDef = TypedDict(
+    "FieldFilterTypeDef",
     {
-        "caseId": str,
-        "domainId": str,
-        "fields": Sequence[FieldValueTypeDef],
-        "performedBy": NotRequired[UserUnionTypeDef],
+        "contains": NotRequired[FieldValueTypeDef],
+        "equalTo": NotRequired[FieldValueTypeDef],
+        "greaterThan": NotRequired[FieldValueTypeDef],
+        "greaterThanOrEqualTo": NotRequired[FieldValueTypeDef],
+        "lessThan": NotRequired[FieldValueTypeDef],
+        "lessThanOrEqualTo": NotRequired[FieldValueTypeDef],
     },
 )
+FieldValueExtraUnionTypeDef = Union[FieldValueTypeDef, FieldValueExtraOutputTypeDef]
 GetCaseAuditEventsResponseTypeDef = TypedDict(
     "GetCaseAuditEventsResponseTypeDef",
     {
         "auditEvents": List[AuditEventTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+EventBridgeConfigurationOutputTypeDef = TypedDict(
+    "EventBridgeConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "includedData": NotRequired[EventIncludedDataOutputTypeDef],
+    },
+)
 EventBridgeConfigurationTypeDef = TypedDict(
     "EventBridgeConfigurationTypeDef",
     {
         "enabled": bool,
         "includedData": NotRequired[EventIncludedDataTypeDef],
     },
 )
@@ -863,51 +957,86 @@
     "SearchRelatedItemsResponseTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+LayoutSectionsOutputTypeDef = TypedDict(
+    "LayoutSectionsOutputTypeDef",
+    {
+        "sections": NotRequired[List[SectionOutputTypeDef]],
+    },
+)
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": NotRequired[Sequence[SectionTypeDef]],
     },
 )
+SearchCasesResponseTypeDef = TypedDict(
+    "SearchCasesResponseTypeDef",
+    {
+        "cases": List[SearchCasesResponseItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CaseFilterTypeDef = TypedDict(
     "CaseFilterTypeDef",
     {
         "andAll": NotRequired[Sequence[Dict[str, Any]]],
         "field": NotRequired[FieldFilterTypeDef],
         "not": NotRequired[Dict[str, Any]],
         "orAll": NotRequired[Sequence[Dict[str, Any]]],
     },
 )
-SearchCasesResponseTypeDef = TypedDict(
-    "SearchCasesResponseTypeDef",
+CreateCaseRequestRequestTypeDef = TypedDict(
+    "CreateCaseRequestRequestTypeDef",
     {
-        "cases": List[SearchCasesResponseItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "domainId": str,
+        "fields": Sequence[FieldValueExtraUnionTypeDef],
+        "templateId": str,
+        "clientToken": NotRequired[str],
+        "performedBy": NotRequired[UserUnionTypeDef],
+    },
+)
+UpdateCaseRequestRequestTypeDef = TypedDict(
+    "UpdateCaseRequestRequestTypeDef",
+    {
+        "caseId": str,
+        "domainId": str,
+        "fields": Sequence[FieldValueExtraUnionTypeDef],
+        "performedBy": NotRequired[UserUnionTypeDef],
     },
 )
 GetCaseEventConfigurationResponseTypeDef = TypedDict(
     "GetCaseEventConfigurationResponseTypeDef",
     {
-        "eventBridge": EventBridgeConfigurationTypeDef,
+        "eventBridge": EventBridgeConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+EventBridgeConfigurationUnionTypeDef = Union[
+    EventBridgeConfigurationTypeDef, EventBridgeConfigurationOutputTypeDef
+]
 PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "PutCaseEventConfigurationRequestRequestTypeDef",
     {
         "domainId": str,
         "eventBridge": EventBridgeConfigurationTypeDef,
     },
 )
+BasicLayoutOutputTypeDef = TypedDict(
+    "BasicLayoutOutputTypeDef",
+    {
+        "moreInfo": NotRequired[LayoutSectionsOutputTypeDef],
+        "topPanel": NotRequired[LayoutSectionsOutputTypeDef],
+    },
+)
 BasicLayoutTypeDef = TypedDict(
     "BasicLayoutTypeDef",
     {
         "moreInfo": NotRequired[LayoutSectionsTypeDef],
         "topPanel": NotRequired[LayoutSectionsTypeDef],
     },
 )
@@ -918,39 +1047,49 @@
         "fields": NotRequired[Sequence[FieldIdentifierTypeDef]],
         "filter": NotRequired[CaseFilterTypeDef],
         "searchTerm": NotRequired[str],
         "sorts": NotRequired[Sequence[SortTypeDef]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-LayoutContentTypeDef = TypedDict(
-    "LayoutContentTypeDef",
+LayoutContentOutputTypeDef = TypedDict(
+    "LayoutContentOutputTypeDef",
     {
-        "basic": NotRequired[BasicLayoutTypeDef],
+        "basic": NotRequired[BasicLayoutOutputTypeDef],
     },
 )
-CreateLayoutRequestRequestTypeDef = TypedDict(
-    "CreateLayoutRequestRequestTypeDef",
+LayoutContentTypeDef = TypedDict(
+    "LayoutContentTypeDef",
     {
-        "content": LayoutContentTypeDef,
-        "domainId": str,
-        "name": str,
+        "basic": NotRequired[BasicLayoutTypeDef],
     },
 )
 GetLayoutResponseTypeDef = TypedDict(
     "GetLayoutResponseTypeDef",
     {
-        "content": LayoutContentTypeDef,
+        "content": LayoutContentOutputTypeDef,
+        "createdTime": datetime,
+        "deleted": bool,
+        "lastModifiedTime": datetime,
         "layoutArn": str,
         "layoutId": str,
         "name": str,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateLayoutRequestRequestTypeDef = TypedDict(
+    "CreateLayoutRequestRequestTypeDef",
+    {
+        "content": LayoutContentTypeDef,
+        "domainId": str,
+        "name": str,
+    },
+)
+LayoutContentUnionTypeDef = Union[LayoutContentTypeDef, LayoutContentOutputTypeDef]
 UpdateLayoutRequestRequestTypeDef = TypedDict(
     "UpdateLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
         "content": NotRequired[LayoutContentTypeDef],
         "name": NotRequired[str],
```

### Comparing `mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases.egg-info/PKG-INFO` & `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.34.24
-Summary: Type annotations for boto3.ConnectCases 1.34.24 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.94
+Summary: Type annotations for boto3.ConnectCases 1.34.94 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcases)](https://pepy.tech/project/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.34.24](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-connectcases-1.34.24/mypy_boto3_connectcases.egg-info/SOURCES.txt` & `mypy_boto3_connectcases-1.34.94/mypy_boto3_connectcases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.34.24/setup.py` & `mypy_boto3_connectcases-1.34.94/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connectcases",
-    version="1.34.24",
+    version="1.34.94",
     packages=["mypy_boto3_connectcases"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.ConnectCases 1.34.24 service generated with mypy-boto3-builder"
-        " 7.23.1"
-    ),
+    description="Type annotations for boto3.ConnectCases 1.34.94 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

