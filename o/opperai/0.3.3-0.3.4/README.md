# Comparing `tmp/opperai-0.3.3.tar.gz` & `tmp/opperai-0.3.4.tar.gz`

## Comparing `opperai-0.3.3.tar` & `opperai-0.3.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.3.3/pytest.ini
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.3.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/__init__.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/_client.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/_http_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/functions/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/functions/_async_functions.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/functions/_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/functions/decorator/__init__.py
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/functions/decorator/_decorator.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/functions/decorator/_schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/indexes/__init__.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/indexes/_async_indexes.py
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/indexes/_indexes.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/spans/__init__.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/spans/_async_spans.py
--rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/spans/_decorator.py
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/spans/_spans.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/types/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/types/exceptions.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/types/indexes.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/types/spans.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/types/validators.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.3.3/src/opperai/utils/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/conftest.py
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_async_functions.py
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_async_indexes.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_async_spans.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_decorator.py
--rw-r--r--   0        0        0     8184 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_functions.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_indexes.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_spans.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_trace_decorator.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/test_types.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
--rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml
--rw-r--r--   0        0        0     9714 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_spans/test_save_feedback.yaml
--rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
--rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_get.yaml
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_upload_file.yaml
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.3.3/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.3.3/.gitignore
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.3.3/LICENSE
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 opperai-0.3.3/README.md
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 opperai-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 opperai-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.3.4/pytest.ini
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.3.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/__init__.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/_client.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/_http_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/functions/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/functions/_async_functions.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/functions/_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/functions/decorator/__init__.py
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/functions/decorator/_decorator.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/functions/decorator/_schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/indexes/__init__.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/indexes/_async_indexes.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/indexes/_indexes.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/spans/__init__.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/spans/_async_spans.py
+-rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/spans/_decorator.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/spans/_spans.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/types/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/types/exceptions.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/types/indexes.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/types/spans.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/types/validators.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.3.4/src/opperai/utils/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/conftest.py
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_async_functions.py
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_async_indexes.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_async_spans.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_decorator.py
+-rw-r--r--   0        0        0     8184 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_functions.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_indexes.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_spans.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_trace_decorator.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/test_types.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml
+-rw-r--r--   0        0        0     9714 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_spans/test_save_feedback.yaml
+-rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_get.yaml
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_upload_file.yaml
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 opperai-0.3.4/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.3.4/.gitignore
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 opperai-0.3.4/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 opperai-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 opperai-0.3.4/PKG-INFO
```

### Comparing `opperai-0.3.3/.github/workflows/publish.yml` & `opperai-0.3.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/src/opperai/_client.py` & `opperai-0.3.4/src/opperai/_client.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/src/opperai/_http_clients.py` & `opperai-0.3.4/src/opperai/_http_clients.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/src/opperai/functions/_async_functions.py` & `opperai-0.3.4/src/opperai/functions/_async_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/src/opperai/functions/_functions.py` & `opperai-0.3.4/src/opperai/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/src/opperai/functions/decorator/_decorator.py` & `opperai-0.3.4/src/opperai/functions/decorator/_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/src/opperai/functions/decorator/_schemas.py` & `opperai-0.3.4/src/opperai/functions/decorator/_schemas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,63 @@
 import inspect
 from typing import Dict, List, Union, get_args, get_origin, get_type_hints
 
 from pydantic import BaseModel
 
 
 def type_to_json_schema(type_hint):
+    schema = _type_to_json_schema(type_hint)
+    schema, defs = _lift_defs(schema, {})
+    schema["$defs"] = defs
+    return schema
+
+
+def _lift_defs(schema: Dict, defs: Dict = {}):
+    if "$defs" in schema:
+        for k, v in schema["$defs"].items():
+            defs[k] = v
+        schema.pop("$defs")
+
+    for k, v in schema.items():
+        if isinstance(v, dict):
+            _lift_defs(v, defs)
+        elif isinstance(v, list):
+            for item in v:
+                if isinstance(item, dict):
+                    _lift_defs(item, defs)
+
+    return schema, defs
+
+
+def _type_to_json_schema(type_hint):
     """Convert a Python type to a JSON schema."""
     if type_hint == int:
         return {"type": "integer"}
     elif type_hint == str:
         return {"type": "string"}
     elif type_hint == float:
         return {"type": "number"}
     elif type_hint == bool:
         return {"type": "boolean"}
     elif inspect.isclass(type_hint) and issubclass(type_hint, BaseModel):
         return type_hint.model_json_schema()
     elif hasattr(type_hint, "__origin__"):
         # Handling generic types (List, Dict, etc.)
         if get_origin(type_hint) == Union and type(None) in get_args(type_hint):
-            return type_to_json_schema(get_args(type_hint)[0])  # for Optional
+            return _type_to_json_schema(get_args(type_hint)[0])  # for Optional
         elif type_hint.__origin__ in (List, list):
             item_type = get_args(type_hint)[0]
             if inspect.isclass(item_type):
-                return {"type": "array", "items": type_to_json_schema(item_type)}
+                return {"type": "array", "items": _type_to_json_schema(item_type)}
             if get_origin(item_type) == List:
-                return {"type": "array", "items": type_to_json_schema(item_type)}
+                return {"type": "array", "items": _type_to_json_schema(item_type)}
             elif inspect.isclass(item_type) and issubclass(item_type, BaseModel):
-                return {"type": "array", "items": item_type.schema()}
+                return {"type": "array", "items": item_type.model_json_schema()}
             else:
-                return {"type": "array", "items": type_to_json_schema(item_type)}
+                return {"type": "array", "items": _type_to_json_schema(item_type)}
         elif get_origin(type_hint) == Dict:
             return {"type": "object"}
         else:
             raise NotImplementedError(
                 f"Type {type_hint} is not supported for JSON schema generation.{get_origin(type_hint)}"
             )
     else:
```

### Comparing `opperai-0.3.3/src/opperai/indexes/_async_indexes.py` & `opperai-0.3.4/src/opperai/indexes/_async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/src/opperai/indexes/_indexes.py` & `opperai-0.3.4/src/opperai/indexes/_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/src/opperai/spans/_async_spans.py` & `opperai-0.3.4/src/opperai/spans/_async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/src/opperai/spans/_decorator.py` & `opperai-0.3.4/src/opperai/spans/_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/src/opperai/spans/_spans.py` & `opperai-0.3.4/src/opperai/spans/_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/src/opperai/types/__init__.py` & `opperai-0.3.4/src/opperai/types/__init__.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/src/opperai/types/indexes.py` & `opperai-0.3.4/src/opperai/types/indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/src/opperai/types/spans.py` & `opperai-0.3.4/src/opperai/types/spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/src/opperai/types/validators.py` & `opperai-0.3.4/src/opperai/types/validators.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/src/opperai/utils/__init__.py` & `opperai-0.3.4/src/opperai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/conftest.py` & `opperai-0.3.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/test_async_functions.py` & `opperai-0.3.4/tests/test_async_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/test_async_indexes.py` & `opperai-0.3.4/tests/test_async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/test_async_spans.py` & `opperai-0.3.4/tests/test_async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/test_decorator.py` & `opperai-0.3.4/tests/test_decorator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import os
 from typing import Dict, List, Optional, Union
 from unittest.mock import MagicMock, patch
 
+import pytest
+from jsonschema import validate
 from opperai import fn
+from opperai.functions.decorator._schemas import type_to_json_schema
 from opperai.utils import (
     convert_function_call_to_json,
 )
 from pydantic import BaseModel
 
 
 @patch("opperai._http_clients._http_client.do_request")
@@ -133,7 +135,75 @@
 
     json = convert_function_call_to_json(advanced, "Hello", "es", model)
     assert json == {
         "text": "Hello",
         "target_language": "es",
         "model": model.model_dump(),
     }
+
+
+class ToyModel(BaseModel):
+    name: str
+
+
+class ChildModel(BaseModel):
+    toy: ToyModel
+    toys: List[ToyModel]
+
+
+class ParentModel(BaseModel):
+    child: ChildModel
+    children: List[ChildModel]
+
+
+@pytest.mark.parametrize(
+    "type_input,  example_input",
+    [
+        (int, 1),
+        (str, "string"),
+        (float, 1.0),
+        (bool, True),
+        (List[int], [1, 2, 3]),
+        (
+            ParentModel,
+            {
+                "child": {
+                    "toy": {"name": "name"},
+                    "toys": [{"name": "name"}],
+                },
+                "children": [{"toy": {"name": "name"}, "toys": [{"name": "name"}]}],
+            },
+        ),
+        (
+            List[ParentModel],
+            [
+                {
+                    "child": {
+                        "toy": {"name": "name"},
+                        "toys": [{"name": "name"}],
+                    },
+                    "children": [{"toy": {"name": "name"}, "toys": [{"name": "name"}]}],
+                }
+            ],
+        ),
+        (
+            List[List[ParentModel]],
+            [
+                [
+                    {
+                        "child": {
+                            "toy": {"name": "name"},
+                            "toys": [{"name": "name"}],
+                        },
+                        "children": [
+                            {"toy": {"name": "name"}, "toys": [{"name": "name"}]}
+                        ],
+                    }
+                ],
+            ],
+        ),
+    ],
+)
+def test_type_to_json_schema(type_input, example_input):
+    schema = type_to_json_schema(type_input)
+    print(schema)
+    assert validate(example_input, schema) is None
```

### Comparing `opperai-0.3.3/tests/test_functions.py` & `opperai-0.3.4/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/test_indexes.py` & `opperai-0.3.4/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/test_spans.py` & `opperai-0.3.4/tests/test_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/test_trace_decorator.py` & `opperai-0.3.4/tests/test_trace_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/test_types.py` & `opperai-0.3.4/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_async_spans/test_save_feedback.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_async_spans/test_save_feedback.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_get.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_get.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_indexes/test_upload_file.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_indexes/test_upload_file.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml` & `opperai-0.3.4/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/LICENSE` & `opperai-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/README.md` & `opperai-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `opperai-0.3.3/pyproject.toml` & `opperai-0.3.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "opperai"
-version = "0.3.3"
+version = "0.3.4"
 description = "Opper Python client"
 authors = [
   {name = "Opper", email = "opper@opper.ai"},
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -28,15 +28,16 @@
 Platform = "https://platform.opper.ai"
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
-    "vcrpy"
+    "vcrpy",
+    "jsonschema"
 ]
 
 
 [tool.pytest.ini_options]
 pythonpath = [
   "src"
 ]
```

### Comparing `opperai-0.3.3/PKG-INFO` & `opperai-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.3
 Name: opperai
-Version: 0.3.3
+Version: 0.3.4
 Summary: Opper Python client
 Project-URL: Homepage, https://opper.ai
 Project-URL: Documentation, https://docs.opper.ai
 Project-URL: Platform, https://platform.opper.ai
 Author-email: Opper <opper@opper.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: httpx
 Requires-Dist: httpx-sse
 Requires-Dist: pydantic
 Provides-Extra: test
+Requires-Dist: jsonschema; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: vcrpy; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Opper Python SDK
```

