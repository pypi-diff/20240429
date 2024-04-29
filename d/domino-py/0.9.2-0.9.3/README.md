# Comparing `tmp/domino_py-0.9.2.tar.gz` & `tmp/domino_py-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino_py-0.9.2.tar", last modified: Fri Apr 19 19:05:41 2024, max compression
+gzip compressed data, was "domino_py-0.9.3.tar", last modified: Mon Apr 29 18:25:27 2024, max compression
```

## Comparing `domino_py-0.9.2.tar` & `domino_py-0.9.3.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.299061 domino_py-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-04-19 19:05:27.000000 domino_py-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-04-19 19:05:41.299061 domino_py-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-04-19 19:05:27.000000 domino_py-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-19 19:05:27.000000 domino_py-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:05:41.303061 domino_py-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.283062 domino_py-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.287062 domino_py-0.9.2/src/domino/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.287062 domino_py-0.9.2/src/domino/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/actions/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17610 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/base_piece.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.287062 domino_py-0.9.2/src/domino/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13151 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.287062 domino_py-0.9.2/src/domino/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/utils/config-domino-local.toml
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/utils/docker-compose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    20726 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/utils/pieces_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    40723 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/utils/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.287062 domino_py-0.9.2/src/domino/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/client/domino_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/client/github_rest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.287062 domino_py-0.9.2/src/domino/client/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/client/legacy/fs_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/client/legacy/s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/client/local_files_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.291061 domino_py-0.9.2/src/domino/custom_operators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.291061 domino_py-0.9.2/src/domino/custom_operators/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/deprecated/base_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/deprecated/external_python_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/docker_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    26228 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/python_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.291061 domino_py-0.9.2/src/domino/custom_operators/sidecar/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/sidecar/fuse.conf
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/sidecar/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/sidecar/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/sidecar/rclone.conf
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/sidecar/sidecar_lifecycle.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/worker_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.291061 domino_py-0.9.2/src/domino/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.291061 domino_py-0.9.2/src/domino/models/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/models/output_modifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.291061 domino_py-0.9.2/src/domino/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/schemas/container_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/schemas/deploy_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/schemas/display_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/schemas/piece_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/schemas/shared_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.295061 domino_py-0.9.2/src/domino/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/build_docker_images_pieces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.295061 domino_py-0.9.2/src/domino/scripts/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/deprecated/create_docker_compose_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/deprecated/deprecated_piece_dry_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/deprecated/docker_compose_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/deprecated/docker_compose_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/deprecated/run_piece_bash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/load_piece.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/run_piece_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.295061 domino_py-0.9.2/src/domino/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/storage/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.295061 domino_py-0.9.2/src/domino/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/testing/dry_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/testing/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/testing/http_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.295061 domino_py-0.9.2/src/domino/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/utils/metadata_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/utils/piece_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/utils/workflow_shared_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.299061 domino_py-0.9.2/src/domino_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-04-19 19:05:41.000000 domino_py-0.9.2/src/domino_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-19 19:05:41.000000 domino_py-0.9.2/src/domino_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:05:41.000000 domino_py-0.9.2/src/domino_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 19:05:41.000000 domino_py-0.9.2/src/domino_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-19 19:05:41.000000 domino_py-0.9.2/src/domino_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 19:05:41.000000 domino_py-0.9.2/src/domino_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.536545 domino_py-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-04-29 18:25:15.000000 domino_py-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-04-29 18:25:27.532545 domino_py-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-04-29 18:25:15.000000 domino_py-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-29 18:25:15.000000 domino_py-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 18:25:27.536545 domino_py-0.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.516545 domino_py-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.520545 domino_py-0.9.3/src/domino/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.520545 domino_py-0.9.3/src/domino/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/actions/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17610 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/base_piece.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.520545 domino_py-0.9.3/src/domino/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.520545 domino_py-0.9.3/src/domino/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/cli/utils/config-domino-local.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/cli/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/cli/utils/docker-compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    20726 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/cli/utils/pieces_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40723 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/cli/utils/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.520545 domino_py-0.9.3/src/domino/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/client/domino_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/client/github_rest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.520545 domino_py-0.9.3/src/domino/client/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/client/legacy/fs_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/client/legacy/s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/client/local_files_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.524545 domino_py-0.9.3/src/domino/custom_operators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/custom_operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.524545 domino_py-0.9.3/src/domino/custom_operators/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/custom_operators/deprecated/base_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/custom_operators/deprecated/external_python_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/custom_operators/docker_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26228 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/custom_operators/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/custom_operators/python_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.524545 domino_py-0.9.3/src/domino/custom_operators/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/custom_operators/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/custom_operators/sidecar/fuse.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/custom_operators/sidecar/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/custom_operators/sidecar/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/custom_operators/sidecar/rclone.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/custom_operators/sidecar/sidecar_lifecycle.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/custom_operators/worker_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.524545 domino_py-0.9.3/src/domino/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/exceptions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.524545 domino_py-0.9.3/src/domino/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/models/output_modifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.524545 domino_py-0.9.3/src/domino/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/schemas/container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/schemas/deploy_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/schemas/display_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/schemas/piece_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/schemas/shared_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.528545 domino_py-0.9.3/src/domino/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/scripts/build_docker_images_pieces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.528545 domino_py-0.9.3/src/domino/scripts/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/scripts/deprecated/create_docker_compose_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/scripts/deprecated/deprecated_piece_dry_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/scripts/deprecated/docker_compose_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/scripts/deprecated/docker_compose_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/scripts/deprecated/run_piece_bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/scripts/load_piece.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/scripts/run_piece_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.528545 domino_py-0.9.3/src/domino/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/storage/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.528545 domino_py-0.9.3/src/domino/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/testing/dry_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/testing/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/testing/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.528545 domino_py-0.9.3/src/domino/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/utils/metadata_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/utils/piece_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-29 18:25:15.000000 domino_py-0.9.3/src/domino/utils/workflow_shared_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:25:27.532545 domino_py-0.9.3/src/domino_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-04-29 18:25:27.000000 domino_py-0.9.3/src/domino_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-29 18:25:27.000000 domino_py-0.9.3/src/domino_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:25:27.000000 domino_py-0.9.3/src/domino_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-29 18:25:27.000000 domino_py-0.9.3/src/domino_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-29 18:25:27.000000 domino_py-0.9.3/src/domino_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 18:25:27.000000 domino_py-0.9.3/src/domino_py.egg-info/top_level.txt
```

### Comparing `domino_py-0.9.2/LICENSE` & `domino_py-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/PKG-INFO` & `domino_py-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python package for Domino.
 Author-email: Luiz Tauffer <luiz@taufferconsulting.com>, Vinicius Vaz <vinicius@taufferconsulting.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `domino_py-0.9.2/README.md` & `domino_py-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/pyproject.toml` & `domino_py-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/actions/github_actions.py` & `domino_py-0.9.3/src/domino/actions/github_actions.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/base_piece.py` & `domino_py-0.9.3/src/domino/base_piece.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/cli/cli.py` & `domino_py-0.9.3/src/domino/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 import click
 import os
 import uuid
 import tomli
 from domino.cli.utils import pieces_repository, platform
 import ast
+import domino
 
 console = Console()
 
 # Ref: https://patorjk.com/software/taag/
 # Font: standard
 msg = """
 ==============================================
@@ -403,14 +404,15 @@
 
 
 ###############################################################################
 # PARENT GROUP
 ###############################################################################
 
 @click.group()
+@click.version_option(domino.__version__)
 @click.pass_context
 def cli(ctx):
     # console.print(msg, style="rgb(109,125,176)", highlight=False)
     console.print("")
     console.print("Welcome to Domino! :red_heart-emoji:")
     console.print("")
```

### Comparing `domino_py-0.9.2/src/domino/cli/utils/config-domino-local.toml` & `domino_py-0.9.3/src/domino/cli/utils/config-domino-local.toml`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/cli/utils/docker-compose.yaml` & `domino_py-0.9.3/src/domino/cli/utils/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/cli/utils/pieces_repository.py` & `domino_py-0.9.3/src/domino/cli/utils/pieces_repository.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/cli/utils/platform.py` & `domino_py-0.9.3/src/domino/cli/utils/platform.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/client/domino_backend_client.py` & `domino_py-0.9.3/src/domino/client/domino_backend_client.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/client/github_rest_client.py` & `domino_py-0.9.3/src/domino/client/github_rest_client.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/client/legacy/fs_client.py` & `domino_py-0.9.3/src/domino/client/legacy/fs_client.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/client/legacy/s3_client.py` & `domino_py-0.9.3/src/domino/client/legacy/s3_client.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/client/local_files_client.py` & `domino_py-0.9.3/src/domino/client/local_files_client.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/custom_operators/deprecated/base_operator.py` & `domino_py-0.9.3/src/domino/custom_operators/deprecated/base_operator.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/custom_operators/deprecated/external_python_operator.py` & `domino_py-0.9.3/src/domino/custom_operators/deprecated/external_python_operator.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/custom_operators/docker_operator.py` & `domino_py-0.9.3/src/domino/custom_operators/docker_operator.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/custom_operators/k8s_operator.py` & `domino_py-0.9.3/src/domino/custom_operators/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/custom_operators/python_operator.py` & `domino_py-0.9.3/src/domino/custom_operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/custom_operators/sidecar/logger.py` & `domino_py-0.9.3/src/domino/custom_operators/sidecar/logger.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/custom_operators/sidecar/mount.py` & `domino_py-0.9.3/src/domino/custom_operators/sidecar/mount.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/custom_operators/worker_operator.py` & `domino_py-0.9.3/src/domino/custom_operators/worker_operator.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/exceptions/exceptions.py` & `domino_py-0.9.3/src/domino/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/logger.py` & `domino_py-0.9.3/src/domino/logger.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/models/output_modifier.py` & `domino_py-0.9.3/src/domino/models/output_modifier.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/schemas/piece_metadata.py` & `domino_py-0.9.3/src/domino/schemas/piece_metadata.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/schemas/shared_storage.py` & `domino_py-0.9.3/src/domino/schemas/shared_storage.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/scripts/build_docker_images_pieces.py` & `domino_py-0.9.3/src/domino/scripts/build_docker_images_pieces.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/scripts/deprecated/create_docker_compose_file.py` & `domino_py-0.9.3/src/domino/scripts/deprecated/create_docker_compose_file.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/scripts/deprecated/deprecated_piece_dry_run.py` & `domino_py-0.9.3/src/domino/scripts/deprecated/deprecated_piece_dry_run.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/scripts/deprecated/docker_compose_constants.py` & `domino_py-0.9.3/src/domino/scripts/deprecated/docker_compose_constants.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/scripts/deprecated/docker_compose_scripts.py` & `domino_py-0.9.3/src/domino/scripts/deprecated/docker_compose_scripts.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/scripts/deprecated/run_piece_bash.py` & `domino_py-0.9.3/src/domino/scripts/deprecated/run_piece_bash.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/scripts/load_piece.py` & `domino_py-0.9.3/src/domino/scripts/load_piece.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/scripts/run_piece_docker.py` & `domino_py-0.9.3/src/domino/scripts/run_piece_docker.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/storage/s3.py` & `domino_py-0.9.3/src/domino/storage/s3.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/task.py` & `domino_py-0.9.3/src/domino/task.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/testing/dry_run.py` & `domino_py-0.9.3/src/domino/testing/dry_run.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/testing/http_client.py` & `domino_py-0.9.3/src/domino/testing/http_client.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino/utils/piece_generator.py` & `domino_py-0.9.3/src/domino/utils/piece_generator.py`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino_py.egg-info/PKG-INFO` & `domino_py-0.9.3/src/domino_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python package for Domino.
 Author-email: Luiz Tauffer <luiz@taufferconsulting.com>, Vinicius Vaz <vinicius@taufferconsulting.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `domino_py-0.9.2/src/domino_py.egg-info/SOURCES.txt` & `domino_py-0.9.3/src/domino_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domino_py-0.9.2/src/domino_py.egg-info/requires.txt` & `domino_py-0.9.3/src/domino_py.egg-info/requires.txt`

 * *Files identical despite different names*

