# Comparing `tmp/bmsdna_sql_utils-0.11.7.tar.gz` & `tmp/bmsdna_sql_utils-0.11.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_sql_utils-0.11.7.tar", max compression
+gzip compressed data, was "bmsdna_sql_utils-0.11.8.tar", max compression
```

## Comparing `bmsdna_sql_utils-0.11.7.tar` & `bmsdna_sql_utils-0.11.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      110 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/README.md
--rw-r--r--   0        0        0        0 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/__init__.py
--rw-r--r--   0        0        0      382 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/__init__.py
--rw-r--r--   0        0        0     3133 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/async_db_helper.py
--rw-r--r--   0        0        0     1169 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/case_preserving_set.py
--rw-r--r--   0        0        0     3529 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_helper.py
--rw-r--r--   0        0        0        0 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/__init__.py
--rw-r--r--   0        0        0     1991 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/db_logging.py
--rw-r--r--   0        0        0     5290 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/delta_polars_source.py
--rw-r--r--   0        0        0     5941 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/delta_source.py
--rw-r--r--   0        0        0    25944 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/fill_table.py
--rw-r--r--   0        0        0     2123 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/json_insert.py
--rw-r--r--   0        0        0     5060 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/lake_source.py
--rw-r--r--   0        0        0     1754 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/meta_sql_store.py
--rw-r--r--   0        0        0     1476 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/odbc_insert.py
--rw-r--r--   0        0        0     1725 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/source.py
--rw-r--r--   0        0        0      739 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/sql_utils.py
--rw-r--r--   0        0        0    14561 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/sqlschema.py
--rw-r--r--   0        0        0     1258 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/dbapi.py
--rw-r--r--   0        0        0     1332 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/integrity_check.py
--rw-r--r--   0        0        0      189 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/lake/__init__.py
--rw-r--r--   0        0        0     2423 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/lake/lake_meta.py
--rw-r--r--   0        0        0     1058 2024-04-29 09:21:50.204178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/lake/type_fromarrow.py
--rw-r--r--   0        0        0      719 2024-04-29 09:21:50.208178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/lake/types.py
--rw-r--r--   0        0        0     5671 2024-04-29 09:21:50.208178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/metadata/__init__.py
--rw-r--r--   0        0        0     4024 2024-04-29 09:21:50.208178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/query.py
--rw-r--r--   0        0        0     2759 2024-04-29 09:21:50.208178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/query_generation.py
--rw-r--r--   0        0        0     2620 2024-04-29 09:21:50.208178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/result.py
--rw-r--r--   0        0        0     4026 2024-04-29 09:21:50.208178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/server_info.py
--rw-r--r--   0        0        0     1078 2024-04-29 09:21:50.208178 bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/sql_gen.py
--rw-r--r--   0        0        0     1621 2024-04-29 09:21:50.208178 bmsdna_sql_utils-0.11.7/pyproject.toml
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 bmsdna_sql_utils-0.11.7/PKG-INFO
+-rw-r--r--   0        0        0      255 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/__init__.py
+-rw-r--r--   0        0        0     3133 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/async_db_helper.py
+-rw-r--r--   0        0        0     1169 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/case_preserving_set.py
+-rw-r--r--   0        0        0     3529 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_helper.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/__init__.py
+-rw-r--r--   0        0        0     1991 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/db_logging.py
+-rw-r--r--   0        0        0     5290 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/delta_polars_source.py
+-rw-r--r--   0        0        0     5941 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/delta_source.py
+-rw-r--r--   0        0        0    25944 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/fill_table.py
+-rw-r--r--   0        0        0     2123 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/json_insert.py
+-rw-r--r--   0        0        0     5060 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/lake_source.py
+-rw-r--r--   0        0        0     1754 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/meta_sql_store.py
+-rw-r--r--   0        0        0     1476 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/odbc_insert.py
+-rw-r--r--   0        0        0     1725 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/source.py
+-rw-r--r--   0        0        0      739 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/sql_utils.py
+-rw-r--r--   0        0        0    14527 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/sqlschema.py
+-rw-r--r--   0        0        0     1258 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/dbapi.py
+-rw-r--r--   0        0        0     1332 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/integrity_check.py
+-rw-r--r--   0        0        0      189 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/lake/__init__.py
+-rw-r--r--   0        0        0     2423 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/lake/lake_meta.py
+-rw-r--r--   0        0        0     1058 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/lake/type_fromarrow.py
+-rw-r--r--   0        0        0      719 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/lake/types.py
+-rw-r--r--   0        0        0     5671 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/metadata/__init__.py
+-rw-r--r--   0        0        0     4024 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/query.py
+-rw-r--r--   0        0        0     2759 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/query_generation.py
+-rw-r--r--   0        0        0     2619 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/result.py
+-rw-r--r--   0        0        0     4026 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/server_info.py
+-rw-r--r--   0        0        0     1078 2024-04-29 09:31:28.533246 bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/sql_gen.py
+-rw-r--r--   0        0        0     1625 2024-04-29 09:31:28.537246 bmsdna_sql_utils-0.11.8/pyproject.toml
+-rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 bmsdna_sql_utils-0.11.8/PKG-INFO
```

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/async_db_helper.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/async_db_helper.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/case_preserving_set.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/case_preserving_set.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_helper.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_helper.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/db_logging.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/db_logging.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/delta_polars_source.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/delta_polars_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/delta_source.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/delta_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/fill_table.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/fill_table.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/json_insert.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/json_insert.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/lake_source.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/lake_source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/meta_sql_store.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/meta_sql_store.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/odbc_insert.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/odbc_insert.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/source.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/source.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/sql_utils.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/sql_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/db_io/sqlschema.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/db_io/sqlschema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from dataclasses import dataclass
 from typing import Callable, Literal, Union, Optional, Any, TYPE_CHECKING
 import logging
-
-from pydantic import BaseModel
 from bmsdna.sql_utils.lake import FieldWithType
 from bmsdna.sql_utils.query import sql_quote_name, sql_quote_value
 
 if TYPE_CHECKING:
     import pyodbc
     import pytds
 logger = logging.getLogger(__name__)
```

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/dbapi.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/dbapi.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/integrity_check.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/integrity_check.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/lake/lake_meta.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/lake/lake_meta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/lake/type_fromarrow.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/lake/type_fromarrow.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/lake/types.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/lake/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/metadata/__init__.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/query.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/query.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/query_generation.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/query_generation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/result.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,38 +5,35 @@
     import pydantic
 
 SomeDataClass = TypeVar("SomeDataClass")
 Row = Tuple
 
 
 @overload
-def make_class_from_cursor(classtype: type[dict], description: Sequence[Tuple], values: Sequence) -> list[dict]:
-    ...
+def make_class_from_cursor(classtype: type[dict], description: Sequence[Tuple], values: Sequence) -> list[dict]: ...
 
 
 @overload
-def make_class_from_cursor(classtype: type[dict], description: Sequence[Tuple], values: tuple) -> dict:
-    ...
+def make_class_from_cursor(classtype: type[dict], description: Sequence[Tuple], values: tuple) -> dict: ...
 
 
 @overload
-def make_class_from_cursor(classtype: type, description: Sequence[Tuple], values: None) -> None:
-    ...
+def make_class_from_cursor(classtype: type, description: Sequence[Tuple], values: None) -> None: ...
 
 
 @overload
 def make_class_from_cursor(
     classtype: type[SomeDataClass], description: Sequence[Tuple], values: Sequence[Row]
-) -> List[SomeDataClass]:
-    ...
+) -> List[SomeDataClass]: ...
 
 
 @overload
-def make_class_from_cursor(classtype: type[SomeDataClass], description: Sequence[Tuple], values: Row) -> SomeDataClass:
-    ...
+def make_class_from_cursor(
+    classtype: type[SomeDataClass], description: Sequence[Tuple], values: Row
+) -> SomeDataClass: ...
 
 
 def make_class_from_cursor(
     classtype: type[SomeDataClass],
     description: Sequence[Tuple],
     values: Union[Sequence[Row], Row, None],
 ) -> Union[SomeDataClass, List[SomeDataClass], None]:
@@ -60,15 +57,15 @@
     if type(values) == tuple or type(values).__name__ == "Row" or type(values).__name__ == "pyodbc.Row":
         if classtype == dict:
             names = [d[0] for d in description]
             return {name: get_vl(name, None) for name in names}  # type: ignore
         elif dataclasses.is_dataclass(classtype):
             prms = {f.name: get_vl(f.name, f.type) for f in dataclasses.fields(classtype)}  # type: ignore
             return classtype(**prms)
-        elif hasattr(classtype, "model_validate"):
+        elif hasattr(classtype, "model_validate"):  # Pydantic 2.0
             mod: "Type[pydantic.BaseModel]" = classtype  # type: ignore
             prms = {f: get_vl(f, None) for f in mod.model_fields.keys()}
             return mod.model_validate(prms)  # type: ignore
         else:
             import pydantic
 
             adapt = pydantic.TypeAdapter(classtype)
```

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/server_info.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/server_info.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/bmsdna/sql_utils/sql_gen.py` & `bmsdna_sql_utils-0.11.8/bmsdna/sql_utils/sql_gen.py`

 * *Files identical despite different names*

### Comparing `bmsdna_sql_utils-0.11.7/pyproject.toml` & `bmsdna_sql_utils-0.11.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "bmsdna-sql-utils"
-version = "0.11.7"
+version = "0.11.8"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 readme = "README.md"
 packages = [{ include = "bmsdna" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pyodbc = { version = "^5.0.1", optional = true }
 aioodbc = { version = "^0.5.0", optional = true }
 python-tds = { version = "^1.13.0", optional = true }
 pydantic = { version = "^2.3.0", optional = true }
 aiohttp = "^3.8.5"
-requests = "^2.31.0"
+requests = ">=2.28.0"
 duckdb = { version = "^0.10.1", optional = true }
 lakeapi2sql = { version = ">=0.7.4", optional = true }
 deltalake = { version = ">=0.16.4", optional = true }
 python-dateutil = { version = "^2.8.2", python = "<3.11" }
 arrow-odbc = { version = "^5.0.0", optional = true }
 deltalake2db = ">=0.3.0"
 polars = { version = ">=0.20.21", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.325"
 black = "^23.7.0"
-pyodbc = { version = "^5.0.1" }
+pyodbc = { version = ">=4.0.0" }
 aioodbc = { version = "^0.5.0" }
 python-tds = { version = "^1.13.0" }
-pydantic = "^2.3.0"
+pydantic = ">=1.10.0"
 isort = "^5.12.0"
 pycln = "^2.4.0"
 sqlglot = ">=20.0.0"
 pytest = "^7.4.3"
 
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `bmsdna_sql_utils-0.11.7/PKG-INFO` & `bmsdna_sql_utils-0.11.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-sql-utils
-Version: 0.11.7
+Version: 0.11.8
 Summary: 
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,15 +21,17 @@
 Requires-Dist: duckdb (>=0.10.1,<0.11.0) ; extra == "delta" or extra == "db2delta"
 Requires-Dist: lakeapi2sql (>=0.7.4) ; extra == "db-io"
 Requires-Dist: polars (>=0.20.21) ; extra == "polars"
 Requires-Dist: pydantic (>=2.3.0,<3.0.0)
 Requires-Dist: pyodbc (>=5.0.1,<6.0.0) ; extra == "db-io"
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) ; python_version < "3.11"
 Requires-Dist: python-tds (>=1.13.0,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.28.0)
 Description-Content-Type: text/markdown
 
 # Libary for minimal SQL Server Utils
 
 - Call a stored proc with results and store in a data class list
--
+- Load a Table from DeltaLake into SQL Server
+
+This package has very few docs. It's used internally and maybe documented better in a later stage
```

