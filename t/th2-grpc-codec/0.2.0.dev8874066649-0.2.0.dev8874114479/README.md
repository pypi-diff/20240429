# Comparing `tmp/th2_grpc_codec-0.2.0.dev8874066649.tar.gz` & `tmp/th2_grpc_codec-0.2.0.dev8874114479.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_codec-0.2.0.dev8874066649.tar", last modified: Mon Apr 29 06:09:35 2024, max compression
+gzip compressed data, was "dist/th2_grpc_codec-0.2.0.dev8874114479.tar", last modified: Mon Apr 29 06:14:36 2024, max compression
```

## Comparing `th2_grpc_codec-0.2.0.dev8874066649.tar` & `th2_grpc_codec-0.2.0.dev8874114479.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-29 06:08:48.000000 th2_grpc_codec-0.2.0.dev8874066649/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-29 06:08:48.000000 th2_grpc_codec-0.2.0.dev8874066649/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-29 06:08:48.000000 th2_grpc_codec-0.2.0.dev8874066649/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-29 06:08:48.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-29 06:09:19.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec_service.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:14:36.000000 th2_grpc_codec-0.2.0.dev8874114479/
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-29 06:14:36.000000 th2_grpc_codec-0.2.0.dev8874114479/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-29 06:13:46.000000 th2_grpc_codec-0.2.0.dev8874114479/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-29 06:13:46.000000 th2_grpc_codec-0.2.0.dev8874114479/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 06:14:36.000000 th2_grpc_codec-0.2.0.dev8874114479/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-29 06:13:46.000000 th2_grpc_codec-0.2.0.dev8874114479/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:14:36.000000 th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 06:14:36.000000 th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-29 06:13:46.000000 th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec/codec.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-29 06:14:36.000000 th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec/codec_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-29 06:14:36.000000 th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec/codec_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-29 06:14:36.000000 th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec/codec_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-29 06:14:20.000000 th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec/codec_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 06:14:36.000000 th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:14:36.000000 th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-29 06:14:36.000000 th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-29 06:14:36.000000 th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 06:14:36.000000 th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 06:14:36.000000 th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 06:14:36.000000 th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec.egg-info/top_level.txt
```

### Comparing `th2_grpc_codec-0.2.0.dev8874066649/PKG-INFO` & `th2_grpc_codec-0.2.0.dev8874114479/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_codec
-Version: 0.2.0.dev8874066649
+Version: 0.2.0.dev8874114479
 Summary: th2_grpc_codec
 Home-page: https://github.com/th2-net/th2-grpc-codec
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC codec library (0.2.0)
```

### Comparing `th2_grpc_codec-0.2.0.dev8874066649/README.md` & `th2_grpc_codec-0.2.0.dev8874114479/README.md`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.2.0.dev8874066649/setup.py` & `th2_grpc_codec-0.2.0.dev8874114479/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec.proto` & `th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec/codec.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec_pb2.py` & `th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec/codec_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec_pb2.pyi` & `th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec/codec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec_pb2_grpc.py` & `th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec/codec_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec.egg-info/PKG-INFO` & `th2_grpc_codec-0.2.0.dev8874114479/th2_grpc_codec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-codec
-Version: 0.2.0.dev8874066649
+Version: 0.2.0.dev8874114479
 Summary: th2_grpc_codec
 Home-page: https://github.com/th2-net/th2-grpc-codec
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC codec library (0.2.0)
```

