# Comparing `tmp/reactpy_table-0.0.13.tar.gz` & `tmp/reactpy_table-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactpy_table-0.0.13.tar", max compression
+gzip compressed data, was "reactpy_table-0.0.14.tar", max compression
```

## Comparing `reactpy_table-0.0.13.tar` & `reactpy_table-0.0.14.tar`

### file list

```diff
@@ -1,29 +1,32 @@
--rw-r--r--   0        0        0     1469 2024-04-02 12:33:22.477220 reactpy_table-0.0.13/pyproject.toml
--rw-r--r--   0        0        0      287 2024-04-02 12:33:13.538920 reactpy_table-0.0.13/reactpy_table/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 09:34:43.413923 reactpy_table-0.0.13/reactpy_table/core/__init__.py
--rw-r--r--   0        0        0      434 2024-03-16 16:20:49.561713 reactpy_table-0.0.13/reactpy_table/core/feature_factories.py
--rw-r--r--   0        0        0     3276 2024-04-02 07:18:15.118079 reactpy_table-0.0.13/reactpy_table/core/options.py
--rw-r--r--   0        0        0     3294 2024-04-02 07:48:29.950742 reactpy_table-0.0.13/reactpy_table/core/reactpy_table.py
--rw-r--r--   0        0        0     1890 2024-04-02 10:29:24.687616 reactpy_table-0.0.13/reactpy_table/core/reactpy_table_init.py
--rw-r--r--   0        0        0      316 2024-04-02 07:14:51.990561 reactpy_table-0.0.13/reactpy_table/features/__init__.py
--rw-r--r--   0        0        0     3567 2024-04-02 07:21:37.484748 reactpy_table-0.0.13/reactpy_table/features/column_sort.py
--rw-r--r--   0        0        0      471 2024-04-01 11:39:24.234353 reactpy_table-0.0.13/reactpy_table/features/null_updater.py
--rw-r--r--   0        0        0     4594 2024-04-02 07:31:18.811981 reactpy_table-0.0.13/reactpy_table/features/paginator.py
--rw-r--r--   0        0        0     2649 2024-03-31 06:22:03.596864 reactpy_table-0.0.13/reactpy_table/features/row_model.py
--rw-r--r--   0        0        0     2304 2024-04-01 10:32:16.291727 reactpy_table-0.0.13/reactpy_table/features/table_search.py
--rw-r--r--   0        0        0      787 2024-04-02 10:29:16.464273 reactpy_table-0.0.13/reactpy_table/types/__init__.py
--rw-r--r--   0        0        0      405 2024-03-31 06:24:13.605740 reactpy_table-0.0.13/reactpy_table/types/abstract_column_sort.py
--rw-r--r--   0        0        0     1460 2024-03-27 08:30:11.088878 reactpy_table-0.0.13/reactpy_table/types/abstract_paginator.py
--rw-r--r--   0        0        0      405 2024-03-12 08:54:26.176120 reactpy_table-0.0.13/reactpy_table/types/abstract_row_model.py
--rw-r--r--   0        0        0     1179 2024-04-02 07:02:00.776177 reactpy_table-0.0.13/reactpy_table/types/abstract_table.py
--rw-r--r--   0        0        0      327 2024-04-01 16:08:43.301863 reactpy_table-0.0.13/reactpy_table/types/abstract_table_search.py
--rw-r--r--   0        0        0     1756 2024-04-02 10:20:19.175628 reactpy_table-0.0.13/reactpy_table/types/feature.py
--rw-r--r--   0        0        0      105 2024-04-01 09:21:02.103481 reactpy_table-0.0.13/reactpy_table/types/feature_control.py
--rw-r--r--   0        0        0      451 2024-04-02 10:39:06.135382 reactpy_table-0.0.13/reactpy_table/types/paginator_state.py
--rw-r--r--   0        0        0      303 2024-04-01 16:08:43.302835 reactpy_table-0.0.13/reactpy_table/types/search_state.py
--rw-r--r--   0        0        0      356 2024-03-31 06:24:13.608661 reactpy_table-0.0.13/reactpy_table/types/sort_state.py
--rw-r--r--   0        0        0      806 2024-04-02 10:25:58.585141 reactpy_table-0.0.13/reactpy_table/types/table.py
--rw-r--r--   0        0        0     1164 2024-04-02 10:24:22.290194 reactpy_table-0.0.13/reactpy_table/types/table_data.py
--rw-r--r--   0        0        0     2058 2024-04-02 06:59:10.101228 reactpy_table-0.0.13/reactpy_table/types/table_state.py
--rw-r--r--   0        0        0     3782 2024-04-02 12:14:38.146196 reactpy_table-0.0.13/README.md
--rw-r--r--   0        0        0     4417 1970-01-01 00:00:00.000000 reactpy_table-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-01-11 14:40:34.000000 reactpy_table-0.0.14/LICENSE
+-rw-r--r--   0        0        0     3844 2024-04-21 16:50:22.000000 reactpy_table-0.0.14/README.md
+-rw-r--r--   0        0        0     1469 2024-04-29 06:11:13.121856 reactpy_table-0.0.14/pyproject.toml
+-rw-r--r--   0        0        0      287 2024-04-29 06:11:23.692277 reactpy_table-0.0.14/reactpy_table/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 09:34:43.000000 reactpy_table-0.0.14/reactpy_table/core/__init__.py
+-rw-r--r--   0        0        0      434 2024-03-16 16:20:49.000000 reactpy_table-0.0.14/reactpy_table/core/feature_factories.py
+-rw-r--r--   0        0        0     3276 2024-04-02 12:44:44.000000 reactpy_table-0.0.14/reactpy_table/core/options.py
+-rw-r--r--   0        0        0     3294 2024-04-02 12:44:44.000000 reactpy_table-0.0.14/reactpy_table/core/reactpy_table.py
+-rw-r--r--   0        0        0     1890 2024-04-02 12:44:44.000000 reactpy_table-0.0.14/reactpy_table/core/reactpy_table_init.py
+-rw-r--r--   0        0        0      316 2024-04-02 07:14:51.000000 reactpy_table-0.0.14/reactpy_table/features/__init__.py
+-rw-r--r--   0        0        0     3581 2024-04-29 06:06:14.049435 reactpy_table-0.0.14/reactpy_table/features/column_sort.py
+-rw-r--r--   0        0        0      485 2024-04-29 06:06:14.049435 reactpy_table-0.0.14/reactpy_table/features/null_updater.py
+-rw-r--r--   0        0        0     4608 2024-04-29 06:06:14.049435 reactpy_table-0.0.14/reactpy_table/features/paginator.py
+-rw-r--r--   0        0        0     2663 2024-04-29 06:06:14.049435 reactpy_table-0.0.14/reactpy_table/features/row_model.py
+-rw-r--r--   0        0        0     2318 2024-04-29 06:06:14.049435 reactpy_table-0.0.14/reactpy_table/features/table_search.py
+-rw-r--r--   0        0        0      787 2024-04-02 12:44:44.000000 reactpy_table-0.0.14/reactpy_table/types/__init__.py
+-rw-r--r--   0        0        0      405 2024-04-02 12:44:44.000000 reactpy_table-0.0.14/reactpy_table/types/abstract_column_sort.py
+-rw-r--r--   0        0        0     1460 2024-04-02 12:44:44.000000 reactpy_table-0.0.14/reactpy_table/types/abstract_paginator.py
+-rw-r--r--   0        0        0      405 2024-03-12 08:54:26.000000 reactpy_table-0.0.14/reactpy_table/types/abstract_row_model.py
+-rw-r--r--   0        0        0     1193 2024-04-29 06:06:14.049435 reactpy_table-0.0.14/reactpy_table/types/abstract_table.py
+-rw-r--r--   0        0        0      327 2024-04-01 16:08:43.000000 reactpy_table-0.0.14/reactpy_table/types/abstract_table_search.py
+-rw-r--r--   0        0        0     1756 2024-04-02 12:44:44.000000 reactpy_table-0.0.14/reactpy_table/types/feature.py
+-rw-r--r--   0        0        0      105 2024-04-02 12:44:44.000000 reactpy_table-0.0.14/reactpy_table/types/feature_control.py
+-rw-r--r--   0        0        0      451 2024-04-02 12:44:44.000000 reactpy_table-0.0.14/reactpy_table/types/paginator_state.py
+-rw-r--r--   0        0        0      303 2024-04-02 12:44:44.000000 reactpy_table-0.0.14/reactpy_table/types/search_state.py
+-rw-r--r--   0        0        0      356 2024-04-02 12:44:44.000000 reactpy_table-0.0.14/reactpy_table/types/sort_state.py
+-rw-r--r--   0        0        0      806 2024-04-02 12:44:44.000000 reactpy_table-0.0.14/reactpy_table/types/table.py
+-rw-r--r--   0        0        0     1164 2024-04-02 12:44:44.000000 reactpy_table-0.0.14/reactpy_table/types/table_data.py
+-rw-r--r--   0        0        0     2058 2024-04-02 12:44:44.000000 reactpy_table-0.0.14/reactpy_table/types/table_state.py
+-rw-r--r--   0        0        0        0 2024-04-29 06:02:41.781703 reactpy_table-0.0.14/reactpy_table/utils/__init__.py
+-rw-r--r--   0        0        0     1986 2024-04-02 12:44:44.000000 reactpy_table-0.0.14/reactpy_table/utils/memo.py
+-rw-r--r--   0        0        0     4479 1970-01-01 00:00:00.000000 reactpy_table-0.0.14/PKG-INFO
```

### Comparing `reactpy_table-0.0.13/pyproject.toml` & `reactpy_table-0.0.14/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reactpy-table"
-version = "0.0.13"
+version = "0.0.14"
 description = "Headless UI for building powerful tables"
 authors = ["Steve Jones <jonesst2608@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/stevej2608/reactpy-table/blob/master/README.md"
 repository = "https://github.com/stevej2608/reactpy-table"
 include = ["reactpy-tablet/*.py"]
```

### Comparing `reactpy_table-0.0.13/reactpy_table/core/options.py` & `reactpy_table-0.0.14/reactpy_table/core/options.py`

 * *Files identical despite different names*

### Comparing `reactpy_table-0.0.13/reactpy_table/core/reactpy_table.py` & `reactpy_table-0.0.14/reactpy_table/core/reactpy_table.py`

 * *Files identical despite different names*

### Comparing `reactpy_table-0.0.13/reactpy_table/core/reactpy_table_init.py` & `reactpy_table-0.0.14/reactpy_table/core/reactpy_table_init.py`

 * *Files identical despite different names*

### Comparing `reactpy_table-0.0.13/reactpy_table/features/column_sort.py` & `reactpy_table-0.0.14/reactpy_table/features/column_sort.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict, Tuple
 
 from pydantic import BaseModel
 
-from utils.memo import MemoOpts, memo
+from reactpy_table.utils.memo import MemoOpts, memo
 
 from ..types import (
     ColumnDef,
     ColumnSort,
     FeatureControl,
     ITable,
     SortState,
```

### Comparing `reactpy_table-0.0.13/reactpy_table/features/paginator.py` & `reactpy_table-0.0.14/reactpy_table/features/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import math
 from ctypes import ArgumentError
 from typing import Tuple
 
 
-from utils.memo import MemoOpts, memo
+from reactpy_table.utils.memo import MemoOpts, memo
 
 from ..types import FeatureControl, ITable, Paginator, PaginatorState, TableData, TData, TFeatureFactory, UpstreamData
 from .null_updater import null_updater
 
 log = logging.getLogger(__name__)
 
 DEFAULT_PAGE_SIZE = 10
```

### Comparing `reactpy_table-0.0.13/reactpy_table/features/row_model.py` & `reactpy_table-0.0.14/reactpy_table/features/row_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Tuple, Any, List
 from enum import Enum
 from ctypes import ArgumentError
 from pydantic import BaseModel
-from utils.memo import memo, MemoOpts
+from reactpy_table.utils.memo import memo, MemoOpts
 from ..types import ITable, RowModel, TData, TableData, TFeatureFactory, UpstreamData, update_state
 
 class Action(Enum):
     DELETE = 1
     UPDATE = 2
 
 class RowAction(BaseModel):
```

### Comparing `reactpy_table-0.0.13/reactpy_table/features/table_search.py` & `reactpy_table-0.0.14/reactpy_table/features/table_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Tuple
 
-from utils.memo import MemoOpts, memo
+from reactpy_table.utils.memo import MemoOpts, memo
 
 from ..types import ITable, TableData, TableSearch, SearchState, TData, TFeatureFactory, UpstreamData
 
 
 class DefaultTableSearch(TableSearch[TData]):
 
     def __init__(self, table: ITable[TData], upstream_data: UpstreamData[TData]):
```

### Comparing `reactpy_table-0.0.13/reactpy_table/types/__init__.py` & `reactpy_table-0.0.14/reactpy_table/types/__init__.py`

 * *Files identical despite different names*

### Comparing `reactpy_table-0.0.13/reactpy_table/types/abstract_paginator.py` & `reactpy_table-0.0.14/reactpy_table/types/abstract_paginator.py`

 * *Files identical despite different names*

### Comparing `reactpy_table-0.0.13/reactpy_table/types/abstract_table.py` & `reactpy_table-0.0.14/reactpy_table/types/abstract_table.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Generic, Protocol, Callable, Self
-from utils.memo import TMemoResult
+from reactpy_table.utils.memo import TMemoResult
 from .table_data import TableData, TData
 from .table_state import TableState
 
 
 class ITable(Generic[TData], Protocol):
 
     @property
```

### Comparing `reactpy_table-0.0.13/reactpy_table/types/feature.py` & `reactpy_table-0.0.14/reactpy_table/types/feature.py`

 * *Files identical despite different names*

### Comparing `reactpy_table-0.0.13/reactpy_table/types/table.py` & `reactpy_table-0.0.14/reactpy_table/types/table.py`

 * *Files identical despite different names*

### Comparing `reactpy_table-0.0.13/reactpy_table/types/table_data.py` & `reactpy_table-0.0.14/reactpy_table/types/table_data.py`

 * *Files identical despite different names*

### Comparing `reactpy_table-0.0.13/reactpy_table/types/table_state.py` & `reactpy_table-0.0.14/reactpy_table/types/table_state.py`

 * *Files identical despite different names*

### Comparing `reactpy_table-0.0.13/README.md` & `reactpy_table-0.0.14/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 takes its design ideas from the hugely popular, ReactJS based, [TanStack Table].
 
 The initial release supports the following features:
 
 - [X] Headless UI, CSS agnostic
 - [X] Freeform text search
 - [X] Forward/Reverse column based sort
-- [X] Pagination
-- [X] Integration with SQLAlchemy (full text search, sort and pagination)
-- [ ] Integration with Pandas and SQLAlchemy (in progress)
-- [ ] Remote large dataset support
+- [X] Pagination (offset, limit)
+- [X] Integration with SQLModel/SQLAlchemy (fts5 based full text search, sort and pagination)
+- [ ] Integration with Pandas (in progress)
+- [ ] Remote large dataset support (in progress)
 
 ## Usage
 
 	pip install reactpy-table
 
 *[basic_example.py](examples/basic_example.py)*
 ```python
@@ -76,16 +76,16 @@
 **examples/table_example.py** demonstrates search, sort and pagination on SP500 
 companies table. The built-in feature data pipeline is used.
 
 **examples/books/books_example.py** demonstrates search, sort and pagination on
 a SQLite book database containing 100k books. Search, sort and 
 pagination is handled by SQL queries.
 
-* Full text search on database < 20ms
-* Page traversal < 2ms
+* FTS5 full text search on database < 20ms
+* Next/Prev page traversal < 2ms
 
 
 ## Feature Set
 
 The row data presented to the user for display is pre-processed by a
 data-pipeline of table features:
 
@@ -111,16 +111,16 @@
 All features are instantiated using a strict pattern. As
 an example a custom paginator that accepts *page _size* and
 *start_page* would be created as follows:
 
 ```
 def getCustomPaginator(page_size, start_page) 
 
-    def _feature_factory(table, updater):
-        return CustomPaginator(table, updater, page_size, start_page)
+    def _feature_factory(table, upstream_data):
+        return CustomPaginator(table, upstream_data, page_size, start_page)
     
     return _feature_factory
 
 ```
 The custom feature is passed as an option when the table is created:
 ```
 table = use_reactpy_table(Options(
```

### Comparing `reactpy_table-0.0.13/PKG-INFO` & `reactpy_table-0.0.14/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy-table
-Version: 0.0.13
+Version: 0.0.14
 Summary: Headless UI for building powerful tables
 Home-page: https://github.com/stevej2608/reactpy-table/blob/master/README.md
 License: MIT
 Author: Steve Jones
 Author-email: jonesst2608@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -23,18 +23,18 @@
 takes its design ideas from the hugely popular, ReactJS based, [TanStack Table].
 
 The initial release supports the following features:
 
 - [X] Headless UI, CSS agnostic
 - [X] Freeform text search
 - [X] Forward/Reverse column based sort
-- [X] Pagination
-- [X] Integration with SQLAlchemy (full text search, sort and pagination)
-- [ ] Integration with Pandas and SQLAlchemy (in progress)
-- [ ] Remote large dataset support
+- [X] Pagination (offset, limit)
+- [X] Integration with SQLModel/SQLAlchemy (fts5 based full text search, sort and pagination)
+- [ ] Integration with Pandas (in progress)
+- [ ] Remote large dataset support (in progress)
 
 ## Usage
 
 	pip install reactpy-table
 
 *[basic_example.py](examples/basic_example.py)*
 ```python
@@ -93,16 +93,16 @@
 **examples/table_example.py** demonstrates search, sort and pagination on SP500 
 companies table. The built-in feature data pipeline is used.
 
 **examples/books/books_example.py** demonstrates search, sort and pagination on
 a SQLite book database containing 100k books. Search, sort and 
 pagination is handled by SQL queries.
 
-* Full text search on database < 20ms
-* Page traversal < 2ms
+* FTS5 full text search on database < 20ms
+* Next/Prev page traversal < 2ms
 
 
 ## Feature Set
 
 The row data presented to the user for display is pre-processed by a
 data-pipeline of table features:
 
@@ -128,16 +128,16 @@
 All features are instantiated using a strict pattern. As
 an example a custom paginator that accepts *page _size* and
 *start_page* would be created as follows:
 
 ```
 def getCustomPaginator(page_size, start_page) 
 
-    def _feature_factory(table, updater):
-        return CustomPaginator(table, updater, page_size, start_page)
+    def _feature_factory(table, upstream_data):
+        return CustomPaginator(table, upstream_data, page_size, start_page)
     
     return _feature_factory
 
 ```
 The custom feature is passed as an option when the table is created:
 ```
 table = use_reactpy_table(Options(
```

