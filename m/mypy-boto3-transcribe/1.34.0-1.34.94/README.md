# Comparing `tmp/mypy-boto3-transcribe-1.34.0.tar.gz` & `tmp/mypy_boto3_transcribe-1.34.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-transcribe-1.34.0.tar", last modified: Wed Dec 13 21:24:02 2023, max compression
+gzip compressed data, was "mypy_boto3_transcribe-1.34.94.tar", last modified: Mon Apr 29 19:32:09 2024, max compression
```

## Comparing `mypy-boto3-transcribe-1.34.0.tar` & `mypy_boto3_transcribe-1.34.94.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:02.603406 mypy-boto3-transcribe-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:20:46.000000 mypy-boto3-transcribe-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12266 2023-12-13 21:24:02.603406 mypy-boto3-transcribe-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2023-12-13 21:20:46.000000 mypy-boto3-transcribe-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:02.603406 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2023-12-13 21:20:46.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-12-13 21:20:46.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-13 21:20:46.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32744 2023-12-13 21:20:46.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    32740 2023-12-13 21:20:46.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12224 2023-12-13 21:20:46.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2023-12-13 21:20:46.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:20:46.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    42148 2023-12-13 21:20:47.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42147 2023-12-13 21:20:47.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:20:46.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:02.603406 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12266 2023-12-13 21:24:02.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-13 21:24:02.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:24:02.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:24:02.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:24:02.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 21:24:02.000000 mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:24:02.603406 mypy-boto3-transcribe-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2023-12-13 21:20:46.000000 mypy-boto3-transcribe-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:09.726770 mypy_boto3_transcribe-1.34.94/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 19:31:54.000000 mypy_boto3_transcribe-1.34.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-04-29 19:32:09.726770 mypy_boto3_transcribe-1.34.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-04-29 19:31:54.000000 mypy_boto3_transcribe-1.34.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:09.726770 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-29 19:31:54.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-29 19:31:54.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-29 19:31:54.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32871 2024-04-29 19:31:55.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32868 2024-04-29 19:31:54.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12657 2024-04-29 19:31:55.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12657 2024-04-29 19:31:55.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:31:54.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    46022 2024-04-29 19:31:56.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46022 2024-04-29 19:31:55.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 19:31:54.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:09.726770 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-04-29 19:32:09.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-29 19:32:09.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:09.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:09.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 19:32:09.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 19:32:09.000000 mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:32:09.726770 mypy_boto3_transcribe-1.34.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-29 19:31:54.000000 mypy_boto3_transcribe-1.34.94/setup.py
```

### Comparing `mypy-boto3-transcribe-1.34.0/LICENSE` & `mypy_boto3_transcribe-1.34.94/LICENSE`

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

### Comparing `mypy-boto3-transcribe-1.34.0/PKG-INFO` & `mypy_boto3_transcribe-1.34.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transcribe
-Version: 1.34.0
-Summary: Type annotations for boto3.TranscribeService 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.94
+Summary: Type annotations for boto3.TranscribeService 1.34.94 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/
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
 
 <a id="mypy-boto3-transcribe"></a>
 
 # mypy-boto3-transcribe
 
 [![PyPI - mypy-boto3-transcribe](https://img.shields.io/pypi/v/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transcribe)](https://pepy.tech/project/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
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
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-transcribe-1.34.0/README.md` & `mypy_boto3_transcribe-1.34.94/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transcribe)](https://pepy.tech/project/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
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
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/__main__.py` & `mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TranscribeService 1.34.0\nVersion:         1.34.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.TranscribeService 1.34.94\n"
+        "Version:         1.34.94\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService\n"
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

### Comparing `mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/client.py` & `mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     MedicalScribeJobStatusType,
     ModelStatusType,
     TranscriptionJobStatusType,
     TypeType,
     VocabularyStateType,
 )
 from .type_defs import (
-    CallAnalyticsJobSettingsTypeDef,
+    CallAnalyticsJobSettingsUnionTypeDef,
     ChannelDefinitionTypeDef,
-    ContentRedactionTypeDef,
+    ContentRedactionUnionTypeDef,
     CreateCallAnalyticsCategoryResponseTypeDef,
     CreateLanguageModelResponseTypeDef,
     CreateMedicalVocabularyResponseTypeDef,
     CreateVocabularyFilterResponseTypeDef,
     CreateVocabularyResponseTypeDef,
     DescribeLanguageModelResponseTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -65,35 +65,34 @@
     ListVocabulariesResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MediaTypeDef,
     MedicalScribeChannelDefinitionTypeDef,
     MedicalScribeSettingsTypeDef,
     MedicalTranscriptionSettingTypeDef,
     ModelSettingsTypeDef,
-    RuleTypeDef,
+    RuleUnionTypeDef,
     SettingsTypeDef,
     StartCallAnalyticsJobResponseTypeDef,
     StartMedicalScribeJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     SubtitlesTypeDef,
     TagTypeDef,
-    ToxicityDetectionSettingsTypeDef,
+    ToxicityDetectionSettingsUnionTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
     UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyResponseTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("TranscribeServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -140,15 +139,19 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#close)
         """
 
     def create_call_analytics_category(
-        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
+        self,
+        *,
+        CategoryName: str,
+        Rules: Sequence[RuleUnionTypeDef],
+        InputType: InputTypeType = ...,
     ) -> CreateCallAnalyticsCategoryResponseTypeDef:
         """
         Creates a new Call Analytics category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_call_analytics_category)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_call_analytics_category)
         """
@@ -156,30 +159,30 @@
     def create_language_model(
         self,
         *,
         LanguageCode: CLMLanguageCodeType,
         BaseModelName: BaseModelNameType,
         ModelName: str,
         InputDataConfig: InputDataConfigTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLanguageModelResponseTypeDef:
         """
         Creates a new custom language model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_language_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_language_model)
         """
 
     def create_medical_vocabulary(
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         VocabularyFileUri: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMedicalVocabularyResponseTypeDef:
         """
         Creates a new custom medical vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_medical_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_medical_vocabulary)
         """
@@ -188,15 +191,15 @@
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         Phrases: Sequence[str] = ...,
         VocabularyFileUri: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> CreateVocabularyResponseTypeDef:
         """
         Creates a new custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_vocabulary)
         """
@@ -205,15 +208,15 @@
         self,
         *,
         VocabularyFilterName: str,
         LanguageCode: LanguageCodeType,
         Words: Sequence[str] = ...,
         VocabularyFilterFileUri: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> CreateVocabularyFilterResponseTypeDef:
         """
         Creates a new custom vocabulary filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_vocabulary_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_vocabulary_filter)
         """
@@ -410,75 +413,75 @@
 
     def list_call_analytics_jobs(
         self,
         *,
         Status: CallAnalyticsJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCallAnalyticsJobsResponseTypeDef:
         """
         Provides a list of Call Analytics jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_call_analytics_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_call_analytics_jobs)
         """
 
     def list_language_models(
         self,
         *,
         StatusEquals: ModelStatusType = ...,
         NameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLanguageModelsResponseTypeDef:
         """
         Provides a list of custom language models that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_language_models)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_language_models)
         """
 
     def list_medical_scribe_jobs(
         self,
         *,
         Status: MedicalScribeJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListMedicalScribeJobsResponseTypeDef:
         """
         Provides a list of Medical Scribe jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_scribe_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_medical_scribe_jobs)
         """
 
     def list_medical_transcription_jobs(
         self,
         *,
         Status: TranscriptionJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListMedicalTranscriptionJobsResponseTypeDef:
         """
         Provides a list of medical transcription jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_transcription_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_medical_transcription_jobs)
         """
 
     def list_medical_vocabularies(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         StateEquals: VocabularyStateType = ...,
-        NameContains: str = ...
+        NameContains: str = ...,
     ) -> ListMedicalVocabulariesResponseTypeDef:
         """
         Provides a list of custom medical vocabularies that match the specified
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_medical_vocabularies)
@@ -496,30 +499,30 @@
 
     def list_transcription_jobs(
         self,
         *,
         Status: TranscriptionJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTranscriptionJobsResponseTypeDef:
         """
         Provides a list of transcription jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_transcription_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_transcription_jobs)
         """
 
     def list_vocabularies(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         StateEquals: VocabularyStateType = ...,
-        NameContains: str = ...
+        NameContains: str = ...,
     ) -> ListVocabulariesResponseTypeDef:
         """
         Provides a list of custom vocabularies that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_vocabularies)
         """
@@ -538,16 +541,16 @@
         self,
         *,
         CallAnalyticsJobName: str,
         Media: MediaTypeDef,
         OutputLocation: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         DataAccessRoleArn: str = ...,
-        Settings: CallAnalyticsJobSettingsTypeDef = ...,
-        ChannelDefinitions: Sequence[ChannelDefinitionTypeDef] = ...
+        Settings: CallAnalyticsJobSettingsUnionTypeDef = ...,
+        ChannelDefinitions: Sequence[ChannelDefinitionTypeDef] = ...,
     ) -> StartCallAnalyticsJobResponseTypeDef:
         """
         Transcribes the audio from a customer service call and applies any additional
         Request Parameters you choose to include in your
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_call_analytics_job)
@@ -561,15 +564,15 @@
         Media: MediaTypeDef,
         OutputBucketName: str,
         DataAccessRoleArn: str,
         Settings: MedicalScribeSettingsTypeDef,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         ChannelDefinitions: Sequence[MedicalScribeChannelDefinitionTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartMedicalScribeJobResponseTypeDef:
         """
         Transcribes patient-clinician conversations and generates clinical notes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_medical_scribe_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#start_medical_scribe_job)
         """
@@ -586,15 +589,15 @@
         MediaSampleRateHertz: int = ...,
         MediaFormat: MediaFormatType = ...,
         OutputKey: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         Settings: MedicalTranscriptionSettingTypeDef = ...,
         ContentIdentificationType: Literal["PHI"] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartMedicalTranscriptionJobResponseTypeDef:
         """
         Transcribes the audio from a medical dictation or conversation and applies any
         additional Request Parameters you choose to include in your
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_medical_transcription_job)
@@ -612,22 +615,22 @@
         OutputBucketName: str = ...,
         OutputKey: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         Settings: SettingsTypeDef = ...,
         ModelSettings: ModelSettingsTypeDef = ...,
         JobExecutionSettings: JobExecutionSettingsTypeDef = ...,
-        ContentRedaction: ContentRedactionTypeDef = ...,
+        ContentRedaction: ContentRedactionUnionTypeDef = ...,
         IdentifyLanguage: bool = ...,
         IdentifyMultipleLanguages: bool = ...,
         LanguageOptions: Sequence[LanguageCodeType] = ...,
         Subtitles: SubtitlesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...,
-        ToxicityDetection: Sequence[ToxicityDetectionSettingsTypeDef] = ...
+        ToxicityDetection: Sequence[ToxicityDetectionSettingsUnionTypeDef] = ...,
     ) -> StartTranscriptionJobResponseTypeDef:
         """
         Transcribes the audio from a media file and applies any additional Request
         Parameters you choose to include in your
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_transcription_job)
@@ -649,15 +652,19 @@
         Removes the specified tags from the specified Amazon Transcribe resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#untag_resource)
         """
 
     def update_call_analytics_category(
-        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
+        self,
+        *,
+        CategoryName: str,
+        Rules: Sequence[RuleUnionTypeDef],
+        InputType: InputTypeType = ...,
     ) -> UpdateCallAnalyticsCategoryResponseTypeDef:
         """
         Updates the specified Call Analytics category with new rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_call_analytics_category)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#update_call_analytics_category)
         """
@@ -675,30 +682,30 @@
     def update_vocabulary(
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         Phrases: Sequence[str] = ...,
         VocabularyFileUri: str = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> UpdateVocabularyResponseTypeDef:
         """
         Updates an existing custom vocabulary with new values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#update_vocabulary)
         """
 
     def update_vocabulary_filter(
         self,
         *,
         VocabularyFilterName: str,
         Words: Sequence[str] = ...,
         VocabularyFilterFileUri: str = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> UpdateVocabularyFilterResponseTypeDef:
         """
         Updates an existing custom vocabulary filter with a new list of words.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_vocabulary_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#update_vocabulary_filter)
         """
```

### Comparing `mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/client.pyi` & `mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     MedicalScribeJobStatusType,
     ModelStatusType,
     TranscriptionJobStatusType,
     TypeType,
     VocabularyStateType,
 )
 from .type_defs import (
-    CallAnalyticsJobSettingsTypeDef,
+    CallAnalyticsJobSettingsUnionTypeDef,
     ChannelDefinitionTypeDef,
-    ContentRedactionTypeDef,
+    ContentRedactionUnionTypeDef,
     CreateCallAnalyticsCategoryResponseTypeDef,
     CreateLanguageModelResponseTypeDef,
     CreateMedicalVocabularyResponseTypeDef,
     CreateVocabularyFilterResponseTypeDef,
     CreateVocabularyResponseTypeDef,
     DescribeLanguageModelResponseTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -65,23 +65,23 @@
     ListVocabulariesResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MediaTypeDef,
     MedicalScribeChannelDefinitionTypeDef,
     MedicalScribeSettingsTypeDef,
     MedicalTranscriptionSettingTypeDef,
     ModelSettingsTypeDef,
-    RuleTypeDef,
+    RuleUnionTypeDef,
     SettingsTypeDef,
     StartCallAnalyticsJobResponseTypeDef,
     StartMedicalScribeJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     SubtitlesTypeDef,
     TagTypeDef,
-    ToxicityDetectionSettingsTypeDef,
+    ToxicityDetectionSettingsUnionTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
     UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyResponseTypeDef,
 )
 
 if sys.version_info >= (3, 12):
@@ -136,15 +136,19 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#close)
         """
 
     def create_call_analytics_category(
-        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
+        self,
+        *,
+        CategoryName: str,
+        Rules: Sequence[RuleUnionTypeDef],
+        InputType: InputTypeType = ...,
     ) -> CreateCallAnalyticsCategoryResponseTypeDef:
         """
         Creates a new Call Analytics category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_call_analytics_category)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_call_analytics_category)
         """
@@ -152,30 +156,30 @@
     def create_language_model(
         self,
         *,
         LanguageCode: CLMLanguageCodeType,
         BaseModelName: BaseModelNameType,
         ModelName: str,
         InputDataConfig: InputDataConfigTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLanguageModelResponseTypeDef:
         """
         Creates a new custom language model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_language_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_language_model)
         """
 
     def create_medical_vocabulary(
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         VocabularyFileUri: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMedicalVocabularyResponseTypeDef:
         """
         Creates a new custom medical vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_medical_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_medical_vocabulary)
         """
@@ -184,15 +188,15 @@
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         Phrases: Sequence[str] = ...,
         VocabularyFileUri: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> CreateVocabularyResponseTypeDef:
         """
         Creates a new custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_vocabulary)
         """
@@ -201,15 +205,15 @@
         self,
         *,
         VocabularyFilterName: str,
         LanguageCode: LanguageCodeType,
         Words: Sequence[str] = ...,
         VocabularyFilterFileUri: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> CreateVocabularyFilterResponseTypeDef:
         """
         Creates a new custom vocabulary filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_vocabulary_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#create_vocabulary_filter)
         """
@@ -406,75 +410,75 @@
 
     def list_call_analytics_jobs(
         self,
         *,
         Status: CallAnalyticsJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCallAnalyticsJobsResponseTypeDef:
         """
         Provides a list of Call Analytics jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_call_analytics_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_call_analytics_jobs)
         """
 
     def list_language_models(
         self,
         *,
         StatusEquals: ModelStatusType = ...,
         NameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLanguageModelsResponseTypeDef:
         """
         Provides a list of custom language models that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_language_models)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_language_models)
         """
 
     def list_medical_scribe_jobs(
         self,
         *,
         Status: MedicalScribeJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListMedicalScribeJobsResponseTypeDef:
         """
         Provides a list of Medical Scribe jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_scribe_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_medical_scribe_jobs)
         """
 
     def list_medical_transcription_jobs(
         self,
         *,
         Status: TranscriptionJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListMedicalTranscriptionJobsResponseTypeDef:
         """
         Provides a list of medical transcription jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_transcription_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_medical_transcription_jobs)
         """
 
     def list_medical_vocabularies(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         StateEquals: VocabularyStateType = ...,
-        NameContains: str = ...
+        NameContains: str = ...,
     ) -> ListMedicalVocabulariesResponseTypeDef:
         """
         Provides a list of custom medical vocabularies that match the specified
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_medical_vocabularies)
@@ -492,30 +496,30 @@
 
     def list_transcription_jobs(
         self,
         *,
         Status: TranscriptionJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTranscriptionJobsResponseTypeDef:
         """
         Provides a list of transcription jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_transcription_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_transcription_jobs)
         """
 
     def list_vocabularies(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         StateEquals: VocabularyStateType = ...,
-        NameContains: str = ...
+        NameContains: str = ...,
     ) -> ListVocabulariesResponseTypeDef:
         """
         Provides a list of custom vocabularies that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_vocabularies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#list_vocabularies)
         """
@@ -534,16 +538,16 @@
         self,
         *,
         CallAnalyticsJobName: str,
         Media: MediaTypeDef,
         OutputLocation: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         DataAccessRoleArn: str = ...,
-        Settings: CallAnalyticsJobSettingsTypeDef = ...,
-        ChannelDefinitions: Sequence[ChannelDefinitionTypeDef] = ...
+        Settings: CallAnalyticsJobSettingsUnionTypeDef = ...,
+        ChannelDefinitions: Sequence[ChannelDefinitionTypeDef] = ...,
     ) -> StartCallAnalyticsJobResponseTypeDef:
         """
         Transcribes the audio from a customer service call and applies any additional
         Request Parameters you choose to include in your
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_call_analytics_job)
@@ -557,15 +561,15 @@
         Media: MediaTypeDef,
         OutputBucketName: str,
         DataAccessRoleArn: str,
         Settings: MedicalScribeSettingsTypeDef,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         ChannelDefinitions: Sequence[MedicalScribeChannelDefinitionTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartMedicalScribeJobResponseTypeDef:
         """
         Transcribes patient-clinician conversations and generates clinical notes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_medical_scribe_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#start_medical_scribe_job)
         """
@@ -582,15 +586,15 @@
         MediaSampleRateHertz: int = ...,
         MediaFormat: MediaFormatType = ...,
         OutputKey: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         Settings: MedicalTranscriptionSettingTypeDef = ...,
         ContentIdentificationType: Literal["PHI"] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartMedicalTranscriptionJobResponseTypeDef:
         """
         Transcribes the audio from a medical dictation or conversation and applies any
         additional Request Parameters you choose to include in your
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_medical_transcription_job)
@@ -608,22 +612,22 @@
         OutputBucketName: str = ...,
         OutputKey: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         Settings: SettingsTypeDef = ...,
         ModelSettings: ModelSettingsTypeDef = ...,
         JobExecutionSettings: JobExecutionSettingsTypeDef = ...,
-        ContentRedaction: ContentRedactionTypeDef = ...,
+        ContentRedaction: ContentRedactionUnionTypeDef = ...,
         IdentifyLanguage: bool = ...,
         IdentifyMultipleLanguages: bool = ...,
         LanguageOptions: Sequence[LanguageCodeType] = ...,
         Subtitles: SubtitlesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...,
-        ToxicityDetection: Sequence[ToxicityDetectionSettingsTypeDef] = ...
+        ToxicityDetection: Sequence[ToxicityDetectionSettingsUnionTypeDef] = ...,
     ) -> StartTranscriptionJobResponseTypeDef:
         """
         Transcribes the audio from a media file and applies any additional Request
         Parameters you choose to include in your
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_transcription_job)
@@ -645,15 +649,19 @@
         Removes the specified tags from the specified Amazon Transcribe resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#untag_resource)
         """
 
     def update_call_analytics_category(
-        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
+        self,
+        *,
+        CategoryName: str,
+        Rules: Sequence[RuleUnionTypeDef],
+        InputType: InputTypeType = ...,
     ) -> UpdateCallAnalyticsCategoryResponseTypeDef:
         """
         Updates the specified Call Analytics category with new rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_call_analytics_category)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#update_call_analytics_category)
         """
@@ -671,30 +679,30 @@
     def update_vocabulary(
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         Phrases: Sequence[str] = ...,
         VocabularyFileUri: str = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> UpdateVocabularyResponseTypeDef:
         """
         Updates an existing custom vocabulary with new values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#update_vocabulary)
         """
 
     def update_vocabulary_filter(
         self,
         *,
         VocabularyFilterName: str,
         Words: Sequence[str] = ...,
         VocabularyFilterFileUri: str = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> UpdateVocabularyFilterResponseTypeDef:
         """
         Updates an existing custom vocabulary filter with a new list of words.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_vocabulary_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#update_vocabulary_filter)
         """
```

### Comparing `mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/literals.py` & `mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "BaseModelNameType",
     "CLMLanguageCodeType",
+    "CallAnalyticsFeatureType",
     "CallAnalyticsJobStatusType",
+    "CallAnalyticsSkippedReasonCodeType",
     "InputTypeType",
     "LanguageCodeType",
     "MediaFormatType",
     "MedicalContentIdentificationTypeType",
     "MedicalScribeJobStatusType",
     "MedicalScribeLanguageCodeType",
     "MedicalScribeParticipantRoleType",
@@ -48,18 +49,21 @@
     "VocabularyStateType",
     "TranscribeServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 BaseModelNameType = Literal["NarrowBand", "WideBand"]
 CLMLanguageCodeType = Literal["de-DE", "en-AU", "en-GB", "en-US", "es-US", "hi-IN", "ja-JP"]
+CallAnalyticsFeatureType = Literal["GENERATIVE_SUMMARIZATION"]
 CallAnalyticsJobStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "QUEUED"]
+CallAnalyticsSkippedReasonCodeType = Literal[
+    "FAILED_SAFETY_GUIDELINES", "INSUFFICIENT_CONVERSATION_CONTENT"
+]
 InputTypeType = Literal["POST_CALL", "REAL_TIME"]
 LanguageCodeType = Literal[
     "ab-GE",
     "af-ZA",
     "ar-AE",
     "ar-SA",
     "ast-ES",
@@ -218,14 +222,15 @@
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
@@ -236,14 +241,15 @@
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
@@ -261,14 +267,15 @@
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
@@ -281,24 +288,26 @@
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
@@ -359,15 +368,14 @@
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
@@ -439,17 +447,19 @@
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
@@ -494,14 +504,15 @@
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
@@ -539,19 +550,21 @@
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

### Comparing `mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/literals.pyi` & `mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,17 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "BaseModelNameType",
     "CLMLanguageCodeType",
+    "CallAnalyticsFeatureType",
     "CallAnalyticsJobStatusType",
+    "CallAnalyticsSkippedReasonCodeType",
     "InputTypeType",
     "LanguageCodeType",
     "MediaFormatType",
     "MedicalContentIdentificationTypeType",
     "MedicalScribeJobStatusType",
     "MedicalScribeLanguageCodeType",
     "MedicalScribeParticipantRoleType",
@@ -49,15 +51,19 @@
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 BaseModelNameType = Literal["NarrowBand", "WideBand"]
 CLMLanguageCodeType = Literal["de-DE", "en-AU", "en-GB", "en-US", "es-US", "hi-IN", "ja-JP"]
+CallAnalyticsFeatureType = Literal["GENERATIVE_SUMMARIZATION"]
 CallAnalyticsJobStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "QUEUED"]
+CallAnalyticsSkippedReasonCodeType = Literal[
+    "FAILED_SAFETY_GUIDELINES", "INSUFFICIENT_CONVERSATION_CONTENT"
+]
 InputTypeType = Literal["POST_CALL", "REAL_TIME"]
 LanguageCodeType = Literal[
     "ab-GE",
     "af-ZA",
     "ar-AE",
     "ar-SA",
     "ast-ES",
@@ -216,14 +222,15 @@
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
@@ -234,14 +241,15 @@
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
@@ -259,14 +267,15 @@
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
@@ -279,24 +288,26 @@
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
@@ -357,15 +368,14 @@
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
@@ -437,17 +447,19 @@
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
@@ -492,14 +504,15 @@
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
@@ -537,19 +550,21 @@
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

### Comparing `mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/type_defs.py` & `mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 
     data: AbsoluteTimeRangeTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     BaseModelNameType,
     CallAnalyticsJobStatusType,
+    CallAnalyticsSkippedReasonCodeType,
     CLMLanguageCodeType,
     InputTypeType,
     LanguageCodeType,
     MediaFormatType,
     MedicalScribeJobStatusType,
     MedicalScribeParticipantRoleType,
     ModelStatusType,
@@ -47,21 +48,21 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AbsoluteTimeRangeTypeDef",
-    "ContentRedactionTypeDef",
+    "CallAnalyticsSkippedFeatureTypeDef",
+    "ContentRedactionOutputTypeDef",
     "LanguageIdSettingsTypeDef",
     "SummarizationTypeDef",
-    "CallAnalyticsJobSummaryTypeDef",
+    "ContentRedactionTypeDef",
     "ChannelDefinitionTypeDef",
     "MediaTypeDef",
     "TranscriptTypeDef",
     "ResponseMetadataTypeDef",
     "InputDataConfigTypeDef",
     "TagTypeDef",
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
@@ -103,90 +104,109 @@
     "MedicalScribeOutputTypeDef",
     "MedicalScribeSettingsTypeDef",
     "MedicalTranscriptTypeDef",
     "MedicalTranscriptionSettingTypeDef",
     "ModelSettingsTypeDef",
     "SettingsTypeDef",
     "SubtitlesTypeDef",
-    "ToxicityDetectionSettingsTypeDef",
     "SubtitlesOutputTypeDef",
+    "ToxicityDetectionSettingsOutputTypeDef",
+    "ToxicityDetectionSettingsTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMedicalVocabularyRequestRequestTypeDef",
     "UpdateVocabularyFilterRequestRequestTypeDef",
     "UpdateVocabularyRequestRequestTypeDef",
+    "CallAnalyticsJobDetailsTypeDef",
+    "CallAnalyticsJobSettingsOutputTypeDef",
     "CallAnalyticsJobSettingsTypeDef",
+    "ContentRedactionUnionTypeDef",
     "CreateMedicalVocabularyResponseTypeDef",
     "CreateVocabularyFilterResponseTypeDef",
     "CreateVocabularyResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetMedicalVocabularyResponseTypeDef",
     "GetVocabularyFilterResponseTypeDef",
     "GetVocabularyResponseTypeDef",
-    "ListCallAnalyticsJobsResponseTypeDef",
     "UpdateMedicalVocabularyResponseTypeDef",
     "UpdateVocabularyFilterResponseTypeDef",
     "UpdateVocabularyResponseTypeDef",
     "CreateLanguageModelResponseTypeDef",
     "LanguageModelTypeDef",
     "CreateLanguageModelRequestRequestTypeDef",
     "CreateMedicalVocabularyRequestRequestTypeDef",
     "CreateVocabularyFilterRequestRequestTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "InterruptionFilterTypeDef",
     "NonTalkTimeFilterTypeDef",
+    "SentimentFilterOutputTypeDef",
     "SentimentFilterTypeDef",
+    "TranscriptFilterOutputTypeDef",
     "TranscriptFilterTypeDef",
     "ListMedicalScribeJobsResponseTypeDef",
     "ListMedicalTranscriptionJobsResponseTypeDef",
     "ListMedicalVocabulariesResponseTypeDef",
     "ListVocabulariesResponseTypeDef",
     "ListVocabularyFiltersResponseTypeDef",
     "MedicalScribeJobTypeDef",
     "StartMedicalScribeJobRequestRequestTypeDef",
     "MedicalTranscriptionJobTypeDef",
     "StartMedicalTranscriptionJobRequestRequestTypeDef",
-    "StartTranscriptionJobRequestRequestTypeDef",
     "TranscriptionJobSummaryTypeDef",
     "TranscriptionJobTypeDef",
+    "ToxicityDetectionSettingsUnionTypeDef",
+    "CallAnalyticsJobSummaryTypeDef",
     "CallAnalyticsJobTypeDef",
+    "CallAnalyticsJobSettingsUnionTypeDef",
     "StartCallAnalyticsJobRequestRequestTypeDef",
     "DescribeLanguageModelResponseTypeDef",
     "ListLanguageModelsResponseTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
     "GetMedicalScribeJobResponseTypeDef",
     "StartMedicalScribeJobResponseTypeDef",
     "GetMedicalTranscriptionJobResponseTypeDef",
     "StartMedicalTranscriptionJobResponseTypeDef",
     "ListTranscriptionJobsResponseTypeDef",
     "GetTranscriptionJobResponseTypeDef",
     "StartTranscriptionJobResponseTypeDef",
+    "StartTranscriptionJobRequestRequestTypeDef",
+    "ListCallAnalyticsJobsResponseTypeDef",
     "GetCallAnalyticsJobResponseTypeDef",
     "StartCallAnalyticsJobResponseTypeDef",
     "CategoryPropertiesTypeDef",
-    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
-    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
+    "RuleUnionTypeDef",
     "CreateCallAnalyticsCategoryResponseTypeDef",
     "GetCallAnalyticsCategoryResponseTypeDef",
     "ListCallAnalyticsCategoriesResponseTypeDef",
     "UpdateCallAnalyticsCategoryResponseTypeDef",
+    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
+    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
 )
 
 AbsoluteTimeRangeTypeDef = TypedDict(
     "AbsoluteTimeRangeTypeDef",
     {
         "StartTime": NotRequired[int],
         "EndTime": NotRequired[int],
         "First": NotRequired[int],
         "Last": NotRequired[int],
     },
 )
-ContentRedactionTypeDef = TypedDict(
-    "ContentRedactionTypeDef",
+CallAnalyticsSkippedFeatureTypeDef = TypedDict(
+    "CallAnalyticsSkippedFeatureTypeDef",
+    {
+        "Feature": NotRequired[Literal["GENERATIVE_SUMMARIZATION"]],
+        "ReasonCode": NotRequired[CallAnalyticsSkippedReasonCodeType],
+        "Message": NotRequired[str],
+    },
+)
+ContentRedactionOutputTypeDef = TypedDict(
+    "ContentRedactionOutputTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
         "PiiEntityTypes": NotRequired[List[PiiEntityTypeType]],
     },
 )
 LanguageIdSettingsTypeDef = TypedDict(
@@ -199,24 +219,20 @@
 )
 SummarizationTypeDef = TypedDict(
     "SummarizationTypeDef",
     {
         "GenerateAbstractiveSummary": bool,
     },
 )
-CallAnalyticsJobSummaryTypeDef = TypedDict(
-    "CallAnalyticsJobSummaryTypeDef",
+ContentRedactionTypeDef = TypedDict(
+    "ContentRedactionTypeDef",
     {
-        "CallAnalyticsJobName": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "StartTime": NotRequired[datetime],
-        "CompletionTime": NotRequired[datetime],
-        "LanguageCode": NotRequired[LanguageCodeType],
-        "CallAnalyticsJobStatus": NotRequired[CallAnalyticsJobStatusType],
-        "FailureReason": NotRequired[str],
+        "RedactionType": Literal["PII"],
+        "RedactionOutput": RedactionOutputType,
+        "PiiEntityTypes": NotRequired[Sequence[PiiEntityTypeType]],
     },
 )
 ChannelDefinitionTypeDef = TypedDict(
     "ChannelDefinitionTypeDef",
     {
         "ChannelId": NotRequired[int],
         "ParticipantRole": NotRequired[ParticipantRoleType],
@@ -236,18 +252,18 @@
         "RedactedTranscriptFileUri": NotRequired[str],
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
 InputDataConfigTypeDef = TypedDict(
     "InputDataConfigTypeDef",
     {
         "S3Uri": str,
         "DataAccessRoleArn": str,
@@ -585,28 +601,34 @@
 SubtitlesTypeDef = TypedDict(
     "SubtitlesTypeDef",
     {
         "Formats": NotRequired[Sequence[SubtitleFormatType]],
         "OutputStartIndex": NotRequired[int],
     },
 )
-ToxicityDetectionSettingsTypeDef = TypedDict(
-    "ToxicityDetectionSettingsTypeDef",
-    {
-        "ToxicityCategories": List[Literal["ALL"]],
-    },
-)
 SubtitlesOutputTypeDef = TypedDict(
     "SubtitlesOutputTypeDef",
     {
         "Formats": NotRequired[List[SubtitleFormatType]],
         "SubtitleFileUris": NotRequired[List[str]],
         "OutputStartIndex": NotRequired[int],
     },
 )
+ToxicityDetectionSettingsOutputTypeDef = TypedDict(
+    "ToxicityDetectionSettingsOutputTypeDef",
+    {
+        "ToxicityCategories": List[Literal["ALL"]],
+    },
+)
+ToxicityDetectionSettingsTypeDef = TypedDict(
+    "ToxicityDetectionSettingsTypeDef",
+    {
+        "ToxicityCategories": Sequence[Literal["ALL"]],
+    },
+)
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -633,27 +655,47 @@
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "Phrases": NotRequired[Sequence[str]],
         "VocabularyFileUri": NotRequired[str],
         "DataAccessRoleArn": NotRequired[str],
     },
 )
+CallAnalyticsJobDetailsTypeDef = TypedDict(
+    "CallAnalyticsJobDetailsTypeDef",
+    {
+        "Skipped": NotRequired[List[CallAnalyticsSkippedFeatureTypeDef]],
+    },
+)
+CallAnalyticsJobSettingsOutputTypeDef = TypedDict(
+    "CallAnalyticsJobSettingsOutputTypeDef",
+    {
+        "VocabularyName": NotRequired[str],
+        "VocabularyFilterName": NotRequired[str],
+        "VocabularyFilterMethod": NotRequired[VocabularyFilterMethodType],
+        "LanguageModelName": NotRequired[str],
+        "ContentRedaction": NotRequired[ContentRedactionOutputTypeDef],
+        "LanguageOptions": NotRequired[List[LanguageCodeType]],
+        "LanguageIdSettings": NotRequired[Dict[LanguageCodeType, LanguageIdSettingsTypeDef]],
+        "Summarization": NotRequired[SummarizationTypeDef],
+    },
+)
 CallAnalyticsJobSettingsTypeDef = TypedDict(
     "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": NotRequired[str],
         "VocabularyFilterName": NotRequired[str],
         "VocabularyFilterMethod": NotRequired[VocabularyFilterMethodType],
         "LanguageModelName": NotRequired[str],
         "ContentRedaction": NotRequired[ContentRedactionTypeDef],
-        "LanguageOptions": NotRequired[List[LanguageCodeType]],
-        "LanguageIdSettings": NotRequired[Dict[LanguageCodeType, LanguageIdSettingsTypeDef]],
+        "LanguageOptions": NotRequired[Sequence[LanguageCodeType]],
+        "LanguageIdSettings": NotRequired[Mapping[LanguageCodeType, LanguageIdSettingsTypeDef]],
         "Summarization": NotRequired[SummarizationTypeDef],
     },
 )
+ContentRedactionUnionTypeDef = Union[ContentRedactionTypeDef, ContentRedactionOutputTypeDef]
 CreateMedicalVocabularyResponseTypeDef = TypedDict(
     "CreateMedicalVocabularyResponseTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "VocabularyState": VocabularyStateType,
         "LastModifiedTime": datetime,
@@ -717,23 +759,14 @@
         "VocabularyState": VocabularyStateType,
         "LastModifiedTime": datetime,
         "FailureReason": str,
         "DownloadUri": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListCallAnalyticsJobsResponseTypeDef = TypedDict(
-    "ListCallAnalyticsJobsResponseTypeDef",
-    {
-        "Status": CallAnalyticsJobStatusType,
-        "NextToken": str,
-        "CallAnalyticsJobSummaries": List[CallAnalyticsJobSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 UpdateMedicalVocabularyResponseTypeDef = TypedDict(
     "UpdateMedicalVocabularyResponseTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
         "VocabularyState": VocabularyStateType,
@@ -855,24 +888,45 @@
     {
         "Threshold": NotRequired[int],
         "AbsoluteTimeRange": NotRequired[AbsoluteTimeRangeTypeDef],
         "RelativeTimeRange": NotRequired[RelativeTimeRangeTypeDef],
         "Negate": NotRequired[bool],
     },
 )
+SentimentFilterOutputTypeDef = TypedDict(
+    "SentimentFilterOutputTypeDef",
+    {
+        "Sentiments": List[SentimentValueType],
+        "AbsoluteTimeRange": NotRequired[AbsoluteTimeRangeTypeDef],
+        "RelativeTimeRange": NotRequired[RelativeTimeRangeTypeDef],
+        "ParticipantRole": NotRequired[ParticipantRoleType],
+        "Negate": NotRequired[bool],
+    },
+)
 SentimentFilterTypeDef = TypedDict(
     "SentimentFilterTypeDef",
     {
         "Sentiments": Sequence[SentimentValueType],
         "AbsoluteTimeRange": NotRequired[AbsoluteTimeRangeTypeDef],
         "RelativeTimeRange": NotRequired[RelativeTimeRangeTypeDef],
         "ParticipantRole": NotRequired[ParticipantRoleType],
         "Negate": NotRequired[bool],
     },
 )
+TranscriptFilterOutputTypeDef = TypedDict(
+    "TranscriptFilterOutputTypeDef",
+    {
+        "TranscriptFilterType": Literal["EXACT"],
+        "Targets": List[str],
+        "AbsoluteTimeRange": NotRequired[AbsoluteTimeRangeTypeDef],
+        "RelativeTimeRange": NotRequired[RelativeTimeRangeTypeDef],
+        "ParticipantRole": NotRequired[ParticipantRoleType],
+        "Negate": NotRequired[bool],
+    },
+)
 TranscriptFilterTypeDef = TypedDict(
     "TranscriptFilterTypeDef",
     {
         "TranscriptFilterType": Literal["EXACT"],
         "Targets": Sequence[str],
         "AbsoluteTimeRange": NotRequired[AbsoluteTimeRangeTypeDef],
         "RelativeTimeRange": NotRequired[RelativeTimeRangeTypeDef],
@@ -880,52 +934,52 @@
         "Negate": NotRequired[bool],
     },
 )
 ListMedicalScribeJobsResponseTypeDef = TypedDict(
     "ListMedicalScribeJobsResponseTypeDef",
     {
         "Status": MedicalScribeJobStatusType,
-        "NextToken": str,
         "MedicalScribeJobSummaries": List[MedicalScribeJobSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListMedicalTranscriptionJobsResponseTypeDef = TypedDict(
     "ListMedicalTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
-        "NextToken": str,
         "MedicalTranscriptionJobSummaries": List[MedicalTranscriptionJobSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListMedicalVocabulariesResponseTypeDef = TypedDict(
     "ListMedicalVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
-        "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListVocabulariesResponseTypeDef = TypedDict(
     "ListVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
-        "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListVocabularyFiltersResponseTypeDef = TypedDict(
     "ListVocabularyFiltersResponseTypeDef",
     {
-        "NextToken": str,
         "VocabularyFilters": List[VocabularyFilterInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 MedicalScribeJobTypeDef = TypedDict(
     "MedicalScribeJobTypeDef",
     {
         "MedicalScribeJobName": NotRequired[str],
         "MedicalScribeJobStatus": NotRequired[MedicalScribeJobStatusType],
@@ -992,57 +1046,32 @@
         "OutputEncryptionKMSKeyId": NotRequired[str],
         "KMSEncryptionContext": NotRequired[Mapping[str, str]],
         "Settings": NotRequired[MedicalTranscriptionSettingTypeDef],
         "ContentIdentificationType": NotRequired[Literal["PHI"]],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
-StartTranscriptionJobRequestRequestTypeDef = TypedDict(
-    "StartTranscriptionJobRequestRequestTypeDef",
-    {
-        "TranscriptionJobName": str,
-        "Media": MediaTypeDef,
-        "LanguageCode": NotRequired[LanguageCodeType],
-        "MediaSampleRateHertz": NotRequired[int],
-        "MediaFormat": NotRequired[MediaFormatType],
-        "OutputBucketName": NotRequired[str],
-        "OutputKey": NotRequired[str],
-        "OutputEncryptionKMSKeyId": NotRequired[str],
-        "KMSEncryptionContext": NotRequired[Mapping[str, str]],
-        "Settings": NotRequired[SettingsTypeDef],
-        "ModelSettings": NotRequired[ModelSettingsTypeDef],
-        "JobExecutionSettings": NotRequired[JobExecutionSettingsTypeDef],
-        "ContentRedaction": NotRequired[ContentRedactionTypeDef],
-        "IdentifyLanguage": NotRequired[bool],
-        "IdentifyMultipleLanguages": NotRequired[bool],
-        "LanguageOptions": NotRequired[Sequence[LanguageCodeType]],
-        "Subtitles": NotRequired[SubtitlesTypeDef],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "LanguageIdSettings": NotRequired[Mapping[LanguageCodeType, LanguageIdSettingsTypeDef]],
-        "ToxicityDetection": NotRequired[Sequence[ToxicityDetectionSettingsTypeDef]],
-    },
-)
 TranscriptionJobSummaryTypeDef = TypedDict(
     "TranscriptionJobSummaryTypeDef",
     {
         "TranscriptionJobName": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "StartTime": NotRequired[datetime],
         "CompletionTime": NotRequired[datetime],
         "LanguageCode": NotRequired[LanguageCodeType],
         "TranscriptionJobStatus": NotRequired[TranscriptionJobStatusType],
         "FailureReason": NotRequired[str],
         "OutputLocationType": NotRequired[OutputLocationTypeType],
-        "ContentRedaction": NotRequired[ContentRedactionTypeDef],
+        "ContentRedaction": NotRequired[ContentRedactionOutputTypeDef],
         "ModelSettings": NotRequired[ModelSettingsTypeDef],
         "IdentifyLanguage": NotRequired[bool],
         "IdentifyMultipleLanguages": NotRequired[bool],
         "IdentifiedLanguageScore": NotRequired[float],
         "LanguageCodes": NotRequired[List[LanguageCodeItemTypeDef]],
-        "ToxicityDetection": NotRequired[List[ToxicityDetectionSettingsTypeDef]],
+        "ToxicityDetection": NotRequired[List[ToxicityDetectionSettingsOutputTypeDef]],
     },
 )
 TranscriptionJobTypeDef = TypedDict(
     "TranscriptionJobTypeDef",
     {
         "TranscriptionJobName": NotRequired[str],
         "TranscriptionJobStatus": NotRequired[TranscriptionJobStatusType],
@@ -1054,46 +1083,66 @@
         "StartTime": NotRequired[datetime],
         "CreationTime": NotRequired[datetime],
         "CompletionTime": NotRequired[datetime],
         "FailureReason": NotRequired[str],
         "Settings": NotRequired[SettingsTypeDef],
         "ModelSettings": NotRequired[ModelSettingsTypeDef],
         "JobExecutionSettings": NotRequired[JobExecutionSettingsTypeDef],
-        "ContentRedaction": NotRequired[ContentRedactionTypeDef],
+        "ContentRedaction": NotRequired[ContentRedactionOutputTypeDef],
         "IdentifyLanguage": NotRequired[bool],
         "IdentifyMultipleLanguages": NotRequired[bool],
         "LanguageOptions": NotRequired[List[LanguageCodeType]],
         "IdentifiedLanguageScore": NotRequired[float],
         "LanguageCodes": NotRequired[List[LanguageCodeItemTypeDef]],
         "Tags": NotRequired[List[TagTypeDef]],
         "Subtitles": NotRequired[SubtitlesOutputTypeDef],
         "LanguageIdSettings": NotRequired[Dict[LanguageCodeType, LanguageIdSettingsTypeDef]],
-        "ToxicityDetection": NotRequired[List[ToxicityDetectionSettingsTypeDef]],
+        "ToxicityDetection": NotRequired[List[ToxicityDetectionSettingsOutputTypeDef]],
+    },
+)
+ToxicityDetectionSettingsUnionTypeDef = Union[
+    ToxicityDetectionSettingsTypeDef, ToxicityDetectionSettingsOutputTypeDef
+]
+CallAnalyticsJobSummaryTypeDef = TypedDict(
+    "CallAnalyticsJobSummaryTypeDef",
+    {
+        "CallAnalyticsJobName": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "StartTime": NotRequired[datetime],
+        "CompletionTime": NotRequired[datetime],
+        "LanguageCode": NotRequired[LanguageCodeType],
+        "CallAnalyticsJobStatus": NotRequired[CallAnalyticsJobStatusType],
+        "CallAnalyticsJobDetails": NotRequired[CallAnalyticsJobDetailsTypeDef],
+        "FailureReason": NotRequired[str],
     },
 )
 CallAnalyticsJobTypeDef = TypedDict(
     "CallAnalyticsJobTypeDef",
     {
         "CallAnalyticsJobName": NotRequired[str],
         "CallAnalyticsJobStatus": NotRequired[CallAnalyticsJobStatusType],
+        "CallAnalyticsJobDetails": NotRequired[CallAnalyticsJobDetailsTypeDef],
         "LanguageCode": NotRequired[LanguageCodeType],
         "MediaSampleRateHertz": NotRequired[int],
         "MediaFormat": NotRequired[MediaFormatType],
         "Media": NotRequired[MediaTypeDef],
         "Transcript": NotRequired[TranscriptTypeDef],
         "StartTime": NotRequired[datetime],
         "CreationTime": NotRequired[datetime],
         "CompletionTime": NotRequired[datetime],
         "FailureReason": NotRequired[str],
         "DataAccessRoleArn": NotRequired[str],
         "IdentifiedLanguageScore": NotRequired[float],
-        "Settings": NotRequired[CallAnalyticsJobSettingsTypeDef],
+        "Settings": NotRequired[CallAnalyticsJobSettingsOutputTypeDef],
         "ChannelDefinitions": NotRequired[List[ChannelDefinitionTypeDef]],
     },
 )
+CallAnalyticsJobSettingsUnionTypeDef = Union[
+    CallAnalyticsJobSettingsTypeDef, CallAnalyticsJobSettingsOutputTypeDef
+]
 StartCallAnalyticsJobRequestRequestTypeDef = TypedDict(
     "StartCallAnalyticsJobRequestRequestTypeDef",
     {
         "CallAnalyticsJobName": str,
         "Media": MediaTypeDef,
         "OutputLocation": NotRequired[str],
         "OutputEncryptionKMSKeyId": NotRequired[str],
@@ -1108,17 +1157,26 @@
         "LanguageModel": LanguageModelTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListLanguageModelsResponseTypeDef = TypedDict(
     "ListLanguageModelsResponseTypeDef",
     {
-        "NextToken": str,
         "Models": List[LanguageModelTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "NonTalkTimeFilter": NotRequired[NonTalkTimeFilterTypeDef],
+        "InterruptionFilter": NotRequired[InterruptionFilterTypeDef],
+        "TranscriptFilter": NotRequired[TranscriptFilterOutputTypeDef],
+        "SentimentFilter": NotRequired[SentimentFilterOutputTypeDef],
     },
 )
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NotRequired[NonTalkTimeFilterTypeDef],
         "InterruptionFilter": NotRequired[InterruptionFilterTypeDef],
@@ -1154,17 +1212,17 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTranscriptionJobsResponseTypeDef = TypedDict(
     "ListTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
-        "NextToken": str,
         "TranscriptionJobSummaries": List[TranscriptionJobSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetTranscriptionJobResponseTypeDef = TypedDict(
     "GetTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1173,14 +1231,48 @@
 StartTranscriptionJobResponseTypeDef = TypedDict(
     "StartTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StartTranscriptionJobRequestRequestTypeDef = TypedDict(
+    "StartTranscriptionJobRequestRequestTypeDef",
+    {
+        "TranscriptionJobName": str,
+        "Media": MediaTypeDef,
+        "LanguageCode": NotRequired[LanguageCodeType],
+        "MediaSampleRateHertz": NotRequired[int],
+        "MediaFormat": NotRequired[MediaFormatType],
+        "OutputBucketName": NotRequired[str],
+        "OutputKey": NotRequired[str],
+        "OutputEncryptionKMSKeyId": NotRequired[str],
+        "KMSEncryptionContext": NotRequired[Mapping[str, str]],
+        "Settings": NotRequired[SettingsTypeDef],
+        "ModelSettings": NotRequired[ModelSettingsTypeDef],
+        "JobExecutionSettings": NotRequired[JobExecutionSettingsTypeDef],
+        "ContentRedaction": NotRequired[ContentRedactionTypeDef],
+        "IdentifyLanguage": NotRequired[bool],
+        "IdentifyMultipleLanguages": NotRequired[bool],
+        "LanguageOptions": NotRequired[Sequence[LanguageCodeType]],
+        "Subtitles": NotRequired[SubtitlesTypeDef],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "LanguageIdSettings": NotRequired[Mapping[LanguageCodeType, LanguageIdSettingsTypeDef]],
+        "ToxicityDetection": NotRequired[Sequence[ToxicityDetectionSettingsUnionTypeDef]],
+    },
+)
+ListCallAnalyticsJobsResponseTypeDef = TypedDict(
+    "ListCallAnalyticsJobsResponseTypeDef",
+    {
+        "Status": CallAnalyticsJobStatusType,
+        "CallAnalyticsJobSummaries": List[CallAnalyticsJobSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
 GetCallAnalyticsJobResponseTypeDef = TypedDict(
     "GetCallAnalyticsJobResponseTypeDef",
     {
         "CallAnalyticsJob": CallAnalyticsJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1191,36 +1283,21 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CategoryPropertiesTypeDef = TypedDict(
     "CategoryPropertiesTypeDef",
     {
         "CategoryName": NotRequired[str],
-        "Rules": NotRequired[List[RuleTypeDef]],
+        "Rules": NotRequired[List[RuleOutputTypeDef]],
         "CreateTime": NotRequired[datetime],
         "LastUpdateTime": NotRequired[datetime],
         "InputType": NotRequired[InputTypeType],
     },
 )
-CreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
-    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
-    {
-        "CategoryName": str,
-        "Rules": Sequence[RuleTypeDef],
-        "InputType": NotRequired[InputTypeType],
-    },
-)
-UpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
-    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
-    {
-        "CategoryName": str,
-        "Rules": Sequence[RuleTypeDef],
-        "InputType": NotRequired[InputTypeType],
-    },
-)
+RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
 CreateCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "CreateCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1230,19 +1307,35 @@
         "CategoryProperties": CategoryPropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListCallAnalyticsCategoriesResponseTypeDef = TypedDict(
     "ListCallAnalyticsCategoriesResponseTypeDef",
     {
-        "NextToken": str,
         "Categories": List[CategoryPropertiesTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "UpdateCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
+    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
+    {
+        "CategoryName": str,
+        "Rules": Sequence[RuleUnionTypeDef],
+        "InputType": NotRequired[InputTypeType],
+    },
+)
+UpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
+    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
+    {
+        "CategoryName": str,
+        "Rules": Sequence[RuleUnionTypeDef],
+        "InputType": NotRequired[InputTypeType],
+    },
+)
```

### Comparing `mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe/type_defs.pyi` & `mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 
     data: AbsoluteTimeRangeTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     BaseModelNameType,
     CallAnalyticsJobStatusType,
+    CallAnalyticsSkippedReasonCodeType,
     CLMLanguageCodeType,
     InputTypeType,
     LanguageCodeType,
     MediaFormatType,
     MedicalScribeJobStatusType,
     MedicalScribeParticipantRoleType,
     ModelStatusType,
@@ -49,18 +50,19 @@
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AbsoluteTimeRangeTypeDef",
-    "ContentRedactionTypeDef",
+    "CallAnalyticsSkippedFeatureTypeDef",
+    "ContentRedactionOutputTypeDef",
     "LanguageIdSettingsTypeDef",
     "SummarizationTypeDef",
-    "CallAnalyticsJobSummaryTypeDef",
+    "ContentRedactionTypeDef",
     "ChannelDefinitionTypeDef",
     "MediaTypeDef",
     "TranscriptTypeDef",
     "ResponseMetadataTypeDef",
     "InputDataConfigTypeDef",
     "TagTypeDef",
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
@@ -102,90 +104,109 @@
     "MedicalScribeOutputTypeDef",
     "MedicalScribeSettingsTypeDef",
     "MedicalTranscriptTypeDef",
     "MedicalTranscriptionSettingTypeDef",
     "ModelSettingsTypeDef",
     "SettingsTypeDef",
     "SubtitlesTypeDef",
-    "ToxicityDetectionSettingsTypeDef",
     "SubtitlesOutputTypeDef",
+    "ToxicityDetectionSettingsOutputTypeDef",
+    "ToxicityDetectionSettingsTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMedicalVocabularyRequestRequestTypeDef",
     "UpdateVocabularyFilterRequestRequestTypeDef",
     "UpdateVocabularyRequestRequestTypeDef",
+    "CallAnalyticsJobDetailsTypeDef",
+    "CallAnalyticsJobSettingsOutputTypeDef",
     "CallAnalyticsJobSettingsTypeDef",
+    "ContentRedactionUnionTypeDef",
     "CreateMedicalVocabularyResponseTypeDef",
     "CreateVocabularyFilterResponseTypeDef",
     "CreateVocabularyResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetMedicalVocabularyResponseTypeDef",
     "GetVocabularyFilterResponseTypeDef",
     "GetVocabularyResponseTypeDef",
-    "ListCallAnalyticsJobsResponseTypeDef",
     "UpdateMedicalVocabularyResponseTypeDef",
     "UpdateVocabularyFilterResponseTypeDef",
     "UpdateVocabularyResponseTypeDef",
     "CreateLanguageModelResponseTypeDef",
     "LanguageModelTypeDef",
     "CreateLanguageModelRequestRequestTypeDef",
     "CreateMedicalVocabularyRequestRequestTypeDef",
     "CreateVocabularyFilterRequestRequestTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "InterruptionFilterTypeDef",
     "NonTalkTimeFilterTypeDef",
+    "SentimentFilterOutputTypeDef",
     "SentimentFilterTypeDef",
+    "TranscriptFilterOutputTypeDef",
     "TranscriptFilterTypeDef",
     "ListMedicalScribeJobsResponseTypeDef",
     "ListMedicalTranscriptionJobsResponseTypeDef",
     "ListMedicalVocabulariesResponseTypeDef",
     "ListVocabulariesResponseTypeDef",
     "ListVocabularyFiltersResponseTypeDef",
     "MedicalScribeJobTypeDef",
     "StartMedicalScribeJobRequestRequestTypeDef",
     "MedicalTranscriptionJobTypeDef",
     "StartMedicalTranscriptionJobRequestRequestTypeDef",
-    "StartTranscriptionJobRequestRequestTypeDef",
     "TranscriptionJobSummaryTypeDef",
     "TranscriptionJobTypeDef",
+    "ToxicityDetectionSettingsUnionTypeDef",
+    "CallAnalyticsJobSummaryTypeDef",
     "CallAnalyticsJobTypeDef",
+    "CallAnalyticsJobSettingsUnionTypeDef",
     "StartCallAnalyticsJobRequestRequestTypeDef",
     "DescribeLanguageModelResponseTypeDef",
     "ListLanguageModelsResponseTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
     "GetMedicalScribeJobResponseTypeDef",
     "StartMedicalScribeJobResponseTypeDef",
     "GetMedicalTranscriptionJobResponseTypeDef",
     "StartMedicalTranscriptionJobResponseTypeDef",
     "ListTranscriptionJobsResponseTypeDef",
     "GetTranscriptionJobResponseTypeDef",
     "StartTranscriptionJobResponseTypeDef",
+    "StartTranscriptionJobRequestRequestTypeDef",
+    "ListCallAnalyticsJobsResponseTypeDef",
     "GetCallAnalyticsJobResponseTypeDef",
     "StartCallAnalyticsJobResponseTypeDef",
     "CategoryPropertiesTypeDef",
-    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
-    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
+    "RuleUnionTypeDef",
     "CreateCallAnalyticsCategoryResponseTypeDef",
     "GetCallAnalyticsCategoryResponseTypeDef",
     "ListCallAnalyticsCategoriesResponseTypeDef",
     "UpdateCallAnalyticsCategoryResponseTypeDef",
+    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
+    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
 )
 
 AbsoluteTimeRangeTypeDef = TypedDict(
     "AbsoluteTimeRangeTypeDef",
     {
         "StartTime": NotRequired[int],
         "EndTime": NotRequired[int],
         "First": NotRequired[int],
         "Last": NotRequired[int],
     },
 )
-ContentRedactionTypeDef = TypedDict(
-    "ContentRedactionTypeDef",
+CallAnalyticsSkippedFeatureTypeDef = TypedDict(
+    "CallAnalyticsSkippedFeatureTypeDef",
+    {
+        "Feature": NotRequired[Literal["GENERATIVE_SUMMARIZATION"]],
+        "ReasonCode": NotRequired[CallAnalyticsSkippedReasonCodeType],
+        "Message": NotRequired[str],
+    },
+)
+ContentRedactionOutputTypeDef = TypedDict(
+    "ContentRedactionOutputTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
         "PiiEntityTypes": NotRequired[List[PiiEntityTypeType]],
     },
 )
 LanguageIdSettingsTypeDef = TypedDict(
@@ -198,24 +219,20 @@
 )
 SummarizationTypeDef = TypedDict(
     "SummarizationTypeDef",
     {
         "GenerateAbstractiveSummary": bool,
     },
 )
-CallAnalyticsJobSummaryTypeDef = TypedDict(
-    "CallAnalyticsJobSummaryTypeDef",
+ContentRedactionTypeDef = TypedDict(
+    "ContentRedactionTypeDef",
     {
-        "CallAnalyticsJobName": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "StartTime": NotRequired[datetime],
-        "CompletionTime": NotRequired[datetime],
-        "LanguageCode": NotRequired[LanguageCodeType],
-        "CallAnalyticsJobStatus": NotRequired[CallAnalyticsJobStatusType],
-        "FailureReason": NotRequired[str],
+        "RedactionType": Literal["PII"],
+        "RedactionOutput": RedactionOutputType,
+        "PiiEntityTypes": NotRequired[Sequence[PiiEntityTypeType]],
     },
 )
 ChannelDefinitionTypeDef = TypedDict(
     "ChannelDefinitionTypeDef",
     {
         "ChannelId": NotRequired[int],
         "ParticipantRole": NotRequired[ParticipantRoleType],
@@ -235,18 +252,18 @@
         "RedactedTranscriptFileUri": NotRequired[str],
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
 InputDataConfigTypeDef = TypedDict(
     "InputDataConfigTypeDef",
     {
         "S3Uri": str,
         "DataAccessRoleArn": str,
@@ -584,28 +601,34 @@
 SubtitlesTypeDef = TypedDict(
     "SubtitlesTypeDef",
     {
         "Formats": NotRequired[Sequence[SubtitleFormatType]],
         "OutputStartIndex": NotRequired[int],
     },
 )
-ToxicityDetectionSettingsTypeDef = TypedDict(
-    "ToxicityDetectionSettingsTypeDef",
-    {
-        "ToxicityCategories": List[Literal["ALL"]],
-    },
-)
 SubtitlesOutputTypeDef = TypedDict(
     "SubtitlesOutputTypeDef",
     {
         "Formats": NotRequired[List[SubtitleFormatType]],
         "SubtitleFileUris": NotRequired[List[str]],
         "OutputStartIndex": NotRequired[int],
     },
 )
+ToxicityDetectionSettingsOutputTypeDef = TypedDict(
+    "ToxicityDetectionSettingsOutputTypeDef",
+    {
+        "ToxicityCategories": List[Literal["ALL"]],
+    },
+)
+ToxicityDetectionSettingsTypeDef = TypedDict(
+    "ToxicityDetectionSettingsTypeDef",
+    {
+        "ToxicityCategories": Sequence[Literal["ALL"]],
+    },
+)
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -632,27 +655,47 @@
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "Phrases": NotRequired[Sequence[str]],
         "VocabularyFileUri": NotRequired[str],
         "DataAccessRoleArn": NotRequired[str],
     },
 )
+CallAnalyticsJobDetailsTypeDef = TypedDict(
+    "CallAnalyticsJobDetailsTypeDef",
+    {
+        "Skipped": NotRequired[List[CallAnalyticsSkippedFeatureTypeDef]],
+    },
+)
+CallAnalyticsJobSettingsOutputTypeDef = TypedDict(
+    "CallAnalyticsJobSettingsOutputTypeDef",
+    {
+        "VocabularyName": NotRequired[str],
+        "VocabularyFilterName": NotRequired[str],
+        "VocabularyFilterMethod": NotRequired[VocabularyFilterMethodType],
+        "LanguageModelName": NotRequired[str],
+        "ContentRedaction": NotRequired[ContentRedactionOutputTypeDef],
+        "LanguageOptions": NotRequired[List[LanguageCodeType]],
+        "LanguageIdSettings": NotRequired[Dict[LanguageCodeType, LanguageIdSettingsTypeDef]],
+        "Summarization": NotRequired[SummarizationTypeDef],
+    },
+)
 CallAnalyticsJobSettingsTypeDef = TypedDict(
     "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": NotRequired[str],
         "VocabularyFilterName": NotRequired[str],
         "VocabularyFilterMethod": NotRequired[VocabularyFilterMethodType],
         "LanguageModelName": NotRequired[str],
         "ContentRedaction": NotRequired[ContentRedactionTypeDef],
-        "LanguageOptions": NotRequired[List[LanguageCodeType]],
-        "LanguageIdSettings": NotRequired[Dict[LanguageCodeType, LanguageIdSettingsTypeDef]],
+        "LanguageOptions": NotRequired[Sequence[LanguageCodeType]],
+        "LanguageIdSettings": NotRequired[Mapping[LanguageCodeType, LanguageIdSettingsTypeDef]],
         "Summarization": NotRequired[SummarizationTypeDef],
     },
 )
+ContentRedactionUnionTypeDef = Union[ContentRedactionTypeDef, ContentRedactionOutputTypeDef]
 CreateMedicalVocabularyResponseTypeDef = TypedDict(
     "CreateMedicalVocabularyResponseTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "VocabularyState": VocabularyStateType,
         "LastModifiedTime": datetime,
@@ -716,23 +759,14 @@
         "VocabularyState": VocabularyStateType,
         "LastModifiedTime": datetime,
         "FailureReason": str,
         "DownloadUri": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListCallAnalyticsJobsResponseTypeDef = TypedDict(
-    "ListCallAnalyticsJobsResponseTypeDef",
-    {
-        "Status": CallAnalyticsJobStatusType,
-        "NextToken": str,
-        "CallAnalyticsJobSummaries": List[CallAnalyticsJobSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 UpdateMedicalVocabularyResponseTypeDef = TypedDict(
     "UpdateMedicalVocabularyResponseTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
         "VocabularyState": VocabularyStateType,
@@ -854,24 +888,45 @@
     {
         "Threshold": NotRequired[int],
         "AbsoluteTimeRange": NotRequired[AbsoluteTimeRangeTypeDef],
         "RelativeTimeRange": NotRequired[RelativeTimeRangeTypeDef],
         "Negate": NotRequired[bool],
     },
 )
+SentimentFilterOutputTypeDef = TypedDict(
+    "SentimentFilterOutputTypeDef",
+    {
+        "Sentiments": List[SentimentValueType],
+        "AbsoluteTimeRange": NotRequired[AbsoluteTimeRangeTypeDef],
+        "RelativeTimeRange": NotRequired[RelativeTimeRangeTypeDef],
+        "ParticipantRole": NotRequired[ParticipantRoleType],
+        "Negate": NotRequired[bool],
+    },
+)
 SentimentFilterTypeDef = TypedDict(
     "SentimentFilterTypeDef",
     {
         "Sentiments": Sequence[SentimentValueType],
         "AbsoluteTimeRange": NotRequired[AbsoluteTimeRangeTypeDef],
         "RelativeTimeRange": NotRequired[RelativeTimeRangeTypeDef],
         "ParticipantRole": NotRequired[ParticipantRoleType],
         "Negate": NotRequired[bool],
     },
 )
+TranscriptFilterOutputTypeDef = TypedDict(
+    "TranscriptFilterOutputTypeDef",
+    {
+        "TranscriptFilterType": Literal["EXACT"],
+        "Targets": List[str],
+        "AbsoluteTimeRange": NotRequired[AbsoluteTimeRangeTypeDef],
+        "RelativeTimeRange": NotRequired[RelativeTimeRangeTypeDef],
+        "ParticipantRole": NotRequired[ParticipantRoleType],
+        "Negate": NotRequired[bool],
+    },
+)
 TranscriptFilterTypeDef = TypedDict(
     "TranscriptFilterTypeDef",
     {
         "TranscriptFilterType": Literal["EXACT"],
         "Targets": Sequence[str],
         "AbsoluteTimeRange": NotRequired[AbsoluteTimeRangeTypeDef],
         "RelativeTimeRange": NotRequired[RelativeTimeRangeTypeDef],
@@ -879,52 +934,52 @@
         "Negate": NotRequired[bool],
     },
 )
 ListMedicalScribeJobsResponseTypeDef = TypedDict(
     "ListMedicalScribeJobsResponseTypeDef",
     {
         "Status": MedicalScribeJobStatusType,
-        "NextToken": str,
         "MedicalScribeJobSummaries": List[MedicalScribeJobSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListMedicalTranscriptionJobsResponseTypeDef = TypedDict(
     "ListMedicalTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
-        "NextToken": str,
         "MedicalTranscriptionJobSummaries": List[MedicalTranscriptionJobSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListMedicalVocabulariesResponseTypeDef = TypedDict(
     "ListMedicalVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
-        "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListVocabulariesResponseTypeDef = TypedDict(
     "ListVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
-        "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListVocabularyFiltersResponseTypeDef = TypedDict(
     "ListVocabularyFiltersResponseTypeDef",
     {
-        "NextToken": str,
         "VocabularyFilters": List[VocabularyFilterInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 MedicalScribeJobTypeDef = TypedDict(
     "MedicalScribeJobTypeDef",
     {
         "MedicalScribeJobName": NotRequired[str],
         "MedicalScribeJobStatus": NotRequired[MedicalScribeJobStatusType],
@@ -991,57 +1046,32 @@
         "OutputEncryptionKMSKeyId": NotRequired[str],
         "KMSEncryptionContext": NotRequired[Mapping[str, str]],
         "Settings": NotRequired[MedicalTranscriptionSettingTypeDef],
         "ContentIdentificationType": NotRequired[Literal["PHI"]],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
-StartTranscriptionJobRequestRequestTypeDef = TypedDict(
-    "StartTranscriptionJobRequestRequestTypeDef",
-    {
-        "TranscriptionJobName": str,
-        "Media": MediaTypeDef,
-        "LanguageCode": NotRequired[LanguageCodeType],
-        "MediaSampleRateHertz": NotRequired[int],
-        "MediaFormat": NotRequired[MediaFormatType],
-        "OutputBucketName": NotRequired[str],
-        "OutputKey": NotRequired[str],
-        "OutputEncryptionKMSKeyId": NotRequired[str],
-        "KMSEncryptionContext": NotRequired[Mapping[str, str]],
-        "Settings": NotRequired[SettingsTypeDef],
-        "ModelSettings": NotRequired[ModelSettingsTypeDef],
-        "JobExecutionSettings": NotRequired[JobExecutionSettingsTypeDef],
-        "ContentRedaction": NotRequired[ContentRedactionTypeDef],
-        "IdentifyLanguage": NotRequired[bool],
-        "IdentifyMultipleLanguages": NotRequired[bool],
-        "LanguageOptions": NotRequired[Sequence[LanguageCodeType]],
-        "Subtitles": NotRequired[SubtitlesTypeDef],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "LanguageIdSettings": NotRequired[Mapping[LanguageCodeType, LanguageIdSettingsTypeDef]],
-        "ToxicityDetection": NotRequired[Sequence[ToxicityDetectionSettingsTypeDef]],
-    },
-)
 TranscriptionJobSummaryTypeDef = TypedDict(
     "TranscriptionJobSummaryTypeDef",
     {
         "TranscriptionJobName": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "StartTime": NotRequired[datetime],
         "CompletionTime": NotRequired[datetime],
         "LanguageCode": NotRequired[LanguageCodeType],
         "TranscriptionJobStatus": NotRequired[TranscriptionJobStatusType],
         "FailureReason": NotRequired[str],
         "OutputLocationType": NotRequired[OutputLocationTypeType],
-        "ContentRedaction": NotRequired[ContentRedactionTypeDef],
+        "ContentRedaction": NotRequired[ContentRedactionOutputTypeDef],
         "ModelSettings": NotRequired[ModelSettingsTypeDef],
         "IdentifyLanguage": NotRequired[bool],
         "IdentifyMultipleLanguages": NotRequired[bool],
         "IdentifiedLanguageScore": NotRequired[float],
         "LanguageCodes": NotRequired[List[LanguageCodeItemTypeDef]],
-        "ToxicityDetection": NotRequired[List[ToxicityDetectionSettingsTypeDef]],
+        "ToxicityDetection": NotRequired[List[ToxicityDetectionSettingsOutputTypeDef]],
     },
 )
 TranscriptionJobTypeDef = TypedDict(
     "TranscriptionJobTypeDef",
     {
         "TranscriptionJobName": NotRequired[str],
         "TranscriptionJobStatus": NotRequired[TranscriptionJobStatusType],
@@ -1053,46 +1083,66 @@
         "StartTime": NotRequired[datetime],
         "CreationTime": NotRequired[datetime],
         "CompletionTime": NotRequired[datetime],
         "FailureReason": NotRequired[str],
         "Settings": NotRequired[SettingsTypeDef],
         "ModelSettings": NotRequired[ModelSettingsTypeDef],
         "JobExecutionSettings": NotRequired[JobExecutionSettingsTypeDef],
-        "ContentRedaction": NotRequired[ContentRedactionTypeDef],
+        "ContentRedaction": NotRequired[ContentRedactionOutputTypeDef],
         "IdentifyLanguage": NotRequired[bool],
         "IdentifyMultipleLanguages": NotRequired[bool],
         "LanguageOptions": NotRequired[List[LanguageCodeType]],
         "IdentifiedLanguageScore": NotRequired[float],
         "LanguageCodes": NotRequired[List[LanguageCodeItemTypeDef]],
         "Tags": NotRequired[List[TagTypeDef]],
         "Subtitles": NotRequired[SubtitlesOutputTypeDef],
         "LanguageIdSettings": NotRequired[Dict[LanguageCodeType, LanguageIdSettingsTypeDef]],
-        "ToxicityDetection": NotRequired[List[ToxicityDetectionSettingsTypeDef]],
+        "ToxicityDetection": NotRequired[List[ToxicityDetectionSettingsOutputTypeDef]],
+    },
+)
+ToxicityDetectionSettingsUnionTypeDef = Union[
+    ToxicityDetectionSettingsTypeDef, ToxicityDetectionSettingsOutputTypeDef
+]
+CallAnalyticsJobSummaryTypeDef = TypedDict(
+    "CallAnalyticsJobSummaryTypeDef",
+    {
+        "CallAnalyticsJobName": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "StartTime": NotRequired[datetime],
+        "CompletionTime": NotRequired[datetime],
+        "LanguageCode": NotRequired[LanguageCodeType],
+        "CallAnalyticsJobStatus": NotRequired[CallAnalyticsJobStatusType],
+        "CallAnalyticsJobDetails": NotRequired[CallAnalyticsJobDetailsTypeDef],
+        "FailureReason": NotRequired[str],
     },
 )
 CallAnalyticsJobTypeDef = TypedDict(
     "CallAnalyticsJobTypeDef",
     {
         "CallAnalyticsJobName": NotRequired[str],
         "CallAnalyticsJobStatus": NotRequired[CallAnalyticsJobStatusType],
+        "CallAnalyticsJobDetails": NotRequired[CallAnalyticsJobDetailsTypeDef],
         "LanguageCode": NotRequired[LanguageCodeType],
         "MediaSampleRateHertz": NotRequired[int],
         "MediaFormat": NotRequired[MediaFormatType],
         "Media": NotRequired[MediaTypeDef],
         "Transcript": NotRequired[TranscriptTypeDef],
         "StartTime": NotRequired[datetime],
         "CreationTime": NotRequired[datetime],
         "CompletionTime": NotRequired[datetime],
         "FailureReason": NotRequired[str],
         "DataAccessRoleArn": NotRequired[str],
         "IdentifiedLanguageScore": NotRequired[float],
-        "Settings": NotRequired[CallAnalyticsJobSettingsTypeDef],
+        "Settings": NotRequired[CallAnalyticsJobSettingsOutputTypeDef],
         "ChannelDefinitions": NotRequired[List[ChannelDefinitionTypeDef]],
     },
 )
+CallAnalyticsJobSettingsUnionTypeDef = Union[
+    CallAnalyticsJobSettingsTypeDef, CallAnalyticsJobSettingsOutputTypeDef
+]
 StartCallAnalyticsJobRequestRequestTypeDef = TypedDict(
     "StartCallAnalyticsJobRequestRequestTypeDef",
     {
         "CallAnalyticsJobName": str,
         "Media": MediaTypeDef,
         "OutputLocation": NotRequired[str],
         "OutputEncryptionKMSKeyId": NotRequired[str],
@@ -1107,17 +1157,26 @@
         "LanguageModel": LanguageModelTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListLanguageModelsResponseTypeDef = TypedDict(
     "ListLanguageModelsResponseTypeDef",
     {
-        "NextToken": str,
         "Models": List[LanguageModelTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "NonTalkTimeFilter": NotRequired[NonTalkTimeFilterTypeDef],
+        "InterruptionFilter": NotRequired[InterruptionFilterTypeDef],
+        "TranscriptFilter": NotRequired[TranscriptFilterOutputTypeDef],
+        "SentimentFilter": NotRequired[SentimentFilterOutputTypeDef],
     },
 )
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NotRequired[NonTalkTimeFilterTypeDef],
         "InterruptionFilter": NotRequired[InterruptionFilterTypeDef],
@@ -1153,17 +1212,17 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTranscriptionJobsResponseTypeDef = TypedDict(
     "ListTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
-        "NextToken": str,
         "TranscriptionJobSummaries": List[TranscriptionJobSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetTranscriptionJobResponseTypeDef = TypedDict(
     "GetTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1172,14 +1231,48 @@
 StartTranscriptionJobResponseTypeDef = TypedDict(
     "StartTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StartTranscriptionJobRequestRequestTypeDef = TypedDict(
+    "StartTranscriptionJobRequestRequestTypeDef",
+    {
+        "TranscriptionJobName": str,
+        "Media": MediaTypeDef,
+        "LanguageCode": NotRequired[LanguageCodeType],
+        "MediaSampleRateHertz": NotRequired[int],
+        "MediaFormat": NotRequired[MediaFormatType],
+        "OutputBucketName": NotRequired[str],
+        "OutputKey": NotRequired[str],
+        "OutputEncryptionKMSKeyId": NotRequired[str],
+        "KMSEncryptionContext": NotRequired[Mapping[str, str]],
+        "Settings": NotRequired[SettingsTypeDef],
+        "ModelSettings": NotRequired[ModelSettingsTypeDef],
+        "JobExecutionSettings": NotRequired[JobExecutionSettingsTypeDef],
+        "ContentRedaction": NotRequired[ContentRedactionTypeDef],
+        "IdentifyLanguage": NotRequired[bool],
+        "IdentifyMultipleLanguages": NotRequired[bool],
+        "LanguageOptions": NotRequired[Sequence[LanguageCodeType]],
+        "Subtitles": NotRequired[SubtitlesTypeDef],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "LanguageIdSettings": NotRequired[Mapping[LanguageCodeType, LanguageIdSettingsTypeDef]],
+        "ToxicityDetection": NotRequired[Sequence[ToxicityDetectionSettingsUnionTypeDef]],
+    },
+)
+ListCallAnalyticsJobsResponseTypeDef = TypedDict(
+    "ListCallAnalyticsJobsResponseTypeDef",
+    {
+        "Status": CallAnalyticsJobStatusType,
+        "CallAnalyticsJobSummaries": List[CallAnalyticsJobSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
 GetCallAnalyticsJobResponseTypeDef = TypedDict(
     "GetCallAnalyticsJobResponseTypeDef",
     {
         "CallAnalyticsJob": CallAnalyticsJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1190,36 +1283,21 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CategoryPropertiesTypeDef = TypedDict(
     "CategoryPropertiesTypeDef",
     {
         "CategoryName": NotRequired[str],
-        "Rules": NotRequired[List[RuleTypeDef]],
+        "Rules": NotRequired[List[RuleOutputTypeDef]],
         "CreateTime": NotRequired[datetime],
         "LastUpdateTime": NotRequired[datetime],
         "InputType": NotRequired[InputTypeType],
     },
 )
-CreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
-    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
-    {
-        "CategoryName": str,
-        "Rules": Sequence[RuleTypeDef],
-        "InputType": NotRequired[InputTypeType],
-    },
-)
-UpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
-    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
-    {
-        "CategoryName": str,
-        "Rules": Sequence[RuleTypeDef],
-        "InputType": NotRequired[InputTypeType],
-    },
-)
+RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
 CreateCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "CreateCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1229,19 +1307,35 @@
         "CategoryProperties": CategoryPropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListCallAnalyticsCategoriesResponseTypeDef = TypedDict(
     "ListCallAnalyticsCategoriesResponseTypeDef",
     {
-        "NextToken": str,
         "Categories": List[CategoryPropertiesTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "UpdateCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
+    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
+    {
+        "CategoryName": str,
+        "Rules": Sequence[RuleUnionTypeDef],
+        "InputType": NotRequired[InputTypeType],
+    },
+)
+UpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
+    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
+    {
+        "CategoryName": str,
+        "Rules": Sequence[RuleUnionTypeDef],
+        "InputType": NotRequired[InputTypeType],
+    },
+)
```

### Comparing `mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe.egg-info/PKG-INFO` & `mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transcribe
-Version: 1.34.0
-Summary: Type annotations for boto3.TranscribeService 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.94
+Summary: Type annotations for boto3.TranscribeService 1.34.94 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/
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
 
 <a id="mypy-boto3-transcribe"></a>
 
 # mypy-boto3-transcribe
 
 [![PyPI - mypy-boto3-transcribe](https://img.shields.io/pypi/v/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transcribe)](https://pepy.tech/project/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
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
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-transcribe-1.34.0/mypy_boto3_transcribe.egg-info/SOURCES.txt` & `mypy_boto3_transcribe-1.34.94/mypy_boto3_transcribe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.34.0/setup.py` & `mypy_boto3_transcribe-1.34.94/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-transcribe",
-    version="1.34.0",
+    version="1.34.94",
     packages=["mypy_boto3_transcribe"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.TranscribeService 1.34.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.TranscribeService 1.34.94 service generated with mypy-boto3-builder 7.24.0",
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
     keywords="boto3 transcribe type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_transcribe": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

