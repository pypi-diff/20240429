# Comparing `tmp/credsweeper-1.6.3.tar.gz` & `tmp/credsweeper-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credsweeper-1.6.3.tar", last modified: Wed Apr 24 08:22:04 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `credsweeper-1.6.3.tar` & `credsweeper-1.6.4.tar`

### file list

```diff
@@ -1,170 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.284752 credsweeper-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-24 08:22:00.000000 credsweeper-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-04-24 08:22:04.284752 credsweeper-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-04-24 08:22:00.000000 credsweeper-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.260752 credsweeper-1.6.3/credsweeper/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15952 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18285 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.260752 credsweeper-1.6.3/credsweeper/common/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/common/keyword_checklist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/common/keyword_checklist.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8711 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/common/morpheme_checklist.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.260752 credsweeper-1.6.3/credsweeper/config/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.264752 credsweeper-1.6.3/credsweeper/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/credentials/augment_candidates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/credentials/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/credentials/candidate_group_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/credentials/candidate_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/credentials/credential_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9027 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/credentials/line_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.264752 credsweeper-1.6.3/credsweeper/deep_scanner/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/abstract_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/byte_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/bzip2_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/deep_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/docx_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/eml_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/encoder_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/gzip_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/html_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/jks_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/lang_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/pdf_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/pkcs12_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/tar_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/xml_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/deep_scanner/zip_scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.268752 credsweeper-1.6.3/credsweeper/file_handler/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/abstract_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/analysis_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/byte_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/content_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    15353 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/data_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/diff_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/file_path_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/files_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/patches_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/string_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/struct_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/file_handler/text_content_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.272752 credsweeper-1.6.3/credsweeper/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.276752 credsweeper-1.6.3/credsweeper/filters/group/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/general_keyword.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/general_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/password_keyword.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/token_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/url_credentials_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/weird_base36_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/group/weird_base64_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/line_git_binary_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/line_specific_key_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/separator_unusual_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_allowlist_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_array_dictionary_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_atlassian_token_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_base32_data_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_base64_data_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_base64_encoded_pem_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_base64_key_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_blocklist_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_camel_case_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_couple_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_dictionary_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_dictionary_value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_entropy_base32_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_entropy_base36_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_entropy_base64_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_file_path_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_first_word_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_github_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_grafana_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_hex_number_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_ip_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_jfrog_token_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_json_web_token_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_last_word_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_method_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_not_allowed_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_not_part_encoded_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_number_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_pattern_length_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_similarity_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_split_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_string_type_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_token_base32_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_token_base36_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_token_base64_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_token_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/value_useless_word_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/filters/variable_not_allowed_pattern_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.276752 credsweeper-1.6.3/credsweeper/logger/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.276752 credsweeper-1.6.3/credsweeper/ml_model/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/ml_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/ml_model/features.py
--rw-r--r--   0 runner    (1001) docker     (127)   868645 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/ml_model/ml_model.onnx
--rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/ml_model/ml_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9538 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/ml_model/model_config.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.276752 credsweeper-1.6.3/credsweeper/rules/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24774 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/rules/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.276752 credsweeper-1.6.3/credsweeper/scanner/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/scanner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.280752 credsweeper-1.6.3/credsweeper/scanner/scan_type/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/scanner/scan_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/scanner/scan_type/multi_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/scanner/scan_type/pem_key_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/scanner/scan_type/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/scanner/scan_type/single_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/scanner/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.280752 credsweeper-1.6.3/credsweeper/secret/
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/secret/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/secret/log.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.280752 credsweeper-1.6.3/credsweeper/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/utils/entropy_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/utils/pem_key_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    24067 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.280752 credsweeper-1.6.3/credsweeper/validations/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/apply_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/github_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/google_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/google_multi_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/mailchimp_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/slack_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/square_access_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/square_client_id_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/stripe_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-24 08:22:00.000000 credsweeper-1.6.3/credsweeper/validations/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.280752 credsweeper-1.6.3/credsweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-04-24 08:22:04.000000 credsweeper-1.6.3/credsweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-24 08:22:04.000000 credsweeper-1.6.3/credsweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:22:04.000000 credsweeper-1.6.3/credsweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 08:22:04.000000 credsweeper-1.6.3/credsweeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-24 08:22:04.000000 credsweeper-1.6.3/credsweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 08:22:04.000000 credsweeper-1.6.3/credsweeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-24 08:22:04.284752 credsweeper-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-24 08:22:00.000000 credsweeper-1.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:22:04.280752 credsweeper-1.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    32156 2024-04-24 08:22:00.000000 credsweeper-1.6.3/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-24 08:22:00.000000 credsweeper-1.6.3/tests/test_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)    41777 2024-04-24 08:22:00.000000 credsweeper-1.6.3/tests/test_main.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/__init__.py
+-rw-r--r--   0        0        0    15952 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/__main__.py
+-rw-r--r--   0        0        0    18285 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/py.typed
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/common/__init__.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/common/constants.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/common/keyword_checklist.py
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/common/keyword_checklist.txt
+-rw-r--r--   0        0        0     8711 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/common/morpheme_checklist.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/config/__init__.py
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/config/config.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/credentials/__init__.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/credentials/augment_candidates.py
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/credentials/candidate.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/credentials/candidate_group_generator.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/credentials/candidate_key.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/credentials/credential_manager.py
+-rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/credentials/line_data.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/__init__.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/abstract_scanner.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/byte_scanner.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/bzip2_scanner.py
+-rw-r--r--   0        0        0    13907 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/deep_scanner.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/docx_scanner.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/eml_scanner.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/encoder_scanner.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/gzip_scanner.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/html_scanner.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/jks_scanner.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/lang_scanner.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/pdf_scanner.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/pkcs12_scanner.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/tar_scanner.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/xml_scanner.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/deep_scanner/zip_scanner.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/__init__.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/abstract_provider.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/analysis_target.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/byte_content_provider.py
+-rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/content_provider.py
+-rw-r--r--   0        0        0    15353 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/data_content_provider.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/descriptor.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/diff_content_provider.py
+-rw-r--r--   0        0        0     6723 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/file_path_extractor.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/files_provider.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/patches_provider.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/string_content_provider.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/struct_content_provider.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/file_handler/text_content_provider.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/__init__.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/filter.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/line_git_binary_check.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/line_specific_key_check.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/separator_unusual_check.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_allowlist_check.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_array_dictionary_check.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_atlassian_token_check.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_base32_data_check.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_base64_data_check.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_base64_encoded_pem_check.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_base64_key_check.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_blocklist_check.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_camel_case_check.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_couple_keyword_check.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_dictionary_keyword_check.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_dictionary_value_length_check.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_entropy_base32_check.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_entropy_base36_check.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_entropy_base64_check.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_file_path_check.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_first_word_check.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_github_check.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_grafana_check.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_hex_number_check.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_ip_check.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_jfrog_token_check.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_json_web_token_check.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_last_word_check.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_length_check.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_method_check.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_not_allowed_pattern_check.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_not_part_encoded_check.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_number_check.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_pattern_check.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_pattern_length_check.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_similarity_check.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_split_keyword_check.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_string_type_check.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_token_base32_check.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_token_base36_check.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_token_base64_check.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_token_check.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/value_useless_word_check.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/variable_not_allowed_pattern_check.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/general_keyword.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/general_pattern.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/group.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/password_keyword.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/token_pattern.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/url_credentials_group.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/weird_base36_token.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/filters/group/weird_base64_token.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/logger/__init__.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/logger/logger.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/ml_model/__init__.py
+-rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/ml_model/features.py
+-rw-r--r--   0        0        0   868645 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/ml_model/ml_model.onnx
+-rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/ml_model/ml_validator.py
+-rw-r--r--   0        0        0     9538 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/ml_model/model_config.json
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/rules/__init__.py
+-rw-r--r--   0        0        0    24774 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/rules/config.yaml
+-rw-r--r--   0        0        0    10857 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/rules/rule.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/scanner/__init__.py
+-rw-r--r--   0        0        0     9550 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/scanner/scanner.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/scanner/scan_type/__init__.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/scanner/scan_type/multi_pattern.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/scanner/scan_type/pem_key_pattern.py
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/scanner/scan_type/scan_type.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/scanner/scan_type/single_pattern.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/secret/config.json
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/secret/log.yaml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/utils/__init__.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/utils/entropy_validator.py
+-rw-r--r--   0        0        0     7715 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/utils/pem_key_detector.py
+-rw-r--r--   0        0        0    24067 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/utils/util.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/__init__.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/apply_validation.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/github_token_validation.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/google_api_key_validation.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/google_multi_validation.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/mailchimp_key_validation.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/slack_token_validation.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/square_access_token_validation.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/square_client_id_validation.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/stripe_api_key_validation.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 credsweeper-1.6.4/credsweeper/validations/validation.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 credsweeper-1.6.4/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 credsweeper-1.6.4/LICENSE
+-rw-r--r--   0        0        0     9026 2020-02-02 00:00:00.000000 credsweeper-1.6.4/README.md
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 credsweeper-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 credsweeper-1.6.4/PKG-INFO
```

### Comparing `credsweeper-1.6.3/LICENSE` & `credsweeper-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/PKG-INFO` & `credsweeper-1.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: credsweeper
-Version: 1.6.3
+Version: 1.6.4
 Summary: Credential Sweeper
-Home-page: https://github.com/Samsung/CredSweeper
+Project-URL: Homepage, https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
+License: MIT
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: base58
 Requires-Dist: beautifulsoup4>=4.11.0
 Requires-Dist: cryptography
-Requires-Dist: GitPython
-Requires-Dist: google_auth_oauthlib
+Requires-Dist: gitpython
+Requires-Dist: google-auth-oauthlib
 Requires-Dist: humanfriendly
-Requires-Dist: lxml
+Requires-Dist: lxml; platform_system != 'Darwin'
+Requires-Dist: lxml==4.9.4; platform_system == 'Darwin' and python_version < '3.9'
+Requires-Dist: numpy
 Requires-Dist: oauthlib
+Requires-Dist: onnxruntime
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: password-strength
-Requires-Dist: pdfminer.six
-Requires-Dist: PyYAML
+Requires-Dist: pdfminer-six
+Requires-Dist: pybase62
+Requires-Dist: pyjks
+Requires-Dist: python-dateutil
 Requires-Dist: python-docx
+Requires-Dist: pyyaml
 Requires-Dist: requests
-Requires-Dist: scipy
 Requires-Dist: schwifty
-Requires-Dist: typing_extensions
-Requires-Dist: whatthepatch
-Requires-Dist: numpy
 Requires-Dist: scikit-learn
-Requires-Dist: onnxruntime
-Requires-Dist: python-dateutil
-Requires-Dist: pyjks
-Requires-Dist: pybase62
-Requires-Dist: base58
+Requires-Dist: scipy
+Requires-Dist: typing-extensions
+Requires-Dist: whatthepatch
+Description-Content-Type: text/markdown
 
 # CredSweeper
 
 [![GitHub release (latestSemVer)](https://img.shields.io/github/v/release/Samsung/CredSweeper)](https://github.com/Samsung/CredSweeper/releases)
 [![Documentation Status](https://readthedocs.org/projects/credsweeper/badge/?version=latest)](https://credsweeper.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/badge/licence-MIT-green.svg?style=flat)](LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/credsweeper)](https://pypi.org/project/credsweeper/)
```

### Comparing `credsweeper-1.6.3/README.md` & `credsweeper-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/__init__.py` & `credsweeper-1.6.4/credsweeper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     'MlValidator',  #
     'StringContentProvider',  #
     'TextContentProvider',  #
     'ThresholdPreset',  #
     '__version__'
 ]
 
-__version__ = "1.6.3"
+__version__ = "1.6.4"
```

### Comparing `credsweeper-1.6.3/credsweeper/__main__.py` & `credsweeper-1.6.4/credsweeper/__main__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/app.py` & `credsweeper-1.6.4/credsweeper/app.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/common/constants.py` & `credsweeper-1.6.4/credsweeper/common/constants.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/common/keyword_checklist.py` & `credsweeper-1.6.4/credsweeper/common/keyword_checklist.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/common/keyword_checklist.txt` & `credsweeper-1.6.4/credsweeper/common/keyword_checklist.txt`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/common/morpheme_checklist.txt` & `credsweeper-1.6.4/credsweeper/common/morpheme_checklist.txt`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/config/config.py` & `credsweeper-1.6.4/credsweeper/config/config.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/credentials/augment_candidates.py` & `credsweeper-1.6.4/credsweeper/credentials/augment_candidates.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/credentials/candidate.py` & `credsweeper-1.6.4/credsweeper/credentials/candidate.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/credentials/candidate_group_generator.py` & `credsweeper-1.6.4/credsweeper/credentials/candidate_group_generator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/credentials/candidate_key.py` & `credsweeper-1.6.4/credsweeper/credentials/candidate_key.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/credentials/credential_manager.py` & `credsweeper-1.6.4/credsweeper/credentials/credential_manager.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/credentials/line_data.py` & `credsweeper-1.6.4/credsweeper/credentials/line_data.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/abstract_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/abstract_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/byte_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/byte_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/bzip2_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/bzip2_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/deep_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/deep_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/docx_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/docx_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/eml_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/eml_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/encoder_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/encoder_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/gzip_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/gzip_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/html_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/html_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/jks_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/jks_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/lang_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/lang_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/pdf_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/pdf_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/pkcs12_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/pkcs12_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/tar_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/tar_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/xml_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/xml_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/deep_scanner/zip_scanner.py` & `credsweeper-1.6.4/credsweeper/deep_scanner/zip_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/file_handler/__init__.py` & `credsweeper-1.6.4/credsweeper/file_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/file_handler/abstract_provider.py` & `credsweeper-1.6.4/credsweeper/file_handler/abstract_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/file_handler/analysis_target.py` & `credsweeper-1.6.4/credsweeper/file_handler/analysis_target.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/file_handler/byte_content_provider.py` & `credsweeper-1.6.4/credsweeper/file_handler/byte_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/file_handler/content_provider.py` & `credsweeper-1.6.4/credsweeper/file_handler/content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/file_handler/data_content_provider.py` & `credsweeper-1.6.4/credsweeper/file_handler/data_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/file_handler/diff_content_provider.py` & `credsweeper-1.6.4/credsweeper/file_handler/diff_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/file_handler/file_path_extractor.py` & `credsweeper-1.6.4/credsweeper/file_handler/file_path_extractor.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/file_handler/files_provider.py` & `credsweeper-1.6.4/credsweeper/file_handler/files_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/file_handler/patches_provider.py` & `credsweeper-1.6.4/credsweeper/file_handler/patches_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/file_handler/string_content_provider.py` & `credsweeper-1.6.4/credsweeper/file_handler/string_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/file_handler/struct_content_provider.py` & `credsweeper-1.6.4/credsweeper/file_handler/struct_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/file_handler/text_content_provider.py` & `credsweeper-1.6.4/credsweeper/file_handler/text_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/__init__.py` & `credsweeper-1.6.4/credsweeper/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/filter.py` & `credsweeper-1.6.4/credsweeper/filters/filter.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/group/__init__.py` & `credsweeper-1.6.4/credsweeper/filters/group/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/group/group.py` & `credsweeper-1.6.4/credsweeper/filters/group/group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/group/password_keyword.py` & `credsweeper-1.6.4/credsweeper/filters/group/password_keyword.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/group/token_pattern.py` & `credsweeper-1.6.4/credsweeper/filters/group/token_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/group/url_credentials_group.py` & `credsweeper-1.6.4/credsweeper/filters/group/url_credentials_group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/group/weird_base36_token.py` & `credsweeper-1.6.4/credsweeper/filters/group/weird_base36_token.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/group/weird_base64_token.py` & `credsweeper-1.6.4/credsweeper/filters/group/weird_base64_token.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/line_git_binary_check.py` & `credsweeper-1.6.4/credsweeper/filters/line_git_binary_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/line_specific_key_check.py` & `credsweeper-1.6.4/credsweeper/filters/line_specific_key_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/separator_unusual_check.py` & `credsweeper-1.6.4/credsweeper/filters/separator_unusual_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_allowlist_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_allowlist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_array_dictionary_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_array_dictionary_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_atlassian_token_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_atlassian_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_base32_data_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_base32_data_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_base64_data_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_base64_data_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_base64_encoded_pem_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_base64_encoded_pem_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_base64_key_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_base64_key_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_blocklist_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_blocklist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_camel_case_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_camel_case_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_couple_keyword_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_couple_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_dictionary_keyword_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_dictionary_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_dictionary_value_length_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_dictionary_value_length_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_entropy_base32_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_entropy_base32_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_entropy_base36_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_entropy_base36_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_entropy_base64_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_entropy_base64_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_file_path_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_file_path_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_first_word_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_first_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_github_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_github_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_grafana_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_grafana_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_hex_number_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_hex_number_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_ip_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_ip_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_jfrog_token_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_jfrog_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_json_web_token_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_json_web_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_last_word_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_last_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_length_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_length_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_method_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_method_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_not_allowed_pattern_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_not_allowed_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_not_part_encoded_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_not_part_encoded_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_number_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_number_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_pattern_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_similarity_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_similarity_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_split_keyword_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_split_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_string_type_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_string_type_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_token_base32_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_token_base32_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_token_base36_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_token_base36_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_token_base64_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_token_base64_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_token_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/value_useless_word_check.py` & `credsweeper-1.6.4/credsweeper/filters/value_useless_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/filters/variable_not_allowed_pattern_check.py` & `credsweeper-1.6.4/credsweeper/filters/variable_not_allowed_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/logger/logger.py` & `credsweeper-1.6.4/credsweeper/logger/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,9 +44,9 @@
                 logging_config = Util.yaml_load(APP_PATH / "secret" / "log.yaml")
             log_dir = Path(logging_config["handlers"]["logfile"]["filename"]).resolve().parent
             log_dir.mkdir(exist_ok=True)
             logging_config["handlers"]["console"]["level"] = level
             logging.config.dictConfig(logging_config)
             for module in logging_config["ignore"]:
                 logging.getLogger(module).setLevel(logging.ERROR)
-        except (IOError, OSError):
+        except OSError:
             logging.basicConfig(level=logging.WARNING)
```

### Comparing `credsweeper-1.6.3/credsweeper/ml_model/features.py` & `credsweeper-1.6.4/credsweeper/ml_model/features.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/ml_model/ml_model.onnx` & `credsweeper-1.6.4/credsweeper/ml_model/ml_model.onnx`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/ml_model/ml_validator.py` & `credsweeper-1.6.4/credsweeper/ml_model/ml_validator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/ml_model/model_config.json` & `credsweeper-1.6.4/credsweeper/ml_model/model_config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/rules/config.yaml` & `credsweeper-1.6.4/credsweeper/rules/config.yaml`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/rules/rule.py` & `credsweeper-1.6.4/credsweeper/rules/rule.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/scanner/scan_type/multi_pattern.py` & `credsweeper-1.6.4/credsweeper/scanner/scan_type/multi_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/scanner/scan_type/pem_key_pattern.py` & `credsweeper-1.6.4/credsweeper/scanner/scan_type/pem_key_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/scanner/scan_type/scan_type.py` & `credsweeper-1.6.4/credsweeper/scanner/scan_type/scan_type.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/scanner/scan_type/single_pattern.py` & `credsweeper-1.6.4/credsweeper/scanner/scan_type/single_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/scanner/scanner.py` & `credsweeper-1.6.4/credsweeper/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/secret/config.json` & `credsweeper-1.6.4/credsweeper/secret/config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/secret/log.yaml` & `credsweeper-1.6.4/credsweeper/secret/log.yaml`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/utils/entropy_validator.py` & `credsweeper-1.6.4/credsweeper/utils/entropy_validator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/utils/pem_key_detector.py` & `credsweeper-1.6.4/credsweeper/utils/pem_key_detector.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/utils/util.py` & `credsweeper-1.6.4/credsweeper/utils/util.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/validations/__init__.py` & `credsweeper-1.6.4/credsweeper/validations/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/validations/apply_validation.py` & `credsweeper-1.6.4/credsweeper/validations/apply_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/validations/github_token_validation.py` & `credsweeper-1.6.4/credsweeper/validations/github_token_validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
         """
         try:
             r = requests.get(
                 "https://api.github.com",
                 headers={"Authorization": f"token {line_data_list[0].value}"},
             )
-        except (requests.exceptions.ConnectionError, Exception) as exc:
+        except Exception as exc:
             logger.error(f"Cannot validate {line_data_list[0].value} token using API\n{exc}")
             return KeyValidationOption.UNDECIDED
 
         # According to documentation, authentication with wrong credentials return 401
         # After detecting several requests with invalid credentials within a short period,
         # the API will temporarily reject all auth attempts with 403
         if r.status_code == 401:
```

### Comparing `credsweeper-1.6.3/credsweeper/validations/google_api_key_validation.py` & `credsweeper-1.6.4/credsweeper/validations/google_api_key_validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         """
         try:
             # Note that requests without "input" and "inputtype" URL arguments
             #  requests is invalid and will always be denied. But Google will still
             #  validate the "key", so we will know if it's real or not.
             r = requests.get(
                 f"https://maps.googleapis.com/maps/api/place/findplacefromtext/json?key={line_data_list[0].value}")
-        except (requests.exceptions.ConnectionError, Exception) as exc:
+        except Exception as exc:
             logger.error(f"Cannot validate {line_data_list[0].value} token using API\n{exc}")
             return KeyValidationOption.UNDECIDED
 
         # Google sends 200 even in case of REQUEST_DENIED
         if r.status_code == 200:
             try:
                 data = r.json()
```

### Comparing `credsweeper-1.6.3/credsweeper/validations/google_multi_validation.py` & `credsweeper-1.6.4/credsweeper/validations/google_multi_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/validations/mailchimp_key_validation.py` & `credsweeper-1.6.4/credsweeper/validations/mailchimp_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.6.3/credsweeper/validations/slack_token_validation.py` & `credsweeper-1.6.4/credsweeper/validations/slack_token_validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             Enum object, returns the validation status for the passed value
             can take values: VALIDATED_KEY, INVALID_KEY or UNDECIDED
 
         """
         try:
             headers = {"Content-type": "application/json", "Authorization": f"Bearer {line_data_list[0].value}"}
             r = requests.post("https://slack.com/api/auth.test/", headers=headers)
-        except (requests.exceptions.ConnectionError, Exception) as exc:
+        except Exception as exc:
             logger.error(f"Cannot validate {line_data_list[0].value} token using API\n{exc}")
             return KeyValidationOption.UNDECIDED
 
         try:
             data = r.json()
 
             if data.get("ok"):
```

### Comparing `credsweeper-1.6.3/credsweeper/validations/square_access_token_validation.py` & `credsweeper-1.6.4/credsweeper/validations/square_access_token_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         """
         try:
             r = requests.post(
                 "https://connect.squareup.com/v2/payments",
                 headers={"Authorization": f"Bearer {line_data_list[0].value}"},
             )
-        except (requests.exceptions.ConnectionError, Exception) as exc:
+        except Exception as exc:
             logger.error(f"Cannot validate {line_data_list[0].value} token using API\n{exc}")
             return KeyValidationOption.UNDECIDED
 
         # We actually expect successfully authenticated request to fail with 400
         #  (Bad Request) as we provided no body for the POST. If authentication
         #  failed we will see 401, not 400
         if r.status_code in [200, 400]:
```

### Comparing `credsweeper-1.6.3/credsweeper/validations/square_client_id_validation.py` & `credsweeper-1.6.4/credsweeper/validations/square_client_id_validation.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             Enum object, returns the validation status for the passed value
             can take values: VALIDATED_KEY, INVALID_KEY or UNDECIDED
 
         """
         try:
             r = requests.get(f"https://squareup.com/oauth2/authorize?client_id={line_data_list[0].value}",
                              allow_redirects=False)
-        except (requests.exceptions.ConnectionError, Exception) as exc:
+        except Exception as exc:
             logger.error(f"Cannot validate {line_data_list[0].value} token using API\n{exc}")
             return KeyValidationOption.UNDECIDED
 
         positive_start = "<body>You are being <a"
         positive_end = ">redirected"
         negative = "Unable to find client by that `client_id`"
```

### Comparing `credsweeper-1.6.3/credsweeper/validations/stripe_api_key_validation.py` & `credsweeper-1.6.4/credsweeper/validations/stripe_api_key_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         Return:
             Enum object, returns the validation status for the passed value
             can take values: VALIDATED_KEY, INVALID_KEY or UNDECIDED
 
         """
         try:
             r = requests.get("https://api.stripe.com/v1/charges", auth=(line_data_list[0].value, ""))
-        except (requests.exceptions.ConnectionError, Exception) as exc:
+        except Exception as exc:
             logger.error(f"Cannot validate {line_data_list[0].value} token using API\n{exc}")
             return KeyValidationOption.UNDECIDED
         # According to documentation, authentication with wrong credentials return 401
         # If key provided is of restricted type, valid but doesn't have right permission,
         # then 403 will be returned and a message with description
         if r.status_code == 401:
             return KeyValidationOption.INVALID_KEY
```

### Comparing `credsweeper-1.6.3/credsweeper/validations/validation.py` & `credsweeper-1.6.4/credsweeper/validations/validation.py`

 * *Files identical despite different names*

