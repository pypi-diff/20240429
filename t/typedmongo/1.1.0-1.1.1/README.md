# Comparing `tmp/typedmongo-1.1.0.tar.gz` & `tmp/typedmongo-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedmongo-1.1.0.tar", last modified: Sun Apr 28 08:08:40 2024, max compression
+gzip compressed data, was "typedmongo-1.1.1.tar", last modified: Mon Apr 29 09:26:54 2024, max compression
```

## Comparing `typedmongo-1.1.0.tar` & `typedmongo-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-28 08:08:23.132404 typedmongo-1.1.0/LICENSE
--rw-r--r--   0        0        0      108 2024-04-28 08:08:23.132404 typedmongo-1.1.0/README.md
--rw-r--r--   0        0        0     1441 2024-04-28 08:08:40.600456 typedmongo-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-28 08:08:23.136404 typedmongo-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 08:08:23.136404 typedmongo-1.1.0/tests/asyncio/__init__.py
--rw-r--r--   0        0        0     5789 2024-04-28 08:08:23.136404 typedmongo-1.1.0/tests/asyncio/test_client.py
--rw-r--r--   0        0        0     3749 2024-04-28 08:08:23.136404 typedmongo-1.1.0/tests/asyncio/test_table.py
--rw-r--r--   0        0        0     1218 2024-04-28 08:08:23.136404 typedmongo-1.1.0/tests/sync.py
--rw-r--r--   0        0        0     5549 2024-04-28 08:08:23.136404 typedmongo-1.1.0/tests/test_client.py
--rw-r--r--   0        0        0     2930 2024-04-28 08:08:23.136404 typedmongo-1.1.0/tests/test_expressions.py
--rw-r--r--   0        0        0      582 2024-04-28 08:08:23.136404 typedmongo-1.1.0/tests/test_marshamallow.py
--rw-r--r--   0        0        0     3741 2024-04-28 08:08:23.136404 typedmongo-1.1.0/tests/test_table.py
--rw-r--r--   0        0        0      781 2024-04-28 08:08:23.136404 typedmongo-1.1.0/typedmongo/__init__.py
--rw-r--r--   0        0        0      781 2024-04-28 08:08:23.136404 typedmongo-1.1.0/typedmongo/asyncio/__init__.py
--rw-r--r--   0        0        0    11612 2024-04-28 08:08:23.136404 typedmongo-1.1.0/typedmongo/asyncio/client.py
--rw-r--r--   0        0        0     9095 2024-04-28 08:08:23.136404 typedmongo-1.1.0/typedmongo/asyncio/fields.py
--rw-r--r--   0        0        0     7820 2024-04-28 08:08:23.136404 typedmongo-1.1.0/typedmongo/asyncio/table.py
--rw-r--r--   0        0        0    11394 2024-04-28 08:08:23.136404 typedmongo-1.1.0/typedmongo/client.py
--rw-r--r--   0        0        0      163 2024-04-28 08:08:23.136404 typedmongo-1.1.0/typedmongo/exceptions.py
--rw-r--r--   0        0        0     5452 2024-04-28 08:08:23.136404 typedmongo-1.1.0/typedmongo/expressions.py
--rw-r--r--   0        0        0     9095 2024-04-28 08:08:23.136404 typedmongo-1.1.0/typedmongo/fields.py
--rw-r--r--   0        0        0      351 2024-04-28 08:08:23.136404 typedmongo-1.1.0/typedmongo/marshamallow.py
--rw-r--r--   0        0        0     1325 2024-04-28 08:08:23.136404 typedmongo-1.1.0/typedmongo/sync.py
--rw-r--r--   0        0        0     7820 2024-04-28 08:08:23.136404 typedmongo-1.1.0/typedmongo/table.py
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 typedmongo-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-29 09:26:40.977586 typedmongo-1.1.1/LICENSE
+-rw-r--r--   0        0        0      108 2024-04-29 09:26:40.977586 typedmongo-1.1.1/README.md
+-rw-r--r--   0        0        0     1441 2024-04-29 09:26:54.473665 typedmongo-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/asyncio/__init__.py
+-rw-r--r--   0        0        0     5789 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/asyncio/test_client.py
+-rw-r--r--   0        0        0     3749 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/asyncio/test_table.py
+-rw-r--r--   0        0        0     1218 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/sync.py
+-rw-r--r--   0        0        0     5549 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/test_client.py
+-rw-r--r--   0        0        0     2930 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/test_expressions.py
+-rw-r--r--   0        0        0      582 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/test_marshamallow.py
+-rw-r--r--   0        0        0     3741 2024-04-29 09:26:40.981586 typedmongo-1.1.1/tests/test_table.py
+-rw-r--r--   0        0        0      781 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/__init__.py
+-rw-r--r--   0        0        0      781 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/asyncio/__init__.py
+-rw-r--r--   0        0        0    11612 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/asyncio/client.py
+-rw-r--r--   0        0        0     9494 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/asyncio/fields.py
+-rw-r--r--   0        0        0     8071 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/asyncio/table.py
+-rw-r--r--   0        0        0    11394 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/client.py
+-rw-r--r--   0        0        0      163 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/exceptions.py
+-rw-r--r--   0        0        0     5452 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/expressions.py
+-rw-r--r--   0        0        0     9494 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/fields.py
+-rw-r--r--   0        0        0      538 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/marshamallow.py
+-rw-r--r--   0        0        0     1325 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/sync.py
+-rw-r--r--   0        0        0     8071 2024-04-29 09:26:40.981586 typedmongo-1.1.1/typedmongo/table.py
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 typedmongo-1.1.1/PKG-INFO
```

### Comparing `typedmongo-1.1.0/LICENSE` & `typedmongo-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.0/pyproject.toml` & `typedmongo-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "typedmongo"
-version = "1.1.0"
+version = "1.1.1"
 description = "A production-ready modern Python MongoDB ODM"
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "pymongo>=4.6.3",
     "motor>=3.4.0",
```

### Comparing `typedmongo-1.1.0/tests/asyncio/test_client.py` & `typedmongo-1.1.1/tests/asyncio/test_client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.0/tests/asyncio/test_table.py` & `typedmongo-1.1.1/tests/asyncio/test_table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.0/tests/sync.py` & `typedmongo-1.1.1/tests/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.0/tests/test_client.py` & `typedmongo-1.1.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.0/tests/test_expressions.py` & `typedmongo-1.1.1/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.0/tests/test_marshamallow.py` & `typedmongo-1.1.1/tests/test_marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.0/tests/test_table.py` & `typedmongo-1.1.1/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.0/typedmongo/__init__.py` & `typedmongo-1.1.1/typedmongo/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.0/typedmongo/asyncio/__init__.py` & `typedmongo-1.1.1/typedmongo/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.0/typedmongo/asyncio/client.py` & `typedmongo-1.1.1/typedmongo/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.0/typedmongo/asyncio/fields.py` & `typedmongo-1.1.1/typedmongo/asyncio/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,17 @@
 
     def load(self, value: Any, *, partial: bool = False) -> FieldType:
         return value
 
     def dump(self, value: FieldType) -> Any:
         return value
 
+    def to_mongo(self, value: FieldType) -> Any:
+        return value
+
 
 @dataclasses.dataclass(eq=False)
 class ObjectIdField(Field[ObjectId]):
     """
     ObjectId field
     """
 
@@ -218,16 +221,20 @@
 
         def load(value: Any, *, partial: bool = False) -> T:
             return self.schema.load(value, partial=partial)
 
         def dump(value: T) -> dict[str, Any]:
             return self.schema.dump(value)
 
+        def to_mongo(value: T) -> dict[str, Any]:
+            return self.schema.to_mongo(value)
+
         self.load = load
         self.dump = dump
+        self.to_mongo = to_mongo
 
     def __set_name__(self, owner: type[Table], name: str) -> None:
         if not issubclass(self.schema, owner):
             self.schema.__lazy_init_fields__()
         return super().__set_name__(owner, name)
 
     def get_field_type(self) -> type[T]:
@@ -281,16 +288,20 @@
 
             def load(value: Any, *, partial: bool = False) -> list[FieldType]:
                 return [self.field.load(item, partial=partial) for item in value]  # type: ignore
 
             def dump(value: list[FieldType]) -> list[dict[str, Any]]:
                 return [self.field.dump(item) for item in value]  # type: ignore
 
+            def to_mongo(value: list[FieldType]) -> list[dict[str, Any]]:
+                return [self.field.to_mongo(item) for item in value]  # type: ignore
+
             self.load = load
             self.dump = dump
+            self.to_mongo = to_mongo
 
     def get_field_type(self) -> type[list[FieldType]]:
         return list[self.field.get_field_type()]  # type: ignore
 
 
 def type_to_field(type_: type) -> Field:
     from .table import Table
```

### Comparing `typedmongo-1.1.0/typedmongo/asyncio/table.py` & `typedmongo-1.1.1/typedmongo/asyncio/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,19 +219,28 @@
             key: getattr(cls.__fields__[key], "load")(value, partial=partial)
             for key, value in validated.items()
         }
         return cls(**loaded)
 
     @classmethod
     def dump(cls, instance: Self) -> dict[str, Any]:
+        """
+        Dump the instance to jsonable dict.
+        """
         dumped = {
             key: getattr(instance.__fields__[key], "dump")(value)
             for key, value in instance.__dict__.items()
         }
         return cls.__schema__.dump(dumped)  # type: ignore
 
     @classmethod
     def indexes(cls) -> list[Index]:
         return []
 
     def to_mongo(self) -> dict[str, Any]:
-        return self.dump(self)
+        """
+        Dump the instance to dict for mongo.
+        """
+        return {
+            key: getattr(self.__fields__[key], "to_mongo")(value)
+            for key, value in self.__dict__.items()
+        }
```

### Comparing `typedmongo-1.1.0/typedmongo/client.py` & `typedmongo-1.1.1/typedmongo/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.0/typedmongo/expressions.py` & `typedmongo-1.1.1/typedmongo/expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.0/typedmongo/fields.py` & `typedmongo-1.1.1/typedmongo/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,17 @@
 
     def load(self, value: Any, *, partial: bool = False) -> FieldType:
         return value
 
     def dump(self, value: FieldType) -> Any:
         return value
 
+    def to_mongo(self, value: FieldType) -> Any:
+        return value
+
 
 @dataclasses.dataclass(eq=False)
 class ObjectIdField(Field[ObjectId]):
     """
     ObjectId field
     """
 
@@ -218,16 +221,20 @@
 
         def load(value: Any, *, partial: bool = False) -> T:
             return self.schema.load(value, partial=partial)
 
         def dump(value: T) -> dict[str, Any]:
             return self.schema.dump(value)
 
+        def to_mongo(value: T) -> dict[str, Any]:
+            return self.schema.to_mongo(value)
+
         self.load = load
         self.dump = dump
+        self.to_mongo = to_mongo
 
     def __set_name__(self, owner: type[Table], name: str) -> None:
         if not issubclass(self.schema, owner):
             self.schema.__lazy_init_fields__()
         return super().__set_name__(owner, name)
 
     def get_field_type(self) -> type[T]:
@@ -281,16 +288,20 @@
 
             def load(value: Any, *, partial: bool = False) -> list[FieldType]:
                 return [self.field.load(item, partial=partial) for item in value]  # type: ignore
 
             def dump(value: list[FieldType]) -> list[dict[str, Any]]:
                 return [self.field.dump(item) for item in value]  # type: ignore
 
+            def to_mongo(value: list[FieldType]) -> list[dict[str, Any]]:
+                return [self.field.to_mongo(item) for item in value]  # type: ignore
+
             self.load = load
             self.dump = dump
+            self.to_mongo = to_mongo
 
     def get_field_type(self) -> type[list[FieldType]]:
         return list[self.field.get_field_type()]  # type: ignore
 
 
 def type_to_field(type_: type) -> Field:
     from .table import Table
```

### Comparing `typedmongo-1.1.0/typedmongo/sync.py` & `typedmongo-1.1.1/typedmongo/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.0/typedmongo/table.py` & `typedmongo-1.1.1/typedmongo/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,19 +219,28 @@
             key: getattr(cls.__fields__[key], "load")(value, partial=partial)
             for key, value in validated.items()
         }
         return cls(**loaded)
 
     @classmethod
     def dump(cls, instance: Self) -> dict[str, Any]:
+        """
+        Dump the instance to jsonable dict.
+        """
         dumped = {
             key: getattr(instance.__fields__[key], "dump")(value)
             for key, value in instance.__dict__.items()
         }
         return cls.__schema__.dump(dumped)  # type: ignore
 
     @classmethod
     def indexes(cls) -> list[Index]:
         return []
 
     def to_mongo(self) -> dict[str, Any]:
-        return self.dump(self)
+        """
+        Dump the instance to dict for mongo.
+        """
+        return {
+            key: getattr(self.__fields__[key], "to_mongo")(value)
+            for key, value in self.__dict__.items()
+        }
```

