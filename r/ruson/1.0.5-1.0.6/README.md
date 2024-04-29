# Comparing `tmp/ruson-1.0.5.tar.gz` & `tmp/ruson-1.0.6.tar.gz`

## Comparing `ruson-1.0.5.tar` & `ruson-1.0.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      314 1970-01-01 00:00:00.000000 ruson-1.0.5/Cargo.toml
--rw-r--r--   0     1001      127     3187 2024-04-12 23:00:10.000000 ruson-1.0.5/.github/workflows/pypi.yml
--rw-r--r--   0     1001      127     1984 2024-04-12 23:00:10.000000 ruson-1.0.5/.github/workflows/test.yml
--rw-r--r--   0     1001      127     4699 2024-04-12 23:00:10.000000 ruson-1.0.5/.gitignore
--rw-r--r--   0     1001      127     6459 2024-04-12 23:00:10.000000 ruson-1.0.5/README.md
--rw-r--r--   0     1001      127      201 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/core/__init__.py
--rw-r--r--   0     1001      127      140 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/core/config.py
--rw-r--r--   0     1001      127     1009 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/core/instance.py
--rw-r--r--   0     1001      127    18549 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/core/ruson_doc.py
--rw-r--r--   0     1001      127        0 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/__init__.py
--rw-r--r--   0     1001      127     1114 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/client.py
--rw-r--r--   0     1001      127      389 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/client.pyi
--rw-r--r--   0     1001      127     5657 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/collection.py
--rw-r--r--   0     1001      127     2971 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/collection.pyi
--rw-r--r--   0     1001      127      723 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/database.py
--rw-r--r--   0     1001      127      211 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/database.pyi
--rw-r--r--   0     1001      127     2138 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/results.py
--rw-r--r--   0     1001      127      944 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/results.pyi
--rw-r--r--   0     1001      127      172 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/session.py
--rw-r--r--   0     1001      127       19 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/session.pyi
--rw-r--r--   0     1001      127     2795 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/types.py
--rw-r--r--   0     1001      127     8211 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/driver/types.pyi
--rw-r--r--   0     1001      127        0 2024-04-12 23:00:10.000000 ruson-1.0.5/ruson/py.typed
--rw-r--r--   0     1001      127    17604 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/bson_binding.rs
--rw-r--r--   0     1001      127     2404 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/client_binding.rs
--rw-r--r--   0     1001      127    13492 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/collection_binding.rs
--rw-r--r--   0     1001      127     1111 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/database_biding.rs
--rw-r--r--   0     1001      127     5730 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/document_binding.rs
--rw-r--r--   0     1001      127     3908 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/index_binding.rs
--rw-r--r--   0     1001      127     3409 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/iterator_binding.rs
--rw-r--r--   0     1001      127     6403 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/mod.rs
--rw-r--r--   0     1001      127     1048 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/results_binding.rs
--rw-r--r--   0     1001      127      444 2024-04-12 23:00:10.000000 ruson-1.0.5/src/bindings/utils.rs
--rw-r--r--   0     1001      127    10666 2024-04-12 23:00:10.000000 ruson-1.0.5/src/interface.rs
--rw-r--r--   0     1001      127      431 2024-04-12 23:00:10.000000 ruson-1.0.5/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/__init__.py
--rw-r--r--   0     1001      127     1432 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/conftest.py
--rw-r--r--   0     1001      127        0 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_aggregate.py
--rw-r--r--   0     1001      127      642 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_connection.py
--rw-r--r--   0     1001      127      386 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_count.py
--rw-r--r--   0     1001      127     1173 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_delete.py
--rw-r--r--   0     1001      127      673 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_distinct.py
--rw-r--r--   0     1001      127      407 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_drop.py
--rw-r--r--   0     1001      127     2474 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_find.py
--rw-r--r--   0     1001      127     1343 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_indexes.py
--rw-r--r--   0     1001      127     1049 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_insert.py
--rw-r--r--   0     1001      127     1477 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_update.py
--rw-r--r--   0     1001      127     1570 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_core/test_upsert.py
--rw-r--r--   0     1001      127        0 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_driver/__init__.py
--rw-r--r--   0     1001      127     1073 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_driver/test_client.py
--rw-r--r--   0     1001      127    11664 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_driver/test_collection.py
--rw-r--r--   0     1001      127      638 2024-04-12 23:00:10.000000 ruson-1.0.5/tests/test_driver/test_db.py
--rw-r--r--   0     1001      127    48136 2024-04-12 23:00:14.000000 ruson-1.0.5/Cargo.lock
--rw-r--r--   0     1001      127      756 2024-04-12 23:00:10.000000 ruson-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 ruson-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      314 1970-01-01 00:00:00.000000 ruson-1.0.6/Cargo.toml
+-rw-r--r--   0     1001      127     3187 2024-04-29 03:04:27.000000 ruson-1.0.6/.github/workflows/pypi.yml
+-rw-r--r--   0     1001      127     1984 2024-04-29 03:04:27.000000 ruson-1.0.6/.github/workflows/test.yml
+-rw-r--r--   0     1001      127     4699 2024-04-29 03:04:27.000000 ruson-1.0.6/.gitignore
+-rw-r--r--   0     1001      127     6459 2024-04-29 03:04:27.000000 ruson-1.0.6/README.md
+-rw-r--r--   0     1001      127      201 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/core/__init__.py
+-rw-r--r--   0     1001      127      140 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/core/config.py
+-rw-r--r--   0     1001      127     1009 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/core/instance.py
+-rw-r--r--   0     1001      127    18586 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/core/ruson_doc.py
+-rw-r--r--   0     1001      127        0 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/driver/__init__.py
+-rw-r--r--   0     1001      127     1114 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/driver/client.py
+-rw-r--r--   0     1001      127      389 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/driver/client.pyi
+-rw-r--r--   0     1001      127     5657 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/driver/collection.py
+-rw-r--r--   0     1001      127     2971 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/driver/collection.pyi
+-rw-r--r--   0     1001      127      723 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/driver/database.py
+-rw-r--r--   0     1001      127      211 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/driver/database.pyi
+-rw-r--r--   0     1001      127     2138 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/driver/results.py
+-rw-r--r--   0     1001      127      944 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/driver/results.pyi
+-rw-r--r--   0     1001      127      172 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/driver/session.py
+-rw-r--r--   0     1001      127       19 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/driver/session.pyi
+-rw-r--r--   0     1001      127     2795 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/driver/types.py
+-rw-r--r--   0     1001      127     8211 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/driver/types.pyi
+-rw-r--r--   0     1001      127        0 2024-04-29 03:04:27.000000 ruson-1.0.6/ruson/py.typed
+-rw-r--r--   0     1001      127    17604 2024-04-29 03:04:27.000000 ruson-1.0.6/src/bindings/bson_binding.rs
+-rw-r--r--   0     1001      127     2404 2024-04-29 03:04:27.000000 ruson-1.0.6/src/bindings/client_binding.rs
+-rw-r--r--   0     1001      127    13492 2024-04-29 03:04:27.000000 ruson-1.0.6/src/bindings/collection_binding.rs
+-rw-r--r--   0     1001      127     1111 2024-04-29 03:04:27.000000 ruson-1.0.6/src/bindings/database_biding.rs
+-rw-r--r--   0     1001      127     5730 2024-04-29 03:04:27.000000 ruson-1.0.6/src/bindings/document_binding.rs
+-rw-r--r--   0     1001      127     3908 2024-04-29 03:04:27.000000 ruson-1.0.6/src/bindings/index_binding.rs
+-rw-r--r--   0     1001      127     3409 2024-04-29 03:04:27.000000 ruson-1.0.6/src/bindings/iterator_binding.rs
+-rw-r--r--   0     1001      127     6403 2024-04-29 03:04:27.000000 ruson-1.0.6/src/bindings/mod.rs
+-rw-r--r--   0     1001      127     1048 2024-04-29 03:04:27.000000 ruson-1.0.6/src/bindings/results_binding.rs
+-rw-r--r--   0     1001      127      444 2024-04-29 03:04:27.000000 ruson-1.0.6/src/bindings/utils.rs
+-rw-r--r--   0     1001      127    10666 2024-04-29 03:04:27.000000 ruson-1.0.6/src/interface.rs
+-rw-r--r--   0     1001      127      431 2024-04-29 03:04:27.000000 ruson-1.0.6/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/__init__.py
+-rw-r--r--   0     1001      127     1432 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/conftest.py
+-rw-r--r--   0     1001      127        0 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_core/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_core/test_aggregate.py
+-rw-r--r--   0     1001      127      642 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_core/test_connection.py
+-rw-r--r--   0     1001      127      386 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_core/test_count.py
+-rw-r--r--   0     1001      127     1173 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_core/test_delete.py
+-rw-r--r--   0     1001      127      673 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_core/test_distinct.py
+-rw-r--r--   0     1001      127      407 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_core/test_drop.py
+-rw-r--r--   0     1001      127     2474 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_core/test_find.py
+-rw-r--r--   0     1001      127     1343 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_core/test_indexes.py
+-rw-r--r--   0     1001      127     1049 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_core/test_insert.py
+-rw-r--r--   0     1001      127     1477 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_core/test_update.py
+-rw-r--r--   0     1001      127     1570 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_core/test_upsert.py
+-rw-r--r--   0     1001      127        0 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_driver/__init__.py
+-rw-r--r--   0     1001      127     1073 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_driver/test_client.py
+-rw-r--r--   0     1001      127    11664 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_driver/test_collection.py
+-rw-r--r--   0     1001      127      638 2024-04-29 03:04:27.000000 ruson-1.0.6/tests/test_driver/test_db.py
+-rw-r--r--   0     1001      127    48341 2024-04-29 03:04:31.000000 ruson-1.0.6/Cargo.lock
+-rw-r--r--   0     1001      127      756 2024-04-29 03:04:27.000000 ruson-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 ruson-1.0.6/PKG-INFO
```

### Comparing `ruson-1.0.5/.github/workflows/pypi.yml` & `ruson-1.0.6/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/.github/workflows/test.yml` & `ruson-1.0.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/.gitignore` & `ruson-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/README.md` & `ruson-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/ruson/core/instance.py` & `ruson-1.0.6/ruson/core/instance.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/ruson/core/ruson_doc.py` & `ruson-1.0.6/ruson/core/ruson_doc.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,17 @@
     db = client.database(db_name)
     return db.collection(collection_name)
 
 
 def _recurse_value(
     value: BaseTypes | CollectionTypes,
 ) -> BaseTypes | Document | list[BaseTypes | Document]:
+    if isinstance(value, bytes):
+        return list(value)
+
     if isinstance(value, Mapping):
         doc = Document()
         for key, val in value.items():
             doc[key] = _recurse_value(val)
         return doc
 
     if isinstance(value, list):
@@ -203,48 +206,45 @@
         batch_size: int | None = None,
         projection: Projection | Document | None = None,
         timeout: int | None = None,
         formatter: Callable[[Document], T | Awaitable[T]] = noop_formatter,
         session: Session | None = None,
         db_name: str | None = None,
         conn_name: str | None = None,
-    ) -> T:
-        ...
+    ) -> T: ...
 
     @overload
     async def find(
         self: Self,
         many: Literal[True],
         skip: int | None = None,
         sort: list[FieldSort] | None = None,
         batch_size: int | None = None,
         projection: Projection | Document | None = None,
         timeout: int | None = None,
         formatter: Callable[[Document], T | Awaitable[T]] = noop_formatter,
         session: Session | None = None,
         db_name: str | None = None,
         conn_name: str | None = None,
-    ) -> DocumentsCursor[T]:
-        ...
+    ) -> DocumentsCursor[T]: ...
 
     @overload
     async def find(
         self: Self,
         many=False,
         skip: int | None = None,
         sort: list[FieldSort] | None = None,
         batch_size: int | None = None,
         projection: Projection | Document | None = None,
         timeout: int | None = None,
         formatter: Callable[[Document], T | Awaitable[T]] = noop_formatter,
         session: Session | None = None,
         db_name: str | None = None,
         conn_name: str | None = None,
-    ) -> T:
-        ...
+    ) -> T: ...
 
     async def find(
         self: Self,
         skip: int | None = None,
         sort: list[FieldSort] | None = None,
         batch_size: int | None = None,
         projection: Projection | Document | None = None,
```

### Comparing `ruson-1.0.5/ruson/driver/client.py` & `ruson-1.0.6/ruson/driver/client.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/ruson/driver/collection.py` & `ruson-1.0.6/ruson/driver/collection.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/ruson/driver/collection.pyi` & `ruson-1.0.6/ruson/driver/collection.pyi`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/ruson/driver/database.py` & `ruson-1.0.6/ruson/driver/database.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/ruson/driver/results.py` & `ruson-1.0.6/ruson/driver/results.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/ruson/driver/results.pyi` & `ruson-1.0.6/ruson/driver/results.pyi`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/ruson/driver/types.py` & `ruson-1.0.6/ruson/driver/types.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/ruson/driver/types.pyi` & `ruson-1.0.6/ruson/driver/types.pyi`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/src/bindings/bson_binding.rs` & `ruson-1.0.6/src/bindings/bson_binding.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/src/bindings/client_binding.rs` & `ruson-1.0.6/src/bindings/client_binding.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/src/bindings/collection_binding.rs` & `ruson-1.0.6/src/bindings/collection_binding.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/src/bindings/database_biding.rs` & `ruson-1.0.6/src/bindings/database_biding.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/src/bindings/document_binding.rs` & `ruson-1.0.6/src/bindings/document_binding.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/src/bindings/index_binding.rs` & `ruson-1.0.6/src/bindings/index_binding.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/src/bindings/iterator_binding.rs` & `ruson-1.0.6/src/bindings/iterator_binding.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/src/bindings/mod.rs` & `ruson-1.0.6/src/bindings/mod.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/src/bindings/results_binding.rs` & `ruson-1.0.6/src/bindings/results_binding.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/src/interface.rs` & `ruson-1.0.6/src/interface.rs`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/tests/conftest.py` & `ruson-1.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/tests/test_core/test_connection.py` & `ruson-1.0.6/tests/test_core/test_connection.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/tests/test_core/test_delete.py` & `ruson-1.0.6/tests/test_core/test_delete.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/tests/test_core/test_distinct.py` & `ruson-1.0.6/tests/test_core/test_distinct.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/tests/test_core/test_find.py` & `ruson-1.0.6/tests/test_core/test_find.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/tests/test_core/test_indexes.py` & `ruson-1.0.6/tests/test_core/test_indexes.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/tests/test_core/test_insert.py` & `ruson-1.0.6/tests/test_core/test_insert.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/tests/test_core/test_update.py` & `ruson-1.0.6/tests/test_core/test_update.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/tests/test_core/test_upsert.py` & `ruson-1.0.6/tests/test_core/test_upsert.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/tests/test_driver/test_client.py` & `ruson-1.0.6/tests/test_driver/test_client.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/tests/test_driver/test_collection.py` & `ruson-1.0.6/tests/test_driver/test_collection.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/tests/test_driver/test_db.py` & `ruson-1.0.6/tests/test_driver/test_db.py`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/Cargo.lock` & `ruson-1.0.6/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 name = "async-trait"
 version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
@@ -92,14 +92,20 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
+
+[[package]]
 name = "bitvec"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
 dependencies = [
  "funty",
  "radium",
@@ -147,29 +153,29 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.92"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.37"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "num-traits",
  "windows-targets 0.52.5",
 ]
 
@@ -237,17 +243,17 @@
  "darling_core",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "data-encoding"
-version = "2.5.0"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e962a19be5cfc3f3bf6dd8f61eb50107f356ad6270fbb3ed41476571db78be5"
+checksum = "e8566979429cf69b49a5c740c60791108e86440e8be149bbea4fe54d2c32d6e2"
 
 [[package]]
 name = "deranged"
 version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
@@ -386,15 +392,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -448,17 +454,17 @@
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
@@ -609,17 +615,17 @@
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -697,15 +703,15 @@
 name = "mongodb"
 version = "2.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef206acb1b72389b49bc9985efe7eb1f8a9bb18e5680d262fac26c07f44025f1"
 dependencies = [
  "async-trait",
  "base64 0.13.1",
- "bitflags",
+ "bitflags 1.3.2",
  "bson",
  "chrono",
  "derivative",
  "derive_more",
  "futures-core",
  "futures-executor",
  "futures-io",
@@ -778,33 +784,33 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "pbkdf2"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "83a0692ec44e4cf1ef28ca317f14f8f07da2d95ec3fa01f86e4467b725e60917"
@@ -840,17 +846,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.19.2"
@@ -985,19 +991,19 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "resolv-conf"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "52e44394d2086d010551b14b53b1f24e31647570cd1deb0379e2c21b329aba00"
@@ -1019,15 +1025,15 @@
  "spin",
  "untrusted",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "ruson"
-version = "1.0.5"
+version = "1.0.6"
 dependencies = [
  "mongodb",
  "pyo3",
  "pyo3-asyncio",
  "serde",
  "tokio",
 ]
@@ -1064,17 +1070,17 @@
 dependencies = [
  "rustc_version 0.2.3",
  "semver 0.9.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.10"
+version = "0.21.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
+checksum = "3f56a14d1f48b391359b22f731fd4bd7e43c97f3c50eee276f3aa09c94784d3e"
 dependencies = [
  "log",
  "ring",
  "rustls-webpki",
  "sct",
 ]
 
@@ -1138,17 +1144,17 @@
 name = "semver-parser"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388a1df253eca08550bef6c72392cfe7c30914bf41df5269b68cbd6ff8f570a3"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
 version = "0.11.14"
@@ -1156,28 +1162,28 @@
 checksum = "8b8497c313fd43ab992087548117643f6fcd935cbf36f176ffda0aacf9591734"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
@@ -1223,17 +1229,17 @@
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "slab"
 version = "0.4.9"
@@ -1307,17 +1313,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1336,30 +1342,30 @@
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "time"
 version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
@@ -1426,15 +1432,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
@@ -1602,15 +1608,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1624,15 +1630,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -1853,9 +1859,9 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
```

### Comparing `ruson-1.0.5/pyproject.toml` & `ruson-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ruson-1.0.5/PKG-INFO` & `ruson-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ruson
-Version: 1.0.5
+Version: 1.0.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pydantic >=2.5
 Requires-Dist: pytz
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: pytest-asyncio ; extra == 'test'
```

