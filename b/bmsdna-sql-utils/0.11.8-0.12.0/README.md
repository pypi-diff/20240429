# Comparing `tmp/bmsdna_sql_utils-0.11.8.tar.gz` & `tmp/bmsdna_sql_utils-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_sql_utils-0.11.8.tar", max compression
+gzip compressed data, was "bmsdna_sql_utils-0.12.0.tar", max compression
```

## Comparing `bmsdna_sql_utils-0.11.8.tar` & `bmsdna_sql_utils-0.12.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      255 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/README.md
--rw-r--r--   0        0        0        0 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/__init__.py
--rw-r--r--   0        0        0      382 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/__init__.py
--rw-r--r--   0        0        0     3133 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/async_db_helper.py
--rw-r--r--   0        0        0     1169 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/case_preserving_set.py
--rw-r--r--   0        0        0     3529 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_helper.py
--rw-r--r--   0        0        0        0 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/__init__.py
--rw-r--r--   0        0        0     1991 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/db_logging.py
--rw-r--r--   0        0        0     5290 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/delta_polars_source.py
--rw-r--r--   0        0        0     5941 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/delta_source.py
--rw-r--r--   0        0        0    25944 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/fill_table.py
--rw-r--r--   0        0        0     2123 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/json_insert.py
--rw-r--r--   0        0        0     5060 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/lake_source.py
--rw-r--r--   0        0        0     1754 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/meta_sql_store.py
--rw-r--r--   0        0        0     1476 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/odbc_insert.py
--rw-r--r--   0        0        0     1725 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/source.py
--rw-r--r--   0        0        0      739 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/sql_utils.py
--rw-r--r--   0        0        0    14527 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/sqlschema.py
--rw-r--r--   0        0        0     1258 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/dbapi.py
--rw-r--r--   0        0        0     1332 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/integrity_check.py
--rw-r--r--   0        0        0      189 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/lake/__init__.py
--rw-r--r--   0        0        0     2423 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/lake/lake_meta.py
--rw-r--r--   0        0        0     1058 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/lake/type_fromarrow.py
--rw-r--r--   0        0        0      719 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/lake/types.py
--rw-r--r--   0        0        0     5671 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/metadata/__init__.py
--rw-r--r--   0        0        0     4024 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/query.py
--rw-r--r--   0        0        0     2759 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/query_generation.py
--rw-r--r--   0        0        0     2619 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/result.py
--rw-r--r--   0        0        0     4026 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/server_info.py
--rw-r--r--   0        0        0     1078 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/sql_gen.py
--rw-r--r--   0        0        0     1625 2024-04-29 09:31:28.537246 bmsdna_sql_utils-0.11.8/pyproject.toml
--rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 bmsdna_sql_utils-0.11.8/PKG-INFO
+-rw-r--r--   0        0        0      255 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/__init__.py
+-rw-r--r--   0        0        0     3133 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/async_db_helper.py
+-rw-r--r--   0        0        0     1169 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/case_preserving_set.py
+-rw-r--r--   0        0        0     3529 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_helper.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/__init__.py
+-rw-r--r--   0        0        0     2113 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/db_logging.py
+-rw-r--r--   0        0        0     5382 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/delta_polars_source.py
+-rw-r--r--   0        0        0     6060 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/delta_source.py
+-rw-r--r--   0        0        0    26081 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/fill_table.py
+-rw-r--r--   0        0        0     2116 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/json_insert.py
+-rw-r--r--   0        0        0     5178 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/lake_source.py
+-rw-r--r--   0        0        0     1754 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/meta_sql_store.py
+-rw-r--r--   0        0        0     1481 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/odbc_insert.py
+-rw-r--r--   0        0        0     1736 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/source.py
+-rw-r--r--   0        0        0      739 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/sql_utils.py
+-rw-r--r--   0        0        0    15908 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/sqlschema.py
+-rw-r--r--   0        0        0     1258 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/dbapi.py
+-rw-r--r--   0        0        0     1332 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/integrity_check.py
+-rw-r--r--   0        0        0      199 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/lake/__init__.py
+-rw-r--r--   0        0        0     2423 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/lake/lake_meta.py
+-rw-r--r--   0        0        0      822 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/lake/type_fromarrow.py
+-rw-r--r--   0        0        0      884 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/lake/types.py
+-rw-r--r--   0        0        0     5671 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/metadata/__init__.py
+-rw-r--r--   0        0        0     4024 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/query.py
+-rw-r--r--   0        0        0     2759 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/query_generation.py
+-rw-r--r--   0        0        0     2619 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/result.py
+-rw-r--r--   0        0        0     4026 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/server_info.py
+-rw-r--r--   0        0        0     1078 2024-04-29 13:57:26.016626 bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/sql_gen.py
+-rw-r--r--   0        0        0     1754 2024-04-29 13:57:26.020626 bmsdna_sql_utils-0.12.0/pyproject.toml
+-rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 bmsdna_sql_utils-0.12.0/PKG-INFO
```

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/async_db_helper.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/async_db_helper.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/case_preserving_set.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/case_preserving_set.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_helper.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_helper.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/delta_polars_source.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/delta_polars_source.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from datetime import datetime, timezone
 
 from deltalake2db import polars_scan_delta
 from .source import ImportSource, WriteInfo
 import urllib.parse
 from bmsdna.sql_utils.query import build_connection_string
 import logging
-from bmsdna.sql_utils.lake.types import FieldWithType
+from bmsdna.sql_utils.lake.types import FieldWithType, SQLField
 from bmsdna.sql_utils.lake.type_fromarrow import recursive_get_type
 from bmsdna.sql_utils.query import sql_quote_name
+from .sqlschema import with_max_str_length
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     import deltalake
 logger = logging.getLogger(__name__)
 
 
@@ -22,15 +23,15 @@
         super().__init__()
         import deltalake
 
         if isinstance(path_or_table, str):
             self.delta_lake = deltalake.DeltaTable(path_or_table, storage_options=storage_options)
         else:
             self.delta_lake = path_or_table
-        self._schema: list[FieldWithType] | None = None
+        self._schema: list[SQLField] | None = None
         self.use_json_insert = use_json_insert
         self.batch_size = 1048576 if not use_json_insert else 1000
 
     async def write_to_sql_server(
         self,
         target_table: str | tuple[str, str],
         connection_string: str | dict,
@@ -55,19 +56,19 @@
         connection_string_sql = build_connection_string(connection_string, odbc=False)
         if self.use_json_insert:
             from .json_insert import insert_into_table_via_json_from_batches
             import pyodbc
 
             with pyodbc.connect(build_connection_string(connection_string, odbc=True)) as con:
                 schema = self.get_schema()
-                filtered_schema = schema if not select else [f for f in schema if f["name"] in select]
+                filtered_schema = schema if not select else [f for f in schema if f.column_name in select]
                 await insert_into_table_via_json_from_batches(
                     reader=record_batch_reader, table_name=target_table, connection=con, schema=filtered_schema
                 )
-                col_names = [f["name"] for f in filtered_schema]
+                col_names = [f.column_name for f in filtered_schema]
         else:
             res = await insert_record_batch_to_sql(connection_string_sql, table_str, record_batch_reader, select)
             col_names = [f["name"] for f in res["fields"]]
             # r.raise_for_status()
         return WriteInfo(column_names=col_names, table_name=target_table)
 
     def get_partition_values(self) -> list[dict]:
@@ -78,51 +79,51 @@
         if len(part_cols) == 0:
             return []
         sorted = (
             polars_scan_delta(self.delta_lake).select([pl.col(pc) for pc in part_cols]).unique().sort(part_cols[0])
         )
         return sorted.collect().to_dicts()
 
-    def get_schema(self) -> list[FieldWithType]:
+    def get_schema(self) -> list[SQLField]:
         import pyarrow as pa
 
         if self._schema is not None:
             return self._schema
         import polars as pl
 
         schema = self.delta_lake.schema().to_pyarrow()
         sql_lens = []
         length_fields: list[str] = []
-        fields: dict[str, FieldWithType] = dict()
+        fields: dict[str, SQLField] = dict()
         for fieldname in schema.names:
             if fieldname.startswith("__"):
                 continue
             f = schema.field(fieldname)
             t = f.type
             is_complex = (
                 pa.types.is_list(t)
                 or pa.types.is_large_list(t)
                 or pa.types.is_fixed_size_list(t)
                 and t.value_type is not None
             )
             is_string = pa.types.is_string(t) or pa.types.is_large_string(t)
-            fields[fieldname] = FieldWithType(name=fieldname, type=recursive_get_type(t, True), max_str_length=None)
+            fields[fieldname] = SQLField(column_name=fieldname, data_type=recursive_get_type(t, True))
             if is_complex:
                 length_fields.append(fieldname)
                 import json
 
                 sql_lens.append(pl.col(fieldname).apply(lambda x: len(json.dumps(x))).max().alias(fieldname))
             elif is_string:
                 length_fields.append(fieldname)
                 sql_lens.append(pl.col(fieldname).str.len_chars().max().alias(fieldname))
 
         if len(sql_lens) > 0:
             res = polars_scan_delta(self.delta_lake).select(*sql_lens).collect().to_dicts()
             for lf in length_fields:
-                fields[lf]["max_str_length"] = res[0][lf]
+                fields[lf] = SQLField(fields[lf].column_name, with_max_str_length(fields[lf].data_type, res[0][lf]))
 
         self._schema = list(fields.values())
         return self._schema
 
     def get_last_change_date(self):
         return datetime.fromtimestamp(
             self.delta_lake.history(1)[-1]["timestamp"] / 1000.0,
```

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/delta_source.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/delta_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from datetime import datetime, timezone
 
 from deltalake2db import get_sql_for_delta
 from .source import ImportSource, WriteInfo
 import urllib.parse
 from bmsdna.sql_utils.query import build_connection_string
 import logging
-from bmsdna.sql_utils.lake.types import FieldWithType
+from bmsdna.sql_utils.lake.types import SQLField
 from bmsdna.sql_utils.lake.type_fromarrow import recursive_get_type
 from bmsdna.sql_utils.query import sql_quote_name
 from typing import TYPE_CHECKING
+from .sqlschema import with_max_str_length
 
 if TYPE_CHECKING:
     import deltalake
 logger = logging.getLogger(__name__)
 
 
 class DeltaSource(ImportSource):
@@ -22,15 +23,15 @@
         super().__init__()
         import deltalake
 
         if isinstance(path_or_table, str):
             self.delta_lake = deltalake.DeltaTable(path_or_table, storage_options=storage_options)
         else:
             self.delta_lake = path_or_table
-        self._schema: list[FieldWithType] | None = None
+        self._schema: list[SQLField] | None = None
         self.use_json_insert = use_json_insert
         self.batch_size = 1048576 if not use_json_insert else 1000
 
     async def write_to_sql_server(
         self,
         target_table: str | tuple[str, str],
         connection_string: str | dict,
@@ -48,19 +49,19 @@
                 connection_string_sql = build_connection_string(connection_string, odbc=False)
                 if self.use_json_insert:
                     from .json_insert import insert_into_table_via_json_from_batches
                     import pyodbc
 
                     with pyodbc.connect(build_connection_string(connection_string, odbc=True)) as con:
                         schema = self.get_schema()
-                        filtered_schema = schema if not select else [f for f in schema if f["name"] in select]
+                        filtered_schema = schema if not select else [f for f in schema if f.column_name in select]
                         await insert_into_table_via_json_from_batches(
                             reader=record_batch_reader, table_name=target_table, connection=con, schema=filtered_schema
                         )
-                        col_names = [f["name"] for f in filtered_schema]
+                        col_names = [f.column_name for f in filtered_schema]
                 else:
                     res = await insert_record_batch_to_sql(
                         connection_string_sql, table_str, record_batch_reader, select
                     )
                     col_names = [f["name"] for f in res["fields"]]
                 # r.raise_for_status()
         else:
@@ -78,38 +79,38 @@
         if delta_sql is None:
             return []  # no files
         sql = delta_sql + " ORDER BY " + ",".join([sql_quote_name(pc) for pc in part_cols])
         with duckdb.connect() as con:
             ls = con.execute(sql).fetchall()
             return [{p: it[i] for i, p in enumerate(part_cols)} for it in ls]
 
-    def get_schema(self) -> list[FieldWithType]:
+    def get_schema(self) -> list[SQLField]:
         import pyarrow as pa
 
         if self._schema is not None:
             return self._schema
         import duckdb
 
         schema = self.delta_lake.schema().to_pyarrow()
         sql_lens = []
         length_fields: list[str] = []
-        fields: dict[str, FieldWithType] = dict()
+        fields: dict[str, SQLField] = dict()
         for fieldname in schema.names:
             if fieldname.startswith("__"):
                 continue
             f = schema.field(fieldname)
             t = f.type
             is_complex = (
                 pa.types.is_list(t)
                 or pa.types.is_large_list(t)
                 or pa.types.is_fixed_size_list(t)
                 and t.value_type is not None
             )
             is_string = pa.types.is_string(t) or pa.types.is_large_string(t)
-            fields[fieldname] = FieldWithType(name=fieldname, type=recursive_get_type(t, True), max_str_length=None)
+            fields[fieldname] = SQLField(fieldname, recursive_get_type(t, True))
             if is_complex:
                 length_fields.append(fieldname)
                 sql_lens.append(f"MAX(LEN(to_json({sql_quote_name(fieldname)}))) as {sql_quote_name(fieldname)}")
             elif is_string:
                 length_fields.append(fieldname)
                 sql_lens.append(f"MAX(LEN({sql_quote_name(fieldname)})) as {sql_quote_name(fieldname)}")
 
@@ -120,15 +121,17 @@
 
                 with duckdb.connect() as con:
                     with con.cursor() as cur:
                         cur.execute(sql)
                         res = cur.fetchone()
                         assert res is not None
                         for i, lf in enumerate(length_fields):
-                            fields[lf]["max_str_length"] = res[i]
+                            fields[lf] = SQLField(
+                                fields[lf].column_name, with_max_str_length(fields[lf].data_type, res[i])
+                            )
 
         self._schema = list(fields.values())
         return self._schema
 
     def get_last_change_date(self):
         return datetime.fromtimestamp(
             self.delta_lake.history(1)[-1]["timestamp"] / 1000.0,
```

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/fill_table.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/fill_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from dataclasses import dataclass
-from typing import Any, Callable, List, Literal, Optional, TypeVar, TYPE_CHECKING
+from typing import Any, Callable, List, Literal, Optional, TypeVar, TYPE_CHECKING, Mapping
 from typing_extensions import TypedDict, NotRequired
-from bmsdna.sql_utils.lake import (
-    FieldWithType,
-)
+from bmsdna.sql_utils.lake import FieldWithType, SQLField
 from bmsdna.sql_utils.server_info import DBInfo
 from .db_logging import init_logging, insert_into_log
 from .sqlschema import (
-    sql_quote_value_field,
     create_table,
     is_table_empty,
     get_max_update_col_value,
     CreateTableCallbackParams,
+    sql_quote_value_with_type,
+    get_str_length,
 )
 from bmsdna.sql_utils.query import sql_quote_name, build_connection_string, sql_quote_value
 from bmsdna.sql_utils.db_io.source import ImportSource
 import uuid
 import logging
 from datetime import datetime
 from bmsdna.sql_utils.db_io.meta_sql_store import set_extended_property, get_extended_property
@@ -59,22 +58,22 @@
 def _str_part_filter(partition_filter: Optional[dict]):
     return "&".join((k + "=" + str(v) for k, v in partition_filter.items())) if partition_filter else None
 
 
 async def _do_merge(
     source: ImportSource,
     target_table: tuple[str, str],
-    schema: list[FieldWithType],
+    schema: list[SQLField],
     conn: "pyodbc.Connection | pytds.Connection",
     partition_filter: Optional[dict],
     primary_keys: list[str],
     connection_string: str | dict,
     select: list[str] | None,
     temp_table_callback: list[Callable[[CreateTableCallbackParams], Any]] | None,
-    constant_values: dict[str, tuple[FieldWithType, Any]] | None,
+    constant_values: Mapping[str, tuple[SQLField, Any]] | None,
 ):
     temp_table_name = "##" + target_table[1] + "_" + str(uuid.uuid4()).replace("-", "")
     create_table(
         temp_table_name,
         schema,
         conn,
         primary_keys=[],
@@ -86,23 +85,23 @@
     await execute_merge(conn, target_table, write_info, partition_filter, primary_keys, incl_delete=True)
     return temp_table_name
 
 
 async def _do_merge_updatecol(
     source: ImportSource,
     target_table: tuple[str, str],
-    schema: list[FieldWithType],
+    schema: list[SQLField],
     conn: "pyodbc.Connection | pytds.Connection",
     partition_filter: Optional[dict],
     primary_keys: list[str],
     update_col: str,
     connection_string: str | dict,
     select: list[str] | None,
     table_per_partition: bool,
-    constant_values: dict[str, tuple[FieldWithType, Any]] | None,
+    constant_values: Mapping[str, tuple[SQLField, Any]] | None,
     temp_table_callback: list[Callable[[CreateTableCallbackParams], Any]] | None,
 ) -> list[str]:
     vl = get_max_update_col_value(conn, target_table, update_col, _get_filter_sql(partition_filter))
     if vl is None:
         return await _do_full_load(
             source=source,
             target_table=target_table,
@@ -119,15 +118,15 @@
             temp_mode="global_temp",
         )
     else:
         temp_table_name_pk = "##" + target_table[1] + "_" + str(uuid.uuid4()).replace("-", "") + "_pk"
         temp_table_name_updates = "##" + target_table[1] + "_" + str(uuid.uuid4()).replace("-", "") + "_updates"
         create_table(
             temp_table_name_pk,
-            [f for f in schema if f["name"] in primary_keys],
+            [f for f in schema if f.column_name in primary_keys],
             conn,
             [],
             True,
             callback=temp_table_callback,
             default_values=constant_values,
         )
         create_table(
@@ -142,15 +141,15 @@
         write_info_pk = await source.write_to_sql_server(
             temp_table_name_pk, connection_string, partition_filter or {}, primary_keys
         )
 
         write_info_updates = await source.write_to_sql_server(
             temp_table_name_updates, connection_string, (partition_filter or {}) | {update_col + "_gte": vl}, select
         )
-        exclude_cols = [f["name"] for f in schema if (f.get("max_str_length", 0) or 0) > 8000]
+        exclude_cols = [f.column_name for f in schema if (get_str_length(f.data_type) or 0) > 8000]
         await execute_merge(
             conn,
             target_table,
             write_info_updates,
             partition_filter,
             primary_keys,
             incl_delete=False,
@@ -178,25 +177,25 @@
     table_per_partition: bool = False
 
 
 async def _do_full_load(
     *,
     source: ImportSource,
     target_table: tuple[str, str],
-    schema: list[FieldWithType],
+    schema: list[SQLField],
     conn: "pyodbc.Connection | pytds.Connection",
     partition_filter: Optional[dict],
     connection_string: str | dict,
     is_empty: bool,
     table_per_partition: bool,
     select: list[str] | None,
     temp_mode: FULL_TEMP_MODES = "global_temp",
     after_swap: list[Callable[[AfterSwapParams], Any]] | None,
     temp_table_callback: list[Callable[[CreateTableCallbackParams], Any]] | None,
-    constant_values: dict[str, tuple[FieldWithType, Any]] | None,
+    constant_values: Mapping[str, tuple[SQLField, Any]] | None,
 ):
     if is_empty:  # insert directly
         await source.write_to_sql_server(target_table, connection_string, partition_filter, select)
         return []
     elif temp_mode == "table_swap":
         temp_table_name = (target_table[0], target_table[1] + "_staging4fl")
         create_table(
@@ -206,15 +205,15 @@
             primary_keys=[],
             overwrite=True,
             callback=temp_table_callback,
             default_values=constant_values,
         )
         select_4_insert = select
         if constant_values:
-            select_4_insert = select or [f["name"] for f in schema]
+            select_4_insert = select or [f.column_name for f in schema]
             select_4_insert = [s for s in select_4_insert if s not in constant_values.keys()]
         write_info = await source.write_to_sql_server(
             temp_table_name, connection_string, partition_filter, select_4_insert
         )
         with conn.cursor() as cur:
             cur.execute(
                 f"DROP TABLE IF EXISTS {sql_quote_name(target_table)}; exec sp_rename '{sql_quote_name(temp_table_name)}', '{target_table[1]}'"
@@ -232,48 +231,50 @@
             primary_keys=[],
             overwrite=True,
             callback=temp_table_callback,
             default_values=constant_values,
         )
         select_4_insert = select
         if constant_values:
-            select_4_insert = select or [f["name"] for f in schema]
+            select_4_insert = select or [f.column_name for f in schema]
             select_4_insert = [s for s in select_4_insert if s not in constant_values.keys()]
         write_info = await source.write_to_sql_server(
             temp_table_name, connection_string, partition_filter, select_4_insert
         )
         execute_full_load(conn, target_table, write_info, partition_filter)
     return [temp_table_name]
 
 
 async def insert_into_table_partition(
     *,
     source: ImportSource,
     target_table: tuple[str, str],
     connection: str | dict,
     partition_filter: Optional[dict],
-    schema: list[FieldWithType],
+    schema: list[SQLField],
     primary_keys: list[str] | None,
     update_col: Optional[str],
     select: Optional[list[str]],
     skip_create_table=False,
-    constant_values: dict[str, tuple[FieldWithType, Any]] | None = None,
-    calculated_values: dict[str, str] | None = None,
+    constant_values: Mapping[str, tuple[SQLField, Any]] | None = None,
+    calculated_values: Mapping[str, str] | None = None,
     temp_full_mode: FULL_TEMP_MODES = "global_temp",
     after_swap: list[Callable[[AfterSwapParams], Any]] | None = None,
     table_callback: list[Callable[[CreateTableCallbackParams], Any]] | None,
     temp_table_callback: list[Callable[[CreateTableCallbackParams], Any]] | None,
     table_per_partition: bool,
 ):
     if select:
         partition_filter_keys = partition_filter.keys() if partition_filter and not table_per_partition else []
         schema = [
             f
             for f in schema
-            if f["name"] in select or f["name"] in (primary_keys or []) or f["name"] in partition_filter_keys
+            if f.column_name in select
+            or f.column_name in (primary_keys or [])
+            or f.column_name in partition_filter_keys
         ]
     partition_filter_str = _str_part_filter(partition_filter)
     temp_tables = []
     connstr_odbc = build_connection_string(connection, odbc=True)
     import pyodbc
 
     with pyodbc.connect(connstr_odbc) as conn:
@@ -428,15 +429,15 @@
                         """
     logger.info(f"Executing SQL: {sql}")
     insert_into_log(conn, sql_table_name, "start_merge", partition_filter=partition_filter_str, sql=sql)
     with conn.cursor() as cur:
         cur.execute(sql)
 
 
-def _part_tbl(part_values: dict):
+def _part_tbl(part_values: Mapping):
     if len(part_values) == 1:
         return "_" + str(list(part_values.values())[0])
     sorted_items = sorted(part_values.items(), key=lambda x: x[0])  # sort keys alphabetically
     return "_" + "_".join(str(v) for _, v in sorted_items)
 
 
 T = TypeVar("T")
@@ -444,19 +445,19 @@
 
 def _make_list(x: T | list[T] | None) -> list[T] | None:
     if x is None or isinstance(x, list):
         return x
     return [x]
 
 
-def _get_select(c: str, constant_values: dict, calculated_columns: dict):
+def _get_select(c: str, constant_values: Mapping, calculated_columns: Mapping):
     if c not in constant_values and c not in calculated_columns:
         return sql_quote_name(c)
     if c in constant_values.keys():
-        return f"{sql_quote_value_field(*constant_values[c])} as {sql_quote_name(c)}"
+        return f"{sql_quote_value_with_type(*constant_values[c])} as {sql_quote_name(c)}"
     return calculated_columns[c] + " as  " + sql_quote_name(c)
 
 
 async def has_delta(
     source: ImportSource,
     connection: "str | dict | pyodbc.Connection | pytds.Connection",
     target_table: tuple[str, str],
@@ -494,15 +495,15 @@
     temp_full_mode: FULL_TEMP_MODES | None = None,
     table_callback: (
         list[Callable[[CreateTableCallbackParams], Any]] | Callable[[CreateTableCallbackParams], Any] | None
     ) = None,
     temp_table_callback: (
         list[Callable[[CreateTableCallbackParams], Any]] | Callable[[CreateTableCallbackParams], Any] | None
     ) = None,
-    calculated_columns: dict[str, Any] | None = None,
+    calculated_columns: Mapping[str, Any] | None = None,
     await_partitions=True,
     force=False,
 ):
     import pyodbc
 
     calculated_columns = calculated_columns or dict()
     part_values = source.get_partition_values()
@@ -517,15 +518,15 @@
                 if dt >= mod_date:
                     logger.info(f"Skipping table {target_table}, because it is already up to date")
                     return
     assert schema is not None
     if part_values is not None and len(part_values) > 0:
         table_sql: list[str] = []
         if table_per_partition:
-            all_cols = CasePreservingSet(select or [f["name"] for f in schema])
+            all_cols = CasePreservingSet(select or [f.column_name for f in schema])
             for k in calculated_columns.keys():
                 all_cols.add(k)
             for k in part_values[0].keys():
                 all_cols.add(k)
         else:
             all_cols = CasePreservingSet()
         first = True
@@ -538,19 +539,19 @@
                 sql = (
                     "SELECT "
                     + ", ".join(_get_select(c, constant_values, calculated_columns) for c in all_cols)
                     + " FROM "
                     + sql_quote_name(target_table_part)
                 )
                 select = select or [
-                    f["name"]
+                    f.column_name
                     for f in schema
-                    if not f["name"].startswith("__")
-                    and f["name"] not in constant_values.keys()
-                    and f["name"] not in calculated_columns.keys()
+                    if not f.column_name.startswith("__")
+                    and f.column_name not in constant_values.keys()
+                    and f.column_name not in calculated_columns.keys()
                 ]
                 table_sql.append(sql)
             prom = insert_into_table_partition(
                 target_table=target_table_part,
                 source=source,
                 connection=connection_string,
                 skip_create_table=not first and not table_per_partition,
@@ -593,15 +594,17 @@
             with pyodbc.connect(connstr_odbc) as conn:
                 conn.execute(view)
 
     else:
         constant_values = source.get_constant_values(None, select=select)
 
         select = select or [
-            f["name"] for f in schema if not f["name"].startswith("__") and f["name"] not in constant_values.keys()
+            f.column_name
+            for f in schema
+            if not f.column_name.startswith("__") and f.column_name not in constant_values.keys()
         ]
         await insert_into_table_partition(
             target_table=target_table,
             source=source,
             connection=connection_string,
             partition_filter=None,
             schema=schema,
```

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/json_insert.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/json_insert.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from bmsdna.sql_utils.db_io.sqlschema import get_field_col_definition
 from bmsdna.sql_utils.query import sql_quote_name
-from bmsdna.sql_utils.lake import FieldWithType
+from bmsdna.sql_utils.lake import SQLField
 from typing import TYPE_CHECKING, AsyncIterable
 import json
 
 if TYPE_CHECKING:
     import pyodbc
     import pytds
     import pyarrow as pa
 
 
 async def insert_into_table_via_json(
     *,
     json_batches: AsyncIterable[str],
     table_name: tuple[str, str] | str,
     connection: "pyodbc.Connection | pytds.Connection",
-    schema: list[FieldWithType],
+    schema: list[SQLField],
     colnames: list[str] | None = None,
 ):
-    colnames = colnames or [f["name"] for f in schema]
+    colnames = colnames or [f.column_name for f in schema]
     cols = ", ".join([sql_quote_name(c) for c in colnames])
     col_defs = ", ".join([get_field_col_definition(f) for f in schema])
     insert_to_tmp_tbl_stmt = (
         f"INSERT INTO {sql_quote_name(table_name)}({cols}) SELECT {cols} from openjson(?) with ({col_defs})"
     )
     async for batch_json in json_batches:
         with connection.cursor() as cursor:
@@ -44,15 +44,15 @@
 
 
 async def insert_into_table_via_json_from_batches(
     *,
     reader: "pa.RecordBatchReader",
     table_name: tuple[str, str] | str,
     connection: "pyodbc.Connection | pytds.Connection",
-    schema: list[FieldWithType],
+    schema: list[SQLField],
     colnames: list[str] | None = None,
 ):
-    colnames = colnames or reader.schema.names or [f["name"] for f in schema]
+    colnames = colnames or reader.schema.names or [f.column_name for f in schema]
     r = _batch_reader_to_json(reader)
     await insert_into_table_via_json(
         json_batches=r, schema=schema, table_name=table_name, colnames=colnames, connection=connection
     )
```

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/lake_source.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/lake_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from bmsdna.sql_utils.db_io.source import WriteInfo
 from bmsdna.sql_utils.lake.lake_meta import get_metadata
-from bmsdna.sql_utils.lake.types import FieldWithType, LakeMetadata
+from bmsdna.sql_utils.lake.types import FieldWithType, LakeMetadata, SQLField
 from .source import ImportSource
 import os
 import urllib.parse
 from bmsdna.sql_utils.query import build_connection_string
+from .sqlschema import convert_to_sql_field
 import logging
 from datetime import datetime
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     import aiohttp
 
@@ -50,17 +51,18 @@
             self._meta = jsd
         return self._meta
 
     def get_partition_values(self) -> list[dict]:
         jsd = self._get_meta()
         return jsd["partition_values"]
 
-    def get_schema(self) -> list[FieldWithType]:
+    def get_schema(self) -> list[SQLField]:
         jsd = self._get_meta()
-        return jsd.get("data_schema", jsd.get("schema", None))
+        fields = jsd.get("data_schema", jsd.get("schema", None))
+        return [convert_to_sql_field(f) for f in fields]
 
     def get_last_change_date(self):
         jsd = self._get_meta()
         return datetime.fromisoformat(jsd["modified_date"])
 
     async def write_to_sql_server(
         self,
@@ -92,25 +94,25 @@
         if self.use_json_insert:
             from .json_insert import insert_into_table_via_json
             import pyodbc
             import aiohttp
 
             with pyodbc.connect(build_connection_string(connection_string, odbc=True)) as con:
                 schema = self.get_schema()
-                filtered_schema = schema if not select else [f for f in schema if f["name"] in select]
+                filtered_schema = schema if not select else [f for f in schema if f.column_name in select]
                 async with aiohttp.ClientSession() as session:
                     async with session.get(
                         full_url, auth=aiohttp.BasicAuth(self.lake_api_auth[0], self.lake_api_auth[1])
                     ) as req:
                         req.raise_for_status()
                         r = _req_to_json_batches(req)
                         await insert_into_table_via_json(
                             json_batches=r, table_name=target_table, connection=con, schema=filtered_schema
                         )
-                        col_names = [f["name"] for f in filtered_schema]
+                        col_names = [f.column_name for f in filtered_schema]
             return WriteInfo(column_names=col_names, table_name=target_table)
         else:
             logger.info(f"Get Data from {full_url}")
             from lakeapi2sql.bulk_insert import insert_http_arrow_stream_to_sql
 
             table_str = target_table if isinstance(target_table, str) else target_table[0] + "." + target_table[1]
             connection_string_sql = build_connection_string(connection_string, odbc=False)
```

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/meta_sql_store.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/meta_sql_store.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/odbc_insert.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/odbc_insert.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import pyodbc
 import pyarrow as pa
 from typing import Union, Tuple
 
-from bmsdna.sql_utils.lake.types import FieldWithType
+from bmsdna.sql_utils.lake.types import FieldWithType, SQLField
 from ..query import sql_quote_name
 
 MINIMAL_JSON_COMPATIBILITY_LEVEL = 130
 
 
 async def pyodbc_insert_into_table(
     *,
     reader: pa.RecordBatchReader,
     table_name: Union[Tuple[str, str], str],
     connection: pyodbc.Connection,
-    schema: list[FieldWithType],
+    schema: list[SQLField],
     supports_json_insert: bool | None = None,
 ):
     if supports_json_insert is None:
         from ..metadata import get_compatibility_level
 
         supports_json_insert = get_compatibility_level(connection) >= MINIMAL_JSON_COMPATIBILITY_LEVEL
```

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/source.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/source.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import abstractmethod, ABC
 from dataclasses import dataclass
 from datetime import datetime
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Mapping
+import sqlglot.expressions as ex
 
 if TYPE_CHECKING:
-    from bmsdna.sql_utils.lake.types import FieldWithType
+    from bmsdna.sql_utils.lake.types import SQLField
 
 
 @dataclass(frozen=True)
 class WriteInfo:
     column_names: list[str]
     table_name: str | tuple[str, str]
 
@@ -17,41 +18,37 @@
     @abstractmethod
     async def write_to_sql_server(
         self,
         target_table: str | tuple[str, str],
         connection_string: str | dict,
         partition_filters: dict | None,
         select: list[str] | None = None,
-    ) -> WriteInfo:
-        ...
+    ) -> WriteInfo: ...
 
     @abstractmethod
-    def get_partition_values(self) -> list[dict] | None:
-        ...
+    def get_partition_values(self) -> list[dict] | None: ...
 
     @abstractmethod
-    def get_schema(self) -> "list[FieldWithType]":
-        ...
+    def get_schema(self) -> "list[SQLField]": ...
 
     @abstractmethod
-    def get_last_change_date(self) -> datetime | None:
-        ...
+    def get_last_change_date(self) -> datetime | None: ...
 
     def get_constant_values(
         self, partition_filter: dict | None, *, select: list[str] | None
-    ) -> "dict[str, tuple[FieldWithType, Any]]":
+    ) -> "Mapping[str, tuple[SQLField, Any]]":
         from bmsdna.sql_utils.lake.types import FieldWithType
 
         partition_filter = partition_filter or {}
         sc = self.get_schema()
-        res: dict[str, tuple[FieldWithType, Any]] = {}
+        res: dict[str, tuple[SQLField, Any]] = {}
         for fn in partition_filter.keys():
-            scf = next((f for f in sc if f["name"] == fn))
-            res[scf["name"]] = (scf, partition_filter[fn])
+            scf = next((f for f in sc if f.column_name == fn))
+            res[scf.column_name] = (scf, partition_filter[fn])
         for f in sc:
             if (
-                f["name"] not in partition_filter
-                and f.get("max_str_length", None) is None
-                and f["type"]["type_str"] == "string"
+                f.column_name not in partition_filter
+                and len(f.data_type.expressions) == 0
+                and f.data_type.Type in ex.DataType.TEXT_TYPES
             ):
-                res[f["name"]] = (f, None)
+                res[f.column_name] = (f, None)
         return res
```

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/sql_utils.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/sql_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/sqlschema.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/db_io/sqlschema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,57 @@
 from dataclasses import dataclass
-from typing import Callable, Literal, Union, Optional, Any, TYPE_CHECKING
+from typing import Callable, Literal, Union, Optional, Any, TYPE_CHECKING, Mapping
 import logging
-from bmsdna.sql_utils.lake import FieldWithType
+from bmsdna.sql_utils.lake import FieldWithType, SQLField
 from bmsdna.sql_utils.query import sql_quote_name, sql_quote_value
+import sqlglot.expressions as ex
 
 if TYPE_CHECKING:
     import pyodbc
     import pytds
 logger = logging.getLogger(__name__)
 
 table_name_type = Union[str, tuple[str, str]]
 
 
+def convert_to_sql_field(field: FieldWithType):
+
+    sqt = get_sql_type(field["type"]["type_str"], field.get("max_str_length", None))
+    return SQLField(field["name"], ex.DataType.build(sqt, dialect="tsql"))
+
+
+def with_max_str_length(t: ex.DataType, max_str_length: int) -> ex.DataType:
+    sql_str = t.sql("tsql")
+    if "(" in sql_str:
+        sql_str = sql_str[0 : sql_str.find("(")]
+    new_str = f"{sql_str}({max_str_length})" if max_str_length != -1 else sql_str + "(MAX)"
+    return ex.DataType.build(new_str, dialect="tsql")
+
+
+def get_str_length(field: SQLField | ex.DataType):
+    if isinstance(field, SQLField):
+        return get_str_length(field.data_type)
+    if len(field.expressions) != 1:
+        return None
+    t_zero = field.expressions[0]
+    if not isinstance(t_zero, int):
+        t_zero = t_zero.this
+    if not isinstance(t_zero, int):
+        t_zero = t_zero.this
+    assert isinstance(t_zero, int)
+    return t_zero
+
+
 def get_field_col_definition(
-    field: FieldWithType, nullable=True, default: str | None = None, formula: str | None = None
+    field: FieldWithType | SQLField, nullable=True, default: str | None = None, formula: str | None = None
 ) -> str:
+    if not isinstance(field, SQLField):
+        field = convert_to_sql_field(field)
     return get_col_definition(
-        field_name=field["name"],
-        type_str=field["type"]["type_str"],
-        max_str_length=field.get("max_str_length", None),
+        field=field,
         default=default,
         formula=formula,
     )
 
 
 def get_sql_type(type_str: str, max_str_length: Optional[int]):
     assert type_str not in ["List", "Struct"]
@@ -88,76 +117,73 @@
     elif type_str.startswith("timestamp[ms"):
         return "datetime"
     else:
         raise ValueError("Unkown type " + type_str)
 
 
 def get_col_definition(
-    field_name: str,
-    type_str: str,
-    max_str_length: Optional[int],
+    field: SQLField,
     nullable=True,
     default: str | None = None,
     formula: str | None = None,
 ) -> str:
     if formula is not None:
-        return sql_quote_name(field_name) + " AS " + formula
-    sql_type = get_sql_type(type_str, max_str_length)
-    definit = sql_quote_name(field_name) + " " + sql_type + (" NOT NULL" if not nullable else "")
+        return sql_quote_name(field.column_name) + " AS " + formula
+    sql_type = field.data_type.sql("tsql")
+    definit = sql_quote_name(field.column_name) + " " + sql_type + (" NOT NULL" if not nullable else "")
     if default is not None and default.lower() != "null":
         definit += " DEFAULT (" + default + ")"
     return definit
 
 
-def sql_quote_value_field(type: FieldWithType, value: Any):
-    return sql_quote_value_with_type(type["type"]["type_str"], type.get("max_str_length", None), value)
+def sql_quote_value_with_type(field: FieldWithType | SQLField, value: Any) -> str:
+    if not isinstance(field, SQLField):
+        field = convert_to_sql_field(field)
 
-
-def sql_quote_value_with_type(type_str: str, max_str_length: int | None, value: Any) -> str:
-    if value is not None and type_str.lower() in ["bit", "bool", "boolean"]:
+    if value is not None and field.data_type.type in [ex.DataType.Type.BOOLEAN, ex.DataType.Type.BIT]:
         assert type(value) == bool
         if value == True:
             return f"CAST(1 as bit)"
         else:
             return f"CAST(0 as bit)"
-    if value is not None and type_str.lower() in ["string", "int32", "varchar", "int"]:
+    if value is not None and str(field.data_type.type).lower() in ["string", "int32", "varchar", "int"]:
         return sql_quote_value(value)  # string / int32 are defaults for sql server
-    sql_type = get_sql_type(type_str, max_str_length)
+    sql_type = field.data_type.sql("tsql")
     if value is not None:
         return f"CAST({sql_quote_value(value)} as {sql_type})"
     else:
         return f"CAST(NULL AS {sql_type})"
 
 
 def get_sql_for_schema(
     table_name: table_name_type,
-    schema: list[FieldWithType],
+    schema: list[SQLField],
     primary_keys: list[str] | None,
     with_exist_check: bool,
-    default_values: dict[str, tuple[FieldWithType, Any]] | None = None,
-    calculated_values: dict[str, str] | None = None,
+    default_values: Mapping[str, tuple[FieldWithType | SQLField, Any]] | None = None,
+    calculated_values: Mapping[str, str] | None = None,
 ):
     cols_sql = [
         get_field_col_definition(
             f,
-            primary_keys is None or f["name"] not in primary_keys,
+            primary_keys is None or f.column_name not in primary_keys,
             default=(
-                sql_quote_value_field(*default_values[f["name"]])
-                if default_values and f["name"] in default_values
+                sql_quote_value_with_type(*default_values[f.column_name])
+                if default_values and f.column_name in default_values
                 else None
             ),
             formula=(
-                calculated_values[f["name"]]
-                if calculated_values is not None and f["name"] in calculated_values
+                calculated_values[f.column_name]
+                if calculated_values is not None and f.column_name in calculated_values
                 else None
             ),
         )
         for f in schema
     ]
-    l_col_names = [f["name"].lower() for f in schema]
+    l_col_names = [f.column_name.lower() for f in schema]
     if calculated_values is not None:
         for k, v in calculated_values.items():
             if k.lower() not in l_col_names:
                 cols_sql.append(sql_quote_name(k) + " AS " + v)
 
     cols = ", ".join(cols_sql)
     pkdef = ""
@@ -179,46 +205,54 @@
             begin
                 select 'nothing' as action
             end 
         """
     return create_sql
 
 
-def get_raw_type(type: str):
+def get_raw_type(type: str | ex.DataType | ex.DataType.Type) -> str:
+    if isinstance(type, ex.DataType.Type):
+        return str(type).lower()
+    if isinstance(type, ex.DataType):
+        return str(type.type).lower()
     if "(" in type:
         return type[: type.find("(")]
     return type
 
 
-def col_approx_eq(type1: str, type2: str):
+def col_approx_eq(type1: str, type2: str | ex.DataType | ex.DataType.Type):
     if type1 == type2:
         return True
+    if isinstance(type2, ex.DataType.Type):
+        type2 = str(type2).lower()
+    elif isinstance(type2, ex.DataType):
+        type2 = str(type2.type).lower()
     if type1 in ["varchar", "nvarchar"] and type2 in ["varchar", "nvarchar"]:
         return True
     return False
 
 
 @dataclass(frozen=True)
 class CreateTableCallbackParams:
     table_name: table_name_type
-    schema: list[FieldWithType]
+    schema: list[SQLField]
     conn: "pyodbc.Connection | pytds.Connection"
     primary_keys: list[str] | None
     action: Literal["create", "adjusted", "none"]
     truncated: bool
 
 
 def create_table(
     table_name: table_name_type,
-    schema: list[FieldWithType],
+    schema: list[SQLField],
     conn: "pyodbc.Connection | pytds.Connection",
     primary_keys: list[str] | None,
     overwrite: bool,
-    default_values: dict[str, tuple[FieldWithType, Any]] | None = None,
-    calculated_values: dict[str, str] | None = None,
+    default_values: Mapping[str, tuple[SQLField, Any]] | None = None,
+    calculated_values: Mapping[str, str] | None = None,
     callback: list[Callable[[CreateTableCallbackParams], Any]] | None = None,
 ):
     created = False
     truncated = False
     adjusted = False
     if overwrite:
         with conn.cursor() as cur:
@@ -243,58 +277,60 @@
                 cols.append(dict(zip(columns, row)))
         if len(cols) > 0:
             col_dict = {col["column_name"].lower(): col for col in cols}
             todos: list[str] = []
             truncate = False
             separate_cursors = False
             for scc in schema:
-                max_len = scc.get("max_str_length", None)
-                existing_col = col_dict.get(scc["name"].lower(), None)
+                max_len = get_str_length(scc.data_type)
+                existing_col = col_dict.get(scc.column_name.lower(), None)
                 if existing_col is None:
                     defini = get_field_col_definition(
                         scc,
-                        primary_keys is None or scc["name"] not in primary_keys,
+                        primary_keys is None or scc.column_name not in primary_keys,
                         default=(
-                            sql_quote_value_field(*default_values[scc["name"]])
-                            if default_values and scc["name"] in default_values
+                            sql_quote_value_with_type(*default_values[scc.column_name])
+                            if default_values and scc.column_name in default_values
                             else None
                         ),
-                        formula=calculated_values.get(scc["name"], None) if calculated_values is not None else None,
+                        formula=(
+                            calculated_values.get(scc.column_name, None) if calculated_values is not None else None
+                        ),
                     )
                     truncate = True
                     todos.append(f"ALTER TABLE {sql_quote_name(table_name)} ADD {defini}")
 
                 elif (
-                    not col_approx_eq(
-                        existing_col["data_type"], get_raw_type(get_sql_type(scc["type"]["type_str"], None))
-                    )
-                    and scc["name"] not in (calculated_values or dict())
-                    and scc["name"] not in (default_values or dict())
+                    not col_approx_eq(existing_col["data_type"], scc.data_type)
+                    and scc.column_name not in (calculated_values or dict())
+                    and scc.column_name not in (default_values or dict())
                 ):
                     truncate = True
                     separate_cursors = True
-                    todos.append(f"ALTER TABLE {sql_quote_name(table_name)} DROP COLUMN {sql_quote_name(scc['name'])}")
-                    defini = get_field_col_definition(scc, primary_keys is None or scc["name"] not in primary_keys)
+                    todos.append(
+                        f"ALTER TABLE {sql_quote_name(table_name)} DROP COLUMN {sql_quote_name(scc.column_name)}"
+                    )
+                    defini = get_field_col_definition(scc, primary_keys is None or scc.column_name not in primary_keys)
                     todos.append(f"ALTER TABLE {sql_quote_name(table_name)} ADD {defini}")
                 elif (
                     max_len is not None
                     and existing_col["max_len"]
                     and max_len > existing_col["max_len"]
                     and existing_col["max_len"] != -1
-                    and scc["name"] not in (calculated_values or dict())
-                    and scc["name"] not in (default_values or dict())
+                    and scc.column_name not in (calculated_values or dict())
+                    and scc.column_name not in (default_values or dict())
                 ):
                     max_len_str = str(max_len)
                     if (max_len > 4000 and existing_col["data_type"] == "nvarchar") or (
                         existing_col["data_type"] == "varchar" and max_len > 8000
                     ):
                         max_len_str = "MAX"
                     sql_t = existing_col["data_type"] + "(" + max_len_str + ")"
                     todos.append(
-                        f"ALTER TABLE {sql_quote_name(table_name)} ALTER COLUMN {sql_quote_name(scc['name'])} {sql_t}"
+                        f"ALTER TABLE {sql_quote_name(table_name)} ALTER COLUMN {sql_quote_name(scc.column_name)} {sql_t}"
                     )
             if truncate:
                 todos.insert(0, f"TRUNCATE TABLE {sql_quote_name(table_name)}")
                 truncated = True
             if len(todos) > 0:
                 adjusted = True
                 if separate_cursors:
```

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/dbapi.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/dbapi.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/integrity_check.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/integrity_check.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/lake/lake_meta.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/lake/lake_meta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/lake/types.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/lake/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 from typing_extensions import TypedDict, NotRequired
 from typing import List, Optional
+from dataclasses import dataclass
+import sqlglot.expressions as ex
 
 
 class FieldType(TypedDict):
     type_str: str
     fields: NotRequired[Optional[list["FieldWithType"]]]
     inner: NotRequired[Optional["FieldType"]]
 
 
+@dataclass(frozen=True)
+class SQLField:
+    column_name: str
+    data_type: ex.DataType
+
+
 class FieldWithType(TypedDict):
     name: str
     type: FieldType
     max_str_length: NotRequired[Optional[int]]
 
 
 class LakeMetadata(TypedDict):
```

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/metadata/__init__.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/query.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/query.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/query_generation.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/query_generation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/result.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/result.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/server_info.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/server_info.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/sql_gen.py` & `bmsdna_sql_utils-0.12.0/bmsdna/sql_utils/sql_gen.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.8/pyproject.toml` & `bmsdna_sql_utils-0.12.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-sql-utils"
-version = "0.11.8"
+version = "0.12.0"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 readme = "README.md"
 packages = [{ include = "bmsdna" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -28,20 +28,25 @@
 pyodbc = { version = ">=4.0.0" }
 aioodbc = { version = "^0.5.0" }
 python-tds = { version = "^1.13.0" }
 pydantic = ">=1.10.0"
 isort = "^5.12.0"
 pycln = "^2.4.0"
 sqlglot = ">=20.0.0"
-pytest = "^7.4.3"
 
 
 [tool.poetry.group.test.dependencies]
 pytest-asyncio = "^0.23.5"
+pytest = "^7.4.3"
 pytest-order = "^1.2.0"
+docker = "^7.0.0"
+pytest-cov = "^5.0.0"
+azure-identity = "^1.16.0"
+azure-storage-blob = "^12.19.1"
+python-dotenv = "^1.0.1"
 
 [tool.poetry.extras]
 db-io = ["pyodbc", "lakeapi2sql"]
 delta = ["duckdb", "deltalake"]
 db2delta = ["duckdb", "deltalake", "arrow-odbc"]
 polars = ["polars"]
```

### Comparing `bmsdna_sql_utils-0.11.8/PKG-INFO` & `bmsdna_sql_utils-0.12.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-sql-utils
-Version: 0.11.8
+Version: 0.12.0
 Summary: 
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

