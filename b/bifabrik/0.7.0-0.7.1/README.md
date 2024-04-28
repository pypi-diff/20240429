# Comparing `tmp/bifabrik-0.7.0.tar.gz` & `tmp/bifabrik-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bifabrik-0.7.0.tar", max compression
+gzip compressed data, was "bifabrik-0.7.1.tar", max compression
```

## Comparing `bifabrik-0.7.0.tar` & `bifabrik-0.7.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1073 2024-04-27 16:34:27.127625 bifabrik-0.7.0/LICENSE
--rw-r--r--   0        0        0     4792 2024-04-27 16:34:27.127625 bifabrik-0.7.0/README.md
--rw-r--r--   0        0        0      575 2024-04-27 16:34:27.131625 bifabrik-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     6451 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/__init__.py
--rw-r--r--   0        0        0     2896 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/base/Pipeline.py
--rw-r--r--   0        0        0     1631 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/base/Task.py
--rw-r--r--   0        0        0     4899 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/CompleteConfiguration.py
--rw-r--r--   0        0        0        0 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/Configuration.py
--rw-r--r--   0        0        0      755 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/CsvSourceConfiguration.py
--rw-r--r--   0        0        0      570 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/DataDestinationConfigurationBase.py
--rw-r--r--   0        0        0      525 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/DataSourceConfigurationBase.py
--rw-r--r--   0        0        0      729 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/ExcelSourceConfiguration.py
--rw-r--r--   0        0        0      715 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/JsonSourceConfiguration.py
--rw-r--r--   0        0        0      512 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/SharePointListSourceConfiguration.py
--rw-r--r--   0        0        0      605 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/TableDestinationConfiguration.py
--rw-r--r--   0        0        0        0 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/__init__.py
--rw-r--r--   0        0        0     5045 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/engine/ConfigContainer.py
--rw-r--r--   0        0        0      411 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/engine/Configuration.py
--rw-r--r--   0        0        0     3895 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/CsvConfiguration.py
--rw-r--r--   0        0        0     2617 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py
--rw-r--r--   0        0        0     4700 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/ExcelConfiguration.py
--rw-r--r--   0        0        0     2699 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/FileSourceConfiguration.py
--rw-r--r--   0        0        0     7254 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/JsonConfiguration.py
--rw-r--r--   0        0        0     3782 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/LogConfiguration.py
--rw-r--r--   0        0        0     2159 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py
--rw-r--r--   0        0        0     2350 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/SecurityConfiguration.py
--rw-r--r--   0        0        0     2421 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/SourceStorageConfiguration.py
--rw-r--r--   0        0        0     4673 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/cfg/specific/TableConfiguration.py
--rw-r--r--   0        0        0      931 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/dst/DataDestination.py
--rw-r--r--   0        0        0    13828 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/dst/LakehouseTableDestination.py
--rw-r--r--   0        0        0      909 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/dst/PandasDfDestination.py
--rw-r--r--   0        0        0      834 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/dst/SparkDfDestination.py
--rw-r--r--   0        0        0    24469 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/dst/WarehouseTableDestination.py
--rw-r--r--   0        0        0        0 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/dst/__init__.py
--rw-r--r--   0        0        0     3916 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/CsvSource.py
--rw-r--r--   0        0        0     3803 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/DataSource.py
--rw-r--r--   0        0        0     3925 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/ExcelSource.py
--rw-r--r--   0        0        0     3447 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/JsonSource.py
--rw-r--r--   0        0        0      919 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/PandasDfSource.py
--rw-r--r--   0        0        0     3588 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/SharePointListSource.py
--rw-r--r--   0        0        0      914 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/SparkDfSource.py
--rw-r--r--   0        0        0      941 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/SparkSqlSource.py
--rw-r--r--   0        0        0     2844 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/WarehouseSqlSource.py
--rw-r--r--   0        0        0        0 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/src/__init__.py
--rw-r--r--   0        0        0     3548 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/tsf/DataTransformation.py
--rw-r--r--   0        0        0     1086 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/tsf/PandasDfTransformation.py
--rw-r--r--   0        0        0      916 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/tsf/SparkDfTransformation.py
--rw-r--r--   0        0        0    15243 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/utils/fsUtils.py
--rw-r--r--   0        0        0     7064 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/utils/log.py
--rw-r--r--   0        0        0     2500 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/utils/tableUtils.py
--rw-r--r--   0        0        0     6158 2024-04-27 16:34:27.131625 bifabrik-0.7.0/src/bifabrik/utils/tmslUtils.py
--rw-r--r--   0        0        0     5556 1970-01-01 00:00:00.000000 bifabrik-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-28 22:11:01.170596 bifabrik-0.7.1/LICENSE
+-rw-r--r--   0        0        0     4792 2024-04-28 22:11:01.170596 bifabrik-0.7.1/README.md
+-rw-r--r--   0        0        0      575 2024-04-28 22:11:01.170596 bifabrik-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6451 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/__init__.py
+-rw-r--r--   0        0        0     2896 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/base/Pipeline.py
+-rw-r--r--   0        0        0     1631 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/base/Task.py
+-rw-r--r--   0        0        0     4899 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/CompleteConfiguration.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/Configuration.py
+-rw-r--r--   0        0        0      755 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/CsvSourceConfiguration.py
+-rw-r--r--   0        0        0      570 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/DataDestinationConfigurationBase.py
+-rw-r--r--   0        0        0      525 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/DataSourceConfigurationBase.py
+-rw-r--r--   0        0        0      729 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/ExcelSourceConfiguration.py
+-rw-r--r--   0        0        0      715 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/JsonSourceConfiguration.py
+-rw-r--r--   0        0        0      512 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/SharePointListSourceConfiguration.py
+-rw-r--r--   0        0        0      605 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/TableDestinationConfiguration.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/__init__.py
+-rw-r--r--   0        0        0     5045 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/engine/ConfigContainer.py
+-rw-r--r--   0        0        0      411 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/engine/Configuration.py
+-rw-r--r--   0        0        0     3895 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/CsvConfiguration.py
+-rw-r--r--   0        0        0     2617 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py
+-rw-r--r--   0        0        0     4700 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/ExcelConfiguration.py
+-rw-r--r--   0        0        0     2699 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/FileSourceConfiguration.py
+-rw-r--r--   0        0        0     7254 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/JsonConfiguration.py
+-rw-r--r--   0        0        0     3782 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/LogConfiguration.py
+-rw-r--r--   0        0        0     2159 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py
+-rw-r--r--   0        0        0     2462 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/SecurityConfiguration.py
+-rw-r--r--   0        0        0     2421 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/SourceStorageConfiguration.py
+-rw-r--r--   0        0        0     4673 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/TableConfiguration.py
+-rw-r--r--   0        0        0      931 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/dst/DataDestination.py
+-rw-r--r--   0        0        0    13828 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/dst/LakehouseTableDestination.py
+-rw-r--r--   0        0        0      909 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/dst/PandasDfDestination.py
+-rw-r--r--   0        0        0      834 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/dst/SparkDfDestination.py
+-rw-r--r--   0        0        0    26211 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/dst/WarehouseTableDestination.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/dst/__init__.py
+-rw-r--r--   0        0        0     3916 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/CsvSource.py
+-rw-r--r--   0        0        0     3803 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/DataSource.py
+-rw-r--r--   0        0        0     3925 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/ExcelSource.py
+-rw-r--r--   0        0        0     3447 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/JsonSource.py
+-rw-r--r--   0        0        0      919 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/PandasDfSource.py
+-rw-r--r--   0        0        0     3588 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/SharePointListSource.py
+-rw-r--r--   0        0        0      914 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/SparkDfSource.py
+-rw-r--r--   0        0        0      941 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/SparkSqlSource.py
+-rw-r--r--   0        0        0     3945 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/WarehouseSqlSource.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/__init__.py
+-rw-r--r--   0        0        0     3548 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/tsf/DataTransformation.py
+-rw-r--r--   0        0        0     1086 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/tsf/PandasDfTransformation.py
+-rw-r--r--   0        0        0      916 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/tsf/SparkDfTransformation.py
+-rw-r--r--   0        0        0    15243 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/utils/fsUtils.py
+-rw-r--r--   0        0        0     7064 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/utils/log.py
+-rw-r--r--   0        0        0     2500 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/utils/tableUtils.py
+-rw-r--r--   0        0        0     6158 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/utils/tmslUtils.py
+-rw-r--r--   0        0        0     5556 1970-01-01 00:00:00.000000 bifabrik-0.7.1/PKG-INFO
```

### Comparing `bifabrik-0.7.0/LICENSE` & `bifabrik-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/README.md` & `bifabrik-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/pyproject.toml` & `bifabrik-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bifabrik"
-version = "0.7.0"
+version = "0.7.1"
 description = "Microsoft Fabric ETL toolbox"
 authors = ["Radovan Jankovič"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://rjankovic.github.io/bifabrik/"
 documentation = "https://rjankovic.github.io/bifabrik/"
 repository = "https://github.com/rjankovic/bifabrik/"
```

### Comparing `bifabrik-0.7.0/src/bifabrik/__init__.py` & `bifabrik-0.7.1/src/bifabrik/__init__.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/base/Pipeline.py` & `bifabrik-0.7.1/src/bifabrik/base/Pipeline.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/base/Task.py` & `bifabrik-0.7.1/src/bifabrik/base/Task.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/CompleteConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/CompleteConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/CsvSourceConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/CsvSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/DataDestinationConfigurationBase.py` & `bifabrik-0.7.1/src/bifabrik/cfg/DataDestinationConfigurationBase.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/DataSourceConfigurationBase.py` & `bifabrik-0.7.1/src/bifabrik/cfg/DataSourceConfigurationBase.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/ExcelSourceConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/ExcelSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/JsonSourceConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/JsonSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/SharePointListSourceConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/SharePointListSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/TableDestinationConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/TableDestinationConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/engine/ConfigContainer.py` & `bifabrik-0.7.1/src/bifabrik/cfg/engine/ConfigContainer.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/specific/CsvConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/specific/CsvConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/specific/ExcelConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/specific/ExcelConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/specific/FileSourceConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/specific/FileSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/specific/JsonConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/specific/JsonConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/specific/LogConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/specific/LogConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/specific/SecurityConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/specific/SecurityConfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
     (Passwords aren't actually stored here, this configuration only refers to KeyVault secrets.)
     """
     def __init__(self):
         self._explicitProps = {}
         self.__keyVaultUrl = None
         self.__loginKVSecretName = None
         self.__passwordKVSecretName = None
+        self.__servicePrincipalClientId = None
+        self.__servicePrincipalClientSecretKVSecretName = None
 
     @CfgProperty
     def keyVaultUrl(self) -> str:
         """Key Vault URL - e.g. 'https://kv-fabrik.vault.azure.net/'
         """
         return self.__keyVaultUrl
     @keyVaultUrl.setter(key='keyVaultUrl')
```

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/specific/SourceStorageConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/specific/SourceStorageConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/cfg/specific/TableConfiguration.py` & `bifabrik-0.7.1/src/bifabrik/cfg/specific/TableConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/dst/DataDestination.py` & `bifabrik-0.7.1/src/bifabrik/dst/DataDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/dst/LakehouseTableDestination.py` & `bifabrik-0.7.1/src/bifabrik/dst/LakehouseTableDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/dst/PandasDfDestination.py` & `bifabrik-0.7.1/src/bifabrik/dst/PandasDfDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/dst/SparkDfDestination.py` & `bifabrik-0.7.1/src/bifabrik/dst/SparkDfDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/dst/WarehouseTableDestination.py` & `bifabrik-0.7.1/src/bifabrik/dst/WarehouseTableDestination.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,26 @@
         self.__incrementMethod = incrementMethod
         
         # connect ODBC
         odbcServer = mergedConfig.destinationStorage.destinationWarehouseConnectionString
         odbcDatabase = mergedConfig.destinationStorage.destinationWarehouseName
         odbcTimeout = mergedConfig.destinationStorage.destinationWarehouseConnectionTimeout
         principalClientId = mergedConfig.security.servicePrincipalClientId
+        
+        if odbcServer is None:
+            raise Exception('Cannot connect to warehouse - destinationStorage.destinationWarehouseConnectionString not configured (copy this from the properties of your warehouse)')
+        if odbcDatabase is None:
+            raise Exception('Cannot connect to warehouse - destinationStorage.destinationWarehouseName not configured')
+        if principalClientId is None:
+            raise Exception('Cannot connect to warehouse - security.servicePrincipalClientId not configured (service principal authentication is used)')
+        if mergedConfig.security.keyVaultUrl is None:
+            raise Exception('Cannot connect to warehouse - security.keyVaultUrl not configured (service principal authentication is used and the client secret needs to be stored in key vault)')
+        if mergedConfig.security.servicePrincipalClientSecretKVSecretName is None:
+            raise Exception('Cannot connect to warehouse - security.servicePrincipalClientSecretKVSecretName not configured (service principal authentication is used and the client secret needs to be stored in key vault)')
+        
         principalClientSecret = notebookutils.mssparkutils.credentials.getSecret(mergedConfig.security.keyVaultUrl, mergedConfig.security.servicePrincipalClientSecretKVSecretName)
         constr = f"driver=ODBC Driver 18 for SQL Server;server={odbcServer};database={odbcDatabase};UID={principalClientId};PWD={principalClientSecret};Authentication=ActiveDirectoryServicePrincipal;Encrypt=yes;Timeout={odbcTimeout};"
         self.__odbcConnection = pyodbc.connect(constr)
 
         # create schema if not exists
         findSchemaQuery = f"SELECT COUNT(*) FROM sys.schemas WHERE [name] = '{self.__targetSchemaName}'"
         findSchemaDf = self.__execute_select(findSchemaQuery)
@@ -158,17 +170,17 @@
             elif s_type.startswith('bool'):
                 col_type = 'BIT'
             elif s_type.startswith('int'):
                 col_type = 'INT'
             elif s_type == 'tinyint' or s_type == 'byte' or s_type == 'smallint' or s_type == 'short':
                 col_type = 'SMALLINT'
             elif s_type == 'double':
-                col_type = 'DOUBLE'
+                col_type = 'FLOAT'
             elif s_type == 'float' or s_type == 'real':
-                col_type = 'REAL'
+                col_type = 'FLOAT'
             elif s_type == 'date' or s_type == 'timestamp':
                 col_type = 'DATETIME2(6)'
             elif s_type.startswith('binary') or s_type.startswith('byte'):
                 col_type = 'VARBINARY(8000)'
             elif s_type.startswith('decimal('):
                 col_type = s_type.replace('decimal', 'DECIMAL')
             
@@ -191,14 +203,16 @@
 {column_defs_join}
 )
 '''
 
         if not self.__tableExists:
             self.__execute_dml(createTableSql)
             self.__append_target()
+            self.__odbcConnection.close()
+            self._completed = True
             return
 
         # sync schema if table exists
         origColumnsTypesDf = self.__execute_select(f'''
 SELECT s.name schema_name, t.name table_name, c.name column_name, tt.name type_name, tt.max_length, tt.precision, tt.scale 
 FROM sys.schemas s
 INNER JOIN sys.tables t ON s.schema_id = t.schema_id
@@ -268,14 +282,16 @@
                 dropTableSql = f'''
 DROP TABLE [{self.__targetSchemaName}].[{self.__targetTableName}]
 '''
                 lgr.info('Recreating the table due to schema changes')
                 self.__execute_dml(dropTableSql)
                 self.__execute_dml(createTableSql)
                 self.__append_target()
+                self.__odbcConnection.close()
+                self._completed = True
                 return
             
             raise Exception(f'Cannot resolve schema chnages in table [{self.__targetSchemaName}].[{self.__targetTableName}], column {broken_column_name}({broken_column_type}) - {type_error}')
             
         if schema_change:
             canAddColumns = self.__tableConfig.canAddNewColumns
             if not canAddColumns:
@@ -309,16 +325,14 @@
             FROM [{self.__targetSchemaName}].[{whTempTableName}]
             '''
             self.__execute_dml(insertBackQuery)
 
             # DROP temp_old table
             dropQuery = f'DROP TABLE [{self.__targetSchemaName}].[{whTempTableName}]'
             self.__execute_dml(dropQuery)
-            pass
-        
             
         # handle increments as in a lakehouse
         if incrementMethod == 'overwrite':
             self.__overwrite_target()
         elif incrementMethod == 'append':
             self.__append_target()
         elif incrementMethod == 'merge':
@@ -351,14 +365,22 @@
                 warn = 'Waiting 5 s for blocking DDL to finish'
                 print(warn)
                 self.__logger.warning(e.args[1])
                 self.__logger.warning(warn)
                 time.sleep(5)
                 self.__odbcConnection.execute(query)
                 self.__odbcConnection.commit()
+            elif str(e.args[0]) == '42S02' and e.args[1].find('Invalid object name') > -1 and e.args[1].find('temp') > -1:
+                warn = 'Waiting 5 s for the lakehouse temp table to come online'
+                print(warn)
+                self.__logger.warning(e.args[1])
+                self.__logger.warning(warn)
+                time.sleep(5)
+                self.__odbcConnection.execute(query)
+                self.__odbcConnection.commit()
             else:
                 raise e
 
     def __list_diff(self, first_list, second_list):
         diff = [item for item in first_list if item not in second_list]
         return diff
```

### Comparing `bifabrik-0.7.0/src/bifabrik/src/CsvSource.py` & `bifabrik-0.7.1/src/bifabrik/src/CsvSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/src/DataSource.py` & `bifabrik-0.7.1/src/bifabrik/src/DataSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/src/ExcelSource.py` & `bifabrik-0.7.1/src/bifabrik/src/ExcelSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/src/JsonSource.py` & `bifabrik-0.7.1/src/bifabrik/src/JsonSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/src/PandasDfSource.py` & `bifabrik-0.7.1/src/bifabrik/src/PandasDfSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/src/SharePointListSource.py` & `bifabrik-0.7.1/src/bifabrik/src/SharePointListSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/src/SparkDfSource.py` & `bifabrik-0.7.1/src/bifabrik/src/SparkDfSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/src/SparkSqlSource.py` & `bifabrik-0.7.1/src/bifabrik/src/SparkSqlSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/src/WarehouseSqlSource.py` & `bifabrik-0.7.1/src/bifabrik/src/WarehouseSqlSource.py`

 * *Files 23% similar despite different names*

```diff
@@ -42,14 +42,26 @@
         self.__config = config
         
         # connect ODBC
         odbcServer = config.sourceStorage.sourceWarehouseConnectionString
         odbcDatabase = config.sourceStorage.sourceWarehouseName
         odbcTimeout = config.sourceStorage.sourceWarehouseConnectionTimeout
         principalClientId = config.security.servicePrincipalClientId
+
+        if odbcServer is None:
+            raise Exception('Cannot connect to warehouse - sourceStorage.sourceWarehouseConnectionString not configured (copy this from the properties of your warehouse)')
+        if odbcDatabase is None:
+            raise Exception('Cannot connect to warehouse - sourceStorage.sourceWarehouseName not configured')
+        if principalClientId is None:
+            raise Exception('Cannot connect to warehouse - security.servicePrincipalClientId not configured (service principal authentication is used)')
+        if config.security.keyVaultUrl is None:
+            raise Exception('Cannot connect to warehouse - security.keyVaultUrl not configured (service principal authentication is used and the client secret needs to be stored in key vault)')
+        if config.security.servicePrincipalClientSecretKVSecretName is None:
+            raise Exception('Cannot connect to warehouse - security.servicePrincipalClientSecretKVSecretName not configured (service principal authentication is used and the client secret needs to be stored in key vault)')
+        
         principalClientSecret = notebookutils.mssparkutils.credentials.getSecret(config.security.keyVaultUrl, config.security.servicePrincipalClientSecretKVSecretName)
         constr = f"driver=ODBC Driver 18 for SQL Server;server={odbcServer};database={odbcDatabase};UID={principalClientId};PWD={principalClientSecret};Authentication=ActiveDirectoryServicePrincipal;Encrypt=yes;Timeout={odbcTimeout};"
         if odbcDatabase is None:
             constr = f"driver=ODBC Driver 18 for SQL Server;server={odbcServer};UID={principalClientId};PWD={principalClientSecret};Authentication=ActiveDirectoryServicePrincipal;Encrypt=yes;Timeout={odbcTimeout};"
         self.__odbcConnection = pyodbc.connect(constr)
 
         pd_df = pd.read_sql(self.__query, self.__odbcConnection)
```

### Comparing `bifabrik-0.7.0/src/bifabrik/tsf/DataTransformation.py` & `bifabrik-0.7.1/src/bifabrik/tsf/DataTransformation.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/tsf/PandasDfTransformation.py` & `bifabrik-0.7.1/src/bifabrik/tsf/PandasDfTransformation.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/tsf/SparkDfTransformation.py` & `bifabrik-0.7.1/src/bifabrik/tsf/SparkDfTransformation.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/utils/fsUtils.py` & `bifabrik-0.7.1/src/bifabrik/utils/fsUtils.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/utils/log.py` & `bifabrik-0.7.1/src/bifabrik/utils/log.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/utils/tableUtils.py` & `bifabrik-0.7.1/src/bifabrik/utils/tableUtils.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/src/bifabrik/utils/tmslUtils.py` & `bifabrik-0.7.1/src/bifabrik/utils/tmslUtils.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.0/PKG-INFO` & `bifabrik-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bifabrik
-Version: 0.7.0
+Version: 0.7.1
 Summary: Microsoft Fabric ETL toolbox
 Home-page: https://rjankovic.github.io/bifabrik/
 License: MIT
 Author: Radovan Jankovič
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

