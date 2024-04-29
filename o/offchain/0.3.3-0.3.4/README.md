# Comparing `tmp/offchain-0.3.3.tar.gz` & `tmp/offchain-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offchain-0.3.3.tar", max compression
+gzip compressed data, was "offchain-0.3.4.tar", max compression
```

## Comparing `offchain-0.3.3.tar` & `offchain-0.3.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1066 2024-04-26 01:20:28.512962 offchain-0.3.3/LICENSE
--rw-r--r--   0        0        0     2805 2024-04-26 01:20:28.512962 offchain-0.3.3/README.md
--rw-r--r--   0        0        0      193 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/base/__init__.py
--rw-r--r--   0        0        0       45 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/base/base_model.py
--rw-r--r--   0        0        0      486 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/base/types.py
--rw-r--r--   0        0        0     1891 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/concurrency.py
--rw-r--r--   0        0        0        0 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/constants/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/constants/addresses.py
--rw-r--r--   0        0        0      183 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/constants/providers.py
--rw-r--r--   0        0        0        0 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/logger/__init__.py
--rw-r--r--   0        0        0      417 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/logger/logging.py
--rw-r--r--   0        0        0      217 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/__init__.py
--rw-r--r--   0        0        0      264 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/adapters/__init__.py
--rw-r--r--   0        0        0     3627 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/adapters/arweave.py
--rw-r--r--   0        0        0     3084 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/adapters/base_adapter.py
--rw-r--r--   0        0        0     3292 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/adapters/data_uri.py
--rw-r--r--   0        0        0     1190 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/adapters/default_adapter_configs.py
--rw-r--r--   0        0        0      317 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/adapters/http_adapter.py
--rw-r--r--   0        0        0     5046 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/adapters/ipfs.py
--rw-r--r--   0        0        0        0 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/constants/__init__.py
--rw-r--r--   0        0        0      359 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/constants/autoglyphs.py
--rw-r--r--   0        0        0     7181 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/constants/nouns.py
--rw-r--r--   0        0        0       84 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/fetchers/__init__.py
--rw-r--r--   0        0        0     2796 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/fetchers/base_fetcher.py
--rw-r--r--   0        0        0     7430 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/fetchers/metadata_fetcher.py
--rw-r--r--   0        0        0      642 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/get_token_metadata.py
--rw-r--r--   0        0        0      225 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/models/__init__.py
--rw-r--r--   0        0        0     3572 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/models/metadata.py
--rw-r--r--   0        0        0      844 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/models/metadata_processing_error.py
--rw-r--r--   0        0        0     1139 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/models/token.py
--rw-r--r--   0        0        0      867 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/parsers/__init__.py
--rw-r--r--   0        0        0     3168 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/parsers/catchall/__init__.py
--rw-r--r--   0        0        0      628 2024-04-26 01:20:28.512962 offchain-0.3.3/offchain/metadata/parsers/catchall/catchall_parser.py
--rw-r--r--   0        0        0    10166 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/catchall/default_catchall.py
--rw-r--r--   0        0        0        0 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/collection/__init__.py
--rw-r--r--   0        0        0    12266 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/collection/artblocks.py
--rw-r--r--   0        0        0     8386 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/collection/autoglyphs.py
--rw-r--r--   0        0        0     2786 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/collection/chainrunners.py
--rw-r--r--   0        0        0     2112 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/collection/collection_parser.py
--rw-r--r--   0        0        0     3875 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/collection/decentraland.py
--rw-r--r--   0        0        0     7619 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/collection/ens.py
--rw-r--r--   0        0        0     2769 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/collection/foundation.py
--rw-r--r--   0        0        0     5651 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/collection/hashmasks.py
--rw-r--r--   0        0        0     6284 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/collection/loot.py
--rw-r--r--   0        0        0     5314 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/collection/makersplace.py
--rw-r--r--   0        0        0     7188 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/collection/nouns.py
--rw-r--r--   0        0        0     6495 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/collection/punks.py
--rw-r--r--   0        0        0     6921 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/collection/superrare.py
--rw-r--r--   0        0        0     6143 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/collection/zora.py
--rw-r--r--   0        0        0        0 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/schema/__init__.py
--rw-r--r--   0        0        0     8197 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/schema/opensea.py
--rw-r--r--   0        0        0      713 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/parsers/schema/schema_parser.py
--rw-r--r--   0        0        0       88 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/pipelines/__init__.py
--rw-r--r--   0        0        0      248 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/pipelines/base_pipeline.py
--rw-r--r--   0        0        0    15052 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/pipelines/metadata_pipeline.py
--rw-r--r--   0        0        0        0 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/registries/__init__.py
--rw-r--r--   0        0        0     1043 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/registries/adapter_registry.py
--rw-r--r--   0        0        0     1577 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/registries/base_registry.py
--rw-r--r--   0        0        0      907 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/registries/fetcher_registry.py
--rw-r--r--   0        0        0     2661 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/metadata/registries/parser_registry.py
--rw-r--r--   0        0        0     1350 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/utils/utils.py
--rw-r--r--   0        0        0        0 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/web3/__init__.py
--rw-r--r--   0        0        0     7277 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/web3/contract_caller.py
--rw-r--r--   0        0        0      531 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/web3/contract_utils.py
--rw-r--r--   0        0        0     3671 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/web3/jsonrpc.py
--rw-r--r--   0        0        0     9440 2024-04-26 01:20:28.516962 offchain-0.3.3/offchain/web3/read_async.py
--rw-r--r--   0        0        0      920 2024-04-26 01:20:28.516962 offchain-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 offchain-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-29 15:58:16.226318 offchain-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2805 2024-04-29 15:58:16.226318 offchain-0.3.4/README.md
+-rw-r--r--   0        0        0      193 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/base/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/base/base_model.py
+-rw-r--r--   0        0        0      486 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/base/types.py
+-rw-r--r--   0        0        0     1891 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/concurrency.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/constants/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/constants/addresses.py
+-rw-r--r--   0        0        0      183 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/constants/providers.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/logger/__init__.py
+-rw-r--r--   0        0        0      417 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/logger/logging.py
+-rw-r--r--   0        0        0      217 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/__init__.py
+-rw-r--r--   0        0        0      264 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/adapters/__init__.py
+-rw-r--r--   0        0        0     3627 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/adapters/arweave.py
+-rw-r--r--   0        0        0     3084 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/adapters/base_adapter.py
+-rw-r--r--   0        0        0     3292 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/adapters/data_uri.py
+-rw-r--r--   0        0        0     1190 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/adapters/default_adapter_configs.py
+-rw-r--r--   0        0        0      317 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/adapters/http_adapter.py
+-rw-r--r--   0        0        0     5046 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/adapters/ipfs.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/constants/__init__.py
+-rw-r--r--   0        0        0      359 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/constants/autoglyphs.py
+-rw-r--r--   0        0        0     7181 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/constants/nouns.py
+-rw-r--r--   0        0        0       84 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/fetchers/__init__.py
+-rw-r--r--   0        0        0     2796 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/fetchers/base_fetcher.py
+-rw-r--r--   0        0        0     7430 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/fetchers/metadata_fetcher.py
+-rw-r--r--   0        0        0      642 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/get_token_metadata.py
+-rw-r--r--   0        0        0      225 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/models/__init__.py
+-rw-r--r--   0        0        0     3572 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/models/metadata.py
+-rw-r--r--   0        0        0      844 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/models/metadata_processing_error.py
+-rw-r--r--   0        0        0     1139 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/models/token.py
+-rw-r--r--   0        0        0      867 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/__init__.py
+-rw-r--r--   0        0        0     3168 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/catchall/__init__.py
+-rw-r--r--   0        0        0      628 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/catchall/catchall_parser.py
+-rw-r--r--   0        0        0    10166 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/catchall/default_catchall.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/collection/__init__.py
+-rw-r--r--   0        0        0    12266 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/collection/artblocks.py
+-rw-r--r--   0        0        0     8386 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/collection/autoglyphs.py
+-rw-r--r--   0        0        0     2786 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/collection/chainrunners.py
+-rw-r--r--   0        0        0     2112 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/collection/collection_parser.py
+-rw-r--r--   0        0        0     3875 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/collection/decentraland.py
+-rw-r--r--   0        0        0     7619 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/collection/ens.py
+-rw-r--r--   0        0        0     2769 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/collection/foundation.py
+-rw-r--r--   0        0        0     5651 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/collection/hashmasks.py
+-rw-r--r--   0        0        0     6284 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/collection/loot.py
+-rw-r--r--   0        0        0     5314 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/collection/makersplace.py
+-rw-r--r--   0        0        0     7989 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/collection/nouns.py
+-rw-r--r--   0        0        0     6495 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/collection/punks.py
+-rw-r--r--   0        0        0     6921 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/collection/superrare.py
+-rw-r--r--   0        0        0     6143 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/collection/zora.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/schema/__init__.py
+-rw-r--r--   0        0        0     8197 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/schema/opensea.py
+-rw-r--r--   0        0        0      713 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/parsers/schema/schema_parser.py
+-rw-r--r--   0        0        0       88 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/pipelines/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/pipelines/base_pipeline.py
+-rw-r--r--   0        0        0    15052 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/pipelines/metadata_pipeline.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/registries/__init__.py
+-rw-r--r--   0        0        0     1043 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/registries/adapter_registry.py
+-rw-r--r--   0        0        0     1577 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/registries/base_registry.py
+-rw-r--r--   0        0        0      907 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/registries/fetcher_registry.py
+-rw-r--r--   0        0        0     2661 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/metadata/registries/parser_registry.py
+-rw-r--r--   0        0        0     1350 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/utils/utils.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/web3/__init__.py
+-rw-r--r--   0        0        0     7277 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/web3/contract_caller.py
+-rw-r--r--   0        0        0      531 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/web3/contract_utils.py
+-rw-r--r--   0        0        0     3671 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/web3/jsonrpc.py
+-rw-r--r--   0        0        0     9440 2024-04-29 15:58:16.226318 offchain-0.3.4/offchain/web3/read_async.py
+-rw-r--r--   0        0        0      920 2024-04-29 15:58:16.230318 offchain-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 offchain-0.3.4/PKG-INFO
```

### Comparing `offchain-0.3.3/LICENSE` & `offchain-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/README.md` & `offchain-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/concurrency.py` & `offchain-0.3.4/offchain/concurrency.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/constants/addresses.py` & `offchain-0.3.4/offchain/constants/addresses.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/adapters/arweave.py` & `offchain-0.3.4/offchain/metadata/adapters/arweave.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/adapters/base_adapter.py` & `offchain-0.3.4/offchain/metadata/adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/adapters/data_uri.py` & `offchain-0.3.4/offchain/metadata/adapters/data_uri.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/adapters/default_adapter_configs.py` & `offchain-0.3.4/offchain/metadata/adapters/default_adapter_configs.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/adapters/ipfs.py` & `offchain-0.3.4/offchain/metadata/adapters/ipfs.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/constants/nouns.py` & `offchain-0.3.4/offchain/metadata/constants/nouns.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/fetchers/base_fetcher.py` & `offchain-0.3.4/offchain/metadata/fetchers/base_fetcher.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/fetchers/metadata_fetcher.py` & `offchain-0.3.4/offchain/metadata/fetchers/metadata_fetcher.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/get_token_metadata.py` & `offchain-0.3.4/offchain/metadata/get_token_metadata.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/models/metadata.py` & `offchain-0.3.4/offchain/metadata/models/metadata.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/models/metadata_processing_error.py` & `offchain-0.3.4/offchain/metadata/models/metadata_processing_error.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/models/token.py` & `offchain-0.3.4/offchain/metadata/models/token.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/__init__.py` & `offchain-0.3.4/offchain/metadata/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/base_parser.py` & `offchain-0.3.4/offchain/metadata/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/catchall/catchall_parser.py` & `offchain-0.3.4/offchain/metadata/parsers/catchall/catchall_parser.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/catchall/default_catchall.py` & `offchain-0.3.4/offchain/metadata/parsers/catchall/default_catchall.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/collection/artblocks.py` & `offchain-0.3.4/offchain/metadata/parsers/collection/artblocks.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/collection/autoglyphs.py` & `offchain-0.3.4/offchain/metadata/parsers/collection/autoglyphs.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/collection/chainrunners.py` & `offchain-0.3.4/offchain/metadata/parsers/collection/chainrunners.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/collection/collection_parser.py` & `offchain-0.3.4/offchain/metadata/parsers/collection/collection_parser.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/collection/decentraland.py` & `offchain-0.3.4/offchain/metadata/parsers/collection/decentraland.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/collection/ens.py` & `offchain-0.3.4/offchain/metadata/parsers/collection/ens.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/collection/foundation.py` & `offchain-0.3.4/offchain/metadata/parsers/collection/foundation.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/collection/hashmasks.py` & `offchain-0.3.4/offchain/metadata/parsers/collection/hashmasks.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/collection/loot.py` & `offchain-0.3.4/offchain/metadata/parsers/collection/loot.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/collection/makersplace.py` & `offchain-0.3.4/offchain/metadata/parsers/collection/makersplace.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/collection/nouns.py` & `offchain-0.3.4/offchain/metadata/parsers/collection/nouns.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
 from dataclasses import dataclass
 from typing import Optional
-from urllib.parse import quote
 
 from offchain.constants.addresses import CollectionAddress
 from offchain.metadata.constants.nouns import ACCESSORY, BACKGROUND, BODY, GLASSES, HEAD
 from offchain.metadata.models.metadata import Attribute, MediaDetails, Metadata
 from offchain.metadata.models.token import Token
 from offchain.metadata.parsers.collection.collection_parser import CollectionParser
 from offchain.metadata.registries.parser_registry import ParserRegistry
@@ -24,44 +23,67 @@
         cls,
         background_index: int,
         body_index: int,
         accessory_index: int,
         head_index: int,
         glasses_index: int,
     ):
-        background = BACKGROUND[background_index]
-        body = BODY[body_index]
-        accessory = ACCESSORY[accessory_index]
-        head = HEAD[head_index]
-        glasses = GLASSES[glasses_index]
+        # indexes here come from contract calls and can be out of bounds
+        background = (
+            BACKGROUND[background_index]
+            if 0 <= background_index < len(BACKGROUND)
+            else f"unknown({background_index})"
+        )
+        body = (
+            BODY[body_index]
+            if 0 <= body_index < len(BODY)
+            else f"unknown({body_index})"
+        )
+        accessory = (
+            ACCESSORY[accessory_index]
+            if 0 <= accessory_index < len(ACCESSORY)
+            else f"unknown({accessory_index})"
+        )
+        head = (
+            HEAD[head_index]
+            if 0 <= head_index < len(HEAD)
+            else f"unknown({head_index})"
+        )
+        glasses = (
+            GLASSES[glasses_index]
+            if 0 <= glasses_index < len(GLASSES)
+            else f"unknown({glasses_index})"
+        )
 
         return Seeds(background, body, accessory, head, glasses)
 
 
 @ParserRegistry.register
 class NounsParser(CollectionParser):
     _COLLECTION_ADDRESSES: list[str] = [
         CollectionAddress.NOUNS,
         CollectionAddress.LIL_NOUNS,
     ]
 
     def get_image(self, raw_data: dict) -> Optional[MediaDetails]:  # type: ignore[type-arg]  # noqa: E501
         raw_image_uri = raw_data.get("image")
-        image_uri = quote(self.fetcher.fetch_content(raw_image_uri))  # type: ignore[arg-type]  # noqa: E501
+        mime_type, size = self.fetcher.fetch_mime_type_and_size(raw_image_uri)  # type: ignore[arg-type]
+        image_uri = raw_image_uri
 
         return MediaDetails(
-            uri=image_uri, size=None, sha256=None, mime_type="image/svg+xml"
+            uri=image_uri, size=size, sha256=None, mime_type="image/svg+xml"
         )  # noqa: E501
 
     async def gen_image(self, raw_data: dict) -> Optional[MediaDetails]:  # type: ignore[type-arg]  # noqa: E501
         raw_image_uri = raw_data.get("image")
-        image_uri = quote(await self.fetcher.gen_fetch_content(raw_image_uri))  # type: ignore[arg-type]  # noqa: E501
+        mime_type, size = await self.fetcher.gen_fetch_mime_type_and_size(raw_image_uri)  # type: ignore[arg-type]
+        image_uri = raw_image_uri
 
         return MediaDetails(
-            uri=image_uri, size=None, sha256=None, mime_type="image/svg+xml"
+            uri=image_uri, size=size, sha256=None, mime_type="image/svg+xml"
         )  # noqa: E501
 
     def seeds(self, token: Token) -> Optional[Seeds]:
         results = self.contract_caller.single_address_single_fn_many_args(
             address=token.collection_address,
             function_sig="seeds(uint256)",
             return_type=["uint48", "uint48", "uint48", "uint48", "uint48"],
@@ -161,38 +183,44 @@
                 value=normalize_value(value),
                 display_type=None,
             )
             for trait, value in seeds.__dict__.items()
         ]
 
     def parse_metadata(self, token: Token, raw_data: dict, *args, **kwargs) -> Metadata:  # type: ignore[no-untyped-def, type-arg]  # noqa: E501
-        token.uri = self.get_uri(token)
+        if token.uri is None:
+            token.uri = self.get_uri(token)
 
-        raw_data = self.fetcher.fetch_content(token.uri)  # type: ignore[arg-type, assignment]  # noqa: E501
+        if not isinstance(raw_data, dict):
+            raw_data = self.fetcher.fetch_content(token.uri)  # type: ignore[arg-type, assignment]  # noqa: E501
         mime_type, _ = self.fetcher.fetch_mime_type_and_size(token.uri)  # type: ignore[arg-type]  # noqa: E501
 
         return Metadata(
             token=token,
             raw_data=raw_data,
             name=raw_data.get("name"),
             description=raw_data.get("description"),
             mime_type=mime_type,
             image=self.get_image(raw_data),
             attributes=self.get_seed_attributes(token),
         )
 
     async def _gen_parse_metadata_impl(self, token: Token, raw_data: dict, *args, **kwargs) -> Metadata:  # type: ignore[no-untyped-def, type-arg]  # noqa: E501
-        token.uri = await self.gen_uri(token)
+        if token.uri is None:
+            token.uri = await self.gen_uri(token)
+
+        if not isinstance(raw_data, dict):
+            raw_data = await self.fetcher.gen_fetch_content(token.uri)
 
-        raw_data, mime_type_and_size, attributes = await asyncio.gather(
-            self.fetcher.gen_fetch_content(token.uri),  # type: ignore[arg-type, assignment]  # noqa: E501
+        mime_type_and_size, attributes, image = await asyncio.gather(
             self.fetcher.gen_fetch_mime_type_and_size(token.uri),  # type: ignore[arg-type]  # noqa: E501
             self.gen_seed_attributes(token),
+            self.gen_image(raw_data),
         )
-        image = await self.gen_image(raw_data)
+
         mime_type, _ = mime_type_and_size
 
         return Metadata(
             token=token,
             raw_data=raw_data,
             name=raw_data.get("name"),
             description=raw_data.get("description"),
```

### Comparing `offchain-0.3.3/offchain/metadata/parsers/collection/punks.py` & `offchain-0.3.4/offchain/metadata/parsers/collection/punks.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/collection/superrare.py` & `offchain-0.3.4/offchain/metadata/parsers/collection/superrare.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/collection/zora.py` & `offchain-0.3.4/offchain/metadata/parsers/collection/zora.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/schema/opensea.py` & `offchain-0.3.4/offchain/metadata/parsers/schema/opensea.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/parsers/schema/schema_parser.py` & `offchain-0.3.4/offchain/metadata/parsers/schema/schema_parser.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/pipelines/metadata_pipeline.py` & `offchain-0.3.4/offchain/metadata/pipelines/metadata_pipeline.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/registries/adapter_registry.py` & `offchain-0.3.4/offchain/metadata/registries/adapter_registry.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/registries/base_registry.py` & `offchain-0.3.4/offchain/metadata/registries/base_registry.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/registries/fetcher_registry.py` & `offchain-0.3.4/offchain/metadata/registries/fetcher_registry.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/metadata/registries/parser_registry.py` & `offchain-0.3.4/offchain/metadata/registries/parser_registry.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/utils/utils.py` & `offchain-0.3.4/offchain/utils/utils.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/web3/contract_caller.py` & `offchain-0.3.4/offchain/web3/contract_caller.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/web3/contract_utils.py` & `offchain-0.3.4/offchain/web3/contract_utils.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/web3/jsonrpc.py` & `offchain-0.3.4/offchain/web3/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/offchain/web3/read_async.py` & `offchain-0.3.4/offchain/web3/read_async.py`

 * *Files identical despite different names*

### Comparing `offchain-0.3.3/pyproject.toml` & `offchain-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "offchain"
-version = "0.3.3"
+version = "0.3.4"
 description = "Open source metadata processing framework"
 authors = ["Zora eng <eng@zora.co>"]
 readme = "README.md"
 documentation = "https://ourzora.github.io/offchain"
 
 [tool.poetry.dependencies]
 python = ">=3.9 <4"
```

### Comparing `offchain-0.3.3/PKG-INFO` & `offchain-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offchain
-Version: 0.3.3
+Version: 0.3.4
 Summary: Open source metadata processing framework
 Author: Zora eng
 Author-email: eng@zora.co
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

