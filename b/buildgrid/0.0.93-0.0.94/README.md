# Comparing `tmp/buildgrid-0.0.93.tar.gz` & `tmp/buildgrid-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildgrid-0.0.93.tar", last modified: Fri Apr 26 14:31:28 2024, max compression
+gzip compressed data, was "buildgrid-0.0.94.tar", last modified: Mon Apr 29 15:22:12 2024, max compression
```

## Comparing `buildgrid-0.0.93.tar` & `buildgrid-0.0.94.tar`

### file list

```diff
@@ -1,498 +1,498 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.819027 buildgrid-0.0.93/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-26 14:31:00.000000 buildgrid-0.0.93/BuildGrid.doap
--rw-rw-rw-   0 root         (0) root         (0)     9648 2024-04-26 14:31:00.000000 buildgrid-0.0.93/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    11338 2024-04-26 14:31:00.000000 buildgrid-0.0.93/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      500 2024-04-26 14:31:00.000000 buildgrid-0.0.93/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6931 2024-04-26 14:31:28.819027 buildgrid-0.0.93/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2868 2024-04-26 14:31:00.000000 buildgrid-0.0.93/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.713609 buildgrid-0.0.93/buildgrid/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.715443 buildgrid-0.0.93/buildgrid/_app/
--rw-rw-rw-   0 root         (0) root         (0)      621 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5661 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.718193 buildgrid-0.0.93/buildgrid/_app/commands/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6755 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_actioncache.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_browser_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     3170 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_capabilities.py
--rw-rw-rw-   0 root         (0) root         (0)    10608 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_cas.py
--rw-rw-rw-   0 root         (0) root         (0)     8817 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)    12570 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     2840 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_janitor.py
--rw-rw-rw-   0 root         (0) root         (0)     4842 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_logstream.py
--rw-rw-rw-   0 root         (0) root         (0)    11215 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_operation.py
--rw-rw-rw-   0 root         (0) root         (0)     8166 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_server.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/rpc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.719109 buildgrid-0.0.93/buildgrid/_app/settings/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   110917 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     8691 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/reference.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.719109 buildgrid-0.0.93/buildgrid/_app/settings/schemas/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.720026 buildgrid-0.0.93/buildgrid/_app/settings/schemas/caches/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/caches/lru-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/caches/mirrored-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      676 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/caches/with-cache.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.720943 buildgrid-0.0.93/buildgrid/_app/settings/schemas/clients/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/clients/asset-client.yaml
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2785 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.720943 buildgrid-0.0.93/buildgrid/_app/settings/schemas/connections/
--rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/connections/redis.yaml
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/connections/sql.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.720943 buildgrid-0.0.93/buildgrid/_app/settings/schemas/misc/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/misc/channel.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.721859 buildgrid-0.0.93/buildgrid/_app/settings/schemas/scheduler/
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/scheduler/memory.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3907 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/scheduler/sql.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.723693 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      971 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/bots.yaml
--rw-rw-rw-   0 root         (0) root         (0)      343 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/bytestream.yaml
--rw-rw-rw-   0 root         (0) root         (0)      273 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/cas.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1557 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/execution.yaml
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/platform-queues.yml
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/s3-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/write-once-action-cache.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.726443 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/disk.yaml
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/lru.yaml
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/operations_sql_storage.yaml
--rw-rw-rw-   0 root         (0) root         (0)      207 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/redis-index.yaml
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/redis.yaml
--rw-rw-rw-   0 root         (0) root         (0)      601 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/remote.yaml
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/replicated.yaml
--rw-rw-rw-   0 root         (0) root         (0)      592 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/s3.yaml
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/sharded.yaml
--rw-rw-rw-   0 root         (0) root         (0)      530 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/sql-index.yaml
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/sql.yaml
--rw-rw-rw-   0 root         (0) root         (0)      281 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/with-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4776 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_enums.py
--rw-rw-rw-   0 root         (0) root         (0)     8802 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.726443 buildgrid-0.0.93/buildgrid/_protos/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.726443 buildgrid-0.0.93/buildgrid/_protos/build/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.727359 buildgrid-0.0.93/buildgrid/_protos/build/bazel/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.727359 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.727359 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 14:31:01.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.730109 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7795 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    27103 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    16783 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    15404 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    16783 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)    15550 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.730109 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.731943 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30140 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)   136470 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    59894 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    47588 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    59894 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)    47884 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.731943 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.733776 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2066 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3176 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    12298 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7788 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    12298 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7844 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.735609 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1484 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     2068 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.736526 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 14:31:01.000000 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1944 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4156 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.736526 buildgrid-0.0.93/buildgrid/_protos/buildgrid/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.741109 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3156 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    10940 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3824 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     9955 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2881 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2872 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2872 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.742026 buildgrid-0.0.93/buildgrid/_protos/google/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.746610 buildgrid-0.0.93/buildgrid/_protos/google/api/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1622 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1926 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2291 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18246 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.748443 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3246 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     7478 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10732 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     8880 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10732 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     8996 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.748443 buildgrid-0.0.93/buildgrid/_protos/google/devtools/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.749359 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.753943 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5933 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18014 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2545 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     5408 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6758 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    10427 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     5547 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.753943 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.759443 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7859 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    23457 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    11879 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7140 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    11879 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7256 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6133 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    21890 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5337 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     9321 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     7651 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     7651 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     4498 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2751 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    11299 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.762193 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5084 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     7984 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10950 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7133 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10950 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7279 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.766776 buildgrid-0.0.93/buildgrid/_protos/google/rpc/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    13407 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4774 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18695 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1573 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4889 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1358 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_types.py
--rw-rw-rw-   0 root         (0) root         (0)      604 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.767693 buildgrid-0.0.93/buildgrid/browser/
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/browser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4469 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/browser/app.py
--rw-rw-rw-   0 root         (0) root         (0)    34436 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/browser/rest_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2277 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/browser/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.767693 buildgrid-0.0.93/buildgrid/cleanup/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/cleanup/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9520 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/cleanup/cleanup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.768610 buildgrid-0.0.93/buildgrid/cleanup/janitor/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/cleanup/janitor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1745 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/cleanup/janitor/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3318 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/cleanup/janitor/index.py
--rw-rw-rw-   0 root         (0) root         (0)     4565 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/cleanup/janitor/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     1403 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/cleanup/janitor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.771360 buildgrid-0.0.93/buildgrid/client/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5099 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/actioncache.py
--rw-rw-rw-   0 root         (0) root         (0)     4361 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/asset.py
--rw-rw-rw-   0 root         (0) root         (0)     1631 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/auth_token_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     5113 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/authentication.py
--rwxrwxrwx   0 root         (0) root         (0)     1650 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/capabilities.py
--rw-rw-rw-   0 root         (0) root         (0)    41408 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/cas.py
--rw-rw-rw-   0 root         (0) root         (0)    13926 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/channel.py
--rw-rw-rw-   0 root         (0) root         (0)     4437 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/interceptors.py
--rw-rw-rw-   0 root         (0) root         (0)     2012 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/logstream.py
--rw-rw-rw-   0 root         (0) root         (0)     3410 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/retrier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.775026 buildgrid-0.0.93/buildgrid/server/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.775943 buildgrid-0.0.93/buildgrid/server/actioncache/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.777776 buildgrid-0.0.93/buildgrid/server/actioncache/caches/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5564 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/action_cache_abc.py
--rw-rw-rw-   0 root         (0) root         (0)     5593 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4197 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/mirrored_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     6534 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/redis_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     6573 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/remote_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    11662 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/s3_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4686 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/with_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3341 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/write_once_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3623 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     4045 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.778693 buildgrid-0.0.93/buildgrid/server/auth/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2363 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/auth/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1905 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/auth/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/auth/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/auth/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.779610 buildgrid-0.0.93/buildgrid/server/bots/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/bots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11154 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/bots/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     7343 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/bots/job_assigner.py
--rw-rw-rw-   0 root         (0) root         (0)     5647 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/bots/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.780526 buildgrid-0.0.93/buildgrid/server/build_events/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/build_events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6045 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/build_events/service.py
--rw-rw-rw-   0 root         (0) root         (0)     7213 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/build_events/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.781443 buildgrid-0.0.93/buildgrid/server/capabilities/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/capabilities/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7113 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/capabilities/instance.py
--rwxrwxrwx   0 root         (0) root         (0)     3342 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/capabilities/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.781443 buildgrid-0.0.93/buildgrid/server/cas/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21869 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/instance.py
--rw-rw-rw-   0 root         (0) root         (0)    11124 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.785110 buildgrid-0.0.93/buildgrid/server/cas/storage/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3702 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.786027 buildgrid-0.0.93/buildgrid/server/cas/storage/index/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/index/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3335 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/index/index_abc.py
--rw-rw-rw-   0 root         (0) root         (0)    13464 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/index/redis.py
--rw-rw-rw-   0 root         (0) root         (0)    38426 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.786943 buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql_dialect_delegates/
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql_dialect_delegates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2136 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py
--rw-rw-rw-   0 root         (0) root         (0)     2120 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py
--rw-rw-rw-   0 root         (0) root         (0)     4436 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/lru_memory_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     5330 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/redis.py
--rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/remote.py
--rw-rw-rw-   0 root         (0) root         (0)    11295 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/replicated.py
--rw-rw-rw-   0 root         (0) root         (0)    14426 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     6002 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/sharded.py
--rw-rw-rw-   0 root         (0) root         (0)     6985 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/size_differentiated.py
--rw-rw-rw-   0 root         (0) root         (0)     9519 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/sql.py
--rw-rw-rw-   0 root         (0) root         (0)     8154 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/storage_abc.py
--rw-rw-rw-   0 root         (0) root         (0)     7796 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/with_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3029 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/context.py
--rw-rw-rw-   0 root         (0) root         (0)     2194 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.787860 buildgrid-0.0.93/buildgrid/server/execution/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/execution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9599 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/execution/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     7517 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/execution/service.py
--rw-rw-rw-   0 root         (0) root         (0)     3813 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/job_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    18121 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/metrics_names.py
--rw-rw-rw-   0 root         (0) root         (0)    14482 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/metrics_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    19548 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.787860 buildgrid-0.0.93/buildgrid/server/operations/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.789693 buildgrid-0.0.93/buildgrid/server/operations/filtering/
--rw-rw-rw-   0 root         (0) root         (0)      813 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/filtering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/filtering/filter.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/filtering/filter_grammar.lark
--rw-rw-rw-   0 root         (0) root         (0)     5769 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/filtering/interpreter.py
--rw-rw-rw-   0 root         (0) root         (0)     2510 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/filtering/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4594 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/filtering/sanitizer.py
--rw-rw-rw-   0 root         (0) root         (0)     4802 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     6034 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.789693 buildgrid-0.0.93/buildgrid/server/persistence/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.790610 buildgrid-0.0.93/buildgrid/server/persistence/sql/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.791526 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/README
--rw-rw-rw-   0 root         (0) root         (0)     2919 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/env.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.797026 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/
--rw-rw-rw-   0 root         (0) root         (0)     1127 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)     1718 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py
--rw-rw-rw-   0 root         (0) root         (0)     1463 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py
--rw-rw-rw-   0 root         (0) root         (0)     2422 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py
--rw-rw-rw-   0 root         (0) root         (0)     1269 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py
--rw-rw-rw-   0 root         (0) root         (0)     1581 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1793 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py
--rw-rw-rw-   0 root         (0) root         (0)     2343 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1191 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1418 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py
--rw-rw-rw-   0 root         (0) root         (0)     4625 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py
--rw-rw-rw-   0 root         (0) root         (0)     2072 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py
--rw-rw-rw-   0 root         (0) root         (0)    79385 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/impl.py
--rw-rw-rw-   0 root         (0) root         (0)     8915 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6206 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/notifier.py
--rw-rw-rw-   0 root         (0) root         (0)    10298 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.797026 buildgrid-0.0.93/buildgrid/server/redis/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/redis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6197 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/redis/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4739 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/request_metadata_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.797943 buildgrid-0.0.93/buildgrid/server/s3/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18695 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/s3/s3utils.py
--rw-rw-rw-   0 root         (0) root         (0)    30687 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/server.py
--rw-rw-rw-   0 root         (0) root         (0)     6126 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/servicer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.798860 buildgrid-0.0.93/buildgrid/server/sql/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/sql/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22206 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/sql/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     6225 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/sql/sqlutils.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/threading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.799777 buildgrid-0.0.93/buildgrid/server/utils/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4484 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/utils/async_lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/utils/context.py
--rw-rw-rw-   0 root         (0) root         (0)    10885 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/utils/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     5450 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/settings.py
--rw-rw-rw-   0 root         (0) root         (0)    12244 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.811693 buildgrid-0.0.93/buildgrid.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6931 2024-04-26 14:31:28.000000 buildgrid-0.0.93/buildgrid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21169 2024-04-26 14:31:28.000000 buildgrid-0.0.93/buildgrid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 14:31:28.000000 buildgrid-0.0.93/buildgrid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-26 14:31:28.000000 buildgrid-0.0.93/buildgrid.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1213 2024-04-26 14:31:28.000000 buildgrid-0.0.93/buildgrid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-26 14:31:28.000000 buildgrid-0.0.93/buildgrid.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.709026 buildgrid-0.0.93/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.803443 buildgrid-0.0.93/data/config/
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/all-in-one.yml
--rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/artifacts.yml
--rwxrwxrwx   0 root         (0) root         (0)     1351 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/basic-with-disk.yml
--rw-rw-rw-   0 root         (0) root         (0)     1159 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/bots-interface.yml
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/cache.yml
--rw-rw-rw-   0 root         (0) root         (0)     1302 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/controller.yml
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/default.yml
--rw-rw-rw-   0 root         (0) root         (0)      832 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/index-sqlite-no-execution.yml
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/index-sqlite.yml
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/logstream.yml
--rw-rw-rw-   0 root         (0) root         (0)     1239 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/monitoring-controller.yml
--rw-rw-rw-   0 root         (0) root         (0)     1143 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/multi-layer-storage.yml
--rw-rw-rw-   0 root         (0) root         (0)     1474 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/redis-cache.yml
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/s3-indexed-cas.yml
--rw-rw-rw-   0 root         (0) root         (0)     1270 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/storage-redis.yml
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/storage-s3.yml
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/storage.yml
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/with-metering.yml
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/with-pgbouncer.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.803443 buildgrid-0.0.93/docs/
--rw-rw-rw-   0 root         (0) root         (0)      610 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.804360 buildgrid-0.0.93/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.806193 buildgrid-0.0.93/docs/source/data/
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/data/basic-disk-cas.yml
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/data/bazel-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      490 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/data/buildstream-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      446 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/data/cas-and-ac.yml
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/data/cas-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/data/execution-and-bots.yml
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/data/sqlite-index-cas-only.yml
--rw-rw-rw-   0 root         (0) root         (0)     1425 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5436 2024-04-26 14:31:01.000000 buildgrid-0.0.93/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-26 14:31:28.819943 buildgrid-0.0.93/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      643 2024-04-26 14:31:01.000000 buildgrid-0.0.93/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.808943 buildgrid-0.0.93/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.709943 buildgrid-0.0.93/tests/auth/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.811693 buildgrid-0.0.93/tests/auth/data/
--rw-rw-rw-   0 root         (0) root         (0)      733 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/auth.yaml
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwks-valid.json
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-hs256-conflicting.secret
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-hs256-expired.token
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-hs256-matching.secret
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-hs256-unbounded.token
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-hs256-valid.token
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-rs256-conflicting.pub.key
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-rs256-expired.token
--rw-rw-rw-   0 root         (0) root         (0)      559 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-rs256-jwk-encrypted.token
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-rs256-matching.priv.key
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-rs256-matching.pub.key
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-rs256-unbounded.token
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-rs256-valid.token
--rw-rw-rw-   0 root         (0) root         (0)     3829 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_async_lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    15407 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_execution_instance.py
--rw-rw-rw-   0 root         (0) root         (0)     2199 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_job_assigner.py
--rw-rw-rw-   0 root         (0) root         (0)    12358 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_metrics_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3447 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_mirrored_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_multithreaded_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_request_metadata_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    32384 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)    10567 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.272567 buildgrid-0.0.94/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-29 15:21:45.000000 buildgrid-0.0.94/BuildGrid.doap
+-rw-rw-rw-   0 root         (0) root         (0)     9648 2024-04-29 15:21:45.000000 buildgrid-0.0.94/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11338 2024-04-29 15:21:45.000000 buildgrid-0.0.94/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      500 2024-04-29 15:21:45.000000 buildgrid-0.0.94/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6931 2024-04-29 15:22:12.272567 buildgrid-0.0.94/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2024-04-29 15:21:45.000000 buildgrid-0.0.94/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.162566 buildgrid-0.0.94/buildgrid/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.164566 buildgrid-0.0.94/buildgrid/_app/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5661 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.167566 buildgrid-0.0.94/buildgrid/_app/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6755 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_actioncache.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_browser_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     3170 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    10608 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_cas.py
+-rw-rw-rw-   0 root         (0) root         (0)     8817 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)    12570 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2840 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_janitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4842 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_logstream.py
+-rw-rw-rw-   0 root         (0) root         (0)    11215 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_operation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8166 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_server.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/rpc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.168566 buildgrid-0.0.94/buildgrid/_app/settings/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   110917 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     8691 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/reference.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.168566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.169566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/caches/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/caches/lru-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/caches/mirrored-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      676 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/caches/with-cache.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.170566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/clients/asset-client.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.170566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/connections/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/connections/redis.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/connections/sql.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.171566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/misc/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/misc/channel.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.171566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/scheduler/memory.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3907 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/scheduler/sql.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.173566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      971 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/bots.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      343 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/bytestream.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/cas.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/execution.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/platform-queues.yml
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/s3-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/write-once-action-cache.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.177566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/disk.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/lru.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/operations_sql_storage.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      207 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/redis-index.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/redis.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      601 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/remote.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/replicated.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      592 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/s3.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/sharded.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      530 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/sql-index.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/sql.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      281 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/with-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4776 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     8802 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.177566 buildgrid-0.0.94/buildgrid/_protos/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.177566 buildgrid-0.0.94/buildgrid/_protos/build/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.177566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.178566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.178566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.180566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7795 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    27103 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    16783 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)    15404 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    16783 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)    15550 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.180566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.182566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30140 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)   136470 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    59894 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)    47588 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    59894 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)    47884 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.183566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.185566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2066 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3176 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    12298 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7788 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    12298 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7844 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.186566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.188566 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1944 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4156 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.188566 buildgrid-0.0.94/buildgrid/_protos/buildgrid/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.193566 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3156 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10940 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3824 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     9955 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2881 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2872 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2872 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.193566 buildgrid-0.0.94/buildgrid/_protos/google/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.199566 buildgrid-0.0.94/buildgrid/_protos/google/api/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18246 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.201566 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3246 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7478 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10732 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     8880 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10732 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     8996 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.201566 buildgrid-0.0.94/buildgrid/_protos/google/devtools/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.201566 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.206566 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5933 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18014 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5408 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     6758 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10427 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     5547 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.206566 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.212566 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7859 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    23457 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    11879 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7140 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    11879 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7256 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     6133 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    21890 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5337 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     9321 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     4498 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    11299 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.214566 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5084 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7984 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10950 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7133 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10950 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7279 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.218567 buildgrid-0.0.94/buildgrid/_protos/google/rpc/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    13407 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4774 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18695 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1573 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4889 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.219566 buildgrid-0.0.94/buildgrid/browser/
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/browser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4469 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/browser/app.py
+-rw-rw-rw-   0 root         (0) root         (0)    34436 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/browser/rest_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/browser/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.220566 buildgrid-0.0.94/buildgrid/cleanup/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/cleanup/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10716 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/cleanup/cleanup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.221567 buildgrid-0.0.94/buildgrid/cleanup/janitor/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/cleanup/janitor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/cleanup/janitor/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3318 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/cleanup/janitor/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     4565 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/cleanup/janitor/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/cleanup/janitor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.224567 buildgrid-0.0.94/buildgrid/client/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5099 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/actioncache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4361 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/auth_token_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/authentication.py
+-rwxrwxrwx   0 root         (0) root         (0)     1650 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    41408 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/cas.py
+-rw-rw-rw-   0 root         (0) root         (0)    13926 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/channel.py
+-rw-rw-rw-   0 root         (0) root         (0)     4437 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/interceptors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/logstream.py
+-rw-rw-rw-   0 root         (0) root         (0)     3410 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/retrier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.227567 buildgrid-0.0.94/buildgrid/server/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.227567 buildgrid-0.0.94/buildgrid/server/actioncache/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.230567 buildgrid-0.0.94/buildgrid/server/actioncache/caches/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5564 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/action_cache_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5593 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4197 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/mirrored_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     6534 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/redis_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     6573 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/remote_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    11662 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/s3_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/with_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/write_once_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3623 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.231567 buildgrid-0.0.94/buildgrid/server/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2363 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/auth/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/auth/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/auth/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/auth/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.231567 buildgrid-0.0.94/buildgrid/server/bots/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/bots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11156 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/bots/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     7343 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/bots/job_assigner.py
+-rw-rw-rw-   0 root         (0) root         (0)     5647 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/bots/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.232566 buildgrid-0.0.94/buildgrid/server/build_events/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/build_events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6045 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/build_events/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7213 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/build_events/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.233567 buildgrid-0.0.94/buildgrid/server/capabilities/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/capabilities/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7113 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/capabilities/instance.py
+-rwxrwxrwx   0 root         (0) root         (0)     3342 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/capabilities/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.234567 buildgrid-0.0.94/buildgrid/server/cas/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21601 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)    12330 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.237567 buildgrid-0.0.94/buildgrid/server/cas/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3702 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.238566 buildgrid-0.0.94/buildgrid/server/cas/storage/index/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/index/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3335 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/index/index_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)    13464 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/index/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)    38426 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.239567 buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql_dialect_delegates/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql_dialect_delegates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2136 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2120 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4436 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/lru_memory_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/remote.py
+-rw-rw-rw-   0 root         (0) root         (0)    11295 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/replicated.py
+-rw-rw-rw-   0 root         (0) root         (0)    14426 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     6002 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/sharded.py
+-rw-rw-rw-   0 root         (0) root         (0)     6985 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/size_differentiated.py
+-rw-rw-rw-   0 root         (0) root         (0)     9519 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8154 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/storage_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7796 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/with_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3029 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2194 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.239567 buildgrid-0.0.94/buildgrid/server/execution/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/execution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9599 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/execution/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     7517 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/execution/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/job_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    18608 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/metrics_names.py
+-rw-rw-rw-   0 root         (0) root         (0)    14482 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/metrics_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    19548 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.240567 buildgrid-0.0.94/buildgrid/server/operations/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.242567 buildgrid-0.0.94/buildgrid/server/operations/filtering/
+-rw-rw-rw-   0 root         (0) root         (0)      813 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/filtering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/filtering/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/filtering/filter_grammar.lark
+-rw-rw-rw-   0 root         (0) root         (0)     5769 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/filtering/interpreter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/filtering/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4594 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/filtering/sanitizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4802 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     6034 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.242567 buildgrid-0.0.94/buildgrid/server/persistence/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.243567 buildgrid-0.0.94/buildgrid/server/persistence/sql/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.244567 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/README
+-rw-rw-rw-   0 root         (0) root         (0)     2919 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/env.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.249567 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2422 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1191 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py
+-rw-rw-rw-   0 root         (0) root         (0)     4625 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py
+-rw-rw-rw-   0 root         (0) root         (0)     2072 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py
+-rw-rw-rw-   0 root         (0) root         (0)    79716 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     8915 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6206 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/notifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    10298 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.249567 buildgrid-0.0.94/buildgrid/server/redis/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/redis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6197 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/redis/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4739 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/request_metadata_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.250567 buildgrid-0.0.94/buildgrid/server/s3/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18695 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/s3/s3utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    30687 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/server.py
+-rw-rw-rw-   0 root         (0) root         (0)     6126 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/servicer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.251567 buildgrid-0.0.94/buildgrid/server/sql/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/sql/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22206 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/sql/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     6225 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/sql/sqlutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/threading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.252567 buildgrid-0.0.94/buildgrid/server/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4484 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/utils/async_lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/utils/context.py
+-rw-rw-rw-   0 root         (0) root         (0)    10885 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/utils/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5450 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    12244 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.265567 buildgrid-0.0.94/buildgrid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6931 2024-04-29 15:22:12.000000 buildgrid-0.0.94/buildgrid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21169 2024-04-29 15:22:12.000000 buildgrid-0.0.94/buildgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 15:22:12.000000 buildgrid-0.0.94/buildgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-29 15:22:12.000000 buildgrid-0.0.94/buildgrid.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1213 2024-04-29 15:22:12.000000 buildgrid-0.0.94/buildgrid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-29 15:22:12.000000 buildgrid-0.0.94/buildgrid.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.157566 buildgrid-0.0.94/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.256567 buildgrid-0.0.94/data/config/
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/all-in-one.yml
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/artifacts.yml
+-rwxrwxrwx   0 root         (0) root         (0)     1351 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/basic-with-disk.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/bots-interface.yml
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/cache.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/controller.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/default.yml
+-rw-rw-rw-   0 root         (0) root         (0)      832 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/index-sqlite-no-execution.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/index-sqlite.yml
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/logstream.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/monitoring-controller.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/multi-layer-storage.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/redis-cache.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/s3-indexed-cas.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/storage-redis.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/storage-s3.yml
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/storage.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/with-metering.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/with-pgbouncer.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.256567 buildgrid-0.0.94/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      610 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.257567 buildgrid-0.0.94/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.258567 buildgrid-0.0.94/docs/source/data/
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/data/basic-disk-cas.yml
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/data/bazel-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/data/buildstream-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      446 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/data/cas-and-ac.yml
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/data/cas-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/data/execution-and-bots.yml
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/data/sqlite-index-cas-only.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5436 2024-04-29 15:21:45.000000 buildgrid-0.0.94/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-29 15:22:12.272567 buildgrid-0.0.94/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      643 2024-04-29 15:21:45.000000 buildgrid-0.0.94/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.261567 buildgrid-0.0.94/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.158566 buildgrid-0.0.94/tests/auth/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.264567 buildgrid-0.0.94/tests/auth/data/
+-rw-rw-rw-   0 root         (0) root         (0)      733 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/auth.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwks-valid.json
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-hs256-conflicting.secret
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-hs256-expired.token
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-hs256-matching.secret
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-hs256-unbounded.token
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-hs256-valid.token
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-rs256-conflicting.pub.key
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-rs256-expired.token
+-rw-rw-rw-   0 root         (0) root         (0)      559 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-rs256-jwk-encrypted.token
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-rs256-matching.priv.key
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-rs256-matching.pub.key
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-rs256-unbounded.token
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-rs256-valid.token
+-rw-rw-rw-   0 root         (0) root         (0)     3829 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_async_lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    15407 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_execution_instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     2199 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_job_assigner.py
+-rw-rw-rw-   0 root         (0) root         (0)    12358 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_metrics_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_mirrored_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_multithreaded_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_request_metadata_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    32384 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)    10567 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_utils.py
```

### Comparing `buildgrid-0.0.93/BuildGrid.doap` & `buildgrid-0.0.94/BuildGrid.doap`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/CONTRIBUTING.rst` & `buildgrid-0.0.94/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/LICENSE` & `buildgrid-0.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/PKG-INFO` & `buildgrid-0.0.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildgrid
-Version: 0.0.93
+Version: 0.0.94
 Summary: A remote execution service
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://buildgrid.build
 Project-URL: Documentation, https://buildgrid.build
 Project-URL: Repository, https://gitlab.com/BuildGrid/buildgrid
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `buildgrid-0.0.93/README.rst` & `buildgrid-0.0.94/README.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/__init__.py` & `buildgrid-0.0.94/buildgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/__init__.py` & `buildgrid-0.0.94/buildgrid/_app/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/cli.py` & `buildgrid-0.0.94/buildgrid/_app/cli.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/commands/__init__.py` & `buildgrid-0.0.94/buildgrid/_app/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/commands/cmd_actioncache.py` & `buildgrid-0.0.94/buildgrid/_app/commands/cmd_actioncache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/commands/cmd_browser_backend.py` & `buildgrid-0.0.94/buildgrid/_app/commands/cmd_browser_backend.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/commands/cmd_capabilities.py` & `buildgrid-0.0.94/buildgrid/_app/commands/cmd_capabilities.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/commands/cmd_cas.py` & `buildgrid-0.0.94/buildgrid/_app/commands/cmd_cas.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/commands/cmd_cleanup.py` & `buildgrid-0.0.94/buildgrid/_app/commands/cmd_cleanup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/commands/cmd_execute.py` & `buildgrid-0.0.94/buildgrid/_app/commands/cmd_execute.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/commands/cmd_janitor.py` & `buildgrid-0.0.94/buildgrid/_app/commands/cmd_janitor.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/commands/cmd_logstream.py` & `buildgrid-0.0.94/buildgrid/_app/commands/cmd_logstream.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/commands/cmd_operation.py` & `buildgrid-0.0.94/buildgrid/_app/commands/cmd_operation.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/commands/cmd_server.py` & `buildgrid-0.0.94/buildgrid/_app/commands/cmd_server.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/commands/rpc_utils.py` & `buildgrid-0.0.94/buildgrid/_app/commands/rpc_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/__init__.py` & `buildgrid-0.0.94/buildgrid/_app/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/parser.py` & `buildgrid-0.0.94/buildgrid/_app/settings/parser.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/reference.yml` & `buildgrid-0.0.94/buildgrid/_app/settings/reference.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml` & `buildgrid-0.0.94/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml` & `buildgrid-0.0.94/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/schemas/config.yaml` & `buildgrid-0.0.94/buildgrid/_app/settings/schemas/config.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/schemas/connections/sql.yaml` & `buildgrid-0.0.94/buildgrid/_app/settings/schemas/connections/sql.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/schemas/misc/channel.yaml` & `buildgrid-0.0.94/buildgrid/_app/settings/schemas/misc/channel.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/schemas/scheduler/sql.yaml` & `buildgrid-0.0.94/buildgrid/_app/settings/schemas/scheduler/sql.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/action-cache.yaml` & `buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/bots.yaml` & `buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/bots.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/execution.yaml` & `buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/execution.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml` & `buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/remote.yaml` & `buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/remote.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/s3.yaml` & `buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/s3.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml` & `buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/sql-index.yaml` & `buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/sql-index.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_enums.py` & `buildgrid-0.0.94/buildgrid/_enums.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_exceptions.py` & `buildgrid-0.0.94/buildgrid/_exceptions.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/build/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/google/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/bytestream/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/google/bytestream/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py` & `buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py` & `buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/longrunning/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/google/longrunning/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py` & `buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py` & `buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/rpc/__init__.py` & `buildgrid-0.0.94/buildgrid/_protos/google/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2.py` & `buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi` & `buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_types.py` & `buildgrid-0.0.94/buildgrid/_types.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/_version.py` & `buildgrid-0.0.94/buildgrid/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.0.93"
+__version__ = "0.0.94"
```

### Comparing `buildgrid-0.0.93/buildgrid/browser/__init__.py` & `buildgrid-0.0.94/buildgrid/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/browser/app.py` & `buildgrid-0.0.94/buildgrid/browser/app.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/browser/rest_api.py` & `buildgrid-0.0.94/buildgrid/browser/rest_api.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/browser/utils.py` & `buildgrid-0.0.94/buildgrid/browser/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/cleanup/__init__.py` & `buildgrid-0.0.94/buildgrid/cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/cleanup/cleanup.py` & `buildgrid-0.0.94/buildgrid/cleanup/cleanup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,22 @@
 import time
 from contextlib import ExitStack
 from datetime import datetime, timedelta
 from typing import Any, Dict, List, Optional
 
 from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2 import Digest
 from buildgrid.server.cas.storage.index.index_abc import IndexABC
-from buildgrid.server.metrics_names import CLEANUP_BYTES_DELETION_RATE_METRIC_NAME, CLEANUP_RUNTIME_METRIC_NAME
-from buildgrid.server.metrics_utils import DurationMetric, publish_gauge_metric
+from buildgrid.server.metrics_names import (
+    CLEANUP_BYTES_DELETED_METRIC_NAME,
+    CLEANUP_BYTES_DELETION_RATE_METRIC_NAME,
+    CLEANUP_INDEX_TOTAL_SIZE_BYTES_EXCLUDE_MARKED_METRIC_NAME,
+    CLEANUP_INDEX_TOTAL_SIZE_BYTES_INCLUDE_MARKED_METRIC_NAME,
+    CLEANUP_RUNTIME_METRIC_NAME,
+)
+from buildgrid.server.metrics_utils import DurationMetric, publish_counter_metric, publish_gauge_metric
 from buildgrid.server.monitoring import (
     MonitoringBus,
     MonitoringOutputFormat,
     MonitoringOutputType,
     get_monitoring_bus,
     set_monitoring_bus,
 )
@@ -177,25 +183,33 @@
 
         if self._is_instrumented:
             batch_duration = time.time() - batch_start_time
             bytes_deleted_per_second = bytes_deleted / batch_duration
             publish_gauge_metric(
                 CLEANUP_BYTES_DELETION_RATE_METRIC_NAME, bytes_deleted_per_second, {"instance-name": instance_name}
             )
+            publish_counter_metric(CLEANUP_BYTES_DELETED_METRIC_NAME, bytes_deleted, {"instance-name": instance_name})
 
     def _cleanup_worker(self, instance_name: str, stop_requested: threading.Event) -> None:
         """Cleanup when full"""
         index = self._indexes[instance_name]
         index.set_instance_name(instance_name)
         LOGGER.info(f"Cleanup for instance '{instance_name}' started.")
 
         while not stop_requested.is_set():
             # When first starting a loop, we will also include any remaining delete markers as part of
             # the total size.
             total_size = index.get_total_size(include_marked=True)
+            if self._is_instrumented:
+                publish_gauge_metric(
+                    CLEANUP_INDEX_TOTAL_SIZE_BYTES_INCLUDE_MARKED_METRIC_NAME,
+                    total_size,
+                    {"instance-name": instance_name},
+                )
+
             if total_size >= self._high_watermark:
                 to_delete = total_size - self._low_watermark
                 LOGGER.info(
                     f"CAS size for instance '{instance_name}' is {total_size} bytes, at least "
                     f"{to_delete} bytes will be cleared."
                 )
                 LOGGER.info(f"Deleting items from storage/index for instance '{instance_name}'.")
@@ -209,17 +223,30 @@
                             only_delete_before=only_delete_before,
                             total_size=total_size,
                             stop_requested=stop_requested,
                         )
                         # Here we should have already deleted any remaining delete markers,
                         # Our cleanup target should be based on finding new entries.
                         total_size = index.get_total_size(include_marked=False)
+                        if self._is_instrumented:
+                            publish_gauge_metric(
+                                CLEANUP_INDEX_TOTAL_SIZE_BYTES_EXCLUDE_MARKED_METRIC_NAME,
+                                total_size,
+                                {"instance-name": instance_name},
+                            )
+
                         LOGGER.info(f"After batch, the non-stale total size is {total_size} bytes.")
 
                 # Report the final size including the marked deleted items.
                 total_size = index.get_total_size(include_marked=True)
+                if self._is_instrumented:
+                    publish_gauge_metric(
+                        CLEANUP_INDEX_TOTAL_SIZE_BYTES_INCLUDE_MARKED_METRIC_NAME,
+                        total_size,
+                        {"instance-name": instance_name},
+                    )
                 LOGGER.info(f"Finished cleanup. CAS size is now {total_size} bytes.")
 
             stop_requested.wait(timeout=self._sleep_interval)
 
     def _get_last_accessed_threshold(self) -> datetime:
         return datetime.utcnow() - self._only_if_unused_for
```

### Comparing `buildgrid-0.0.93/buildgrid/cleanup/janitor/__init__.py` & `buildgrid-0.0.94/buildgrid/cleanup/janitor/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/cleanup/janitor/config.py` & `buildgrid-0.0.94/buildgrid/cleanup/janitor/config.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/cleanup/janitor/index.py` & `buildgrid-0.0.94/buildgrid/cleanup/janitor/index.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/cleanup/janitor/s3.py` & `buildgrid-0.0.94/buildgrid/cleanup/janitor/s3.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/cleanup/janitor/utils.py` & `buildgrid-0.0.94/buildgrid/cleanup/janitor/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/client/__init__.py` & `buildgrid-0.0.94/buildgrid/client/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/client/actioncache.py` & `buildgrid-0.0.94/buildgrid/client/actioncache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/client/asset.py` & `buildgrid-0.0.94/buildgrid/client/asset.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/client/auth_token_loader.py` & `buildgrid-0.0.94/buildgrid/client/auth_token_loader.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/client/authentication.py` & `buildgrid-0.0.94/buildgrid/client/authentication.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/client/capabilities.py` & `buildgrid-0.0.94/buildgrid/client/capabilities.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/client/cas.py` & `buildgrid-0.0.94/buildgrid/client/cas.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/client/channel.py` & `buildgrid-0.0.94/buildgrid/client/channel.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/client/interceptors.py` & `buildgrid-0.0.94/buildgrid/client/interceptors.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/client/logstream.py` & `buildgrid-0.0.94/buildgrid/client/logstream.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/client/retrier.py` & `buildgrid-0.0.94/buildgrid/client/retrier.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/__init__.py` & `buildgrid-0.0.94/buildgrid/server/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/actioncache/__init__.py` & `buildgrid-0.0.94/buildgrid/server/actioncache/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/actioncache/caches/__init__.py` & `buildgrid-0.0.94/buildgrid/server/actioncache/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/actioncache/caches/action_cache_abc.py` & `buildgrid-0.0.94/buildgrid/server/actioncache/caches/action_cache_abc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/actioncache/caches/lru_cache.py` & `buildgrid-0.0.94/buildgrid/server/actioncache/caches/lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/actioncache/caches/mirrored_cache.py` & `buildgrid-0.0.94/buildgrid/server/actioncache/caches/mirrored_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/actioncache/caches/redis_cache.py` & `buildgrid-0.0.94/buildgrid/server/actioncache/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/actioncache/caches/remote_cache.py` & `buildgrid-0.0.94/buildgrid/server/actioncache/caches/remote_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/actioncache/caches/s3_cache.py` & `buildgrid-0.0.94/buildgrid/server/actioncache/caches/s3_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/actioncache/caches/with_cache.py` & `buildgrid-0.0.94/buildgrid/server/actioncache/caches/with_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/actioncache/caches/write_once_cache.py` & `buildgrid-0.0.94/buildgrid/server/actioncache/caches/write_once_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/actioncache/instance.py` & `buildgrid-0.0.94/buildgrid/server/actioncache/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/actioncache/service.py` & `buildgrid-0.0.94/buildgrid/server/actioncache/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/auth/__init__.py` & `buildgrid-0.0.94/buildgrid/server/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/auth/config.py` & `buildgrid-0.0.94/buildgrid/server/auth/config.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/auth/enums.py` & `buildgrid-0.0.94/buildgrid/server/auth/enums.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/auth/exceptions.py` & `buildgrid-0.0.94/buildgrid/server/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/auth/manager.py` & `buildgrid-0.0.94/buildgrid/server/auth/manager.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/bots/__init__.py` & `buildgrid-0.0.94/buildgrid/server/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/bots/instance.py` & `buildgrid-0.0.94/buildgrid/server/bots/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,11 +236,11 @@
             f"instance_name=[{self._instance_name}]"
             f" request.bot_name=[{bot_session.name}]"
             f" request.bot_id=[{bot_session.bot_id}]"
             f" request.bot_status=[{bot_session.status}]"
         )
         if bot_session.leases:
             lease = bot_session.leases[0]
-            log_tags += f"request.lease_id=[{lease.id}] request.lease_state=[{lease.state}]"
+            log_tags += f" request.lease_id=[{lease.id}] request.lease_state=[{lease.state}]"
         else:
-            log_tags += "request.lease_id=[] request.lease_state=[]"
+            log_tags += " request.lease_id=[] request.lease_state=[]"
         return log_tags
```

### Comparing `buildgrid-0.0.93/buildgrid/server/bots/job_assigner.py` & `buildgrid-0.0.94/buildgrid/server/bots/job_assigner.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/bots/service.py` & `buildgrid-0.0.94/buildgrid/server/bots/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/build_events/__init__.py` & `buildgrid-0.0.94/buildgrid/server/build_events/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/build_events/service.py` & `buildgrid-0.0.94/buildgrid/server/build_events/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/build_events/storage.py` & `buildgrid-0.0.94/buildgrid/server/build_events/storage.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/capabilities/__init__.py` & `buildgrid-0.0.94/buildgrid/server/capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/capabilities/instance.py` & `buildgrid-0.0.94/buildgrid/server/capabilities/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/capabilities/service.py` & `buildgrid-0.0.94/buildgrid/server/capabilities/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/__init__.py` & `buildgrid-0.0.94/buildgrid/server/cas/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/instance.py` & `buildgrid-0.0.94/buildgrid/server/cas/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -394,22 +394,15 @@
     bytestream_read_ignored_exceptions = (NotFoundError, RetriableError)
 
     @generator_method_duration_metric(CAS_BYTESTREAM_READ_TIME_METRIC_NAME)
     @generator_method_exception_counter(
         CAS_BYTESTREAM_READ_EXCEPTION_COUNT_METRIC_NAME,
         ignored_exceptions=bytestream_read_ignored_exceptions,
     )
-    def read_cas_blob(
-        self, digest_hash: str, digest_size: str, read_offset: int, read_limit: int
-    ) -> Iterator[bs_pb2.ReadResponse]:
-        if len(digest_hash) != HASH_LENGTH or not digest_size.isdigit():
-            raise InvalidArgumentError(f"Invalid digest [{digest_hash}/{digest_size}]")
-
-        digest = Digest(hash=digest_hash, size_bytes=int(digest_size))
-
+    def read_cas_blob(self, digest: Digest, read_offset: int, read_limit: int) -> Iterator[bs_pb2.ReadResponse]:
         # Check the given read offset and limit.
         if read_offset < 0 or read_offset > digest.size_bytes:
             raise OutOfRangeError("Read offset out of range")
 
         elif read_limit == 0:
             bytes_remaining = digest.size_bytes - read_offset
```

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/service.py` & `buildgrid-0.0.94/buildgrid/server/cas/service.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from buildgrid._exceptions import InvalidArgumentError
 from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2 import DESCRIPTOR as RE_DESCRIPTOR
 from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2 import (
     BatchReadBlobsRequest,
     BatchReadBlobsResponse,
     BatchUpdateBlobsRequest,
     BatchUpdateBlobsResponse,
+    Digest,
     FindMissingBlobsRequest,
     FindMissingBlobsResponse,
     GetTreeRequest,
     GetTreeResponse,
 )
 from buildgrid._protos.build.bazel.remote.execution.v2.remote_execution_pb2_grpc import (
     ContentAddressableStorageServicer,
@@ -76,14 +77,15 @@
 from buildgrid.server.utils.decorators import (
     handle_errors_stream_unary,
     handle_errors_unary_stream,
     handle_errors_unary_unary,
     track_request_id,
     track_request_id_generator,
 )
+from buildgrid.settings import HASH_LENGTH
 
 LOGGER = logging.getLogger(__name__)
 
 
 def _printable_batch_update_blobs_request(request: BatchUpdateBlobsRequest) -> Dict[str, Any]:
     # Log the digests but not the data
     return {
@@ -206,29 +208,53 @@
     @authorize_unary_stream(lambda r: _parse_resource_name(r.resource_name, ResourceNameRegex.READ)[0])
     @context_module.metadatacontext()
     @track_request_id_generator
     @generator_method_duration_metric(CAS_BYTESTREAM_READ_TIME_METRIC_NAME)
     @handle_errors_unary_stream(ReadResponse)
     def Read(self, request: ReadRequest, context: grpc.ServicerContext) -> Iterator[ReadResponse]:
         LOGGER.info(
-            f"Read request from [{context.peer()}] " f"([{printable_request_metadata(context.invocation_metadata())}])"
+            f"Read request from [{context.peer()}] ([{printable_request_metadata(context.invocation_metadata())}])"
         )
         instance_name, resource_name, resource_type = _parse_resource_name(
             request.resource_name, ResourceNameRegex.READ
         )
         instance = self.get_instance(instance_name)
         if resource_type == ByteStreamResourceType.CAS:
             blob_details = resource_name.split("/")
-            hash_, size_bytes = blob_details[1], blob_details[2]
-            if size_bytes == "0":
-                if hash_ != EMPTY_BLOB_DIGEST.hash:
-                    raise InvalidArgumentError(f"Invalid digest [{hash_}/{size_bytes}]")
-                yield bytestream_pb2.ReadResponse(data=EMPTY_BLOB)
-            else:
-                yield from instance.read_cas_blob(hash_, size_bytes, request.read_offset, request.read_limit)
+            if len(blob_details[1]) != HASH_LENGTH:
+                raise InvalidArgumentError(f"Invalid digest [{resource_name}]")
+            try:
+                digest = Digest(hash=blob_details[1], size_bytes=int(blob_details[2]))
+            except ValueError:
+                raise InvalidArgumentError(f"Invalid digest [{resource_name}]")
+
+            bytes_returned = 0
+            expected_bytes = digest.size_bytes - request.read_offset
+            if request.read_limit:
+                expected_bytes = min(expected_bytes, request.read_limit)
+
+            try:
+                if digest.size_bytes == 0:
+                    if digest.hash != EMPTY_BLOB_DIGEST.hash:
+                        raise InvalidArgumentError(f"Invalid digest [{digest.hash}/{digest.size_bytes}]")
+                    yield bytestream_pb2.ReadResponse(data=EMPTY_BLOB)
+                    return
+
+                for blob in instance.read_cas_blob(digest, request.read_offset, request.read_limit):
+                    bytes_returned += len(blob.data)
+                    yield blob
+            finally:
+                if bytes_returned != expected_bytes:
+                    LOGGER.warning(
+                        f"Read request {digest.hash}/{digest.size_bytes} exited early."
+                        f" bytes_returned={bytes_returned} expected_bytes={expected_bytes}"
+                        f" read_offset={request.read_offset} read_limit={request.read_limit}"
+                    )
+                else:
+                    LOGGER.info(f"Read request {digest.hash}/{digest.size_bytes} completed")
 
     @authorize_stream_unary(lambda r: _parse_resource_name(r.resource_name, ResourceNameRegex.WRITE)[0])
     @context_module.metadatacontext()
     @track_request_id
     @DurationMetric(CAS_BYTESTREAM_WRITE_TIME_METRIC_NAME)
     @handle_errors_stream_unary(WriteResponse, get_printable_request=_printable_write_request)
     def Write(self, request_iterator: Iterator[WriteRequest], context: grpc.ServicerContext) -> WriteResponse:
```

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/__init__.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/disk.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/disk.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/index/__init__.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/index/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/index/index_abc.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/index/index_abc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/index/redis.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/index/redis.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/lru_memory_cache.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/lru_memory_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/redis.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/redis.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/remote.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/remote.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/replicated.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/replicated.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/s3.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/s3.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/sharded.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/sharded.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/size_differentiated.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/size_differentiated.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/sql.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/sql.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/storage_abc.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/storage_abc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/cas/storage/with_cache.py` & `buildgrid-0.0.94/buildgrid/server/cas/storage/with_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/context.py` & `buildgrid-0.0.94/buildgrid/server/context.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/controller.py` & `buildgrid-0.0.94/buildgrid/server/controller.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/execution/__init__.py` & `buildgrid-0.0.94/buildgrid/server/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/execution/instance.py` & `buildgrid-0.0.94/buildgrid/server/execution/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/execution/service.py` & `buildgrid-0.0.94/buildgrid/server/execution/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/job_metrics.py` & `buildgrid-0.0.94/buildgrid/server/job_metrics.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/metrics_names.py` & `buildgrid-0.0.94/buildgrid/server/metrics_names.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,23 @@
 
 #: Number of blobs deleted per second in a cleanup batch
 CLEANUP_BLOBS_DELETION_RATE_METRIC_NAME = "cleanup.blobs-deleted-per-second"
 
 #: Number of bytes deleted per second in a cleanup batch
 CLEANUP_BYTES_DELETION_RATE_METRIC_NAME = "cleanup.bytes-deleted-per-second"
 
+#: Number of bytes deleted in a cleanup batch
+CLEANUP_BYTES_DELETED_METRIC_NAME = "cleanup.bytes-deleted"
+
+#: Number of bytes reported by index not including blobs that are marked as deleted
+CLEANUP_INDEX_TOTAL_SIZE_BYTES_EXCLUDE_MARKED_METRIC_NAME = "cleanup.index.total-size-bytes-exclude-stale"
+
+#: Number of bytes reported by index including blobs that are marked as deleted
+CLEANUP_INDEX_TOTAL_SIZE_BYTES_INCLUDE_MARKED_METRIC_NAME = "cleanup.index.total-size-bytes-include-stale"
+
 #: Total time taken to clean enough blobs to get the CAS size down to the low watermark
 CLEANUP_RUNTIME_METRIC_NAME = "cleanup.runtime-timer"
 
 #: Time taken to bulk delete a set of blobs from the index
 CLEANUP_INDEX_BULK_DELETE_METRIC_NAME = "cleanup.index.bulk-delete-timer"
 
 #: Time taken to mark a set of blobs as deleted in the index
```

### Comparing `buildgrid-0.0.93/buildgrid/server/metrics_utils.py` & `buildgrid-0.0.94/buildgrid/server/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/monitoring.py` & `buildgrid-0.0.94/buildgrid/server/monitoring.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/operations/__init__.py` & `buildgrid-0.0.94/buildgrid/server/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/operations/filtering/__init__.py` & `buildgrid-0.0.94/buildgrid/server/operations/filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/operations/filtering/filter.py` & `buildgrid-0.0.94/buildgrid/server/operations/filtering/filter.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/operations/filtering/filter_grammar.lark` & `buildgrid-0.0.94/buildgrid/server/operations/filtering/filter_grammar.lark`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/operations/filtering/interpreter.py` & `buildgrid-0.0.94/buildgrid/server/operations/filtering/interpreter.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/operations/filtering/parser.py` & `buildgrid-0.0.94/buildgrid/server/operations/filtering/parser.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/operations/filtering/sanitizer.py` & `buildgrid-0.0.94/buildgrid/server/operations/filtering/sanitizer.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/operations/instance.py` & `buildgrid-0.0.94/buildgrid/server/operations/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/operations/service.py` & `buildgrid-0.0.94/buildgrid/server/operations/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/__init__.py` & `buildgrid-0.0.94/buildgrid/server/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/__init__.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/env.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/env.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/script.py.mako` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/impl.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1300,24 +1300,30 @@
                 #   lease was completed before the bot has had the opportunity to transition to ACTIVE, or if the
                 #   update transitioning the lease to the ACTIVE state was lost.
                 #
                 if session_lease.state == LeaseState.COMPLETED.value and db_lease.state in (
                     LeaseState.PENDING.value,
                     LeaseState.ACTIVE.value,
                 ):
+                    log_tags += f" request.lease_status_code=[{session_lease.status.code}]"
+                    log_tags += f" request.lease_status_message=[{session_lease.status.message}]"
+                    log_tags += f" db.n_tries=[{job.n_tries}]"
+
                     bot.lease_id = None
                     if (
                         session_lease.status.code in self.RETRYABLE_STATUS_CODES
                         and (job.n_tries or 1) < self.max_job_attempts
                     ):
+                        LOGGER.debug(f"Retrying bot lease. {log_tags}")
                         self._retry_job_lease(session, job, db_lease)
                     else:
+                        LOGGER.debug(f"Bot completed lease. {log_tags}")
                         self._complete_lease(session, job, db_lease, session_lease.status, session_lease.result)
+
                     self._notify_job_updated(job.name, session)
-                    LOGGER.debug(f"Bot completed lease. {log_tags}")
                     return None
 
                 # Cancel:
                 #
                 #   At any time, the service may change the state of a lease from PENDING or ACTIVE to CANCELLED;
                 #   the bot may not change to this state. The service then waits for the bot to acknowledge the
                 #   change by updating its own status to CANCELLED as well. Once both the service and the bot agree,
```

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/models.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/models.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/notifier.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/notifier.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/persistence/sql/utils.py` & `buildgrid-0.0.94/buildgrid/server/persistence/sql/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/redis/__init__.py` & `buildgrid-0.0.94/buildgrid/server/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/redis/provider.py` & `buildgrid-0.0.94/buildgrid/server/redis/provider.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/request_metadata_utils.py` & `buildgrid-0.0.94/buildgrid/server/request_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/s3/__init__.py` & `buildgrid-0.0.94/buildgrid/server/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/s3/s3utils.py` & `buildgrid-0.0.94/buildgrid/server/s3/s3utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/server.py` & `buildgrid-0.0.94/buildgrid/server/server.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/servicer.py` & `buildgrid-0.0.94/buildgrid/server/servicer.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/sql/__init__.py` & `buildgrid-0.0.94/buildgrid/server/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/sql/provider.py` & `buildgrid-0.0.94/buildgrid/server/sql/provider.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/sql/sqlutils.py` & `buildgrid-0.0.94/buildgrid/server/sql/sqlutils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/threading.py` & `buildgrid-0.0.94/buildgrid/server/threading.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/utils/__init__.py` & `buildgrid-0.0.94/buildgrid/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/utils/async_lru_cache.py` & `buildgrid-0.0.94/buildgrid/server/utils/async_lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/utils/context.py` & `buildgrid-0.0.94/buildgrid/server/utils/context.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/server/utils/decorators.py` & `buildgrid-0.0.94/buildgrid/server/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/settings.py` & `buildgrid-0.0.94/buildgrid/settings.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid/utils.py` & `buildgrid-0.0.94/buildgrid/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid.egg-info/PKG-INFO` & `buildgrid-0.0.94/buildgrid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildgrid
-Version: 0.0.93
+Version: 0.0.94
 Summary: A remote execution service
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://buildgrid.build
 Project-URL: Documentation, https://buildgrid.build
 Project-URL: Repository, https://gitlab.com/BuildGrid/buildgrid
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `buildgrid-0.0.93/buildgrid.egg-info/SOURCES.txt` & `buildgrid-0.0.94/buildgrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/buildgrid.egg-info/requires.txt` & `buildgrid-0.0.94/buildgrid.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/all-in-one.yml` & `buildgrid-0.0.94/data/config/all-in-one.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/artifacts.yml` & `buildgrid-0.0.94/data/config/artifacts.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/basic-with-disk.yml` & `buildgrid-0.0.94/data/config/basic-with-disk.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/bots-interface.yml` & `buildgrid-0.0.94/data/config/bots-interface.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/cache.yml` & `buildgrid-0.0.94/data/config/cache.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/controller.yml` & `buildgrid-0.0.94/data/config/controller.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/default.yml` & `buildgrid-0.0.94/data/config/default.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/index-sqlite-no-execution.yml` & `buildgrid-0.0.94/data/config/index-sqlite-no-execution.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/index-sqlite.yml` & `buildgrid-0.0.94/data/config/index-sqlite.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/monitoring-controller.yml` & `buildgrid-0.0.94/data/config/monitoring-controller.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/multi-layer-storage.yml` & `buildgrid-0.0.94/data/config/multi-layer-storage.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/redis-cache.yml` & `buildgrid-0.0.94/data/config/redis-cache.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/s3-indexed-cas.yml` & `buildgrid-0.0.94/data/config/s3-indexed-cas.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/storage-redis.yml` & `buildgrid-0.0.94/data/config/storage-redis.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/storage-s3.yml` & `buildgrid-0.0.94/data/config/storage-s3.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/storage.yml` & `buildgrid-0.0.94/data/config/storage.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/with-metering.yml` & `buildgrid-0.0.94/data/config/with-metering.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/data/config/with-pgbouncer.yml` & `buildgrid-0.0.94/data/config/with-pgbouncer.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/docs/Makefile` & `buildgrid-0.0.94/docs/Makefile`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/docs/source/data/execution-and-bots.yml` & `buildgrid-0.0.94/docs/source/data/execution-and-bots.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/docs/source/data/sqlite-index-cas-only.yml` & `buildgrid-0.0.94/docs/source/data/sqlite-index-cas-only.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/docs/source/index.rst` & `buildgrid-0.0.94/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/pyproject.toml` & `buildgrid-0.0.94/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "setuptools >= 44",
     "wheel >= 0.35",
 ]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "buildgrid"
-version = "0.0.93"
+version = "0.0.94"
 requires-python = ">=3.8"
 description = "A remote execution service"
 readme = "README.rst"
 license = {text = "Apache License, Version 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
```

### Comparing `buildgrid-0.0.93/setup.cfg` & `buildgrid-0.0.94/setup.cfg`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/setup.py` & `buildgrid-0.0.94/setup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/tests/auth/data/auth.yaml` & `buildgrid-0.0.94/tests/auth/data/auth.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/tests/auth/data/jwt-rs256-jwk-encrypted.token` & `buildgrid-0.0.94/tests/auth/data/jwt-rs256-jwk-encrypted.token`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/tests/auth/data/jwt-rs256-matching.priv.key` & `buildgrid-0.0.94/tests/auth/data/jwt-rs256-matching.priv.key`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/tests/test_async_lru_cache.py` & `buildgrid-0.0.94/tests/test_async_lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/tests/test_execution_instance.py` & `buildgrid-0.0.94/tests/test_execution_instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/tests/test_job_assigner.py` & `buildgrid-0.0.94/tests/test_job_assigner.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/tests/test_metrics_utils.py` & `buildgrid-0.0.94/tests/test_metrics_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/tests/test_mirrored_cache.py` & `buildgrid-0.0.94/tests/test_mirrored_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/tests/test_multithreaded_metrics.py` & `buildgrid-0.0.94/tests/test_multithreaded_metrics.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/tests/test_parser.py` & `buildgrid-0.0.94/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/tests/test_request_metadata_utils.py` & `buildgrid-0.0.94/tests/test_request_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/tests/test_scheduler.py` & `buildgrid-0.0.94/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.93/tests/test_utils.py` & `buildgrid-0.0.94/tests/test_utils.py`

 * *Files identical despite different names*

