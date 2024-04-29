# Comparing `tmp/alibabacloud_dbs20210101-1.0.4.tar.gz` & `tmp/alibabacloud_dbs20210101-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dbs20210101-1.0.4.tar", last modified: Mon Aug 21 01:59:35 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dbs20210101-2.0.0.tar", last modified: Mon Apr 29 04:42:49 2024, max compression
```

## Comparing `alibabacloud_dbs20210101-1.0.4.tar` & `alibabacloud_dbs20210101-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      189 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2328 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/alibabacloud_dbs20210101/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/alibabacloud_dbs20210101/__init__.py
--rw-r--r--   0 root         (0) root         (0)    74521 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/alibabacloud_dbs20210101/client.py
--rw-r--r--   0 root         (0) root         (0)   112015 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/alibabacloud_dbs20210101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/alibabacloud_dbs20210101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/alibabacloud_dbs20210101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/alibabacloud_dbs20210101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/alibabacloud_dbs20210101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/alibabacloud_dbs20210101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/alibabacloud_dbs20210101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2611 2023-08-21 01:59:35.000000 alibabacloud_dbs20210101-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      255 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79419 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101/client.py
+-rw-r--r--   0 root         (0) root         (0)   136353 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/setup.py
```

### Comparing `alibabacloud_dbs20210101-1.0.4/LICENSE` & `alibabacloud_dbs20210101-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dbs20210101-1.0.4/PKG-INFO` & `alibabacloud_dbs20210101-2.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dbs20210101
-Version: 1.0.4
+Version: 2.0.0
 Summary: Alibaba Cloud Dbs (20210101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dbs-20210101/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_dbs20210101-1.0.4/README-CN.md` & `alibabacloud_dbs20210101-2.0.0/README-CN.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dbs-20210101/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_dbs20210101-1.0.4/README.md` & `alibabacloud_dbs20210101-2.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dbs-20210101/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_dbs20210101-1.0.4/alibabacloud_dbs20210101/client.py` & `alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,14 +73,16 @@
     ) -> dbs_20210101_models.ChangeResourceGroupResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.new_resource_group_id):
             query['NewResourceGroupId'] = request.new_resource_group_id
+        if not UtilClient.is_unset(request.region_code):
+            query['RegionCode'] = request.region_code
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -107,14 +109,16 @@
     ) -> dbs_20210101_models.ChangeResourceGroupResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.new_resource_group_id):
             query['NewResourceGroupId'] = request.new_resource_group_id
+        if not UtilClient.is_unset(request.region_code):
+            query['RegionCode'] = request.region_code
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -150,15 +154,23 @@
 
     def create_download_with_options(
         self,
         request: dbs_20210101_models.CreateDownloadRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.CreateDownloadResponse:
         """
-        For ApsaraDB RDS for MySQL instances that use standard SSDs or enhanced SSDs (ESSDs) and meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        For the instances that meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: CreateDownloadRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDownloadResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -205,15 +217,23 @@
 
     async def create_download_with_options_async(
         self,
         request: dbs_20210101_models.CreateDownloadRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.CreateDownloadResponse:
         """
-        For ApsaraDB RDS for MySQL instances that use standard SSDs or enhanced SSDs (ESSDs) and meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        For the instances that meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: CreateDownloadRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDownloadResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -259,274 +279,358 @@
         )
 
     def create_download(
         self,
         request: dbs_20210101_models.CreateDownloadRequest,
     ) -> dbs_20210101_models.CreateDownloadResponse:
         """
-        For ApsaraDB RDS for MySQL instances that use standard SSDs or enhanced SSDs (ESSDs) and meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        For the instances that meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: CreateDownloadRequest
         @return: CreateDownloadResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_download_with_options(request, runtime)
 
     async def create_download_async(
         self,
         request: dbs_20210101_models.CreateDownloadRequest,
     ) -> dbs_20210101_models.CreateDownloadResponse:
         """
-        For ApsaraDB RDS for MySQL instances that use standard SSDs or enhanced SSDs (ESSDs) and meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        For the instances that meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: CreateDownloadRequest
         @return: CreateDownloadResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_download_with_options_async(request, runtime)
 
-    def create_sandbox_instance_with_options(
+    def delete_sandbox_instance_with_options(
         self,
-        request: dbs_20210101_models.CreateSandboxInstanceRequest,
+        request: dbs_20210101_models.DeleteSandboxInstanceRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> dbs_20210101_models.CreateSandboxInstanceResponse:
+    ) -> dbs_20210101_models.DeleteSandboxInstanceResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
-        @param request: CreateSandboxInstanceRequest
+        @param request: DeleteSandboxInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateSandboxInstanceResponse
+        @return: DeleteSandboxInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_plan_id):
             query['BackupPlanId'] = request.backup_plan_id
-        if not UtilClient.is_unset(request.backup_set_id):
-            query['BackupSetId'] = request.backup_set_id
-        if not UtilClient.is_unset(request.restore_time):
-            query['RestoreTime'] = request.restore_time
-        if not UtilClient.is_unset(request.sandbox_instance_name):
-            query['SandboxInstanceName'] = request.sandbox_instance_name
-        if not UtilClient.is_unset(request.sandbox_password):
-            query['SandboxPassword'] = request.sandbox_password
-        if not UtilClient.is_unset(request.sandbox_specification):
-            query['SandboxSpecification'] = request.sandbox_specification
-        if not UtilClient.is_unset(request.sandbox_type):
-            query['SandboxType'] = request.sandbox_type
-        if not UtilClient.is_unset(request.sandbox_user):
-            query['SandboxUser'] = request.sandbox_user
-        if not UtilClient.is_unset(request.vpc_id):
-            query['VpcId'] = request.vpc_id
-        if not UtilClient.is_unset(request.vpc_switch_id):
-            query['VpcSwitchId'] = request.vpc_switch_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.zone_id):
             query['ZoneId'] = request.zone_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='CreateSandboxInstance',
+            action='DeleteSandboxInstance',
             version='2021-01-01',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
             req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            dbs_20210101_models.CreateSandboxInstanceResponse(),
+            dbs_20210101_models.DeleteSandboxInstanceResponse(),
             self.call_api(params, req, runtime)
         )
 
-    async def create_sandbox_instance_with_options_async(
+    async def delete_sandbox_instance_with_options_async(
         self,
-        request: dbs_20210101_models.CreateSandboxInstanceRequest,
+        request: dbs_20210101_models.DeleteSandboxInstanceRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> dbs_20210101_models.CreateSandboxInstanceResponse:
+    ) -> dbs_20210101_models.DeleteSandboxInstanceResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
-        @param request: CreateSandboxInstanceRequest
+        @param request: DeleteSandboxInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
-        @return: CreateSandboxInstanceResponse
+        @return: DeleteSandboxInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_plan_id):
             query['BackupPlanId'] = request.backup_plan_id
-        if not UtilClient.is_unset(request.backup_set_id):
-            query['BackupSetId'] = request.backup_set_id
-        if not UtilClient.is_unset(request.restore_time):
-            query['RestoreTime'] = request.restore_time
-        if not UtilClient.is_unset(request.sandbox_instance_name):
-            query['SandboxInstanceName'] = request.sandbox_instance_name
-        if not UtilClient.is_unset(request.sandbox_password):
-            query['SandboxPassword'] = request.sandbox_password
-        if not UtilClient.is_unset(request.sandbox_specification):
-            query['SandboxSpecification'] = request.sandbox_specification
-        if not UtilClient.is_unset(request.sandbox_type):
-            query['SandboxType'] = request.sandbox_type
-        if not UtilClient.is_unset(request.sandbox_user):
-            query['SandboxUser'] = request.sandbox_user
-        if not UtilClient.is_unset(request.vpc_id):
-            query['VpcId'] = request.vpc_id
-        if not UtilClient.is_unset(request.vpc_switch_id):
-            query['VpcSwitchId'] = request.vpc_switch_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.zone_id):
             query['ZoneId'] = request.zone_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='CreateSandboxInstance',
+            action='DeleteSandboxInstance',
             version='2021-01-01',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
             req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            dbs_20210101_models.CreateSandboxInstanceResponse(),
+            dbs_20210101_models.DeleteSandboxInstanceResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def create_sandbox_instance(
-        self,
-        request: dbs_20210101_models.CreateSandboxInstanceRequest,
-    ) -> dbs_20210101_models.CreateSandboxInstanceResponse:
-        """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
-        
-        @param request: CreateSandboxInstanceRequest
-        @return: CreateSandboxInstanceResponse
-        """
-        runtime = util_models.RuntimeOptions()
-        return self.create_sandbox_instance_with_options(request, runtime)
-
-    async def create_sandbox_instance_async(
+    def delete_sandbox_instance(
         self,
-        request: dbs_20210101_models.CreateSandboxInstanceRequest,
-    ) -> dbs_20210101_models.CreateSandboxInstanceResponse:
+        request: dbs_20210101_models.DeleteSandboxInstanceRequest,
+    ) -> dbs_20210101_models.DeleteSandboxInstanceResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
-        @param request: CreateSandboxInstanceRequest
-        @return: CreateSandboxInstanceResponse
+        @param request: DeleteSandboxInstanceRequest
+        @return: DeleteSandboxInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
-        return await self.create_sandbox_instance_with_options_async(request, runtime)
+        return self.delete_sandbox_instance_with_options(request, runtime)
 
-    def delete_sandbox_instance_with_options(
+    async def delete_sandbox_instance_async(
         self,
         request: dbs_20210101_models.DeleteSandboxInstanceRequest,
-        runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DeleteSandboxInstanceResponse:
         """
         This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DeleteSandboxInstanceRequest
-        @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteSandboxInstanceResponse
         """
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_sandbox_instance_with_options_async(request, runtime)
+
+    def describe_backup_data_list_with_options(
+        self,
+        request: dbs_20210101_models.DescribeBackupDataListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dbs_20210101_models.DescribeBackupDataListResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.backup_plan_id):
-            query['BackupPlanId'] = request.backup_plan_id
-        if not UtilClient.is_unset(request.instance_id):
-            query['InstanceId'] = request.instance_id
-        if not UtilClient.is_unset(request.zone_id):
-            query['ZoneId'] = request.zone_id
+        if not UtilClient.is_unset(request.backup_id):
+            query['BackupId'] = request.backup_id
+        if not UtilClient.is_unset(request.backup_method):
+            query['BackupMethod'] = request.backup_method
+        if not UtilClient.is_unset(request.backup_mode):
+            query['BackupMode'] = request.backup_mode
+        if not UtilClient.is_unset(request.backup_scale):
+            query['BackupScale'] = request.backup_scale
+        if not UtilClient.is_unset(request.backup_status):
+            query['BackupStatus'] = request.backup_status
+        if not UtilClient.is_unset(request.backup_type):
+            query['BackupType'] = request.backup_type
+        if not UtilClient.is_unset(request.data_source_id):
+            query['DataSourceId'] = request.data_source_id
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_is_deleted):
+            query['InstanceIsDeleted'] = request.instance_is_deleted
+        if not UtilClient.is_unset(request.instance_name):
+            query['InstanceName'] = request.instance_name
+        if not UtilClient.is_unset(request.instance_region):
+            query['InstanceRegion'] = request.instance_region
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_code):
+            query['RegionCode'] = request.region_code
+        if not UtilClient.is_unset(request.scene_type):
+            query['SceneType'] = request.scene_type
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='DeleteSandboxInstance',
+            action='DescribeBackupDataList',
             version='2021-01-01',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
             req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            dbs_20210101_models.DeleteSandboxInstanceResponse(),
+            dbs_20210101_models.DescribeBackupDataListResponse(),
             self.call_api(params, req, runtime)
         )
 
-    async def delete_sandbox_instance_with_options_async(
+    async def describe_backup_data_list_with_options_async(
         self,
-        request: dbs_20210101_models.DeleteSandboxInstanceRequest,
+        request: dbs_20210101_models.DescribeBackupDataListRequest,
         runtime: util_models.RuntimeOptions,
-    ) -> dbs_20210101_models.DeleteSandboxInstanceResponse:
-        """
-        This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
-        
-        @param request: DeleteSandboxInstanceRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: DeleteSandboxInstanceResponse
-        """
+    ) -> dbs_20210101_models.DescribeBackupDataListResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.backup_plan_id):
-            query['BackupPlanId'] = request.backup_plan_id
-        if not UtilClient.is_unset(request.instance_id):
-            query['InstanceId'] = request.instance_id
-        if not UtilClient.is_unset(request.zone_id):
-            query['ZoneId'] = request.zone_id
+        if not UtilClient.is_unset(request.backup_id):
+            query['BackupId'] = request.backup_id
+        if not UtilClient.is_unset(request.backup_method):
+            query['BackupMethod'] = request.backup_method
+        if not UtilClient.is_unset(request.backup_mode):
+            query['BackupMode'] = request.backup_mode
+        if not UtilClient.is_unset(request.backup_scale):
+            query['BackupScale'] = request.backup_scale
+        if not UtilClient.is_unset(request.backup_status):
+            query['BackupStatus'] = request.backup_status
+        if not UtilClient.is_unset(request.backup_type):
+            query['BackupType'] = request.backup_type
+        if not UtilClient.is_unset(request.data_source_id):
+            query['DataSourceId'] = request.data_source_id
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_is_deleted):
+            query['InstanceIsDeleted'] = request.instance_is_deleted
+        if not UtilClient.is_unset(request.instance_name):
+            query['InstanceName'] = request.instance_name
+        if not UtilClient.is_unset(request.instance_region):
+            query['InstanceRegion'] = request.instance_region
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_code):
+            query['RegionCode'] = request.region_code
+        if not UtilClient.is_unset(request.scene_type):
+            query['SceneType'] = request.scene_type
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='DeleteSandboxInstance',
+            action='DescribeBackupDataList',
             version='2021-01-01',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
             req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
-            dbs_20210101_models.DeleteSandboxInstanceResponse(),
+            dbs_20210101_models.DescribeBackupDataListResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def delete_sandbox_instance(
+    def describe_backup_data_list(
         self,
-        request: dbs_20210101_models.DeleteSandboxInstanceRequest,
-    ) -> dbs_20210101_models.DeleteSandboxInstanceResponse:
-        """
-        This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
-        
-        @param request: DeleteSandboxInstanceRequest
-        @return: DeleteSandboxInstanceResponse
-        """
+        request: dbs_20210101_models.DescribeBackupDataListRequest,
+    ) -> dbs_20210101_models.DescribeBackupDataListResponse:
         runtime = util_models.RuntimeOptions()
-        return self.delete_sandbox_instance_with_options(request, runtime)
+        return self.describe_backup_data_list_with_options(request, runtime)
 
-    async def delete_sandbox_instance_async(
+    async def describe_backup_data_list_async(
         self,
-        request: dbs_20210101_models.DeleteSandboxInstanceRequest,
-    ) -> dbs_20210101_models.DeleteSandboxInstanceResponse:
-        """
-        This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
-        
-        @param request: DeleteSandboxInstanceRequest
-        @return: DeleteSandboxInstanceResponse
-        """
+        request: dbs_20210101_models.DescribeBackupDataListRequest,
+    ) -> dbs_20210101_models.DescribeBackupDataListResponse:
         runtime = util_models.RuntimeOptions()
-        return await self.delete_sandbox_instance_with_options_async(request, runtime)
+        return await self.describe_backup_data_list_with_options_async(request, runtime)
+
+    def describe_backup_policy_with_options(
+        self,
+        request: dbs_20210101_models.DescribeBackupPolicyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dbs_20210101_models.DescribeBackupPolicyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_name):
+            query['InstanceName'] = request.instance_name
+        if not UtilClient.is_unset(request.region_code):
+            query['RegionCode'] = request.region_code
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeBackupPolicy',
+            version='2021-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dbs_20210101_models.DescribeBackupPolicyResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_backup_policy_with_options_async(
+        self,
+        request: dbs_20210101_models.DescribeBackupPolicyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dbs_20210101_models.DescribeBackupPolicyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_name):
+            query['InstanceName'] = request.instance_name
+        if not UtilClient.is_unset(request.region_code):
+            query['RegionCode'] = request.region_code
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeBackupPolicy',
+            version='2021-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dbs_20210101_models.DescribeBackupPolicyResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_backup_policy(
+        self,
+        request: dbs_20210101_models.DescribeBackupPolicyRequest,
+    ) -> dbs_20210101_models.DescribeBackupPolicyResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_backup_policy_with_options(request, runtime)
+
+    async def describe_backup_policy_async(
+        self,
+        request: dbs_20210101_models.DescribeBackupPolicyRequest,
+    ) -> dbs_20210101_models.DescribeBackupPolicyResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_backup_policy_with_options_async(request, runtime)
 
     def describe_dbtables_recovery_backup_set_with_options(
         self,
         request: dbs_20210101_models.DescribeDBTablesRecoveryBackupSetRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryBackupSetResponse:
         UtilClient.validate_model(request)
@@ -748,15 +852,22 @@
 
     def describe_download_backup_set_storage_info_with_options(
         self,
         request: dbs_20210101_models.DescribeDownloadBackupSetStorageInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadBackupSetStorageInfoResponse:
         """
-        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: DescribeDownloadBackupSetStorageInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadBackupSetStorageInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -791,15 +902,22 @@
 
     async def describe_download_backup_set_storage_info_with_options_async(
         self,
         request: dbs_20210101_models.DescribeDownloadBackupSetStorageInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadBackupSetStorageInfoResponse:
         """
-        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: DescribeDownloadBackupSetStorageInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadBackupSetStorageInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -833,42 +951,64 @@
         )
 
     def describe_download_backup_set_storage_info(
         self,
         request: dbs_20210101_models.DescribeDownloadBackupSetStorageInfoRequest,
     ) -> dbs_20210101_models.DescribeDownloadBackupSetStorageInfoResponse:
         """
-        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: DescribeDownloadBackupSetStorageInfoRequest
         @return: DescribeDownloadBackupSetStorageInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_download_backup_set_storage_info_with_options(request, runtime)
 
     async def describe_download_backup_set_storage_info_async(
         self,
         request: dbs_20210101_models.DescribeDownloadBackupSetStorageInfoRequest,
     ) -> dbs_20210101_models.DescribeDownloadBackupSetStorageInfoResponse:
         """
-        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: DescribeDownloadBackupSetStorageInfoRequest
         @return: DescribeDownloadBackupSetStorageInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_download_backup_set_storage_info_with_options_async(request, runtime)
 
     def describe_download_support_with_options(
         self,
         request: dbs_20210101_models.DescribeDownloadSupportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadSupportResponse:
         """
-        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        You can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: DescribeDownloadSupportRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadSupportResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -897,15 +1037,23 @@
 
     async def describe_download_support_with_options_async(
         self,
         request: dbs_20210101_models.DescribeDownloadSupportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadSupportResponse:
         """
-        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        You can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: DescribeDownloadSupportRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadSupportResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -933,42 +1081,65 @@
         )
 
     def describe_download_support(
         self,
         request: dbs_20210101_models.DescribeDownloadSupportRequest,
     ) -> dbs_20210101_models.DescribeDownloadSupportResponse:
         """
-        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        You can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: DescribeDownloadSupportRequest
         @return: DescribeDownloadSupportResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_download_support_with_options(request, runtime)
 
     async def describe_download_support_async(
         self,
         request: dbs_20210101_models.DescribeDownloadSupportRequest,
     ) -> dbs_20210101_models.DescribeDownloadSupportResponse:
         """
-        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        You can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: DescribeDownloadSupportRequest
         @return: DescribeDownloadSupportResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_download_support_with_options_async(request, runtime)
 
     def describe_download_task_with_options(
         self,
         request: dbs_20210101_models.DescribeDownloadTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadTaskResponse:
         """
-        You can create an advanced download task by point in time or backup set. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: DescribeDownloadTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1017,15 +1188,22 @@
 
     async def describe_download_task_with_options_async(
         self,
         request: dbs_20210101_models.DescribeDownloadTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadTaskResponse:
         """
-        You can create an advanced download task by point in time or backup set. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: DescribeDownloadTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1073,28 +1251,42 @@
         )
 
     def describe_download_task(
         self,
         request: dbs_20210101_models.DescribeDownloadTaskRequest,
     ) -> dbs_20210101_models.DescribeDownloadTaskResponse:
         """
-        You can create an advanced download task by point in time or backup set. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: DescribeDownloadTaskRequest
         @return: DescribeDownloadTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_download_task_with_options(request, runtime)
 
     async def describe_download_task_async(
         self,
         request: dbs_20210101_models.DescribeDownloadTaskRequest,
     ) -> dbs_20210101_models.DescribeDownloadTaskResponse:
         """
-        You can create an advanced download task by point in time or backup set. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
+        ### [](#)Supported database engines
+        *   ApsaraDB RDS for MySQL
+        *   ApsaraDB RDS for PostgreSQL
+        *   PolarDB for MySQL
+        ### [](#)References
+        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
+        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
+        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
         
         @param request: DescribeDownloadTaskRequest
         @return: DescribeDownloadTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_download_task_with_options_async(request, runtime)
```

### Comparing `alibabacloud_dbs20210101-1.0.4/alibabacloud_dbs20210101/models.py` & `alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,21 +5,24 @@
 
 
 class ChangeResourceGroupRequest(TeaModel):
     def __init__(
         self,
         client_token: str = None,
         new_resource_group_id: str = None,
+        region_code: str = None,
         resource_id: str = None,
         resource_type: str = None,
     ):
         # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token
         # The ID of the resource group to which you want to move the resource.
         self.new_resource_group_id = new_resource_group_id
+        # The region ID of the instance.
+        self.region_code = region_code
         # The ID of the resource.
         self.resource_id = resource_id
         # The type of the resource. Set the value to backupplan.
         self.resource_type = resource_type
 
     def validate(self):
         pass
@@ -30,26 +33,30 @@
             return _map
 
         result = dict()
         if self.client_token is not None:
             result['ClientToken'] = self.client_token
         if self.new_resource_group_id is not None:
             result['NewResourceGroupId'] = self.new_resource_group_id
+        if self.region_code is not None:
+            result['RegionCode'] = self.region_code
         if self.resource_id is not None:
             result['ResourceId'] = self.resource_id
         if self.resource_type is not None:
             result['ResourceType'] = self.resource_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ClientToken') is not None:
             self.client_token = m.get('ClientToken')
         if m.get('NewResourceGroupId') is not None:
             self.new_resource_group_id = m.get('NewResourceGroupId')
+        if m.get('RegionCode') is not None:
+            self.region_code = m.get('RegionCode')
         if m.get('ResourceId') is not None:
             self.resource_id = m.get('ResourceId')
         if m.get('ResourceType') is not None:
             self.resource_type = m.get('ResourceType')
         return self
 
 
@@ -137,17 +144,14 @@
         body: ChangeResourceGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -340,15 +344,15 @@
         # 
         # > If the task is in the preparation stage, 0/0 is returned.
         self.progress = progress
         # The ID of the region in which the instance resides.
         self.region_code = region_code
         # The destination path to which the backup set is downloaded.
         # 
-        # > This parameter is returned if the TargetType parameter is set to OSS.
+        # >  This parameter is returned if the value of **TargetType is OSS**.
         self.target_path = target_path
         # The type of the destination to which the backup set is downloaded.
         self.target_type = target_type
         # The ID of the download task.
         self.task_id = task_id
 
     def validate(self):
@@ -428,15 +432,15 @@
         err_message: str = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
         # The status code returned.
         self.code = code
-        # The returned data.
+        # The information about the download task.
         self.data = data
         # The error code returned if the request failed.
         self.err_code = err_code
         # The error message returned if the request failed.
         self.err_message = err_message
         # The error message returned if the request failed.
         self.message = message
@@ -502,17 +506,14 @@
         body: CreateDownloadResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -534,193 +535,579 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateDownloadResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class CreateSandboxInstanceRequest(TeaModel):
+class DeleteSandboxInstanceRequest(TeaModel):
     def __init__(
         self,
         backup_plan_id: str = None,
-        backup_set_id: str = None,
-        restore_time: str = None,
-        sandbox_instance_name: str = None,
-        sandbox_password: str = None,
-        sandbox_specification: str = None,
-        sandbox_type: str = None,
-        sandbox_user: str = None,
-        vpc_id: str = None,
-        vpc_switch_id: str = None,
+        instance_id: str = None,
         zone_id: str = None,
     ):
-        # The ID of the backup schedule. You can call the [DescribeBackupPlanList](~~437215~~) operation to obtain the ID of the backup schedule.
+        # The ID of the backup schedule. You can call the [DescribeBackupPlanList](~~437215~~) operation to query the ID of the backup schedule.
         # 
         # > If your instance is an ApsaraDB RDS for MySQL instance, you can [configure automatic access to a data source](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
         self.backup_plan_id = backup_plan_id
-        # The ID of the backup set to be restored, which is the point in time when a snapshot was created. You can call the [DescribeSandboxBackupSets](~~437256~~) operation to obtain the ID.
-        # 
-        # > You need to specify only one of the **BackupSetId** and **RestoreTime** parameters.
-        self.backup_set_id = backup_set_id
-        # The point in time of the sandbox instance to be restored. You can call the [DescribeSandboxRecoveryTime](~~437258~~) operation to view the recoverable time range. Specify the time in the format of *yyyy-MM-ddTHH:mm:ssZ*. The time must be in UTC.
-        self.restore_time = restore_time
-        # The custom name of the sandbox instance.
-        self.sandbox_instance_name = sandbox_instance_name
-        # The password of the privileged account created in the sandbox instance.
-        self.sandbox_password = sandbox_password
-        # The specifications of the sandbox instance. Valid values:
-        # 
-        # *   **MYSQL\_1C\_1M_SD**: 1 CPU core and 1 GB of memory.
-        # *   **MYSQL\_1C\_2M_SD**: 1 CPU core and 2 GB of memory.
-        # *   **MYSQL\_2C\_4M_SD**: 2 CPU cores and 4 GB of memory.
-        # *   **MYSQL\_2C\_8M_SD**: 2 CPU cores and 8 GB of memory.
-        # *   **MYSQL\_4C\_8M_SD**: 4 CPU cores and 8 GB of memory.
-        # *   **MYSQL\_4C\_16M_SD**: 4 CPU cores and 16 GB of memory.
-        # *   **MYSQL\_8C\_16M_SD**: 8 CPU cores and 16 GB of memory.
-        # *   **MYSQL\_8C\_32M_SD**: 8 CPU cores and 32 GB of memory.
-        # 
-        # > Different specifications have little impact on the recovery speed. High-specification instances provide better performance after restoration. For more information, see [DBS sandbox fees](~~201466~~).
-        self.sandbox_specification = sandbox_specification
-        # The type of the sandbox instance. You can call this operation only to create an instance of the **Sandbox** type. After the sandbox instance is created, the MySQL endpoint of the instance is provided.
-        self.sandbox_type = sandbox_type
-        # The privileged account created in the sandbox instance.
-        # 
-        # *   After you specify this parameter, the system creates a privileged account in the sandbox instance. The account is granted the permissions on all databases in the instance.
-        # 
-        # The account of the source database is retained in the sandbox instance.
-        # 
-        # *   If you do not specify this parameter, the database account is the same as that of the source database.
-        self.sandbox_user = sandbox_user
-        # The ID of the virtual private cloud (VPC) that is used to connect to the sandbox instance. If you want to connect to the sandbox instance by using Elastic Compute Service (ECS) instances, you must set this parameter to the VPC in which the ECS instances reside.
-        # 
-        # > You can set this parameter if you want to use it in a recovery drill scenario.
-        self.vpc_id = vpc_id
-        # The ID of the VSwitch that is used to connect to the sandbox instance.
-        self.vpc_switch_id = vpc_switch_id
+        # The ID of the sandbox instance. You can call the [DescribeSandboxInstances](~~437257~~) operation to query the ID of the sandbox instance.
+        self.instance_id = instance_id
         self.zone_id = zone_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.backup_plan_id is not None:
             result['BackupPlanId'] = self.backup_plan_id
-        if self.backup_set_id is not None:
-            result['BackupSetId'] = self.backup_set_id
-        if self.restore_time is not None:
-            result['RestoreTime'] = self.restore_time
-        if self.sandbox_instance_name is not None:
-            result['SandboxInstanceName'] = self.sandbox_instance_name
-        if self.sandbox_password is not None:
-            result['SandboxPassword'] = self.sandbox_password
-        if self.sandbox_specification is not None:
-            result['SandboxSpecification'] = self.sandbox_specification
-        if self.sandbox_type is not None:
-            result['SandboxType'] = self.sandbox_type
-        if self.sandbox_user is not None:
-            result['SandboxUser'] = self.sandbox_user
-        if self.vpc_id is not None:
-            result['VpcId'] = self.vpc_id
-        if self.vpc_switch_id is not None:
-            result['VpcSwitchId'] = self.vpc_switch_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
         if self.zone_id is not None:
             result['ZoneId'] = self.zone_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('BackupPlanId') is not None:
             self.backup_plan_id = m.get('BackupPlanId')
-        if m.get('BackupSetId') is not None:
-            self.backup_set_id = m.get('BackupSetId')
-        if m.get('RestoreTime') is not None:
-            self.restore_time = m.get('RestoreTime')
-        if m.get('SandboxInstanceName') is not None:
-            self.sandbox_instance_name = m.get('SandboxInstanceName')
-        if m.get('SandboxPassword') is not None:
-            self.sandbox_password = m.get('SandboxPassword')
-        if m.get('SandboxSpecification') is not None:
-            self.sandbox_specification = m.get('SandboxSpecification')
-        if m.get('SandboxType') is not None:
-            self.sandbox_type = m.get('SandboxType')
-        if m.get('SandboxUser') is not None:
-            self.sandbox_user = m.get('SandboxUser')
-        if m.get('VpcId') is not None:
-            self.vpc_id = m.get('VpcId')
-        if m.get('VpcSwitchId') is not None:
-            self.vpc_switch_id = m.get('VpcSwitchId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
         if m.get('ZoneId') is not None:
             self.zone_id = m.get('ZoneId')
         return self
 
 
-class CreateSandboxInstanceResponseBodyData(TeaModel):
+class DeleteSandboxInstanceResponseBody(TeaModel):
     def __init__(
         self,
-        backup_plan_id: str = None,
-        instance_id: str = None,
+        code: str = None,
+        data: str = None,
+        err_code: str = None,
+        err_message: str = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
     ):
-        # The ID of the backup plan.
-        self.backup_plan_id = backup_plan_id
-        # The ID of the sandbox instance.
-        self.instance_id = instance_id
+        # The error code returned if the request failed.
+        self.code = code
+        # The returned data.
+        self.data = data
+        # The error code returned if the request failed.
+        self.err_code = err_code
+        # The error message returned if the request failed.
+        self.err_message = err_message
+        # The error message returned if the request failed.
+        self.message = message
+        # The ID of the request.
+        self.request_id = request_id
+        # Indicates whether the request was successful.
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.backup_plan_id is not None:
-            result['BackupPlanId'] = self.backup_plan_id
-        if self.instance_id is not None:
-            result['InstanceId'] = self.instance_id
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.err_code is not None:
+            result['ErrCode'] = self.err_code
+        if self.err_message is not None:
+            result['ErrMessage'] = self.err_message
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('BackupPlanId') is not None:
-            self.backup_plan_id = m.get('BackupPlanId')
-        if m.get('InstanceId') is not None:
-            self.instance_id = m.get('InstanceId')
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('ErrCode') is not None:
+            self.err_code = m.get('ErrCode')
+        if m.get('ErrMessage') is not None:
+            self.err_message = m.get('ErrMessage')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class DeleteSandboxInstanceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteSandboxInstanceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteSandboxInstanceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeBackupDataListRequest(TeaModel):
+    def __init__(
+        self,
+        backup_id: str = None,
+        backup_method: str = None,
+        backup_mode: str = None,
+        backup_scale: str = None,
+        backup_status: str = None,
+        backup_type: str = None,
+        data_source_id: str = None,
+        end_time: str = None,
+        instance_is_deleted: bool = None,
+        instance_name: str = None,
+        instance_region: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        region_code: str = None,
+        scene_type: str = None,
+        start_time: str = None,
+    ):
+        self.backup_id = backup_id
+        self.backup_method = backup_method
+        self.backup_mode = backup_mode
+        self.backup_scale = backup_scale
+        self.backup_status = backup_status
+        self.backup_type = backup_type
+        self.data_source_id = data_source_id
+        self.end_time = end_time
+        self.instance_is_deleted = instance_is_deleted
+        self.instance_name = instance_name
+        self.instance_region = instance_region
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_code = region_code
+        self.scene_type = scene_type
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.backup_id is not None:
+            result['BackupId'] = self.backup_id
+        if self.backup_method is not None:
+            result['BackupMethod'] = self.backup_method
+        if self.backup_mode is not None:
+            result['BackupMode'] = self.backup_mode
+        if self.backup_scale is not None:
+            result['BackupScale'] = self.backup_scale
+        if self.backup_status is not None:
+            result['BackupStatus'] = self.backup_status
+        if self.backup_type is not None:
+            result['BackupType'] = self.backup_type
+        if self.data_source_id is not None:
+            result['DataSourceId'] = self.data_source_id
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.instance_is_deleted is not None:
+            result['InstanceIsDeleted'] = self.instance_is_deleted
+        if self.instance_name is not None:
+            result['InstanceName'] = self.instance_name
+        if self.instance_region is not None:
+            result['InstanceRegion'] = self.instance_region
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_code is not None:
+            result['RegionCode'] = self.region_code
+        if self.scene_type is not None:
+            result['SceneType'] = self.scene_type
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BackupId') is not None:
+            self.backup_id = m.get('BackupId')
+        if m.get('BackupMethod') is not None:
+            self.backup_method = m.get('BackupMethod')
+        if m.get('BackupMode') is not None:
+            self.backup_mode = m.get('BackupMode')
+        if m.get('BackupScale') is not None:
+            self.backup_scale = m.get('BackupScale')
+        if m.get('BackupStatus') is not None:
+            self.backup_status = m.get('BackupStatus')
+        if m.get('BackupType') is not None:
+            self.backup_type = m.get('BackupType')
+        if m.get('DataSourceId') is not None:
+            self.data_source_id = m.get('DataSourceId')
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('InstanceIsDeleted') is not None:
+            self.instance_is_deleted = m.get('InstanceIsDeleted')
+        if m.get('InstanceName') is not None:
+            self.instance_name = m.get('InstanceName')
+        if m.get('InstanceRegion') is not None:
+            self.instance_region = m.get('InstanceRegion')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionCode') is not None:
+            self.region_code = m.get('RegionCode')
+        if m.get('SceneType') is not None:
+            self.scene_type = m.get('SceneType')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class DescribeBackupDataListResponseBodyDataContentPolarSnapshot(TeaModel):
+    def __init__(
+        self,
+        dump_id: int = None,
+        dump_size: int = None,
+        expect_expire_time: str = None,
+        expect_expire_type: str = None,
+    ):
+        self.dump_id = dump_id
+        self.dump_size = dump_size
+        self.expect_expire_time = expect_expire_time
+        self.expect_expire_type = expect_expire_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dump_id is not None:
+            result['DumpId'] = self.dump_id
+        if self.dump_size is not None:
+            result['DumpSize'] = self.dump_size
+        if self.expect_expire_time is not None:
+            result['ExpectExpireTime'] = self.expect_expire_time
+        if self.expect_expire_type is not None:
+            result['expectExpireType'] = self.expect_expire_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DumpId') is not None:
+            self.dump_id = m.get('DumpId')
+        if m.get('DumpSize') is not None:
+            self.dump_size = m.get('DumpSize')
+        if m.get('ExpectExpireTime') is not None:
+            self.expect_expire_time = m.get('ExpectExpireTime')
+        if m.get('expectExpireType') is not None:
+            self.expect_expire_type = m.get('expectExpireType')
+        return self
+
+
+class DescribeBackupDataListResponseBodyDataContent(TeaModel):
+    def __init__(
+        self,
+        backup_download_url: str = None,
+        backup_end_time: str = None,
+        backup_id: str = None,
+        backup_intranet_download_url: str = None,
+        backup_location: str = None,
+        backup_method: str = None,
+        backup_mode: str = None,
+        backup_name: str = None,
+        backup_scale: str = None,
+        backup_size: int = None,
+        backup_start_time: str = None,
+        backup_status: str = None,
+        backup_type: str = None,
+        checksum: str = None,
+        consistent_time: int = None,
+        encryption: str = None,
+        engine: str = None,
+        engine_version: str = None,
+        expect_expire_time: str = None,
+        expect_expire_type: str = None,
+        instance_name: str = None,
+        is_avail: int = None,
+        polar_snapshot: DescribeBackupDataListResponseBodyDataContentPolarSnapshot = None,
+        support_deletion: int = None,
+    ):
+        self.backup_download_url = backup_download_url
+        self.backup_end_time = backup_end_time
+        self.backup_id = backup_id
+        self.backup_intranet_download_url = backup_intranet_download_url
+        self.backup_location = backup_location
+        self.backup_method = backup_method
+        self.backup_mode = backup_mode
+        self.backup_name = backup_name
+        self.backup_scale = backup_scale
+        self.backup_size = backup_size
+        self.backup_start_time = backup_start_time
+        self.backup_status = backup_status
+        self.backup_type = backup_type
+        self.checksum = checksum
+        self.consistent_time = consistent_time
+        self.encryption = encryption
+        self.engine = engine
+        self.engine_version = engine_version
+        self.expect_expire_time = expect_expire_time
+        self.expect_expire_type = expect_expire_type
+        self.instance_name = instance_name
+        self.is_avail = is_avail
+        self.polar_snapshot = polar_snapshot
+        self.support_deletion = support_deletion
+
+    def validate(self):
+        if self.polar_snapshot:
+            self.polar_snapshot.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.backup_download_url is not None:
+            result['BackupDownloadURL'] = self.backup_download_url
+        if self.backup_end_time is not None:
+            result['BackupEndTime'] = self.backup_end_time
+        if self.backup_id is not None:
+            result['BackupId'] = self.backup_id
+        if self.backup_intranet_download_url is not None:
+            result['BackupIntranetDownloadURL'] = self.backup_intranet_download_url
+        if self.backup_location is not None:
+            result['BackupLocation'] = self.backup_location
+        if self.backup_method is not None:
+            result['BackupMethod'] = self.backup_method
+        if self.backup_mode is not None:
+            result['BackupMode'] = self.backup_mode
+        if self.backup_name is not None:
+            result['BackupName'] = self.backup_name
+        if self.backup_scale is not None:
+            result['BackupScale'] = self.backup_scale
+        if self.backup_size is not None:
+            result['BackupSize'] = self.backup_size
+        if self.backup_start_time is not None:
+            result['BackupStartTime'] = self.backup_start_time
+        if self.backup_status is not None:
+            result['BackupStatus'] = self.backup_status
+        if self.backup_type is not None:
+            result['BackupType'] = self.backup_type
+        if self.checksum is not None:
+            result['Checksum'] = self.checksum
+        if self.consistent_time is not None:
+            result['ConsistentTime'] = self.consistent_time
+        if self.encryption is not None:
+            result['Encryption'] = self.encryption
+        if self.engine is not None:
+            result['Engine'] = self.engine
+        if self.engine_version is not None:
+            result['EngineVersion'] = self.engine_version
+        if self.expect_expire_time is not None:
+            result['ExpectExpireTime'] = self.expect_expire_time
+        if self.expect_expire_type is not None:
+            result['ExpectExpireType'] = self.expect_expire_type
+        if self.instance_name is not None:
+            result['InstanceName'] = self.instance_name
+        if self.is_avail is not None:
+            result['IsAvail'] = self.is_avail
+        if self.polar_snapshot is not None:
+            result['PolarSnapshot'] = self.polar_snapshot.to_map()
+        if self.support_deletion is not None:
+            result['SupportDeletion'] = self.support_deletion
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BackupDownloadURL') is not None:
+            self.backup_download_url = m.get('BackupDownloadURL')
+        if m.get('BackupEndTime') is not None:
+            self.backup_end_time = m.get('BackupEndTime')
+        if m.get('BackupId') is not None:
+            self.backup_id = m.get('BackupId')
+        if m.get('BackupIntranetDownloadURL') is not None:
+            self.backup_intranet_download_url = m.get('BackupIntranetDownloadURL')
+        if m.get('BackupLocation') is not None:
+            self.backup_location = m.get('BackupLocation')
+        if m.get('BackupMethod') is not None:
+            self.backup_method = m.get('BackupMethod')
+        if m.get('BackupMode') is not None:
+            self.backup_mode = m.get('BackupMode')
+        if m.get('BackupName') is not None:
+            self.backup_name = m.get('BackupName')
+        if m.get('BackupScale') is not None:
+            self.backup_scale = m.get('BackupScale')
+        if m.get('BackupSize') is not None:
+            self.backup_size = m.get('BackupSize')
+        if m.get('BackupStartTime') is not None:
+            self.backup_start_time = m.get('BackupStartTime')
+        if m.get('BackupStatus') is not None:
+            self.backup_status = m.get('BackupStatus')
+        if m.get('BackupType') is not None:
+            self.backup_type = m.get('BackupType')
+        if m.get('Checksum') is not None:
+            self.checksum = m.get('Checksum')
+        if m.get('ConsistentTime') is not None:
+            self.consistent_time = m.get('ConsistentTime')
+        if m.get('Encryption') is not None:
+            self.encryption = m.get('Encryption')
+        if m.get('Engine') is not None:
+            self.engine = m.get('Engine')
+        if m.get('EngineVersion') is not None:
+            self.engine_version = m.get('EngineVersion')
+        if m.get('ExpectExpireTime') is not None:
+            self.expect_expire_time = m.get('ExpectExpireTime')
+        if m.get('ExpectExpireType') is not None:
+            self.expect_expire_type = m.get('ExpectExpireType')
+        if m.get('InstanceName') is not None:
+            self.instance_name = m.get('InstanceName')
+        if m.get('IsAvail') is not None:
+            self.is_avail = m.get('IsAvail')
+        if m.get('PolarSnapshot') is not None:
+            temp_model = DescribeBackupDataListResponseBodyDataContentPolarSnapshot()
+            self.polar_snapshot = temp_model.from_map(m['PolarSnapshot'])
+        if m.get('SupportDeletion') is not None:
+            self.support_deletion = m.get('SupportDeletion')
+        return self
+
+
+class DescribeBackupDataListResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        content: List[DescribeBackupDataListResponseBodyDataContent] = None,
+        extra: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        total_elements: int = None,
+        total_pages: int = None,
+    ):
+        self.content = content
+        self.extra = extra
+        self.page_number = page_number
+        self.page_size = page_size
+        self.total_elements = total_elements
+        self.total_pages = total_pages
+
+    def validate(self):
+        if self.content:
+            for k in self.content:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Content'] = []
+        if self.content is not None:
+            for k in self.content:
+                result['Content'].append(k.to_map() if k else None)
+        if self.extra is not None:
+            result['Extra'] = self.extra
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total_elements is not None:
+            result['TotalElements'] = self.total_elements
+        if self.total_pages is not None:
+            result['TotalPages'] = self.total_pages
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.content = []
+        if m.get('Content') is not None:
+            for k in m.get('Content'):
+                temp_model = DescribeBackupDataListResponseBodyDataContent()
+                self.content.append(temp_model.from_map(k))
+        if m.get('Extra') is not None:
+            self.extra = m.get('Extra')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('TotalElements') is not None:
+            self.total_elements = m.get('TotalElements')
+        if m.get('TotalPages') is not None:
+            self.total_pages = m.get('TotalPages')
         return self
 
 
-class CreateSandboxInstanceResponseBody(TeaModel):
+class DescribeBackupDataListResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
-        data: CreateSandboxInstanceResponseBodyData = None,
+        data: DescribeBackupDataListResponseBodyData = None,
         err_code: str = None,
         err_message: str = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
-        # The error code returned if the request fails.
         self.code = code
-        # The response parameters.
         self.data = data
-        # The error code returned if the request fails.
         self.err_code = err_code
-        # The error message returned if the request fails.
         self.err_message = err_message
-        # The error message returned if the request fails.
         self.message = message
-        # The ID of the request.
         self.request_id = request_id
-        # Indicates whether the request was successful.
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -746,44 +1133,41 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('Data') is not None:
-            temp_model = CreateSandboxInstanceResponseBodyData()
+            temp_model = DescribeBackupDataListResponseBodyData()
             self.data = temp_model.from_map(m['Data'])
         if m.get('ErrCode') is not None:
             self.err_code = m.get('ErrCode')
         if m.get('ErrMessage') is not None:
             self.err_message = m.get('ErrMessage')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
-class CreateSandboxInstanceResponse(TeaModel):
+class DescribeBackupDataListResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: CreateSandboxInstanceResponseBody = None,
+        body: DescribeBackupDataListResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -800,101 +1184,405 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = CreateSandboxInstanceResponseBody()
+            temp_model = DescribeBackupDataListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DeleteSandboxInstanceRequest(TeaModel):
+class DescribeBackupPolicyRequest(TeaModel):
     def __init__(
         self,
-        backup_plan_id: str = None,
-        instance_id: str = None,
-        zone_id: str = None,
+        instance_name: str = None,
+        region_code: str = None,
     ):
-        # The ID of the backup schedule. You can call the [DescribeBackupPlanList](~~437215~~) operation to query the ID of the backup schedule.
-        # 
-        # > If your instance is an ApsaraDB RDS for MySQL instance, you can [configure automatic access to a data source](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
-        self.backup_plan_id = backup_plan_id
-        # The ID of the sandbox instance. You can call the [DescribeSandboxInstances](~~437257~~) operation to query the ID of the sandbox instance.
-        self.instance_id = instance_id
-        self.zone_id = zone_id
+        self.instance_name = instance_name
+        self.region_code = region_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.backup_plan_id is not None:
-            result['BackupPlanId'] = self.backup_plan_id
-        if self.instance_id is not None:
-            result['InstanceId'] = self.instance_id
-        if self.zone_id is not None:
-            result['ZoneId'] = self.zone_id
+        if self.instance_name is not None:
+            result['InstanceName'] = self.instance_name
+        if self.region_code is not None:
+            result['RegionCode'] = self.region_code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('BackupPlanId') is not None:
-            self.backup_plan_id = m.get('BackupPlanId')
-        if m.get('InstanceId') is not None:
-            self.instance_id = m.get('InstanceId')
-        if m.get('ZoneId') is not None:
-            self.zone_id = m.get('ZoneId')
+        if m.get('InstanceName') is not None:
+            self.instance_name = m.get('InstanceName')
+        if m.get('RegionCode') is not None:
+            self.region_code = m.get('RegionCode')
         return self
 
 
-class DeleteSandboxInstanceResponseBody(TeaModel):
+class DescribeBackupPolicyResponseBodyDataAdvanceDataPolicies(TeaModel):
+    def __init__(
+        self,
+        auto_created: bool = None,
+        bak_type: str = None,
+        dest_region: str = None,
+        dest_type: str = None,
+        dump_action: str = None,
+        filter_key: str = None,
+        filter_type: str = None,
+        filter_value: str = None,
+        retention_type: str = None,
+        retention_value: str = None,
+        src_region: str = None,
+        src_type: str = None,
+        strategy_id: str = None,
+    ):
+        self.auto_created = auto_created
+        self.bak_type = bak_type
+        self.dest_region = dest_region
+        self.dest_type = dest_type
+        self.dump_action = dump_action
+        self.filter_key = filter_key
+        self.filter_type = filter_type
+        self.filter_value = filter_value
+        self.retention_type = retention_type
+        self.retention_value = retention_value
+        self.src_region = src_region
+        self.src_type = src_type
+        self.strategy_id = strategy_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auto_created is not None:
+            result['AutoCreated'] = self.auto_created
+        if self.bak_type is not None:
+            result['BakType'] = self.bak_type
+        if self.dest_region is not None:
+            result['DestRegion'] = self.dest_region
+        if self.dest_type is not None:
+            result['DestType'] = self.dest_type
+        if self.dump_action is not None:
+            result['DumpAction'] = self.dump_action
+        if self.filter_key is not None:
+            result['FilterKey'] = self.filter_key
+        if self.filter_type is not None:
+            result['FilterType'] = self.filter_type
+        if self.filter_value is not None:
+            result['FilterValue'] = self.filter_value
+        if self.retention_type is not None:
+            result['RetentionType'] = self.retention_type
+        if self.retention_value is not None:
+            result['RetentionValue'] = self.retention_value
+        if self.src_region is not None:
+            result['SrcRegion'] = self.src_region
+        if self.src_type is not None:
+            result['SrcType'] = self.src_type
+        if self.strategy_id is not None:
+            result['StrategyId'] = self.strategy_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AutoCreated') is not None:
+            self.auto_created = m.get('AutoCreated')
+        if m.get('BakType') is not None:
+            self.bak_type = m.get('BakType')
+        if m.get('DestRegion') is not None:
+            self.dest_region = m.get('DestRegion')
+        if m.get('DestType') is not None:
+            self.dest_type = m.get('DestType')
+        if m.get('DumpAction') is not None:
+            self.dump_action = m.get('DumpAction')
+        if m.get('FilterKey') is not None:
+            self.filter_key = m.get('FilterKey')
+        if m.get('FilterType') is not None:
+            self.filter_type = m.get('FilterType')
+        if m.get('FilterValue') is not None:
+            self.filter_value = m.get('FilterValue')
+        if m.get('RetentionType') is not None:
+            self.retention_type = m.get('RetentionType')
+        if m.get('RetentionValue') is not None:
+            self.retention_value = m.get('RetentionValue')
+        if m.get('SrcRegion') is not None:
+            self.src_region = m.get('SrcRegion')
+        if m.get('SrcType') is not None:
+            self.src_type = m.get('SrcType')
+        if m.get('StrategyId') is not None:
+            self.strategy_id = m.get('StrategyId')
+        return self
+
+
+class DescribeBackupPolicyResponseBodyDataAdvanceLogPolicies(TeaModel):
+    def __init__(
+        self,
+        dest_region: str = None,
+        dest_type: str = None,
+        enable_log_backup: bool = None,
+        log_retention_type: str = None,
+        log_retention_value: str = None,
+        src_region: str = None,
+        src_type: str = None,
+        strategy_id: str = None,
+    ):
+        self.dest_region = dest_region
+        self.dest_type = dest_type
+        self.enable_log_backup = enable_log_backup
+        self.log_retention_type = log_retention_type
+        self.log_retention_value = log_retention_value
+        self.src_region = src_region
+        self.src_type = src_type
+        self.strategy_id = strategy_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dest_region is not None:
+            result['DestRegion'] = self.dest_region
+        if self.dest_type is not None:
+            result['DestType'] = self.dest_type
+        if self.enable_log_backup is not None:
+            result['EnableLogBackup'] = self.enable_log_backup
+        if self.log_retention_type is not None:
+            result['LogRetentionType'] = self.log_retention_type
+        if self.log_retention_value is not None:
+            result['LogRetentionValue'] = self.log_retention_value
+        if self.src_region is not None:
+            result['SrcRegion'] = self.src_region
+        if self.src_type is not None:
+            result['SrcType'] = self.src_type
+        if self.strategy_id is not None:
+            result['StrategyId'] = self.strategy_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DestRegion') is not None:
+            self.dest_region = m.get('DestRegion')
+        if m.get('DestType') is not None:
+            self.dest_type = m.get('DestType')
+        if m.get('EnableLogBackup') is not None:
+            self.enable_log_backup = m.get('EnableLogBackup')
+        if m.get('LogRetentionType') is not None:
+            self.log_retention_type = m.get('LogRetentionType')
+        if m.get('LogRetentionValue') is not None:
+            self.log_retention_value = m.get('LogRetentionValue')
+        if m.get('SrcRegion') is not None:
+            self.src_region = m.get('SrcRegion')
+        if m.get('SrcType') is not None:
+            self.src_type = m.get('SrcType')
+        if m.get('StrategyId') is not None:
+            self.strategy_id = m.get('StrategyId')
+        return self
+
+
+class DescribeBackupPolicyResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        advance_data_policies: List[DescribeBackupPolicyResponseBodyDataAdvanceDataPolicies] = None,
+        advance_log_policies: List[DescribeBackupPolicyResponseBodyDataAdvanceLogPolicies] = None,
+        backup_method: str = None,
+        backup_priority: int = None,
+        backup_retention_period: int = None,
+        backup_retention_policy_on_cluster_deletion: str = None,
+        category: str = None,
+        enable_backup: int = None,
+        enable_inc_backup: int = None,
+        enable_log_backup: int = None,
+        high_frequency_bak_interval: int = None,
+        high_space_usage_protection: str = None,
+        inc_backup_interval: int = None,
+        local_log_retention_space: int = None,
+        log_backup_local_retention_number: str = None,
+        log_backup_retention: int = None,
+        preferred_backup_date: str = None,
+        preferred_backup_window: str = None,
+        preferred_backup_window_begin: str = None,
+    ):
+        self.advance_data_policies = advance_data_policies
+        self.advance_log_policies = advance_log_policies
+        self.backup_method = backup_method
+        self.backup_priority = backup_priority
+        self.backup_retention_period = backup_retention_period
+        self.backup_retention_policy_on_cluster_deletion = backup_retention_policy_on_cluster_deletion
+        self.category = category
+        self.enable_backup = enable_backup
+        self.enable_inc_backup = enable_inc_backup
+        self.enable_log_backup = enable_log_backup
+        self.high_frequency_bak_interval = high_frequency_bak_interval
+        self.high_space_usage_protection = high_space_usage_protection
+        self.inc_backup_interval = inc_backup_interval
+        self.local_log_retention_space = local_log_retention_space
+        self.log_backup_local_retention_number = log_backup_local_retention_number
+        self.log_backup_retention = log_backup_retention
+        self.preferred_backup_date = preferred_backup_date
+        self.preferred_backup_window = preferred_backup_window
+        self.preferred_backup_window_begin = preferred_backup_window_begin
+
+    def validate(self):
+        if self.advance_data_policies:
+            for k in self.advance_data_policies:
+                if k:
+                    k.validate()
+        if self.advance_log_policies:
+            for k in self.advance_log_policies:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['AdvanceDataPolicies'] = []
+        if self.advance_data_policies is not None:
+            for k in self.advance_data_policies:
+                result['AdvanceDataPolicies'].append(k.to_map() if k else None)
+        result['AdvanceLogPolicies'] = []
+        if self.advance_log_policies is not None:
+            for k in self.advance_log_policies:
+                result['AdvanceLogPolicies'].append(k.to_map() if k else None)
+        if self.backup_method is not None:
+            result['BackupMethod'] = self.backup_method
+        if self.backup_priority is not None:
+            result['BackupPriority'] = self.backup_priority
+        if self.backup_retention_period is not None:
+            result['BackupRetentionPeriod'] = self.backup_retention_period
+        if self.backup_retention_policy_on_cluster_deletion is not None:
+            result['BackupRetentionPolicyOnClusterDeletion'] = self.backup_retention_policy_on_cluster_deletion
+        if self.category is not None:
+            result['Category'] = self.category
+        if self.enable_backup is not None:
+            result['EnableBackup'] = self.enable_backup
+        if self.enable_inc_backup is not None:
+            result['EnableIncBackup'] = self.enable_inc_backup
+        if self.enable_log_backup is not None:
+            result['EnableLogBackup'] = self.enable_log_backup
+        if self.high_frequency_bak_interval is not None:
+            result['HighFrequencyBakInterval'] = self.high_frequency_bak_interval
+        if self.high_space_usage_protection is not None:
+            result['HighSpaceUsageProtection'] = self.high_space_usage_protection
+        if self.inc_backup_interval is not None:
+            result['IncBackupInterval'] = self.inc_backup_interval
+        if self.local_log_retention_space is not None:
+            result['LocalLogRetentionSpace'] = self.local_log_retention_space
+        if self.log_backup_local_retention_number is not None:
+            result['LogBackupLocalRetentionNumber'] = self.log_backup_local_retention_number
+        if self.log_backup_retention is not None:
+            result['LogBackupRetention'] = self.log_backup_retention
+        if self.preferred_backup_date is not None:
+            result['PreferredBackupDate'] = self.preferred_backup_date
+        if self.preferred_backup_window is not None:
+            result['PreferredBackupWindow'] = self.preferred_backup_window
+        if self.preferred_backup_window_begin is not None:
+            result['PreferredBackupWindowBegin'] = self.preferred_backup_window_begin
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.advance_data_policies = []
+        if m.get('AdvanceDataPolicies') is not None:
+            for k in m.get('AdvanceDataPolicies'):
+                temp_model = DescribeBackupPolicyResponseBodyDataAdvanceDataPolicies()
+                self.advance_data_policies.append(temp_model.from_map(k))
+        self.advance_log_policies = []
+        if m.get('AdvanceLogPolicies') is not None:
+            for k in m.get('AdvanceLogPolicies'):
+                temp_model = DescribeBackupPolicyResponseBodyDataAdvanceLogPolicies()
+                self.advance_log_policies.append(temp_model.from_map(k))
+        if m.get('BackupMethod') is not None:
+            self.backup_method = m.get('BackupMethod')
+        if m.get('BackupPriority') is not None:
+            self.backup_priority = m.get('BackupPriority')
+        if m.get('BackupRetentionPeriod') is not None:
+            self.backup_retention_period = m.get('BackupRetentionPeriod')
+        if m.get('BackupRetentionPolicyOnClusterDeletion') is not None:
+            self.backup_retention_policy_on_cluster_deletion = m.get('BackupRetentionPolicyOnClusterDeletion')
+        if m.get('Category') is not None:
+            self.category = m.get('Category')
+        if m.get('EnableBackup') is not None:
+            self.enable_backup = m.get('EnableBackup')
+        if m.get('EnableIncBackup') is not None:
+            self.enable_inc_backup = m.get('EnableIncBackup')
+        if m.get('EnableLogBackup') is not None:
+            self.enable_log_backup = m.get('EnableLogBackup')
+        if m.get('HighFrequencyBakInterval') is not None:
+            self.high_frequency_bak_interval = m.get('HighFrequencyBakInterval')
+        if m.get('HighSpaceUsageProtection') is not None:
+            self.high_space_usage_protection = m.get('HighSpaceUsageProtection')
+        if m.get('IncBackupInterval') is not None:
+            self.inc_backup_interval = m.get('IncBackupInterval')
+        if m.get('LocalLogRetentionSpace') is not None:
+            self.local_log_retention_space = m.get('LocalLogRetentionSpace')
+        if m.get('LogBackupLocalRetentionNumber') is not None:
+            self.log_backup_local_retention_number = m.get('LogBackupLocalRetentionNumber')
+        if m.get('LogBackupRetention') is not None:
+            self.log_backup_retention = m.get('LogBackupRetention')
+        if m.get('PreferredBackupDate') is not None:
+            self.preferred_backup_date = m.get('PreferredBackupDate')
+        if m.get('PreferredBackupWindow') is not None:
+            self.preferred_backup_window = m.get('PreferredBackupWindow')
+        if m.get('PreferredBackupWindowBegin') is not None:
+            self.preferred_backup_window_begin = m.get('PreferredBackupWindowBegin')
+        return self
+
+
+class DescribeBackupPolicyResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
-        data: str = None,
+        data: DescribeBackupPolicyResponseBodyData = None,
         err_code: str = None,
         err_message: str = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
-        # The error code returned if the request failed.
         self.code = code
-        # The returned data.
         self.data = data
-        # The error code returned if the request failed.
         self.err_code = err_code
-        # The error message returned if the request failed.
         self.err_message = err_message
-        # The error message returned if the request failed.
         self.message = message
-        # The ID of the request.
         self.request_id = request_id
-        # Indicates whether the request was successful.
         self.success = success
 
     def validate(self):
-        pass
+        if self.data:
+            self.data.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
         if self.data is not None:
-            result['Data'] = self.data
+            result['Data'] = self.data.to_map()
         if self.err_code is not None:
             result['ErrCode'] = self.err_code
         if self.err_message is not None:
             result['ErrMessage'] = self.err_message
         if self.message is not None:
             result['Message'] = self.message
         if self.request_id is not None:
@@ -904,43 +1592,41 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('Data') is not None:
-            self.data = m.get('Data')
+            temp_model = DescribeBackupPolicyResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('ErrCode') is not None:
             self.err_code = m.get('ErrCode')
         if m.get('ErrMessage') is not None:
             self.err_message = m.get('ErrMessage')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
-class DeleteSandboxInstanceResponse(TeaModel):
+class DescribeBackupPolicyResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: DeleteSandboxInstanceResponseBody = None,
+        body: DescribeBackupPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -957,15 +1643,15 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = DeleteSandboxInstanceResponseBody()
+            temp_model = DescribeBackupPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDBTablesRecoveryBackupSetRequest(TeaModel):
     def __init__(
         self,
@@ -1070,17 +1756,14 @@
         body: DescribeDBTablesRecoveryBackupSetResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1210,17 +1893,14 @@
         body: DescribeDBTablesRecoveryStateResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1350,17 +2030,14 @@
         body: DescribeDBTablesRecoveryTimeRangeResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1578,17 +2255,14 @@
         body: DescribeDownloadBackupSetStorageInfoResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1733,17 +2407,14 @@
         body: DescribeDownloadSupportResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1809,15 +2480,15 @@
         # The ID of the region in which the instance resides. You can call the [DescribeDBInstanceAttribute](~~26231~~) operation to query the region ID of the instance.
         self.region_code = region_code
         # The beginning of the time range to query. Specify this parameter as a timestamp of the LONG type. Unit: milliseconds.
         self.start_time = start_time
         # The state of the download task. Valid values:
         # 
         # *   **Initializing**: The download task is being initialized.
-        # *   **queuing**: The download task is queuing.
+        # *   **queueing**: The download task is queuing.
         # *   **running**: The download task is running.
         # *   **failed**: The download task fails.
         # *   **finished**: The download task is complete.
         # *   **expired**: The download task expires.
         self.state = state
         # The type of the download task. Valid values:
         # 
@@ -1902,28 +2573,28 @@
         import_data_size: str = None,
         progress: str = None,
         region_code: str = None,
         target_path: str = None,
         target_type: str = None,
         task_id: str = None,
     ):
-        # The point in time of the backup set if the task is used to download a backup set at a specific point in time. The value is a timestamp of the LONG type. Unit: milliseconds.
+        # The point in time of the backup set if the task is used to download a backup set at a specific point in time. The value is a timestamp of the LONG type. Unit: millisecond.
         self.backup_set_time = backup_set_time
         # The ID of the full backup set.
         self.bak_set_id = bak_set_id
-        # The databases.
+        # The details of the databases.
         self.db_list = db_list
-        # The state of the download task. Valid values:
+        # The status of the download task. Valid values:
         # 
-        # *   **Initializing**: The download task was being initialized.
-        # *   **queuing**: The download task was queuing.
-        # *   **running**: The download task was running.
-        # *   **failed**: The download task failed.
-        # *   **finished**: The download task was complete.
-        # *   **expired**: The download task expired.
+        # *   **Initializing**: The download task is being initialized.
+        # *   **queuing**: The download task is queuing.
+        # *   **running**: The download task is running.
+        # *   **failed**: The download task fails.
+        # *   **finished**: The download task is complete.
+        # *   **expired**: The download task expires.
         self.download_status = download_status
         # The amount of output data. Unit: bytes.
         self.export_data_size = export_data_size
         # The format to which the downloaded backup set is converted. Valid values:
         # 
         # *   **csv**\
         # *   **SQL**\
@@ -1933,22 +2604,22 @@
         self.gmt_create = gmt_create
         # The amount of data that is processed. Unit: bytes.
         self.import_data_size = import_data_size
         # The number of tables that have been downloaded and the total number of tables to be downloaded.
         self.progress = progress
         # The ID of the region in which the instance resides.
         self.region_code = region_code
-        # The destination path to which the data is downloaded if the TargeType parameter is set to OSS.
+        # The destination path to which the data is downloaded if the value of **TargetType is OSS**.
         self.target_path = target_path
         # The type of the method in which the backup set is downloaded. Valid values:
         # 
         # *   **OSS**\
         # *   **URL**\
         self.target_type = target_type
-        # The ID of the download task.
+        # The download task ID.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2056,15 +2727,15 @@
         content: DescribeDownloadTaskResponseBodyDataContent = None,
         extra: str = None,
         page_number: int = None,
         page_size: int = None,
         total_elements: int = None,
         total_pages: int = None,
     ):
-        # The details of the download task.
+        # The details of the task.
         self.content = content
         # The extra description of the download tasks.
         self.extra = extra
         # The page number of the returned page. The value must be an integer that is greater than 0. Default value: 1.
         self.page_number = page_number
         # The number of entries returned per page.
         self.page_size = page_size
@@ -2124,15 +2795,15 @@
         err_message: str = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
         # The error code returned if the request fails.
         self.code = code
-        # The details of the download task.
+        # The details of the tasks.
         self.data = data
         # The error code returned if the request fails.
         self.err_code = err_code
         # The error message returned if the request fails.
         self.err_message = err_message
         # The error message returned if the request fails.
         self.message = message
@@ -2198,17 +2869,14 @@
         body: DescribeDownloadTaskResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2372,17 +3040,14 @@
         body: DescribeSandboxBackupSetsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2553,17 +3218,14 @@
         body: DescribeSandboxInstancesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2741,17 +3403,14 @@
         body: DescribeSandboxRecoveryTimeResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2893,17 +3552,14 @@
         body: ModifyDBTablesRecoveryStateResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3033,17 +3689,14 @@
         body: SupportDBTableRecoveryResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_dbs20210101-1.0.4/alibabacloud_dbs20210101.egg-info/PKG-INFO` & `alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dbs20210101
-Version: 1.0.4
+Version: 2.0.0
 Summary: Alibaba Cloud Dbs (20210101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dbs-20210101/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_dbs20210101-1.0.4/setup.py` & `alibabacloud_dbs20210101-2.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dbs20210101.
 
-Created on 21/08/2023
+Created on 29/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dbs20210101"
 NAME = "alibabacloud_dbs20210101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dbs (20210101) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

