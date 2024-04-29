# Comparing `tmp/veilid-0.3.1.tar.gz` & `tmp/veilid-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilid-0.3.1.tar", max compression
+gzip compressed data, was "veilid-0.3.2.tar", max compression
```

## Comparing `veilid-0.3.1.tar` & `veilid-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    15581 2023-07-19 16:52:47.952728 veilid-0.3.1/LICENSE.md
--rw-r--r--   0        0        0      833 2024-04-05 01:29:50.201762 veilid-0.3.1/README.md
--rw-r--r--   0        0        0      541 2024-04-05 01:29:50.201762 veilid-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      128 2023-07-17 21:54:35.187940 veilid-0.3.1/veilid/__init__.py
--rw-r--r--   0        0        0    10005 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/api.py
--rw-r--r--   0        0        0     5217 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/config.py
--rw-r--r--   0        0        0     3594 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/error.py
--rw-r--r--   0        0        0    41203 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/json_api.py
--rw-r--r--   0        0        0     3039 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/operations.py
--rw-r--r--   0        0        0   103960 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/schema/RecvMessage.json
--rw-r--r--   0        0        0    38789 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/schema/Request.json
--rw-r--r--   0        0        0    12291 2024-04-05 01:29:50.201762 veilid-0.3.1/veilid/state.py
--rw-r--r--   0        0        0    12702 2024-04-05 01:29:50.205762 veilid-0.3.1/veilid/types.py
--rw-r--r--   0        0        0     1211 1970-01-01 00:00:00.000000 veilid-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    15581 2023-07-19 16:52:47.952728 veilid-0.3.2/LICENSE.md
+-rw-r--r--   0        0        0      833 2024-04-05 01:29:50.201762 veilid-0.3.2/README.md
+-rw-r--r--   0        0        0      541 2024-04-29 01:56:12.437594 veilid-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-07-17 21:54:35.187940 veilid-0.3.2/veilid/__init__.py
+-rw-r--r--   0        0        0    10059 2024-04-29 01:56:12.437594 veilid-0.3.2/veilid/api.py
+-rw-r--r--   0        0        0     5217 2024-04-05 01:29:50.201762 veilid-0.3.2/veilid/config.py
+-rw-r--r--   0        0        0     3594 2024-04-05 01:29:50.201762 veilid-0.3.2/veilid/error.py
+-rw-r--r--   0        0        0    41251 2024-04-29 01:56:12.437594 veilid-0.3.2/veilid/json_api.py
+-rw-r--r--   0        0        0     3039 2024-04-05 01:29:50.201762 veilid-0.3.2/veilid/operations.py
+-rw-r--r--   0        0        0   104576 2024-04-29 01:56:12.437594 veilid-0.3.2/veilid/schema/RecvMessage.json
+-rw-r--r--   0        0        0    38789 2024-04-05 01:29:50.201762 veilid-0.3.2/veilid/schema/Request.json
+-rw-r--r--   0        0        0    12291 2024-04-05 01:29:50.201762 veilid-0.3.2/veilid/state.py
+-rw-r--r--   0        0        0    12971 2024-04-29 01:56:12.437594 veilid-0.3.2/veilid/types.py
+-rw-r--r--   0        0        0     1211 1970-01-01 00:00:00.000000 veilid-0.3.2/PKG-INFO
```

### Comparing `veilid-0.3.1/LICENSE.md` & `veilid-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `veilid-0.3.1/README.md` & `veilid-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `veilid-0.3.1/pyproject.toml` & `veilid-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # --- Bumpversion match - do not reorder
 name = "veilid"
-version = "0.3.1"
+version = "0.3.2"
 # ---
 description = ""
 authors = ["Veilid Team <contact@veilid.com>"]
 readme = "README.md"
 packages = [{ include = "veilid" }]
 
 [tool.poetry.dependencies]
```

### Comparing `veilid-0.3.1/veilid/api.py` & `veilid-0.3.2/veilid/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,31 +65,31 @@
 
     @abstractmethod
     async def delete_dht_record(self, key: types.TypedKey):
         pass
 
     @abstractmethod
     async def get_dht_value(
-        self, key: types.TypedKey, subkey: types.ValueSubkey, force_refresh: bool
+        self, key: types.TypedKey, subkey: types.ValueSubkey, force_refresh: bool = False
     ) -> Optional[types.ValueData]:
         pass
 
     @abstractmethod
     async def set_dht_value(
         self, key: types.TypedKey, subkey: types.ValueSubkey, data: bytes, writer: Optional[types.KeyPair] = None
     ) -> Optional[types.ValueData]:
         pass
 
     @abstractmethod
     async def watch_dht_values(
         self,
         key: types.TypedKey,
         subkeys: list[tuple[types.ValueSubkey, types.ValueSubkey]],
-        expiration: types.Timestamp,
-        count: int,
+        expiration: types.Timestamp = 0,
+        count: int = 0xFFFFFFFF,
     ) -> types.Timestamp:
         pass
 
     @abstractmethod
     async def cancel_dht_watch(
         self,
         key: types.TypedKey,
@@ -98,15 +98,15 @@
         pass
 
     @abstractmethod
     async def inspect_dht_record(
         self,
         key: types.TypedKey,
         subkeys: list[tuple[types.ValueSubkey, types.ValueSubkey]],
-        scope: types.DHTReportScope,
+        scope: types.DHTReportScope = types.DHTReportScope.LOCAL,
     ) -> types.DHTRecordReport:
         pass
 
 
 
 class TableDbTransaction(ABC):
     async def __aenter__(self) -> Self:
```

### Comparing `veilid-0.3.1/veilid/config.py` & `veilid-0.3.2/veilid/config.py`

 * *Files identical despite different names*

### Comparing `veilid-0.3.1/veilid/error.py` & `veilid-0.3.2/veilid/error.py`

 * *Files identical despite different names*

### Comparing `veilid-0.3.1/veilid/json_api.py` & `veilid-0.3.2/veilid/json_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -615,15 +615,15 @@
                 rc_id=self.rc_id,
                 rc_op=RoutingContextOperation.DELETE_DHT_RECORD,
                 key=key,
             )
         )
 
     async def get_dht_value(
-        self, key: TypedKey, subkey: ValueSubkey, force_refresh: bool
+        self, key: TypedKey, subkey: ValueSubkey, force_refresh: bool = False
     ) -> Optional[ValueData]:
         ret = raise_api_result(
             await self.api.send_ndjson_request(
                 Operation.ROUTING_CONTEXT,
                 validate=validate_rc_op,
                 rc_id=self.rc_id,
                 rc_op=RoutingContextOperation.GET_DHT_VALUE,
@@ -651,16 +651,16 @@
         )
         return None if ret is None else ValueData.from_json(ret)
 
     async def watch_dht_values(
         self,
         key: TypedKey,
         subkeys: list[tuple[ValueSubkey, ValueSubkey]],
-        expiration: Timestamp,
-        count: int,
+        expiration: Timestamp = 0,
+        count: int = 0xFFFFFFFF,
     ) -> Timestamp:
         return Timestamp(
             raise_api_result(
                 await self.api.send_ndjson_request(
                     Operation.ROUTING_CONTEXT,
                     validate=validate_rc_op,
                     rc_id=self.rc_id,
@@ -687,15 +687,15 @@
             )
         )
 
     async def inspect_dht_record(
         self,
         key: TypedKey,
         subkeys: list[tuple[ValueSubkey, ValueSubkey]],
-        scope: DHTReportScope,
+        scope: DHTReportScope = DHTReportScope.LOCAL,
     ) -> DHTRecordReport:
         return DHTRecordReport.from_json(            
             raise_api_result(
                 await self.api.send_ndjson_request(
                     Operation.ROUTING_CONTEXT,
                     validate=validate_rc_op,
                     rc_id=self.rc_id,
```

### Comparing `veilid-0.3.1/veilid/operations.py` & `veilid-0.3.2/veilid/operations.py`

 * *Files identical despite different names*

### Comparing `veilid-0.3.1/veilid/schema/RecvMessage.json` & `veilid-0.3.2/veilid/schema/RecvMessage.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999069940476191%*

 * *Differences: {"'definitions'": "{'DHTRecordReport': {'required': {insert: [(2, 'offline_subkeys')]}, "*

 * *                  "'properties': {'offline_subkeys': OrderedDict([('description', 'The subkeys "*

 * *                  "that have been writen offline that still need to be flushed'), ('type', "*

 * *                  "'array'), ('items', OrderedDict([('type', 'array'), ('items', "*

 * *                  "[OrderedDict([('type', 'integer'), ('format', 'uint32'), ('minimum', 0.0)]), "*

 * *                  "OrderedDict([('type', 'integer') […]*

```diff
@@ -66,14 +66,35 @@
                     "items": {
                         "format": "uint32",
                         "minimum": 0.0,
                         "type": "integer"
                     },
                     "type": "array"
                 },
+                "offline_subkeys": {
+                    "description": "The subkeys that have been writen offline that still need to be flushed",
+                    "items": {
+                        "items": [
+                            {
+                                "format": "uint32",
+                                "minimum": 0.0,
+                                "type": "integer"
+                            },
+                            {
+                                "format": "uint32",
+                                "minimum": 0.0,
+                                "type": "integer"
+                            }
+                        ],
+                        "maxItems": 2,
+                        "minItems": 2,
+                        "type": "array"
+                    },
+                    "type": "array"
+                },
                 "subkeys": {
                     "description": "The actual subkey range within the schema being reported on This may be a subset of the requested range if it exceeds the schema limits or has more than 512 subkeys",
                     "items": {
                         "items": [
                             {
                                 "format": "uint32",
                                 "minimum": 0.0,
@@ -91,14 +112,15 @@
                     },
                     "type": "array"
                 }
             },
             "required": [
                 "local_seqs",
                 "network_seqs",
+                "offline_subkeys",
                 "subkeys"
             ],
             "type": "object"
         },
         "DHTSchema": {
             "description": "Enum over all the supported DHT Schemas",
             "oneOf": [
```

### Comparing `veilid-0.3.1/veilid/schema/Request.json` & `veilid-0.3.2/veilid/schema/Request.json`

 * *Files identical despite different names*

### Comparing `veilid-0.3.1/veilid/state.py` & `veilid-0.3.2/veilid/state.py`

 * *Files identical despite different names*

### Comparing `veilid-0.3.1/veilid/types.py` & `veilid-0.3.2/veilid/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,34 +378,38 @@
     def to_json(self) -> dict:
         return self.__dict__
 
 
 
 class DHTRecordReport:
     subkeys: list[tuple[ValueSubkey, ValueSubkey]]
+    offline_subkeys: list[tuple[ValueSubkey, ValueSubkey]]
     local_seqs: list[ValueSeqNum]
     network_seqs: list[ValueSeqNum]
 
     def __init__(
         self,
         subkeys: list[tuple[ValueSubkey, ValueSubkey]],
+        offline_subkeys: list[tuple[ValueSubkey, ValueSubkey]],
         local_seqs: list[ValueSeqNum],
         network_seqs: list[ValueSeqNum],
     ):
         self.subkeys = subkeys
+        self.offline_subkey = offline_subkeys
         self.local_seqs = local_seqs
         self.network_seqs = network_seqs
 
     def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}(subkeys={self.subkeys!r}, local_seqs={self.local_seqs!r}, network_seqs={self.network_seqs!r})>"
+        return f"<{self.__class__.__name__}(subkeys={self.subkeys!r}, offline_subkeys={self.offline_subkeys!r}, local_seqs={self.local_seqs!r}, network_seqs={self.network_seqs!r})>"
 
     @classmethod
     def from_json(cls, j: dict) -> Self:
         return cls(
             [[p[0], p[1]] for p in j["subkeys"]],
+            [[p[0], p[1]] for p in j["offline_subkeys"]],
             [ValueSeqNum(s) for s in j["local_seqs"]],
             [ValueSeqNum(s) for s in j["network_seqs"]],
         )
 
     def to_json(self) -> dict:
         return self.__dict__
```

### Comparing `veilid-0.3.1/PKG-INFO` & `veilid-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilid
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: Veilid Team
 Author-email: contact@veilid.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

