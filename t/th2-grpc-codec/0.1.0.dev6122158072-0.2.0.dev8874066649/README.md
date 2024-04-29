# Comparing `tmp/th2_grpc_codec-0.1.0.dev6122158072.tar.gz` & `tmp/th2_grpc_codec-0.2.0.dev8874066649.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_codec-0.1.0.dev6122158072.tar", last modified: Fri Sep  8 13:12:17 2023, max compression
+gzip compressed data, was "dist/th2_grpc_codec-0.2.0.dev8874066649.tar", last modified: Mon Apr 29 06:09:35 2024, max compression
```

## Comparing `th2_grpc_codec-0.1.0.dev6122158072.tar` & `th2_grpc_codec-0.2.0.dev8874066649.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:12:17.000000 th2_grpc_codec-0.1.0.dev6122158072/
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-09-08 13:12:17.000000 th2_grpc_codec-0.1.0.dev6122158072/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2023-09-08 13:11:10.000000 th2_grpc_codec-0.1.0.dev6122158072/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-09-08 13:11:11.000000 th2_grpc_codec-0.1.0.dev6122158072/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-08 13:12:17.000000 th2_grpc_codec-0.1.0.dev6122158072/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2023-09-08 13:11:10.000000 th2_grpc_codec-0.1.0.dev6122158072/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:12:17.000000 th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 13:12:16.000000 th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-08 13:11:10.000000 th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec/codec.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-09-08 13:12:16.000000 th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec/codec_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-09-08 13:12:16.000000 th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec/codec_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2023-09-08 13:12:16.000000 th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec/codec_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2023-09-08 13:11:53.000000 th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec/codec_service.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 13:12:16.000000 th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:12:17.000000 th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-09-08 13:12:16.000000 th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-09-08 13:12:17.000000 th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 13:12:16.000000 th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-09-08 13:12:16.000000 th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-08 13:12:16.000000 th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-29 06:08:48.000000 th2_grpc_codec-0.2.0.dev8874066649/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-29 06:08:48.000000 th2_grpc_codec-0.2.0.dev8874066649/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-29 06:08:48.000000 th2_grpc_codec-0.2.0.dev8874066649/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-29 06:08:48.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-29 06:09:19.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 06:09:35.000000 th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec.egg-info/top_level.txt
```

### Comparing `th2_grpc_codec-0.1.0.dev6122158072/PKG-INFO` & `th2_grpc_codec-0.2.0.dev8874066649/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: th2_grpc_codec
-Version: 0.1.0.dev6122158072
+Version: 0.2.0.dev8874066649
 Summary: th2_grpc_codec
 Home-page: https://github.com/th2-net/th2-grpc-codec
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
-Description: # th2 gRPC codec library (0.1.0)
+Description: # th2 gRPC codec library (0.2.0)
         
         This library contains proto messages and `Codec` service with RPC methods that are used in [th2 codec](https://github.com/th2-net/th2-codec "th2-codec"). See [codec.proto](src/main/proto/th2_grpc_codec/codec.proto "codec.proto") file for details. <br>
         Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to the specified repositories.
         
         ## How to maintain a project
         1. Perform the necessary changes.
         2. Update the package version of Java in `gradle.properties` file.
@@ -42,22 +42,28 @@
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
             `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
+        ### 0.2.0
+        
+        + Migrated to th2 gradle plugin: `0.0.6` based on bom: `4.6.1`
+        + Updated grpc-common: `4.5.0-dev`
+        
         ### 0.1.0
         
         + Updated grpc-common 4.3.0
         
         ### 0.0.2
         
         + Added 'encode' method
         + Updated serviceGeneratorVersion and grpcCommonVersion to support gRPC pins filters.
         
         ### 0.0.1
         
         + 'decode' method
+        
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `th2_grpc_codec-0.1.0.dev6122158072/README.md` & `th2_grpc_codec-0.2.0.dev8874066649/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# th2 gRPC codec library (0.1.0)
+# th2 gRPC codec library (0.2.0)
 
 This library contains proto messages and `Codec` service with RPC methods that are used in [th2 codec](https://github.com/th2-net/th2-codec "th2-codec"). See [codec.proto](src/main/proto/th2_grpc_codec/codec.proto "codec.proto") file for details. <br>
 Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to the specified repositories.
 
 ## How to maintain a project
 1. Perform the necessary changes.
 2. Update the package version of Java in `gradle.properties` file.
@@ -34,19 +34,24 @@
     python setup.py sdist
     twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
     ```
     `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
 
 ## Release notes
 
+### 0.2.0
+
++ Migrated to th2 gradle plugin: `0.0.6` based on bom: `4.6.1`
++ Updated grpc-common: `4.5.0-dev`
+
 ### 0.1.0
 
 + Updated grpc-common 4.3.0
 
 ### 0.0.2
 
 + Added 'encode' method
 + Updated serviceGeneratorVersion and grpcCommonVersion to support gRPC pins filters.
 
 ### 0.0.1
 
-+ 'decode' method
++ 'decode' method
```

### Comparing `th2_grpc_codec-0.1.0.dev6122158072/setup.py` & `th2_grpc_codec-0.2.0.dev8874066649/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright 2020-2023 Exactpro (Exactpro Systems Limited)
+#   Copyright 2020-2024 Exactpro (Exactpro Systems Limited)
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -116,15 +116,15 @@
     long_description_content_type='text/markdown',
     author='TH2-devs',
     author_email='th2-devs@exactprosystems.com',
     url='https://github.com/th2-net/th2-grpc-codec',
     license='Apache License 2.0',
     python_requires='>=3.7',
     install_requires=[
-        'th2-grpc-common==4.3.0.dev0',
+        'th2-grpc-common==4.5.0rc1',
         'mypy-protobuf==3.4'
     ],
     packages=packages,
     package_data=package_data,
     cmdclass={
         'generate': ProtoGenerator,
         'sdist': CustomDist
```

### Comparing `th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec/codec.proto` & `th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec/codec_pb2.py` & `th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec/codec_pb2.pyi` & `th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec/codec_pb2_grpc.py` & `th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec/codec_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_codec-0.1.0.dev6122158072/th2_grpc_codec.egg-info/PKG-INFO` & `th2_grpc_codec-0.2.0.dev8874066649/th2_grpc_codec.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: th2-grpc-codec
-Version: 0.1.0.dev6122158072
+Version: 0.2.0.dev8874066649
 Summary: th2_grpc_codec
 Home-page: https://github.com/th2-net/th2-grpc-codec
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
-Description: # th2 gRPC codec library (0.1.0)
+Description: # th2 gRPC codec library (0.2.0)
         
         This library contains proto messages and `Codec` service with RPC methods that are used in [th2 codec](https://github.com/th2-net/th2-codec "th2-codec"). See [codec.proto](src/main/proto/th2_grpc_codec/codec.proto "codec.proto") file for details. <br>
         Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to the specified repositories.
         
         ## How to maintain a project
         1. Perform the necessary changes.
         2. Update the package version of Java in `gradle.properties` file.
@@ -42,22 +42,28 @@
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
             `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
+        ### 0.2.0
+        
+        + Migrated to th2 gradle plugin: `0.0.6` based on bom: `4.6.1`
+        + Updated grpc-common: `4.5.0-dev`
+        
         ### 0.1.0
         
         + Updated grpc-common 4.3.0
         
         ### 0.0.2
         
         + Added 'encode' method
         + Updated serviceGeneratorVersion and grpcCommonVersion to support gRPC pins filters.
         
         ### 0.0.1
         
         + 'decode' method
+        
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

