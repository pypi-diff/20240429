# Comparing `tmp/cottontaildb-client-0.14.2.tar.gz` & `tmp/cottontaildb_client-0.16.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cottontaildb-client-0.14.2.tar", last modified: Mon Jun 12 18:53:01 2023, max compression
+gzip compressed data, was "cottontaildb_client-0.16.6.tar", last modified: Mon Apr 29 09:49:13 2024, max compression
```

## Comparing `cottontaildb-client-0.14.2.tar` & `cottontaildb_client-0.16.6.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:53:01.691947 cottontaildb-client-0.14.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-12 18:53:01.691947 cottontaildb-client-0.14.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:53:01.691947 cottontaildb-client-0.14.2/cottontaildb_client/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/cottontaildb_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/cottontaildb_client/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50592 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/cottontaildb_client/cottontail_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/cottontaildb_client/cottontail_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/cottontaildb_client/cottontaildb_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21761 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/cottontaildb_client/cottontaildb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:53:01.691947 cottontaildb-client-0.14.2/cottontaildb_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-12 18:53:01.000000 cottontaildb-client-0.14.2/cottontaildb_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-12 18:53:01.000000 cottontaildb-client-0.14.2/cottontaildb_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:53:01.000000 cottontaildb-client-0.14.2/cottontaildb_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 18:53:01.000000 cottontaildb-client-0.14.2/cottontaildb_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 18:53:01.000000 cottontaildb-client-0.14.2/cottontaildb_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-12 18:53:01.000000 cottontaildb-client-0.14.2/cottontaildb_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-12 18:53:01.691947 cottontaildb-client-0.14.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:53:01.691947 cottontaildb-client-0.14.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/tests/test_cottontaildb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:49:13.183917 cottontaildb_client-0.16.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 09:49:05.000000 cottontaildb_client-0.16.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-29 09:49:13.183917 cottontaildb_client-0.16.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-29 09:49:05.000000 cottontaildb_client-0.16.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:49:13.183917 cottontaildb_client-0.16.6/cottontaildb_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-29 09:49:05.000000 cottontaildb_client-0.16.6/cottontaildb_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-29 09:49:05.000000 cottontaildb_client-0.16.6/cottontaildb_client/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30024 2024-04-29 09:49:05.000000 cottontaildb_client-0.16.6/cottontaildb_client/cottontail_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35326 2024-04-29 09:49:05.000000 cottontaildb_client-0.16.6/cottontaildb_client/cottontail_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    49101 2024-04-29 09:49:05.000000 cottontaildb_client-0.16.6/cottontaildb_client/cottontail_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-29 09:49:05.000000 cottontaildb_client-0.16.6/cottontaildb_client/cottontaildb_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21854 2024-04-29 09:49:05.000000 cottontaildb_client-0.16.6/cottontaildb_client/cottontaildb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:49:13.183917 cottontaildb_client-0.16.6/cottontaildb_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-29 09:49:13.000000 cottontaildb_client-0.16.6/cottontaildb_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-29 09:49:13.000000 cottontaildb_client-0.16.6/cottontaildb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:49:13.000000 cottontaildb_client-0.16.6/cottontaildb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-29 09:49:13.000000 cottontaildb_client-0.16.6/cottontaildb_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-29 09:49:13.000000 cottontaildb_client-0.16.6/cottontaildb_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 09:49:13.000000 cottontaildb_client-0.16.6/cottontaildb_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 09:49:05.000000 cottontaildb_client-0.16.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-29 09:49:13.183917 cottontaildb_client-0.16.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 09:49:05.000000 cottontaildb_client-0.16.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:49:13.183917 cottontaildb_client-0.16.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 09:49:05.000000 cottontaildb_client-0.16.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13085 2024-04-29 09:49:05.000000 cottontaildb_client-0.16.6/tests/test_cottontaildb_client.py
```

### Comparing `cottontaildb-client-0.14.2/LICENSE` & `cottontaildb_client-0.16.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cottontaildb-client-0.14.2/PKG-INFO` & `cottontaildb_client-0.16.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: cottontaildb-client
-Version: 0.14.2
+Version: 0.16.6
 Summary: A Cottontail DB gRPC client.
 Home-page: https://github.com/Spiess/cottontaildb-python-client
 Author: Florian Spiess
 Author-email: florian.spiess@unibas.ch
 Project-URL: Bug Tracker, https://github.com/Spiess/cottontaildb-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: grpcio
+Requires-Dist: grpcio-tools
 
 # Cottontail DB gRPC Python Client
 
 [![pypi](https://img.shields.io/pypi/v/cottontaildb-client.svg)](https://pypi.org/project/cottontaildb-client/)
 [![Python package workflow](https://github.com/Spiess/cottontaildb-python-client/actions/workflows/python-package.yml/badge.svg)](https://github.com/Spiess/cottontaildb-python-client/actions/workflows/python-package.yml)
 
 A Cottontail DB gRPC client for Python. Built with [Cottontail DB Proto](https://github.com/vitrivr/cottontaildb-proto)
@@ -57,23 +59,23 @@
         [Literal(stringData='test_null'), Literal()]
     ]
     client.insert_batch('example_schema', 'example_entity', columns, values)
 ```
 
 ## Developing
 
-To update the gRPC client, regenerate `cottontaildb_pb2.py` and `cottontaildb_pb2_grpc.py` from the proto definitions
-file in the [Cottontail DB Proto](https://github.com/vitrivr/cottontaildb-proto) repository.
+To update the gRPC client, regenerate `cottontaildb_pb2.py`, `cottontail_pb2.pyi`, and `cottontaildb_pb2_grpc.py` from the proto definitions
+file in the [Cottontail DB](https://github.com/vitrivr/cottontaildb) repository.
 
 The following is an approximate guide on how to do so from a terminal:
 
 ```bash
 # Get the latest version of the Cottontail DB proto (and download to cottontaildb_client directory)
-wget https://github.com/vitrivr/cottontaildb-proto/raw/master/src/main/protobuf/cottontail.proto -P ./cottontaildb_client/
+wget https://github.com/vitrivr/cottontaildb/raw/master/cottontaildb-client/src/main/protobuf/cottontail.proto -P ./cottontaildb_client/
 # Install necessary python packages
 pip install grpcio grpcio-tools
 # Generate the gRPC client
-python -m grpc_tools.protoc -I. --python_out=. --grpc_python_out=. ./cottontaildb_client/cottontail.proto
+python -m grpc_tools.protoc -I. --python_out=. --pyi_out=. --grpc_python_out=. ./cottontaildb_client/cottontail.proto
 ```
 
 It is important that the path to the `cottontail.proto` file reflects the location of the gRPC Python files, such that
 the imports can be generated correctly.
```

### Comparing `cottontaildb-client-0.14.2/README.md` & `cottontaildb_client-0.16.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -42,23 +42,23 @@
         [Literal(stringData='test_null'), Literal()]
     ]
     client.insert_batch('example_schema', 'example_entity', columns, values)
 ```
 
 ## Developing
 
-To update the gRPC client, regenerate `cottontaildb_pb2.py` and `cottontaildb_pb2_grpc.py` from the proto definitions
-file in the [Cottontail DB Proto](https://github.com/vitrivr/cottontaildb-proto) repository.
+To update the gRPC client, regenerate `cottontaildb_pb2.py`, `cottontail_pb2.pyi`, and `cottontaildb_pb2_grpc.py` from the proto definitions
+file in the [Cottontail DB](https://github.com/vitrivr/cottontaildb) repository.
 
 The following is an approximate guide on how to do so from a terminal:
 
 ```bash
 # Get the latest version of the Cottontail DB proto (and download to cottontaildb_client directory)
-wget https://github.com/vitrivr/cottontaildb-proto/raw/master/src/main/protobuf/cottontail.proto -P ./cottontaildb_client/
+wget https://github.com/vitrivr/cottontaildb/raw/master/cottontaildb-client/src/main/protobuf/cottontail.proto -P ./cottontaildb_client/
 # Install necessary python packages
 pip install grpcio grpcio-tools
 # Generate the gRPC client
-python -m grpc_tools.protoc -I. --python_out=. --grpc_python_out=. ./cottontaildb_client/cottontail.proto
+python -m grpc_tools.protoc -I. --python_out=. --pyi_out=. --grpc_python_out=. ./cottontaildb_client/cottontail.proto
 ```
 
 It is important that the path to the `cottontail.proto` file reflects the location of the gRPC Python files, such that
 the imports can be generated correctly.
```

### Comparing `cottontaildb-client-0.14.2/cottontaildb_client/cottontail_pb2_grpc.py` & `cottontaildb_client-0.16.6/cottontaildb_client/cottontail_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,24 @@
                 response_deserializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.FromString,
                 )
         self.EntityDetails = channel.unary_unary(
                 '/org.vitrivr.cottontail.grpc.DDL/EntityDetails',
                 request_serializer=cottontaildb__client_dot_cottontail__pb2.EntityDetailsMessage.SerializeToString,
                 response_deserializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.FromString,
                 )
+        self.EntityStatistics = channel.unary_unary(
+                '/org.vitrivr.cottontail.grpc.DDL/EntityStatistics',
+                request_serializer=cottontaildb__client_dot_cottontail__pb2.EntityDetailsMessage.SerializeToString,
+                response_deserializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.FromString,
+                )
+        self.IndexDetails = channel.unary_unary(
+                '/org.vitrivr.cottontail.grpc.DDL/IndexDetails',
+                request_serializer=cottontaildb__client_dot_cottontail__pb2.IndexDetailsMessage.SerializeToString,
+                response_deserializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.FromString,
+                )
         self.CreateEntity = channel.unary_unary(
                 '/org.vitrivr.cottontail.grpc.DDL/CreateEntity',
                 request_serializer=cottontaildb__client_dot_cottontail__pb2.CreateEntityMessage.SerializeToString,
                 response_deserializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.FromString,
                 )
         self.DropEntity = channel.unary_unary(
                 '/org.vitrivr.cottontail.grpc.DDL/DropEntity',
@@ -51,17 +61,17 @@
                 response_deserializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.FromString,
                 )
         self.TruncateEntity = channel.unary_unary(
                 '/org.vitrivr.cottontail.grpc.DDL/TruncateEntity',
                 request_serializer=cottontaildb__client_dot_cottontail__pb2.TruncateEntityMessage.SerializeToString,
                 response_deserializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.FromString,
                 )
-        self.OptimizeEntity = channel.unary_unary(
-                '/org.vitrivr.cottontail.grpc.DDL/OptimizeEntity',
-                request_serializer=cottontaildb__client_dot_cottontail__pb2.OptimizeEntityMessage.SerializeToString,
+        self.AnalyzeEntity = channel.unary_unary(
+                '/org.vitrivr.cottontail.grpc.DDL/AnalyzeEntity',
+                request_serializer=cottontaildb__client_dot_cottontail__pb2.AnalyzeEntityMessage.SerializeToString,
                 response_deserializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.FromString,
                 )
         self.CreateIndex = channel.unary_unary(
                 '/org.vitrivr.cottontail.grpc.DDL/CreateIndex',
                 request_serializer=cottontaildb__client_dot_cottontail__pb2.CreateIndexMessage.SerializeToString,
                 response_deserializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.FromString,
                 )
@@ -111,14 +121,28 @@
     def EntityDetails(self, request, context):
         """Returns details about the given entity. 
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def EntityStatistics(self, request, context):
+        """Returns details about the given column. 
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def IndexDetails(self, request, context):
+        """Returns details about the given index. 
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def CreateEntity(self, request, context):
         """* Creates a new entity. 
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -132,15 +156,15 @@
     def TruncateEntity(self, request, context):
         """* Truncates an existing entity. 
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def OptimizeEntity(self, request, context):
+    def AnalyzeEntity(self, request, context):
         """Optimizing and truncating entities. 
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CreateIndex(self, request, context):
@@ -188,14 +212,24 @@
                     response_serializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.SerializeToString,
             ),
             'EntityDetails': grpc.unary_unary_rpc_method_handler(
                     servicer.EntityDetails,
                     request_deserializer=cottontaildb__client_dot_cottontail__pb2.EntityDetailsMessage.FromString,
                     response_serializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.SerializeToString,
             ),
+            'EntityStatistics': grpc.unary_unary_rpc_method_handler(
+                    servicer.EntityStatistics,
+                    request_deserializer=cottontaildb__client_dot_cottontail__pb2.EntityDetailsMessage.FromString,
+                    response_serializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.SerializeToString,
+            ),
+            'IndexDetails': grpc.unary_unary_rpc_method_handler(
+                    servicer.IndexDetails,
+                    request_deserializer=cottontaildb__client_dot_cottontail__pb2.IndexDetailsMessage.FromString,
+                    response_serializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.SerializeToString,
+            ),
             'CreateEntity': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateEntity,
                     request_deserializer=cottontaildb__client_dot_cottontail__pb2.CreateEntityMessage.FromString,
                     response_serializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.SerializeToString,
             ),
             'DropEntity': grpc.unary_unary_rpc_method_handler(
                     servicer.DropEntity,
@@ -203,17 +237,17 @@
                     response_serializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.SerializeToString,
             ),
             'TruncateEntity': grpc.unary_unary_rpc_method_handler(
                     servicer.TruncateEntity,
                     request_deserializer=cottontaildb__client_dot_cottontail__pb2.TruncateEntityMessage.FromString,
                     response_serializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.SerializeToString,
             ),
-            'OptimizeEntity': grpc.unary_unary_rpc_method_handler(
-                    servicer.OptimizeEntity,
-                    request_deserializer=cottontaildb__client_dot_cottontail__pb2.OptimizeEntityMessage.FromString,
+            'AnalyzeEntity': grpc.unary_unary_rpc_method_handler(
+                    servicer.AnalyzeEntity,
+                    request_deserializer=cottontaildb__client_dot_cottontail__pb2.AnalyzeEntityMessage.FromString,
                     response_serializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.SerializeToString,
             ),
             'CreateIndex': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateIndex,
                     request_deserializer=cottontaildb__client_dot_cottontail__pb2.CreateIndexMessage.FromString,
                     response_serializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.SerializeToString,
             ),
@@ -319,14 +353,48 @@
         return grpc.experimental.unary_unary(request, target, '/org.vitrivr.cottontail.grpc.DDL/EntityDetails',
             cottontaildb__client_dot_cottontail__pb2.EntityDetailsMessage.SerializeToString,
             cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def EntityStatistics(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/org.vitrivr.cottontail.grpc.DDL/EntityStatistics',
+            cottontaildb__client_dot_cottontail__pb2.EntityDetailsMessage.SerializeToString,
+            cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def IndexDetails(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/org.vitrivr.cottontail.grpc.DDL/IndexDetails',
+            cottontaildb__client_dot_cottontail__pb2.IndexDetailsMessage.SerializeToString,
+            cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def CreateEntity(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -370,26 +438,26 @@
         return grpc.experimental.unary_unary(request, target, '/org.vitrivr.cottontail.grpc.DDL/TruncateEntity',
             cottontaildb__client_dot_cottontail__pb2.TruncateEntityMessage.SerializeToString,
             cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def OptimizeEntity(request,
+    def AnalyzeEntity(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/org.vitrivr.cottontail.grpc.DDL/OptimizeEntity',
-            cottontaildb__client_dot_cottontail__pb2.OptimizeEntityMessage.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/org.vitrivr.cottontail.grpc.DDL/AnalyzeEntity',
+            cottontaildb__client_dot_cottontail__pb2.AnalyzeEntityMessage.SerializeToString,
             cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def CreateIndex(request,
             target,
@@ -757,30 +825,30 @@
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Begin = channel.unary_unary(
                 '/org.vitrivr.cottontail.grpc.TXN/Begin',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=cottontaildb__client_dot_cottontail__pb2.Metadata.FromString,
+                request_serializer=cottontaildb__client_dot_cottontail__pb2.BeginTransaction.SerializeToString,
+                response_deserializer=cottontaildb__client_dot_cottontail__pb2.ResponseMetadata.FromString,
                 )
         self.Commit = channel.unary_unary(
                 '/org.vitrivr.cottontail.grpc.TXN/Commit',
-                request_serializer=cottontaildb__client_dot_cottontail__pb2.Metadata.SerializeToString,
+                request_serializer=cottontaildb__client_dot_cottontail__pb2.RequestMetadata.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.Rollback = channel.unary_unary(
                 '/org.vitrivr.cottontail.grpc.TXN/Rollback',
-                request_serializer=cottontaildb__client_dot_cottontail__pb2.Metadata.SerializeToString,
+                request_serializer=cottontaildb__client_dot_cottontail__pb2.RequestMetadata.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.Kill = channel.unary_unary(
                 '/org.vitrivr.cottontail.grpc.TXN/Kill',
-                request_serializer=cottontaildb__client_dot_cottontail__pb2.Metadata.SerializeToString,
+                request_serializer=cottontaildb__client_dot_cottontail__pb2.RequestMetadata.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.ListTransactions = channel.unary_stream(
                 '/org.vitrivr.cottontail.grpc.TXN/ListTransactions',
                 request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
                 response_deserializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.FromString,
                 )
@@ -839,30 +907,30 @@
         raise NotImplementedError('Method not implemented!')
 
 
 def add_TXNServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Begin': grpc.unary_unary_rpc_method_handler(
                     servicer.Begin,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=cottontaildb__client_dot_cottontail__pb2.Metadata.SerializeToString,
+                    request_deserializer=cottontaildb__client_dot_cottontail__pb2.BeginTransaction.FromString,
+                    response_serializer=cottontaildb__client_dot_cottontail__pb2.ResponseMetadata.SerializeToString,
             ),
             'Commit': grpc.unary_unary_rpc_method_handler(
                     servicer.Commit,
-                    request_deserializer=cottontaildb__client_dot_cottontail__pb2.Metadata.FromString,
+                    request_deserializer=cottontaildb__client_dot_cottontail__pb2.RequestMetadata.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'Rollback': grpc.unary_unary_rpc_method_handler(
                     servicer.Rollback,
-                    request_deserializer=cottontaildb__client_dot_cottontail__pb2.Metadata.FromString,
+                    request_deserializer=cottontaildb__client_dot_cottontail__pb2.RequestMetadata.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'Kill': grpc.unary_unary_rpc_method_handler(
                     servicer.Kill,
-                    request_deserializer=cottontaildb__client_dot_cottontail__pb2.Metadata.FromString,
+                    request_deserializer=cottontaildb__client_dot_cottontail__pb2.RequestMetadata.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'ListTransactions': grpc.unary_stream_rpc_method_handler(
                     servicer.ListTransactions,
                     request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                     response_serializer=cottontaildb__client_dot_cottontail__pb2.QueryResponseMessage.SerializeToString,
             ),
@@ -891,16 +959,16 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/org.vitrivr.cottontail.grpc.TXN/Begin',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            cottontaildb__client_dot_cottontail__pb2.Metadata.FromString,
+            cottontaildb__client_dot_cottontail__pb2.BeginTransaction.SerializeToString,
+            cottontaildb__client_dot_cottontail__pb2.ResponseMetadata.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Commit(request,
             target,
             options=(),
@@ -908,15 +976,15 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/org.vitrivr.cottontail.grpc.TXN/Commit',
-            cottontaildb__client_dot_cottontail__pb2.Metadata.SerializeToString,
+            cottontaildb__client_dot_cottontail__pb2.RequestMetadata.SerializeToString,
             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Rollback(request,
             target,
@@ -925,15 +993,15 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/org.vitrivr.cottontail.grpc.TXN/Rollback',
-            cottontaildb__client_dot_cottontail__pb2.Metadata.SerializeToString,
+            cottontaildb__client_dot_cottontail__pb2.RequestMetadata.SerializeToString,
             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Kill(request,
             target,
@@ -942,15 +1010,15 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/org.vitrivr.cottontail.grpc.TXN/Kill',
-            cottontaildb__client_dot_cottontail__pb2.Metadata.SerializeToString,
+            cottontaildb__client_dot_cottontail__pb2.RequestMetadata.SerializeToString,
             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ListTransactions(request,
             target,
```

### Comparing `cottontaildb-client-0.14.2/cottontaildb_client/cottontaildb_cli.py` & `cottontaildb_client-0.16.6/cottontaildb_client/cottontaildb_cli.py`

 * *Files identical despite different names*

### Comparing `cottontaildb-client-0.14.2/cottontaildb_client/cottontaildb_client.py` & `cottontaildb_client-0.16.6/cottontaildb_client/cottontaildb_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from datetime import datetime, timezone
+from typing import List
 
 import grpc
 from google.protobuf.empty_pb2 import Empty
-from typing import List
 
 from .cottontail_pb2 import SchemaName, CreateSchemaMessage, DropSchemaMessage, EntityName, ColumnDefinition, \
-    EntityDefinition, CreateEntityMessage, InsertMessage, ColumnName, Scan, From, Type, ListSchemaMessage, \
-    ListEntityMessage, EntityDetailsMessage, DropEntityMessage, TruncateEntityMessage, OptimizeEntityMessage, \
-    IndexName, IndexType, CreateIndexMessage, DropIndexMessage, RebuildIndexMessage, UpdateMessage, \
-    DeleteMessage, Literal, Vector, FloatVector, BatchInsertMessage, Metadata, QueryMessage, Query, Expression, \
-    FunctionName, Function, Projection, Order
+    CreateEntityMessage, InsertMessage, ColumnName, Scan, From, Type, ListSchemaMessage, ListEntityMessage, \
+    EntityDetailsMessage, DropEntityMessage, TruncateEntityMessage, IndexName, IndexType, CreateIndexMessage, \
+    DropIndexMessage, RebuildIndexMessage, UpdateMessage, DeleteMessage, Literal, Vector, FloatVector, \
+    BatchInsertMessage, RequestMetadata, QueryMessage, Query, AnalyzeEntityMessage, Expression, FunctionName, Function, \
+    Projection, Order
 from .cottontail_pb2_grpc import DDLStub, DMLStub, TXNStub, DQLStub
 
 
 class CottontailDBClient:
     def __init__(self, host, port, with_transaction=False):
         self._host = host
         self._port = port
@@ -48,31 +48,31 @@
         metadata = self._txn.Begin(Empty())
         self._tid = metadata.transactionId
 
     def commit_transaction(self):
         """Commits the current transaction."""
         if not self._transaction:
             raise Exception('No transaction running!')
-        self._txn.Commit(Metadata(transactionId=self._tid))
+        self._txn.Commit(RequestMetadata(transactionId=self._tid))
         self._tid = None
         self._transaction = False
 
     def abort_transaction(self):
         """Aborts the current transaction and rolls back work. Blocks if a query is ongoing."""
         if not self._transaction:
             raise Exception('No transaction running!')
-        self._txn.Rollback(Metadata(transactionId=self._tid))
+        self._txn.Rollback(RequestMetadata(transactionId=self._tid))
         self._tid = None
         self._transaction = False
 
     def kill_transaction(self):
         """Kills the current transaction and rolls back work."""
         if not self._transaction:
             raise Exception('No transaction running!')
-        self._txn.Kill(Metadata(transactionId=self._tid))
+        self._txn.Kill(RequestMetadata(transactionId=self._tid))
         self._tid = None
         self._transaction = False
 
     def list_transactions(self):
         """Lists all active transactions."""
         responses = [response for response in self._txn.ListTransactions(Empty())]
         # TODO: Parse into Python data structure
@@ -94,22 +94,22 @@
         @param exist_ok: if the client should first check if the schema already exists
         @return: query response if there was a schema create attempt or None if exist_ok and schema already exists
         """
         if exist_ok and schema in [s.split('.')[-1] for s in self.list_schemas()]:
             return
         schema_name = SchemaName(name=schema)
         response = self._ddl.CreateSchema(
-            CreateSchemaMessage(metadata=Metadata(transactionId=self._tid), schema=schema_name))
+            CreateSchemaMessage(metadata=RequestMetadata(transactionId=self._tid), schema=schema_name))
         return self._parse_query_response(response)
 
     def drop_schema(self, schema):
         """Drops the schema with the given name."""
         schema_name = SchemaName(name=schema)
         response = self._ddl.DropSchema(
-            DropSchemaMessage(metadata=Metadata(transactionId=self._tid), schema=schema_name))
+            DropSchemaMessage(metadata=RequestMetadata(transactionId=self._tid), schema=schema_name))
         return self._parse_query_response(response)
 
     def create_entity(self, schema, entity, columns, exist_ok=False):
         """
         Creates an entity in the given schema with the defined columns.
 
         Columns are defined by a list of column definitions, e.g.:
@@ -117,142 +117,144 @@
 
         @param schema: name of the entity's schema
         @param entity: entity name
         @param columns: list of ColumnDefinition objects defining the entity's columns
         @param exist_ok: if the client should first check if the entity already exists
         @return: query response if there was an entity create attempt or None if exist_ok and entity already exists
         """
-        if exist_ok and entity in [s.split('.')[-1] for s in self.list_entities(schema)]:
-            return
         schema_name = SchemaName(name=schema)
         entity_name = EntityName(schema=schema_name, name=entity)
-        entity_def = EntityDefinition(entity=entity_name, columns=columns)
         response = self._ddl.CreateEntity(
-            CreateEntityMessage(metadata=Metadata(transactionId=self._tid), definition=entity_def))
+            CreateEntityMessage(metadata=RequestMetadata(transactionId=self._tid), entity=entity_name, columns=columns,
+                                mayExist=exist_ok))
         return self._parse_query_response(response)
 
     def drop_entity(self, schema, entity, not_exist_ok=True):
         """Drops the given entity from the given schema."""
         if not_exist_ok and entity not in [s.split('.')[-1] for s in self.list_entities(schema)]:
             return
         schema_name = SchemaName(name=schema)
         entity_name = EntityName(schema=schema_name, name=entity)
         response = self._ddl.DropEntity(
-            DropEntityMessage(metadata=Metadata(transactionId=self._tid), entity=entity_name))
+            DropEntityMessage(metadata=RequestMetadata(transactionId=self._tid), entity=entity_name))
         return self._parse_query_response(response)
 
     def truncate_entity(self, schema, entity, not_exist_ok=True):
         """Truncates the specified entity."""
         if not_exist_ok and entity not in [s.split('.')[-1] for s in self.list_entities(schema)]:
             return
         schema_name = SchemaName(name=schema)
         entity_name = EntityName(schema=schema_name, name=entity)
         response = self._ddl.TruncateEntity(
-            TruncateEntityMessage(metadata=Metadata(transactionId=self._tid), entity=entity_name))
+            TruncateEntityMessage(metadata=RequestMetadata(transactionId=self._tid), entity=entity_name))
         return self._parse_query_response(response)
 
-    def optimize_entity(self, schema, entity):
+    def analyze_entity(self, schema, entity, async_=False):
         """Optimizes the specified entity."""
         schema_name = SchemaName(name=schema)
         entity_name = EntityName(schema=schema_name, name=entity)
-        response = self._ddl.OptimizeEntity(
-            OptimizeEntityMessage(metadata=Metadata(transactionId=self._tid), entity=entity_name))
+        kwargs = {
+            'async': async_
+        }
+        response = self._ddl.AnalyzeEntity(
+            AnalyzeEntityMessage(metadata=RequestMetadata(transactionId=self._tid), entity=entity_name, **kwargs))
         return self._parse_query_response(response)
 
-    def create_index(self, schema, entity, index, index_type: IndexType, columns: List[str], rebuild: bool = False):
+    def create_index(self, schema, entity, index, index_type: IndexType, columns: List[str]):
         """
         Creates an index on a column.
 
         @param schema: name of the index's schema
         @param entity: name of the index's entity
         @param index: index name
         @param index_type: type of index
         @param columns: columns to build index for
-        @param rebuild: TODO
         """
         schema_name = SchemaName(name=schema)
         entity_name = EntityName(schema=schema_name, name=entity)
         # TODO: map<string,string> params
         response = self._ddl.CreateIndex(
-            CreateIndexMessage(metadata=Metadata(transactionId=self._tid), entity=entity_name, type=index_type,
-                               indexName=index, columns=columns, rebuild=rebuild))
+            CreateIndexMessage(metadata=RequestMetadata(transactionId=self._tid), entity=entity_name, type=index_type,
+                               indexName=index, columns=columns))
         return self._parse_query_response(response)
 
     def drop_index(self, schema, entity, index):
         """
         Drops the specified index.
 
         @param schema: name of the index's schema
         @param entity: name of the index's entity
         @param index: index name
         """
         schema_name = SchemaName(name=schema)
         entity_name = EntityName(schema=schema_name, name=entity)
         index_name = IndexName(entity=entity_name, name=index)
-        response = self._ddl.DropIndex(DropIndexMessage(metadata=Metadata(transactionId=self._tid), index=index_name))
+        response = self._ddl.DropIndex(
+            DropIndexMessage(metadata=RequestMetadata(transactionId=self._tid), index=index_name))
         return self._parse_query_response(response)
 
     def rebuild_index(self, schema, entity, index):
         """
         Rebuilds the specified index.
 
         @param schema: name of the index's schema
         @param entity: name of the index's entity
         @param index: index name
         """
         schema_name = SchemaName(name=schema)
         entity_name = EntityName(schema=schema_name, name=entity)
         index_name = IndexName(entity=entity_name, name=index)
         response = self._ddl.RebuildIndex(
-            RebuildIndexMessage(metadata=Metadata(transactionId=self._tid), index=index_name))
+            RebuildIndexMessage(metadata=RequestMetadata(transactionId=self._tid), index=index_name))
         return self._parse_query_response(response)
 
     def list_schemas(self):
         """Lists all schemas in the database."""
         responses = [response for response in
-                     self._ddl.ListSchemas(ListSchemaMessage(metadata=Metadata(transactionId=self._tid)))]
+                     self._ddl.ListSchemas(ListSchemaMessage(metadata=RequestMetadata(transactionId=self._tid)))]
         tuples = [t.data[0].stringData for response in responses for t in response.tuples]
         return tuples
 
     def list_entities(self, schema):
         """
         Lists all entities of the specified schema
 
         @param schema: schema of which to list entities
         @return: list of entity names
         """
         schema_name = SchemaName(name=schema)
         responses = [response for response in
                      self._ddl.ListEntities(
-                         ListEntityMessage(metadata=Metadata(transactionId=self._tid), schema=schema_name))]
+                         ListEntityMessage(metadata=RequestMetadata(transactionId=self._tid), schema=schema_name))]
         tuples = [t.data[0].stringData for response in responses for t in response.tuples]
         return tuples
 
     def get_entity_details(self, schema, entity):
         """
         Retrieves details about an entity.
 
         @param schema: the entity's schema
         @param entity: entity name
         @return: dictionary containing entity details
         """
         schema_name = SchemaName(name=schema)
         entity_name = EntityName(schema=schema_name, name=entity)
         response = self._ddl.EntityDetails(
-            EntityDetailsMessage(metadata=Metadata(transactionId=self._tid), entity=entity_name))
+            EntityDetailsMessage(metadata=RequestMetadata(transactionId=self._tid), entity=entity_name))
         entity_data = response.tuples[0]
         data_names = [c.name.name for c in response.columns]
         name_index = data_names.index('dbo')
         class_index = data_names.index('class')
         type_index = data_names.index('type')
+        rows_index = data_names.index('rows')
         size_index = data_names.index('l_size')
         nullable_index = data_names.index('nullable')
         entity_details = {
             'name': entity_data.data[name_index].stringData,
-            'rows': entity_data.data[data_names.index('rows')].intData,
+            'rows': entity_data.data[rows_index].longData,
             'columns': [
                 {
                     'name': c.data[name_index].stringData,
                     'type': c.data[type_index].stringData,
                     'size': c.data[size_index].intData,
                     'nullable': c.data[nullable_index].booleanData
                 } for c in response.tuples if c.data[class_index].stringData == 'COLUMN'
@@ -262,15 +264,15 @@
                     'name': c.data[name_index].stringData,
                     'type': c.data[type_index].stringData
                 } for c in response.tuples if c.data[class_index].stringData == 'INDEX'
             ]
         }
 
         return entity_details
-    
+
     def sample_entity(self, schema, entity, limit=10, skip=0):
         """
         Retrieves a preview of the specified entity.
 
         @param schema: the entity's schema
         @param entity: entity name
         @param limit: number of rows to return
@@ -316,15 +318,15 @@
 
         kwargs = {
             'from': From(scan=Scan(entity=entity_name)),
             'columns': column_names,
             'inserts': inserts
         }
 
-        message = BatchInsertMessage(metadata=Metadata(transactionId=self._tid), **kwargs)
+        message = BatchInsertMessage(metadata=RequestMetadata(transactionId=self._tid), **kwargs)
 
         self._dml.InsertBatch(message)
 
     def update(self, schema, entity, where, updates):
         """
         Updates the rows in schema.entity selected through the where clause with the values from updates.
 
@@ -336,29 +338,31 @@
         schema_name = SchemaName(name=schema)
         entity_name = EntityName(schema=schema_name, name=entity)
         from_kwarg = {'from': From(scan=Scan(entity=entity_name))}
         updates_list = [UpdateMessage.UpdateElement(column=ColumnName(name=column), value=value)
                         for column, value in updates.items()]
         # TODO: Simplify where specification
         return self._dml.Update(
-            UpdateMessage(metadata=Metadata(transactionId=self._tid), **from_kwarg, where=where, updates=updates_list))
+            UpdateMessage(metadata=RequestMetadata(transactionId=self._tid), **from_kwarg, where=where,
+                          updates=updates_list))
 
     def delete(self, schema, entity, where):
         """
         Deletes the rows in schema.entity selected through the where clause.
 
         @param schema: the schema containing the entity to delete
         @param entity: the entity containing rows to delete
         @param where: where clause selecting rows to delete
         """
         schema_name = SchemaName(name=schema)
         entity_name = EntityName(schema=schema_name, name=entity)
         from_kwarg = {'from': From(scan=Scan(entity=entity_name))}
         # TODO: Simplify where specification
-        return self._dml.Delete(DeleteMessage(metadata=Metadata(transactionId=self._tid), **from_kwarg, where=where))
+        return self._dml.Delete(
+            DeleteMessage(metadata=RequestMetadata(transactionId=self._tid), **from_kwarg, where=where))
 
     # Data query
 
     def ping(self):
         """Sends a ping message to the endpoint. If method returns without exception endpoint is connected."""
         self._dql.Ping(Empty())
 
@@ -411,15 +415,15 @@
         @param skip: number of rows to skip
         @param from_: from clause, defaults to scan of the entity
         """
         schema_name = SchemaName(name=schema)
         entity_name = EntityName(schema=schema_name, name=entity)
         from_kwarg = {'from': from_ if from_ else From(scan=Scan(entity=entity_name))}
         query = Query(**from_kwarg, projection=projection, where=where, order=order, limit=limit, skip=skip)
-        responses = self._dql.Query(QueryMessage(metadata=Metadata(transactionId=self._tid), query=query))
+        responses = self._dql.Query(QueryMessage(metadata=RequestMetadata(transactionId=self._tid), query=query))
         return [r for response in responses for r in self._parse_query_response(response)]
 
     @staticmethod
     def _parse_query_response(response):
         data_names = [c.name.name for c in response.columns]
         return [
             {
@@ -466,15 +470,15 @@
 
     def _insert_helper(self, schema, entity, values):
         schema_name = SchemaName(name=schema)
         entity_name = EntityName(schema=schema_name, name=entity)
         from_kwarg = {'from': From(scan=Scan(entity=entity_name))}
         elements = [InsertMessage.InsertElement(column=ColumnName(name=column), value=value)
                     for column, value in values.items()]
-        return InsertMessage(metadata=Metadata(transactionId=self._tid), **from_kwarg, elements=elements)
+        return InsertMessage(metadata=RequestMetadata(transactionId=self._tid), **from_kwarg, elements=elements)
 
 
 def column_def(name: str, type_: Type, length: int = None, primary: bool = None, nullable: bool = None):
     """
     Creates a column definition.
 
     @param name: column name
@@ -495,8 +499,8 @@
     if nullable is not None:
         kwargs['nullable'] = nullable
 
     return ColumnDefinition(**kwargs)
 
 
 def float_vector(*elements):
-    return Literal(vectorData=Vector(floatVector=FloatVector(vector=elements)))
+    return Literal(vectorData=Vector(float=FloatVector(vector=elements)))
```

### Comparing `cottontaildb-client-0.14.2/cottontaildb_client.egg-info/PKG-INFO` & `cottontaildb_client-0.16.6/cottontaildb_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: cottontaildb-client
-Version: 0.14.2
+Version: 0.16.6
 Summary: A Cottontail DB gRPC client.
 Home-page: https://github.com/Spiess/cottontaildb-python-client
 Author: Florian Spiess
 Author-email: florian.spiess@unibas.ch
 Project-URL: Bug Tracker, https://github.com/Spiess/cottontaildb-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: grpcio
+Requires-Dist: grpcio-tools
 
 # Cottontail DB gRPC Python Client
 
 [![pypi](https://img.shields.io/pypi/v/cottontaildb-client.svg)](https://pypi.org/project/cottontaildb-client/)
 [![Python package workflow](https://github.com/Spiess/cottontaildb-python-client/actions/workflows/python-package.yml/badge.svg)](https://github.com/Spiess/cottontaildb-python-client/actions/workflows/python-package.yml)
 
 A Cottontail DB gRPC client for Python. Built with [Cottontail DB Proto](https://github.com/vitrivr/cottontaildb-proto)
@@ -57,23 +59,23 @@
         [Literal(stringData='test_null'), Literal()]
     ]
     client.insert_batch('example_schema', 'example_entity', columns, values)
 ```
 
 ## Developing
 
-To update the gRPC client, regenerate `cottontaildb_pb2.py` and `cottontaildb_pb2_grpc.py` from the proto definitions
-file in the [Cottontail DB Proto](https://github.com/vitrivr/cottontaildb-proto) repository.
+To update the gRPC client, regenerate `cottontaildb_pb2.py`, `cottontail_pb2.pyi`, and `cottontaildb_pb2_grpc.py` from the proto definitions
+file in the [Cottontail DB](https://github.com/vitrivr/cottontaildb) repository.
 
 The following is an approximate guide on how to do so from a terminal:
 
 ```bash
 # Get the latest version of the Cottontail DB proto (and download to cottontaildb_client directory)
-wget https://github.com/vitrivr/cottontaildb-proto/raw/master/src/main/protobuf/cottontail.proto -P ./cottontaildb_client/
+wget https://github.com/vitrivr/cottontaildb/raw/master/cottontaildb-client/src/main/protobuf/cottontail.proto -P ./cottontaildb_client/
 # Install necessary python packages
 pip install grpcio grpcio-tools
 # Generate the gRPC client
-python -m grpc_tools.protoc -I. --python_out=. --grpc_python_out=. ./cottontaildb_client/cottontail.proto
+python -m grpc_tools.protoc -I. --python_out=. --pyi_out=. --grpc_python_out=. ./cottontaildb_client/cottontail.proto
 ```
 
 It is important that the path to the `cottontail.proto` file reflects the location of the gRPC Python files, such that
 the imports can be generated correctly.
```

### Comparing `cottontaildb-client-0.14.2/cottontaildb_client.egg-info/SOURCES.txt` & `cottontaildb_client-0.16.6/cottontaildb_client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 cottontaildb_client/__init__.py
 cottontaildb_client/__main__.py
 cottontaildb_client/cottontail_pb2.py
+cottontaildb_client/cottontail_pb2.pyi
 cottontaildb_client/cottontail_pb2_grpc.py
 cottontaildb_client/cottontaildb_cli.py
 cottontaildb_client/cottontaildb_client.py
 cottontaildb_client.egg-info/PKG-INFO
 cottontaildb_client.egg-info/SOURCES.txt
 cottontaildb_client.egg-info/dependency_links.txt
 cottontaildb_client.egg-info/entry_points.txt
```

### Comparing `cottontaildb-client-0.14.2/setup.cfg` & `cottontaildb_client-0.16.6/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cottontaildb-client
-version = 0.14.2
+version = 0.16.6
 author = Florian Spiess
 author_email = florian.spiess@unibas.ch
 description = A Cottontail DB gRPC client.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Spiess/cottontaildb-python-client
 project_urls =
```

### Comparing `cottontaildb-client-0.14.2/tests/test_cottontaildb_client.py` & `cottontaildb_client-0.16.6/tests/test_cottontaildb_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from unittest import TestCase
 
 from grpc import RpcError
 
 from cottontaildb_client import CottontailDBClient, column_def, Type, Literal, float_vector
-from cottontaildb_client.cottontail_pb2 import Where, AtomicBooleanPredicate, ColumnName, AtomicBooleanOperand, \
-    ComparisonOperator, Expressions, Expression, Projection, IndexType, EntityName, SchemaName
+from cottontaildb_client.cottontail_pb2 import Where, ColumnName, Expression, Projection, IndexType, EntityName, \
+    SchemaName, Predicate
 
 DB_HOST = 'localhost'
 DB_PORT = 1865
 
 TEST_SCHEMA_STR = 'schema_test'
 TEST_ENTITY_STR = 'entity_test'
 TEST_VECTOR_ENTITY_STR = 'entity_test_vector'
@@ -79,46 +79,45 @@
         self.assert_in(TEST_ENTITY_STR, self.client.list_entities(TEST_SCHEMA_STR), 'entity was dropped')
 
     def test_insert(self):
         self._create_schema()
         self._create_entity()
         self._insert()
         details = self.client.get_entity_details(TEST_SCHEMA_STR, TEST_ENTITY_STR)
-        self.assertEqual(details['rows'], 1, 'unexpected number of rows in entity after insert')
+        self.assertEqual(1, details['rows'], 'unexpected number of rows in entity after insert')
 
     def test_vector_insert(self):
         self._create_schema()
         self._create_vector_entity()
         self._insert_vector()
         details = self.client.get_entity_details(TEST_SCHEMA_STR, TEST_VECTOR_ENTITY_STR)
         self.assertEqual(details['rows'], 1, 'unexpected number of rows in vector entity after insert')
-        print('success')
 
     def test_batch_insert(self):
         self._create_schema()
         self._create_entity()
         self._batch_insert()
         details = self.client.get_entity_details(TEST_SCHEMA_STR, TEST_ENTITY_STR)
-        self.assertEqual(details['rows'], 3, 'unexpected number of rows in entity after batch insert')
+        self.assertEqual(3, details['rows'], 'unexpected number of rows in entity after batch insert')
 
     def test_batch_insert_vectors(self):
         self._create_schema()
         self._create_vector_entity()
         self._batch_insert_vectors()
         details = self.client.get_entity_details(TEST_SCHEMA_STR, TEST_VECTOR_ENTITY_STR)
-        self.assertEqual(details['rows'], 3, 'unexpected number of rows in entity after batch insert')
+        self.assertEqual(3, details['rows'], 'unexpected number of rows in entity after batch insert')
 
     def test_query(self):
         self._create_schema()
         self._create_entity()
         self._batch_insert()
         query_key = 'test_1'
         query_result = self._query_value_with_key(query_key)
         self.assertEqual(len(query_result), 1, 'unexpected number of rows returned from query')
-    
+
     def test_sample_entity(self):
         self._create_schema()
         self._create_entity()
         self._batch_insert()
         sample = self.client.sample_entity(TEST_SCHEMA_STR, TEST_ENTITY_STR, limit=2)
         should = [{'id': 'test_1', 'value': 1}, {'id': 'test_2', 'value': 2}]
         self.assertEqual(sample, should, 'unexpected preview result')
@@ -129,32 +128,31 @@
         self._batch_insert_vectors()
         query = [0.1, 0.2, 0.4]
 
         results = self.client.nns(TEST_SCHEMA_STR, TEST_VECTOR_ENTITY_STR, query, vector_col='value')
         self.assertEqual(len(results), 3, 'unexpected number of rows returned from query')
         # test with limit
         results = self.client.nns(TEST_SCHEMA_STR, TEST_VECTOR_ENTITY_STR, query, vector_col='value', limit=1)
-        print(results)
         self.assertEqual(len(results), 1, 'unexpected number of rows returned from query')
 
     def test_update(self):
         self._create_schema()
         self._create_entity()
         self._insert()
         update_key = 'test_0'
         update_value = 5
         self._update_value_with_key(update_key, update_value)
         query_results = self._query_value_with_key(update_key)
         self.assertEqual(query_results[0][TEST_COLUMN_VALUE], update_value, 'value not correctly updated')
 
-    def test_optimize(self):
+    def test_analyze(self):
         self._create_schema()
         self._create_entity()
         self._batch_insert()
-        self.client.optimize_entity(TEST_SCHEMA_STR, TEST_ENTITY_STR)
+        self.client.analyze_entity(TEST_SCHEMA_STR, TEST_ENTITY_STR)
 
     def test_create_rebuild_drop_index(self):
         self._create_schema()
         self._create_entity()
         self._batch_insert()
         details = self.client.get_entity_details(TEST_SCHEMA_STR, TEST_ENTITY_STR)
         self.assertEqual(len(details['indexes']), 0, 'unexpected number of indexes in entity before index creation')
@@ -186,16 +184,18 @@
         details = self.client.get_entity_details(TEST_SCHEMA_STR, TEST_ENTITY_STR)
         self.assertEqual(details['rows'], 0, 'unexpected number of rows in entity after aborted insert')
 
     def test_delete(self):
         self._create_schema()
         self._create_entity()
         self._insert()
-        where = Where(atomic=AtomicBooleanPredicate(left=ColumnName(name=TEST_COLUMN_VALUE), right=AtomicBooleanOperand(
-            expressions=Expressions(expression=[Expression(literal=Literal(intData=0))])), op=ComparisonOperator.EQUAL))
+        where = Where(predicate=Predicate(
+            comparison=Predicate.Comparison(lexp=Expression(column=ColumnName(name=TEST_COLUMN_VALUE)),
+                                            operator=Predicate.Comparison.Operator.EQUAL,
+                                            rexp=Expression(literal=Literal(intData=0)))))
         self.client.delete(TEST_SCHEMA_STR, TEST_ENTITY_STR, where)
         details = self.client.get_entity_details(TEST_SCHEMA_STR, TEST_ENTITY_STR)
         self.assertEqual(details['rows'], 0, 'unexpected number of rows in entity after delete')
 
     def assert_in(self, name, names, message):
         """Shortcut to test if the name of a database object is contained in a list of fully qualified names."""
         self.assertIn(name, [n.split('.')[-1] for n in names], message)
@@ -213,15 +213,15 @@
             column_def(TEST_COLUMN_VALUE, Type.INTEGER, nullable=False)
         ]
         self.client.create_entity(TEST_SCHEMA_STR, TEST_ENTITY_STR, columns)
 
     def _create_vector_entity(self):
         columns = [
             column_def(TEST_COLUMN_ID, Type.STRING, nullable=False),
-            column_def(TEST_COLUMN_VALUE, Type.FLOAT_VEC, length=3, nullable=False)
+            column_def(TEST_COLUMN_VALUE, Type.FLOAT_VECTOR, length=3, nullable=False)
         ]
         self.client.create_entity(TEST_SCHEMA_STR, TEST_VECTOR_ENTITY_STR, columns)
 
     def _insert(self):
         values = {'id': Literal(stringData='test_0'), TEST_COLUMN_VALUE: Literal(intData=0)}
         self.client.insert(TEST_SCHEMA_STR, TEST_ENTITY_STR, values)
 
@@ -249,27 +249,23 @@
             [Literal(stringData='test_1'), float_vector(*one)],
             [Literal(stringData='test_2'), float_vector(*two)],
             [Literal(stringData='test_3'), float_vector(*three)]
         ]
         self.client.insert_batch(TEST_SCHEMA_STR, TEST_VECTOR_ENTITY_STR, columns, values)
 
     def _update_value_with_key(self, key, value):
-        where = Where(atomic=AtomicBooleanPredicate(
-            left=ColumnName(name=TEST_COLUMN_ID),
-            right=AtomicBooleanOperand(
-                expressions=Expressions(expression=[Expression(literal=Literal(stringData=key))])),
-            op=ComparisonOperator.EQUAL
-        ))
+        where = Where(predicate=Predicate(
+            comparison=Predicate.Comparison(lexp=Expression(column=ColumnName(name=TEST_COLUMN_ID)),
+                                            operator=Predicate.Comparison.Operator.EQUAL,
+                                            rexp=Expression(literal=Literal(stringData=key)))))
         updates = {TEST_COLUMN_VALUE: Expression(literal=Literal(intData=value))}
         self.client.update(TEST_SCHEMA_STR, TEST_ENTITY_STR, where, updates)
 
     def _query_value_with_key(self, key):
         expression = Expression(column=ColumnName(entity=TEST_ENTITY_NAME, name=TEST_COLUMN_VALUE))
         projection_element = Projection.ProjectionElement(expression=expression)
         projection = Projection(op=Projection.ProjectionOperation.SELECT, elements=[projection_element])
-        where = Where(atomic=AtomicBooleanPredicate(
-            left=ColumnName(name=TEST_COLUMN_ID),
-            right=AtomicBooleanOperand(
-                expressions=Expressions(expression=[Expression(literal=Literal(stringData=key))])),
-            op=ComparisonOperator.EQUAL
-        ))
+        where = Where(predicate=Predicate(
+            comparison=Predicate.Comparison(lexp=Expression(column=ColumnName(name=TEST_COLUMN_ID)),
+                                            operator=Predicate.Comparison.Operator.EQUAL,
+                                            rexp=Expression(literal=Literal(stringData=key)))))
         return self.client.query(TEST_SCHEMA_STR, TEST_ENTITY_STR, projection, where)
```

