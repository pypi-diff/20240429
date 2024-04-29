# Comparing `tmp/foursquare.map-sdk-2.0.0.tar.gz` & `tmp/foursquare.map-sdk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursquare.map-sdk-2.0.0.tar", last modified: Wed Apr 24 19:04:37 2024, max compression
+gzip compressed data, was "foursquare.map-sdk-2.1.0.tar", last modified: Mon Apr 29 17:10:22 2024, max compression
```

## Comparing `foursquare.map-sdk-2.0.0.tar` & `foursquare.map-sdk-2.1.0.tar`

### file list

```diff
@@ -1,130 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.207736 foursquare.map-sdk-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-24 19:04:37.207736 foursquare.map-sdk-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.187736 foursquare.map-sdk-2.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.187736 foursquare.map-sdk-2.0.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.195736 foursquare.map-sdk-2.0.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    30020 2024-04-24 19:03:16.000000 foursquare.map-sdk-2.0.0/docs/source/_static/embed-bundle.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.187736 foursquare.map-sdk-2.0.0/foursquare/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.195736 foursquare.map-sdk-2.0.0/foursquare/map_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.195736 foursquare.map-sdk-2.0.0/foursquare/map_sdk/_poll_v56/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/_poll_v56/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/_poll_v56/_async_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/_poll_v56/_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/_poll_v56/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.199736 foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/annotation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/create_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    27510 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/effect_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/event_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/filter_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20221 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/layer_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26206 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/map_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/colab.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.199736 foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/Animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/Annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    43381 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/Chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/CustomMapState.py
--rw-r--r--   0 runner    (1001) docker     (127)    13727 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/Effect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/Filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/FilterAnimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    65488 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/Layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/MapState.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.199736 foursquare.map-sdk-2.0.0/foursquare/map_sdk/labextension/
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-24 19:04:36.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.203736 foursquare.map-sdk-2.0.0/foursquare/map_sdk/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (127)    18894 2024-04-24 19:04:36.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/labextension/static/480.8564242f18457c329a6c.js
--rw-r--r--   0 runner    (1001) docker     (127)    17928 2024-04-24 19:04:36.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/labextension/static/568.678b6de0871522f1ae1f.js
--rw-r--r--   0 runner    (1001) docker     (127)    11681 2024-04-24 19:04:36.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/labextension/static/645.cf30cf0f2cf9aac000f8.js
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-24 19:04:36.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/labextension/static/remoteEntry.56fa1f1cd9ddfb15b82f.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-24 19:04:35.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-24 19:04:36.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.203736 foursquare.map-sdk-2.0.0/foursquare/map_sdk/map/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/map/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/map/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/map/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.203736 foursquare.map-sdk-2.0.0/foursquare/map_sdk/nbextension/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (127)    30608 2024-04-24 19:04:32.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/nbextension/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/poll.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.203736 foursquare.map-sdk-2.0.0/foursquare/map_sdk/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/templates/html_map_sdk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/transfer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.203736 foursquare.map-sdk-2.0.0/foursquare/map_sdk/transport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/transport/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/transport/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/transport/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.203736 foursquare.map-sdk-2.0.0/foursquare/map_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/utils/action_type_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare/map_sdk/utils/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.195736 foursquare.map-sdk-2.0.0/foursquare.map_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-24 19:04:37.000000 foursquare.map-sdk-2.0.0/foursquare.map_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-24 19:04:37.000000 foursquare.map-sdk-2.0.0/foursquare.map_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:04:37.000000 foursquare.map-sdk-2.0.0/foursquare.map_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-24 19:04:37.000000 foursquare.map-sdk-2.0.0/foursquare.map_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 19:04:37.000000 foursquare.map-sdk-2.0.0/foursquare.map_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/foursquare.map_sdk.json
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/install.json
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.203736 foursquare.map-sdk-2.0.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/scripts/rename_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-24 19:04:37.207736 foursquare.map-sdk-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.207736 foursquare.map-sdk-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.207736 foursquare.map-sdk-2.0.0/tests/api/
--rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/api/test_dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/api/test_effect_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/api/test_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/api/test_layer_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/api/test_map_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.207736 foursquare.map-sdk-2.0.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/fixtures/dataset_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.191736 foursquare.map-sdk-2.0.0/tests/fixtures/raster/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.207736 foursquare.map-sdk-2.0.0/tests/fixtures/raster/collection/
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.207736 foursquare.map-sdk-2.0.0/tests/fixtures/raster/item/
--rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/fixtures/raster/item/sentinel-2-l2a.json
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/fixtures/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.207736 foursquare.map-sdk-2.0.0/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/mocks/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.191736 foursquare.map-sdk-2.0.0/tests/snapshots/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.191736 foursquare.map-sdk-2.0.0/tests/snapshots/test_html_map/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.207736 foursquare.map-sdk-2.0.0/tests/snapshots/test_html_map/test_iframe_template_rendering/
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.207736 foursquare.map-sdk-2.0.0/tests/snapshots/test_html_map/test_template_rendering/
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/snapshots/test_html_map/test_template_rendering/map.html
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/test_html_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/test_nbextension_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/test_subclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/test_widget_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:37.207736 foursquare.map-sdk-2.0.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tests/utils/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-24 18:59:16.000000 foursquare.map-sdk-2.0.0/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.352217 foursquare.map-sdk-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-29 17:10:22.352217 foursquare.map-sdk-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.320217 foursquare.map-sdk-2.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.320217 foursquare.map-sdk-2.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.332217 foursquare.map-sdk-2.1.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    30038 2024-04-29 17:07:00.000000 foursquare.map-sdk-2.1.0/docs/source/_static/embed-bundle.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.324217 foursquare.map-sdk-2.1.0/foursquare/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.332217 foursquare.map-sdk-2.1.0/foursquare/map_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.332217 foursquare.map-sdk-2.1.0/foursquare/map_sdk/_poll_v56/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/_poll_v56/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/_poll_v56/_async_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/_poll_v56/_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/_poll_v56/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.336217 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/annotation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/create_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27510 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/effect_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/event_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.336217 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/columns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.336217 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/layer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8441 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/layer/arc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/layer/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/layer/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/layer/h3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10996 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/layer/hexbin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/layer/icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/layer/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13451 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/layer/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16639 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/layer/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/layer/threed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17637 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/layer/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/experimental/text_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20221 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/layer_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26206 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/map_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/colab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.340217 foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/Animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/Annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43381 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/Chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/CustomMapState.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13727 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/Effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/Filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/FilterAnimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65488 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/Layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/MapState.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.340217 foursquare.map-sdk-2.1.0/foursquare/map_sdk/labextension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-29 17:10:22.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.340217 foursquare.map-sdk-2.1.0/foursquare/map_sdk/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    18894 2024-04-29 17:10:22.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/labextension/static/480.fda607fe17f5f9c59341.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17928 2024-04-29 17:10:22.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/labextension/static/568.29dd46dc8f97daf4b009.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-04-29 17:10:22.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/labextension/static/645.16b1b5e2bfb3ca879bfd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-29 17:10:22.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/labextension/static/remoteEntry.c8d40a54b33b36dba80c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-29 17:10:20.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-29 17:10:22.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.340217 foursquare.map-sdk-2.1.0/foursquare/map_sdk/map/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/map/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/map/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/map/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.340217 foursquare.map-sdk-2.1.0/foursquare/map_sdk/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (127)    30626 2024-04-29 17:10:17.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/nbextension/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/poll.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.340217 foursquare.map-sdk-2.1.0/foursquare/map_sdk/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/templates/html_map_sdk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/transfer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.344217 foursquare.map-sdk-2.1.0/foursquare/map_sdk/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/transport/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/transport/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/transport/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.344217 foursquare.map-sdk-2.1.0/foursquare/map_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/utils/action_type_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare/map_sdk/utils/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.332217 foursquare.map-sdk-2.1.0/foursquare.map_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-29 17:10:22.000000 foursquare.map-sdk-2.1.0/foursquare.map_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-29 17:10:22.000000 foursquare.map-sdk-2.1.0/foursquare.map_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:10:22.000000 foursquare.map-sdk-2.1.0/foursquare.map_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-29 17:10:22.000000 foursquare.map-sdk-2.1.0/foursquare.map_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 17:10:22.000000 foursquare.map-sdk-2.1.0/foursquare.map_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/foursquare.map_sdk.json
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/install.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.344217 foursquare.map-sdk-2.1.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/scripts/rename_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-29 17:10:22.352217 foursquare.map-sdk-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.344217 foursquare.map-sdk-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.348217 foursquare.map-sdk-2.1.0/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/api/test_dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/api/test_effect_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/api/test_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/api/test_layer_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/api/test_map_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.348217 foursquare.map-sdk-2.1.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/fixtures/dataset_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.324217 foursquare.map-sdk-2.1.0/tests/fixtures/raster/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.348217 foursquare.map-sdk-2.1.0/tests/fixtures/raster/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.352217 foursquare.map-sdk-2.1.0/tests/fixtures/raster/item/
+-rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/fixtures/raster/item/sentinel-2-l2a.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/fixtures/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.352217 foursquare.map-sdk-2.1.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/mocks/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.324217 foursquare.map-sdk-2.1.0/tests/snapshots/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.324217 foursquare.map-sdk-2.1.0/tests/snapshots/test_html_map/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.352217 foursquare.map-sdk-2.1.0/tests/snapshots/test_html_map/test_iframe_template_rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.352217 foursquare.map-sdk-2.1.0/tests/snapshots/test_html_map/test_template_rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/snapshots/test_html_map/test_template_rendering/map.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/test_html_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20313 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/test_layers_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/test_nbextension_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/test_subclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/test_widget_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:10:22.352217 foursquare.map-sdk-2.1.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tests/utils/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-29 17:02:41.000000 foursquare.map-sdk-2.1.0/webpack.config.js
```

### Comparing `foursquare.map-sdk-2.0.0/MANIFEST.in` & `foursquare.map-sdk-2.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/PKG-INFO` & `foursquare.map-sdk-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursquare.map-sdk
-Version: 2.0.0
+Version: 2.1.0
 Summary: Jupyter Widget for Foursquare Studio Maps
 Author: Foursquare Labs
 Author-email: info-studio@foursquare.com
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
```

### Comparing `foursquare.map-sdk-2.0.0/docs/source/_static/embed-bundle.js` & `foursquare.map-sdk-2.1.0/docs/source/_static/embed-bundle.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -43,15 +43,15 @@
                         o((n = n.apply(e, t)).next())
                     })),
                     f = ["legend", "toggle-3d", "split-map", "map-draw", "chart", "annotation", "viewport-json", "effect"],
                     E = ((a = E || {}).REMOVE_DATASET = "remove-dataset", a.ADD_LAYER = "add-layer", a.REMOVE_LAYER = "remove-layer", a.ADD_LAYER_GROUP = "add-layer-group", a.REMOVE_LAYER_GROUP = "remove-layer-group", a.ACTIVATE_MAP_CONTROL = "activate-map-control", a.CHANGE_SIDE_PANEL_SECTION = "change-side-panel-section", a.API_KEY_GENERATED_STARTED = "API Key Generated Started", a.API_KEY_GENERATED = "API Key Generated", a.COPY_API_KEY = "Copy API Key", a);
 
                 function _(e, t) {
                     return u(this, null, (function*() {
-                        let n, a = "http://localhost:8080/studio-bundle.js";
+                        let n, a = "https://studio.foursquare.com/studio-bundle.js";
                         (function(e) {
                             return "object" == typeof e && null !== e && "url" in e && "string" == typeof e.url && ("string" == typeof e.namespace || void 0 === e.namespace)
                         })(t) && (a = t.url, n = t.namespace);
                         let {
                             showPlaceholder: i = !0
                         } = e;
                         return e.container && i && (e.container.innerHTML = '<div style="position:relative;width:100%;height:100%;"><div class="map-placeholder">\n  <style>\n    .map-placeholder {\n      position: absolute;\n      top: 0;\n      left: 0;\n      right: 0;\n      width: 100%;\n      height: 100%;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .scene {\n      width: 50px;\n      height: 50px;\n      transform-style: preserve-3d;\n      transform: rotateY(0deg) rotateX(56deg) rotateZ(-45deg);\n    }\n\n    @keyframes fsq-rotate {\n      0% {\n        transform: rotateY(0deg);\n      }\n      5%, 25% {\n        transform: rotateX(-90deg);\n      }\n      30%, 50% {\n        transform: rotateX(-90deg) rotateY(-90deg);\n      }\n      55%, 75% {\n        transform: rotateX(-90deg) rotateY(-90deg) rotateX(-90deg);\n      }\n      80%, 100% {\n        transform: rotateX(-90deg) rotateY(0deg) rotateX(-90deg);\n      }\n    }\n\n    .fsq {\n      width: 50px;\n      height: 50px;\n      position: relative;\n      transform-style: preserve-3d;\n      transition: transform 1s;\n      animation-name: fsq-rotate;\n      animation-iteration-count: infinite;\n      animation-duration: 6s;\n      animation-timing-function: ease;\n    }\n\n    .fsq__face {\n      position: absolute;\n      width: 50px;\n      height: 50px;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .fsq__face--front-f {\n      background: #000;\n      transform: rotateY(0deg) translateZ(25px);\n    }\n\n    .fsq__face--back-f {\n      background: #000;\n      transform: rotateZ(-180deg) rotateY(180deg) translateZ(25px);\n    }\n\n    .fsq__face--right-s {\n      background: #fff;\n      transform: rotateY(90deg) translateZ(25px);\n    }\n\n    .fsq__face--left-s {\n      background: #fff;\n      transform: rotateX(-90deg) rotateY(-90deg) rotateZ(180deg) translateZ(25px);\n    }\n\n    .fsq__face--top-q {\n      background: #3545f5;\n      transform: rotateX(90deg) translateZ(25px);\n    }\n\n    .fsq__face--bottom-q {\n      background: #3545f5;\n      transform: rotateX(-90deg) translateZ(25px);\n    }\n  </style>\n\n\n  <div class="scene">\n    <div class="fsq">\n      <div class="fsq__face fsq__face--front-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--back-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--right-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--left-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--top-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--bottom-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n    </div>\n  </div>\n</div></div>'), (yield function(e) {
@@ -80,15 +80,15 @@
                         }))(((e, t) => r(e, s(t)))(((e, t) => {
                             for (var n in t || (t = {})) d.call(t, n) && p(e, n, t[n]);
                             if (o)
                                 for (var n of o(t)) l.call(t, n) && p(e, n, t[n]);
                             return e
                         })({}, e), {
                             assetUrl: new URL(a).origin,
-                            apiKeyValidationUrl: "http://localhost:8000/catalog/v1/api-key/validate"
+                            apiKeyValidationUrl: "https://data-api.foursquare.com/catalog/v1/api-key/validate"
                         }))
                     }))
                 }
                 var m = {},
                     v = class e extends Error {
                         constructor(t) {
                             super(t), Object.setPrototypeOf(this, e.prototype)
@@ -622,15 +622,15 @@
             },
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"@foursquare/jupyter-map-sdk","version":"2.0.0","description":"JavaScript bindings for Foursquare\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css","LICENSE.txt"],"license":"SEE LICENSE IN LICENSE.txt","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf foursquare/map_sdk/labextension","clean:nbextension":"rimraf \'foursquare/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@foursquare/map-sdk":"^2.0.0","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","aws-sdk":"^2.988.0","csstype":"^3.1.0"},"devDependencies":{"@babel/preset-env":"^7.21.4","@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"foursquare/map_sdk/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+                e.exports = JSON.parse('{"name":"@foursquare/jupyter-map-sdk","version":"2.1.0","description":"JavaScript bindings for Foursquare\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css","LICENSE.txt"],"license":"SEE LICENSE IN LICENSE.txt","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf foursquare/map_sdk/labextension","clean:nbextension":"rimraf \'foursquare/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@foursquare/map-sdk":"^2.1.0","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","aws-sdk":"^2.988.0","csstype":"^3.1.0"},"devDependencies":{"@babel/preset-env":"^7.21.4","@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"foursquare/map_sdk/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
             }
         },
         n = {};
 
     function a(e) {
         var i = n[e];
         if (void 0 !== i) return i.exports;
```

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/__init__.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/_poll.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/_poll.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/_poll_v56/_async_thread.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/_poll_v56/_async_thread.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/_poll_v56/_poll.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/_poll_v56/_poll.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/annotation_api.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/annotation_api.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/base.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/base.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/create_map.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/create_map.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/dataset_api.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/dataset_api.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/effect_api.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/effect_api.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/enums.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/enums.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/event_api.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/event_api.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/filter_api.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/filter_api.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/layer_api.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/layer_api.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/api/map_api.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/api/map_api.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/environment.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/environment.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/Animation.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/Animation.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/Annotation.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/Annotation.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/Chart.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/Chart.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/Effect.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/Effect.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/Filter.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/Filter.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/FilterAnimation.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/FilterAnimation.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/Layer.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/Layer.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/generated/MapState.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/generated/MapState.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/labextension/package.json` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9606186224489796%*

 * *Differences: {"'dependencies'": "{'@foursquare/map-sdk': '^2.1.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.c8d40a54b33b36dba80c.js'}}",*

 * * "'version'": "'2.1.0'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": {
         "email": "info-studio@foursquare.com",
         "name": "Foursquare Labs"
     },
     "dependencies": {
         "@aws-amplify/core": "^4.2.9",
-        "@foursquare/map-sdk": "^2.0.0",
+        "@foursquare/map-sdk": "^2.1.0",
         "@jupyter-widgets/base": "^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0",
         "@lumino/application": "^1.16.0",
         "@lumino/widgets": "^1.30.0",
         "aws-sdk": "^2.988.0",
         "csstype": "^3.1.0"
     },
     "description": "JavaScript bindings for Foursquare's Jupyter Map SDK",
@@ -35,15 +35,15 @@
         "dist/*.js",
         "css/*.css",
         "LICENSE.txt"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.56fa1f1cd9ddfb15b82f.js"
+            "load": "static/remoteEntry.c8d40a54b33b36dba80c.js"
         },
         "extension": "lib/plugin",
         "outputDir": "foursquare/map_sdk/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -79,12 +79,12 @@
         "typecheck": "tsc",
         "typescript": "yarn run -T tsc --noEmit",
         "watch": "npm-run-all -p watch:*",
         "watch:lib": "yarn run -T tsc -w",
         "watch:nbextension": "webpack --watch --mode development"
     },
     "types": "lib/index.d.ts",
-    "version": "2.0.0",
+    "version": "2.1.0",
     "volta": {
         "extends": "../../../package.json"
     }
 }
```

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/labextension/static/480.8564242f18457c329a6c.js` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/labextension/static/480.fda607fe17f5f9c59341.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -360,15 +360,15 @@
                     }
                     d((a = a.apply(e, t || [])).next())
                 }))
             };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.UnfoldedMapView = void 0;
-            const s = n(108),
+            const s = n(178),
                 i = n(565);
             n(204);
             const r = "foursquare-widget";
             class o extends i.DOMWidgetView {
                 initialize() {
                     return a(this, void 0, void 0, (function*() {
                         const e = {
@@ -573,11 +573,11 @@
                         n = d
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"@foursquare/jupyter-map-sdk","version":"2.0.0","description":"JavaScript bindings for Foursquare\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css","LICENSE.txt"],"license":"SEE LICENSE IN LICENSE.txt","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf foursquare/map_sdk/labextension","clean:nbextension":"rimraf \'foursquare/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@foursquare/map-sdk":"^2.0.0","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","aws-sdk":"^2.988.0","csstype":"^3.1.0"},"devDependencies":{"@babel/preset-env":"^7.21.4","@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"foursquare/map_sdk/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+            e.exports = JSON.parse('{"name":"@foursquare/jupyter-map-sdk","version":"2.1.0","description":"JavaScript bindings for Foursquare\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css","LICENSE.txt"],"license":"SEE LICENSE IN LICENSE.txt","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf foursquare/map_sdk/labextension","clean:nbextension":"rimraf \'foursquare/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@foursquare/map-sdk":"^2.1.0","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","aws-sdk":"^2.988.0","csstype":"^3.1.0"},"devDependencies":{"@babel/preset-env":"^7.21.4","@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"foursquare/map_sdk/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
         }
     }
 ]);
```

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/labextension/static/568.678b6de0871522f1ae1f.js` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/labextension/static/568.29dd46dc8f97daf4b009.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
 (self.webpackChunk_foursquare_jupyter_map_sdk = self.webpackChunk_foursquare_jupyter_map_sdk || []).push([
-    [568, 377], {
+    [568, 398], {
         568: function(e, t, n) {
             "use strict";
             var a = this && this.__createBinding || (Object.create ? function(e, t, n, a) {
                     void 0 === a && (a = n);
                     var s = Object.getOwnPropertyDescriptor(t, n);
                     s && !("get" in s ? !t.__esModule : s.writable || s.configurable) || (s = {
                         enumerable: !0,
@@ -311,15 +311,15 @@
                     }
                     d((a = a.apply(e, t || [])).next())
                 }))
             };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.UnfoldedMapView = void 0;
-            const s = n(108),
+            const s = n(178),
                 i = n(565);
             n(204);
             const r = "foursquare-widget";
             class o extends i.DOMWidgetView {
                 initialize() {
                     return a(this, void 0, void 0, (function*() {
                         const e = {
@@ -524,11 +524,11 @@
                         n = d
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"@foursquare/jupyter-map-sdk","version":"2.0.0","description":"JavaScript bindings for Foursquare\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css","LICENSE.txt"],"license":"SEE LICENSE IN LICENSE.txt","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf foursquare/map_sdk/labextension","clean:nbextension":"rimraf \'foursquare/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@foursquare/map-sdk":"^2.0.0","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","aws-sdk":"^2.988.0","csstype":"^3.1.0"},"devDependencies":{"@babel/preset-env":"^7.21.4","@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"foursquare/map_sdk/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+            e.exports = JSON.parse('{"name":"@foursquare/jupyter-map-sdk","version":"2.1.0","description":"JavaScript bindings for Foursquare\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css","LICENSE.txt"],"license":"SEE LICENSE IN LICENSE.txt","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf foursquare/map_sdk/labextension","clean:nbextension":"rimraf \'foursquare/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@foursquare/map-sdk":"^2.1.0","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","aws-sdk":"^2.988.0","csstype":"^3.1.0"},"devDependencies":{"@babel/preset-env":"^7.21.4","@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"foursquare/map_sdk/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
         }
     }
 ]);
```

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/labextension/static/645.cf30cf0f2cf9aac000f8.js` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/labextension/static/645.16b1b5e2bfb3ca879bfd.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -40,59 +40,59 @@
                     s((t = t.apply(e, n)).next())
                 })),
                 u = ["legend", "toggle-3d", "split-map", "map-draw", "chart", "annotation", "viewport-json", "effect"],
                 v = ((a = v || {}).REMOVE_DATASET = "remove-dataset", a.ADD_LAYER = "add-layer", a.REMOVE_LAYER = "remove-layer", a.ADD_LAYER_GROUP = "add-layer-group", a.REMOVE_LAYER_GROUP = "remove-layer-group", a.ACTIVATE_MAP_CONTROL = "activate-map-control", a.CHANGE_SIDE_PANEL_SECTION = "change-side-panel-section", a.API_KEY_GENERATED_STARTED = "API Key Generated Started", a.API_KEY_GENERATED = "API Key Generated", a.COPY_API_KEY = "Copy API Key", a);
 
             function g(e, n) {
                 return c(this, null, (function*() {
-                    let t, a = "http://localhost:8080/studio-bundle.js";
+                    let t, a = "https://studio.foursquare.com/studio-bundle.js";
                     (function(e) {
                         return "object" == typeof e && null !== e && "url" in e && "string" == typeof e.url && ("string" == typeof e.namespace || void 0 === e.namespace)
                     })(n) && (a = n.url, t = n.namespace);
                     let {
                         showPlaceholder: r = !0
                     } = e;
                     return e.container && r && (e.container.innerHTML = '<div style="position:relative;width:100%;height:100%;"><div class="map-placeholder">\n  <style>\n    .map-placeholder {\n      position: absolute;\n      top: 0;\n      left: 0;\n      right: 0;\n      width: 100%;\n      height: 100%;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .scene {\n      width: 50px;\n      height: 50px;\n      transform-style: preserve-3d;\n      transform: rotateY(0deg) rotateX(56deg) rotateZ(-45deg);\n    }\n\n    @keyframes fsq-rotate {\n      0% {\n        transform: rotateY(0deg);\n      }\n      5%, 25% {\n        transform: rotateX(-90deg);\n      }\n      30%, 50% {\n        transform: rotateX(-90deg) rotateY(-90deg);\n      }\n      55%, 75% {\n        transform: rotateX(-90deg) rotateY(-90deg) rotateX(-90deg);\n      }\n      80%, 100% {\n        transform: rotateX(-90deg) rotateY(0deg) rotateX(-90deg);\n      }\n    }\n\n    .fsq {\n      width: 50px;\n      height: 50px;\n      position: relative;\n      transform-style: preserve-3d;\n      transition: transform 1s;\n      animation-name: fsq-rotate;\n      animation-iteration-count: infinite;\n      animation-duration: 6s;\n      animation-timing-function: ease;\n    }\n\n    .fsq__face {\n      position: absolute;\n      width: 50px;\n      height: 50px;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .fsq__face--front-f {\n      background: #000;\n      transform: rotateY(0deg) translateZ(25px);\n    }\n\n    .fsq__face--back-f {\n      background: #000;\n      transform: rotateZ(-180deg) rotateY(180deg) translateZ(25px);\n    }\n\n    .fsq__face--right-s {\n      background: #fff;\n      transform: rotateY(90deg) translateZ(25px);\n    }\n\n    .fsq__face--left-s {\n      background: #fff;\n      transform: rotateX(-90deg) rotateY(-90deg) rotateZ(180deg) translateZ(25px);\n    }\n\n    .fsq__face--top-q {\n      background: #3545f5;\n      transform: rotateX(90deg) translateZ(25px);\n    }\n\n    .fsq__face--bottom-q {\n      background: #3545f5;\n      transform: rotateX(-90deg) translateZ(25px);\n    }\n  </style>\n\n\n  <div class="scene">\n    <div class="fsq">\n      <div class="fsq__face fsq__face--front-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--back-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--right-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--left-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--top-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--bottom-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n    </div>\n  </div>\n</div></div>'), (yield function(e) {
                         let {
                             url: n,
                             namespace: t = "Unfolded.SDK.v1"
                         } = e, a = `${n}::${t}`;
-                        if (void 0 !== h[a]) return h[a];
+                        if (void 0 !== w[a]) return w[a];
                         let r = document.createElement("script");
-                        h[a] = new Promise(((e, a) => {
+                        w[a] = new Promise(((e, a) => {
                             r.onload = () => c(this, null, (function*() {
                                 var r;
                                 let o = null == (r = function(e, n) {
                                     return n.split(".").reduce(((e, n) => {
                                         if (e && "object" == typeof e && n in e) return e[n]
                                     }), e)
                                 }(globalThis, t)) ? void 0 : r.createMap;
                                 o ? e(o) : a(new Error(`Failed to load map interface from ${n}`))
                             })), r.onerror = a
                         })), r.type = "text/javascript", r.src = n;
                         let o = document.querySelector("head");
-                        return null == o || o.appendChild(r), h[a]
+                        return null == o || o.appendChild(r), w[a]
                     }({
                         url: a,
                         namespace: t
                     }))(((e, n) => o(e, i(n)))(((e, n) => {
                         for (var t in n || (n = {})) l.call(n, t) && f(e, t, n[t]);
                         if (s)
                             for (var t of s(n)) d.call(n, t) && f(e, t, n[t]);
                         return e
                     })({}, e), {
                         assetUrl: new URL(a).origin,
-                        apiKeyValidationUrl: "http://localhost:8000/catalog/v1/api-key/validate"
+                        apiKeyValidationUrl: "https://data-api.foursquare.com/catalog/v1/api-key/validate"
                     }))
                 }))
             }
-            var h = {},
-                w = class e extends Error {
+            var w = {},
+                h = class e extends Error {
                     constructor(n) {
                         super(n), Object.setPrototypeOf(this, e.prototype)
                     }
                 };
-            p(w, "invalidApiKey", (() => new w("Map SDK init failed: The supplied API Key is not valid. Please provide a valid API Key."))), p(w, "referrerNotAllowed", (() => new w("Map SDK init failed: This referrer is not allowed for this API Key. Please check the API Key's options for the list of allowed referrers, and update if necessary."))), p(w, "stateUpdateFailure", (() => "State not available. Did you forget to add the map?")), p(w, "alreadyExists", ((e, n) => new w(`Creation failed: ${e} with id '${n}' already exists`))), p(w, "couldNotCreate", (e => new w(`Creation failed: ${e} could not be created`))), p(w, "couldNotUpdate", (e => new w(`Update failed: ${e} could not be updated`))), p(w, "couldNotRemove", (e => new w(`Removal failed: ${e} could not be removed`))), p(w, "notFound", ((e, n) => new w(`Not found: ${e} with id '${n}' not found`))), p(w, "parsingFailed", (e => new w(`Parsing failed: values provided for ${e} are invalid`))), p(w, "unsupported", ((e, n) => new w(`Unsupported feature: ${e} as '${n}'`))), p(w, "datasetFormatUnsupported", (() => "Unsupported data format")), p(w, "datasetFieldNotFound", ((e, n) => new w(`Field with name '${e}' not found for dataset '${n}'`))), p(w, "datasetTypeInvalid", (e => new w(`Invalid type: cannot get data for dataset with type '${e}'`))), p(w, "datasetForFieldNotFound", (e => new w(`No dataset found for field with id '${e}'`))), p(w, "datasetReplaceFailure", (() => "Replace failed: dataset could not be replaced")), p(w, "timelineUpdateFailure", (() => new w("Unable to update layer timeline, one does not exist"))), p(w, "filterTypeInvalid", (() => new w("Filter type invalid: filter type must be time range"))), p(w, "timeFormatInvalid", (() => new w("Time format invalid: time format used internally was invalid"))), p(w, "mapStyleIconNotFound", (() => new w("No default map style icon found"))), p(w, "filterSourceInvalid", (() => new w("No filter source provided"))), p(w, "filterSourcesInvalid", (() => new w("Currently only time-range filters support multiple sources"))), p(w, "identifierInvalid", (() => new w("Invalid identifier: an identifier must be a non-empty string"))), p(w, "custom", (e => new w(e)));
-            var m = w
+            p(h, "invalidApiKey", (() => new h("Map SDK init failed: The supplied API Key is not valid. Please provide a valid API Key."))), p(h, "referrerNotAllowed", (() => new h("Map SDK init failed: This referrer is not allowed for this API Key. Please check the API Key's options for the list of allowed referrers, and update if necessary."))), p(h, "stateUpdateFailure", (() => "State not available. Did you forget to add the map?")), p(h, "alreadyExists", ((e, n) => new h(`Creation failed: ${e} with id '${n}' already exists`))), p(h, "couldNotCreate", (e => new h(`Creation failed: ${e} could not be created`))), p(h, "couldNotUpdate", (e => new h(`Update failed: ${e} could not be updated`))), p(h, "couldNotRemove", (e => new h(`Removal failed: ${e} could not be removed`))), p(h, "notFound", ((e, n) => new h(`Not found: ${e} with id '${n}' not found`))), p(h, "parsingFailed", (e => new h(`Parsing failed: values provided for ${e} are invalid`))), p(h, "unsupported", ((e, n) => new h(`Unsupported feature: ${e} as '${n}'`))), p(h, "datasetFormatUnsupported", (() => "Unsupported data format")), p(h, "datasetFieldNotFound", ((e, n) => new h(`Field with name '${e}' not found for dataset '${n}'`))), p(h, "datasetTypeInvalid", (e => new h(`Invalid type: cannot get data for dataset with type '${e}'`))), p(h, "datasetForFieldNotFound", (e => new h(`No dataset found for field with id '${e}'`))), p(h, "datasetReplaceFailure", (() => "Replace failed: dataset could not be replaced")), p(h, "timelineUpdateFailure", (() => new h("Unable to update layer timeline, one does not exist"))), p(h, "filterTypeInvalid", (() => new h("Filter type invalid: filter type must be time range"))), p(h, "timeFormatInvalid", (() => new h("Time format invalid: time format used internally was invalid"))), p(h, "mapStyleIconNotFound", (() => new h("No default map style icon found"))), p(h, "filterSourceInvalid", (() => new h("No filter source provided"))), p(h, "filterSourcesInvalid", (() => new h("Currently only time-range filters support multiple sources"))), p(h, "identifierInvalid", (() => new h("Invalid identifier: an identifier must be a non-empty string"))), p(h, "custom", (e => new h(e)));
+            var m = h
         }
     }
 ]);
```

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/labextension/static/remoteEntry.56fa1f1cd9ddfb15b82f.js` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/labextension/static/remoteEntry.c8d40a54b33b36dba80c.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, s, f, l, d, c, p, h, v, b, m, g = {
+    var e, r, t, n, o, a, i, u, s, f, l, d, p, c, h, v, b, m, g = {
             148: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
-                        "./extension": () => Promise.all([t.e(377), t.e(480)]).then((() => () => t(480)))
+                        "./extension": () => Promise.all([t.e(398), t.e(480)]).then((() => () => t(480)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
                             var n = t.S.default,
@@ -37,23 +37,23 @@
     }
     w.m = g, w.c = y, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        377: "38a36bf7022c0cbc85dc",
-        480: "8564242f18457c329a6c",
-        568: "678b6de0871522f1ae1f",
-        645: "cf30cf0f2cf9aac000f8"
+        398: "f5b2e6c4d4f58f3b98c1",
+        480: "fda607fe17f5f9c59341",
+        568: "29dd46dc8f97daf4b009",
+        645: "16b1b5e2bfb3ca879bfd"
     } [e] + ".js?v=" + {
-        377: "38a36bf7022c0cbc85dc",
-        480: "8564242f18457c329a6c",
-        568: "678b6de0871522f1ae1f",
-        645: "cf30cf0f2cf9aac000f8"
+        398: "f5b2e6c4d4f58f3b98c1",
+        480: "fda607fe17f5f9c59341",
+        568: "29dd46dc8f97daf4b009",
+        645: "16b1b5e2bfb3ca879bfd"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -67,19 +67,19 @@
                     if (l.getAttribute("src") == t || l.getAttribute("data-webpack") == r + o) {
                         i = l;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(d.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -105,15 +105,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     s = [];
-                return "default" === t && (u("@foursquare/jupyter-map-sdk", "2.0.0", (() => w.e(568).then((() => () => w(568))))), u("@foursquare/map-sdk", "2.0.0", (() => w.e(645).then((() => () => w(106)))))), e[t] = s.length ? Promise.all(s).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@foursquare/jupyter-map-sdk", "2.1.0", (() => w.e(568).then((() => () => w(568))))), u("@foursquare/map-sdk", "2.1.0", (() => w.e(645).then((() => () => w(106)))))), e[t] = s.length ? Promise.all(s).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -183,50 +183,50 @@
                     s = !1, u--
                 } else {
                     if (u <= n || l < d != o) return !1;
                     s = !1
                 } else "s" != d && "n" != d && (s = !1, u--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, i = (e, r) => {
         var t = w.S[e];
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
         return a(n, o) || "undefined" != typeof console && console.warn && console.warn(s(e, t, o, n)), d(e[t][o])
     }, l = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, d = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, n, o) {
+    }, d = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, o) {
         var a = w.I(r);
         return a && a.then ? a.then(e.bind(e, r, w.S[r], t, n, o)) : e(r, w.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), h = c(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), h = p(((e, r, t, n, o) => {
         var a = r && w.o(r, t) && l(r, t, n);
         return a ? d(a) : o()
     })), v = {}, b = {
-        108: () => h("default", "@foursquare/map-sdk", [1, 2, 0, 0], (() => w.e(645).then((() => () => w(106))))),
-        565: () => p("default", "@jupyter-widgets/base", [, [1, 4, 0, 0],
+        178: () => h("default", "@foursquare/map-sdk", [1, 2, 1, 0], (() => w.e(645).then((() => () => w(106))))),
+        565: () => c("default", "@jupyter-widgets/base", [, [1, 4, 0, 0],
             [1, 3, 0, 0],
             [1, 2, 0, 0],
             [1, 1, 1, 10], 1, 1, 1
         ])
     }, m = {
-        377: [108, 565],
-        568: [108, 565]
+        398: [178, 565],
+        568: [178, 565]
     }, w.f.consumes = (e, r) => {
         w.o(m, e) && m[e].forEach((e => {
             if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
@@ -247,15 +247,15 @@
         var e = {
             309: 0
         };
         w.f.j = (r, t) => {
             var n = w.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (377 != r) {
+                else if (398 != r) {
                 var o = new Promise(((t, o) => n = e[r] = [t, o]));
                 t.push(n[2] = o);
                 var a = w.p + w.u(r),
                     i = new Error;
                 w.l(a, (t => {
                     if (w.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                         var o = t && ("load" === t.type ? "missing" : t.type),
```

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/labextension/static/third-party-licenses.json` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/labextension/static/third-party-licenses.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '2.1.0'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "SEE LICENSE IN LICENSE.txt",
             "name": "@foursquare/map-sdk",
-            "versionInfo": "2.0.0"
+            "versionInfo": "2.1.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "3.6.0"
         },
```

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/map/base.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/map/base.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/map/html.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/map/html.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/map/widget.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/map/widget.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/nbextension/index.js` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/nbextension/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -43,15 +43,15 @@
                         o((n = n.apply(e, t)).next())
                     })),
                     f = ["legend", "toggle-3d", "split-map", "map-draw", "chart", "annotation", "viewport-json", "effect"],
                     _ = ((a = _ || {}).REMOVE_DATASET = "remove-dataset", a.ADD_LAYER = "add-layer", a.REMOVE_LAYER = "remove-layer", a.ADD_LAYER_GROUP = "add-layer-group", a.REMOVE_LAYER_GROUP = "remove-layer-group", a.ACTIVATE_MAP_CONTROL = "activate-map-control", a.CHANGE_SIDE_PANEL_SECTION = "change-side-panel-section", a.API_KEY_GENERATED_STARTED = "API Key Generated Started", a.API_KEY_GENERATED = "API Key Generated", a.COPY_API_KEY = "Copy API Key", a);
 
                 function E(e, t) {
                     return u(this, null, (function*() {
-                        let n, a = "http://localhost:8080/studio-bundle.js";
+                        let n, a = "https://studio.foursquare.com/studio-bundle.js";
                         (function(e) {
                             return "object" == typeof e && null !== e && "url" in e && "string" == typeof e.url && ("string" == typeof e.namespace || void 0 === e.namespace)
                         })(t) && (a = t.url, n = t.namespace);
                         let {
                             showPlaceholder: i = !0
                         } = e;
                         return e.container && i && (e.container.innerHTML = '<div style="position:relative;width:100%;height:100%;"><div class="map-placeholder">\n  <style>\n    .map-placeholder {\n      position: absolute;\n      top: 0;\n      left: 0;\n      right: 0;\n      width: 100%;\n      height: 100%;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .scene {\n      width: 50px;\n      height: 50px;\n      transform-style: preserve-3d;\n      transform: rotateY(0deg) rotateX(56deg) rotateZ(-45deg);\n    }\n\n    @keyframes fsq-rotate {\n      0% {\n        transform: rotateY(0deg);\n      }\n      5%, 25% {\n        transform: rotateX(-90deg);\n      }\n      30%, 50% {\n        transform: rotateX(-90deg) rotateY(-90deg);\n      }\n      55%, 75% {\n        transform: rotateX(-90deg) rotateY(-90deg) rotateX(-90deg);\n      }\n      80%, 100% {\n        transform: rotateX(-90deg) rotateY(0deg) rotateX(-90deg);\n      }\n    }\n\n    .fsq {\n      width: 50px;\n      height: 50px;\n      position: relative;\n      transform-style: preserve-3d;\n      transition: transform 1s;\n      animation-name: fsq-rotate;\n      animation-iteration-count: infinite;\n      animation-duration: 6s;\n      animation-timing-function: ease;\n    }\n\n    .fsq__face {\n      position: absolute;\n      width: 50px;\n      height: 50px;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .fsq__face--front-f {\n      background: #000;\n      transform: rotateY(0deg) translateZ(25px);\n    }\n\n    .fsq__face--back-f {\n      background: #000;\n      transform: rotateZ(-180deg) rotateY(180deg) translateZ(25px);\n    }\n\n    .fsq__face--right-s {\n      background: #fff;\n      transform: rotateY(90deg) translateZ(25px);\n    }\n\n    .fsq__face--left-s {\n      background: #fff;\n      transform: rotateX(-90deg) rotateY(-90deg) rotateZ(180deg) translateZ(25px);\n    }\n\n    .fsq__face--top-q {\n      background: #3545f5;\n      transform: rotateX(90deg) translateZ(25px);\n    }\n\n    .fsq__face--bottom-q {\n      background: #3545f5;\n      transform: rotateX(-90deg) translateZ(25px);\n    }\n  </style>\n\n\n  <div class="scene">\n    <div class="fsq">\n      <div class="fsq__face fsq__face--front-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--back-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--right-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--left-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--top-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--bottom-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n    </div>\n  </div>\n</div></div>'), (yield function(e) {
@@ -80,15 +80,15 @@
                         }))(((e, t) => r(e, s(t)))(((e, t) => {
                             for (var n in t || (t = {})) d.call(t, n) && c(e, n, t[n]);
                             if (o)
                                 for (var n of o(t)) l.call(t, n) && c(e, n, t[n]);
                             return e
                         })({}, e), {
                             assetUrl: new URL(a).origin,
-                            apiKeyValidationUrl: "http://localhost:8000/catalog/v1/api-key/validate"
+                            apiKeyValidationUrl: "https://data-api.foursquare.com/catalog/v1/api-key/validate"
                         }))
                     }))
                 }
                 var m = {},
                     v = class e extends Error {
                         constructor(t) {
                             super(t), Object.setPrototypeOf(this, e.prototype)
@@ -643,15 +643,15 @@
             },
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"@foursquare/jupyter-map-sdk","version":"2.0.0","description":"JavaScript bindings for Foursquare\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css","LICENSE.txt"],"license":"SEE LICENSE IN LICENSE.txt","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf foursquare/map_sdk/labextension","clean:nbextension":"rimraf \'foursquare/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@foursquare/map-sdk":"^2.0.0","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","aws-sdk":"^2.988.0","csstype":"^3.1.0"},"devDependencies":{"@babel/preset-env":"^7.21.4","@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"foursquare/map_sdk/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+                e.exports = JSON.parse('{"name":"@foursquare/jupyter-map-sdk","version":"2.1.0","description":"JavaScript bindings for Foursquare\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css","LICENSE.txt"],"license":"SEE LICENSE IN LICENSE.txt","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf foursquare/map_sdk/labextension","clean:nbextension":"rimraf \'foursquare/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@foursquare/map-sdk":"^2.1.0","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","aws-sdk":"^2.988.0","csstype":"^3.1.0"},"devDependencies":{"@babel/preset-env":"^7.21.4","@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"foursquare/map_sdk/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
             }
         },
         n = {};
 
     function a(e) {
         var i = n[e];
         if (void 0 !== i) return i.exports;
```

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/poll.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/poll.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/templates/html_map_sdk.j2` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/templates/html_map_sdk.j2`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/transfer_utils.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/transfer_utils.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/transport/base.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/transport/base.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/transport/html.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/transport/html.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/transport/widget.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/transport/widget.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/types.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/types.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/utils/action_type_mapping.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/utils/action_type_mapping.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/utils/serialization.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare/map_sdk/utils/validators.py` & `foursquare.map-sdk-2.1.0/foursquare/map_sdk/utils/validators.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/foursquare.map_sdk.egg-info/PKG-INFO` & `foursquare.map-sdk-2.1.0/foursquare.map_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursquare.map-sdk
-Version: 2.0.0
+Version: 2.1.0
 Summary: Jupyter Widget for Foursquare Studio Maps
 Author: Foursquare Labs
 Author-email: info-studio@foursquare.com
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
```

### Comparing `foursquare.map-sdk-2.0.0/foursquare.map_sdk.egg-info/SOURCES.txt` & `foursquare.map-sdk-2.1.0/foursquare.map_sdk.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -37,28 +37,45 @@
 foursquare/map_sdk/api/dataset_api.py
 foursquare/map_sdk/api/effect_api.py
 foursquare/map_sdk/api/enums.py
 foursquare/map_sdk/api/event_api.py
 foursquare/map_sdk/api/filter_api.py
 foursquare/map_sdk/api/layer_api.py
 foursquare/map_sdk/api/map_api.py
+foursquare/map_sdk/api/experimental/__init__.py
+foursquare/map_sdk/api/experimental/_utils.py
+foursquare/map_sdk/api/experimental/color.py
+foursquare/map_sdk/api/experimental/columns.py
+foursquare/map_sdk/api/experimental/text_label.py
+foursquare/map_sdk/api/experimental/layer/__init__.py
+foursquare/map_sdk/api/experimental/layer/arc.py
+foursquare/map_sdk/api/experimental/layer/flow.py
+foursquare/map_sdk/api/experimental/layer/grid.py
+foursquare/map_sdk/api/experimental/layer/h3.py
+foursquare/map_sdk/api/experimental/layer/hexbin.py
+foursquare/map_sdk/api/experimental/layer/icon.py
+foursquare/map_sdk/api/experimental/layer/line.py
+foursquare/map_sdk/api/experimental/layer/point.py
+foursquare/map_sdk/api/experimental/layer/polygon.py
+foursquare/map_sdk/api/experimental/layer/threed.py
+foursquare/map_sdk/api/experimental/layer/trip.py
 foursquare/map_sdk/generated/Animation.py
 foursquare/map_sdk/generated/Annotation.py
 foursquare/map_sdk/generated/Chart.py
 foursquare/map_sdk/generated/CustomMapState.py
 foursquare/map_sdk/generated/Effect.py
 foursquare/map_sdk/generated/Filter.py
 foursquare/map_sdk/generated/FilterAnimation.py
 foursquare/map_sdk/generated/Layer.py
 foursquare/map_sdk/generated/MapState.py
 foursquare/map_sdk/labextension/package.json
-foursquare/map_sdk/labextension/static/480.8564242f18457c329a6c.js
-foursquare/map_sdk/labextension/static/568.678b6de0871522f1ae1f.js
-foursquare/map_sdk/labextension/static/645.cf30cf0f2cf9aac000f8.js
-foursquare/map_sdk/labextension/static/remoteEntry.56fa1f1cd9ddfb15b82f.js
+foursquare/map_sdk/labextension/static/480.fda607fe17f5f9c59341.js
+foursquare/map_sdk/labextension/static/568.29dd46dc8f97daf4b009.js
+foursquare/map_sdk/labextension/static/645.16b1b5e2bfb3ca879bfd.js
+foursquare/map_sdk/labextension/static/remoteEntry.c8d40a54b33b36dba80c.js
 foursquare/map_sdk/labextension/static/style.js
 foursquare/map_sdk/labextension/static/third-party-licenses.json
 foursquare/map_sdk/map/__init__.py
 foursquare/map_sdk/map/base.py
 foursquare/map_sdk/map/html.py
 foursquare/map_sdk/map/widget.py
 foursquare/map_sdk/nbextension/extension.js
@@ -73,14 +90,15 @@
 foursquare/map_sdk/utils/serialization.py
 foursquare/map_sdk/utils/validators.py
 scripts/rename_package.py
 tests/__init__.py
 tests/_utils.py
 tests/conftest.py
 tests/test_html_map.py
+tests/test_layers_conversion.py
 tests/test_nbextension_path.py
 tests/test_serialization.py
 tests/test_subclass.py
 tests/test_widget_map.py
 tests/api/test_dataset_api.py
 tests/api/test_effect_api.py
 tests/api/test_filter_api.py
```

### Comparing `foursquare.map-sdk-2.0.0/package.json` & `foursquare.map-sdk-2.1.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.961734693877551%*

 * *Differences: {"'dependencies'": "{'@foursquare/map-sdk': '^2.1.0'}", "'version'": "'2.1.0'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": {
         "email": "info-studio@foursquare.com",
         "name": "Foursquare Labs"
     },
     "dependencies": {
         "@aws-amplify/core": "^4.2.9",
-        "@foursquare/map-sdk": "^2.0.0",
+        "@foursquare/map-sdk": "^2.1.0",
         "@jupyter-widgets/base": "^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0",
         "@lumino/application": "^1.16.0",
         "@lumino/widgets": "^1.30.0",
         "aws-sdk": "^2.988.0",
         "csstype": "^3.1.0"
     },
     "description": "JavaScript bindings for Foursquare's Jupyter Map SDK",
@@ -75,12 +75,12 @@
         "typecheck": "tsc",
         "typescript": "yarn run -T tsc --noEmit",
         "watch": "npm-run-all -p watch:*",
         "watch:lib": "yarn run -T tsc -w",
         "watch:nbextension": "webpack --watch --mode development"
     },
     "types": "lib/index.d.ts",
-    "version": "2.0.0",
+    "version": "2.1.0",
     "volta": {
         "extends": "../../../package.json"
     }
 }
```

### Comparing `foursquare.map-sdk-2.0.0/scripts/rename_package.py` & `foursquare.map-sdk-2.1.0/scripts/rename_package.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/setup.cfg` & `foursquare.map-sdk-2.1.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.0.0
+current_version = 2.1.0
 commit = True
 message = chore(map-sdk): Bump version {current_version} → {new_version}
 tag = False
 tag_name = map-sdk/{new_version}
 
 [bdist_wheel]
 universal = 1
```

### Comparing `foursquare.map-sdk-2.0.0/setup.py` & `foursquare.map-sdk-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         "pydantic==2.6.3",
         "traitlets",
         "jupyterlab-widgets<=1.1.2",
         # pin this version until we fix it for newer versions
         "jupyterlab==3.2.9",
         # pin this version until we fix it for newer versions
         "jupyter-server==1.24.*",
+        "glom==23.5.0",
         "",
     ],
     extras_require={
         "test": [
             "pytest<8.1",
             "pytest-cov",
             "pytest-snapshot",
```

### Comparing `foursquare.map-sdk-2.0.0/tests/_utils.py` & `foursquare.map-sdk-2.1.0/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/api/test_dataset_api.py` & `foursquare.map-sdk-2.1.0/tests/api/test_dataset_api.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/api/test_effect_api.py` & `foursquare.map-sdk-2.1.0/tests/api/test_effect_api.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/api/test_filter_api.py` & `foursquare.map-sdk-2.1.0/tests/api/test_filter_api.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/api/test_layer_api.py` & `foursquare.map-sdk-2.1.0/tests/api/test_layer_api.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/api/test_map_api.py` & `foursquare.map-sdk-2.1.0/tests/api/test_map_api.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/conftest.py` & `foursquare.map-sdk-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/fixtures/dataset_api.py` & `foursquare.map-sdk-2.1.0/tests/fixtures/dataset_api.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json` & `foursquare.map-sdk-2.1.0/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/fixtures/raster/item/sentinel-2-l2a.json` & `foursquare.map-sdk-2.1.0/tests/fixtures/raster/item/sentinel-2-l2a.json`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/fixtures/test_data.py` & `foursquare.map-sdk-2.1.0/tests/fixtures/test_data.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/mocks/transport.py` & `foursquare.map-sdk-2.1.0/tests/mocks/transport.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html` & `foursquare.map-sdk-2.1.0/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/snapshots/test_html_map/test_template_rendering/map.html` & `foursquare.map-sdk-2.1.0/tests/snapshots/test_html_map/test_template_rendering/map.html`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/test_html_map.py` & `foursquare.map-sdk-2.1.0/tests/test_html_map.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/test_serialization.py` & `foursquare.map-sdk-2.1.0/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/test_subclass.py` & `foursquare.map-sdk-2.1.0/tests/test_subclass.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/test_widget_map.py` & `foursquare.map-sdk-2.1.0/tests/test_widget_map.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tests/utils/test_validators.py` & `foursquare.map-sdk-2.1.0/tests/utils/test_validators.py`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/tsconfig.json` & `foursquare.map-sdk-2.1.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `foursquare.map-sdk-2.0.0/webpack.config.js` & `foursquare.map-sdk-2.1.0/webpack.config.js`

 * *Files identical despite different names*

