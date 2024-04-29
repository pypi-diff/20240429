# Comparing `tmp/mypy-boto3-inspector2-1.34.29.tar.gz` & `tmp/mypy_boto3_inspector2-1.34.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-inspector2-1.34.29.tar", last modified: Fri Jan 26 20:32:43 2024, max compression
+gzip compressed data, was "mypy_boto3_inspector2-1.34.94.tar", last modified: Mon Apr 29 19:32:09 2024, max compression
```

## Comparing `mypy-boto3-inspector2-1.34.29.tar` & `mypy_boto3_inspector2-1.34.94.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 20:32:43.841912 mypy-boto3-inspector2-1.34.29/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-26 20:32:10.000000 mypy-boto3-inspector2-1.34.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15087 2024-01-26 20:32:43.841912 mypy-boto3-inspector2-1.34.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-01-26 20:32:10.000000 mypy-boto3-inspector2-1.34.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 20:32:43.841912 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-01-26 20:32:10.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-01-26 20:32:10.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-01-26 20:32:10.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48439 2024-01-26 20:32:11.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    48436 2024-01-26 20:32:10.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22063 2024-01-26 20:32:11.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    22063 2024-01-26 20:32:11.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20424 2024-01-26 20:32:11.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    20408 2024-01-26 20:32:11.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 20:32:10.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    94452 2024-01-26 20:32:13.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    94452 2024-01-26 20:32:12.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-26 20:32:10.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 20:32:43.841912 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15087 2024-01-26 20:32:43.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-26 20:32:43.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 20:32:43.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 20:32:43.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-26 20:32:43.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-26 20:32:43.000000 mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 20:32:43.841912 mypy-boto3-inspector2-1.34.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-01-26 20:32:10.000000 mypy-boto3-inspector2-1.34.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:09.006773 mypy_boto3_inspector2-1.34.94/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15087 2024-04-29 19:32:09.006773 mypy_boto3_inspector2-1.34.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:09.006773 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48612 2024-04-29 19:31:50.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48609 2024-04-29 19:31:50.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22435 2024-04-29 19:31:51.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22435 2024-04-29 19:31:51.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20380 2024-04-29 19:31:51.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20364 2024-04-29 19:31:50.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    98703 2024-04-29 19:31:52.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98703 2024-04-29 19:31:52.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:32:09.006773 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15087 2024-04-29 19:32:08.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-29 19:32:08.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:08.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:32:08.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 19:32:08.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 19:32:08.000000 mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:32:09.006773 mypy_boto3_inspector2-1.34.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-29 19:31:49.000000 mypy_boto3_inspector2-1.34.94/setup.py
```

### Comparing `mypy-boto3-inspector2-1.34.29/LICENSE` & `mypy_boto3_inspector2-1.34.94/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.34.29/PKG-INFO` & `mypy_boto3_inspector2-1.34.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.34.29
-Summary: Type annotations for boto3.Inspector2 1.34.29 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.94
+Summary: Type annotations for boto3.Inspector2 1.34.94 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector2)](https://pepy.tech/project/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.34.29](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
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
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-inspector2-1.34.29/README.md` & `mypy_boto3_inspector2-1.34.94/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector2)](https://pepy.tech/project/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.34.29](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
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
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/__init__.py` & `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/__init__.pyi` & `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/__main__.py` & `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Inspector2 1.34.29\n"
-        "Version:         1.34.29\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.Inspector2 1.34.94\n"
+        "Version:         1.34.94\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.29")
+    print("1.34.94")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/client.py` & `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,18 +80,19 @@
     DeleteCisScanConfigurationResponseTypeDef,
     DeleteFilterResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     DestinationTypeDef,
     DisableDelegatedAdminAccountResponseTypeDef,
     DisableResponseTypeDef,
     DisassociateMemberResponseTypeDef,
+    Ec2ConfigurationTypeDef,
     EcrConfigurationTypeDef,
     EnableDelegatedAdminAccountResponseTypeDef,
     EnableResponseTypeDef,
-    FilterCriteriaTypeDef,
+    FilterCriteriaUnionTypeDef,
     GetCisScanReportResponseTypeDef,
     GetCisScanResultDetailsResponseTypeDef,
     GetConfigurationResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusResponseTypeDef,
@@ -110,16 +111,16 @@
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
-    ResourceFilterCriteriaTypeDef,
-    ScheduleTypeDef,
+    ResourceFilterCriteriaUnionTypeDef,
+    ScheduleUnionTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     SortCriteriaTypeDef,
     StartCisSessionMessageTypeDef,
     StopCisSessionMessageTypeDef,
     StringFilterTypeDef,
     UpdateCisScanConfigurationResponseTypeDef,
@@ -283,15 +284,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#close)
         """
 
     def create_cis_scan_configuration(
         self,
         *,
         scanName: str,
-        schedule: ScheduleTypeDef,
+        schedule: ScheduleUnionTypeDef,
         securityLevel: CisSecurityLevelType,
         targets: CreateCisTargetsTypeDef,
         tags: Mapping[str, str] = ...,
     ) -> CreateCisScanConfigurationResponseTypeDef:
         """
         Creates a CIS scan configuration.
 
@@ -299,15 +300,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_cis_scan_configuration)
         """
 
     def create_filter(
         self,
         *,
         action: FilterActionType,
-        filterCriteria: FilterCriteriaTypeDef,
+        filterCriteria: FilterCriteriaUnionTypeDef,
         name: str,
         description: str = ...,
         reason: str = ...,
         tags: Mapping[str, str] = ...,
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
@@ -317,29 +318,29 @@
         """
 
     def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_findings_report)
         """
 
     def create_sbom_export(
         self,
         *,
         reportFormat: SbomReportFormatType,
         s3Destination: DestinationTypeDef,
-        resourceFilterCriteria: ResourceFilterCriteriaTypeDef = ...,
+        resourceFilterCriteria: ResourceFilterCriteriaUnionTypeDef = ...,
     ) -> CreateSbomExportResponseTypeDef:
         """
         Creates a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_sbom_export)
         """
@@ -684,15 +685,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_finding_aggregations)
         """
 
     def list_findings(
         self,
         *,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
@@ -805,26 +806,31 @@
         """
 
     def update_cis_scan_configuration(
         self,
         *,
         scanConfigurationArn: str,
         scanName: str = ...,
-        schedule: ScheduleTypeDef = ...,
+        schedule: ScheduleUnionTypeDef = ...,
         securityLevel: CisSecurityLevelType = ...,
         targets: UpdateCisTargetsTypeDef = ...,
     ) -> UpdateCisScanConfigurationResponseTypeDef:
         """
         Updates a CIS scan configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_cis_scan_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_cis_scan_configuration)
         """
 
-    def update_configuration(self, *, ecrConfiguration: EcrConfigurationTypeDef) -> Dict[str, Any]:
+    def update_configuration(
+        self,
+        *,
+        ec2Configuration: Ec2ConfigurationTypeDef = ...,
+        ecrConfiguration: EcrConfigurationTypeDef = ...,
+    ) -> Dict[str, Any]:
         """
         Updates setting configurations for your Amazon Inspector account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_configuration)
         """
 
@@ -852,15 +858,15 @@
 
     def update_filter(
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         name: str = ...,
         reason: str = ...,
     ) -> UpdateFilterResponseTypeDef:
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
```

### Comparing `mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/client.pyi` & `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -80,18 +80,19 @@
     DeleteCisScanConfigurationResponseTypeDef,
     DeleteFilterResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     DestinationTypeDef,
     DisableDelegatedAdminAccountResponseTypeDef,
     DisableResponseTypeDef,
     DisassociateMemberResponseTypeDef,
+    Ec2ConfigurationTypeDef,
     EcrConfigurationTypeDef,
     EnableDelegatedAdminAccountResponseTypeDef,
     EnableResponseTypeDef,
-    FilterCriteriaTypeDef,
+    FilterCriteriaUnionTypeDef,
     GetCisScanReportResponseTypeDef,
     GetCisScanResultDetailsResponseTypeDef,
     GetConfigurationResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusResponseTypeDef,
@@ -110,16 +111,16 @@
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
-    ResourceFilterCriteriaTypeDef,
-    ScheduleTypeDef,
+    ResourceFilterCriteriaUnionTypeDef,
+    ScheduleUnionTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     SortCriteriaTypeDef,
     StartCisSessionMessageTypeDef,
     StopCisSessionMessageTypeDef,
     StringFilterTypeDef,
     UpdateCisScanConfigurationResponseTypeDef,
@@ -280,15 +281,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#close)
         """
 
     def create_cis_scan_configuration(
         self,
         *,
         scanName: str,
-        schedule: ScheduleTypeDef,
+        schedule: ScheduleUnionTypeDef,
         securityLevel: CisSecurityLevelType,
         targets: CreateCisTargetsTypeDef,
         tags: Mapping[str, str] = ...,
     ) -> CreateCisScanConfigurationResponseTypeDef:
         """
         Creates a CIS scan configuration.
 
@@ -296,15 +297,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_cis_scan_configuration)
         """
 
     def create_filter(
         self,
         *,
         action: FilterActionType,
-        filterCriteria: FilterCriteriaTypeDef,
+        filterCriteria: FilterCriteriaUnionTypeDef,
         name: str,
         description: str = ...,
         reason: str = ...,
         tags: Mapping[str, str] = ...,
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
@@ -314,29 +315,29 @@
         """
 
     def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_findings_report)
         """
 
     def create_sbom_export(
         self,
         *,
         reportFormat: SbomReportFormatType,
         s3Destination: DestinationTypeDef,
-        resourceFilterCriteria: ResourceFilterCriteriaTypeDef = ...,
+        resourceFilterCriteria: ResourceFilterCriteriaUnionTypeDef = ...,
     ) -> CreateSbomExportResponseTypeDef:
         """
         Creates a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_sbom_export)
         """
@@ -681,15 +682,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_finding_aggregations)
         """
 
     def list_findings(
         self,
         *,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
@@ -802,26 +803,31 @@
         """
 
     def update_cis_scan_configuration(
         self,
         *,
         scanConfigurationArn: str,
         scanName: str = ...,
-        schedule: ScheduleTypeDef = ...,
+        schedule: ScheduleUnionTypeDef = ...,
         securityLevel: CisSecurityLevelType = ...,
         targets: UpdateCisTargetsTypeDef = ...,
     ) -> UpdateCisScanConfigurationResponseTypeDef:
         """
         Updates a CIS scan configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_cis_scan_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_cis_scan_configuration)
         """
 
-    def update_configuration(self, *, ecrConfiguration: EcrConfigurationTypeDef) -> Dict[str, Any]:
+    def update_configuration(
+        self,
+        *,
+        ec2Configuration: Ec2ConfigurationTypeDef = ...,
+        ecrConfiguration: EcrConfigurationTypeDef = ...,
+    ) -> Dict[str, Any]:
         """
         Updates setting configurations for your Amazon Inspector account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_configuration)
         """
 
@@ -849,15 +855,15 @@
 
     def update_filter(
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         name: str = ...,
         reason: str = ...,
     ) -> UpdateFilterResponseTypeDef:
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
```

### Comparing `mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/literals.py` & `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     "CoverageStringComparisonType",
     "CurrencyType",
     "DayType",
     "DelegatedAdminStatusType",
     "Ec2DeepInspectionStatusType",
     "Ec2InstanceSortByType",
     "Ec2PlatformType",
+    "Ec2ScanModeStatusType",
+    "Ec2ScanModeType",
     "EcrPullDateRescanDurationType",
     "EcrRescanDurationStatusType",
     "EcrRescanDurationType",
     "EcrScanFrequencyType",
     "ErrorCodeType",
     "ExploitAvailableType",
     "ExternalReportStatusType",
@@ -104,14 +106,15 @@
     "RepositorySortByType",
     "ResourceMapComparisonType",
     "ResourceScanTypeType",
     "ResourceStringComparisonType",
     "ResourceTypeType",
     "RuntimeType",
     "SbomReportFormatType",
+    "ScanModeType",
     "ScanStatusCodeType",
     "ScanStatusReasonType",
     "ScanTypeType",
     "SearchVulnerabilitiesPaginatorName",
     "ServiceType",
     "SeverityType",
     "SortFieldType",
@@ -193,14 +196,16 @@
 CoverageStringComparisonType = Literal["EQUALS", "NOT_EQUALS"]
 CurrencyType = Literal["USD"]
 DayType = Literal["FRI", "MON", "SAT", "SUN", "THU", "TUE", "WED"]
 DelegatedAdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
 Ec2DeepInspectionStatusType = Literal["ACTIVATED", "DEACTIVATED", "FAILED", "PENDING"]
 Ec2InstanceSortByType = Literal["ALL", "CRITICAL", "HIGH", "NETWORK_FINDINGS"]
 Ec2PlatformType = Literal["LINUX", "MACOS", "UNKNOWN", "WINDOWS"]
+Ec2ScanModeStatusType = Literal["PENDING", "SUCCESS"]
+Ec2ScanModeType = Literal["EC2_HYBRID", "EC2_SSM_AGENT_BASED"]
 EcrPullDateRescanDurationType = Literal["DAYS_14", "DAYS_180", "DAYS_30", "DAYS_60", "DAYS_90"]
 EcrRescanDurationStatusType = Literal["FAILED", "PENDING", "SUCCESS"]
 EcrRescanDurationType = Literal["DAYS_14", "DAYS_180", "DAYS_30", "DAYS_60", "DAYS_90", "LIFETIME"]
 EcrScanFrequencyType = Literal["CONTINUOUS_SCAN", "MANUAL", "SCAN_ON_PUSH"]
 ErrorCodeType = Literal[
     "ACCESS_DENIED",
     "ACCOUNT_IS_ISOLATED",
@@ -326,14 +331,15 @@
     "PYTHON_3_10",
     "PYTHON_3_7",
     "PYTHON_3_8",
     "PYTHON_3_9",
     "UNSUPPORTED",
 ]
 SbomReportFormatType = Literal["CYCLONEDX_1_4", "SPDX_2_3"]
+ScanModeType = Literal["EC2_AGENTLESS", "EC2_SSM_AGENT_BASED"]
 ScanStatusCodeType = Literal["ACTIVE", "INACTIVE"]
 ScanStatusReasonType = Literal[
     "ACCESS_DENIED",
     "DEEP_INSPECTION_COLLECTION_TIME_LIMIT_EXCEEDED",
     "DEEP_INSPECTION_DAILY_SSM_INVENTORY_LIMIT_EXCEEDED",
     "DEEP_INSPECTION_NO_INVENTORY",
     "DEEP_INSPECTION_PACKAGE_COLLECTION_LIMIT_EXCEEDED",
@@ -417,14 +423,15 @@
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
@@ -435,14 +442,15 @@
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
@@ -460,14 +468,15 @@
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
@@ -480,24 +489,26 @@
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
@@ -558,15 +569,14 @@
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
@@ -695,14 +705,15 @@
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
@@ -746,14 +757,15 @@
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

### Comparing `mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/literals.pyi` & `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     "CoverageStringComparisonType",
     "CurrencyType",
     "DayType",
     "DelegatedAdminStatusType",
     "Ec2DeepInspectionStatusType",
     "Ec2InstanceSortByType",
     "Ec2PlatformType",
+    "Ec2ScanModeStatusType",
+    "Ec2ScanModeType",
     "EcrPullDateRescanDurationType",
     "EcrRescanDurationStatusType",
     "EcrRescanDurationType",
     "EcrScanFrequencyType",
     "ErrorCodeType",
     "ExploitAvailableType",
     "ExternalReportStatusType",
@@ -104,14 +106,15 @@
     "RepositorySortByType",
     "ResourceMapComparisonType",
     "ResourceScanTypeType",
     "ResourceStringComparisonType",
     "ResourceTypeType",
     "RuntimeType",
     "SbomReportFormatType",
+    "ScanModeType",
     "ScanStatusCodeType",
     "ScanStatusReasonType",
     "ScanTypeType",
     "SearchVulnerabilitiesPaginatorName",
     "ServiceType",
     "SeverityType",
     "SortFieldType",
@@ -193,14 +196,16 @@
 CoverageStringComparisonType = Literal["EQUALS", "NOT_EQUALS"]
 CurrencyType = Literal["USD"]
 DayType = Literal["FRI", "MON", "SAT", "SUN", "THU", "TUE", "WED"]
 DelegatedAdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
 Ec2DeepInspectionStatusType = Literal["ACTIVATED", "DEACTIVATED", "FAILED", "PENDING"]
 Ec2InstanceSortByType = Literal["ALL", "CRITICAL", "HIGH", "NETWORK_FINDINGS"]
 Ec2PlatformType = Literal["LINUX", "MACOS", "UNKNOWN", "WINDOWS"]
+Ec2ScanModeStatusType = Literal["PENDING", "SUCCESS"]
+Ec2ScanModeType = Literal["EC2_HYBRID", "EC2_SSM_AGENT_BASED"]
 EcrPullDateRescanDurationType = Literal["DAYS_14", "DAYS_180", "DAYS_30", "DAYS_60", "DAYS_90"]
 EcrRescanDurationStatusType = Literal["FAILED", "PENDING", "SUCCESS"]
 EcrRescanDurationType = Literal["DAYS_14", "DAYS_180", "DAYS_30", "DAYS_60", "DAYS_90", "LIFETIME"]
 EcrScanFrequencyType = Literal["CONTINUOUS_SCAN", "MANUAL", "SCAN_ON_PUSH"]
 ErrorCodeType = Literal[
     "ACCESS_DENIED",
     "ACCOUNT_IS_ISOLATED",
@@ -326,14 +331,15 @@
     "PYTHON_3_10",
     "PYTHON_3_7",
     "PYTHON_3_8",
     "PYTHON_3_9",
     "UNSUPPORTED",
 ]
 SbomReportFormatType = Literal["CYCLONEDX_1_4", "SPDX_2_3"]
+ScanModeType = Literal["EC2_AGENTLESS", "EC2_SSM_AGENT_BASED"]
 ScanStatusCodeType = Literal["ACTIVE", "INACTIVE"]
 ScanStatusReasonType = Literal[
     "ACCESS_DENIED",
     "DEEP_INSPECTION_COLLECTION_TIME_LIMIT_EXCEEDED",
     "DEEP_INSPECTION_DAILY_SSM_INVENTORY_LIMIT_EXCEEDED",
     "DEEP_INSPECTION_NO_INVENTORY",
     "DEEP_INSPECTION_PACKAGE_COLLECTION_LIMIT_EXCEEDED",
@@ -417,14 +423,15 @@
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
@@ -435,14 +442,15 @@
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
@@ -460,14 +468,15 @@
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
@@ -480,24 +489,26 @@
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
@@ -558,15 +569,14 @@
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
@@ -695,14 +705,15 @@
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
@@ -746,14 +757,15 @@
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

### Comparing `mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/paginator.py` & `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,27 +67,27 @@
 )
 from .type_defs import (
     AggregationRequestTypeDef,
     CisScanResultDetailsFilterCriteriaTypeDef,
     CisScanResultsAggregatedByChecksFilterCriteriaTypeDef,
     CisScanResultsAggregatedByTargetResourceFilterCriteriaTypeDef,
     CoverageFilterCriteriaTypeDef,
-    FilterCriteriaPaginatorTypeDef,
+    FilterCriteriaUnionTypeDef,
     GetCisScanResultDetailsResponseTypeDef,
     ListAccountPermissionsResponseTypeDef,
     ListCisScanConfigurationsFilterCriteriaTypeDef,
-    ListCisScanConfigurationsResponsePaginatorTypeDef,
+    ListCisScanConfigurationsResponseTypeDef,
     ListCisScanResultsAggregatedByChecksResponseTypeDef,
     ListCisScanResultsAggregatedByTargetResourceResponseTypeDef,
     ListCisScansFilterCriteriaTypeDef,
     ListCisScansResponseTypeDef,
     ListCoverageResponseTypeDef,
     ListCoverageStatisticsResponseTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
-    ListFiltersResponsePaginatorTypeDef,
+    ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     PaginatorConfigTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
@@ -170,15 +170,15 @@
     def paginate(
         self,
         *,
         filterCriteria: ListCisScanConfigurationsFilterCriteriaTypeDef = ...,
         sortBy: CisScanConfigurationsSortByType = ...,
         sortOrder: CisSortOrderType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListCisScanConfigurationsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListCisScanConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCisScanConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listcisscanconfigurationspaginator)
         """
 
 
 class ListCisScanResultsAggregatedByChecksPaginator(Paginator):
@@ -304,15 +304,15 @@
 
     def paginate(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListFiltersResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfilterspaginator)
         """
 
 
 class ListFindingAggregationsPaginator(Paginator):
@@ -340,15 +340,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        filterCriteria: FilterCriteriaPaginatorTypeDef = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
         """
```

### Comparing `mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/paginator.pyi` & `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -67,27 +67,27 @@
 )
 from .type_defs import (
     AggregationRequestTypeDef,
     CisScanResultDetailsFilterCriteriaTypeDef,
     CisScanResultsAggregatedByChecksFilterCriteriaTypeDef,
     CisScanResultsAggregatedByTargetResourceFilterCriteriaTypeDef,
     CoverageFilterCriteriaTypeDef,
-    FilterCriteriaPaginatorTypeDef,
+    FilterCriteriaUnionTypeDef,
     GetCisScanResultDetailsResponseTypeDef,
     ListAccountPermissionsResponseTypeDef,
     ListCisScanConfigurationsFilterCriteriaTypeDef,
-    ListCisScanConfigurationsResponsePaginatorTypeDef,
+    ListCisScanConfigurationsResponseTypeDef,
     ListCisScanResultsAggregatedByChecksResponseTypeDef,
     ListCisScanResultsAggregatedByTargetResourceResponseTypeDef,
     ListCisScansFilterCriteriaTypeDef,
     ListCisScansResponseTypeDef,
     ListCoverageResponseTypeDef,
     ListCoverageStatisticsResponseTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
-    ListFiltersResponsePaginatorTypeDef,
+    ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     PaginatorConfigTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
@@ -166,15 +166,15 @@
     def paginate(
         self,
         *,
         filterCriteria: ListCisScanConfigurationsFilterCriteriaTypeDef = ...,
         sortBy: CisScanConfigurationsSortByType = ...,
         sortOrder: CisSortOrderType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListCisScanConfigurationsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListCisScanConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCisScanConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listcisscanconfigurationspaginator)
         """
 
 class ListCisScanResultsAggregatedByChecksPaginator(Paginator):
     """
@@ -293,15 +293,15 @@
 
     def paginate(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListFiltersResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfilterspaginator)
         """
 
 class ListFindingAggregationsPaginator(Paginator):
     """
@@ -327,15 +327,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        filterCriteria: FilterCriteriaPaginatorTypeDef = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
         """
```

### Comparing `mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/type_defs.py` & `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     CoverageResourceTypeType,
     CoverageStringComparisonType,
     DayType,
     DelegatedAdminStatusType,
     Ec2DeepInspectionStatusType,
     Ec2InstanceSortByType,
     Ec2PlatformType,
+    Ec2ScanModeStatusType,
+    Ec2ScanModeType,
     EcrPullDateRescanDurationType,
     EcrRescanDurationStatusType,
     EcrRescanDurationType,
     EcrScanFrequencyType,
     ErrorCodeType,
     ExploitAvailableType,
     ExternalReportStatusType,
@@ -80,14 +82,15 @@
     ReportingErrorCodeType,
     RepositorySortByType,
     ResourceScanTypeType,
     ResourceStringComparisonType,
     ResourceTypeType,
     RuntimeType,
     SbomReportFormatType,
+    ScanModeType,
     ScanStatusCodeType,
     ScanStatusReasonType,
     ScanTypeType,
     ServiceType,
     SeverityType,
     SortFieldType,
     SortOrderType,
@@ -164,22 +167,25 @@
     "CreateCisTargetsTypeDef",
     "DestinationTypeDef",
     "Cvss2TypeDef",
     "Cvss3TypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "TimeTypeDef",
-    "DateFilterPaginatorTypeDef",
+    "DateFilterExtraOutputTypeDef",
+    "DateFilterOutputTypeDef",
     "DelegatedAdminAccountTypeDef",
     "DelegatedAdminTypeDef",
     "DeleteCisScanConfigurationRequestRequestTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     "DisableRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
+    "Ec2ScanModeStateTypeDef",
+    "Ec2ConfigurationTypeDef",
     "MapFilterTypeDef",
     "Ec2MetadataTypeDef",
     "EcrRescanDurationStateTypeDef",
     "EcrConfigurationTypeDef",
     "EcrContainerImageMetadataTypeDef",
     "EcrRepositoryMetadataTypeDef",
     "EnableDelegatedAdminAccountRequestRequestTypeDef",
@@ -287,18 +293,20 @@
     "ListCisScanConfigurationsFilterCriteriaTypeDef",
     "CodeVulnerabilityDetailsTypeDef",
     "CodeSnippetResultTypeDef",
     "ListCoverageStatisticsResponseTypeDef",
     "CvssScoreDetailsTypeDef",
     "DailyScheduleTypeDef",
     "MonthlyScheduleTypeDef",
-    "WeeklySchedulePaginatorTypeDef",
+    "WeeklyScheduleExtraOutputTypeDef",
+    "WeeklyScheduleOutputTypeDef",
     "WeeklyScheduleTypeDef",
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
+    "Ec2ConfigurationStateTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "FindingDetailTypeDef",
     "VulnerabilityTypeDef",
     "PackageFilterTypeDef",
@@ -311,14 +319,15 @@
     "GetMemberResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ResourceScanMetadataTypeDef",
     "ListAccountPermissionsResponseTypeDef",
     "NetworkPathTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
+    "ResourceFilterCriteriaOutputTypeDef",
     "ResourceFilterCriteriaTypeDef",
     "SearchVulnerabilitiesRequestRequestTypeDef",
     "SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
     "StartCisSessionRequestRequestTypeDef",
     "StopCisSessionMessageTypeDef",
     "UsageTotalTypeDef",
     "AggregationResponseTypeDef",
@@ -338,57 +347,58 @@
     "ListCisScanResultsAggregatedByChecksRequestRequestTypeDef",
     "ListCisScanResultsAggregatedByTargetResourceRequestListCisScanResultsAggregatedByTargetResourcePaginateTypeDef",
     "ListCisScanResultsAggregatedByTargetResourceRequestRequestTypeDef",
     "ListCisScanConfigurationsRequestListCisScanConfigurationsPaginateTypeDef",
     "ListCisScanConfigurationsRequestRequestTypeDef",
     "BatchGetCodeSnippetResponseTypeDef",
     "InspectorScoreDetailsTypeDef",
-    "SchedulePaginatorTypeDef",
+    "ScheduleExtraOutputTypeDef",
+    "ScheduleOutputTypeDef",
     "ScheduleTypeDef",
     "AggregationRequestTypeDef",
     "GetConfigurationResponseTypeDef",
     "BatchGetFindingDetailsResponseTypeDef",
     "SearchVulnerabilitiesResponseTypeDef",
-    "FilterCriteriaPaginatorTypeDef",
+    "FilterCriteriaExtraOutputTypeDef",
+    "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "BatchGetFreeTrialInfoResponseTypeDef",
     "CoveredResourceTypeDef",
     "NetworkReachabilityDetailsTypeDef",
-    "CreateSbomExportRequestRequestTypeDef",
     "GetSbomExportResponseTypeDef",
+    "CreateSbomExportRequestRequestTypeDef",
+    "ResourceFilterCriteriaUnionTypeDef",
     "StopCisSessionRequestRequestTypeDef",
     "ListUsageTotalsResponseTypeDef",
     "ListFindingAggregationsResponseTypeDef",
     "BatchGetAccountStatusResponseTypeDef",
     "ResourceTypeDef",
     "ListCisScansRequestListCisScansPaginateTypeDef",
     "ListCisScansRequestRequestTypeDef",
     "ListCoverageRequestListCoveragePaginateTypeDef",
     "ListCoverageRequestRequestTypeDef",
     "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
     "ListCoverageStatisticsRequestRequestTypeDef",
-    "CisScanConfigurationPaginatorTypeDef",
     "CisScanConfigurationTypeDef",
     "CreateCisScanConfigurationRequestRequestTypeDef",
+    "ScheduleUnionTypeDef",
     "UpdateCisScanConfigurationRequestRequestTypeDef",
     "ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     "ListFindingAggregationsRequestRequestTypeDef",
-    "FilterPaginatorTypeDef",
-    "ListFindingsRequestListFindingsPaginateTypeDef",
-    "CreateFilterRequestRequestTypeDef",
-    "CreateFindingsReportRequestRequestTypeDef",
     "FilterTypeDef",
     "GetFindingsReportStatusResponseTypeDef",
+    "CreateFilterRequestRequestTypeDef",
+    "CreateFindingsReportRequestRequestTypeDef",
+    "FilterCriteriaUnionTypeDef",
+    "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "ListCoverageResponseTypeDef",
     "FindingTypeDef",
-    "ListCisScanConfigurationsResponsePaginatorTypeDef",
     "ListCisScanConfigurationsResponseTypeDef",
-    "ListFiltersResponsePaginatorTypeDef",
     "ListFiltersResponseTypeDef",
     "ListFindingsResponseTypeDef",
 )
 
 SeverityCountsTypeDef = TypedDict(
     "SeverityCountsTypeDef",
     {
@@ -446,18 +456,18 @@
         "accountId": str,
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
 AtigDataTypeDef = TypedDict(
     "AtigDataTypeDef",
     {
         "firstSeen": NotRequired[datetime],
         "lastSeen": NotRequired[datetime],
@@ -813,16 +823,23 @@
 TimeTypeDef = TypedDict(
     "TimeTypeDef",
     {
         "timeOfDay": str,
         "timezone": str,
     },
 )
-DateFilterPaginatorTypeDef = TypedDict(
-    "DateFilterPaginatorTypeDef",
+DateFilterExtraOutputTypeDef = TypedDict(
+    "DateFilterExtraOutputTypeDef",
+    {
+        "endInclusive": NotRequired[datetime],
+        "startInclusive": NotRequired[datetime],
+    },
+)
+DateFilterOutputTypeDef = TypedDict(
+    "DateFilterOutputTypeDef",
     {
         "endInclusive": NotRequired[datetime],
         "startInclusive": NotRequired[datetime],
     },
 )
 DelegatedAdminAccountTypeDef = TypedDict(
     "DelegatedAdminAccountTypeDef",
@@ -865,14 +882,27 @@
 )
 DisassociateMemberRequestRequestTypeDef = TypedDict(
     "DisassociateMemberRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
+Ec2ScanModeStateTypeDef = TypedDict(
+    "Ec2ScanModeStateTypeDef",
+    {
+        "scanMode": NotRequired[Ec2ScanModeType],
+        "scanModeStatus": NotRequired[Ec2ScanModeStatusType],
+    },
+)
+Ec2ConfigurationTypeDef = TypedDict(
+    "Ec2ConfigurationTypeDef",
+    {
+        "scanMode": Ec2ScanModeType,
+    },
+)
 MapFilterTypeDef = TypedDict(
     "MapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
         "value": NotRequired[str],
     },
@@ -1816,16 +1846,23 @@
 MonthlyScheduleTypeDef = TypedDict(
     "MonthlyScheduleTypeDef",
     {
         "day": DayType,
         "startTime": TimeTypeDef,
     },
 )
-WeeklySchedulePaginatorTypeDef = TypedDict(
-    "WeeklySchedulePaginatorTypeDef",
+WeeklyScheduleExtraOutputTypeDef = TypedDict(
+    "WeeklyScheduleExtraOutputTypeDef",
+    {
+        "days": List[DayType],
+        "startTime": TimeTypeDef,
+    },
+)
+WeeklyScheduleOutputTypeDef = TypedDict(
+    "WeeklyScheduleOutputTypeDef",
     {
         "days": List[DayType],
         "startTime": TimeTypeDef,
     },
 )
 WeeklyScheduleTypeDef = TypedDict(
     "WeeklyScheduleTypeDef",
@@ -1845,14 +1882,20 @@
 GetDelegatedAdminAccountResponseTypeDef = TypedDict(
     "GetDelegatedAdminAccountResponseTypeDef",
     {
         "delegatedAdmin": DelegatedAdminTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+Ec2ConfigurationStateTypeDef = TypedDict(
+    "Ec2ConfigurationStateTypeDef",
+    {
+        "scanModeState": NotRequired[Ec2ScanModeStateTypeDef],
+    },
+)
 Ec2InstanceAggregationTypeDef = TypedDict(
     "Ec2InstanceAggregationTypeDef",
     {
         "amis": NotRequired[Sequence[StringFilterTypeDef]],
         "instanceIds": NotRequired[Sequence[StringFilterTypeDef]],
         "instanceTags": NotRequired[Sequence[MapFilterTypeDef]],
         "operatingSystems": NotRequired[Sequence[StringFilterTypeDef]],
@@ -1876,15 +1919,16 @@
     {
         "rescanDurationState": NotRequired[EcrRescanDurationStateTypeDef],
     },
 )
 UpdateConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationRequestRequestTypeDef",
     {
-        "ecrConfiguration": EcrConfigurationTypeDef,
+        "ec2Configuration": NotRequired[Ec2ConfigurationTypeDef],
+        "ecrConfiguration": NotRequired[EcrConfigurationTypeDef],
     },
 )
 FindingDetailTypeDef = TypedDict(
     "FindingDetailTypeDef",
     {
         "cisaData": NotRequired[CisaDataTypeDef],
         "cwes": NotRequired[List[str]],
@@ -2029,14 +2073,27 @@
 )
 RemediationTypeDef = TypedDict(
     "RemediationTypeDef",
     {
         "recommendation": NotRequired[RecommendationTypeDef],
     },
 )
+ResourceFilterCriteriaOutputTypeDef = TypedDict(
+    "ResourceFilterCriteriaOutputTypeDef",
+    {
+        "accountId": NotRequired[List[ResourceStringFilterTypeDef]],
+        "ec2InstanceTags": NotRequired[List[ResourceMapFilterTypeDef]],
+        "ecrImageTags": NotRequired[List[ResourceStringFilterTypeDef]],
+        "ecrRepositoryName": NotRequired[List[ResourceStringFilterTypeDef]],
+        "lambdaFunctionName": NotRequired[List[ResourceStringFilterTypeDef]],
+        "lambdaFunctionTags": NotRequired[List[ResourceMapFilterTypeDef]],
+        "resourceId": NotRequired[List[ResourceStringFilterTypeDef]],
+        "resourceType": NotRequired[List[ResourceStringFilterTypeDef]],
+    },
+)
 ResourceFilterCriteriaTypeDef = TypedDict(
     "ResourceFilterCriteriaTypeDef",
     {
         "accountId": NotRequired[Sequence[ResourceStringFilterTypeDef]],
         "ec2InstanceTags": NotRequired[Sequence[ResourceMapFilterTypeDef]],
         "ecrImageTags": NotRequired[Sequence[ResourceStringFilterTypeDef]],
         "ecrRepositoryName": NotRequired[Sequence[ResourceStringFilterTypeDef]],
@@ -2182,14 +2239,15 @@
         "imagePulledAt": NotRequired[Sequence[CoverageDateFilterTypeDef]],
         "lambdaFunctionName": NotRequired[Sequence[CoverageStringFilterTypeDef]],
         "lambdaFunctionRuntime": NotRequired[Sequence[CoverageStringFilterTypeDef]],
         "lambdaFunctionTags": NotRequired[Sequence[CoverageMapFilterTypeDef]],
         "lastScannedAt": NotRequired[Sequence[CoverageDateFilterTypeDef]],
         "resourceId": NotRequired[Sequence[CoverageStringFilterTypeDef]],
         "resourceType": NotRequired[Sequence[CoverageStringFilterTypeDef]],
+        "scanMode": NotRequired[Sequence[CoverageStringFilterTypeDef]],
         "scanStatusCode": NotRequired[Sequence[CoverageStringFilterTypeDef]],
         "scanStatusReason": NotRequired[Sequence[CoverageStringFilterTypeDef]],
         "scanType": NotRequired[Sequence[CoverageStringFilterTypeDef]],
     },
 )
 ListCisScansResponseTypeDef = TypedDict(
     "ListCisScansResponseTypeDef",
@@ -2299,21 +2357,30 @@
 )
 InspectorScoreDetailsTypeDef = TypedDict(
     "InspectorScoreDetailsTypeDef",
     {
         "adjustedCvss": NotRequired[CvssScoreDetailsTypeDef],
     },
 )
-SchedulePaginatorTypeDef = TypedDict(
-    "SchedulePaginatorTypeDef",
+ScheduleExtraOutputTypeDef = TypedDict(
+    "ScheduleExtraOutputTypeDef",
     {
         "daily": NotRequired[DailyScheduleTypeDef],
         "monthly": NotRequired[MonthlyScheduleTypeDef],
         "oneTime": NotRequired[Dict[str, Any]],
-        "weekly": NotRequired[WeeklySchedulePaginatorTypeDef],
+        "weekly": NotRequired[WeeklyScheduleExtraOutputTypeDef],
+    },
+)
+ScheduleOutputTypeDef = TypedDict(
+    "ScheduleOutputTypeDef",
+    {
+        "daily": NotRequired[DailyScheduleTypeDef],
+        "monthly": NotRequired[MonthlyScheduleTypeDef],
+        "oneTime": NotRequired[Dict[str, Any]],
+        "weekly": NotRequired[WeeklyScheduleOutputTypeDef],
     },
 )
 ScheduleTypeDef = TypedDict(
     "ScheduleTypeDef",
     {
         "daily": NotRequired[DailyScheduleTypeDef],
         "monthly": NotRequired[MonthlyScheduleTypeDef],
@@ -2336,14 +2403,15 @@
         "repositoryAggregation": NotRequired[RepositoryAggregationTypeDef],
         "titleAggregation": NotRequired[TitleAggregationTypeDef],
     },
 )
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
+        "ec2Configuration": Ec2ConfigurationStateTypeDef,
         "ecrConfiguration": EcrConfigurationStateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 BatchGetFindingDetailsResponseTypeDef = TypedDict(
     "BatchGetFindingDetailsResponseTypeDef",
     {
@@ -2356,55 +2424,102 @@
     "SearchVulnerabilitiesResponseTypeDef",
     {
         "nextToken": str,
         "vulnerabilities": List[VulnerabilityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-FilterCriteriaPaginatorTypeDef = TypedDict(
-    "FilterCriteriaPaginatorTypeDef",
+FilterCriteriaExtraOutputTypeDef = TypedDict(
+    "FilterCriteriaExtraOutputTypeDef",
     {
         "awsAccountId": NotRequired[List[StringFilterTypeDef]],
         "codeVulnerabilityDetectorName": NotRequired[List[StringFilterTypeDef]],
         "codeVulnerabilityDetectorTags": NotRequired[List[StringFilterTypeDef]],
         "codeVulnerabilityFilePath": NotRequired[List[StringFilterTypeDef]],
         "componentId": NotRequired[List[StringFilterTypeDef]],
         "componentType": NotRequired[List[StringFilterTypeDef]],
         "ec2InstanceImageId": NotRequired[List[StringFilterTypeDef]],
         "ec2InstanceSubnetId": NotRequired[List[StringFilterTypeDef]],
         "ec2InstanceVpcId": NotRequired[List[StringFilterTypeDef]],
         "ecrImageArchitecture": NotRequired[List[StringFilterTypeDef]],
         "ecrImageHash": NotRequired[List[StringFilterTypeDef]],
-        "ecrImagePushedAt": NotRequired[List[DateFilterPaginatorTypeDef]],
+        "ecrImagePushedAt": NotRequired[List[DateFilterExtraOutputTypeDef]],
         "ecrImageRegistry": NotRequired[List[StringFilterTypeDef]],
         "ecrImageRepositoryName": NotRequired[List[StringFilterTypeDef]],
         "ecrImageTags": NotRequired[List[StringFilterTypeDef]],
         "epssScore": NotRequired[List[NumberFilterTypeDef]],
         "exploitAvailable": NotRequired[List[StringFilterTypeDef]],
         "findingArn": NotRequired[List[StringFilterTypeDef]],
         "findingStatus": NotRequired[List[StringFilterTypeDef]],
         "findingType": NotRequired[List[StringFilterTypeDef]],
-        "firstObservedAt": NotRequired[List[DateFilterPaginatorTypeDef]],
+        "firstObservedAt": NotRequired[List[DateFilterExtraOutputTypeDef]],
         "fixAvailable": NotRequired[List[StringFilterTypeDef]],
         "inspectorScore": NotRequired[List[NumberFilterTypeDef]],
         "lambdaFunctionExecutionRoleArn": NotRequired[List[StringFilterTypeDef]],
-        "lambdaFunctionLastModifiedAt": NotRequired[List[DateFilterPaginatorTypeDef]],
+        "lambdaFunctionLastModifiedAt": NotRequired[List[DateFilterExtraOutputTypeDef]],
         "lambdaFunctionLayers": NotRequired[List[StringFilterTypeDef]],
         "lambdaFunctionName": NotRequired[List[StringFilterTypeDef]],
         "lambdaFunctionRuntime": NotRequired[List[StringFilterTypeDef]],
-        "lastObservedAt": NotRequired[List[DateFilterPaginatorTypeDef]],
+        "lastObservedAt": NotRequired[List[DateFilterExtraOutputTypeDef]],
         "networkProtocol": NotRequired[List[StringFilterTypeDef]],
         "portRange": NotRequired[List[PortRangeFilterTypeDef]],
         "relatedVulnerabilities": NotRequired[List[StringFilterTypeDef]],
         "resourceId": NotRequired[List[StringFilterTypeDef]],
         "resourceTags": NotRequired[List[MapFilterTypeDef]],
         "resourceType": NotRequired[List[StringFilterTypeDef]],
         "severity": NotRequired[List[StringFilterTypeDef]],
         "title": NotRequired[List[StringFilterTypeDef]],
-        "updatedAt": NotRequired[List[DateFilterPaginatorTypeDef]],
+        "updatedAt": NotRequired[List[DateFilterExtraOutputTypeDef]],
+        "vendorSeverity": NotRequired[List[StringFilterTypeDef]],
+        "vulnerabilityId": NotRequired[List[StringFilterTypeDef]],
+        "vulnerabilitySource": NotRequired[List[StringFilterTypeDef]],
+        "vulnerablePackages": NotRequired[List[PackageFilterTypeDef]],
+    },
+)
+FilterCriteriaOutputTypeDef = TypedDict(
+    "FilterCriteriaOutputTypeDef",
+    {
+        "awsAccountId": NotRequired[List[StringFilterTypeDef]],
+        "codeVulnerabilityDetectorName": NotRequired[List[StringFilterTypeDef]],
+        "codeVulnerabilityDetectorTags": NotRequired[List[StringFilterTypeDef]],
+        "codeVulnerabilityFilePath": NotRequired[List[StringFilterTypeDef]],
+        "componentId": NotRequired[List[StringFilterTypeDef]],
+        "componentType": NotRequired[List[StringFilterTypeDef]],
+        "ec2InstanceImageId": NotRequired[List[StringFilterTypeDef]],
+        "ec2InstanceSubnetId": NotRequired[List[StringFilterTypeDef]],
+        "ec2InstanceVpcId": NotRequired[List[StringFilterTypeDef]],
+        "ecrImageArchitecture": NotRequired[List[StringFilterTypeDef]],
+        "ecrImageHash": NotRequired[List[StringFilterTypeDef]],
+        "ecrImagePushedAt": NotRequired[List[DateFilterOutputTypeDef]],
+        "ecrImageRegistry": NotRequired[List[StringFilterTypeDef]],
+        "ecrImageRepositoryName": NotRequired[List[StringFilterTypeDef]],
+        "ecrImageTags": NotRequired[List[StringFilterTypeDef]],
+        "epssScore": NotRequired[List[NumberFilterTypeDef]],
+        "exploitAvailable": NotRequired[List[StringFilterTypeDef]],
+        "findingArn": NotRequired[List[StringFilterTypeDef]],
+        "findingStatus": NotRequired[List[StringFilterTypeDef]],
+        "findingType": NotRequired[List[StringFilterTypeDef]],
+        "firstObservedAt": NotRequired[List[DateFilterOutputTypeDef]],
+        "fixAvailable": NotRequired[List[StringFilterTypeDef]],
+        "inspectorScore": NotRequired[List[NumberFilterTypeDef]],
+        "lambdaFunctionExecutionRoleArn": NotRequired[List[StringFilterTypeDef]],
+        "lambdaFunctionLastModifiedAt": NotRequired[List[DateFilterOutputTypeDef]],
+        "lambdaFunctionLayers": NotRequired[List[StringFilterTypeDef]],
+        "lambdaFunctionName": NotRequired[List[StringFilterTypeDef]],
+        "lambdaFunctionRuntime": NotRequired[List[StringFilterTypeDef]],
+        "lastObservedAt": NotRequired[List[DateFilterOutputTypeDef]],
+        "networkProtocol": NotRequired[List[StringFilterTypeDef]],
+        "portRange": NotRequired[List[PortRangeFilterTypeDef]],
+        "relatedVulnerabilities": NotRequired[List[StringFilterTypeDef]],
+        "resourceId": NotRequired[List[StringFilterTypeDef]],
+        "resourceTags": NotRequired[List[MapFilterTypeDef]],
+        "resourceType": NotRequired[List[StringFilterTypeDef]],
+        "severity": NotRequired[List[StringFilterTypeDef]],
+        "title": NotRequired[List[StringFilterTypeDef]],
+        "updatedAt": NotRequired[List[DateFilterOutputTypeDef]],
         "vendorSeverity": NotRequired[List[StringFilterTypeDef]],
         "vulnerabilityId": NotRequired[List[StringFilterTypeDef]],
         "vulnerabilitySource": NotRequired[List[StringFilterTypeDef]],
         "vulnerablePackages": NotRequired[List[PackageFilterTypeDef]],
     },
 )
 FilterCriteriaTypeDef = TypedDict(
@@ -2467,46 +2582,50 @@
     {
         "accountId": str,
         "resourceId": str,
         "resourceType": CoverageResourceTypeType,
         "scanType": ScanTypeType,
         "lastScannedAt": NotRequired[datetime],
         "resourceMetadata": NotRequired[ResourceScanMetadataTypeDef],
+        "scanMode": NotRequired[ScanModeType],
         "scanStatus": NotRequired[ScanStatusTypeDef],
     },
 )
 NetworkReachabilityDetailsTypeDef = TypedDict(
     "NetworkReachabilityDetailsTypeDef",
     {
         "networkPath": NetworkPathTypeDef,
         "openPortRange": PortRangeTypeDef,
         "protocol": NetworkProtocolType,
     },
 )
-CreateSbomExportRequestRequestTypeDef = TypedDict(
-    "CreateSbomExportRequestRequestTypeDef",
-    {
-        "reportFormat": SbomReportFormatType,
-        "s3Destination": DestinationTypeDef,
-        "resourceFilterCriteria": NotRequired[ResourceFilterCriteriaTypeDef],
-    },
-)
 GetSbomExportResponseTypeDef = TypedDict(
     "GetSbomExportResponseTypeDef",
     {
         "errorCode": ReportingErrorCodeType,
         "errorMessage": str,
-        "filterCriteria": ResourceFilterCriteriaTypeDef,
+        "filterCriteria": ResourceFilterCriteriaOutputTypeDef,
         "format": SbomReportFormatType,
         "reportId": str,
         "s3Destination": DestinationTypeDef,
         "status": ExternalReportStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateSbomExportRequestRequestTypeDef = TypedDict(
+    "CreateSbomExportRequestRequestTypeDef",
+    {
+        "reportFormat": SbomReportFormatType,
+        "s3Destination": DestinationTypeDef,
+        "resourceFilterCriteria": NotRequired[ResourceFilterCriteriaTypeDef],
+    },
+)
+ResourceFilterCriteriaUnionTypeDef = Union[
+    ResourceFilterCriteriaTypeDef, ResourceFilterCriteriaOutputTypeDef
+]
 StopCisSessionRequestRequestTypeDef = TypedDict(
     "StopCisSessionRequestRequestTypeDef",
     {
         "message": StopCisSessionMessageTypeDef,
         "scanJobId": str,
         "sessionToken": str,
     },
@@ -2595,33 +2714,21 @@
     "ListCoverageStatisticsRequestRequestTypeDef",
     {
         "filterCriteria": NotRequired[CoverageFilterCriteriaTypeDef],
         "groupBy": NotRequired[GroupKeyType],
         "nextToken": NotRequired[str],
     },
 )
-CisScanConfigurationPaginatorTypeDef = TypedDict(
-    "CisScanConfigurationPaginatorTypeDef",
-    {
-        "scanConfigurationArn": str,
-        "ownerId": NotRequired[str],
-        "scanName": NotRequired[str],
-        "schedule": NotRequired[SchedulePaginatorTypeDef],
-        "securityLevel": NotRequired[CisSecurityLevelType],
-        "tags": NotRequired[Dict[str, str]],
-        "targets": NotRequired[CisTargetsTypeDef],
-    },
-)
 CisScanConfigurationTypeDef = TypedDict(
     "CisScanConfigurationTypeDef",
     {
         "scanConfigurationArn": str,
         "ownerId": NotRequired[str],
         "scanName": NotRequired[str],
-        "schedule": NotRequired[ScheduleTypeDef],
+        "schedule": NotRequired[ScheduleOutputTypeDef],
         "securityLevel": NotRequired[CisSecurityLevelType],
         "tags": NotRequired[Dict[str, str]],
         "targets": NotRequired[CisTargetsTypeDef],
     },
 )
 CreateCisScanConfigurationRequestRequestTypeDef = TypedDict(
     "CreateCisScanConfigurationRequestRequestTypeDef",
@@ -2629,14 +2736,15 @@
         "scanName": str,
         "schedule": ScheduleTypeDef,
         "securityLevel": CisSecurityLevelType,
         "targets": CreateCisTargetsTypeDef,
         "tags": NotRequired[Mapping[str, str]],
     },
 )
+ScheduleUnionTypeDef = Union[ScheduleTypeDef, ScheduleExtraOutputTypeDef]
 UpdateCisScanConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateCisScanConfigurationRequestRequestTypeDef",
     {
         "scanConfigurationArn": str,
         "scanName": NotRequired[str],
         "schedule": NotRequired[ScheduleTypeDef],
         "securityLevel": NotRequired[CisSecurityLevelType],
@@ -2658,35 +2766,39 @@
         "aggregationType": AggregationTypeType,
         "accountIds": NotRequired[Sequence[StringFilterTypeDef]],
         "aggregationRequest": NotRequired[AggregationRequestTypeDef],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
-FilterPaginatorTypeDef = TypedDict(
-    "FilterPaginatorTypeDef",
+FilterTypeDef = TypedDict(
+    "FilterTypeDef",
     {
         "action": FilterActionType,
         "arn": str,
         "createdAt": datetime,
-        "criteria": FilterCriteriaPaginatorTypeDef,
+        "criteria": FilterCriteriaOutputTypeDef,
         "name": str,
         "ownerId": str,
         "updatedAt": datetime,
         "description": NotRequired[str],
         "reason": NotRequired[str],
         "tags": NotRequired[Dict[str, str]],
     },
 )
-ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
-    "ListFindingsRequestListFindingsPaginateTypeDef",
+GetFindingsReportStatusResponseTypeDef = TypedDict(
+    "GetFindingsReportStatusResponseTypeDef",
     {
-        "filterCriteria": NotRequired[FilterCriteriaPaginatorTypeDef],
-        "sortCriteria": NotRequired[SortCriteriaTypeDef],
-        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+        "destination": DestinationTypeDef,
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": FilterCriteriaOutputTypeDef,
+        "reportId": str,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateFilterRequestRequestTypeDef = TypedDict(
     "CreateFilterRequestRequestTypeDef",
     {
         "action": FilterActionType,
         "filterCriteria": FilterCriteriaTypeDef,
@@ -2700,39 +2812,21 @@
     "CreateFindingsReportRequestRequestTypeDef",
     {
         "reportFormat": ReportFormatType,
         "s3Destination": DestinationTypeDef,
         "filterCriteria": NotRequired[FilterCriteriaTypeDef],
     },
 )
-FilterTypeDef = TypedDict(
-    "FilterTypeDef",
-    {
-        "action": FilterActionType,
-        "arn": str,
-        "createdAt": datetime,
-        "criteria": FilterCriteriaTypeDef,
-        "name": str,
-        "ownerId": str,
-        "updatedAt": datetime,
-        "description": NotRequired[str],
-        "reason": NotRequired[str],
-        "tags": NotRequired[Dict[str, str]],
-    },
-)
-GetFindingsReportStatusResponseTypeDef = TypedDict(
-    "GetFindingsReportStatusResponseTypeDef",
+FilterCriteriaUnionTypeDef = Union[FilterCriteriaTypeDef, FilterCriteriaExtraOutputTypeDef]
+ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
+    "ListFindingsRequestListFindingsPaginateTypeDef",
     {
-        "destination": DestinationTypeDef,
-        "errorCode": ReportingErrorCodeType,
-        "errorMessage": str,
-        "filterCriteria": FilterCriteriaTypeDef,
-        "reportId": str,
-        "status": ExternalReportStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "filterCriteria": NotRequired[FilterCriteriaTypeDef],
+        "sortCriteria": NotRequired[SortCriteriaTypeDef],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
         "filterCriteria": NotRequired[FilterCriteriaTypeDef],
         "maxResults": NotRequired[int],
@@ -2781,38 +2875,22 @@
         "inspectorScoreDetails": NotRequired[InspectorScoreDetailsTypeDef],
         "networkReachabilityDetails": NotRequired[NetworkReachabilityDetailsTypeDef],
         "packageVulnerabilityDetails": NotRequired[PackageVulnerabilityDetailsTypeDef],
         "title": NotRequired[str],
         "updatedAt": NotRequired[datetime],
     },
 )
-ListCisScanConfigurationsResponsePaginatorTypeDef = TypedDict(
-    "ListCisScanConfigurationsResponsePaginatorTypeDef",
-    {
-        "nextToken": str,
-        "scanConfigurations": List[CisScanConfigurationPaginatorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListCisScanConfigurationsResponseTypeDef = TypedDict(
     "ListCisScanConfigurationsResponseTypeDef",
     {
         "nextToken": str,
         "scanConfigurations": List[CisScanConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListFiltersResponsePaginatorTypeDef = TypedDict(
-    "ListFiltersResponsePaginatorTypeDef",
-    {
-        "filters": List[FilterPaginatorTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListFiltersResponseTypeDef = TypedDict(
     "ListFiltersResponseTypeDef",
     {
         "filters": List[FilterTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2/type_defs.pyi` & `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     CoverageResourceTypeType,
     CoverageStringComparisonType,
     DayType,
     DelegatedAdminStatusType,
     Ec2DeepInspectionStatusType,
     Ec2InstanceSortByType,
     Ec2PlatformType,
+    Ec2ScanModeStatusType,
+    Ec2ScanModeType,
     EcrPullDateRescanDurationType,
     EcrRescanDurationStatusType,
     EcrRescanDurationType,
     EcrScanFrequencyType,
     ErrorCodeType,
     ExploitAvailableType,
     ExternalReportStatusType,
@@ -80,14 +82,15 @@
     ReportingErrorCodeType,
     RepositorySortByType,
     ResourceScanTypeType,
     ResourceStringComparisonType,
     ResourceTypeType,
     RuntimeType,
     SbomReportFormatType,
+    ScanModeType,
     ScanStatusCodeType,
     ScanStatusReasonType,
     ScanTypeType,
     ServiceType,
     SeverityType,
     SortFieldType,
     SortOrderType,
@@ -164,22 +167,25 @@
     "CreateCisTargetsTypeDef",
     "DestinationTypeDef",
     "Cvss2TypeDef",
     "Cvss3TypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "TimeTypeDef",
-    "DateFilterPaginatorTypeDef",
+    "DateFilterExtraOutputTypeDef",
+    "DateFilterOutputTypeDef",
     "DelegatedAdminAccountTypeDef",
     "DelegatedAdminTypeDef",
     "DeleteCisScanConfigurationRequestRequestTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     "DisableRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
+    "Ec2ScanModeStateTypeDef",
+    "Ec2ConfigurationTypeDef",
     "MapFilterTypeDef",
     "Ec2MetadataTypeDef",
     "EcrRescanDurationStateTypeDef",
     "EcrConfigurationTypeDef",
     "EcrContainerImageMetadataTypeDef",
     "EcrRepositoryMetadataTypeDef",
     "EnableDelegatedAdminAccountRequestRequestTypeDef",
@@ -287,18 +293,20 @@
     "ListCisScanConfigurationsFilterCriteriaTypeDef",
     "CodeVulnerabilityDetailsTypeDef",
     "CodeSnippetResultTypeDef",
     "ListCoverageStatisticsResponseTypeDef",
     "CvssScoreDetailsTypeDef",
     "DailyScheduleTypeDef",
     "MonthlyScheduleTypeDef",
-    "WeeklySchedulePaginatorTypeDef",
+    "WeeklyScheduleExtraOutputTypeDef",
+    "WeeklyScheduleOutputTypeDef",
     "WeeklyScheduleTypeDef",
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
+    "Ec2ConfigurationStateTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "FindingDetailTypeDef",
     "VulnerabilityTypeDef",
     "PackageFilterTypeDef",
@@ -311,14 +319,15 @@
     "GetMemberResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ResourceScanMetadataTypeDef",
     "ListAccountPermissionsResponseTypeDef",
     "NetworkPathTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
+    "ResourceFilterCriteriaOutputTypeDef",
     "ResourceFilterCriteriaTypeDef",
     "SearchVulnerabilitiesRequestRequestTypeDef",
     "SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
     "StartCisSessionRequestRequestTypeDef",
     "StopCisSessionMessageTypeDef",
     "UsageTotalTypeDef",
     "AggregationResponseTypeDef",
@@ -338,57 +347,58 @@
     "ListCisScanResultsAggregatedByChecksRequestRequestTypeDef",
     "ListCisScanResultsAggregatedByTargetResourceRequestListCisScanResultsAggregatedByTargetResourcePaginateTypeDef",
     "ListCisScanResultsAggregatedByTargetResourceRequestRequestTypeDef",
     "ListCisScanConfigurationsRequestListCisScanConfigurationsPaginateTypeDef",
     "ListCisScanConfigurationsRequestRequestTypeDef",
     "BatchGetCodeSnippetResponseTypeDef",
     "InspectorScoreDetailsTypeDef",
-    "SchedulePaginatorTypeDef",
+    "ScheduleExtraOutputTypeDef",
+    "ScheduleOutputTypeDef",
     "ScheduleTypeDef",
     "AggregationRequestTypeDef",
     "GetConfigurationResponseTypeDef",
     "BatchGetFindingDetailsResponseTypeDef",
     "SearchVulnerabilitiesResponseTypeDef",
-    "FilterCriteriaPaginatorTypeDef",
+    "FilterCriteriaExtraOutputTypeDef",
+    "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "BatchGetFreeTrialInfoResponseTypeDef",
     "CoveredResourceTypeDef",
     "NetworkReachabilityDetailsTypeDef",
-    "CreateSbomExportRequestRequestTypeDef",
     "GetSbomExportResponseTypeDef",
+    "CreateSbomExportRequestRequestTypeDef",
+    "ResourceFilterCriteriaUnionTypeDef",
     "StopCisSessionRequestRequestTypeDef",
     "ListUsageTotalsResponseTypeDef",
     "ListFindingAggregationsResponseTypeDef",
     "BatchGetAccountStatusResponseTypeDef",
     "ResourceTypeDef",
     "ListCisScansRequestListCisScansPaginateTypeDef",
     "ListCisScansRequestRequestTypeDef",
     "ListCoverageRequestListCoveragePaginateTypeDef",
     "ListCoverageRequestRequestTypeDef",
     "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
     "ListCoverageStatisticsRequestRequestTypeDef",
-    "CisScanConfigurationPaginatorTypeDef",
     "CisScanConfigurationTypeDef",
     "CreateCisScanConfigurationRequestRequestTypeDef",
+    "ScheduleUnionTypeDef",
     "UpdateCisScanConfigurationRequestRequestTypeDef",
     "ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     "ListFindingAggregationsRequestRequestTypeDef",
-    "FilterPaginatorTypeDef",
-    "ListFindingsRequestListFindingsPaginateTypeDef",
-    "CreateFilterRequestRequestTypeDef",
-    "CreateFindingsReportRequestRequestTypeDef",
     "FilterTypeDef",
     "GetFindingsReportStatusResponseTypeDef",
+    "CreateFilterRequestRequestTypeDef",
+    "CreateFindingsReportRequestRequestTypeDef",
+    "FilterCriteriaUnionTypeDef",
+    "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "ListCoverageResponseTypeDef",
     "FindingTypeDef",
-    "ListCisScanConfigurationsResponsePaginatorTypeDef",
     "ListCisScanConfigurationsResponseTypeDef",
-    "ListFiltersResponsePaginatorTypeDef",
     "ListFiltersResponseTypeDef",
     "ListFindingsResponseTypeDef",
 )
 
 SeverityCountsTypeDef = TypedDict(
     "SeverityCountsTypeDef",
     {
@@ -446,18 +456,18 @@
         "accountId": str,
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
 AtigDataTypeDef = TypedDict(
     "AtigDataTypeDef",
     {
         "firstSeen": NotRequired[datetime],
         "lastSeen": NotRequired[datetime],
@@ -813,16 +823,23 @@
 TimeTypeDef = TypedDict(
     "TimeTypeDef",
     {
         "timeOfDay": str,
         "timezone": str,
     },
 )
-DateFilterPaginatorTypeDef = TypedDict(
-    "DateFilterPaginatorTypeDef",
+DateFilterExtraOutputTypeDef = TypedDict(
+    "DateFilterExtraOutputTypeDef",
+    {
+        "endInclusive": NotRequired[datetime],
+        "startInclusive": NotRequired[datetime],
+    },
+)
+DateFilterOutputTypeDef = TypedDict(
+    "DateFilterOutputTypeDef",
     {
         "endInclusive": NotRequired[datetime],
         "startInclusive": NotRequired[datetime],
     },
 )
 DelegatedAdminAccountTypeDef = TypedDict(
     "DelegatedAdminAccountTypeDef",
@@ -865,14 +882,27 @@
 )
 DisassociateMemberRequestRequestTypeDef = TypedDict(
     "DisassociateMemberRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
+Ec2ScanModeStateTypeDef = TypedDict(
+    "Ec2ScanModeStateTypeDef",
+    {
+        "scanMode": NotRequired[Ec2ScanModeType],
+        "scanModeStatus": NotRequired[Ec2ScanModeStatusType],
+    },
+)
+Ec2ConfigurationTypeDef = TypedDict(
+    "Ec2ConfigurationTypeDef",
+    {
+        "scanMode": Ec2ScanModeType,
+    },
+)
 MapFilterTypeDef = TypedDict(
     "MapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
         "value": NotRequired[str],
     },
@@ -1816,16 +1846,23 @@
 MonthlyScheduleTypeDef = TypedDict(
     "MonthlyScheduleTypeDef",
     {
         "day": DayType,
         "startTime": TimeTypeDef,
     },
 )
-WeeklySchedulePaginatorTypeDef = TypedDict(
-    "WeeklySchedulePaginatorTypeDef",
+WeeklyScheduleExtraOutputTypeDef = TypedDict(
+    "WeeklyScheduleExtraOutputTypeDef",
+    {
+        "days": List[DayType],
+        "startTime": TimeTypeDef,
+    },
+)
+WeeklyScheduleOutputTypeDef = TypedDict(
+    "WeeklyScheduleOutputTypeDef",
     {
         "days": List[DayType],
         "startTime": TimeTypeDef,
     },
 )
 WeeklyScheduleTypeDef = TypedDict(
     "WeeklyScheduleTypeDef",
@@ -1845,14 +1882,20 @@
 GetDelegatedAdminAccountResponseTypeDef = TypedDict(
     "GetDelegatedAdminAccountResponseTypeDef",
     {
         "delegatedAdmin": DelegatedAdminTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+Ec2ConfigurationStateTypeDef = TypedDict(
+    "Ec2ConfigurationStateTypeDef",
+    {
+        "scanModeState": NotRequired[Ec2ScanModeStateTypeDef],
+    },
+)
 Ec2InstanceAggregationTypeDef = TypedDict(
     "Ec2InstanceAggregationTypeDef",
     {
         "amis": NotRequired[Sequence[StringFilterTypeDef]],
         "instanceIds": NotRequired[Sequence[StringFilterTypeDef]],
         "instanceTags": NotRequired[Sequence[MapFilterTypeDef]],
         "operatingSystems": NotRequired[Sequence[StringFilterTypeDef]],
@@ -1876,15 +1919,16 @@
     {
         "rescanDurationState": NotRequired[EcrRescanDurationStateTypeDef],
     },
 )
 UpdateConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationRequestRequestTypeDef",
     {
-        "ecrConfiguration": EcrConfigurationTypeDef,
+        "ec2Configuration": NotRequired[Ec2ConfigurationTypeDef],
+        "ecrConfiguration": NotRequired[EcrConfigurationTypeDef],
     },
 )
 FindingDetailTypeDef = TypedDict(
     "FindingDetailTypeDef",
     {
         "cisaData": NotRequired[CisaDataTypeDef],
         "cwes": NotRequired[List[str]],
@@ -2029,14 +2073,27 @@
 )
 RemediationTypeDef = TypedDict(
     "RemediationTypeDef",
     {
         "recommendation": NotRequired[RecommendationTypeDef],
     },
 )
+ResourceFilterCriteriaOutputTypeDef = TypedDict(
+    "ResourceFilterCriteriaOutputTypeDef",
+    {
+        "accountId": NotRequired[List[ResourceStringFilterTypeDef]],
+        "ec2InstanceTags": NotRequired[List[ResourceMapFilterTypeDef]],
+        "ecrImageTags": NotRequired[List[ResourceStringFilterTypeDef]],
+        "ecrRepositoryName": NotRequired[List[ResourceStringFilterTypeDef]],
+        "lambdaFunctionName": NotRequired[List[ResourceStringFilterTypeDef]],
+        "lambdaFunctionTags": NotRequired[List[ResourceMapFilterTypeDef]],
+        "resourceId": NotRequired[List[ResourceStringFilterTypeDef]],
+        "resourceType": NotRequired[List[ResourceStringFilterTypeDef]],
+    },
+)
 ResourceFilterCriteriaTypeDef = TypedDict(
     "ResourceFilterCriteriaTypeDef",
     {
         "accountId": NotRequired[Sequence[ResourceStringFilterTypeDef]],
         "ec2InstanceTags": NotRequired[Sequence[ResourceMapFilterTypeDef]],
         "ecrImageTags": NotRequired[Sequence[ResourceStringFilterTypeDef]],
         "ecrRepositoryName": NotRequired[Sequence[ResourceStringFilterTypeDef]],
@@ -2182,14 +2239,15 @@
         "imagePulledAt": NotRequired[Sequence[CoverageDateFilterTypeDef]],
         "lambdaFunctionName": NotRequired[Sequence[CoverageStringFilterTypeDef]],
         "lambdaFunctionRuntime": NotRequired[Sequence[CoverageStringFilterTypeDef]],
         "lambdaFunctionTags": NotRequired[Sequence[CoverageMapFilterTypeDef]],
         "lastScannedAt": NotRequired[Sequence[CoverageDateFilterTypeDef]],
         "resourceId": NotRequired[Sequence[CoverageStringFilterTypeDef]],
         "resourceType": NotRequired[Sequence[CoverageStringFilterTypeDef]],
+        "scanMode": NotRequired[Sequence[CoverageStringFilterTypeDef]],
         "scanStatusCode": NotRequired[Sequence[CoverageStringFilterTypeDef]],
         "scanStatusReason": NotRequired[Sequence[CoverageStringFilterTypeDef]],
         "scanType": NotRequired[Sequence[CoverageStringFilterTypeDef]],
     },
 )
 ListCisScansResponseTypeDef = TypedDict(
     "ListCisScansResponseTypeDef",
@@ -2299,21 +2357,30 @@
 )
 InspectorScoreDetailsTypeDef = TypedDict(
     "InspectorScoreDetailsTypeDef",
     {
         "adjustedCvss": NotRequired[CvssScoreDetailsTypeDef],
     },
 )
-SchedulePaginatorTypeDef = TypedDict(
-    "SchedulePaginatorTypeDef",
+ScheduleExtraOutputTypeDef = TypedDict(
+    "ScheduleExtraOutputTypeDef",
     {
         "daily": NotRequired[DailyScheduleTypeDef],
         "monthly": NotRequired[MonthlyScheduleTypeDef],
         "oneTime": NotRequired[Dict[str, Any]],
-        "weekly": NotRequired[WeeklySchedulePaginatorTypeDef],
+        "weekly": NotRequired[WeeklyScheduleExtraOutputTypeDef],
+    },
+)
+ScheduleOutputTypeDef = TypedDict(
+    "ScheduleOutputTypeDef",
+    {
+        "daily": NotRequired[DailyScheduleTypeDef],
+        "monthly": NotRequired[MonthlyScheduleTypeDef],
+        "oneTime": NotRequired[Dict[str, Any]],
+        "weekly": NotRequired[WeeklyScheduleOutputTypeDef],
     },
 )
 ScheduleTypeDef = TypedDict(
     "ScheduleTypeDef",
     {
         "daily": NotRequired[DailyScheduleTypeDef],
         "monthly": NotRequired[MonthlyScheduleTypeDef],
@@ -2336,14 +2403,15 @@
         "repositoryAggregation": NotRequired[RepositoryAggregationTypeDef],
         "titleAggregation": NotRequired[TitleAggregationTypeDef],
     },
 )
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
+        "ec2Configuration": Ec2ConfigurationStateTypeDef,
         "ecrConfiguration": EcrConfigurationStateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 BatchGetFindingDetailsResponseTypeDef = TypedDict(
     "BatchGetFindingDetailsResponseTypeDef",
     {
@@ -2356,55 +2424,102 @@
     "SearchVulnerabilitiesResponseTypeDef",
     {
         "nextToken": str,
         "vulnerabilities": List[VulnerabilityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-FilterCriteriaPaginatorTypeDef = TypedDict(
-    "FilterCriteriaPaginatorTypeDef",
+FilterCriteriaExtraOutputTypeDef = TypedDict(
+    "FilterCriteriaExtraOutputTypeDef",
     {
         "awsAccountId": NotRequired[List[StringFilterTypeDef]],
         "codeVulnerabilityDetectorName": NotRequired[List[StringFilterTypeDef]],
         "codeVulnerabilityDetectorTags": NotRequired[List[StringFilterTypeDef]],
         "codeVulnerabilityFilePath": NotRequired[List[StringFilterTypeDef]],
         "componentId": NotRequired[List[StringFilterTypeDef]],
         "componentType": NotRequired[List[StringFilterTypeDef]],
         "ec2InstanceImageId": NotRequired[List[StringFilterTypeDef]],
         "ec2InstanceSubnetId": NotRequired[List[StringFilterTypeDef]],
         "ec2InstanceVpcId": NotRequired[List[StringFilterTypeDef]],
         "ecrImageArchitecture": NotRequired[List[StringFilterTypeDef]],
         "ecrImageHash": NotRequired[List[StringFilterTypeDef]],
-        "ecrImagePushedAt": NotRequired[List[DateFilterPaginatorTypeDef]],
+        "ecrImagePushedAt": NotRequired[List[DateFilterExtraOutputTypeDef]],
         "ecrImageRegistry": NotRequired[List[StringFilterTypeDef]],
         "ecrImageRepositoryName": NotRequired[List[StringFilterTypeDef]],
         "ecrImageTags": NotRequired[List[StringFilterTypeDef]],
         "epssScore": NotRequired[List[NumberFilterTypeDef]],
         "exploitAvailable": NotRequired[List[StringFilterTypeDef]],
         "findingArn": NotRequired[List[StringFilterTypeDef]],
         "findingStatus": NotRequired[List[StringFilterTypeDef]],
         "findingType": NotRequired[List[StringFilterTypeDef]],
-        "firstObservedAt": NotRequired[List[DateFilterPaginatorTypeDef]],
+        "firstObservedAt": NotRequired[List[DateFilterExtraOutputTypeDef]],
         "fixAvailable": NotRequired[List[StringFilterTypeDef]],
         "inspectorScore": NotRequired[List[NumberFilterTypeDef]],
         "lambdaFunctionExecutionRoleArn": NotRequired[List[StringFilterTypeDef]],
-        "lambdaFunctionLastModifiedAt": NotRequired[List[DateFilterPaginatorTypeDef]],
+        "lambdaFunctionLastModifiedAt": NotRequired[List[DateFilterExtraOutputTypeDef]],
         "lambdaFunctionLayers": NotRequired[List[StringFilterTypeDef]],
         "lambdaFunctionName": NotRequired[List[StringFilterTypeDef]],
         "lambdaFunctionRuntime": NotRequired[List[StringFilterTypeDef]],
-        "lastObservedAt": NotRequired[List[DateFilterPaginatorTypeDef]],
+        "lastObservedAt": NotRequired[List[DateFilterExtraOutputTypeDef]],
         "networkProtocol": NotRequired[List[StringFilterTypeDef]],
         "portRange": NotRequired[List[PortRangeFilterTypeDef]],
         "relatedVulnerabilities": NotRequired[List[StringFilterTypeDef]],
         "resourceId": NotRequired[List[StringFilterTypeDef]],
         "resourceTags": NotRequired[List[MapFilterTypeDef]],
         "resourceType": NotRequired[List[StringFilterTypeDef]],
         "severity": NotRequired[List[StringFilterTypeDef]],
         "title": NotRequired[List[StringFilterTypeDef]],
-        "updatedAt": NotRequired[List[DateFilterPaginatorTypeDef]],
+        "updatedAt": NotRequired[List[DateFilterExtraOutputTypeDef]],
+        "vendorSeverity": NotRequired[List[StringFilterTypeDef]],
+        "vulnerabilityId": NotRequired[List[StringFilterTypeDef]],
+        "vulnerabilitySource": NotRequired[List[StringFilterTypeDef]],
+        "vulnerablePackages": NotRequired[List[PackageFilterTypeDef]],
+    },
+)
+FilterCriteriaOutputTypeDef = TypedDict(
+    "FilterCriteriaOutputTypeDef",
+    {
+        "awsAccountId": NotRequired[List[StringFilterTypeDef]],
+        "codeVulnerabilityDetectorName": NotRequired[List[StringFilterTypeDef]],
+        "codeVulnerabilityDetectorTags": NotRequired[List[StringFilterTypeDef]],
+        "codeVulnerabilityFilePath": NotRequired[List[StringFilterTypeDef]],
+        "componentId": NotRequired[List[StringFilterTypeDef]],
+        "componentType": NotRequired[List[StringFilterTypeDef]],
+        "ec2InstanceImageId": NotRequired[List[StringFilterTypeDef]],
+        "ec2InstanceSubnetId": NotRequired[List[StringFilterTypeDef]],
+        "ec2InstanceVpcId": NotRequired[List[StringFilterTypeDef]],
+        "ecrImageArchitecture": NotRequired[List[StringFilterTypeDef]],
+        "ecrImageHash": NotRequired[List[StringFilterTypeDef]],
+        "ecrImagePushedAt": NotRequired[List[DateFilterOutputTypeDef]],
+        "ecrImageRegistry": NotRequired[List[StringFilterTypeDef]],
+        "ecrImageRepositoryName": NotRequired[List[StringFilterTypeDef]],
+        "ecrImageTags": NotRequired[List[StringFilterTypeDef]],
+        "epssScore": NotRequired[List[NumberFilterTypeDef]],
+        "exploitAvailable": NotRequired[List[StringFilterTypeDef]],
+        "findingArn": NotRequired[List[StringFilterTypeDef]],
+        "findingStatus": NotRequired[List[StringFilterTypeDef]],
+        "findingType": NotRequired[List[StringFilterTypeDef]],
+        "firstObservedAt": NotRequired[List[DateFilterOutputTypeDef]],
+        "fixAvailable": NotRequired[List[StringFilterTypeDef]],
+        "inspectorScore": NotRequired[List[NumberFilterTypeDef]],
+        "lambdaFunctionExecutionRoleArn": NotRequired[List[StringFilterTypeDef]],
+        "lambdaFunctionLastModifiedAt": NotRequired[List[DateFilterOutputTypeDef]],
+        "lambdaFunctionLayers": NotRequired[List[StringFilterTypeDef]],
+        "lambdaFunctionName": NotRequired[List[StringFilterTypeDef]],
+        "lambdaFunctionRuntime": NotRequired[List[StringFilterTypeDef]],
+        "lastObservedAt": NotRequired[List[DateFilterOutputTypeDef]],
+        "networkProtocol": NotRequired[List[StringFilterTypeDef]],
+        "portRange": NotRequired[List[PortRangeFilterTypeDef]],
+        "relatedVulnerabilities": NotRequired[List[StringFilterTypeDef]],
+        "resourceId": NotRequired[List[StringFilterTypeDef]],
+        "resourceTags": NotRequired[List[MapFilterTypeDef]],
+        "resourceType": NotRequired[List[StringFilterTypeDef]],
+        "severity": NotRequired[List[StringFilterTypeDef]],
+        "title": NotRequired[List[StringFilterTypeDef]],
+        "updatedAt": NotRequired[List[DateFilterOutputTypeDef]],
         "vendorSeverity": NotRequired[List[StringFilterTypeDef]],
         "vulnerabilityId": NotRequired[List[StringFilterTypeDef]],
         "vulnerabilitySource": NotRequired[List[StringFilterTypeDef]],
         "vulnerablePackages": NotRequired[List[PackageFilterTypeDef]],
     },
 )
 FilterCriteriaTypeDef = TypedDict(
@@ -2467,46 +2582,50 @@
     {
         "accountId": str,
         "resourceId": str,
         "resourceType": CoverageResourceTypeType,
         "scanType": ScanTypeType,
         "lastScannedAt": NotRequired[datetime],
         "resourceMetadata": NotRequired[ResourceScanMetadataTypeDef],
+        "scanMode": NotRequired[ScanModeType],
         "scanStatus": NotRequired[ScanStatusTypeDef],
     },
 )
 NetworkReachabilityDetailsTypeDef = TypedDict(
     "NetworkReachabilityDetailsTypeDef",
     {
         "networkPath": NetworkPathTypeDef,
         "openPortRange": PortRangeTypeDef,
         "protocol": NetworkProtocolType,
     },
 )
-CreateSbomExportRequestRequestTypeDef = TypedDict(
-    "CreateSbomExportRequestRequestTypeDef",
-    {
-        "reportFormat": SbomReportFormatType,
-        "s3Destination": DestinationTypeDef,
-        "resourceFilterCriteria": NotRequired[ResourceFilterCriteriaTypeDef],
-    },
-)
 GetSbomExportResponseTypeDef = TypedDict(
     "GetSbomExportResponseTypeDef",
     {
         "errorCode": ReportingErrorCodeType,
         "errorMessage": str,
-        "filterCriteria": ResourceFilterCriteriaTypeDef,
+        "filterCriteria": ResourceFilterCriteriaOutputTypeDef,
         "format": SbomReportFormatType,
         "reportId": str,
         "s3Destination": DestinationTypeDef,
         "status": ExternalReportStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateSbomExportRequestRequestTypeDef = TypedDict(
+    "CreateSbomExportRequestRequestTypeDef",
+    {
+        "reportFormat": SbomReportFormatType,
+        "s3Destination": DestinationTypeDef,
+        "resourceFilterCriteria": NotRequired[ResourceFilterCriteriaTypeDef],
+    },
+)
+ResourceFilterCriteriaUnionTypeDef = Union[
+    ResourceFilterCriteriaTypeDef, ResourceFilterCriteriaOutputTypeDef
+]
 StopCisSessionRequestRequestTypeDef = TypedDict(
     "StopCisSessionRequestRequestTypeDef",
     {
         "message": StopCisSessionMessageTypeDef,
         "scanJobId": str,
         "sessionToken": str,
     },
@@ -2595,33 +2714,21 @@
     "ListCoverageStatisticsRequestRequestTypeDef",
     {
         "filterCriteria": NotRequired[CoverageFilterCriteriaTypeDef],
         "groupBy": NotRequired[GroupKeyType],
         "nextToken": NotRequired[str],
     },
 )
-CisScanConfigurationPaginatorTypeDef = TypedDict(
-    "CisScanConfigurationPaginatorTypeDef",
-    {
-        "scanConfigurationArn": str,
-        "ownerId": NotRequired[str],
-        "scanName": NotRequired[str],
-        "schedule": NotRequired[SchedulePaginatorTypeDef],
-        "securityLevel": NotRequired[CisSecurityLevelType],
-        "tags": NotRequired[Dict[str, str]],
-        "targets": NotRequired[CisTargetsTypeDef],
-    },
-)
 CisScanConfigurationTypeDef = TypedDict(
     "CisScanConfigurationTypeDef",
     {
         "scanConfigurationArn": str,
         "ownerId": NotRequired[str],
         "scanName": NotRequired[str],
-        "schedule": NotRequired[ScheduleTypeDef],
+        "schedule": NotRequired[ScheduleOutputTypeDef],
         "securityLevel": NotRequired[CisSecurityLevelType],
         "tags": NotRequired[Dict[str, str]],
         "targets": NotRequired[CisTargetsTypeDef],
     },
 )
 CreateCisScanConfigurationRequestRequestTypeDef = TypedDict(
     "CreateCisScanConfigurationRequestRequestTypeDef",
@@ -2629,14 +2736,15 @@
         "scanName": str,
         "schedule": ScheduleTypeDef,
         "securityLevel": CisSecurityLevelType,
         "targets": CreateCisTargetsTypeDef,
         "tags": NotRequired[Mapping[str, str]],
     },
 )
+ScheduleUnionTypeDef = Union[ScheduleTypeDef, ScheduleExtraOutputTypeDef]
 UpdateCisScanConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateCisScanConfigurationRequestRequestTypeDef",
     {
         "scanConfigurationArn": str,
         "scanName": NotRequired[str],
         "schedule": NotRequired[ScheduleTypeDef],
         "securityLevel": NotRequired[CisSecurityLevelType],
@@ -2658,35 +2766,39 @@
         "aggregationType": AggregationTypeType,
         "accountIds": NotRequired[Sequence[StringFilterTypeDef]],
         "aggregationRequest": NotRequired[AggregationRequestTypeDef],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
-FilterPaginatorTypeDef = TypedDict(
-    "FilterPaginatorTypeDef",
+FilterTypeDef = TypedDict(
+    "FilterTypeDef",
     {
         "action": FilterActionType,
         "arn": str,
         "createdAt": datetime,
-        "criteria": FilterCriteriaPaginatorTypeDef,
+        "criteria": FilterCriteriaOutputTypeDef,
         "name": str,
         "ownerId": str,
         "updatedAt": datetime,
         "description": NotRequired[str],
         "reason": NotRequired[str],
         "tags": NotRequired[Dict[str, str]],
     },
 )
-ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
-    "ListFindingsRequestListFindingsPaginateTypeDef",
+GetFindingsReportStatusResponseTypeDef = TypedDict(
+    "GetFindingsReportStatusResponseTypeDef",
     {
-        "filterCriteria": NotRequired[FilterCriteriaPaginatorTypeDef],
-        "sortCriteria": NotRequired[SortCriteriaTypeDef],
-        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+        "destination": DestinationTypeDef,
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": FilterCriteriaOutputTypeDef,
+        "reportId": str,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateFilterRequestRequestTypeDef = TypedDict(
     "CreateFilterRequestRequestTypeDef",
     {
         "action": FilterActionType,
         "filterCriteria": FilterCriteriaTypeDef,
@@ -2700,39 +2812,21 @@
     "CreateFindingsReportRequestRequestTypeDef",
     {
         "reportFormat": ReportFormatType,
         "s3Destination": DestinationTypeDef,
         "filterCriteria": NotRequired[FilterCriteriaTypeDef],
     },
 )
-FilterTypeDef = TypedDict(
-    "FilterTypeDef",
-    {
-        "action": FilterActionType,
-        "arn": str,
-        "createdAt": datetime,
-        "criteria": FilterCriteriaTypeDef,
-        "name": str,
-        "ownerId": str,
-        "updatedAt": datetime,
-        "description": NotRequired[str],
-        "reason": NotRequired[str],
-        "tags": NotRequired[Dict[str, str]],
-    },
-)
-GetFindingsReportStatusResponseTypeDef = TypedDict(
-    "GetFindingsReportStatusResponseTypeDef",
+FilterCriteriaUnionTypeDef = Union[FilterCriteriaTypeDef, FilterCriteriaExtraOutputTypeDef]
+ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
+    "ListFindingsRequestListFindingsPaginateTypeDef",
     {
-        "destination": DestinationTypeDef,
-        "errorCode": ReportingErrorCodeType,
-        "errorMessage": str,
-        "filterCriteria": FilterCriteriaTypeDef,
-        "reportId": str,
-        "status": ExternalReportStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "filterCriteria": NotRequired[FilterCriteriaTypeDef],
+        "sortCriteria": NotRequired[SortCriteriaTypeDef],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
         "filterCriteria": NotRequired[FilterCriteriaTypeDef],
         "maxResults": NotRequired[int],
@@ -2781,38 +2875,22 @@
         "inspectorScoreDetails": NotRequired[InspectorScoreDetailsTypeDef],
         "networkReachabilityDetails": NotRequired[NetworkReachabilityDetailsTypeDef],
         "packageVulnerabilityDetails": NotRequired[PackageVulnerabilityDetailsTypeDef],
         "title": NotRequired[str],
         "updatedAt": NotRequired[datetime],
     },
 )
-ListCisScanConfigurationsResponsePaginatorTypeDef = TypedDict(
-    "ListCisScanConfigurationsResponsePaginatorTypeDef",
-    {
-        "nextToken": str,
-        "scanConfigurations": List[CisScanConfigurationPaginatorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListCisScanConfigurationsResponseTypeDef = TypedDict(
     "ListCisScanConfigurationsResponseTypeDef",
     {
         "nextToken": str,
         "scanConfigurations": List[CisScanConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListFiltersResponsePaginatorTypeDef = TypedDict(
-    "ListFiltersResponsePaginatorTypeDef",
-    {
-        "filters": List[FilterPaginatorTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListFiltersResponseTypeDef = TypedDict(
     "ListFiltersResponseTypeDef",
     {
         "filters": List[FilterTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2.egg-info/PKG-INFO` & `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.34.29
-Summary: Type annotations for boto3.Inspector2 1.34.29 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.94
+Summary: Type annotations for boto3.Inspector2 1.34.94 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector2)](https://pepy.tech/project/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.34.29](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.34.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
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
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-inspector2-1.34.29/mypy_boto3_inspector2.egg-info/SOURCES.txt` & `mypy_boto3_inspector2-1.34.94/mypy_boto3_inspector2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.34.29/setup.py` & `mypy_boto3_inspector2-1.34.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-inspector2",
-    version="1.34.29",
+    version="1.34.94",
     packages=["mypy_boto3_inspector2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Inspector2 1.34.29 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.Inspector2 1.34.94 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

