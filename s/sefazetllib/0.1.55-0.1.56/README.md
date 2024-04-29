# Comparing `tmp/sefazetllib-0.1.55.tar.gz` & `tmp/sefazetllib-0.1.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sefazetllib-0.1.55.tar", max compression
+gzip compressed data, was "sefazetllib-0.1.56.tar", max compression
```

## Comparing `sefazetllib-0.1.55.tar` & `sefazetllib-0.1.56.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0    10173 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/LICENSE
--rw-r--r--   0        0        0     3159 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/README.md
--rw-r--r--   0        0        0     2442 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/pyproject.toml
--rw-r--r--   0        0        0     1663 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/Builder.py
--rw-r--r--   0        0        0      135 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/__init__.py
--rw-r--r--   0        0        0     2338 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/config/CustomLogging.py
--rw-r--r--   0        0        0       52 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/config/__init__.py
--rw-r--r--   0        0        0     8768 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/etl/ETL.py
--rw-r--r--   0        0        0       36 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/etl/__init__.py
--rw-r--r--   0        0        0      701 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/extract/Extract.py
--rw-r--r--   0        0        0     1986 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/extract/ExtractLocal.py
--rw-r--r--   0        0        0     2699 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/extract/ExtractS3.py
--rw-r--r--   0        0        0     2521 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/extract/ExtractSQL.py
--rw-r--r--   0        0        0     2282 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/extract/ExtractStorage.py
--rw-r--r--   0        0        0      274 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/extract/__init__.py
--rw-r--r--   0        0        0      949 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/Factory.py
--rw-r--r--   0        0        0       89 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/__init__.py
--rw-r--r--   0        0        0      362 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/DatabasePlatform.py
--rw-r--r--   0        0        0      281 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/Platform.py
--rw-r--r--   0        0        0     1049 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/PlatformFactory.py
--rw-r--r--   0        0        0      268 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/__init__.py
--rw-r--r--   0        0        0      723 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/database/MySQL.py
--rw-r--r--   0        0        0     8285 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/database/PostgreSQL.py
--rw-r--r--   0        0        0      134 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/database/__init__.py
--rw-r--r--   0        0        0      259 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/dataframe/Default.py
--rw-r--r--   0        0        0     1793 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/dataframe/Pandas.py
--rw-r--r--   0        0        0     5746 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/dataframe/Spark.py
--rw-r--r--   0        0        0      195 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/factory/platform/dataframe/__init__.py
--rw-r--r--   0        0        0      683 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/load/Load.py
--rw-r--r--   0        0        0     2467 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/load/LoadLocal.py
--rw-r--r--   0        0        0     5029 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/load/LoadS3.py
--rw-r--r--   0        0        0    11970 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/load/LoadSQL.py
--rw-r--r--   0        0        0     2611 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/load/LoadStorage.py
--rw-r--r--   0        0        0      229 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/load/__init__.py
--rw-r--r--   0        0        0      573 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/ColumnsToLowerCase.py
--rw-r--r--   0        0        0     1033 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/ConvertColumnsType.py
--rw-r--r--   0        0        0     1232 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/DataFrameFilterRangeTransform.py
--rw-r--r--   0        0        0     1471 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/MinMaxLineTransform.py
--rw-r--r--   0        0        0     4331 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/QuartileTransform.py
--rw-r--r--   0        0        0      921 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/RemoveColumnsByPrefix.py
--rw-r--r--   0        0        0     1047 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/RoundColumns.py
--rw-r--r--   0        0        0      552 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/Transform.py
--rw-r--r--   0        0        0      502 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/transform/__init__.py
--rw-r--r--   0        0        0       45 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/__init__.py
--rw-r--r--   0        0        0      325 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/key/DefaultKey.py
--rw-r--r--   0        0        0      400 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/key/Key.py
--rw-r--r--   0        0        0      747 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/key/SurrogateKey.py
--rw-r--r--   0        0        0      158 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/key/__init__.py
--rw-r--r--   0        0        0     2097 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/partition/DatePartition.py
--rw-r--r--   0        0        0      627 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/partition/IncrementalRangePartition.py
--rw-r--r--   0        0        0      425 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/partition/Partition.py
--rw-r--r--   0        0        0      229 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/utils/partition/__init__.py
--rw-r--r--   0        0        0     7729 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/validate/DataValidate.py
--rw-r--r--   0        0        0      383 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/validate/Validate.py
--rw-r--r--   0        0        0      110 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllib/validate/__init__.py
--rw-r--r--   0        0        0     3551 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/config/__init__.py
--rw-r--r--   0        0        0     1117 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/config/logging.py
--rw-r--r--   0        0        0      185 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/errors/__init__.py
--rw-r--r--   0        0        0       76 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/errors/method_not_implemented.py
--rw-r--r--   0        0        0       52 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/errors/unsupported_file_extension.py
--rw-r--r--   0        0        0       88 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/errors/variable_processing_error.py
--rw-r--r--   0        0        0        0 2024-04-08 19:27:18.627372 sefazetllib-0.1.55/sefazetllibcli/generators/__init__.py
--rw-r--r--   0        0        0     6415 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/generators/etl_generator.py
--rw-r--r--   0        0        0      884 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/generators/generator.py
--rw-r--r--   0        0        0      374 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/templates/etl_template
--rw-r--r--   0        0        0        0 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/__init__.py
--rw-r--r--   0        0        0      524 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/__init__.py
--rw-r--r--   0        0        0     3484 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_etl_variable.py
--rw-r--r--   0        0        0     1128 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_extract_variable.py
--rw-r--r--   0        0        0      986 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_imports_variable.py
--rw-r--r--   0        0        0     1142 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_key_variable.py
--rw-r--r--   0        0        0     1110 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_load_variable.py
--rw-r--r--   0        0        0     1595 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_partition_variable.py
--rw-r--r--   0        0        0     2086 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_transforms_variable.py
--rw-r--r--   0        0        0     1074 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_validate_variable.py
--rw-r--r--   0        0        0      935 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_variable.py
--rw-r--r--   0        0        0       99 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/replace_template/__init__.py
--rw-r--r--   0        0        0      963 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/replace_template/replace_etl_template.py
--rw-r--r--   0        0        0     1678 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/usecases/replace_template/replace_template.py
--rw-r--r--   0        0        0       32 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/utils/__init__.py
--rw-r--r--   0        0        0     3631 2024-04-08 19:27:18.637372 sefazetllib-0.1.55/sefazetllibcli/utils/parse_etl.py
--rw-r--r--   0        0        0     4728 1970-01-01 00:00:00.000000 sefazetllib-0.1.55/PKG-INFO
+-rw-r--r--   0        0        0    10349 2023-06-16 20:57:30.403958 sefazetllib-0.1.56/LICENSE
+-rw-r--r--   0        0        0     2535 2024-04-27 19:53:23.425089 sefazetllib-0.1.56/pyproject.toml
+-rw-r--r--   0        0        0     3264 2023-06-16 20:57:30.404954 sefazetllib-0.1.56/README.md
+-rw-r--r--   0        0        0      137 2023-06-16 20:57:30.462954 sefazetllib-0.1.56/sefazetllib/__init__.py
+-rw-r--r--   0        0        0     1716 2023-10-31 19:41:45.261519 sefazetllib-0.1.56/sefazetllib/Builder.py
+-rw-r--r--   0        0        0       53 2023-06-16 20:57:30.463953 sefazetllib-0.1.56/sefazetllib/config/__init__.py
+-rw-r--r--   0        0        0     2415 2023-09-14 13:01:03.215884 sefazetllib-0.1.56/sefazetllib/config/CustomLogging.py
+-rw-r--r--   0        0        0       37 2023-06-16 20:57:30.466488 sefazetllib-0.1.56/sefazetllib/etl/__init__.py
+-rw-r--r--   0        0        0     9023 2024-04-08 22:43:31.049932 sefazetllib-0.1.56/sefazetllib/etl/ETL.py
+-rw-r--r--   0        0        0      279 2023-06-16 20:57:30.471496 sefazetllib-0.1.56/sefazetllib/extract/__init__.py
+-rw-r--r--   0        0        0      729 2023-09-14 13:01:03.224996 sefazetllib-0.1.56/sefazetllib/extract/Extract.py
+-rw-r--r--   0        0        0     2047 2023-09-14 13:01:03.227984 sefazetllib-0.1.56/sefazetllib/extract/ExtractLocal.py
+-rw-r--r--   0        0        0     2778 2024-01-23 23:52:35.837036 sefazetllib-0.1.56/sefazetllib/extract/ExtractS3.py
+-rw-r--r--   0        0        0     2600 2023-09-14 13:01:03.236540 sefazetllib-0.1.56/sefazetllib/extract/ExtractSQL.py
+-rw-r--r--   0        0        0     2351 2023-09-14 13:01:03.240085 sefazetllib-0.1.56/sefazetllib/extract/ExtractStorage.py
+-rw-r--r--   0        0        0       91 2023-06-16 20:57:30.472943 sefazetllib-0.1.56/sefazetllib/factory/__init__.py
+-rw-r--r--   0        0        0      967 2023-09-14 13:01:03.243083 sefazetllib-0.1.56/sefazetllib/factory/Factory.py
+-rw-r--r--   0        0        0      272 2023-06-16 20:57:30.477463 sefazetllib-0.1.56/sefazetllib/factory/platform/__init__.py
+-rw-r--r--   0        0        0      136 2023-06-16 20:57:30.480507 sefazetllib-0.1.56/sefazetllib/factory/platform/database/__init__.py
+-rw-r--r--   0        0        0      749 2023-09-14 13:01:03.253166 sefazetllib-0.1.56/sefazetllib/factory/platform/database/MySQL.py
+-rw-r--r--   0        0        0     8534 2023-12-20 20:12:44.691247 sefazetllib-0.1.56/sefazetllib/factory/platform/database/PostgreSQL.py
+-rw-r--r--   0        0        0      380 2023-09-14 13:01:03.245090 sefazetllib-0.1.56/sefazetllib/factory/platform/DatabasePlatform.py
+-rw-r--r--   0        0        0      198 2023-06-16 20:57:30.485499 sefazetllib-0.1.56/sefazetllib/factory/platform/dataframe/__init__.py
+-rw-r--r--   0        0        0      272 2023-09-14 13:01:03.266762 sefazetllib-0.1.56/sefazetllib/factory/platform/dataframe/Default.py
+-rw-r--r--   0        0        0     1854 2023-09-14 13:01:03.273303 sefazetllib-0.1.56/sefazetllib/factory/platform/dataframe/Pandas.py
+-rw-r--r--   0        0        0     5929 2024-04-08 22:43:31.049932 sefazetllib-0.1.56/sefazetllib/factory/platform/dataframe/Spark.py
+-rw-r--r--   0        0        0      297 2023-09-14 13:01:03.248628 sefazetllib-0.1.56/sefazetllib/factory/platform/Platform.py
+-rw-r--r--   0        0        0     1077 2023-09-14 13:01:03.251648 sefazetllib-0.1.56/sefazetllib/factory/platform/PlatformFactory.py
+-rw-r--r--   0        0        0      234 2023-06-16 20:57:30.492061 sefazetllib-0.1.56/sefazetllib/load/__init__.py
+-rw-r--r--   0        0        0      711 2023-09-14 13:01:03.280852 sefazetllib-0.1.56/sefazetllib/load/Load.py
+-rw-r--r--   0        0        0     2539 2024-01-23 23:52:35.838545 sefazetllib-0.1.56/sefazetllib/load/LoadLocal.py
+-rw-r--r--   0        0        0     5159 2024-01-31 23:46:10.933840 sefazetllib-0.1.56/sefazetllib/load/LoadS3.py
+-rw-r--r--   0        0        0    12287 2024-01-23 23:52:35.841553 sefazetllib-0.1.56/sefazetllib/load/LoadSQL.py
+-rw-r--r--   0        0        0     2686 2024-01-23 23:52:35.843555 sefazetllib-0.1.56/sefazetllib/load/LoadStorage.py
+-rw-r--r--   0        0        0      509 2023-12-20 14:16:36.745122 sefazetllib-0.1.56/sefazetllib/transform/__init__.py
+-rw-r--r--   0        0        0      593 2023-09-14 13:01:03.301976 sefazetllib-0.1.56/sefazetllib/transform/ColumnsToLowerCase.py
+-rw-r--r--   0        0        0     1067 2024-03-11 20:29:51.624256 sefazetllib-0.1.56/sefazetllib/transform/ConvertColumnsType.py
+-rw-r--r--   0        0        0     1269 2024-04-03 19:05:32.349035 sefazetllib-0.1.56/sefazetllib/transform/DataFrameFilterRangeTransform.py
+-rw-r--r--   0        0        0     1523 2023-09-14 13:01:03.303976 sefazetllib-0.1.56/sefazetllib/transform/MinMaxLineTransform.py
+-rw-r--r--   0        0        0     4445 2023-09-14 13:01:03.306981 sefazetllib-0.1.56/sefazetllib/transform/QuartileTransform.py
+-rw-r--r--   0        0        0      951 2023-12-18 16:43:09.268995 sefazetllib-0.1.56/sefazetllib/transform/RemoveColumnsByPrefix.py
+-rw-r--r--   0        0        0     1081 2024-03-06 01:41:29.310418 sefazetllib-0.1.56/sefazetllib/transform/RoundColumns.py
+-rw-r--r--   0        0        0      577 2024-04-03 16:05:59.890974 sefazetllib-0.1.56/sefazetllib/transform/Transform.py
+-rw-r--r--   0        0        0       46 2023-06-16 20:57:30.496207 sefazetllib-0.1.56/sefazetllib/utils/__init__.py
+-rw-r--r--   0        0        0      161 2023-06-16 20:57:30.500777 sefazetllib-0.1.56/sefazetllib/utils/key/__init__.py
+-rw-r--r--   0        0        0      339 2023-09-14 13:01:03.311522 sefazetllib-0.1.56/sefazetllib/utils/key/DefaultKey.py
+-rw-r--r--   0        0        0      419 2023-09-14 13:01:03.314065 sefazetllib-0.1.56/sefazetllib/utils/key/Key.py
+-rw-r--r--   0        0        0      775 2023-09-14 13:01:03.318062 sefazetllib-0.1.56/sefazetllib/utils/key/SurrogateKey.py
+-rw-r--r--   0        0        0      234 2023-06-16 20:57:30.505304 sefazetllib-0.1.56/sefazetllib/utils/partition/__init__.py
+-rw-r--r--   0        0        0     2172 2023-09-14 13:01:03.326123 sefazetllib-0.1.56/sefazetllib/utils/partition/DatePartition.py
+-rw-r--r--   0        0        0      652 2023-09-14 13:01:03.328137 sefazetllib-0.1.56/sefazetllib/utils/partition/IncrementalRangePartition.py
+-rw-r--r--   0        0        0      447 2023-09-14 13:01:03.332140 sefazetllib-0.1.56/sefazetllib/utils/partition/Partition.py
+-rw-r--r--   0        0        0      112 2023-06-16 20:57:30.507824 sefazetllib-0.1.56/sefazetllib/validate/__init__.py
+-rw-r--r--   0        0        0     7943 2023-09-14 13:01:03.338139 sefazetllib-0.1.56/sefazetllib/validate/DataValidate.py
+-rw-r--r--   0        0        0      401 2023-09-14 13:01:03.462911 sefazetllib-0.1.56/sefazetllib/validate/Validate.py
+-rw-r--r--   0        0        0     3675 2023-06-16 20:57:30.508846 sefazetllib-0.1.56/sefazetllibcli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 20:57:30.508846 sefazetllib-0.1.56/sefazetllibcli/config/__init__.py
+-rw-r--r--   0        0        0     1153 2023-09-14 13:01:03.544497 sefazetllib-0.1.56/sefazetllibcli/config/logging.py
+-rw-r--r--   0        0        0      188 2023-06-16 20:57:30.510846 sefazetllib-0.1.56/sefazetllibcli/errors/__init__.py
+-rw-r--r--   0        0        0       78 2023-06-16 20:57:30.511846 sefazetllib-0.1.56/sefazetllibcli/errors/method_not_implemented.py
+-rw-r--r--   0        0        0       54 2023-06-16 20:57:30.511846 sefazetllib-0.1.56/sefazetllibcli/errors/unsupported_file_extension.py
+-rw-r--r--   0        0        0       90 2023-06-16 20:57:30.512843 sefazetllib-0.1.56/sefazetllibcli/errors/variable_processing_error.py
+-rw-r--r--   0        0        0        0 2023-06-16 20:57:30.513857 sefazetllib-0.1.56/sefazetllibcli/generators/__init__.py
+-rw-r--r--   0        0        0     6600 2023-06-29 04:00:58.986017 sefazetllib-0.1.56/sefazetllibcli/generators/etl_generator.py
+-rw-r--r--   0        0        0      908 2023-09-14 13:01:03.564764 sefazetllib-0.1.56/sefazetllibcli/generators/generator.py
+-rw-r--r--   0        0        0      390 2023-06-16 20:57:30.516922 sefazetllib-0.1.56/sefazetllibcli/templates/etl_template
+-rw-r--r--   0        0        0        0 2023-06-16 20:57:30.517839 sefazetllib-0.1.56/sefazetllibcli/usecases/__init__.py
+-rw-r--r--   0        0        0      533 2023-06-16 20:57:30.519362 sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/__init__.py
+-rw-r--r--   0        0        0     3582 2023-09-14 13:01:03.579910 sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/process_etl_variable.py
+-rw-r--r--   0        0        0     1158 2023-09-14 13:01:03.635702 sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/process_extract_variable.py
+-rw-r--r--   0        0        0     1014 2023-09-14 13:01:03.675314 sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/process_imports_variable.py
+-rw-r--r--   0        0        0     1174 2023-09-14 13:01:03.706120 sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/process_key_variable.py
+-rw-r--r--   0        0        0     1140 2023-09-14 13:01:03.727103 sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/process_load_variable.py
+-rw-r--r--   0        0        0     1640 2023-09-14 13:01:03.765127 sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/process_partition_variable.py
+-rw-r--r--   0        0        0     2148 2023-09-14 13:01:03.775726 sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/process_transforms_variable.py
+-rw-r--r--   0        0        0     1106 2023-09-14 13:01:03.781380 sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/process_validate_variable.py
+-rw-r--r--   0        0        0      963 2023-09-14 13:01:03.853234 sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/process_variable.py
+-rw-r--r--   0        0        0      101 2023-06-16 20:57:30.525931 sefazetllib-0.1.56/sefazetllibcli/usecases/replace_template/__init__.py
+-rw-r--r--   0        0        0      996 2023-06-16 20:57:30.526953 sefazetllib-0.1.56/sefazetllibcli/usecases/replace_template/replace_etl_template.py
+-rw-r--r--   0        0        0     1724 2023-09-14 13:01:03.868513 sefazetllib-0.1.56/sefazetllibcli/usecases/replace_template/replace_template.py
+-rw-r--r--   0        0        0       33 2023-06-16 20:57:30.529481 sefazetllib-0.1.56/sefazetllibcli/utils/__init__.py
+-rw-r--r--   0        0        0     3744 2023-09-14 13:01:03.896778 sefazetllib-0.1.56/sefazetllibcli/utils/parse_etl.py
+-rw-r--r--   0        0        0     4968 1970-01-01 00:00:00.000000 sefazetllib-0.1.56/setup.py
+-rw-r--r--   0        0        0     4924 1970-01-01 00:00:00.000000 sefazetllib-0.1.56/PKG-INFO
```

### Comparing `sefazetllib-0.1.55/LICENSE` & `sefazetllib-0.1.56/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
```

### Comparing `sefazetllib-0.1.55/README.md` & `sefazetllib-0.1.56/README.md`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-# sefazetllib
-
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
-[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
----
-
-**Documentation**: [https://main.d32to2oidohzrl.amplifyapp.com/](https://main.d32to2oidohzrl.amplifyapp.com/)
-
-**Source code**: [AWS CodeCommit](https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1)
-
----
-
-**sefazetllib** is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.
-
-## Features
-
-- Easy to use and understand library for constructing ETL/ELT pipelines.
-- Compatibility with popular data processing frameworks, such as [pandas](https://pandas.pydata.org/) and [PySpark](https://spark.apache.org/).
-- Support for file formats such as CSV and Parquet.
-- Provides the ability to extract, transform and load data with customizable configurations.
-
-## Requirements
-
-**sefazetllib** requires the following to run:
-
-- [Python](https://www.python.org/) 3.7.1+
-- [pandas](https://pandas.pydata.org/) 1.3+
-- [PyArrow](https://arrow.apache.org/) 6.0+
-- [PySpark](https://spark.apache.org/) 3.0+
-- [PyDeequ](https://pydeequ.readthedocs.io/) 1.0+
-- [Boto3](https://github.com/boto/boto3) 1.24+
-
-## Installation
-
-Use [pip](https://pip.pypa.io/en/stable/) to install **sefazetllib**:
-
-```bash
-pip install sefazetllib
-```
-
-## Usage
-
-Here is an example of how to use the **sefazetllib**:
-
-```Python
-from typing import Tuple
-
-from pandas import DataFrame
-
-from sefazetllib import Builder
-from sefazetllib.etl import ETL
-from sefazetllib.extract import ExtractLocal
-from sefazetllib.factory.platform import PlatformFactory
-from sefazetllib.load import LoadLocal
-from sefazetllib.transform import Transform
-from sefazetllib.utils.key import SurrogateKey
-
-
-@Builder
-class TestingDataFrame(Transform):
-    def execute(self) -> Tuple[str, DataFrame]:
-        return (
-            "dataframe",
-            DataFrame(
-                [["tom", 10], ["nick", 15], ["juli", 14]], columns=["Name", "Age"]
-            ),
-        )
-
-
-(
-    ETL()
-    .setPlatform(PlatformFactory("Pandas").create(name="test_pandas"))
-    .transform(TestingDataFrame)
-    .load(
-        LoadLocal()
-        .setFileFormat("parquet")
-        .setEntity("load_test")
-        .setMode("overwrite")
-        .setReference("dataframe")
-        .setDuplicates(True)
-        .setKey(SurrogateKey().setColumns(["Name", "Age"]).setDistribute(False))
-    )
-    .extract(
-        ExtractLocal()
-        .setFileFormat("parquet")
-        .setUrl("load_test.parquet")
-        .setReference("extract_test")
-    )
-)
-```
-
-## Testing
-
-To run the unit tests, run the following command:
-
-```bash
-py -m unittest tests/main.py -v
-```
-
-## License
-
-**sefazetllib** is released under the [Apache-2.0](/LICENSE).
+# sefazetllib
+
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+---
+
+**Documentation**: [https://main.d32to2oidohzrl.amplifyapp.com/](https://main.d32to2oidohzrl.amplifyapp.com/)
+
+**Source code**: [AWS CodeCommit](https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1)
+
+---
+
+**sefazetllib** is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.
+
+## Features
+
+- Easy to use and understand library for constructing ETL/ELT pipelines.
+- Compatibility with popular data processing frameworks, such as [pandas](https://pandas.pydata.org/) and [PySpark](https://spark.apache.org/).
+- Support for file formats such as CSV and Parquet.
+- Provides the ability to extract, transform and load data with customizable configurations.
+
+## Requirements
+
+**sefazetllib** requires the following to run:
+
+- [Python](https://www.python.org/) 3.7.1+
+- [pandas](https://pandas.pydata.org/) 1.3+
+- [PyArrow](https://arrow.apache.org/) 6.0+
+- [PySpark](https://spark.apache.org/) 3.0+
+- [PyDeequ](https://pydeequ.readthedocs.io/) 1.0+
+- [Boto3](https://github.com/boto/boto3) 1.24+
+
+## Installation
+
+Use [pip](https://pip.pypa.io/en/stable/) to install **sefazetllib**:
+
+```bash
+pip install sefazetllib
+```
+
+## Usage
+
+Here is an example of how to use the **sefazetllib**:
+
+```Python
+from typing import Tuple
+
+from pandas import DataFrame
+
+from sefazetllib import Builder
+from sefazetllib.etl import ETL
+from sefazetllib.extract import ExtractLocal
+from sefazetllib.factory.platform import PlatformFactory
+from sefazetllib.load import LoadLocal
+from sefazetllib.transform import Transform
+from sefazetllib.utils.key import SurrogateKey
+
+
+@Builder
+class TestingDataFrame(Transform):
+    def execute(self) -> Tuple[str, DataFrame]:
+        return (
+            "dataframe",
+            DataFrame(
+                [["tom", 10], ["nick", 15], ["juli", 14]], columns=["Name", "Age"]
+            ),
+        )
+
+
+(
+    ETL()
+    .setPlatform(PlatformFactory("Pandas").create(name="test_pandas"))
+    .transform(TestingDataFrame)
+    .load(
+        LoadLocal()
+        .setFileFormat("parquet")
+        .setEntity("load_test")
+        .setMode("overwrite")
+        .setReference("dataframe")
+        .setDuplicates(True)
+        .setKey(SurrogateKey().setColumns(["Name", "Age"]).setDistribute(False))
+    )
+    .extract(
+        ExtractLocal()
+        .setFileFormat("parquet")
+        .setUrl("load_test.parquet")
+        .setReference("extract_test")
+    )
+)
+```
+
+## Testing
+
+To run the unit tests, run the following command:
+
+```bash
+py -m unittest tests/main.py -v
+```
+
+## License
+
+**sefazetllib** is released under the [Apache-2.0](/LICENSE).
```

### Comparing `sefazetllib-0.1.55/sefazetllib/Builder.py` & `sefazetllib-0.1.56/sefazetllib/Builder.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from dataclasses import dataclass, field
-
-
-class Builder:
-    """A builder class that creates instances of a given dataclass model and sets values
-    for its non-private fields through dynamically created setter methods.
-    """
-
-    def __init__(self, model) -> None:
-        self.model = dataclass(model)
-        self.instance = None
-
-    def __call__(self):
-        """Creates an instance of the dataclass model and sets its non-private fields using
-        dynamically created setter methods.
-
-        Returns:
-            The created instance of the dataclass model.
-        """
-        self.instance = self.model()
-        self.add_setters()
-        self.instance.setup()
-        return self.instance
-
-    def add_setters(self) -> None:
-        """Adds setter methods to the instance of the dataclass model for each of its
-        non-private fields.
-        """
-        keys = [
-            {"name": field.name, "type": field.type}
-            for field in self.model.__dataclass_fields__.values()
-            if field.name[0] != "_"
-        ]
-
-        for key in keys:
-            name: str = key["name"].replace("_", " ").title().replace(" ", "")
-            setattr(self.instance, f"set{name}", self.func(key))
-
-    def func(self, key):
-        """Returns a setter function for a given field.
-
-        Parameters:
-            key: The name and type of the field.
-
-        Returns:
-            A setter function that sets the value of the field in the instance of the dataclass model and returns the instance.
-        """
-
-        def ex(value):
-            setattr(self.instance, key["name"], value)
-            return self.instance
-
-        return ex
+from dataclasses import dataclass, field
+
+
+class Builder:
+    """A builder class that creates instances of a given dataclass model and sets values
+    for its non-private fields through dynamically created setter methods.
+    """
+
+    def __init__(self, model) -> None:
+        self.model = dataclass(model)
+        self.instance = None
+
+    def __call__(self):
+        """Creates an instance of the dataclass model and sets its non-private fields using
+        dynamically created setter methods.
+
+        Returns:
+            The created instance of the dataclass model.
+        """
+        self.instance = self.model()
+        self.add_setters()
+        self.instance.setup()
+        return self.instance
+
+    def add_setters(self) -> None:
+        """Adds setter methods to the instance of the dataclass model for each of its
+        non-private fields.
+        """
+        keys = [
+            {"name": field.name, "type": field.type}
+            for field in self.model.__dataclass_fields__.values()
+            if field.name[0] != "_"
+        ]
+
+        for key in keys:
+            name: str = key["name"].replace("_", " ").title().replace(" ", "")
+            setattr(self.instance, f"set{name}", self.func(key))
+
+    def func(self, key):
+        """Returns a setter function for a given field.
+
+        Parameters:
+            key: The name and type of the field.
+
+        Returns:
+            A setter function that sets the value of the field in the instance of the dataclass model and returns the instance.
+        """
+
+        def ex(value):
+            setattr(self.instance, key["name"], value)
+            return self.instance
+
+        return ex
```

### Comparing `sefazetllib-0.1.55/sefazetllib/config/CustomLogging.py` & `sefazetllib-0.1.56/sefazetllib/config/CustomLogging.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-from logging import (
-    CRITICAL,
-    DEBUG,
-    ERROR,
-    INFO,
-    WARNING,
-    Filter,
-    Formatter,
-    LogRecord,
-    StreamHandler,
-    getLogger,
-)
-from typing import Dict
-from uuid import uuid4
-
-
-class RequestIdFilter(Filter):
-    """RequestIdFilter is a custom logging filter that adds a unique request ID to each log record.
-    The request ID is generated using the UUID library and is added to the log record as the 'request_id' attribute.
-    """
-
-    # def __init__(self, name="", id=uuid4()) -> None:
-    #     super().__init__(name)
-    #     self.id = id
-    def __init__(self) -> None:
-        self.id = uuid4()
-
-    def filter(self, record: LogRecord) -> bool:
-        """Filter method adds a unique request ID to each log record.
-
-        Parameters:
-            record (LogRecord): The log record being processed.
-
-        Returns:
-            bool: Always returns True to indicate that the log record should be processed.
-        """
-        # record.request_name = self.name
-        record.request_id = str(self.id)
-        return True
-
-
-class LogColorFormatter(Formatter):
-    """LogColorFormatter is a custom logging formatter that formats log records with color coding for different log levels.
-    The log format includes the timestamp, request ID, log level, and log message.
-    """
-
-    colors: Dict[int, str] = {
-        DEBUG: "\x1b[30m",
-        INFO: "\x1b[36m",
-        WARNING: "\x1b[33m",
-        ERROR: "\x1b[31m",
-        CRITICAL: "\x1b[31;1m",
-    }
-
-    template: str = "\x1b[32m[%(asctime)s] \x1b[30m[%(request_id)s] {level_color}%(levelname)s \x1b[0m%(message)s"
-
-    def format(self, record: LogRecord) -> str:
-        """Format method that formats a log record with color coding for different log levels.
-
-        Parameters:
-            record (LogRecord): The log record being processed.
-
-        Returns:
-            str: the formatted log record.
-        """
-        # color: Optional[str] = self.colors.get(record.levelno)
-        # log_format: str = self.template.format(level_color=color)
-        log_format: str = "[%(asctime)s] [%(request_id)s] %(levelname)s %(message)s"
-        return Formatter(log_format).format(record)
-
-
-logger = getLogger("sefazetllib")
-logger.setLevel(DEBUG)
-
-handler = StreamHandler()
-handler.setFormatter(LogColorFormatter())
-logger.addHandler(handler)
+from logging import (
+    CRITICAL,
+    DEBUG,
+    ERROR,
+    INFO,
+    WARNING,
+    Filter,
+    Formatter,
+    LogRecord,
+    StreamHandler,
+    getLogger,
+)
+from typing import Dict
+from uuid import uuid4
+
+
+class RequestIdFilter(Filter):
+    """RequestIdFilter is a custom logging filter that adds a unique request ID to each log record.
+    The request ID is generated using the UUID library and is added to the log record as the 'request_id' attribute.
+    """
+
+    # def __init__(self, name="", id=uuid4()) -> None:
+    #     super().__init__(name)
+    #     self.id = id
+    def __init__(self) -> None:
+        self.id = uuid4()
+
+    def filter(self, record: LogRecord) -> bool:
+        """Filter method adds a unique request ID to each log record.
+
+        Parameters:
+            record (LogRecord): The log record being processed.
+
+        Returns:
+            bool: Always returns True to indicate that the log record should be processed.
+        """
+        # record.request_name = self.name
+        record.request_id = str(self.id)
+        return True
+
+
+class LogColorFormatter(Formatter):
+    """LogColorFormatter is a custom logging formatter that formats log records with color coding for different log levels.
+    The log format includes the timestamp, request ID, log level, and log message.
+    """
+
+    colors: Dict[int, str] = {
+        DEBUG: "\x1b[30m",
+        INFO: "\x1b[36m",
+        WARNING: "\x1b[33m",
+        ERROR: "\x1b[31m",
+        CRITICAL: "\x1b[31;1m",
+    }
+
+    template: str = "\x1b[32m[%(asctime)s] \x1b[30m[%(request_id)s] {level_color}%(levelname)s \x1b[0m%(message)s"
+
+    def format(self, record: LogRecord) -> str:
+        """Format method that formats a log record with color coding for different log levels.
+
+        Parameters:
+            record (LogRecord): The log record being processed.
+
+        Returns:
+            str: the formatted log record.
+        """
+        # color: Optional[str] = self.colors.get(record.levelno)
+        # log_format: str = self.template.format(level_color=color)
+        log_format: str = "[%(asctime)s] [%(request_id)s] %(levelname)s %(message)s"
+        return Formatter(log_format).format(record)
+
+
+logger = getLogger("sefazetllib")
+logger.setLevel(DEBUG)
+
+handler = StreamHandler()
+handler.setFormatter(LogColorFormatter())
+logger.addHandler(handler)
```

### Comparing `sefazetllib-0.1.55/sefazetllib/etl/ETL.py` & `sefazetllib-0.1.56/sefazetllib/etl/ETL.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-import argparse
-import re
-import sys
-from typing import List
-
-from pyspark.sql.functions import col
-
-from sefazetllib.Builder import Builder, field
-from sefazetllib.config.CustomLogging import RequestIdFilter, logger
-from sefazetllib.extract.Extract import Extract
-from sefazetllib.factory.platform.dataframe.Default import Default
-from sefazetllib.factory.platform.Platform import Platform
-from sefazetllib.load.Load import Load
-from sefazetllib.transform.Transform import Transform
-from sefazetllib.validate.Validate import Validate
-
-
-@Builder
-class ETL:
-    """
-    ETL class for executing data extraction, transformation, and loading operations.
-    """
-
-    platform: Platform = field(default_factory=Default)
-    partition: List = field(default_factory=list)
-    repository: str = field(default="")
-
-    def setup(self) -> None:
-        """
-        Parse command-line arguments and store them in self.args.
-        """
-        self.args = self.__get_arguments()
-        # logger.addFilter(RequestIdFilter(self.args.jobName, self.args.jobId))
-        logger.addFilter(RequestIdFilter())
-
-    def __get_arguments(self) -> argparse.Namespace:
-        """Parse command-line arguments and return an argparse Namespace object.
-
-        Returns:
-            argparse.Namespace: Namespace object containing parsed command-line arguments.
-        """
-        parser = argparse.ArgumentParser()
-        parser.add_argument("--jobName", help="Job name identifier")
-        parser.add_argument("--jobId", help="Unique job identifier")
-        parser.add_argument("--extractUrl", help="DataLake extraction URL")
-        parser.add_argument(
-            "--extractPartitions", help="Partitions to extract from DataLake"
-        )
-        parser.add_argument(
-            "--extractRepository", help="DataLake extraction repository"
-        )
-        parser.add_argument("--loadUrl", help="DataLake loading URL")
-        parser.add_argument("--loadRepository", help="DataLake loading repository")
-        parser.add_argument("--inputSchema", nargs="*", help="Input parameters schema")
-        parser.add_argument("--inputArgs", nargs="*", help="Input parameters")
-        return parser.parse_args()
-
-    def __get_reference(self, reference):
-        return self.__getattribute__(reference)
-
-    def extract(self, extractor: Extract):
-        """Execute data extraction operation using the specified Extract object.
-
-        Parameters:
-            extractor (Extract): A Extract object to use for data extraction.
-
-        Returns:
-            ETL: Self-reference to ETL object.
-        """
-        try:
-            logger.info("Starting %s extraction..", extractor.reference.upper())
-
-            logger.info("Executing..")
-
-            setattr(
-                self,
-                *extractor.execute(
-                    platform=self.platform,
-                    repository=self.repository,
-                    partition=self.partition,
-                    args=self.args,
-                ),
-            )
-
-            logger.info("Extraction completed!")
-        except Exception as e:
-            logger.error("Failed in %s: %s", extractor.reference.upper(), e)
-            raise
-
-        return self
-
-    def __get_transform(self, transformer):
-        """Create a new instance of the specified transformer object and inject data into its attributes.
-
-        Parameters:
-            transformer: Transformer object to use for data transformation.
-
-        Returns:
-            Transformer object with data injected into its attributes.
-        """
-        if type(transformer) is not Builder:
-            return transformer.setDf(self.__getattribute__(transformer.reference))
-
-        model = transformer()
-        attributes = [
-            attribute for attribute in dir(model) if not attribute.startswith("_")
-        ]
-        setters_attributes = [
-            attribute for attribute in attributes if callable(getattr(model, attribute))
-        ]
-        non_setters_attributes = {
-            f'set{attribute.replace("_", " ").title().replace(" ", "")}': attribute
-            for attribute in attributes
-            if not callable(getattr(model, attribute))
-        }
-        transformer_objects = [
-            non_setters_attributes[attribute]
-            for attribute in setters_attributes
-            if attribute in non_setters_attributes
-        ]
-        logger.info("Starting %s transformation..", transformer.instance)
-
-        logger.info("Injecting data..")
-
-        for transformer_object in transformer_objects:
-            if (
-                not transformer_object.startswith("_")
-                and transformer_object != "execute"
-                and not transformer_object.startswith("set_")
-            ):
-                try:
-                    attribute = self.__getattribute__(transformer_object)
-                    transformer_setter = (
-                        transformer_object.replace("_", " ").title().replace(" ", "")
-                    )
-                    transformer = model.__getattribute__(f"set{transformer_setter}")(
-                        attribute
-                    )
-
-                except Exception as e:
-                    logger.error("Failed in %s: %s", transformer, e)
-                    raise
-
-        logger.info("Data injection completed")
-
-        return model
-
-    def transform(self, transformer: Transform):
-        """Transforms the data using the given transformer object.
-
-        Parameters:
-            transformer (Transform): A Transform object representing the transformation process.
-
-        Returns:
-            ETL: Self-reference to ETL object.
-        """
-        try:
-            transformer = self.__get_transform(transformer)
-
-            logger.info("Executing..")
-
-            setattr(self.__class__, *transformer.execute())
-
-            logger.info("Transformation completed!")
-        except Exception as e:
-            logger.error("Failed in %s: %s", transformer, e)
-            raise
-
-        return self
-
-    def validate(self, validator: Validate):
-        try:
-            logger.info("Starting %s validation..", validator.reference.upper())
-
-            validator.setDf(self.__getattribute__(validator.reference))
-
-            logger.info("Executing..")
-
-            setattr(
-                self.__class__,
-                *validator.execute(
-                    platform=self.platform, hook_reference=self.__get_reference
-                ),
-            )
-            self.platform.session.sparkContext._gateway.shutdown_callback_server()
-
-            df = self.__getattribute__(validator.output)
-
-            df.show(n=df.count(), truncate=False, vertical=False)
-
-            if df.isEmpty():
-                raise RuntimeError("Validator object has no validations")
-
-            if not df.filter(col("constraint_status").isin("Failure")).isEmpty():
-                raise RuntimeError("Validation failed with errors")
-
-            logger.info("Validation completed!")
-
-        except RuntimeError as e:
-            logger.error("Failed in %s: %s", validator.reference.upper(), e)
-            raise
-
-        except Exception as e:
-            self.platform.session.sparkContext._gateway.shutdown_callback_server()
-            logger.error("Failed in %s: %s", validator.reference.upper(), e)
-            raise
-
-        return self
-
-    def load(self, loader: Load):
-        """Loads the data using the given loader object.
-
-        Parameters:
-            loader (Load): A Load object representing the data loading process.
-
-        Returns:
-            ETL: Self-reference to ETL object.
-        """
-        try:
-            logger.info("Starting %s loading..", loader.reference.upper())
-
-            loader.__setattr__("df_writer", self.__getattribute__(loader.reference))
-
-            logger.info("Executing..")
-
-            setattr(
-                self.__class__,
-                *loader.execute(
-                    platform=self.platform,
-                    repository=self.repository,
-                    args=self.args,
-                ),
-            )
-
-            logger.info("Loading completed!")
-        except Exception as e:
-            logger.error("Failed in %s: %s", loader.reference.upper(), e)
-            raise
-
-        return self
-
-    def stop(self):
-        """Stops the platform session."""
-
-        if hasattr(self.platform, "close_session"):
-            logger.info("Stopping %s session...", type(self.platform).__name__)
-            self.platform.close_session()
-            logger.info("%s session stopped!", type(self.platform).__name__)
-        else:
-            logger.warning(
-                "%s has no session to be stopped.", type(self.platform).__name__
-            )
-
-        logger.info("Execution ended!")
-        sys.exit(0)
+import argparse
+import re
+import sys
+from typing import List
+
+from pyspark.sql.functions import col
+
+from sefazetllib.Builder import Builder, field
+from sefazetllib.config.CustomLogging import RequestIdFilter, logger
+from sefazetllib.extract.Extract import Extract
+from sefazetllib.factory.platform.dataframe.Default import Default
+from sefazetllib.factory.platform.Platform import Platform
+from sefazetllib.load.Load import Load
+from sefazetllib.transform.Transform import Transform
+from sefazetllib.validate.Validate import Validate
+
+
+@Builder
+class ETL:
+    """
+    ETL class for executing data extraction, transformation, and loading operations.
+    """
+
+    platform: Platform = field(default_factory=Default)
+    partition: List = field(default_factory=list)
+    repository: str = field(default="")
+
+    def setup(self) -> None:
+        """
+        Parse command-line arguments and store them in self.args.
+        """
+        self.args = self.__get_arguments()
+        # logger.addFilter(RequestIdFilter(self.args.jobName, self.args.jobId))
+        logger.addFilter(RequestIdFilter())
+
+    def __get_arguments(self) -> argparse.Namespace:
+        """Parse command-line arguments and return an argparse Namespace object.
+
+        Returns:
+            argparse.Namespace: Namespace object containing parsed command-line arguments.
+        """
+        parser = argparse.ArgumentParser()
+        parser.add_argument("--jobName", help="Job name identifier")
+        parser.add_argument("--jobId", help="Unique job identifier")
+        parser.add_argument("--extractUrl", help="DataLake extraction URL")
+        parser.add_argument(
+            "--extractPartitions", help="Partitions to extract from DataLake"
+        )
+        parser.add_argument(
+            "--extractRepository", help="DataLake extraction repository"
+        )
+        parser.add_argument("--loadUrl", help="DataLake loading URL")
+        parser.add_argument("--loadRepository", help="DataLake loading repository")
+        parser.add_argument("--inputSchema", nargs="*", help="Input parameters schema")
+        parser.add_argument("--inputArgs", nargs="*", help="Input parameters")
+        return parser.parse_args()
+
+    def __get_reference(self, reference):
+        return self.__getattribute__(reference)
+
+    def extract(self, extractor: Extract):
+        """Execute data extraction operation using the specified Extract object.
+
+        Parameters:
+            extractor (Extract): A Extract object to use for data extraction.
+
+        Returns:
+            ETL: Self-reference to ETL object.
+        """
+        try:
+            logger.info("Starting %s extraction..", extractor.reference.upper())
+
+            logger.info("Executing..")
+
+            setattr(
+                self,
+                *extractor.execute(
+                    platform=self.platform,
+                    repository=self.repository,
+                    partition=self.partition,
+                    args=self.args,
+                ),
+            )
+
+            logger.info("Extraction completed!")
+        except Exception as e:
+            logger.error("Failed in %s: %s", extractor.reference.upper(), e)
+            raise
+
+        return self
+
+    def __get_transform(self, transformer):
+        """Create a new instance of the specified transformer object and inject data into its attributes.
+
+        Parameters:
+            transformer: Transformer object to use for data transformation.
+
+        Returns:
+            Transformer object with data injected into its attributes.
+        """
+        if type(transformer) is not Builder:
+            return transformer.setDf(self.__getattribute__(transformer.reference))
+
+        model = transformer()
+        attributes = [
+            attribute for attribute in dir(model) if not attribute.startswith("_")
+        ]
+        setters_attributes = [
+            attribute for attribute in attributes if callable(getattr(model, attribute))
+        ]
+        non_setters_attributes = {
+            f'set{attribute.replace("_", " ").title().replace(" ", "")}': attribute
+            for attribute in attributes
+            if not callable(getattr(model, attribute))
+        }
+        transformer_objects = [
+            non_setters_attributes[attribute]
+            for attribute in setters_attributes
+            if attribute in non_setters_attributes
+        ]
+        logger.info("Starting %s transformation..", transformer.instance)
+
+        logger.info("Injecting data..")
+
+        for transformer_object in transformer_objects:
+            if (
+                not transformer_object.startswith("_")
+                and transformer_object != "execute"
+                and not transformer_object.startswith("set_")
+            ):
+                try:
+                    attribute = self.__getattribute__(transformer_object)
+                    transformer_setter = (
+                        transformer_object.replace("_", " ").title().replace(" ", "")
+                    )
+                    transformer = model.__getattribute__(f"set{transformer_setter}")(
+                        attribute
+                    )
+
+                except Exception as e:
+                    logger.error("Failed in %s: %s", transformer, e)
+                    raise
+
+        logger.info("Data injection completed")
+
+        return model
+
+    def transform(self, transformer: Transform):
+        """Transforms the data using the given transformer object.
+
+        Parameters:
+            transformer (Transform): A Transform object representing the transformation process.
+
+        Returns:
+            ETL: Self-reference to ETL object.
+        """
+        try:
+            transformer = self.__get_transform(transformer)
+
+            logger.info("Executing..")
+
+            setattr(self.__class__, *transformer.execute())
+
+            logger.info("Transformation completed!")
+        except Exception as e:
+            logger.error("Failed in %s: %s", transformer, e)
+            raise
+
+        return self
+
+    def validate(self, validator: Validate):
+        try:
+            logger.info("Starting %s validation..", validator.reference.upper())
+
+            validator.setDf(self.__getattribute__(validator.reference))
+
+            logger.info("Executing..")
+
+            setattr(
+                self.__class__,
+                *validator.execute(
+                    platform=self.platform, hook_reference=self.__get_reference
+                ),
+            )
+            self.platform.session.sparkContext._gateway.shutdown_callback_server()
+
+            df = self.__getattribute__(validator.output)
+
+            df.show(n=df.count(), truncate=False, vertical=False)
+
+            if df.isEmpty():
+                raise RuntimeError("Validator object has no validations")
+
+            if not df.filter(col("constraint_status").isin("Failure")).isEmpty():
+                raise RuntimeError("Validation failed with errors")
+
+            logger.info("Validation completed!")
+
+        except RuntimeError as e:
+            logger.error("Failed in %s: %s", validator.reference.upper(), e)
+            raise
+
+        except Exception as e:
+            self.platform.session.sparkContext._gateway.shutdown_callback_server()
+            logger.error("Failed in %s: %s", validator.reference.upper(), e)
+            raise
+
+        return self
+
+    def load(self, loader: Load):
+        """Loads the data using the given loader object.
+
+        Parameters:
+            loader (Load): A Load object representing the data loading process.
+
+        Returns:
+            ETL: Self-reference to ETL object.
+        """
+        try:
+            logger.info("Starting %s loading..", loader.reference.upper())
+
+            loader.__setattr__("df_writer", self.__getattribute__(loader.reference))
+
+            logger.info("Executing..")
+
+            setattr(
+                self.__class__,
+                *loader.execute(
+                    platform=self.platform,
+                    repository=self.repository,
+                    args=self.args,
+                ),
+            )
+
+            logger.info("Loading completed!")
+        except Exception as e:
+            logger.error("Failed in %s: %s", loader.reference.upper(), e)
+            raise
+
+        return self
+
+    def stop(self):
+        """Stops the platform session."""
+
+        if hasattr(self.platform, "close_session"):
+            logger.info("Stopping %s session...", type(self.platform).__name__)
+            self.platform.close_session()
+            logger.info("%s session stopped!", type(self.platform).__name__)
+        else:
+            logger.warning(
+                "%s has no session to be stopped.", type(self.platform).__name__
+            )
+
+        logger.info("Execution ended!")
+        sys.exit(0)
```

### Comparing `sefazetllib-0.1.55/sefazetllib/extract/ExtractLocal.py` & `sefazetllib-0.1.56/sefazetllib/extract/ExtractS3.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,79 @@
-from typing import Any, Dict, List
-
-from sefazetllib.Builder import Builder, field
-from sefazetllib.extract.Extract import Extract
-from sefazetllib.factory.platform.dataframe.Default import Default
-from sefazetllib.factory.platform.Platform import Platform
-
-
-@Builder
-class ExtractLocal(Extract):
-    platform: Platform = field(default_factory=Default)
-    file_format: str = field(default="")
-    format_properties: Dict[str, Any] = field(default_factory=dict)
-    repository: str = field(default="")
-    url: str = field(default="")
-    partition: List[str] = field(default_factory=list)
-    reference: str = field(default="")
-    columns: List = field(default_factory=list)
-    duplicates: bool = field(default=False)
-    optional: bool = field(default=False)
-
-    def build_connection_string(self):
-        if self.partition != []:
-            for partition in self.partition:
-                self.setUrl(f"{self.url}/{partition}")
-
-        return self.url
-
-    def execute(self, **kwargs):
-        if isinstance(self.platform, Default):
-            self.setPlatform(kwargs["platform"])
-
-        if self.repository == "":
-            self.setRepository(kwargs["repository"])
-
-        url = self.build_connection_string()
-
-        if kwargs:
-            args = kwargs["args"]
-            if args.extractRepository:
-                self.setRepository(args.extractRepository)
-
-            if args.extractPartitions:
-                self.setPartition(args.extractPartitions)
-
-            if args.extractUrl:
-                url = args.extractUrl
-
-        return (
-            self.reference,
-            self.platform.read(
-                file_format=self.file_format,
-                format_properties=self.format_properties,
-                repository=self.repository,
-                url=url,
-                reference=self.reference,
-                columns=self.columns,
-                duplicates=self.duplicates,
-                optional=self.optional,
-            ),
-        )
+import warnings
+from typing import Any, Dict, List
+from itertools import product
+
+from sefazetllib.Builder import Builder, field
+from sefazetllib.extract.Extract import Extract
+from sefazetllib.factory.platform.dataframe.Default import Default
+from sefazetllib.factory.platform.Platform import Platform
+
+
+@Builder
+class ExtractS3(Extract):
+    warnings.warn(
+        "The 'ExtractS3' class is deprecated. Please use the 'ExtractStorage' class with the protocol parameter (e.g., 's3a')."
+    )
+    platform: Platform = field(default=Default())
+    file_format: str = field(default="")
+    format_properties: Dict[str, Any] = field(default_factory=dict)
+    repository: str = field(default="")
+    layer: str = field(default="")
+    schema: str = field(default="")
+    entity: str = field(default="")
+    url: str = field(default="")
+    partition: List[str] = field(default_factory=list)
+    etl_partition: bool = field(default=False)
+    reference: str = field(default="")
+    duplicates: bool = field(default=False)
+    columns: List[str] = field(default_factory=list)
+    optional: bool = field(default=False)
+    partition_delimiter: str = field(default="/")
+
+    def build_connection_string(self):
+        self.url = f"s3a://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
+
+        if self.partition != []:
+            try:
+                partition = self.partition_delimiter.join(self.partition.get())
+            except AttributeError:
+                partition = self.partition_delimiter.join(self.partition)
+
+            self.setUrl(f"{self.url}/{partition}")
+
+        return self.url
+
+    def execute(self, **kwargs):
+        if isinstance(self.platform, Default):
+            self.setPlatform(kwargs["platform"])
+
+        local_repository = self.repository
+        if local_repository == "":
+            self.setRepository(kwargs["repository"])
+
+        if self.etl_partition:
+            self.setPartition(kwargs["partition"])
+
+        if kwargs:
+            args = kwargs["args"]
+            if args.extractRepository and local_repository == "":
+                self.setRepository(args.extractRepository)
+
+            if args.extractPartitions:
+                self.setPartition(args.extractPartitions)
+
+            if args.extractUrl:
+                url = args.extractUrl
+
+        url = self.build_connection_string()
+
+        return (
+            self.reference,
+            self.platform.read(
+                file_format=self.file_format,
+                format_properties=self.format_properties,
+                url=url,
+                duplicates=self.duplicates,
+                columns=self.columns,
+                optional=self.optional,
+            ),
+        )
```

### Comparing `sefazetllib-0.1.55/sefazetllib/extract/ExtractS3.py` & `sefazetllib-0.1.56/sefazetllib/extract/ExtractStorage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,79 +1,69 @@
-import warnings
-from typing import Any, Dict, List
-from itertools import product
-
-from sefazetllib.Builder import Builder, field
-from sefazetllib.extract.Extract import Extract
-from sefazetllib.factory.platform.dataframe.Default import Default
-from sefazetllib.factory.platform.Platform import Platform
-
-
-@Builder
-class ExtractS3(Extract):
-    warnings.warn(
-        "The 'ExtractS3' class is deprecated. Please use the 'ExtractStorage' class with the protocol parameter (e.g., 's3a')."
-    )
-    platform: Platform = field(default=Default())
-    file_format: str = field(default="")
-    format_properties: Dict[str, Any] = field(default_factory=dict)
-    repository: str = field(default="")
-    layer: str = field(default="")
-    schema: str = field(default="")
-    entity: str = field(default="")
-    url: str = field(default="")
-    partition: List[str] = field(default_factory=list)
-    etl_partition: bool = field(default=False)
-    reference: str = field(default="")
-    duplicates: bool = field(default=False)
-    columns: List[str] = field(default_factory=list)
-    optional: bool = field(default=False)
-    partition_delimiter: str = field(default="/")
-
-    def build_connection_string(self):
-        self.url = f"s3a://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
-
-        if self.partition != []:
-            try:
-                partition = self.partition_delimiter.join(self.partition.get())
-            except AttributeError:
-                partition = self.partition_delimiter.join(self.partition)
-
-            self.setUrl(f"{self.url}/{partition}")
-
-        return self.url
-
-    def execute(self, **kwargs):
-        if isinstance(self.platform, Default):
-            self.setPlatform(kwargs["platform"])
-
-        local_repository = self.repository
-        if local_repository == "":
-            self.setRepository(kwargs["repository"])
-
-        if self.etl_partition:
-            self.setPartition(kwargs["partition"])
-
-        if kwargs:
-            args = kwargs["args"]
-            if args.extractRepository and local_repository == "":
-                self.setRepository(args.extractRepository)
-
-            if args.extractPartitions:
-                self.setPartition(args.extractPartitions)
-
-            if args.extractUrl:
-                url = args.extractUrl
-
-        url = self.build_connection_string()
-
-        return (
-            self.reference,
-            self.platform.read(
-                file_format=self.file_format,
-                format_properties=self.format_properties,
-                url=url,
-                duplicates=self.duplicates,
-                columns=self.columns,
-                optional=self.optional,
-            ),
-        )
+from typing import Any, Dict, List
+
+from sefazetllib.Builder import Builder, field
+from sefazetllib.extract.Extract import Extract
+from sefazetllib.factory.platform.dataframe.Default import Default
+from sefazetllib.factory.platform.Platform import Platform
+
+
+@Builder
+class ExtractStorage(Extract):
+    platform: Platform = field(default=Default())
+    file_format: str = field(default="")
+    format_properties: Dict[str, Any] = field(default_factory=dict)
+    repository: str = field(default="")
+    layer: str = field(default="")
+    schema: str = field(default="")
+    entity: str = field(default="")
+    url: str = field(default="")
+    partition: List[str] = field(default_factory=list)
+    etl_partition: bool = field(default=False)
+    reference: str = field(default="")
+    duplicates: bool = field(default=False)
+    columns: List[str] = field(default_factory=list)
+    optional: bool = field(default=False)
+    protocol: str = field(default="")
+
+    def build_connection_string(self):
+        self.url = f"{self.protocol}://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
+
+        if self.partition != []:
+            for partition in self.partition:
+                self.setUrl(f"{self.url}/{partition}")
+
+        return self.url
+
+    def execute(self, **kwargs):
+        if isinstance(self.platform, Default):
+            self.setPlatform(kwargs["platform"])
+
+        if self.repository == "":
+            self.setRepository(kwargs["repository"])
+
+        if self.etl_partition:
+            self.setPartition(kwargs["partition"].get())
+
+        url = self.build_connection_string()
+
+        if kwargs:
+            args = kwargs["args"]
+            if args.extractRepository:
+                self.setRepository(args.extractRepository)
+
+            if args.extractPartitions:
+                self.setPartition(args.extractPartitions)
+
+            if args.extractUrl:
+                url = args.extractUrl
+
+        return (
+            self.reference,
+            self.platform.read(
+                file_format=self.file_format,
+                format_properties=self.format_properties,
+                url=url,
+                duplicates=self.duplicates,
+                columns=self.columns,
+                optional=self.optional,
+            ),
+        )
```

### Comparing `sefazetllib-0.1.55/sefazetllib/extract/ExtractStorage.py` & `sefazetllib-0.1.56/sefazetllib/extract/ExtractSQL.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,79 @@
-from typing import Any, Dict, List
-
-from sefazetllib.Builder import Builder, field
-from sefazetllib.extract.Extract import Extract
-from sefazetllib.factory.platform.dataframe.Default import Default
-from sefazetllib.factory.platform.Platform import Platform
-
-
-@Builder
-class ExtractStorage(Extract):
-    platform: Platform = field(default=Default())
-    file_format: str = field(default="")
-    format_properties: Dict[str, Any] = field(default_factory=dict)
-    repository: str = field(default="")
-    layer: str = field(default="")
-    schema: str = field(default="")
-    entity: str = field(default="")
-    url: str = field(default="")
-    partition: List[str] = field(default_factory=list)
-    etl_partition: bool = field(default=False)
-    reference: str = field(default="")
-    duplicates: bool = field(default=False)
-    columns: List[str] = field(default_factory=list)
-    optional: bool = field(default=False)
-    protocol: str = field(default="")
-
-    def build_connection_string(self):
-        self.url = f"{self.protocol}://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
-
-        if self.partition != []:
-            for partition in self.partition:
-                self.setUrl(f"{self.url}/{partition}")
-
-        return self.url
-
-    def execute(self, **kwargs):
-        if isinstance(self.platform, Default):
-            self.setPlatform(kwargs["platform"])
-
-        if self.repository == "":
-            self.setRepository(kwargs["repository"])
-
-        if self.etl_partition:
-            self.setPartition(kwargs["partition"].get())
-
-        url = self.build_connection_string()
-
-        if kwargs:
-            args = kwargs["args"]
-            if args.extractRepository:
-                self.setRepository(args.extractRepository)
-
-            if args.extractPartitions:
-                self.setPartition(args.extractPartitions)
-
-            if args.extractUrl:
-                url = args.extractUrl
-
-        return (
-            self.reference,
-            self.platform.read(
-                file_format=self.file_format,
-                format_properties=self.format_properties,
-                url=url,
-                duplicates=self.duplicates,
-                columns=self.columns,
-                optional=self.optional,
-            ),
-        )
+from typing import Any, Dict, List
+
+from sefazetllib.Builder import Builder, field
+from sefazetllib.extract.Extract import Extract
+from sefazetllib.factory.platform.dataframe.Default import Default
+from sefazetllib.factory.platform.Platform import Platform
+from sefazetllib.factory.platform.PlatformFactory import PlatformFactory
+
+
+@Builder
+class ExtractSQL(Extract):
+    platform: Platform = field(default=Default())
+    format: str = field(default="jdbc")
+    operator: str = field(default=":")
+    host: str = field(default="")
+    port: int = field(default=0)
+    database: str = field(default="")
+    instance: str = field(default="")
+    driver: str = field(default="")
+    schema: str = field(default="")
+    table: str = field(default="")
+    authentication: Dict[str, Any] = field(default_factory=dict)
+    url: str = field(default="")
+    reference: str = field(default="")
+    columns: List[str] = field(default_factory=list)
+    optional: bool = field(default=False)
+    duplicates: bool = field(default=False)
+
+    def __build_properties(self):
+        self.properties = {
+            "database": self.database,
+            "driver": self.driver,
+            "user": self.authentication["user"],
+            "password": self.authentication["password"],
+            "dbtable": self.table,
+            "url": self.url,
+        }
+
+        return self.properties
+
+    def build_connection_string(self):
+        platform_db = PlatformFactory(self.database).create(
+            name="get url jdbc",
+        )
+        self.url = platform_db.get_url(
+            format=self.format,
+            operator=self.operator,
+            database=self.database,
+            host=self.host,
+            instance=self.instance,
+            schema=self.schema,
+            port=self.port,
+        )
+
+        self.table = platform_db.get_table_name(table=self.table, schema=self.schema)
+
+        return self.url
+
+    def execute(self, **kwargs):
+        if isinstance(self.platform, Default):
+            self.setPlatform(kwargs["platform"])
+
+        url = self.build_connection_string()
+        properties = self.__build_properties()
+
+        if kwargs:
+            args = kwargs["args"]
+
+            if args.extractUrl:
+                url = args.extractUrl
+
+        return self.reference, self.platform.read(
+            format=self.format,
+            url=url,
+            format_properties=properties,
+            optional=self.optional,
+            columns=self.columns,
+            duplicates=self.duplicates,
+        )
```

### Comparing `sefazetllib-0.1.55/sefazetllib/factory/Factory.py` & `sefazetllib-0.1.56/sefazetllib/factory/Factory.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from abc import ABC, abstractmethod
-
-
-class Creator(ABC):
-    """The Creator class declares the factory method that is supposed to return an object of a Platform class. The Creator's subclasses usually provide the implementation of this method."""
-
-    @abstractmethod
-    def factory_method(self):
-        """Note that the Creator may also provide some default implementation of the factory method."""
-        pass
-
-    def execute(self, **kwargs):
-        """Also note that, despite its name, the Creator's primary responsibility is not creating products. Usually, it contains some core business logic that relies on Platform objects, returned by the factory method.  Subclasses can indirectly change that business logic by overriding the factory method and returning a different type of product from it.
-
-        Parameters:
-            **kwargs: Keyword arguments for the execute method.
-        """
-        return self.factory_method(**kwargs)
+from abc import ABC, abstractmethod
+
+
+class Creator(ABC):
+    """The Creator class declares the factory method that is supposed to return an object of a Platform class. The Creator's subclasses usually provide the implementation of this method."""
+
+    @abstractmethod
+    def factory_method(self):
+        """Note that the Creator may also provide some default implementation of the factory method."""
+        pass
+
+    def execute(self, **kwargs):
+        """Also note that, despite its name, the Creator's primary responsibility is not creating products. Usually, it contains some core business logic that relies on Platform objects, returned by the factory method.  Subclasses can indirectly change that business logic by overriding the factory method and returning a different type of product from it.
+
+        Parameters:
+            **kwargs: Keyword arguments for the execute method.
+        """
+        return self.factory_method(**kwargs)
```

### Comparing `sefazetllib-0.1.55/sefazetllib/factory/platform/PlatformFactory.py` & `sefazetllib-0.1.56/sefazetllib/factory/platform/PlatformFactory.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from sefazetllib.factory.Factory import Creator
-from sefazetllib.factory.platform.database import MySQL, PostgreSQL
-from sefazetllib.factory.platform.dataframe import Default, Pandas, Spark
-
-
-class PlatformFactory(Creator):
-    """
-    Note that the signature of the method still uses the abstract product type,
-    even though the concrete product is actually returned from the method. This
-    way the Creator can stay independent of concrete product classes.
-    """
-
-    def __init__(self, platform) -> None:
-        self.platform = platform
-
-    def create(self, **kwargs):
-        """
-        The client code works with an instance of a concrete creator, albeit through
-        its base interface. As long as the client keeps working with the creator via
-        the base interface, you can pass it any creator's subclass.
-        """
-        return self.execute(**kwargs)
-
-    def factory_method(self, **kwargs):
-        try:
-            return globals()[self.platform](**kwargs)
-        except KeyError:
-            return Default(**kwargs)
+from sefazetllib.factory.Factory import Creator
+from sefazetllib.factory.platform.database import MySQL, PostgreSQL
+from sefazetllib.factory.platform.dataframe import Default, Pandas, Spark
+
+
+class PlatformFactory(Creator):
+    """
+    Note that the signature of the method still uses the abstract product type,
+    even though the concrete product is actually returned from the method. This
+    way the Creator can stay independent of concrete product classes.
+    """
+
+    def __init__(self, platform) -> None:
+        self.platform = platform
+
+    def create(self, **kwargs):
+        """
+        The client code works with an instance of a concrete creator, albeit through
+        its base interface. As long as the client keeps working with the creator via
+        the base interface, you can pass it any creator's subclass.
+        """
+        return self.execute(**kwargs)
+
+    def factory_method(self, **kwargs):
+        try:
+            return globals()[self.platform](**kwargs)
+        except KeyError:
+            return Default(**kwargs)
```

### Comparing `sefazetllib-0.1.55/sefazetllib/factory/platform/database/MySQL.py` & `sefazetllib-0.1.56/sefazetllib/factory/platform/database/MySQL.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from sefazetllib.factory.platform.DatabasePlatform import DatabasePlatform
-
-
-class MySQL(DatabasePlatform):
-    def __init__(self, name="MySQL Job", configs=[]) -> None:
-        self.name = name
-        self.session = None
-
-    def get_url(self, **kwargs):
-        host = kwargs["host"]
-        format = kwargs["format"]
-        operator = kwargs["operator"]
-        database = kwargs["database"].lower()
-        port = kwargs["port"]
-        schema = kwargs["schema"]
-        return f"{format}{operator}{database}://{host}:{port}/{schema}"
-
-    def get_table_name(self, **kwargs):
-        table = kwargs["table"]
-        return table
-
-    def read(self, **kwargs):
-        pass
-
-    def load(self, **kwargs):
-        pass
+from sefazetllib.factory.platform.DatabasePlatform import DatabasePlatform
+
+
+class MySQL(DatabasePlatform):
+    def __init__(self, name="MySQL Job", configs=[]) -> None:
+        self.name = name
+        self.session = None
+
+    def get_url(self, **kwargs):
+        host = kwargs["host"]
+        format = kwargs["format"]
+        operator = kwargs["operator"]
+        database = kwargs["database"].lower()
+        port = kwargs["port"]
+        schema = kwargs["schema"]
+        return f"{format}{operator}{database}://{host}:{port}/{schema}"
+
+    def get_table_name(self, **kwargs):
+        table = kwargs["table"]
+        return table
+
+    def read(self, **kwargs):
+        pass
+
+    def load(self, **kwargs):
+        pass
```

### Comparing `sefazetllib-0.1.55/sefazetllib/factory/platform/database/PostgreSQL.py` & `sefazetllib-0.1.56/sefazetllib/factory/platform/database/PostgreSQL.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,249 +1,249 @@
-from sefazetllib.factory.platform.DatabasePlatform import DatabasePlatform
-from sqlalchemy import create_engine, text
-
-
-class PostgreSQL(DatabasePlatform):
-    def __init__(self, name="PostgreSQL Job", configs=[]) -> None:
-        self.name = name
-        self.session = None
-        self.conn = None
-        self.transaction = None
-
-        if configs != []:
-            url_args = configs
-            if not isinstance(configs, dict):
-                url_args = {config[0]: config[1] for config in configs}
-
-            self.session = create_engine(
-                f"postgresql+psycopg2://"
-                f'{url_args["user"]}:{url_args["password"]}@{url_args["host"]}:'
-                f'{url_args["port"]}/'
-                f'{url_args["instance"]}'
-            )
-            self.create_connection()
-
-    def get_url(self, **kwargs):
-        host = kwargs["host"]
-        port = kwargs["port"]
-        file_format = kwargs["file_format"]
-        operator = kwargs["operator"]
-        database = kwargs["database"].lower()
-        instance = kwargs["instance"]
-        return f"{file_format}{operator}{database}://{host}:{port}/{instance}"
-
-    def get_table_name(self, **kwargs):
-        schema = kwargs["schema"]
-        table = kwargs["table"]
-        return f"{schema}.{table}"
-
-    def create_connection(self):
-        self.conn = self.session.connect()
-        return
-
-    def close_connection(self):
-        self.conn.close()
-        return
-
-    def begin_transaction(self):
-        self.transaction = self.conn.begin()
-        return
-
-    def create_commit(self):
-        if self.transaction is not None:
-            self.transaction.commit()
-        return
-
-    def rollback(self):
-        if self.transaction is not None:
-            self.transaction.rollback()
-        return
-
-    def truncate(self, **kwargs):
-        schema = kwargs["schema"].lower()
-        table = kwargs["table"].lower()
-        self.conn.execute(text(f"TRUNCATE TABLE {schema}.{table}"))
-        return
-
-    def drop_constraints(self, **kwargs):
-        table = kwargs["table"].lower()
-        schema = kwargs["schema"].lower()
-        dependencies = [
-            row._asdict()
-            for row in self.conn.execute(
-                text(
-                    f"""
-        SELECT tc.table_schema,
-            tc.constraint_name,
-            tc.table_name,
-            kcu.column_name,
-            ccu.table_schema AS foreign_table_schema,
-            ccu.table_name AS foreign_table_name,
-            ccu.column_name AS foreign_column_name
-        FROM information_schema.table_constraints AS tc
-            JOIN information_schema.key_column_usage AS kcu ON tc.constraint_name = kcu.constraint_name
-            AND tc.table_schema = kcu.table_schema
-            JOIN information_schema.constraint_column_usage AS ccu ON ccu.constraint_name = tc.constraint_name
-        WHERE tc.constraint_type = 'FOREIGN KEY'
-            AND (tc.table_name = '{table}' OR ccu.table_name = '{table}')
-            AND (tc.table_schema = '{schema}' OR ccu.table_schema = '{schema}')
-        """
-                )
-            ).fetchall()
-        ]
-
-        alter_queries = [
-            f"""ALTER TABLE {dependencie['table_schema']}.{dependencie['table_name']} DROP CONSTRAINT {dependencie['constraint_name']};"""
-            for dependencie in dependencies
-        ]
-        if bool(alter_queries):
-            self.conn.execute(text("\n".join(alter_queries)))
-        return dependencies
-
-    def create_constraints(self, **kwargs):
-        dependencies = kwargs["dependencies"]
-
-        alter_queries = [
-            f"""ALTER TABLE {dependencie['table_schema']}.{dependencie['table_name']} ADD CONSTRAINT {dependencie['constraint_name']} FOREIGN KEY ({dependencie['column_name']}) REFERENCES {dependencie['foreign_table_schema']}.{dependencie['foreign_table_name']}({dependencie['foreign_column_name']});"""
-            for dependencie in dependencies
-        ]
-        if bool(alter_queries):
-            self.conn.execute(text("\n".join(alter_queries)))
-        return
-
-    def merge_temporary_table_with_conflict(self, **kwargs):
-        schema = kwargs["schema"].lower()
-        table = kwargs["table"].lower()
-        temporary_schema = kwargs["temporary_schema"].lower()
-        temporary_table = kwargs["temporary_table"].lower()
-        columns = kwargs["columns"]
-        sk_name = kwargs["sk_name"]
-
-        try:
-            self.begin_transaction()
-            self.conn.execute(
-                text(
-                    f"""
-                INSERT INTO {schema}.{table} ({",".join(columns)})
-                    SELECT {",".join(columns)}
-                    FROM {temporary_schema}.{temporary_table} 
-                        ON CONFLICT ({sk_name})
-                        DO UPDATE SET
-                        {",".join([f"{col}=EXCLUDED.{col}" for col in columns])};
-            """
-                )
-            )
-
-        except Exception as err:
-            self.rollback()
-            raise Exception(str(err))
-
-        else:
-            self.create_commit()
-        return
-
-    def insert_from_temporary_table(self, **kwargs):
-        schema = kwargs["schema"].lower()
-        table = kwargs["table"].lower()
-        temporary_schema = kwargs["temporary_schema"].lower()
-        temporary_table = kwargs["temporary_table"].lower()
-        columns = kwargs["columns"]
-
-        try:
-            self.begin_transaction()
-            self.conn.execute(
-                text(
-                    f"""
-                INSERT INTO {schema}.{table} ({",".join(columns)})
-                    SELECT {",".join(columns)}
-                    FROM {temporary_schema}.{temporary_table} 
-            """
-                )
-            )
-
-        except Exception as err:
-            self.rollback()
-            raise Exception(str(err))
-
-        else:
-            self.create_commit()
-
-        return
-
-    def delete_insert_from_temporary_table(self, **kwargs):
-        schema = kwargs["schema"].lower()
-        table = kwargs["table"].lower()
-        temporary_schema = kwargs["temporary_schema"].lower()
-        temporary_table = kwargs["temporary_table"].lower()
-        columns = kwargs["columns"]
-        sk_name = kwargs["sk_name"]
-
-        try:
-            self.begin_transaction()
-            self.conn.execute(
-                text(
-                    f"""
-                    DELETE FROM {schema}.{table} as tb1
-                    USING {temporary_schema}.{temporary_table} as tb2
-                    WHERE tb1.{sk_name} = tb2.{sk_name};      
-                    """
-                )
-            )
-            self.conn.execute(
-                text(
-                    f"""
-                    INSERT INTO {schema}.{table} ({",".join(columns)})
-                        SELECT {",".join(columns)}
-                        FROM {temporary_schema}.{temporary_table} 
-                """
-                )
-            )
-
-        except Exception as err:
-            self.rollback()
-            raise Exception(str(err))
-
-        else:
-            self.create_commit()
-
-        return
-
-    def delete_matched_temporary_table(self, **kwargs):
-        schema = kwargs["schema"].lower()
-        table = kwargs["table"].lower()
-        temporary_schema = kwargs["temporary_schema"].lower()
-        temporary_table = kwargs["temporary_table"].lower()
-        sk_name = kwargs["sk_name"]
-
-        try:
-            self.begin_transaction()
-            self.conn.execute(
-                text(
-                    f"""
-                DELETE FROM {schema}.{table} as tb1
-                USING {temporary_schema}.{temporary_table} as tb2
-                WHERE tb1.{sk_name} = tb2.{sk_name};      
-                """
-                )
-            )
-
-        except Exception as err:
-            self.rollback()
-            raise Exception(str(err))
-
-        else:
-            self.create_commit()
-        return
-
-    def drop_temporary_table(self, **kwargs):
-        temporary_table = kwargs["temporary_table"].lower()
-        temporary_schema = kwargs["temporary_schema"].lower()
-        self.conn.execute(
-            text(f"DROP TABLE IF EXISTS {temporary_schema}.{temporary_table}")
-        )
-        return
-
-    def read(self, **kwargs):
-        pass
-
-    def load(self, **kwargs):
-        pass
+from sefazetllib.factory.platform.DatabasePlatform import DatabasePlatform
+from sqlalchemy import create_engine, text
+
+
+class PostgreSQL(DatabasePlatform):
+    def __init__(self, name="PostgreSQL Job", configs=[]) -> None:
+        self.name = name
+        self.session = None
+        self.conn = None
+        self.transaction = None
+
+        if configs != []:
+            url_args = configs
+            if not isinstance(configs, dict):
+                url_args = {config[0]: config[1] for config in configs}
+
+            self.session = create_engine(
+                f"postgresql+psycopg2://"
+                f'{url_args["user"]}:{url_args["password"]}@{url_args["host"]}:'
+                f'{url_args["port"]}/'
+                f'{url_args["instance"]}'
+            )
+            self.create_connection()
+
+    def get_url(self, **kwargs):
+        host = kwargs["host"]
+        port = kwargs["port"]
+        file_format = kwargs["file_format"]
+        operator = kwargs["operator"]
+        database = kwargs["database"].lower()
+        instance = kwargs["instance"]
+        return f"{file_format}{operator}{database}://{host}:{port}/{instance}"
+
+    def get_table_name(self, **kwargs):
+        schema = kwargs["schema"]
+        table = kwargs["table"]
+        return f"{schema}.{table}"
+
+    def create_connection(self):
+        self.conn = self.session.connect()
+        return
+
+    def close_connection(self):
+        self.conn.close()
+        return
+
+    def begin_transaction(self):
+        self.transaction = self.conn.begin()
+        return
+
+    def create_commit(self):
+        if self.transaction is not None:
+            self.transaction.commit()
+        return
+
+    def rollback(self):
+        if self.transaction is not None:
+            self.transaction.rollback()
+        return
+
+    def truncate(self, **kwargs):
+        schema = kwargs["schema"].lower()
+        table = kwargs["table"].lower()
+        self.conn.execute(text(f"TRUNCATE TABLE {schema}.{table}"))
+        return
+
+    def drop_constraints(self, **kwargs):
+        table = kwargs["table"].lower()
+        schema = kwargs["schema"].lower()
+        dependencies = [
+            row._asdict()
+            for row in self.conn.execute(
+                text(
+                    f"""
+        SELECT tc.table_schema,
+            tc.constraint_name,
+            tc.table_name,
+            kcu.column_name,
+            ccu.table_schema AS foreign_table_schema,
+            ccu.table_name AS foreign_table_name,
+            ccu.column_name AS foreign_column_name
+        FROM information_schema.table_constraints AS tc
+            JOIN information_schema.key_column_usage AS kcu ON tc.constraint_name = kcu.constraint_name
+            AND tc.table_schema = kcu.table_schema
+            JOIN information_schema.constraint_column_usage AS ccu ON ccu.constraint_name = tc.constraint_name
+        WHERE tc.constraint_type = 'FOREIGN KEY'
+            AND (tc.table_name = '{table}' OR ccu.table_name = '{table}')
+            AND (tc.table_schema = '{schema}' OR ccu.table_schema = '{schema}')
+        """
+                )
+            ).fetchall()
+        ]
+
+        alter_queries = [
+            f"""ALTER TABLE {dependencie['table_schema']}.{dependencie['table_name']} DROP CONSTRAINT {dependencie['constraint_name']};"""
+            for dependencie in dependencies
+        ]
+        if bool(alter_queries):
+            self.conn.execute(text("\n".join(alter_queries)))
+        return dependencies
+
+    def create_constraints(self, **kwargs):
+        dependencies = kwargs["dependencies"]
+
+        alter_queries = [
+            f"""ALTER TABLE {dependencie['table_schema']}.{dependencie['table_name']} ADD CONSTRAINT {dependencie['constraint_name']} FOREIGN KEY ({dependencie['column_name']}) REFERENCES {dependencie['foreign_table_schema']}.{dependencie['foreign_table_name']}({dependencie['foreign_column_name']});"""
+            for dependencie in dependencies
+        ]
+        if bool(alter_queries):
+            self.conn.execute(text("\n".join(alter_queries)))
+        return
+
+    def merge_temporary_table_with_conflict(self, **kwargs):
+        schema = kwargs["schema"].lower()
+        table = kwargs["table"].lower()
+        temporary_schema = kwargs["temporary_schema"].lower()
+        temporary_table = kwargs["temporary_table"].lower()
+        columns = kwargs["columns"]
+        sk_name = kwargs["sk_name"]
+
+        try:
+            self.begin_transaction()
+            self.conn.execute(
+                text(
+                    f"""
+                INSERT INTO {schema}.{table} ({",".join(columns)})
+                    SELECT {",".join(columns)}
+                    FROM {temporary_schema}.{temporary_table} 
+                        ON CONFLICT ({sk_name})
+                        DO UPDATE SET
+                        {",".join([f"{col}=EXCLUDED.{col}" for col in columns])};
+            """
+                )
+            )
+
+        except Exception as err:
+            self.rollback()
+            raise Exception(str(err))
+
+        else:
+            self.create_commit()
+        return
+
+    def insert_from_temporary_table(self, **kwargs):
+        schema = kwargs["schema"].lower()
+        table = kwargs["table"].lower()
+        temporary_schema = kwargs["temporary_schema"].lower()
+        temporary_table = kwargs["temporary_table"].lower()
+        columns = kwargs["columns"]
+
+        try:
+            self.begin_transaction()
+            self.conn.execute(
+                text(
+                    f"""
+                INSERT INTO {schema}.{table} ({",".join(columns)})
+                    SELECT {",".join(columns)}
+                    FROM {temporary_schema}.{temporary_table} 
+            """
+                )
+            )
+
+        except Exception as err:
+            self.rollback()
+            raise Exception(str(err))
+
+        else:
+            self.create_commit()
+
+        return
+
+    def delete_insert_from_temporary_table(self, **kwargs):
+        schema = kwargs["schema"].lower()
+        table = kwargs["table"].lower()
+        temporary_schema = kwargs["temporary_schema"].lower()
+        temporary_table = kwargs["temporary_table"].lower()
+        columns = kwargs["columns"]
+        sk_name = kwargs["sk_name"]
+
+        try:
+            self.begin_transaction()
+            self.conn.execute(
+                text(
+                    f"""
+                    DELETE FROM {schema}.{table} as tb1
+                    USING {temporary_schema}.{temporary_table} as tb2
+                    WHERE tb1.{sk_name} = tb2.{sk_name};      
+                    """
+                )
+            )
+            self.conn.execute(
+                text(
+                    f"""
+                    INSERT INTO {schema}.{table} ({",".join(columns)})
+                        SELECT {",".join(columns)}
+                        FROM {temporary_schema}.{temporary_table} 
+                """
+                )
+            )
+
+        except Exception as err:
+            self.rollback()
+            raise Exception(str(err))
+
+        else:
+            self.create_commit()
+
+        return
+
+    def delete_matched_temporary_table(self, **kwargs):
+        schema = kwargs["schema"].lower()
+        table = kwargs["table"].lower()
+        temporary_schema = kwargs["temporary_schema"].lower()
+        temporary_table = kwargs["temporary_table"].lower()
+        sk_name = kwargs["sk_name"]
+
+        try:
+            self.begin_transaction()
+            self.conn.execute(
+                text(
+                    f"""
+                DELETE FROM {schema}.{table} as tb1
+                USING {temporary_schema}.{temporary_table} as tb2
+                WHERE tb1.{sk_name} = tb2.{sk_name};      
+                """
+                )
+            )
+
+        except Exception as err:
+            self.rollback()
+            raise Exception(str(err))
+
+        else:
+            self.create_commit()
+        return
+
+    def drop_temporary_table(self, **kwargs):
+        temporary_table = kwargs["temporary_table"].lower()
+        temporary_schema = kwargs["temporary_schema"].lower()
+        self.conn.execute(
+            text(f"DROP TABLE IF EXISTS {temporary_schema}.{temporary_table}")
+        )
+        return
+
+    def read(self, **kwargs):
+        pass
+
+    def load(self, **kwargs):
+        pass
```

### Comparing `sefazetllib-0.1.55/sefazetllib/factory/platform/dataframe/Pandas.py` & `sefazetllib-0.1.56/sefazetllib/factory/platform/dataframe/Pandas.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from datetime import date
-
-import pandas as pd
-from pandas.util import hash_pandas_object
-
-from sefazetllib.factory.platform.Platform import Platform
-
-
-class Pandas(Platform):
-    def __init__(self, name=None) -> None:
-        self.session = pd
-        self.name = name
-
-    def __read_csv(self, url):
-        return self.session.read_csv(url)
-
-    def __read_parquet(self, url):
-        return self.session.read_parquet(url)
-
-    def __save_csv(self, df, url, properties):
-        return df.to_csv(url, **properties)
-
-    def __save_parquet(self, df, url, properties):
-        return df.to_parquet(url, **properties)
-
-    def __get_key_method(self, name):
-        return {"SurrogateKey": hash_pandas_object}[name]
-
-    def read(self, **kwargs):
-        file_format = kwargs["file_format"]
-        url = kwargs["url"]
-        return {"csv": self.__read_csv, "parquet": self.__read_parquet}[file_format](
-            url
-        )
-
-    def load(self, **kwargs):
-        df = kwargs["df"]
-        sk_name = kwargs["sk_name"]
-        key = kwargs["key"]
-        columns = kwargs["columns"]
-        duplicates = kwargs["duplicates"]
-        file_format = kwargs["file_format"]
-        format_properties = kwargs["format_properties"]
-        url = kwargs["url"]
-
-        key.setColumns(df[key.columns])
-        key.setMethod(self.__get_key_method(type(key).__name__))
-
-        writer_format = df
-        writer_format[sk_name] = key.get()
-        writer_format["DAT_CARGA"] = date.today()
-
-        if bool(columns):
-            writer_format = writer_format[columns]
-
-        if duplicates:
-            writer_format = writer_format.drop_duplicates()
-
-        return {"csv": self.__save_csv, "parquet": self.__save_parquet}[file_format](
-            writer_format, url, format_properties
-        )
+from datetime import date
+
+import pandas as pd
+from pandas.util import hash_pandas_object
+
+from sefazetllib.factory.platform.Platform import Platform
+
+
+class Pandas(Platform):
+    def __init__(self, name=None) -> None:
+        self.session = pd
+        self.name = name
+
+    def __read_csv(self, url):
+        return self.session.read_csv(url)
+
+    def __read_parquet(self, url):
+        return self.session.read_parquet(url)
+
+    def __save_csv(self, df, url, properties):
+        return df.to_csv(url, **properties)
+
+    def __save_parquet(self, df, url, properties):
+        return df.to_parquet(url, **properties)
+
+    def __get_key_method(self, name):
+        return {"SurrogateKey": hash_pandas_object}[name]
+
+    def read(self, **kwargs):
+        file_format = kwargs["file_format"]
+        url = kwargs["url"]
+        return {"csv": self.__read_csv, "parquet": self.__read_parquet}[file_format](
+            url
+        )
+
+    def load(self, **kwargs):
+        df = kwargs["df"]
+        sk_name = kwargs["sk_name"]
+        key = kwargs["key"]
+        columns = kwargs["columns"]
+        duplicates = kwargs["duplicates"]
+        file_format = kwargs["file_format"]
+        format_properties = kwargs["format_properties"]
+        url = kwargs["url"]
+
+        key.setColumns(df[key.columns])
+        key.setMethod(self.__get_key_method(type(key).__name__))
+
+        writer_format = df
+        writer_format[sk_name] = key.get()
+        writer_format["DAT_CARGA"] = date.today()
+
+        if bool(columns):
+            writer_format = writer_format[columns]
+
+        if duplicates:
+            writer_format = writer_format.drop_duplicates()
+
+        return {"csv": self.__save_csv, "parquet": self.__save_parquet}[file_format](
+            writer_format, url, format_properties
+        )
```

### Comparing `sefazetllib-0.1.55/sefazetllib/factory/platform/dataframe/Spark.py` & `sefazetllib-0.1.56/sefazetllib/factory/platform/dataframe/Spark.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-import subprocess
-
-from pyspark.sql import SparkSession
-from pyspark.sql.functions import (
-    col,
-    current_timestamp,
-    from_utc_timestamp,
-    lit,
-    monotonically_increasing_id,
-    to_date,
-    xxhash64,
-)
-from pyspark.sql.types import StructType
-
-from sefazetllib.config.CustomLogging import logger
-from sefazetllib.factory.platform.Platform import Platform
-
-
-class Spark(Platform):
-    def __init__(self, name="Spark Job", configs=[]) -> None:
-        self.name = name
-        session = SparkSession.builder.appName(name)
-        if configs != []:
-            for config in configs:
-                session = session.config(*config)
-        self.session = session.getOrCreate()
-        self.checkpoint_dir = f"/tmp/checkpoint/{name}"
-        self.session.sparkContext.setCheckpointDir(self.checkpoint_dir)
-
-    def __get_key_method(self, name):
-        return {
-            "SurrogateKey": xxhash64,
-            "IncrementalKey": monotonically_increasing_id,
-        }[name]
-
-    def __define_properties(self, df, type_format, url, properties):
-        if type_format == "jdbc":
-            properties.pop("operation", None)
-            properties["url"] = url
-
-        return df.options(**properties)
-
-    def __define_load(self, df, type_format, url):
-        if type_format == "jdbc":
-            return df.load()
-        return df.load(url)
-
-    def __define_save(self, df, type_format, url):
-        if type_format == "jdbc":
-            return df.save()
-        return df.save(url)
-
-    def columns_to_upper(self, df):
-        return df.select([col(c).alias(c.upper()) for c in df.columns])
-
-    def checkpoint(self, df):
-        return df.checkpoint()
-
-    def clean_checkpoint(self):
-        try:
-            cmd = ["hadoop", "fs", "-rm", "-r", self.checkpoint_dir]
-            subprocess.check_call(
-                cmd, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
-            )
-        except subprocess.CalledProcessError:
-            logger.error("Error deleting %s from HDFS", self.checkpoint_dir)
-        except Exception as e:
-            logger.error("Unexpected error: %s", str(e))
-
-    def select_columns(self, df, columns):
-        return df.select(*columns)
-
-    def join(self, left, right, keys, how):
-        if isinstance(keys, list):
-            left_key, right_key = keys
-        else:
-            left_key = right_key = keys
-
-        return left.join(right, left[left_key] == right[right_key], how)
-
-    def union_by_name(self, left, right):
-        return left.unionByName(right)
-
-    def create_df(self, columns):
-        schema = StructType([])
-        df = self.session.createDataFrame([], schema)
-        for cols in columns:
-            df = df.withColumn(cols, lit(None))
-        return df
-
-    def read(self, **kwargs):
-        type_format = kwargs["file_format"]
-        url = kwargs["url"]
-        format_properties = kwargs["format_properties"]
-        optional = kwargs["optional"]
-        columns = kwargs["columns"]
-        duplicates = kwargs["duplicates"]
-
-        df = self.session.read.format(type_format)
-
-        if bool(format_properties):
-            df = self.__define_properties(df, type_format, url, format_properties)
-
-        try:
-            df = self.__define_load(df, type_format, url)
-
-            if bool(columns):
-                df = df.select(columns)
-
-            if duplicates:
-                df = df.dropDuplicates()
-            return df
-
-        except Exception as e:
-            if not optional:
-                logger.error("The 'optional' attribute is set to False. Error: %s", e)
-                raise Exception("erro dentro do SPARK", str(e))
-            schema = StructType([])
-            df = self.session.createDataFrame([], schema)
-            for cols in columns:
-                df = df.withColumn(cols, lit(None))
-            return df
-
-    def load(self, **kwargs):
-        df = kwargs["df"]
-        sk_name = kwargs["sk_name"]
-        key = kwargs["key"]
-        columns = kwargs["columns"]
-        duplicates = kwargs["duplicates"]
-        type_format = kwargs["file_format"]
-        format_properties = kwargs["format_properties"]
-        url = kwargs["url"]
-        mode = kwargs["mode"]
-        load_date = kwargs["load_date"]
-        load_date_name = kwargs["load_date_name"]
-        load_date_timestamp = kwargs["load_date_timestamp"]
-        load_date_timezone = kwargs["load_date_timezone"]
-
-        df_writer = df
-
-        if load_date:
-            timestamp_in_timezone = from_utc_timestamp(
-                current_timestamp(), load_date_timezone
-            )
-            df_writer = df.withColumn(
-                load_date_name,
-                timestamp_in_timezone
-                if load_date_timestamp
-                else to_date(timestamp_in_timezone),
-            )
-
-        if hasattr(key, "name"):
-            if key.name is not None:
-                sk_name = key.name
-
-            key.setMethod(self.__get_key_method(type(key).__name__))
-            df_writer = df_writer.withColumn(sk_name, key.get())
-
-        if bool(columns):
-            df_writer = df_writer.select(
-                list(dict.fromkeys([sk_name, *columns, load_date_name]))
-            )
-
-        if duplicates:
-            df_writer = df_writer.dropDuplicates()
-
-        writer_format = df_writer.write.format(type_format)
-
-        if bool(format_properties):
-            writer_format = self.__define_properties(
-                writer_format, type_format, url, format_properties
-            )
-
-        if mode is not None:
-            writer_format = writer_format.mode(mode)
-
-        self.__define_save(writer_format, type_format, url)
-
-        return df_writer
-    
-    def close_session(self):
-        self.session.stop()
-        return
+import subprocess
+
+from pyspark.sql import SparkSession
+from pyspark.sql.functions import (
+    col,
+    current_timestamp,
+    from_utc_timestamp,
+    lit,
+    monotonically_increasing_id,
+    to_date,
+    xxhash64,
+)
+from pyspark.sql.types import StructType
+
+from sefazetllib.config.CustomLogging import logger
+from sefazetllib.factory.platform.Platform import Platform
+
+
+class Spark(Platform):
+    def __init__(self, name="Spark Job", configs=[]) -> None:
+        self.name = name
+        session = SparkSession.builder.appName(name)
+        if configs != []:
+            for config in configs:
+                session = session.config(*config)
+        self.session = session.getOrCreate()
+        self.checkpoint_dir = f"/tmp/checkpoint/{name}"
+        self.session.sparkContext.setCheckpointDir(self.checkpoint_dir)
+
+    def __get_key_method(self, name):
+        return {
+            "SurrogateKey": xxhash64,
+            "IncrementalKey": monotonically_increasing_id,
+        }[name]
+
+    def __define_properties(self, df, type_format, url, properties):
+        if type_format == "jdbc":
+            properties.pop("operation", None)
+            properties["url"] = url
+
+        return df.options(**properties)
+
+    def __define_load(self, df, type_format, url):
+        if type_format == "jdbc":
+            return df.load()
+        return df.load(url)
+
+    def __define_save(self, df, type_format, url):
+        if type_format == "jdbc":
+            return df.save()
+        return df.save(url)
+
+    def columns_to_upper(self, df):
+        return df.select([col(c).alias(c.upper()) for c in df.columns])
+
+    def checkpoint(self, df):
+        return df.checkpoint()
+
+    def clean_checkpoint(self):
+        try:
+            cmd = ["hadoop", "fs", "-rm", "-r", self.checkpoint_dir]
+            subprocess.check_call(
+                cmd, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
+            )
+        except subprocess.CalledProcessError:
+            logger.error("Error deleting %s from HDFS", self.checkpoint_dir)
+        except Exception as e:
+            logger.error("Unexpected error: %s", str(e))
+
+    def select_columns(self, df, columns):
+        return df.select(*columns)
+
+    def join(self, left, right, keys, how):
+        if isinstance(keys, list):
+            left_key, right_key = keys
+        else:
+            left_key = right_key = keys
+
+        return left.join(right, left[left_key] == right[right_key], how)
+
+    def union_by_name(self, left, right):
+        return left.unionByName(right)
+
+    def create_df(self, columns):
+        schema = StructType([])
+        df = self.session.createDataFrame([], schema)
+        for cols in columns:
+            df = df.withColumn(cols, lit(None))
+        return df
+
+    def read(self, **kwargs):
+        type_format = kwargs["file_format"]
+        url = kwargs["url"]
+        format_properties = kwargs["format_properties"]
+        optional = kwargs["optional"]
+        columns = kwargs["columns"]
+        duplicates = kwargs["duplicates"]
+
+        df = self.session.read.format(type_format)
+
+        if bool(format_properties):
+            df = self.__define_properties(df, type_format, url, format_properties)
+
+        try:
+            df = self.__define_load(df, type_format, url)
+
+            if bool(columns):
+                df = df.select(columns)
+
+            if duplicates:
+                df = df.dropDuplicates()
+            return df
+
+        except Exception as e:
+            if not optional:
+                logger.error("The 'optional' attribute is set to False. Error: %s", e)
+                raise Exception("erro dentro do SPARK", str(e))
+            schema = StructType([])
+            df = self.session.createDataFrame([], schema)
+            for cols in columns:
+                df = df.withColumn(cols, lit(None))
+            return df
+
+    def load(self, **kwargs):
+        df = kwargs["df"]
+        sk_name = kwargs["sk_name"]
+        key = kwargs["key"]
+        columns = kwargs["columns"]
+        duplicates = kwargs["duplicates"]
+        type_format = kwargs["file_format"]
+        format_properties = kwargs["format_properties"]
+        url = kwargs["url"]
+        mode = kwargs["mode"]
+        load_date = kwargs["load_date"]
+        load_date_name = kwargs["load_date_name"]
+        load_date_timestamp = kwargs["load_date_timestamp"]
+        load_date_timezone = kwargs["load_date_timezone"]
+
+        df_writer = df
+
+        if load_date:
+            timestamp_in_timezone = from_utc_timestamp(
+                current_timestamp(), load_date_timezone
+            )
+            df_writer = df.withColumn(
+                load_date_name,
+                timestamp_in_timezone
+                if load_date_timestamp
+                else to_date(timestamp_in_timezone),
+            )
+
+        if hasattr(key, "name"):
+            if key.name is not None:
+                sk_name = key.name
+
+            key.setMethod(self.__get_key_method(type(key).__name__))
+            df_writer = df_writer.withColumn(sk_name, key.get())
+
+        if bool(columns):
+            df_writer = df_writer.select(
+                list(dict.fromkeys([sk_name, *columns, load_date_name]))
+            )
+
+        if duplicates:
+            df_writer = df_writer.dropDuplicates()
+
+        writer_format = df_writer.write.format(type_format)
+
+        if bool(format_properties):
+            writer_format = self.__define_properties(
+                writer_format, type_format, url, format_properties
+            )
+
+        if mode is not None:
+            writer_format = writer_format.mode(mode)
+
+        self.__define_save(writer_format, type_format, url)
+
+        return df_writer
+    
+    def close_session(self):
+        self.session.stop()
+        return
```

### Comparing `sefazetllib-0.1.55/sefazetllib/load/LoadLocal.py` & `sefazetllib-0.1.56/sefazetllib/load/LoadLocal.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-import os
-from typing import Any, Dict, List
-
-from sefazetllib.Builder import Builder, field
-from sefazetllib.factory.platform.dataframe.Default import Default
-from sefazetllib.factory.platform.Platform import Platform
-from sefazetllib.load.Load import Load
-from sefazetllib.utils.key import DefaultKey, Key
-
-
-@Builder
-class LoadLocal(Load):
-    platform: Platform = field(default=Default())
-    file_format: str = field(default="")
-    format_properties: Dict[str, Any] = field(default_factory=dict)
-    reference: str = field(default="")
-    url: str = field(default="")
-    repository: str = field(default="")
-    entity: str = field(default="")
-    mode: str = field(default="")
-    df_writer: Any = field(default="")
-    duplicates: bool = field(default=False)
-    key: Key = field(default=DefaultKey())
-    columns: List = field(default_factory=list)
-    load_date: bool = field(default=True)
-    load_date_name: str = field(default="DAT_CARGA")
-    load_date_timestamp: bool = field(default=False)
-    load_date_timezone: str = field(default="UTC-3")
-
-    def build_connection_string(self):
-        return f"{os.getcwd()}/{self.entity}.{self.file_format}"
-
-    def execute(self, **kwargs):
-        if isinstance(self.platform, Default):
-            self.setPlatform(kwargs["platform"])
-
-        if self.repository == "":
-            self.setRepository(kwargs["repository"])
-
-        self.url = self.build_connection_string()
-
-        if kwargs:
-            args = kwargs["args"]
-            if args.loadRepository:
-                self.setRepository(args.loadRepository)
-
-            if args.loadUrl:
-                self.url = args.loadUrl
-
-        sk_name = f"SK_{self.entity}"
-        if "/" in self.entity:
-            entity = self.entity.split("/")[1]
-            sk_name = f"SK_{entity}"
-
-        return (
-            self.reference,
-            self.platform.load(
-                df=self.df_writer,
-                sk_name=sk_name,
-                key=self.key,
-                columns=self.columns,
-                duplicates=self.duplicates,
-                file_format=self.file_format,
-                format_properties=self.format_properties,
-                url=self.url,
-                mode=self.mode,
-                load_date=self.load_date,
-                load_date_name=self.load_date_name,
-                load_date_timestamp=self.load_date_timestamp,
-                load_date_timezone=self.load_date_timezone,
-            ),
-        )
+import os
+from typing import Any, Dict, List
+
+from sefazetllib.Builder import Builder, field
+from sefazetllib.factory.platform.dataframe.Default import Default
+from sefazetllib.factory.platform.Platform import Platform
+from sefazetllib.load.Load import Load
+from sefazetllib.utils.key import DefaultKey, Key
+
+
+@Builder
+class LoadLocal(Load):
+    platform: Platform = field(default=Default())
+    file_format: str = field(default="")
+    format_properties: Dict[str, Any] = field(default_factory=dict)
+    reference: str = field(default="")
+    url: str = field(default="")
+    repository: str = field(default="")
+    entity: str = field(default="")
+    mode: str = field(default="")
+    df_writer: Any = field(default="")
+    duplicates: bool = field(default=False)
+    key: Key = field(default=DefaultKey())
+    columns: List = field(default_factory=list)
+    load_date: bool = field(default=True)
+    load_date_name: str = field(default="DAT_CARGA")
+    load_date_timestamp: bool = field(default=False)
+    load_date_timezone: str = field(default="UTC-3")
+
+    def build_connection_string(self):
+        return f"{os.getcwd()}/{self.entity}.{self.file_format}"
+
+    def execute(self, **kwargs):
+        if isinstance(self.platform, Default):
+            self.setPlatform(kwargs["platform"])
+
+        if self.repository == "":
+            self.setRepository(kwargs["repository"])
+
+        self.url = self.build_connection_string()
+
+        if kwargs:
+            args = kwargs["args"]
+            if args.loadRepository:
+                self.setRepository(args.loadRepository)
+
+            if args.loadUrl:
+                self.url = args.loadUrl
+
+        sk_name = f"SK_{self.entity}"
+        if "/" in self.entity:
+            entity = self.entity.split("/")[1]
+            sk_name = f"SK_{entity}"
+
+        return (
+            self.reference,
+            self.platform.load(
+                df=self.df_writer,
+                sk_name=sk_name,
+                key=self.key,
+                columns=self.columns,
+                duplicates=self.duplicates,
+                file_format=self.file_format,
+                format_properties=self.format_properties,
+                url=self.url,
+                mode=self.mode,
+                load_date=self.load_date,
+                load_date_name=self.load_date_name,
+                load_date_timestamp=self.load_date_timestamp,
+                load_date_timezone=self.load_date_timezone,
+            ),
+        )
```

### Comparing `sefazetllib-0.1.55/sefazetllib/load/LoadS3.py` & `sefazetllib-0.1.56/sefazetllib/load/LoadS3.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-import warnings
-from typing import Any, Dict, List
-
-import boto3
-
-from sefazetllib.Builder import Builder, field
-from sefazetllib.config.CustomLogging import logger
-from sefazetllib.factory.platform.dataframe.Default import Default
-from sefazetllib.factory.platform.Platform import Platform
-from sefazetllib.load.Load import Load
-from sefazetllib.utils.key import DefaultKey, Key
-
-
-@Builder
-class LoadS3(Load):
-    warnings.warn(
-        "The 'LoadS3' class is deprecated. Please use the 'LoadStorage' class with the protocol parameter (e.g., 's3a')."
-    )
-    platform: Platform = field(default=Default())
-    file_format: str = field(default="")
-    format_properties: Dict[str, Any] = field(default_factory=dict)
-    reference: str = field(default="")
-    url: str = field(default="")
-    repository: str = field(default="")
-    layer: str = field(default="")
-    schema: str = field(default="")
-    entity: str = field(default="")
-    mode: str = field(default="")
-    df_writer: Any = field(default="")
-    duplicates: bool = field(default=False)
-    key: Key = field(default=DefaultKey())
-    columns: List = field(default_factory=list)
-    load_date: bool = field(default=True)
-    load_date_name: str = field(default="DAT_CARGA")
-    load_date_timestamp: bool = field(default=False)
-    load_date_timezone: str = field(default="UTC-3")
-
-    def build_connection_string(self):
-        self.url = f"s3a://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
-        return self.url
-
-    def get_table_name(self):
-        return self.entity.split("/")[-1] if "/" in self.entity else self.entity
-
-    def delete_aws_glue_table(self, database, table):
-        glue = boto3.client("glue")
-        try:
-            glue.delete_table(DatabaseName=database, Name=table)
-        except glue.exceptions.EntityNotFoundException:
-            logger.warning(
-                "Attempted to delete table %s in AWS Glue's database %s, but the table does not exist. The deletion routine will be ignored.",
-                table.upper(),
-                database.upper(),
-            )
-
-    def execute(self, **kwargs):
-        if isinstance(self.platform, Default):
-            self.setPlatform(kwargs["platform"])
-
-        local_repository = self.repository
-        if local_repository == "":
-            self.setRepository(kwargs["repository"])
-
-        if kwargs:
-            args = kwargs["args"]
-            if args.loadRepository and local_repository == "":
-                self.setRepository(args.loadRepository)
-
-            if args.loadUrl:
-                url = args.loadUrl
-            else:
-                url = self.build_connection_string()
-        else:
-            url = self.build_connection_string()
-
-        sk_name = f"SK_{self.get_table_name()}"
-
-        try:
-            return (
-                self.reference,
-                self.platform.load(
-                    df=self.df_writer,
-                    sk_name=sk_name,
-                    key=self.key,
-                    columns=self.columns,
-                    duplicates=self.duplicates,
-                    file_format=self.file_format,
-                    format_properties=self.format_properties,
-                    url=url,
-                    mode=self.mode,
-                    load_date=self.load_date,
-                    load_date_name=self.load_date_name,
-                    load_date_timestamp=self.load_date_timestamp,
-                    load_date_timezone=self.load_date_timezone,
-                ),
-            )
-        except Exception as e:
-            apache_hudi_type_conversion_exception = "org.apache.hudi.hive.HoodieHiveSyncException: Could not convert field Type"
-            if (
-                self.file_format == "hudi" or "org.apache.hudi"
-            ) and apache_hudi_type_conversion_exception in str(e):
-                database = self.format_properties[
-                    "hoodie.datasource.hive_sync.database"
-                ]
-                table = self.get_table_name().lower()
-                logger.info(
-                    "Detected a change in data type. Deleting %s in AWS Glue's database %s to resolve the issue..",
-                    table.upper(),
-                    database.upper(),
-                )
-                self.delete_aws_glue_table(database, table)
-
-            return (
-                self.reference,
-                self.platform.load(
-                    df=self.df_writer,
-                    sk_name=sk_name,
-                    key=self.key,
-                    columns=self.columns,
-                    duplicates=self.duplicates,
-                    file_format=self.file_format,
-                    format_properties=self.format_properties,
-                    url=url,
-                    mode=self.mode,
-                    load_date=self.load_date,
-                    load_date_name=self.load_date_name,
-                    load_date_timestamp=self.load_date_timestamp,
-                    load_date_timezone=self.load_date_timezone,
-                ),
-            )
+import warnings
+from typing import Any, Dict, List
+
+import boto3
+
+from sefazetllib.Builder import Builder, field
+from sefazetllib.config.CustomLogging import logger
+from sefazetllib.factory.platform.dataframe.Default import Default
+from sefazetllib.factory.platform.Platform import Platform
+from sefazetllib.load.Load import Load
+from sefazetllib.utils.key import DefaultKey, Key
+
+
+@Builder
+class LoadS3(Load):
+    warnings.warn(
+        "The 'LoadS3' class is deprecated. Please use the 'LoadStorage' class with the protocol parameter (e.g., 's3a')."
+    )
+    platform: Platform = field(default=Default())
+    file_format: str = field(default="")
+    format_properties: Dict[str, Any] = field(default_factory=dict)
+    reference: str = field(default="")
+    url: str = field(default="")
+    repository: str = field(default="")
+    layer: str = field(default="")
+    schema: str = field(default="")
+    entity: str = field(default="")
+    mode: str = field(default="")
+    df_writer: Any = field(default="")
+    duplicates: bool = field(default=False)
+    key: Key = field(default=DefaultKey())
+    columns: List = field(default_factory=list)
+    load_date: bool = field(default=True)
+    load_date_name: str = field(default="DAT_CARGA")
+    load_date_timestamp: bool = field(default=False)
+    load_date_timezone: str = field(default="UTC-3")
+
+    def build_connection_string(self):
+        self.url = f"s3a://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
+        return self.url
+
+    def get_table_name(self):
+        return self.entity.split("/")[-1] if "/" in self.entity else self.entity
+
+    def delete_aws_glue_table(self, database, table):
+        glue = boto3.client("glue")
+        try:
+            glue.delete_table(DatabaseName=database, Name=table)
+        except glue.exceptions.EntityNotFoundException:
+            logger.warning(
+                "Attempted to delete table %s in AWS Glue's database %s, but the table does not exist. The deletion routine will be ignored.",
+                table.upper(),
+                database.upper(),
+            )
+
+    def execute(self, **kwargs):
+        if isinstance(self.platform, Default):
+            self.setPlatform(kwargs["platform"])
+
+        local_repository = self.repository
+        if local_repository == "":
+            self.setRepository(kwargs["repository"])
+
+        if kwargs:
+            args = kwargs["args"]
+            if args.loadRepository and local_repository == "":
+                self.setRepository(args.loadRepository)
+
+            if args.loadUrl:
+                url = args.loadUrl
+            else:
+                url = self.build_connection_string()
+        else:
+            url = self.build_connection_string()
+
+        sk_name = f"SK_{self.get_table_name()}"
+
+        try:
+            return (
+                self.reference,
+                self.platform.load(
+                    df=self.df_writer,
+                    sk_name=sk_name,
+                    key=self.key,
+                    columns=self.columns,
+                    duplicates=self.duplicates,
+                    file_format=self.file_format,
+                    format_properties=self.format_properties,
+                    url=url,
+                    mode=self.mode,
+                    load_date=self.load_date,
+                    load_date_name=self.load_date_name,
+                    load_date_timestamp=self.load_date_timestamp,
+                    load_date_timezone=self.load_date_timezone,
+                ),
+            )
+        except Exception as e:
+            apache_hudi_type_conversion_exception = "org.apache.hudi.hive.HoodieHiveSyncException: Could not convert field Type"
+            if (
+                self.file_format == "hudi" or "org.apache.hudi"
+            ) and apache_hudi_type_conversion_exception in str(e):
+                database = self.format_properties[
+                    "hoodie.datasource.hive_sync.database"
+                ]
+                table = self.get_table_name().lower()
+                logger.info(
+                    "Detected a change in data type. Deleting %s in AWS Glue's database %s to resolve the issue..",
+                    table.upper(),
+                    database.upper(),
+                )
+                self.delete_aws_glue_table(database, table)
+
+            return (
+                self.reference,
+                self.platform.load(
+                    df=self.df_writer,
+                    sk_name=sk_name,
+                    key=self.key,
+                    columns=self.columns,
+                    duplicates=self.duplicates,
+                    file_format=self.file_format,
+                    format_properties=self.format_properties,
+                    url=url,
+                    mode=self.mode,
+                    load_date=self.load_date,
+                    load_date_name=self.load_date_name,
+                    load_date_timestamp=self.load_date_timestamp,
+                    load_date_timezone=self.load_date_timezone,
+                ),
+            )
```

### Comparing `sefazetllib-0.1.55/sefazetllib/transform/ConvertColumnsType.py` & `sefazetllib-0.1.56/sefazetllib/transform/ConvertColumnsType.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from typing import List, Optional, Tuple
-
-from pyspark.sql import DataFrame
-from pyspark.sql.functions import col
-from pyspark.sql.types import DataType
-
-from sefazetllib import Builder
-from sefazetllib.transform.Transform import Transform
-
-
-@Builder
-class ConvertColumnsType(Transform):
-    df: Optional[DataFrame] = None
-    reference: Optional[str] = None
-    output: Optional[str] = None
-    columns: Optional[List[str]] = None
-    data_type: Optional[DataType] = None
-
-    def execute(self) -> Tuple[str, DataFrame]:
-        exceeded_columns = set(self.columns) - set(self.df.columns)
-
-        if exceeded_columns:
-            raise Exception(
-                f"The following columns do not exist in {self.reference}: {str(exceeded_columns)}"
-            )
-
-        converted_columns = [
-            column if column not in self.columns else col(column).cast(self.data_type)
-            for column in self.df.columns
-        ]
-        return (
-            self.output,
-            (self.df.select(converted_columns)),
-        )
+from typing import List, Optional, Tuple
+
+from pyspark.sql import DataFrame
+from pyspark.sql.functions import col
+from pyspark.sql.types import DataType
+
+from sefazetllib import Builder
+from sefazetllib.transform.Transform import Transform
+
+
+@Builder
+class ConvertColumnsType(Transform):
+    df: Optional[DataFrame] = None
+    reference: Optional[str] = None
+    output: Optional[str] = None
+    columns: Optional[List[str]] = None
+    data_type: Optional[DataType] = None
+
+    def execute(self) -> Tuple[str, DataFrame]:
+        exceeded_columns = set(self.columns) - set(self.df.columns)
+
+        if exceeded_columns:
+            raise Exception(
+                f"The following columns do not exist in {self.reference}: {str(exceeded_columns)}"
+            )
+
+        converted_columns = [
+            column if column not in self.columns else col(column).cast(self.data_type)
+            for column in self.df.columns
+        ]
+        return (
+            self.output,
+            (self.df.select(converted_columns)),
+        )
```

### Comparing `sefazetllib-0.1.55/sefazetllib/transform/DataFrameFilterRangeTransform.py` & `sefazetllib-0.1.56/sefazetllib/transform/DataFrameFilterRangeTransform.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from typing import Any, Optional, Tuple
-
-from pyspark.sql import DataFrame
-from pyspark.sql.functions import col
-
-from sefazetllib import Builder, field
-from sefazetllib.transform.Transform import Transform
-
-
-@Builder
-class DataFrameFilterRangeTransform(Transform):
-    df: Optional[DataFrame] = None
-    reference: str = field(default="")
-    output: str = field(default="")
-    column_name: str = field(default="")
-    start: Any = field(default="")
-    end: Any = field(default="")
-    inclusive_start: bool = field(default=True)
-    inclusive_end: bool = field(default=True)
-
-    def execute(self) -> Tuple[str, DataFrame]:
-        df_range = self.df
-
-        if self.column_name:
-            if self.start:
-                if self.inclusive_start:
-                    df_range = df_range.filter(col(self.column_name) >= self.start)
-                else:
-                    df_range = df_range.filter(col(self.column_name) > self.start)
-
-            if self.end:
-                if self.inclusive_end:
-                    df_range = df_range.filter(col(self.column_name) <= self.end)
-                else:
-                    df_range = df_range.filter(col(self.column_name) < self.end)
-
-        return (self.output, df_range)
+from typing import Any, Optional, Tuple
+
+from pyspark.sql import DataFrame
+from pyspark.sql.functions import col
+
+from sefazetllib import Builder, field
+from sefazetllib.transform.Transform import Transform
+
+
+@Builder
+class DataFrameFilterRangeTransform(Transform):
+    df: Optional[DataFrame] = None
+    reference: str = field(default="")
+    output: str = field(default="")
+    column_name: str = field(default="")
+    start: Any = field(default="")
+    end: Any = field(default="")
+    inclusive_start: bool = field(default=True)
+    inclusive_end: bool = field(default=True)
+
+    def execute(self) -> Tuple[str, DataFrame]:
+        df_range = self.df
+
+        if self.column_name:
+            if self.start:
+                if self.inclusive_start:
+                    df_range = df_range.filter(col(self.column_name) >= self.start)
+                else:
+                    df_range = df_range.filter(col(self.column_name) > self.start)
+
+            if self.end:
+                if self.inclusive_end:
+                    df_range = df_range.filter(col(self.column_name) <= self.end)
+                else:
+                    df_range = df_range.filter(col(self.column_name) < self.end)
+
+        return (self.output, df_range)
```

### Comparing `sefazetllib-0.1.55/sefazetllib/transform/MinMaxLineTransform.py` & `sefazetllib-0.1.56/sefazetllib/transform/MinMaxLineTransform.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from typing import Any, List, Optional
-
-from pyspark.sql.functions import col, dense_rank
-from pyspark.sql.window import Window
-
-from sefazetllib import Builder, field
-from sefazetllib.transform.Transform import Transform
-
-
-@Builder
-class MinMaxLineTransform(Transform):
-    df: Optional[Any] = None
-    reference: str = field(default="")
-    output: str = field(default="")
-    order: str = field(default="")
-    orders: List[str] = field(default_factory=list)
-    window: str = field(default="")
-    max: bool = field(default=False)
-    min: bool = field(default=False)
-
-    def __get_window(self):
-        if self.max:
-            order_max = []
-
-            for unique_order in self.orders:
-                order_max.append(col(unique_order).desc())
-
-            self.window = Window.orderBy(order_max)
-
-        if self.min:
-            self.window = Window.orderBy(self.orders)
-
-        if self.order != "":
-            if self.max:
-                self.window = Window.orderBy(col(self.order).desc())
-
-            if self.min:
-                self.window = Window.orderBy(self.order)
-
-    def execute(self):
-        self.__get_window()
-        return (
-            self.output,
-            (
-                self.df.withColumn(
-                    "FLG_FILTER_LINE",
-                    dense_rank().over(self.window),
-                )
-                .filter(col("FLG_FILTER_LINE").eqNullSafe(1))
-                .drop("FLG_FILTER_LINE")
-            ),
-        )
+from typing import Any, List, Optional
+
+from pyspark.sql.functions import col, dense_rank
+from pyspark.sql.window import Window
+
+from sefazetllib import Builder, field
+from sefazetllib.transform.Transform import Transform
+
+
+@Builder
+class MinMaxLineTransform(Transform):
+    df: Optional[Any] = None
+    reference: str = field(default="")
+    output: str = field(default="")
+    order: str = field(default="")
+    orders: List[str] = field(default_factory=list)
+    window: str = field(default="")
+    max: bool = field(default=False)
+    min: bool = field(default=False)
+
+    def __get_window(self):
+        if self.max:
+            order_max = []
+
+            for unique_order in self.orders:
+                order_max.append(col(unique_order).desc())
+
+            self.window = Window.orderBy(order_max)
+
+        if self.min:
+            self.window = Window.orderBy(self.orders)
+
+        if self.order != "":
+            if self.max:
+                self.window = Window.orderBy(col(self.order).desc())
+
+            if self.min:
+                self.window = Window.orderBy(self.order)
+
+    def execute(self):
+        self.__get_window()
+        return (
+            self.output,
+            (
+                self.df.withColumn(
+                    "FLG_FILTER_LINE",
+                    dense_rank().over(self.window),
+                )
+                .filter(col("FLG_FILTER_LINE").eqNullSafe(1))
+                .drop("FLG_FILTER_LINE")
+            ),
+        )
```

### Comparing `sefazetllib-0.1.55/sefazetllib/transform/QuartileTransform.py` & `sefazetllib-0.1.56/sefazetllib/transform/QuartileTransform.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-from typing import Any, List, Optional, Tuple
-
-from pyspark.sql.functions import col, first, percentile_approx, when, avg
-from pyspark.sql.window import Window
-
-from sefazetllib import Builder, field
-from sefazetllib.transform.Transform import Transform
-
-
-@Builder
-class QuartileTransform(Transform):
-    df: Optional[Any] = None
-    reference: str = field(default="")
-    output: str = field(default="")
-    partitions: List[str] = field(default_factory=list)
-    target: str = field(default="")
-    outlier: bool = field(default=False)
-    median: bool = field(default=False)
-    average: bool = field(default=False)
-    
-    def __get_window(self):
-        if self.partitions is not None:
-            self.window = Window.partitionBy(self.partitions)
-
-    def __get_quartile(self, percentile):
-        quartile = percentile_approx(self.target, percentile)
-
-        if self.window is not None:
-            return quartile.over(self.window)
-
-        return quartile
-
-    def execute(self) -> Tuple[str, Any]:
-        self.__get_window()
-
-        df_quartile = (
-            self.df.withColumn(f"Q1_{self.target}", self.__get_quartile(0.25))
-            .withColumn(f"Q2_{self.target}", self.__get_quartile(0.5))
-            .withColumn(f"Q3_{self.target}", self.__get_quartile(0.75))
-        )
-
-        if self.outlier:
-            df_quartile = df_quartile.withColumn(
-                f"OUT_{self.target}",
-                col(f"Q3_{self.target}")
-                + 3 * (col(f"Q3_{self.target}") - col(f"Q1_{self.target}")),
-            )
-
-        if (self.median | self.average):
-            group_columns = [
-                *self.partitions,
-                f"Q1_{self.target}",
-                f"Q2_{self.target}",
-                f"Q3_{self.target}",
-            ]
-
-            if self.outlier:
-                group_columns.append(f"OUT_{self.target}")
-
-            df_quartile = (
-                df_quartile.withColumn(
-                    f"STA_R_{self.target}",
-                    when(col(self.target) <= col(f"Q1_{self.target}"), 1)
-                    .when(
-                        (col(self.target) > col(f"Q1_{self.target}"))
-                        & (col(self.target) <= col(f"Q2_{self.target}")),
-                        2,
-                    )
-                    .when(
-                        (col(self.target) > col(f"Q2_{self.target}"))
-                        & (col(self.target) <= col(f"Q3_{self.target}")),
-                        3,
-                    )
-                    .when(col(self.target) > col(f"Q3_{self.target}"), 4),
-                )
-            )
-            
-            if self.median:
-                df_quartile = (df_quartile
-                    .withColumn(
-                        f"MEDIAN_Q_{self.target}",
-                        percentile_approx(self.target, 0.5).over(
-                            Window.partitionBy([*self.partitions, f"STA_R_{self.target}"])
-                        ),
-                    )
-                    .groupBy(group_columns)
-                    .pivot(f"STA_R_{self.target}")
-                    .agg(first(col(f"MEDIAN_Q_{self.target}")))
-                    .withColumnRenamed("1", f"MEDIAN_R1_{self.target}")
-                    .withColumnRenamed("2", f"MEDIAN_R2_{self.target}")
-                    .withColumnRenamed("3", f"MEDIAN_R3_{self.target}")
-                    .withColumnRenamed("4", f"MEDIAN_R4_{self.target}")
-            )
-            if self.average:
-                df_quartile = (df_quartile
-                    .withColumn(
-                        f"AVG_Q_{self.target}",
-                        avg(self.target).over(
-                            Window.partitionBy([*self.partitions, f"STA_R_{self.target}"])
-                        ),
-                    )
-                    .groupBy(group_columns)
-                    .pivot(f"STA_R_{self.target}")
-                    .agg(first(col(f"AVG_Q_{self.target}")))
-                    .withColumnRenamed("1", f"AVG_R1_{self.target}")
-                    .withColumnRenamed("2", f"AVG_R2_{self.target}")
-                    .withColumnRenamed("3", f"AVG_R3_{self.target}")
-                    .withColumnRenamed("4", f"AVG_R4_{self.target}")
-            )
-
-        if self.output is None:
-            self.output = self.reference
-
-        return self.output, df_quartile
+from typing import Any, List, Optional, Tuple
+
+from pyspark.sql.functions import col, first, percentile_approx, when, avg
+from pyspark.sql.window import Window
+
+from sefazetllib import Builder, field
+from sefazetllib.transform.Transform import Transform
+
+
+@Builder
+class QuartileTransform(Transform):
+    df: Optional[Any] = None
+    reference: str = field(default="")
+    output: str = field(default="")
+    partitions: List[str] = field(default_factory=list)
+    target: str = field(default="")
+    outlier: bool = field(default=False)
+    median: bool = field(default=False)
+    average: bool = field(default=False)
+    
+    def __get_window(self):
+        if self.partitions is not None:
+            self.window = Window.partitionBy(self.partitions)
+
+    def __get_quartile(self, percentile):
+        quartile = percentile_approx(self.target, percentile)
+
+        if self.window is not None:
+            return quartile.over(self.window)
+
+        return quartile
+
+    def execute(self) -> Tuple[str, Any]:
+        self.__get_window()
+
+        df_quartile = (
+            self.df.withColumn(f"Q1_{self.target}", self.__get_quartile(0.25))
+            .withColumn(f"Q2_{self.target}", self.__get_quartile(0.5))
+            .withColumn(f"Q3_{self.target}", self.__get_quartile(0.75))
+        )
+
+        if self.outlier:
+            df_quartile = df_quartile.withColumn(
+                f"OUT_{self.target}",
+                col(f"Q3_{self.target}")
+                + 3 * (col(f"Q3_{self.target}") - col(f"Q1_{self.target}")),
+            )
+
+        if (self.median | self.average):
+            group_columns = [
+                *self.partitions,
+                f"Q1_{self.target}",
+                f"Q2_{self.target}",
+                f"Q3_{self.target}",
+            ]
+
+            if self.outlier:
+                group_columns.append(f"OUT_{self.target}")
+
+            df_quartile = (
+                df_quartile.withColumn(
+                    f"STA_R_{self.target}",
+                    when(col(self.target) <= col(f"Q1_{self.target}"), 1)
+                    .when(
+                        (col(self.target) > col(f"Q1_{self.target}"))
+                        & (col(self.target) <= col(f"Q2_{self.target}")),
+                        2,
+                    )
+                    .when(
+                        (col(self.target) > col(f"Q2_{self.target}"))
+                        & (col(self.target) <= col(f"Q3_{self.target}")),
+                        3,
+                    )
+                    .when(col(self.target) > col(f"Q3_{self.target}"), 4),
+                )
+            )
+            
+            if self.median:
+                df_quartile = (df_quartile
+                    .withColumn(
+                        f"MEDIAN_Q_{self.target}",
+                        percentile_approx(self.target, 0.5).over(
+                            Window.partitionBy([*self.partitions, f"STA_R_{self.target}"])
+                        ),
+                    )
+                    .groupBy(group_columns)
+                    .pivot(f"STA_R_{self.target}")
+                    .agg(first(col(f"MEDIAN_Q_{self.target}")))
+                    .withColumnRenamed("1", f"MEDIAN_R1_{self.target}")
+                    .withColumnRenamed("2", f"MEDIAN_R2_{self.target}")
+                    .withColumnRenamed("3", f"MEDIAN_R3_{self.target}")
+                    .withColumnRenamed("4", f"MEDIAN_R4_{self.target}")
+            )
+            if self.average:
+                df_quartile = (df_quartile
+                    .withColumn(
+                        f"AVG_Q_{self.target}",
+                        avg(self.target).over(
+                            Window.partitionBy([*self.partitions, f"STA_R_{self.target}"])
+                        ),
+                    )
+                    .groupBy(group_columns)
+                    .pivot(f"STA_R_{self.target}")
+                    .agg(first(col(f"AVG_Q_{self.target}")))
+                    .withColumnRenamed("1", f"AVG_R1_{self.target}")
+                    .withColumnRenamed("2", f"AVG_R2_{self.target}")
+                    .withColumnRenamed("3", f"AVG_R3_{self.target}")
+                    .withColumnRenamed("4", f"AVG_R4_{self.target}")
+            )
+
+        if self.output is None:
+            self.output = self.reference
+
+        return self.output, df_quartile
```

### Comparing `sefazetllib-0.1.55/sefazetllib/transform/RoundColumns.py` & `sefazetllib-0.1.56/sefazetllib/transform/RoundColumns.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from typing import Any, List, Optional, Tuple
-from pyspark.sql import DataFrame
-from pyspark.sql.functions import col, round
-
-from sefazetllib import Builder, field
-from sefazetllib.transform.Transform import Transform
-
-@Builder
-class RoundColumns(Transform):
-    df: Optional[DataFrame] = None
-    reference: Optional[str] = None
-    output: Optional[str] = None
-    columns: Optional[List[str]] = None
-    precision: int = field(default=2)
-
-    def execute(self) -> Tuple[str, DataFrame]:
-        exceeded_columns = set(self.columns) - set(self.df.columns)
-
-        if exceeded_columns:
-            raise Exception(
-                f"The following columns do not exist in {self.reference}: {str(exceeded_columns)}"
-            )
-
-        rounded_columns = [
-            column
-            if column not in self.columns
-            else round(col(column), self.precision).alias(column)
-            for column in self.df.columns
-        ]
-        return (
-            self.output,
-            (self.df.select(rounded_columns)),
-        )
-        
+from typing import Any, List, Optional, Tuple
+from pyspark.sql import DataFrame
+from pyspark.sql.functions import col, round
+
+from sefazetllib import Builder, field
+from sefazetllib.transform.Transform import Transform
+
+@Builder
+class RoundColumns(Transform):
+    df: Optional[DataFrame] = None
+    reference: Optional[str] = None
+    output: Optional[str] = None
+    columns: Optional[List[str]] = None
+    precision: int = field(default=2)
+
+    def execute(self) -> Tuple[str, DataFrame]:
+        exceeded_columns = set(self.columns) - set(self.df.columns)
+
+        if exceeded_columns:
+            raise Exception(
+                f"The following columns do not exist in {self.reference}: {str(exceeded_columns)}"
+            )
+
+        rounded_columns = [
+            column
+            if column not in self.columns
+            else round(col(column), self.precision).alias(column)
+            for column in self.df.columns
+        ]
+        return (
+            self.output,
+            (self.df.select(rounded_columns)),
+        )
+
```

### Comparing `sefazetllib-0.1.55/sefazetllib/utils/partition/DatePartition.py` & `sefazetllib-0.1.56/sefazetllib/utils/partition/DatePartition.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from datetime import date
-from typing import Optional
-
-from sefazetllib.Builder import Builder
-from sefazetllib.utils.partition.IncrementalRangePartition import (
-    IncrementalRangePartition,
-)
-from sefazetllib.utils.partition.Partition import Partition
-
-
-@Builder
-class DatePartition(Partition):
-    """
-    Implementation of the abstract base class 'Partition' for date partitioning.
-
-    Defines the methods to format and build the partition.
-    """
-
-    year: Optional[str] = None
-    month: Optional[str] = None
-    day: Optional[str] = None
-    years: Optional[IncrementalRangePartition] = None
-    months: Optional[IncrementalRangePartition] = None
-    days: Optional[IncrementalRangePartition] = None
-
-    def __format_partition(self, partition):
-        """Format the given partition.
-
-        Parameters:
-            partition: The partition to be formatted.
-
-        Returns:
-            The formatted partition.
-        """
-        return f"{set(partition.get())}".replace(" ", "")
-
-    def __build_partition(self):
-        """Build the partition.
-
-        Returns:
-            The list of strings representing the partition.
-        """
-        partition = [
-            self.__format_partition(self.years) if bool(self.years) else self.year
-        ]
-
-        if bool(self.month) or bool(self.months):
-            partition.append(
-                self.__format_partition(self.months)
-                if bool(self.months)
-                else self.month
-            )
-
-        if bool(self.day) or bool(self.days):
-            partition.append(
-                self.__format_partition(self.days) if bool(self.days) else self.day
-            )
-
-        return partition
-
-    def get(self):
-        """Get the partition.
-
-        Returns:
-            The list of strings representing the partition.
-        """
-        return self.__build_partition()
-
-    def get_date(self):
-        """Get the date of the partition.
-
-        Returns:
-            The date of the partition in the format 'YYYY/MM/DD'.
-        """
-        return date(*self.__build_partition()).strftime("%Y/%m/%d")
+from datetime import date
+from typing import Optional
+
+from sefazetllib.Builder import Builder
+from sefazetllib.utils.partition.IncrementalRangePartition import (
+    IncrementalRangePartition,
+)
+from sefazetllib.utils.partition.Partition import Partition
+
+
+@Builder
+class DatePartition(Partition):
+    """
+    Implementation of the abstract base class 'Partition' for date partitioning.
+
+    Defines the methods to format and build the partition.
+    """
+
+    year: Optional[str] = None
+    month: Optional[str] = None
+    day: Optional[str] = None
+    years: Optional[IncrementalRangePartition] = None
+    months: Optional[IncrementalRangePartition] = None
+    days: Optional[IncrementalRangePartition] = None
+
+    def __format_partition(self, partition):
+        """Format the given partition.
+
+        Parameters:
+            partition: The partition to be formatted.
+
+        Returns:
+            The formatted partition.
+        """
+        return f"{set(partition.get())}".replace(" ", "")
+
+    def __build_partition(self):
+        """Build the partition.
+
+        Returns:
+            The list of strings representing the partition.
+        """
+        partition = [
+            self.__format_partition(self.years) if bool(self.years) else self.year
+        ]
+
+        if bool(self.month) or bool(self.months):
+            partition.append(
+                self.__format_partition(self.months)
+                if bool(self.months)
+                else self.month
+            )
+
+        if bool(self.day) or bool(self.days):
+            partition.append(
+                self.__format_partition(self.days) if bool(self.days) else self.day
+            )
+
+        return partition
+
+    def get(self):
+        """Get the partition.
+
+        Returns:
+            The list of strings representing the partition.
+        """
+        return self.__build_partition()
+
+    def get_date(self):
+        """Get the date of the partition.
+
+        Returns:
+            The date of the partition in the format 'YYYY/MM/DD'.
+        """
+        return date(*self.__build_partition()).strftime("%Y/%m/%d")
```

### Comparing `sefazetllib-0.1.55/sefazetllib/validate/DataValidate.py` & `sefazetllib-0.1.56/sefazetllib/validate/DataValidate.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,214 +1,214 @@
-from typing import Any, List, Optional
-
-from pydeequ.checks import Check, CheckLevel
-from pydeequ.verification import VerificationResult, VerificationSuite
-from pyspark.sql import Row
-from pyspark.sql.functions import col
-
-from sefazetllib import Builder, field
-from sefazetllib.factory.platform.dataframe.Default import Default
-from sefazetllib.factory.platform.Platform import Platform
-from sefazetllib.validate.Validate import Validate
-
-
-@Builder
-class DataValidate(Validate):
-    df: Optional[Any] = None
-    check: Optional[Any] = None
-    check_name: str = field(default="")
-    custom_check: List[dict] = field(default_factory=list)
-    reference: str = field(default="")
-    output: str = field(default="")
-    platform: Platform = field(default=Default())
-    table_validation: dict = field(default_factory=dict)
-    column_validation: dict = field(default_factory=dict)
-
-    def __get_lambda_assert(self, operator, value):
-        return {
-            "gt": lambda x: x > value,
-            "gte": lambda x: x >= value,
-            "lw": lambda x: x < value,
-            "lwe": lambda x: x <= value,
-            "e": lambda x: x == value,
-        }[operator]
-
-    def __set_custom_check(self, status=False, constraint="", constraint_message=""):
-        if status:
-            self.custom_check.append(
-                {
-                    "check": self.check_name,
-                    "check_level": "Error",
-                    "check_status": "Success",
-                    "constraint": constraint,
-                    "constraint_status": "Success",
-                    "constraint_message": constraint_message,
-                }
-            )
-        else:
-            self.custom_check.append(
-                {
-                    "check": self.check_name,
-                    "check_level": "Error",
-                    "check_status": "Error",
-                    "constraint": constraint,
-                    "constraint_status": "Failure",
-                    "constraint_message": constraint_message,
-                }
-            )
-
-    def __check_columns(self, columns):
-        missing_columns = list(filter(lambda col: col not in self.df.columns, columns))
-        if not missing_columns:
-            self.__set_custom_check(
-                status=True, constraint=f"ColumnsConstraint(Columns({self.reference}))"
-            )
-        else:
-            self.__set_custom_check(
-                status=False,
-                constraint=f"ColumnsConstraint(Columns({self.reference}))",
-                constraint_message=(f"Missing columns: {missing_columns}"),
-            )
-
-    def __check_size(self, assertion, hook_reference):
-        if "reference" in assertion:
-            comparison_df = hook_reference(assertion["reference"])
-
-        if "operator" not in assertion:
-            assertion["operator"] = "igual"
-
-        if "column_reference" not in assertion:
-            assertion["column_reference"] = self.df.columns
-
-        if "value" not in assertion:
-            assertion["value"] = comparison_df.select(
-                assertion["column_reference"]
-            ).count()
-
-        self.check.hasSize(
-            self.__get_lambda_assert(
-                assertion["operator"],
-                assertion["value"],
-            )
-        )
-
-    def __check_distinctness(self, assertion):
-        if assertion:
-            self.check.hasDistinctness(self.df.columns, lambda x: x == 1.0)
-
-    def __unique_key(self, assertion):
-        unique_check = (
-            self.df.groupBy(assertion).count().filter(col("count") > 1).count()
-        )
-
-        if unique_check == 0:
-            self.__set_custom_check(
-                status=True,
-                constraint=f"UniqueKeyConstraint(Columns({assertion}))",
-            )
-        else:
-            self.__set_custom_check(
-                status=False,
-                constraint=f"UniqueKeyConstraint(Columns({assertion}))",
-                constraint_message=(f"Columns {assertion} are not a unique key"),
-            )
-
-    def __check_completeness(self, column, assertion):
-        if isinstance(assertion, dict):
-            self.check.hasCompleteness(
-                column,
-                self.__get_lambda_assert(assertion["operator"], assertion["value"]),
-            )
-        elif assertion:
-            self.check.isComplete(column)
-
-    def __check_uniqueness(self, column, assertion):
-        if isinstance(assertion, dict):
-            self.check.hasUniqueness(
-                [column],
-                self.__get_lambda_assert(assertion["operator"], assertion["value"]),
-            )
-        elif assertion:
-            self.check.isUnique(column)
-
-    def __check_data_type(self, column, column_type):
-        assert_column_type = dict((key, value) for key, value in self.df.dtypes)[column]
-
-        if column_type == assert_column_type:
-            self.__set_custom_check(
-                status=True,
-                constraint=f"DataTypeConstraint(DataType({column}, {column_type}))",
-            )
-        else:
-            self.__set_custom_check(
-                status=False,
-                constraint=f"DataTypeConstraint(DataType({column}, {column_type}))",
-                constraint_message=(
-                    f"{column} of type '{assert_column_type}'"
-                    f"does not meet type '{column_type}' requirement!"
-                ),
-            )
-
-    def __check_min(self, column, value):
-        self.check.hasMin(column, lambda x: x >= value)
-
-    def __check_max(self, column, value):
-        self.check.hasMax(column, lambda x: x <= value)
-
-    def execute(self, **kwargs):
-        if isinstance(self.platform, Default):
-            self.setPlatform(kwargs["platform"])
-
-        if self.check_name == "":
-            self.check_name = f"validacao_{self.reference}"
-
-        self.check = Check(self.platform.session, CheckLevel.Error, self.check_name)
-
-        check_call_map = {
-            "columns": self.__check_columns,
-            "size": self.__check_size,
-            "distinctness": self.__check_distinctness,
-            "unique_key": self.__unique_key,
-            "completeness": self.__check_completeness,
-            "uniqueness": self.__check_uniqueness,
-            "data_type": self.__check_data_type,
-            "min": self.__check_min,
-            "max": self.__check_max,
-            "contained": self.check.isContainedIn,
-        }
-
-        for verification, assertion in self.table_validation.items():
-            if verification == "size":
-                check_call_map[verification](assertion, kwargs["hook_reference"])
-            else:
-                check_call_map[verification](assertion)
-
-        for column, assertion in self.column_validation.items():
-            for verification in assertion.keys():
-                check_call_map[verification](column, assertion[verification])
-
-        if self.custom_check:
-            return (
-                self.output,
-                VerificationResult.checkResultsAsDataFrame(
-                    self.platform.session,
-                    VerificationSuite(self.platform.session)
-                    .onData(self.df)
-                    .addCheck(self.check)
-                    .run(),
-                ).union(
-                    self.platform.session.createDataFrame(
-                        Row(**i) for i in self.custom_check
-                    )
-                ),
-            )
-
-        return (
-            self.output,
-            VerificationResult.checkResultsAsDataFrame(
-                self.platform.session,
-                VerificationSuite(self.platform.session)
-                .onData(self.df)
-                .addCheck(self.check)
-                .run(),
-            ),
-        )
+from typing import Any, List, Optional
+
+from pydeequ.checks import Check, CheckLevel
+from pydeequ.verification import VerificationResult, VerificationSuite
+from pyspark.sql import Row
+from pyspark.sql.functions import col
+
+from sefazetllib import Builder, field
+from sefazetllib.factory.platform.dataframe.Default import Default
+from sefazetllib.factory.platform.Platform import Platform
+from sefazetllib.validate.Validate import Validate
+
+
+@Builder
+class DataValidate(Validate):
+    df: Optional[Any] = None
+    check: Optional[Any] = None
+    check_name: str = field(default="")
+    custom_check: List[dict] = field(default_factory=list)
+    reference: str = field(default="")
+    output: str = field(default="")
+    platform: Platform = field(default=Default())
+    table_validation: dict = field(default_factory=dict)
+    column_validation: dict = field(default_factory=dict)
+
+    def __get_lambda_assert(self, operator, value):
+        return {
+            "gt": lambda x: x > value,
+            "gte": lambda x: x >= value,
+            "lw": lambda x: x < value,
+            "lwe": lambda x: x <= value,
+            "e": lambda x: x == value,
+        }[operator]
+
+    def __set_custom_check(self, status=False, constraint="", constraint_message=""):
+        if status:
+            self.custom_check.append(
+                {
+                    "check": self.check_name,
+                    "check_level": "Error",
+                    "check_status": "Success",
+                    "constraint": constraint,
+                    "constraint_status": "Success",
+                    "constraint_message": constraint_message,
+                }
+            )
+        else:
+            self.custom_check.append(
+                {
+                    "check": self.check_name,
+                    "check_level": "Error",
+                    "check_status": "Error",
+                    "constraint": constraint,
+                    "constraint_status": "Failure",
+                    "constraint_message": constraint_message,
+                }
+            )
+
+    def __check_columns(self, columns):
+        missing_columns = list(filter(lambda col: col not in self.df.columns, columns))
+        if not missing_columns:
+            self.__set_custom_check(
+                status=True, constraint=f"ColumnsConstraint(Columns({self.reference}))"
+            )
+        else:
+            self.__set_custom_check(
+                status=False,
+                constraint=f"ColumnsConstraint(Columns({self.reference}))",
+                constraint_message=(f"Missing columns: {missing_columns}"),
+            )
+
+    def __check_size(self, assertion, hook_reference):
+        if "reference" in assertion:
+            comparison_df = hook_reference(assertion["reference"])
+
+        if "operator" not in assertion:
+            assertion["operator"] = "igual"
+
+        if "column_reference" not in assertion:
+            assertion["column_reference"] = self.df.columns
+
+        if "value" not in assertion:
+            assertion["value"] = comparison_df.select(
+                assertion["column_reference"]
+            ).count()
+
+        self.check.hasSize(
+            self.__get_lambda_assert(
+                assertion["operator"],
+                assertion["value"],
+            )
+        )
+
+    def __check_distinctness(self, assertion):
+        if assertion:
+            self.check.hasDistinctness(self.df.columns, lambda x: x == 1.0)
+
+    def __unique_key(self, assertion):
+        unique_check = (
+            self.df.groupBy(assertion).count().filter(col("count") > 1).count()
+        )
+
+        if unique_check == 0:
+            self.__set_custom_check(
+                status=True,
+                constraint=f"UniqueKeyConstraint(Columns({assertion}))",
+            )
+        else:
+            self.__set_custom_check(
+                status=False,
+                constraint=f"UniqueKeyConstraint(Columns({assertion}))",
+                constraint_message=(f"Columns {assertion} are not a unique key"),
+            )
+
+    def __check_completeness(self, column, assertion):
+        if isinstance(assertion, dict):
+            self.check.hasCompleteness(
+                column,
+                self.__get_lambda_assert(assertion["operator"], assertion["value"]),
+            )
+        elif assertion:
+            self.check.isComplete(column)
+
+    def __check_uniqueness(self, column, assertion):
+        if isinstance(assertion, dict):
+            self.check.hasUniqueness(
+                [column],
+                self.__get_lambda_assert(assertion["operator"], assertion["value"]),
+            )
+        elif assertion:
+            self.check.isUnique(column)
+
+    def __check_data_type(self, column, column_type):
+        assert_column_type = dict((key, value) for key, value in self.df.dtypes)[column]
+
+        if column_type == assert_column_type:
+            self.__set_custom_check(
+                status=True,
+                constraint=f"DataTypeConstraint(DataType({column}, {column_type}))",
+            )
+        else:
+            self.__set_custom_check(
+                status=False,
+                constraint=f"DataTypeConstraint(DataType({column}, {column_type}))",
+                constraint_message=(
+                    f"{column} of type '{assert_column_type}'"
+                    f"does not meet type '{column_type}' requirement!"
+                ),
+            )
+
+    def __check_min(self, column, value):
+        self.check.hasMin(column, lambda x: x >= value)
+
+    def __check_max(self, column, value):
+        self.check.hasMax(column, lambda x: x <= value)
+
+    def execute(self, **kwargs):
+        if isinstance(self.platform, Default):
+            self.setPlatform(kwargs["platform"])
+
+        if self.check_name == "":
+            self.check_name = f"validacao_{self.reference}"
+
+        self.check = Check(self.platform.session, CheckLevel.Error, self.check_name)
+
+        check_call_map = {
+            "columns": self.__check_columns,
+            "size": self.__check_size,
+            "distinctness": self.__check_distinctness,
+            "unique_key": self.__unique_key,
+            "completeness": self.__check_completeness,
+            "uniqueness": self.__check_uniqueness,
+            "data_type": self.__check_data_type,
+            "min": self.__check_min,
+            "max": self.__check_max,
+            "contained": self.check.isContainedIn,
+        }
+
+        for verification, assertion in self.table_validation.items():
+            if verification == "size":
+                check_call_map[verification](assertion, kwargs["hook_reference"])
+            else:
+                check_call_map[verification](assertion)
+
+        for column, assertion in self.column_validation.items():
+            for verification in assertion.keys():
+                check_call_map[verification](column, assertion[verification])
+
+        if self.custom_check:
+            return (
+                self.output,
+                VerificationResult.checkResultsAsDataFrame(
+                    self.platform.session,
+                    VerificationSuite(self.platform.session)
+                    .onData(self.df)
+                    .addCheck(self.check)
+                    .run(),
+                ).union(
+                    self.platform.session.createDataFrame(
+                        Row(**i) for i in self.custom_check
+                    )
+                ),
+            )
+
+        return (
+            self.output,
+            VerificationResult.checkResultsAsDataFrame(
+                self.platform.session,
+                VerificationSuite(self.platform.session)
+                .onData(self.df)
+                .addCheck(self.check)
+                .run(),
+            ),
+        )
```

### Comparing `sefazetllib-0.1.55/sefazetllibcli/__init__.py` & `sefazetllib-0.1.56/sefazetllibcli/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-import json
-import os
-from pathlib import Path
-
-import click
-import yaml
-
-from .config.logging import logger
-from .generators.etl_generator import ETLGenerator
-
-
-def read_entities(source, source_extension, target_extension):
-    extension_file = os.path.splitext(source)[1]
-    is_folder = not extension_file
-    if is_folder:
-        sources = [
-            f"{source}/{file}"
-            for file in filter(
-                lambda file: source_extension in file, os.listdir(source)
-            )
-        ]
-    else:
-        sources = [source]
-    method = {
-        ".json": json.load,
-        ".yaml": yaml.safe_load,
-    }.get(source_extension, lambda textio: textio.read())
-
-    for src in sources:
-        try:
-            with open(src, "r", encoding="utf-8") as file:
-                yield (
-                    f"{os.path.splitext(os.path.basename(src))[0]}{target_extension}",
-                    method(file),
-                )
-        except Exception as err:
-            logger.error("Um erro ocorreu na leitura dos arquivos: %s", err)
-
-
-@click.version_option(message="Sefazetllib (v%(version)s)")
-@click.group(invoke_without_command=True)
-@click.option(
-    "-t",
-    "--type",
-    type=click.Choice(["json", "yaml"]),
-    default="json",
-    help="File Type",
-)
-@click.option(
-    "--template",
-    type=click.Choice(["sefazetllib"]),
-    default="sefazetllib",
-    help="Template",
-)
-@click.pass_context
-def cli(ctx, type, template):
-    ctx.ensure_object(dict)
-    ctx.obj["extension"] = f".{type}"
-    ctx.obj["generator"] = ETLGenerator
-
-
-@cli.command()
-@click.argument("source", type=click.Path(exists=True))
-@click.argument("target")
-@click.pass_context
-def generate(ctx, source, target):
-    entities = read_entities(source, ctx.obj["extension"], ".py")
-    generator = ctx.obj["generator"](list(entities), target=target)
-    generator.generate()
-
-
-@cli.command()
-@click.argument("source", type=click.Path(exists=True))
-@click.argument("target")
-@click.pass_context
-def derive(ctx, source, target):
-    entities = read_entities(source, ".py", ctx.obj["extension"])
-    generator = ctx.obj["generator"](list(entities), target=target)
-    generator.derive()
-
-
-@cli.command()
-@click.pass_context
-def derive_all(ctx):
-    for path in Path(Path.cwd()).rglob("*.py"):
-        entities = read_entities(str(path.absolute()), ".py", ctx.obj["extension"])
-        generator = ctx.obj["generator"](list(entities), target=f"doc")
-        generator.derive()
-
-
-@cli.command()
-@click.pass_context
-def dependencias(ctx):
-    def verify_optional(extract):
-        try:
-            extract["optional"]
-            return False
-        except:
-            return True
-
-    for path in Path(f"{Path.cwd()}/doc").rglob("*.json"):
-        dependencys = {}
-
-        with open(path) as jsonfile:
-            file_json = json.load(jsonfile)
-            extracts = list(
-                map(
-                    lambda extract: f"{extract['schema']}/{extract['entity']}",
-                    filter(
-                        verify_optional,
-                        filter(lambda etl: etl["type"] == "extract", file_json["ETL"]),
-                    ),
-                )
-            )
-
-            dependencys[file_json["platform"]["name"]] = {
-                extract: False for extract in extracts
-            }
-
-            folder = str(path).replace("doc", "dependencias")
-
-            os.makedirs(os.path.dirname(folder), exist_ok=True)
-            with open(folder, "w+") as f:
-                json.dump(dependencys, f, ensure_ascii=False, indent=4)
+import json
+import os
+from pathlib import Path
+
+import click
+import yaml
+
+from .config.logging import logger
+from .generators.etl_generator import ETLGenerator
+
+
+def read_entities(source, source_extension, target_extension):
+    extension_file = os.path.splitext(source)[1]
+    is_folder = not extension_file
+    if is_folder:
+        sources = [
+            f"{source}/{file}"
+            for file in filter(
+                lambda file: source_extension in file, os.listdir(source)
+            )
+        ]
+    else:
+        sources = [source]
+    method = {
+        ".json": json.load,
+        ".yaml": yaml.safe_load,
+    }.get(source_extension, lambda textio: textio.read())
+
+    for src in sources:
+        try:
+            with open(src, "r", encoding="utf-8") as file:
+                yield (
+                    f"{os.path.splitext(os.path.basename(src))[0]}{target_extension}",
+                    method(file),
+                )
+        except Exception as err:
+            logger.error("Um erro ocorreu na leitura dos arquivos: %s", err)
+
+
+@click.version_option(message="Sefazetllib (v%(version)s)")
+@click.group(invoke_without_command=True)
+@click.option(
+    "-t",
+    "--type",
+    type=click.Choice(["json", "yaml"]),
+    default="json",
+    help="File Type",
+)
+@click.option(
+    "--template",
+    type=click.Choice(["sefazetllib"]),
+    default="sefazetllib",
+    help="Template",
+)
+@click.pass_context
+def cli(ctx, type, template):
+    ctx.ensure_object(dict)
+    ctx.obj["extension"] = f".{type}"
+    ctx.obj["generator"] = ETLGenerator
+
+
+@cli.command()
+@click.argument("source", type=click.Path(exists=True))
+@click.argument("target")
+@click.pass_context
+def generate(ctx, source, target):
+    entities = read_entities(source, ctx.obj["extension"], ".py")
+    generator = ctx.obj["generator"](list(entities), target=target)
+    generator.generate()
+
+
+@cli.command()
+@click.argument("source", type=click.Path(exists=True))
+@click.argument("target")
+@click.pass_context
+def derive(ctx, source, target):
+    entities = read_entities(source, ".py", ctx.obj["extension"])
+    generator = ctx.obj["generator"](list(entities), target=target)
+    generator.derive()
+
+
+@cli.command()
+@click.pass_context
+def derive_all(ctx):
+    for path in Path(Path.cwd()).rglob("*.py"):
+        entities = read_entities(str(path.absolute()), ".py", ctx.obj["extension"])
+        generator = ctx.obj["generator"](list(entities), target=f"doc")
+        generator.derive()
+
+
+@cli.command()
+@click.pass_context
+def dependencias(ctx):
+    def verify_optional(extract):
+        try:
+            extract["optional"]
+            return False
+        except:
+            return True
+
+    for path in Path(f"{Path.cwd()}/doc").rglob("*.json"):
+        dependencys = {}
+
+        with open(path) as jsonfile:
+            file_json = json.load(jsonfile)
+            extracts = list(
+                map(
+                    lambda extract: f"{extract['schema']}/{extract['entity']}",
+                    filter(
+                        verify_optional,
+                        filter(lambda etl: etl["type"] == "extract", file_json["ETL"]),
+                    ),
+                )
+            )
+
+            dependencys[file_json["platform"]["name"]] = {
+                extract: False for extract in extracts
+            }
+
+            folder = str(path).replace("doc", "dependencias")
+
+            os.makedirs(os.path.dirname(folder), exist_ok=True)
+            with open(folder, "w+") as f:
+                json.dump(dependencys, f, ensure_ascii=False, indent=4)
```

### Comparing `sefazetllib-0.1.55/sefazetllibcli/config/logging.py` & `sefazetllib-0.1.56/sefazetllibcli/config/logging.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import logging
-
-
-class CustomFormatter(logging.Formatter):
-    """Logging Formatter to add colors and count warning / errors."""
-
-    grey = '\x1b[38;21m'
-    yellow = '\x1b[33;21m'
-    red = '\x1b[31;21m'
-    bold_red = '\x1b[31;1m'
-    reset = '\x1b[0m'
-    info_format = '[%(asctime)s] [%(levelname)s] %(message)s'
-    error_format = '[%(asctime)s] [%(levelname)s] %(message)s (%(module)s.%(funcName)s:%(lineno)d)'
-
-    FORMATS = {
-        logging.DEBUG: grey + info_format + reset,
-        logging.INFO: grey + info_format + reset,
-        logging.WARNING: yellow + error_format + reset,
-        logging.ERROR: red + error_format + reset,
-        logging.CRITICAL: bold_red + error_format + reset,
-    }
-
-    def format(self, record):
-        log_fmt = self.FORMATS.get(record.levelno)
-        formatter = logging.Formatter(log_fmt, datefmt='%Y-%m-%d %H:%M:%S')
-        return formatter.format(record)
-
-
-handler = logging.StreamHandler()
-handler.setFormatter(CustomFormatter())
-handler.setLevel(logging.INFO)
-
-logger = logging.getLogger('sefazetllibcli')
-
-logger.setLevel(logging.INFO)
-logger.addHandler(handler)
+import logging
+
+
+class CustomFormatter(logging.Formatter):
+    """Logging Formatter to add colors and count warning / errors."""
+
+    grey = '\x1b[38;21m'
+    yellow = '\x1b[33;21m'
+    red = '\x1b[31;21m'
+    bold_red = '\x1b[31;1m'
+    reset = '\x1b[0m'
+    info_format = '[%(asctime)s] [%(levelname)s] %(message)s'
+    error_format = '[%(asctime)s] [%(levelname)s] %(message)s (%(module)s.%(funcName)s:%(lineno)d)'
+
+    FORMATS = {
+        logging.DEBUG: grey + info_format + reset,
+        logging.INFO: grey + info_format + reset,
+        logging.WARNING: yellow + error_format + reset,
+        logging.ERROR: red + error_format + reset,
+        logging.CRITICAL: bold_red + error_format + reset,
+    }
+
+    def format(self, record):
+        log_fmt = self.FORMATS.get(record.levelno)
+        formatter = logging.Formatter(log_fmt, datefmt='%Y-%m-%d %H:%M:%S')
+        return formatter.format(record)
+
+
+handler = logging.StreamHandler()
+handler.setFormatter(CustomFormatter())
+handler.setLevel(logging.INFO)
+
+logger = logging.getLogger('sefazetllibcli')
+
+logger.setLevel(logging.INFO)
+logger.addHandler(handler)
```

### Comparing `sefazetllib-0.1.55/sefazetllibcli/generators/etl_generator.py` & `sefazetllib-0.1.56/sefazetllibcli/generators/etl_generator.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-import json
-import os
-import re
-from dataclasses import dataclass, field
-from pathlib import Path
-
-import yaml
-
-from sefazetllibcli.config.logging import logger
-from sefazetllibcli.errors import UnsupportedFileExtension
-from sefazetllibcli.usecases.replace_template import ReplaceETLTemplate, ReplaceTemplate
-from sefazetllibcli.utils import ParseETL
-
-from .generator import Generator
-
-
-@dataclass
-class ETLGenerator(Generator):
-    template_file: str = field(
-        default=Path(__file__).parent / "../templates/etl_template"
-    )
-    __parse_etl: ParseETL = field(default=ParseETL())
-    replace_template: ReplaceTemplate = field(default=ReplaceETLTemplate)
-
-    def generate(self) -> None:
-        for i, entity in enumerate(self.entities):
-            try:
-                etl_name, etl = entity
-
-                logger.info(
-                    "[%s/%s] Iniciando geração do ETL `%s`",
-                    i + 1,
-                    len(self.entities),
-                    etl_name,
-                )
-
-                logger.info("Executando...")
-
-                replace_template = self.replace_template(
-                    template=self.template,
-                    entity=etl,
-                    sources=None,
-                    columns=None,
-                )
-
-                output = replace_template.replace()
-
-                logger.info("Gravando...")
-
-                path = f"{self.target}/{etl_name}"
-                os.makedirs(os.path.dirname(path), exist_ok=True)
-
-                with open(
-                    path,
-                    "w",
-                    encoding="utf-8",
-                ) as file__output:
-                    file__output.write(output)
-
-                logger.info(
-                    "[%s/%s] Geração do ETL `%s` concluída!",
-                    i + 1,
-                    len(self.entities),
-                    etl_name,
-                )
-            except Exception as err:
-                logger.error(
-                    "[%s/%s] Um erro ocorreu na geração do ETL `%s`: %s",
-                    i + 1,
-                    len(self.entities),
-                    etl_name,
-                    err,
-                )
-
-    def derive(self) -> None:
-        for i, entity in enumerate(self.entities):
-            try:
-                etl_name, etl = entity
-
-                logger.info(
-                    "[%s/%s] Iniciando derivação do ETL `%s`",
-                    i + 1,
-                    len(self.entities),
-                    etl_name,
-                )
-
-                logger.info("Executando...")
-
-                # print(self.__get_etl_context(etl))
-                # self.__get_transform_context(etl)
-                # print(self.__get_imports(etl))
-
-                output = self.__parse_etl.parse(self.__get_etl_context(etl))
-
-                path = f"{self.target}/{etl_name}"
-                os.makedirs(os.path.dirname(path), exist_ok=True)
-
-                with Path(path).open("w", encoding="utf-8") as file__output:
-                    extension_file = os.path.splitext(path)[1]
-                    if extension_file == ".json":
-                        file__output.write(json.dumps(output, indent=4))
-                    elif extension_file == ".yaml":
-                        file__output.write(yaml.dump(output, indent=4))
-                    else:
-                        raise UnsupportedFileExtension(
-                            f"Extensão de arquivo não suportada: {path}"
-                        )
-
-                # with open(
-                #     path,
-                #     "w",
-                #     encoding="utf-8",
-                # ) as file__output:
-                #     extension_file = os.path.splitext(path)[1]
-                #     if extension_file == ".json":
-                #         file__output.write(json.dumps(output, indent=4))
-                #     elif extension_file == ".yaml":
-                #         file__output.write(yaml.dump(output, indent=4))
-                #     else:
-                #         raise UnsupportedFileExtension(
-                #             f"Extensão de arquivo não suportada: {path}"
-                #         )
-
-                logger.info(
-                    "[%s/%s] Derivação do ETL `%s` concluída!",
-                    i + 1,
-                    len(self.entities),
-                    etl_name,
-                )
-            except Exception as err:
-                logger.error(
-                    "[%s/%s] Um erro ocorreu na geração do ETL `%s`: %s",
-                    i + 1,
-                    len(self.entities),
-                    etl_name,
-                    err,
-                )
-
-    def __get_etl_context(self, script):
-        etl_pattern = re.compile(r"\((ETL.*)\)$")
-
-        minified = re.sub(r"\s", "", script)
-        return etl_pattern.search(minified).group(1)
-
-    def __get_transform_context(self, script):
-        etl_pattern = re.compile(r"(@Builder[\s\S]*?)(?=\n{3})")
-
-        transforms = etl_pattern.findall(script)
-
-        for transform in transforms:
-            self.__get_transform_references(transform)
-            self.__get_transform_setup(transform)
-            self.__get_transform_private_methods(transform)
-            self.__get_transform_method(transform)
-
-        # return etl_pattern.search(minified).group(1)
-
-    def __get_transform_references(self, transform):
-        etl_pattern = re.compile(r"([(A-Z)|(a-z)].*?): Optional\[DataFrame\] = None")
-
-        return etl_pattern.findall(transform)
-
-    def __get_transform_setup(self, transform):
-        etl_pattern = re.compile(
-            r"self.__(\w[A-Z|a-z].*) = (Window*[\s\S]*?\)\n|[^\(][\s\S]*?\n|\([\s\S]*?\s\))"
-        )
-
-        return etl_pattern.findall(transform)
-
-    def __get_transform_private_methods(self, transform):
-        etl_pattern = re.compile(r"def __(\w[A-Z|a-z].*)\(self\):([^\(][\s\S]*?\s\n)")
-
-        return etl_pattern.findall(transform)
-
-    def __get_transform_method(self, transform):
-        etl_pattern = re.compile(
-            r"def execute\(self\) \-> Tuple\[str, DataFrame\]:([\s\S]*?)\sreturn.*\n\s*.?\"([\s\S].*)\"\,([\s\S]*?)\)\n\n"
-        )
-        print(etl_pattern.findall(etl_pattern))
-
-    def __get_imports(self, etl):
-        etl_pattern = re.compile(
-            r"from ([^sefazetllib]\w.*) import ([^\(][\s\S]*?\n|[\(][\s\S]*?\s[\)])"
-        )
-        return etl_pattern.findall(etl)
+import json
+import os
+import re
+from dataclasses import dataclass, field
+from pathlib import Path
+
+import yaml
+
+from sefazetllibcli.config.logging import logger
+from sefazetllibcli.errors import UnsupportedFileExtension
+from sefazetllibcli.usecases.replace_template import ReplaceETLTemplate, ReplaceTemplate
+from sefazetllibcli.utils import ParseETL
+
+from .generator import Generator
+
+
+@dataclass
+class ETLGenerator(Generator):
+    template_file: str = field(
+        default=Path(__file__).parent / "../templates/etl_template"
+    )
+    __parse_etl: ParseETL = field(default=ParseETL())
+    replace_template: ReplaceTemplate = field(default=ReplaceETLTemplate)
+
+    def generate(self) -> None:
+        for i, entity in enumerate(self.entities):
+            try:
+                etl_name, etl = entity
+
+                logger.info(
+                    "[%s/%s] Iniciando geração do ETL `%s`",
+                    i + 1,
+                    len(self.entities),
+                    etl_name,
+                )
+
+                logger.info("Executando...")
+
+                replace_template = self.replace_template(
+                    template=self.template,
+                    entity=etl,
+                    sources=None,
+                    columns=None,
+                )
+
+                output = replace_template.replace()
+
+                logger.info("Gravando...")
+
+                path = f"{self.target}/{etl_name}"
+                os.makedirs(os.path.dirname(path), exist_ok=True)
+
+                with open(
+                    path,
+                    "w",
+                    encoding="utf-8",
+                ) as file__output:
+                    file__output.write(output)
+
+                logger.info(
+                    "[%s/%s] Geração do ETL `%s` concluída!",
+                    i + 1,
+                    len(self.entities),
+                    etl_name,
+                )
+            except Exception as err:
+                logger.error(
+                    "[%s/%s] Um erro ocorreu na geração do ETL `%s`: %s",
+                    i + 1,
+                    len(self.entities),
+                    etl_name,
+                    err,
+                )
+
+    def derive(self) -> None:
+        for i, entity in enumerate(self.entities):
+            try:
+                etl_name, etl = entity
+
+                logger.info(
+                    "[%s/%s] Iniciando derivação do ETL `%s`",
+                    i + 1,
+                    len(self.entities),
+                    etl_name,
+                )
+
+                logger.info("Executando...")
+
+                # print(self.__get_etl_context(etl))
+                # self.__get_transform_context(etl)
+                # print(self.__get_imports(etl))
+
+                output = self.__parse_etl.parse(self.__get_etl_context(etl))
+
+                path = f"{self.target}/{etl_name}"
+                os.makedirs(os.path.dirname(path), exist_ok=True)
+
+                with Path(path).open("w", encoding="utf-8") as file__output:
+                    extension_file = os.path.splitext(path)[1]
+                    if extension_file == ".json":
+                        file__output.write(json.dumps(output, indent=4))
+                    elif extension_file == ".yaml":
+                        file__output.write(yaml.dump(output, indent=4))
+                    else:
+                        raise UnsupportedFileExtension(
+                            f"Extensão de arquivo não suportada: {path}"
+                        )
+
+                # with open(
+                #     path,
+                #     "w",
+                #     encoding="utf-8",
+                # ) as file__output:
+                #     extension_file = os.path.splitext(path)[1]
+                #     if extension_file == ".json":
+                #         file__output.write(json.dumps(output, indent=4))
+                #     elif extension_file == ".yaml":
+                #         file__output.write(yaml.dump(output, indent=4))
+                #     else:
+                #         raise UnsupportedFileExtension(
+                #             f"Extensão de arquivo não suportada: {path}"
+                #         )
+
+                logger.info(
+                    "[%s/%s] Derivação do ETL `%s` concluída!",
+                    i + 1,
+                    len(self.entities),
+                    etl_name,
+                )
+            except Exception as err:
+                logger.error(
+                    "[%s/%s] Um erro ocorreu na geração do ETL `%s`: %s",
+                    i + 1,
+                    len(self.entities),
+                    etl_name,
+                    err,
+                )
+
+    def __get_etl_context(self, script):
+        etl_pattern = re.compile(r"\((ETL.*)\)$")
+
+        minified = re.sub(r"\s", "", script)
+        return etl_pattern.search(minified).group(1)
+
+    def __get_transform_context(self, script):
+        etl_pattern = re.compile(r"(@Builder[\s\S]*?)(?=\n{3})")
+
+        transforms = etl_pattern.findall(script)
+
+        for transform in transforms:
+            self.__get_transform_references(transform)
+            self.__get_transform_setup(transform)
+            self.__get_transform_private_methods(transform)
+            self.__get_transform_method(transform)
+
+        # return etl_pattern.search(minified).group(1)
+
+    def __get_transform_references(self, transform):
+        etl_pattern = re.compile(r"([(A-Z)|(a-z)].*?): Optional\[DataFrame\] = None")
+
+        return etl_pattern.findall(transform)
+
+    def __get_transform_setup(self, transform):
+        etl_pattern = re.compile(
+            r"self.__(\w[A-Z|a-z].*) = (Window*[\s\S]*?\)\n|[^\(][\s\S]*?\n|\([\s\S]*?\s\))"
+        )
+
+        return etl_pattern.findall(transform)
+
+    def __get_transform_private_methods(self, transform):
+        etl_pattern = re.compile(r"def __(\w[A-Z|a-z].*)\(self\):([^\(][\s\S]*?\s\n)")
+
+        return etl_pattern.findall(transform)
+
+    def __get_transform_method(self, transform):
+        etl_pattern = re.compile(
+            r"def execute\(self\) \-> Tuple\[str, DataFrame\]:([\s\S]*?)\sreturn.*\n\s*.?\"([\s\S].*)\"\,([\s\S]*?)\)\n\n"
+        )
+        print(etl_pattern.findall(etl_pattern))
+
+    def __get_imports(self, etl):
+        etl_pattern = re.compile(
+            r"from ([^sefazetllib]\w.*) import ([^\(][\s\S]*?\n|[\(][\s\S]*?\s[\)])"
+        )
+        return etl_pattern.findall(etl)
```

### Comparing `sefazetllib-0.1.55/sefazetllibcli/generators/generator.py` & `sefazetllib-0.1.56/sefazetllibcli/generators/generator.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from abc import ABC, abstractmethod
-from dataclasses import dataclass, field
-from io import TextIOWrapper
-
-from sefazetllibcli.errors import MethodNotImplemented
-from sefazetllibcli.usecases.replace_template import ReplaceTemplate
-
-
-@dataclass(init=False)
-class Generator(ABC):
-    entities: list = field(default_factory=list)
-    template_file: str = field(default_factory=str)
-    root_path: str = field(default_factory=str)
-    target: str = field(default_factory=str)
-    replace_template: ReplaceTemplate = field(default=None)
-    template: str = field(init=False, default=None)
-
-    def __post_init__(self):
-        with open(self.template_file, 'r', encoding='utf-8') as file_template:
-            object.__setattr__(self, 'template', file_template.read())
-
-    @abstractmethod
-    def generate(self):
-        raise MethodNotImplemented('Deve implementar o método: proccess')
+from abc import ABC, abstractmethod
+from dataclasses import dataclass, field
+from io import TextIOWrapper
+
+from sefazetllibcli.errors import MethodNotImplemented
+from sefazetllibcli.usecases.replace_template import ReplaceTemplate
+
+
+@dataclass(init=False)
+class Generator(ABC):
+    entities: list = field(default_factory=list)
+    template_file: str = field(default_factory=str)
+    root_path: str = field(default_factory=str)
+    target: str = field(default_factory=str)
+    replace_template: ReplaceTemplate = field(default=None)
+    template: str = field(init=False, default=None)
+
+    def __post_init__(self):
+        with open(self.template_file, 'r', encoding='utf-8') as file_template:
+            object.__setattr__(self, 'template', file_template.read())
+
+    @abstractmethod
+    def generate(self):
+        raise MethodNotImplemented('Deve implementar o método: proccess')
```

### Comparing `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/__init__.py` & `sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/__init__.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .process_etl_variable import ProcessETLVariable
-from .process_extract_variable import ProcessExtractVariable
-from .process_imports_variable import ProcessImportsVariable
-from .process_key_variable import ProcessKeyVariable
-from .process_load_variable import ProcessLoadVariable
-from .process_partition_variable import ProcessPartitionVariable
-from .process_transforms_variable import ProcessTransformsVariable
-from .process_validate_variable import ProcessValidateVariable
-from .process_variable import ProcessVariable
+from .process_etl_variable import ProcessETLVariable
+from .process_extract_variable import ProcessExtractVariable
+from .process_imports_variable import ProcessImportsVariable
+from .process_key_variable import ProcessKeyVariable
+from .process_load_variable import ProcessLoadVariable
+from .process_partition_variable import ProcessPartitionVariable
+from .process_transforms_variable import ProcessTransformsVariable
+from .process_validate_variable import ProcessValidateVariable
+from .process_variable import ProcessVariable
```

### Comparing `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_etl_variable.py` & `sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/process_etl_variable.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-import json
-
-from .process_variable import ProcessVariable
-
-
-class ProcessETLVariable(ProcessVariable):
-    """Classe `ProcessETLVariable`.
-
-    A classe implementa o procedimento da saída da variavel `ETL`.
-    """
-
-    variable = 'ETL'
-
-    def _get_platform(self, platform):
-        factory = platform['factory']
-        name = platform['name']
-        return (
-            f'.setPlatform(PlatformFactory("{factory}").create(name="{name}"))'
-        )
-
-    def _get_properties(self, properties, skip_columns=None, height=1):
-        props = []
-        for prop, value in properties.items():
-            if prop not in skip_columns:
-                prop_str = ''.join(
-                    [word.capitalize() for word in prop.split('_')]
-                )
-                if isinstance(value, str):
-                    value = f'"{value}"'
-                elif isinstance(value, dict):
-                    tabs = '\t' * height
-                    if 'factory' in value:
-                        value = (
-                            '\n'
-                            + tabs
-                            + '\t'
-                            + self._visit_factory(value, height + 1)
-                            + '\n'
-                            + tabs
-                        )
-                    else:
-                        value = (
-                            json.dumps(value, indent=4 * (height + 1))
-                            .replace('}', tabs + '}')
-                            .replace('true', 'True')
-                            .replace('false', 'False')
-                        )
-                props.append(f'.set{prop_str}({value})')
-        return props
-
-    def _visit_factory(self, factory, height):
-        name = f'{factory["factory"]}()'
-        properties = self._get_properties(factory, ['factory', 'type'], height)
-        tabs = '\n' + '\t' * height
-        properties = tabs.join(properties)
-        return name + tabs + properties
-
-    def _get_etl(self, etls):
-        list_etl = []
-        for etl in etls:
-            etl_type = etl['type']
-            value = (
-                etl['name']
-                if etl_type == 'transform'
-                else self._visit_factory(etl, 2)
-            )
-            tabs_ini = '\n\t\t'
-            tabs_end = '\n\t'
-            if etl_type == 'transform':
-                tabs_ini = ''
-                tabs_end = ''
-            list_etl.append(f'.{etl_type}({tabs_ini}{value}{tabs_end})')
-
-        return '\n\t'.join(list_etl)
-
-    def process(self, entity, sources, columns):
-        """Retorna uma string do processamento da variável.
-
-        Parâmetros:
-            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
-            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
-            notebook original da entidade.
-            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
-            original.
-        Saída:
-            `processed_variable (str)`: String do processamento da variável.
-        """
-        platform = '\n\t' + self._get_platform(entity['platform'])
-        properties = self._get_properties(
-            entity,
-            skip_columns=['platform', 'ETL'],
-            height=1,
-        )
-        properties = '\n\t' + '\n\t'.join(properties) if properties else ''
-        print('inicio')
-        etls = '\n\t' + self._get_etl(entity['ETL'])
-        print('fim')
-        return '(\n\tETL()' + f'{platform}{properties}{etls}\n)'
+import json
+
+from .process_variable import ProcessVariable
+
+
+class ProcessETLVariable(ProcessVariable):
+    """Classe `ProcessETLVariable`.
+
+    A classe implementa o procedimento da saída da variavel `ETL`.
+    """
+
+    variable = 'ETL'
+
+    def _get_platform(self, platform):
+        factory = platform['factory']
+        name = platform['name']
+        return (
+            f'.setPlatform(PlatformFactory("{factory}").create(name="{name}"))'
+        )
+
+    def _get_properties(self, properties, skip_columns=None, height=1):
+        props = []
+        for prop, value in properties.items():
+            if prop not in skip_columns:
+                prop_str = ''.join(
+                    [word.capitalize() for word in prop.split('_')]
+                )
+                if isinstance(value, str):
+                    value = f'"{value}"'
+                elif isinstance(value, dict):
+                    tabs = '\t' * height
+                    if 'factory' in value:
+                        value = (
+                            '\n'
+                            + tabs
+                            + '\t'
+                            + self._visit_factory(value, height + 1)
+                            + '\n'
+                            + tabs
+                        )
+                    else:
+                        value = (
+                            json.dumps(value, indent=4 * (height + 1))
+                            .replace('}', tabs + '}')
+                            .replace('true', 'True')
+                            .replace('false', 'False')
+                        )
+                props.append(f'.set{prop_str}({value})')
+        return props
+
+    def _visit_factory(self, factory, height):
+        name = f'{factory["factory"]}()'
+        properties = self._get_properties(factory, ['factory', 'type'], height)
+        tabs = '\n' + '\t' * height
+        properties = tabs.join(properties)
+        return name + tabs + properties
+
+    def _get_etl(self, etls):
+        list_etl = []
+        for etl in etls:
+            etl_type = etl['type']
+            value = (
+                etl['name']
+                if etl_type == 'transform'
+                else self._visit_factory(etl, 2)
+            )
+            tabs_ini = '\n\t\t'
+            tabs_end = '\n\t'
+            if etl_type == 'transform':
+                tabs_ini = ''
+                tabs_end = ''
+            list_etl.append(f'.{etl_type}({tabs_ini}{value}{tabs_end})')
+
+        return '\n\t'.join(list_etl)
+
+    def process(self, entity, sources, columns):
+        """Retorna uma string do processamento da variável.
+
+        Parâmetros:
+            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
+            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
+            notebook original da entidade.
+            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
+            original.
+        Saída:
+            `processed_variable (str)`: String do processamento da variável.
+        """
+        platform = '\n\t' + self._get_platform(entity['platform'])
+        properties = self._get_properties(
+            entity,
+            skip_columns=['platform', 'ETL'],
+            height=1,
+        )
+        properties = '\n\t' + '\n\t'.join(properties) if properties else ''
+        print('inicio')
+        etls = '\n\t' + self._get_etl(entity['ETL'])
+        print('fim')
+        return '(\n\tETL()' + f'{platform}{properties}{etls}\n)'
```

### Comparing `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_extract_variable.py` & `sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/process_variable.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from .process_variable import ProcessVariable
-
-
-class ProcessExtractVariable(ProcessVariable):
-    """Classe `ProcessExtractVariable`.
-
-    A classe implementa o procedimento da saída da variavel `EXTRACT`.
-    """
-
-    variable = 'EXTRACT'
-
-    def process(self, entity, sources, columns):
-        """Retorna uma string do processamento da variável.
-
-        Parâmetros:
-            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
-            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
-            notebook original da entidade.
-            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
-            original.
-        Saída:
-            `processed_variable (str)`: String do processamento da variável.
-        """
-        factories = [
-            etl['factory'] for etl in entity['ETL'] if etl['type'] == 'extract'
-        ]
-        factories_without_duplicates = [*set(factories)]
-        factories_without_duplicates.sort()
-
-        return 'from sefazetllib.extract import '+', '.join(factories_without_duplicates) if bool(factories_without_duplicates) else ''
+from abc import ABC, abstractmethod
+
+from sefazetllibcli.errors import MethodNotImplemented
+
+
+class ProcessVariable(ABC):
+    """Interface `ProcessVariable`.
+
+    A interface define como as suas classes que a implemêntam devem processar a
+    saída da variável em questão.
+    """
+
+    variable = ''
+
+    @abstractmethod
+    def process(self, entity, sources, columns):
+        """Retorna uma string do processamento da variável.
+
+        Parâmetros:
+            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
+            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
+            notebook original da entidade.
+            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
+            original.
+        Saída:
+            `processed_variable (str)`: String do processamento da variável.
+        """
+        raise MethodNotImplemented('Deve implementar o método: proccess')
```

### Comparing `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_key_variable.py` & `sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/process_extract_variable.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from .process_variable import ProcessVariable
-
-
-class ProcessKeyVariable(ProcessVariable):
-    """Classe `ProcessKeyVariable`.
-
-    A classe implementa o procedimento da saída da variavel `KEY`.
-    """
-
-    variable = 'KEY'
-
-    def process(self, entity, sources, columns):
-        """Retorna uma string do processamento da variável.
-
-        Parâmetros:
-            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
-            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
-            notebook original da entidade.
-            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
-            original.
-        Saída:
-            `processed_variable (str)`: String do processamento da variável.
-        """
-        factories = [
-            etl['key']['factory']
-            for etl in entity['ETL']
-            if etl['type'] == 'load'
-        ]
-        factories_without_duplicates = [*set(factories)]
-        factories_without_duplicates.sort()
-
-        return 'from sefazetllib.utils.key import '+', '.join(factories_without_duplicates) if bool(factories_without_duplicates) else ''
+from .process_variable import ProcessVariable
+
+
+class ProcessExtractVariable(ProcessVariable):
+    """Classe `ProcessExtractVariable`.
+
+    A classe implementa o procedimento da saída da variavel `EXTRACT`.
+    """
+
+    variable = 'EXTRACT'
+
+    def process(self, entity, sources, columns):
+        """Retorna uma string do processamento da variável.
+
+        Parâmetros:
+            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
+            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
+            notebook original da entidade.
+            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
+            original.
+        Saída:
+            `processed_variable (str)`: String do processamento da variável.
+        """
+        factories = [
+            etl['factory'] for etl in entity['ETL'] if etl['type'] == 'extract'
+        ]
+        factories_without_duplicates = [*set(factories)]
+        factories_without_duplicates.sort()
+
+        return 'from sefazetllib.extract import '+', '.join(factories_without_duplicates) if bool(factories_without_duplicates) else ''
```

### Comparing `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_partition_variable.py` & `sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/process_partition_variable.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from .process_variable import ProcessVariable
-
-
-class ProcessPartitionVariable(ProcessVariable):
-    """Classe `ProcessPartitionVariable`.
-
-    A classe implementa o procedimento da saída da variavel `PARTITION`.
-    """
-
-    variable = 'PARTITION'
-
-    def _get_factories(self, dictionary, factories):
-        for prop, value in dictionary.items():
-            if (
-                prop != 'factory'
-                and isinstance(value, dict)
-                and 'factory' in value
-            ):
-                factories.append(value['factory'])
-                self._get_factories(value, factories)
-
-    def process(self, entity, sources, columns):
-        """Retorna uma string do processamento da variável.
-
-        Parâmetros:
-            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
-            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
-            notebook original da entidade.
-            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
-            original.
-        Saída:
-            `processed_variable (str)`: String do processamento da variável.
-        """
-        if 'partition' in entity:
-            partitions = entity['partition']
-            factories = [partitions['factory']]
-            self._get_factories(entity['partition'], factories)
-
-            factories_without_duplicates = [*set(factories)]
-            factories_without_duplicates.sort()
-
-            return 'from sefazetllib.utils.partition import ' + ', '.join(
-                factories_without_duplicates
-            )
-        return ''
+from .process_variable import ProcessVariable
+
+
+class ProcessPartitionVariable(ProcessVariable):
+    """Classe `ProcessPartitionVariable`.
+
+    A classe implementa o procedimento da saída da variavel `PARTITION`.
+    """
+
+    variable = 'PARTITION'
+
+    def _get_factories(self, dictionary, factories):
+        for prop, value in dictionary.items():
+            if (
+                prop != 'factory'
+                and isinstance(value, dict)
+                and 'factory' in value
+            ):
+                factories.append(value['factory'])
+                self._get_factories(value, factories)
+
+    def process(self, entity, sources, columns):
+        """Retorna uma string do processamento da variável.
+
+        Parâmetros:
+            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
+            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
+            notebook original da entidade.
+            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
+            original.
+        Saída:
+            `processed_variable (str)`: String do processamento da variável.
+        """
+        if 'partition' in entity:
+            partitions = entity['partition']
+            factories = [partitions['factory']]
+            self._get_factories(entity['partition'], factories)
+
+            factories_without_duplicates = [*set(factories)]
+            factories_without_duplicates.sort()
+
+            return 'from sefazetllib.utils.partition import ' + ', '.join(
+                factories_without_duplicates
+            )
+        return ''
```

### Comparing `sefazetllib-0.1.55/sefazetllibcli/usecases/process_variable/process_validate_variable.py` & `sefazetllib-0.1.56/sefazetllibcli/usecases/process_variable/process_load_variable.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from .process_variable import ProcessVariable
-
-
-class ProcessValidateVariable(ProcessVariable):
-    """Classe `ProcessExtractVariable`.
-
-    A classe implementa o procedimento da saída da variavel `EXTRACT`.
-    """
-
-    variable = 'VALIDATE'
-
-    def process(self, entity, sources, columns):
-        """Retorna uma string do processamento da variável.
-
-        Parâmetros:
-            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
-            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
-            notebook original da entidade.
-            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
-            original.
-        Saída:
-            `processed_variable (str)`: String do processamento da variável.
-        """
-        factories = [
-            etl['factory']
-            for etl in entity['ETL']
-            if etl['type'] == 'validate'
-        ]
-        factories_without_duplicates = [*set(factories)]
-        factories_without_duplicates.sort()
-
-        return ', '.join(factories_without_duplicates)
+from .process_variable import ProcessVariable
+
+
+class ProcessLoadVariable(ProcessVariable):
+    """Classe `ProcessLoadVariable`.
+
+    A classe implementa o procedimento da saída da variavel `LOAD`.
+    """
+
+    variable = 'LOAD'
+
+    def process(self, entity, sources, columns):
+        """Retorna uma string do processamento da variável.
+
+        Parâmetros:
+            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
+            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
+            notebook original da entidade.
+            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
+            original.
+        Saída:
+            `processed_variable (str)`: String do processamento da variável.
+        """
+        factories = [
+            etl['factory'] for etl in entity['ETL'] if etl['type'] == 'load'
+        ]
+        factories_without_duplicates = [*set(factories)]
+        factories_without_duplicates.sort()
+
+        return 'from sefazetllib.load import '+', '.join(factories_without_duplicates) if bool(factories_without_duplicates) else ''
```

### Comparing `sefazetllib-0.1.55/sefazetllibcli/usecases/replace_template/replace_etl_template.py` & `sefazetllib-0.1.56/sefazetllibcli/usecases/replace_template/replace_etl_template.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from sefazetllibcli.usecases.process_variable import (
-    ProcessETLVariable,
-    ProcessExtractVariable,
-    ProcessImportsVariable,
-    ProcessKeyVariable,
-    ProcessLoadVariable,
-    ProcessPartitionVariable,
-    ProcessTransformsVariable,
-    ProcessValidateVariable,
-)
-
-from .replace_template import ReplaceTemplate
-
-
-class ReplaceETLTemplate(ReplaceTemplate):
-    """Classe `ReplaceETLTemplate`.
-
-    A classe tem a finalidade de substituir as variáveis que estão definidas no
-    template.
-    """
-
-    def replace(self):
-        """Retorna o template com todas variáveis da lista já substituídas."""
-        return self.replace_variables(
-            ProcessETLVariable(),
-            ProcessExtractVariable(),
-            ProcessImportsVariable(),
-            ProcessKeyVariable(),
-            ProcessLoadVariable(),
-            ProcessPartitionVariable(),
-            ProcessTransformsVariable(),
-            ProcessValidateVariable(),
-        )
+from sefazetllibcli.usecases.process_variable import (
+    ProcessETLVariable,
+    ProcessExtractVariable,
+    ProcessImportsVariable,
+    ProcessKeyVariable,
+    ProcessLoadVariable,
+    ProcessPartitionVariable,
+    ProcessTransformsVariable,
+    ProcessValidateVariable,
+)
+
+from .replace_template import ReplaceTemplate
+
+
+class ReplaceETLTemplate(ReplaceTemplate):
+    """Classe `ReplaceETLTemplate`.
+
+    A classe tem a finalidade de substituir as variáveis que estão definidas no
+    template.
+    """
+
+    def replace(self):
+        """Retorna o template com todas variáveis da lista já substituídas."""
+        return self.replace_variables(
+            ProcessETLVariable(),
+            ProcessExtractVariable(),
+            ProcessImportsVariable(),
+            ProcessKeyVariable(),
+            ProcessLoadVariable(),
+            ProcessPartitionVariable(),
+            ProcessTransformsVariable(),
+            ProcessValidateVariable(),
+        )
```

### Comparing `sefazetllib-0.1.55/sefazetllibcli/utils/parse_etl.py` & `sefazetllib-0.1.56/sefazetllibcli/utils/parse_etl.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-import ast
-import re
-
-
-class ParseETL:
-    def parse(self, string):
-        current_dict = {}
-        key = ''
-        value = ''
-        count = 0
-        for char in string:
-            if char == '(':
-                if count == 0:
-                    key = re.sub(r'^\.', '', value)
-                    value = ''
-                else:
-                    value += char
-                count += 1
-            elif char == ')':
-                count -= 1
-                if count == 0:
-                    key, current_dict, value = self._get_context(
-                        key, current_dict, value
-                    )
-                    value = ''
-                else:
-                    value += char
-            else:
-                value += char
-        if not key:
-            current_dict = self._parse_value(value)
-        return current_dict
-
-    def _validate_key(self, key):
-        if key != 'ETL':
-            if key.startswith('set'):
-                key = '_'.join(self._split_camel_case(key[3:]).split())
-            return key
-        return None
-
-    def __get_objects_by_pattern(self, value):
-        try:
-            platform_pattern = re.compile(
-                r"PlatformFactory\(['\"]([^'\"]+)['\"]\).create\(name=['\"]([^'\"]+)['\"]\,configs=(\[(.*?)\])"
-            )
-            [factory, name, config, *
-                args] = platform_pattern.search(value).groups()
-            return {
-                'factory': factory,
-                'name': name,
-                'config': ast.literal_eval(config)
-            }
-        except AttributeError:
-            platform_pattern = re.compile(
-                r"PlatformFactory\(['\"]([^'\"]+)['\"]\).create\(name=['\"]([^'\"]+)['\"]\)"
-            )
-            factory, name = platform_pattern.search(value).groups()
-            return {
-                'factory': factory,
-                'name': name,
-            }
-
-    def _process_platform_key(self, key, value):
-        if key == 'platform':
-            return self.__get_objects_by_pattern(value)
-        return None
-
-    def _process_etl_keys(self, key, current_dict, value):
-        if key == 'ETL':
-            if key not in current_dict:
-                current_dict[key] = []
-            current_dict[key].append(self.parse(value))
-        else:
-            current_dict[key] = self.parse(value)
-        return current_dict[key]
-
-    def _swap_key_value(self, key, value):
-        if not value:
-            value = 'factory'
-        if value == 'factory':
-            key, value = value, key
-        elif key in ['extract', 'load', 'transform', 'validate']:
-            if key == 'transform':
-                value = f'.setType({key}).setName({value})'
-            else:
-                value = f'.setType({key})' + value
-            key = 'ETL'
-        return key, value
-
-    def _get_context(self, key, current_dict, value):
-        key = self._validate_key(key)
-        processed_value = self._process_platform_key(key, value)
-        if processed_value:
-            current_dict[key] = processed_value
-        elif key:
-            key, value = self._swap_key_value(key, value)
-            current_dict[key] = self._process_etl_keys(
-                key, current_dict, value
-            )
-        return key, current_dict, value
-
-    def _split_camel_case(self, name):
-        return (
-            re.sub('([A-Z][a-z]+)', r' \1', re.sub('([A-Z]+)', r' \1', name))
-            .lower()
-            .strip()
-        )
-
-    def _parse_value(self, value):
-        try:
-            return ast.literal_eval(value)
-        except (ValueError, SyntaxError):
-            return value
+import ast
+import re
+
+
+class ParseETL:
+    def parse(self, string):
+        current_dict = {}
+        key = ''
+        value = ''
+        count = 0
+        for char in string:
+            if char == '(':
+                if count == 0:
+                    key = re.sub(r'^\.', '', value)
+                    value = ''
+                else:
+                    value += char
+                count += 1
+            elif char == ')':
+                count -= 1
+                if count == 0:
+                    key, current_dict, value = self._get_context(
+                        key, current_dict, value
+                    )
+                    value = ''
+                else:
+                    value += char
+            else:
+                value += char
+        if not key:
+            current_dict = self._parse_value(value)
+        return current_dict
+
+    def _validate_key(self, key):
+        if key != 'ETL':
+            if key.startswith('set'):
+                key = '_'.join(self._split_camel_case(key[3:]).split())
+            return key
+        return None
+
+    def __get_objects_by_pattern(self, value):
+        try:
+            platform_pattern = re.compile(
+                r"PlatformFactory\(['\"]([^'\"]+)['\"]\).create\(name=['\"]([^'\"]+)['\"]\,configs=(\[(.*?)\])"
+            )
+            [factory, name, config, *
+                args] = platform_pattern.search(value).groups()
+            return {
+                'factory': factory,
+                'name': name,
+                'config': ast.literal_eval(config)
+            }
+        except AttributeError:
+            platform_pattern = re.compile(
+                r"PlatformFactory\(['\"]([^'\"]+)['\"]\).create\(name=['\"]([^'\"]+)['\"]\)"
+            )
+            factory, name = platform_pattern.search(value).groups()
+            return {
+                'factory': factory,
+                'name': name,
+            }
+
+    def _process_platform_key(self, key, value):
+        if key == 'platform':
+            return self.__get_objects_by_pattern(value)
+        return None
+
+    def _process_etl_keys(self, key, current_dict, value):
+        if key == 'ETL':
+            if key not in current_dict:
+                current_dict[key] = []
+            current_dict[key].append(self.parse(value))
+        else:
+            current_dict[key] = self.parse(value)
+        return current_dict[key]
+
+    def _swap_key_value(self, key, value):
+        if not value:
+            value = 'factory'
+        if value == 'factory':
+            key, value = value, key
+        elif key in ['extract', 'load', 'transform', 'validate']:
+            if key == 'transform':
+                value = f'.setType({key}).setName({value})'
+            else:
+                value = f'.setType({key})' + value
+            key = 'ETL'
+        return key, value
+
+    def _get_context(self, key, current_dict, value):
+        key = self._validate_key(key)
+        processed_value = self._process_platform_key(key, value)
+        if processed_value:
+            current_dict[key] = processed_value
+        elif key:
+            key, value = self._swap_key_value(key, value)
+            current_dict[key] = self._process_etl_keys(
+                key, current_dict, value
+            )
+        return key, current_dict, value
+
+    def _split_camel_case(self, name):
+        return (
+            re.sub('([A-Z][a-z]+)', r' \1', re.sub('([A-Z]+)', r' \1', name))
+            .lower()
+            .strip()
+        )
+
+    def _parse_value(self, value):
+        try:
+            return ast.literal_eval(value)
+        except (ValueError, SyntaxError):
+            return value
```

### Comparing `sefazetllib-0.1.55/PKG-INFO` & `sefazetllib-0.1.56/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sefazetllib
-Version: 0.1.55
+Version: 0.1.56
 Summary: sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.
 Home-page: https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1
 License: Apache-2.0
 Author: Felipe Gochi
 Author-email: felipe.gochi@elogroup.com.br
 Maintainer: Bruno Santos
 Maintainer-email: bruno.santos@elogroup.com.br
@@ -14,22 +14,26 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: boto3 (>=1.24,<2.0)
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: pandas (>=1.3,<2.0)
 Requires-Dist: pyarrow (>=6.0,<7.0)
-Requires-Dist: pydeequ (>=1.0,<2.0)
+Requires-Dist: pydeequ (==1.2.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Documentation, https://main.unavailable.amplifyapp.com/
 Project-URL: Repository, https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1
 Description-Content-Type: text/markdown
 
 # sefazetllib
```

