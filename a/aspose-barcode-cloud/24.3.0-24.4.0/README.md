# Comparing `tmp/aspose-barcode-cloud-24.3.0.tar.gz` & `tmp/aspose_barcode_cloud-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aspose-barcode-cloud-24.3.0.tar", last modified: Mon Mar 25 04:47:21 2024, max compression
+gzip compressed data, was "aspose_barcode_cloud-24.4.0.tar", last modified: Mon Apr 29 11:46:20 2024, max compression
```

## Comparing `aspose-barcode-cloud-24.3.0.tar` & `aspose_barcode_cloud-24.4.0.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 04:47:21.146896 aspose-barcode-cloud-24.3.0/
--rw-r--r--   0 root         (0) root         (0)     1071 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15342 2024-03-25 04:47:21.146896 aspose-barcode-cloud-24.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12409 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 04:47:21.136896 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/
--rw-r--r--   0 root         (0) root         (0)     7307 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 04:47:21.136896 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/api/
--rw-r--r--   0 root         (0) root         (0)      319 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   101341 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/api/barcode_api.py
--rw-r--r--   0 root         (0) root         (0)    24326 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/api/file_api.py
--rw-r--r--   0 root         (0) root         (0)    22481 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/api/folder_api.py
--rw-r--r--   0 root         (0) root         (0)    16149 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/api/storage_api.py
--rw-r--r--   0 root         (0) root         (0)    26047 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/api_client.py
--rw-r--r--   0 root         (0) root         (0)    10460 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 04:47:21.146896 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/
--rw-r--r--   0 root         (0) root         (0)     6851 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6551 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/api_error.py
--rw-r--r--   0 root         (0) root         (0)     4604 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/api_error_response.py
--rw-r--r--   0 root         (0) root         (0)     5459 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/australian_post_params.py
--rw-r--r--   0 root         (0) root         (0)     3401 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/auto_size_mode.py
--rw-r--r--   0 root         (0) root         (0)     3447 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/available_graphics_unit.py
--rw-r--r--   0 root         (0) root         (0)     3415 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/aztec_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)    12190 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/aztec_params.py
--rw-r--r--   0 root         (0) root         (0)     3423 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/aztec_symbol_mode.py
--rw-r--r--   0 root         (0) root         (0)     6255 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/barcode_response.py
--rw-r--r--   0 root         (0) root         (0)     4165 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/barcode_response_list.py
--rw-r--r--   0 root         (0) root         (0)     3443 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/border_dash_style.py
--rw-r--r--   0 root         (0) root         (0)     8345 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/caption_params.py
--rw-r--r--   0 root         (0) root         (0)     3401 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/checksum_validation.py
--rw-r--r--   0 root         (0) root         (0)     3391 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/codabar_checksum_mode.py
--rw-r--r--   0 root         (0) root         (0)     6379 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/codabar_params.py
--rw-r--r--   0 root         (0) root         (0)     3375 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/codabar_symbol.py
--rw-r--r--   0 root         (0) root         (0)     5504 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/codablock_params.py
--rw-r--r--   0 root         (0) root         (0)     3429 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/code128_emulation.py
--rw-r--r--   0 root         (0) root         (0)     3487 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/code128_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     4270 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/code128_params.py
--rw-r--r--   0 root         (0) root         (0)     6543 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/code16_k_params.py
--rw-r--r--   0 root         (0) root         (0)     3381 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/code_location.py
--rw-r--r--   0 root         (0) root         (0)     4268 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/coupon_params.py
--rw-r--r--   0 root         (0) root         (0)     3479 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py
--rw-r--r--   0 root         (0) root         (0)     8038 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/data_bar_params.py
--rw-r--r--   0 root         (0) root         (0)     3499 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py
--rw-r--r--   0 root         (0) root         (0)     3557 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)    12809 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/data_matrix_params.py
--rw-r--r--   0 root         (0) root         (0)     5827 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/data_matrix_version.py
--rw-r--r--   0 root         (0) root         (0)     5905 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/decode_barcode_type.py
--rw-r--r--   0 root         (0) root         (0)     4943 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/disc_usage.py
--rw-r--r--   0 root         (0) root         (0)     3423 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/dot_code_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     9424 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/dot_code_params.py
--rw-r--r--   0 root         (0) root         (0)     4059 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/eci_encodings.py
--rw-r--r--   0 root         (0) root         (0)     3385 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/enable_checksum.py
--rw-r--r--   0 root         (0) root         (0)     5503 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/encode_barcode_type.py
--rw-r--r--   0 root         (0) root         (0)     6000 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/error.py
--rw-r--r--   0 root         (0) root         (0)     4767 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/error_details.py
--rw-r--r--   0 root         (0) root         (0)     8857 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/file_version.py
--rw-r--r--   0 root         (0) root         (0)     4001 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/file_versions.py
--rw-r--r--   0 root         (0) root         (0)     4025 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/files_list.py
--rw-r--r--   0 root         (0) root         (0)     4800 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/files_upload_result.py
--rw-r--r--   0 root         (0) root         (0)     3347 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/font_mode.py
--rw-r--r--   0 root         (0) root         (0)     5237 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/font_params.py
--rw-r--r--   0 root         (0) root         (0)     3431 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/font_style.py
--rw-r--r--   0 root         (0) root         (0)    57609 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/generator_params.py
--rw-r--r--   0 root         (0) root         (0)     5926 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/generator_params_list.py
--rw-r--r--   0 root         (0) root         (0)     3461 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/han_xin_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     3395 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/han_xin_error_level.py
--rw-r--r--   0 root         (0) root         (0)     7442 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/han_xin_params.py
--rw-r--r--   0 root         (0) root         (0)     5697 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/han_xin_version.py
--rw-r--r--   0 root         (0) root         (0)     3437 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/itf14_border_type.py
--rw-r--r--   0 root         (0) root         (0)     6218 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/itf_params.py
--rw-r--r--   0 root         (0) root         (0)     3397 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/macro_character.py
--rw-r--r--   0 root         (0) root         (0)     3427 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     3423 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/maxi_code_mode.py
--rw-r--r--   0 root         (0) root         (0)     5715 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/maxi_code_params.py
--rw-r--r--   0 root         (0) root         (0)     4974 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/object_exist.py
--rw-r--r--   0 root         (0) root         (0)     5780 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/padding.py
--rw-r--r--   0 root         (0) root         (0)     5497 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/patch_code_params.py
--rw-r--r--   0 root         (0) root         (0)     3471 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/patch_format.py
--rw-r--r--   0 root         (0) root         (0)     3437 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py
--rw-r--r--   0 root         (0) root         (0)     3537 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/pdf417_error_level.py
--rw-r--r--   0 root         (0) root         (0)     3411 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py
--rw-r--r--   0 root         (0) root         (0)    30506 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/pdf417_params.py
--rw-r--r--   0 root         (0) root         (0)     4207 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/postal_params.py
--rw-r--r--   0 root         (0) root         (0)     3553 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/preset_type.py
--rw-r--r--   0 root         (0) root         (0)     3489 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/qr_encode_mode.py
--rw-r--r--   0 root         (0) root         (0)     3399 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/qr_encode_type.py
--rw-r--r--   0 root         (0) root         (0)     3411 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/qr_error_level.py
--rw-r--r--   0 root         (0) root         (0)    12083 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/qr_params.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/qr_version.py
--rw-r--r--   0 root         (0) root         (0)    48587 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/reader_params.py
--rw-r--r--   0 root         (0) root         (0)     4570 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/region_point.py
--rw-r--r--   0 root         (0) root         (0)     5746 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/result_image_info.py
--rw-r--r--   0 root         (0) root         (0)     4075 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/storage_exist.py
--rw-r--r--   0 root         (0) root         (0)     7047 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/storage_file.py
--rw-r--r--   0 root         (0) root         (0)     6095 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/structured_append.py
--rw-r--r--   0 root         (0) root         (0)     3387 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/text_alignment.py
--rw-r--r--   0 root         (0) root         (0)    14400 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 04:47:21.146896 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15342 2024-03-25 04:47:21.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4670 2024-03-25 04:47:21.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 04:47:21.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2024-03-25 04:47:21.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-25 04:47:21.000000 aspose-barcode-cloud-24.3.0/aspose_barcode_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-25 04:47:21.146896 aspose-barcode-cloud-24.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5815 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 04:47:21.146896 aspose-barcode-cloud-24.3.0/tests/
--rw-r--r--   0 root         (0) root         (0)     1848 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/tests/test_auth.py
--rw-r--r--   0 root         (0) root         (0)     6492 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/tests/test_barcode_api.py
--rw-r--r--   0 root         (0) root         (0)      300 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/tests/test_configuration.py
--rw-r--r--   0 root         (0) root         (0)     1413 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/tests/test_generate_and_recognize.py
--rw-r--r--   0 root         (0) root         (0)     1803 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/tests/test_headers.py
--rw-r--r--   0 root         (0) root         (0)      885 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/tests/test_load_configuration.py
--rw-r--r--   0 root         (0) root         (0)     2751 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/tests/test_recognize_bytes.py
--rw-r--r--   0 root         (0) root         (0)     2698 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/tests/test_recognize_file.py
--rw-r--r--   0 root         (0) root         (0)     1064 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/tests/test_recognize_url.py
--rw-r--r--   0 root         (0) root         (0)     1401 2024-03-25 04:38:42.000000 aspose-barcode-cloud-24.3.0/tests/test_recognize_with_timeout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:46:20.132451 aspose_barcode_cloud-24.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15474 2024-04-29 11:46:20.132451 aspose_barcode_cloud-24.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12541 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:46:20.122451 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/
+-rw-r--r--   0 root         (0) root         (0)     6208 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:46:20.122451 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)      319 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104561 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/barcode_api.py
+-rw-r--r--   0 root         (0) root         (0)    23228 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/file_api.py
+-rw-r--r--   0 root         (0) root         (0)    21383 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/folder_api.py
+-rw-r--r--   0 root         (0) root         (0)    15051 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/storage_api.py
+-rw-r--r--   0 root         (0) root         (0)    24950 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api_client.py
+-rw-r--r--   0 root         (0) root         (0)     9362 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:46:20.132451 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/
+-rw-r--r--   0 root         (0) root         (0)     5753 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/api_error.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/api_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/australian_post_params.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/auto_size_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/available_graphics_unit.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/aztec_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)    11091 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/aztec_params.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/aztec_symbol_mode.py
+-rw-r--r--   0 root         (0) root         (0)     5156 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/barcode_response.py
+-rw-r--r--   0 root         (0) root         (0)     3066 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/barcode_response_list.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/border_dash_style.py
+-rw-r--r--   0 root         (0) root         (0)     7246 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/caption_params.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/checksum_validation.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/codabar_checksum_mode.py
+-rw-r--r--   0 root         (0) root         (0)     5280 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/codabar_params.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/codabar_symbol.py
+-rw-r--r--   0 root         (0) root         (0)     4405 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/codablock_params.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/code128_emulation.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/code128_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3171 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/code128_params.py
+-rw-r--r--   0 root         (0) root         (0)     5444 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/code16_k_params.py
+-rw-r--r--   0 root         (0) root         (0)     2282 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     3169 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/coupon_params.py
+-rw-r--r--   0 root         (0) root         (0)     2380 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/customer_information_interpreting_type.py
+-rw-r--r--   0 root         (0) root         (0)     6939 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_bar_params.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)    11710 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_matrix_params.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_matrix_version.py
+-rw-r--r--   0 root         (0) root         (0)     4806 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/decode_barcode_type.py
+-rw-r--r--   0 root         (0) root         (0)     3844 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/disc_usage.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/dot_code_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/dot_code_params.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/eci_encodings.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/enable_checksum.py
+-rw-r--r--   0 root         (0) root         (0)     4404 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/encode_barcode_type.py
+-rw-r--r--   0 root         (0) root         (0)     4901 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     3668 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/error_details.py
+-rw-r--r--   0 root         (0) root         (0)     7758 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/file_version.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/file_versions.py
+-rw-r--r--   0 root         (0) root         (0)     2926 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/files_list.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/files_upload_result.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/font_mode.py
+-rw-r--r--   0 root         (0) root         (0)     4138 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/font_params.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/font_style.py
+-rw-r--r--   0 root         (0) root         (0)    56510 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/generator_params.py
+-rw-r--r--   0 root         (0) root         (0)     4827 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/generator_params_list.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/han_xin_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/han_xin_error_level.py
+-rw-r--r--   0 root         (0) root         (0)     6343 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/han_xin_params.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/han_xin_version.py
+-rw-r--r--   0 root         (0) root         (0)     2338 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/itf14_border_type.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/itf_params.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/macro_character.py
+-rw-r--r--   0 root         (0) root         (0)     2328 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/maxi_code_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/maxi_code_mode.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/maxi_code_params.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/object_exist.py
+-rw-r--r--   0 root         (0) root         (0)     4681 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/padding.py
+-rw-r--r--   0 root         (0) root         (0)     4398 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/patch_code_params.py
+-rw-r--r--   0 root         (0) root         (0)     2372 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/patch_format.py
+-rw-r--r--   0 root         (0) root         (0)     2338 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/pdf417_compaction_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/pdf417_error_level.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/pdf417_macro_terminator.py
+-rw-r--r--   0 root         (0) root         (0)    29407 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/pdf417_params.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/postal_params.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/preset_type.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_encode_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_encode_type.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_error_level.py
+-rw-r--r--   0 root         (0) root         (0)    10984 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_params.py
+-rw-r--r--   0 root         (0) root         (0)     3462 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_version.py
+-rw-r--r--   0 root         (0) root         (0)    47480 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/reader_params.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/region_point.py
+-rw-r--r--   0 root         (0) root         (0)     4647 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/result_image_info.py
+-rw-r--r--   0 root         (0) root         (0)     2976 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/storage_exist.py
+-rw-r--r--   0 root         (0) root         (0)     5948 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/storage_file.py
+-rw-r--r--   0 root         (0) root         (0)     4996 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/structured_append.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/text_alignment.py
+-rw-r--r--   0 root         (0) root         (0)    13304 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:46:20.132451 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15474 2024-04-29 11:46:20.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4689 2024-04-29 11:46:20.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 11:46:20.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-29 11:46:20.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-29 11:46:20.000000 aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 11:46:20.132451 aspose_barcode_cloud-24.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4717 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:46:20.132451 aspose_barcode_cloud-24.4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     1848 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_auth.py
+-rw-r--r--   0 root         (0) root         (0)     6492 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_barcode_api.py
+-rw-r--r--   0 root         (0) root         (0)      300 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_generate_and_recognize.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_headers.py
+-rw-r--r--   0 root         (0) root         (0)      885 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_load_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_recognize_bytes.py
+-rw-r--r--   0 root         (0) root         (0)     2698 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_recognize_file.py
+-rw-r--r--   0 root         (0) root         (0)     1064 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_recognize_url.py
+-rw-r--r--   0 root         (0) root         (0)     1401 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_recognize_with_timeout.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2024-04-29 11:44:30.000000 aspose_barcode_cloud-24.4.0/tests/test_scan.py
```

### Comparing `aspose-barcode-cloud-24.3.0/LICENSE` & `aspose_barcode_cloud-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-24.3.0/PKG-INFO` & `aspose_barcode_cloud-24.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-barcode-cloud
-Version: 24.3.0
+Version: 24.4.0
 Summary: Aspose.Barcode Cloud API Reference
 Home-page: https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Author: Aspose Barcode Cloud
 License: MIT
 Project-URL: Source With Tests, https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Project-URL: Website, https://www.aspose.cloud
 Project-URL: Product Home, https://products.aspose.cloud/barcode/
@@ -39,15 +39,15 @@
 # Aspose.BarCode Cloud SDK for Python
 
 [![License](https://img.shields.io/github/license/aspose-barcode-cloud/aspose-barcode-cloud-python)](LICENSE)
 [![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/aspose-barcode-cloud)](https://pypi.org/project/aspose-barcode-cloud/)
 
 - API version: 3.0
-- Package version: 24.3.0
+- Package version: 24.4.0
 
 ## Demo applications
 
 [Scan QR](https://products.aspose.app/barcode/scanqr) | [Generate Barcode](https://products.aspose.app/barcode/generate) | [Recognize Barcode](https://products.aspose.app/barcode/recognize)
 :---: | :---: | :---:
 [![ScanQR](https://products.aspose.app/barcode/scanqr/img/aspose_scanqr-app-48.png)](https://products.aspose.app/barcode/scanqr) | [![Generate](https://products.aspose.app/barcode/generate/img/aspose_generate-app-48.png)](https://products.aspose.app/barcode/generate) | [![Recognize](https://products.aspose.app/barcode/recognize/img/aspose_recognize-app-48.png)](https://products.aspose.app/barcode/recognize)
 [**Generate Wi-Fi QR**](https://products.aspose.app/barcode/wifi-qr) | [**Embed Barcode**](https://products.aspose.app/barcode/embed) | [**Scan Barcode**](https://products.aspose.app/barcode/scan)
@@ -153,14 +153,15 @@
 *BarcodeApi* | [**get_barcode_generate**](docs/BarcodeApi.md#get_barcode_generate) | **GET** /barcode/generate | Generate barcode.
 *BarcodeApi* | [**get_barcode_recognize**](docs/BarcodeApi.md#get_barcode_recognize) | **GET** /barcode/{name}/recognize | Recognize barcode from a file on server.
 *BarcodeApi* | [**post_barcode_recognize_from_url_or_content**](docs/BarcodeApi.md#post_barcode_recognize_from_url_or_content) | **POST** /barcode/recognize | Recognize barcode from an url or from request body. Request body can contain raw data bytes of the image with content-type \&quot;application/octet-stream\&quot;. An image can also be passed as a form field.
 *BarcodeApi* | [**post_generate_multiple**](docs/BarcodeApi.md#post_generate_multiple) | **POST** /barcode/generateMultiple | Generate multiple barcodes and return in response stream
 *BarcodeApi* | [**put_barcode_generate_file**](docs/BarcodeApi.md#put_barcode_generate_file) | **PUT** /barcode/{name}/generate | Generate barcode and save on server (from query params or from file with json or xml content)
 *BarcodeApi* | [**put_barcode_recognize_from_body**](docs/BarcodeApi.md#put_barcode_recognize_from_body) | **PUT** /barcode/{name}/recognize | Recognition of a barcode from file on server with parameters in body.
 *BarcodeApi* | [**put_generate_multiple**](docs/BarcodeApi.md#put_generate_multiple) | **PUT** /barcode/{name}/generateMultiple | Generate image with multiple barcodes and put new file on server
+*BarcodeApi* | [**scan_barcode**](docs/BarcodeApi.md#scan_barcode) | **POST** /barcode/scan | Quickly scan a barcode from an image.
 *FileApi* | [**copy_file**](docs/FileApi.md#copy_file) | **PUT** /barcode/storage/file/copy/{srcPath} | Copy file
 *FileApi* | [**delete_file**](docs/FileApi.md#delete_file) | **DELETE** /barcode/storage/file/{path} | Delete file
 *FileApi* | [**download_file**](docs/FileApi.md#download_file) | **GET** /barcode/storage/file/{path} | Download file
 *FileApi* | [**move_file**](docs/FileApi.md#move_file) | **PUT** /barcode/storage/file/move/{srcPath} | Move file
 *FileApi* | [**upload_file**](docs/FileApi.md#upload_file) | **PUT** /barcode/storage/file/{path} | Upload file
 *FolderApi* | [**copy_folder**](docs/FolderApi.md#copy_folder) | **PUT** /barcode/storage/folder/copy/{srcPath} | Copy folder
 *FolderApi* | [**create_folder**](docs/FolderApi.md#create_folder) | **PUT** /barcode/storage/folder/{path} | Create the folder
```

### Comparing `aspose-barcode-cloud-24.3.0/README.md` & `aspose_barcode_cloud-24.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Aspose.BarCode Cloud SDK for Python
 
 [![License](https://img.shields.io/github/license/aspose-barcode-cloud/aspose-barcode-cloud-python)](LICENSE)
 [![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/aspose-barcode-cloud)](https://pypi.org/project/aspose-barcode-cloud/)
 
 - API version: 3.0
-- Package version: 24.3.0
+- Package version: 24.4.0
 
 ## Demo applications
 
 [Scan QR](https://products.aspose.app/barcode/scanqr) | [Generate Barcode](https://products.aspose.app/barcode/generate) | [Recognize Barcode](https://products.aspose.app/barcode/recognize)
 :---: | :---: | :---:
 [![ScanQR](https://products.aspose.app/barcode/scanqr/img/aspose_scanqr-app-48.png)](https://products.aspose.app/barcode/scanqr) | [![Generate](https://products.aspose.app/barcode/generate/img/aspose_generate-app-48.png)](https://products.aspose.app/barcode/generate) | [![Recognize](https://products.aspose.app/barcode/recognize/img/aspose_recognize-app-48.png)](https://products.aspose.app/barcode/recognize)
 [**Generate Wi-Fi QR**](https://products.aspose.app/barcode/wifi-qr) | [**Embed Barcode**](https://products.aspose.app/barcode/embed) | [**Scan Barcode**](https://products.aspose.app/barcode/scan)
@@ -115,14 +115,15 @@
 *BarcodeApi* | [**get_barcode_generate**](docs/BarcodeApi.md#get_barcode_generate) | **GET** /barcode/generate | Generate barcode.
 *BarcodeApi* | [**get_barcode_recognize**](docs/BarcodeApi.md#get_barcode_recognize) | **GET** /barcode/{name}/recognize | Recognize barcode from a file on server.
 *BarcodeApi* | [**post_barcode_recognize_from_url_or_content**](docs/BarcodeApi.md#post_barcode_recognize_from_url_or_content) | **POST** /barcode/recognize | Recognize barcode from an url or from request body. Request body can contain raw data bytes of the image with content-type \&quot;application/octet-stream\&quot;. An image can also be passed as a form field.
 *BarcodeApi* | [**post_generate_multiple**](docs/BarcodeApi.md#post_generate_multiple) | **POST** /barcode/generateMultiple | Generate multiple barcodes and return in response stream
 *BarcodeApi* | [**put_barcode_generate_file**](docs/BarcodeApi.md#put_barcode_generate_file) | **PUT** /barcode/{name}/generate | Generate barcode and save on server (from query params or from file with json or xml content)
 *BarcodeApi* | [**put_barcode_recognize_from_body**](docs/BarcodeApi.md#put_barcode_recognize_from_body) | **PUT** /barcode/{name}/recognize | Recognition of a barcode from file on server with parameters in body.
 *BarcodeApi* | [**put_generate_multiple**](docs/BarcodeApi.md#put_generate_multiple) | **PUT** /barcode/{name}/generateMultiple | Generate image with multiple barcodes and put new file on server
+*BarcodeApi* | [**scan_barcode**](docs/BarcodeApi.md#scan_barcode) | **POST** /barcode/scan | Quickly scan a barcode from an image.
 *FileApi* | [**copy_file**](docs/FileApi.md#copy_file) | **PUT** /barcode/storage/file/copy/{srcPath} | Copy file
 *FileApi* | [**delete_file**](docs/FileApi.md#delete_file) | **DELETE** /barcode/storage/file/{path} | Delete file
 *FileApi* | [**download_file**](docs/FileApi.md#download_file) | **GET** /barcode/storage/file/{path} | Download file
 *FileApi* | [**move_file**](docs/FileApi.md#move_file) | **PUT** /barcode/storage/file/move/{srcPath} | Move file
 *FileApi* | [**upload_file**](docs/FileApi.md#upload_file) | **PUT** /barcode/storage/file/{path} | Upload file
 *FolderApi* | [**copy_folder**](docs/FolderApi.md#copy_folder) | **PUT** /barcode/storage/folder/copy/{srcPath} | Copy folder
 *FolderApi* | [**create_folder**](docs/FolderApi.md#create_folder) | **PUT** /barcode/storage/folder/{path} | Create the folder
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/__init__.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,11 @@
 # coding: utf-8
 
 # flake8: noqa: F401
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 from __future__ import absolute_import
 
 from aspose_barcode_cloud.rest import ApiException
 
 # import apis into sdk package
 from aspose_barcode_cloud.api.barcode_api import BarcodeApi
 from aspose_barcode_cloud.api.file_api import FileApi
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/api/barcode_api.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/barcode_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
 from __future__ import absolute_import, division
 
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
@@ -485,15 +461,15 @@
         :param bool allow_salt_and_pepper_filtering: Allows engine to recognize barcodes with salt and pepper noise type. Mode can remove small noise with white and black dots. # noqa: E501
         :param bool allow_white_spots_removing: Allows engine to recognize image without small white spots as additional scan. Mode helps to recognize noised image as well as median smoothing filtering. # noqa: E501
         :param bool check_more1_d_variants: Allows engine to recognize 1D barcodes with checksum by checking more recognition variants. Default value: False. # noqa: E501
         :param bool fast_scan_only: Allows engine for 1D barcodes to quickly recognize middle slice of an image and return result without using any time-consuming algorithms. Default value: False. # noqa: E501
         :param bool allow_additional_restorations: Allows engine using additional image restorations to recognize corrupted barcodes. At this time, it is used only in MicroPdf417 barcode type. Default value: False. # noqa: E501
         :param float region_likelihood_threshold_percent: Sets threshold for detected regions that may contain barcodes. Value 0.7 means that bottom 70% of possible regions are filtered out and not processed further. Region likelihood threshold must be between [0.05, 0.9] Use high values for clear images with few barcodes. Use low values for images with many barcodes or for noisy images. Low value may lead to a bigger recognition time. # noqa: E501
         :param list[int] scan_window_sizes: Scan window sizes in pixels. Allowed sizes are 10, 15, 20, 25, 30. Scanning with small window size takes more time and provides more accuracy but may fail in detecting very big barcodes. Combining of several window sizes can improve detection quality. # noqa: E501
-        :param float similarity: Similarity coefficient depends on how homogeneous barcodes are. Use high value for for clear barcodes. Use low values to detect barcodes that ara partly damaged or not lighten evenly. Similarity coefficient must be between [0.5, 0.9] # noqa: E501
+        :param float similarity: Similarity coefficient depends on how homogeneous barcodes are. Use high value for clear barcodes. Use low values to detect barcodes that ara partly damaged or not lighten evenly. Similarity coefficient must be between [0.5, 0.9] # noqa: E501
         :param bool skip_diagonal_search: Allows detector to skip search for diagonal barcodes. Setting it to false will increase detection time but allow to find diagonal barcodes that can be missed otherwise. Enabling of diagonal search leads to a bigger detection time. # noqa: E501
         :param bool read_tiny_barcodes: Allows engine to recognize tiny barcodes on large images. Ignored if AllowIncorrectBarcodes is set to True. Default value: False. # noqa: E501
         :param str australian_post_encoding_table: Interpreting Type for the Customer Information of AustralianPost BarCode.Default is CustomerInformationInterpretingType.Other. # noqa: E501
         :param bool ignore_ending_filling_patterns_for_c_table: The flag which force AustraliaPost decoder to ignore last filling patterns in Customer Information Field during decoding as CTable method. CTable encoding method does not have any gaps in encoding table and sequence \"333\" of filling patterns is decoded as letter \"z\". # noqa: E501
         :param str storage: The image storage. # noqa: E501
         :param str folder: The image folder. # noqa: E501
         :param async_req bool
@@ -861,15 +837,15 @@
         :param bool allow_salt_and_pepper_filtering: Allows engine to recognize barcodes with salt and pepper noise type. Mode can remove small noise with white and black dots. # noqa: E501
         :param bool allow_white_spots_removing: Allows engine to recognize image without small white spots as additional scan. Mode helps to recognize noised image as well as median smoothing filtering. # noqa: E501
         :param bool check_more1_d_variants: Allows engine to recognize 1D barcodes with checksum by checking more recognition variants. Default value: False. # noqa: E501
         :param bool fast_scan_only: Allows engine for 1D barcodes to quickly recognize middle slice of an image and return result without using any time-consuming algorithms. Default value: False. # noqa: E501
         :param bool allow_additional_restorations: Allows engine using additional image restorations to recognize corrupted barcodes. At this time, it is used only in MicroPdf417 barcode type. Default value: False. # noqa: E501
         :param float region_likelihood_threshold_percent: Sets threshold for detected regions that may contain barcodes. Value 0.7 means that bottom 70% of possible regions are filtered out and not processed further. Region likelihood threshold must be between [0.05, 0.9] Use high values for clear images with few barcodes. Use low values for images with many barcodes or for noisy images. Low value may lead to a bigger recognition time. # noqa: E501
         :param list[int] scan_window_sizes: Scan window sizes in pixels. Allowed sizes are 10, 15, 20, 25, 30. Scanning with small window size takes more time and provides more accuracy but may fail in detecting very big barcodes. Combining of several window sizes can improve detection quality. # noqa: E501
-        :param float similarity: Similarity coefficient depends on how homogeneous barcodes are. Use high value for for clear barcodes. Use low values to detect barcodes that ara partly damaged or not lighten evenly. Similarity coefficient must be between [0.5, 0.9] # noqa: E501
+        :param float similarity: Similarity coefficient depends on how homogeneous barcodes are. Use high value for clear barcodes. Use low values to detect barcodes that ara partly damaged or not lighten evenly. Similarity coefficient must be between [0.5, 0.9] # noqa: E501
         :param bool skip_diagonal_search: Allows detector to skip search for diagonal barcodes. Setting it to false will increase detection time but allow to find diagonal barcodes that can be missed otherwise. Enabling of diagonal search leads to a bigger detection time. # noqa: E501
         :param bool read_tiny_barcodes: Allows engine to recognize tiny barcodes on large images. Ignored if AllowIncorrectBarcodes is set to True. Default value: False. # noqa: E501
         :param str australian_post_encoding_table: Interpreting Type for the Customer Information of AustralianPost BarCode.Default is CustomerInformationInterpretingType.Other. # noqa: E501
         :param bool ignore_ending_filling_patterns_for_c_table: The flag which force AustraliaPost decoder to ignore last filling patterns in Customer Information Field during decoding as CTable method. CTable encoding method does not have any gaps in encoding table and sequence \"333\" of filling patterns is decoded as letter \"z\". # noqa: E501
         :param str url: The image file url. # noqa: E501
         :param file image: Image data # noqa: E501
         :param async_req bool
@@ -1881,7 +1857,109 @@
             auth_settings=auth_settings,
             async_req=params.get("async_req"),
             _return_http_data_only=params.get("_return_http_data_only"),
             _preload_content=params.get("_preload_content", True),
             _request_timeout=params.get("_request_timeout"),
             collection_formats=collection_formats,
         )
+
+    def scan_barcode(self, image_file, decode_types=None, timeout=None, async_req=False, **kwargs):
+        """Quickly scan a barcode from an image.
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = BarcodeApi().scan_barcode(image_file, async_req=True)
+        >>> result = thread.get()
+
+        :param file image_file: Image as file # noqa: E501
+        :param list[DecodeBarcodeType] decode_types: Types of barcode to recognize # noqa: E501
+        :param int timeout: Timeout of recognition process in milliseconds.  Default value is 15_000 (15 seconds).  Maximum value is 30_000 (1/2 minute).  In case of a timeout RequestTimeout (408) status will be returned.  Try reducing the image size to avoid timeout. # noqa: E501
+        :param async_req bool
+        :return: BarcodeResponseList
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs["_return_http_data_only"] = True
+        if async_req:
+            return self.scan_barcode_with_http_info(image_file, decode_types=decode_types, timeout=timeout, **kwargs)
+        else:
+            (data) = self.scan_barcode_with_http_info(image_file, decode_types=decode_types, timeout=timeout, **kwargs)
+            return data
+
+    def scan_barcode_with_http_info(self, image_file, **kwargs):
+        """Quickly scan a barcode from an image.
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = BarcodeApi().scan_barcode_with_http_info(image_file, async_req=True)
+        >>> result = thread.get()
+
+        :param file image_file: Image as file # noqa: E501
+        :return: BarcodeResponseList
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = {"image_file", "decode_types", "timeout"}
+        all_params.add("async_req")
+        all_params.add("_return_http_data_only")
+        all_params.add("_preload_content")
+        all_params.add("_request_timeout")
+
+        params = locals()
+        for key, val in six.iteritems(params["kwargs"]):
+            if key not in all_params:
+                raise TypeError("Got an unexpected keyword argument '%s'" " to method scan_barcode" % key)
+            if val is None:
+                continue
+
+            params[key] = val
+        del params["kwargs"]
+        # verify the required parameter "image_file" is set
+        if "image_file" not in params or params["image_file"] is None:
+            raise ValueError("Missing the required parameter 'image_file' when calling 'scan_barcode'")
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+        if "image_file" in params:
+            local_var_files["imageFile"] = params["image_file"]
+        if "decode_types" in params:
+            form_params.append(("decodeTypes", params["decode_types"]))
+            collection_formats["decodeTypes"] = "multi"
+        if "timeout" in params:
+            form_params.append(("timeout", params["timeout"]))
+
+        body_params = None
+        # HTTP header "Accept"
+        header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
+
+        # HTTP header "Content-Type"
+        header_params["Content-Type"] = self.api_client.select_header_content_type(["multipart/form-data"])
+
+        # Authentication setting
+        auth_settings = ["JWT"]
+
+        return self.api_client.call_api(
+            "/barcode/scan",
+            "POST",
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type="BarcodeResponseList",
+            auth_settings=auth_settings,
+            async_req=params.get("async_req"),
+            _return_http_data_only=params.get("_return_http_data_only"),
+            _preload_content=params.get("_preload_content", True),
+            _request_timeout=params.get("_request_timeout"),
+            collection_formats=collection_formats,
+        )
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/api/file_api.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/file_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
 from __future__ import absolute_import, division
 
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/api/folder_api.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/folder_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
 from __future__ import absolute_import, division
 
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/api/storage_api.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api/storage_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
 from __future__ import absolute_import, division
 
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/api_client.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,8 @@
 # coding: utf-8
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
 
 from __future__ import absolute_import, division
 
 import datetime
 import io
 import json
 import mimetypes
@@ -86,21 +63,21 @@
         self.configuration = configuration
 
         # Use the pool property to lazily initialize the ThreadPool.
         self._pool = None
         self.rest_client = RESTClientObject(configuration)
         self.default_headers = {
             "x-aspose-client": "python sdk",
-            "x-aspose-client-version": "24.3.0",
+            "x-aspose-client-version": "24.4.0",
         }
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "Aspose-Barcode-SDK/24.3.0/python"
+        self.user_agent = "Aspose-Barcode-SDK/24.4.0/python"
 
     def __del__(self):
         self.rest_client.close()
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/configuration.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/configuration.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
 from __future__ import absolute_import, division
 
 import contextlib
 import copy
 import json
 import logging
 import multiprocessing
@@ -282,15 +258,15 @@
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
             "Version of the API: 3.0\n"
-            "SDK Package Version: 24.3.0".format(env=sys.platform, pyversion=sys.version)
+            "SDK Package Version: 24.4.0".format(env=sys.platform, pyversion=sys.version)
         )
 
     @staticmethod
     def fetch_token(client_id, client_secret, token_url):
         with contextlib.closing(
             RESTClientObject(Configuration(client_id=client_id, client_secret=client_secret, token_url=token_url))
         ) as client:
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/__init__.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,10 @@
 # coding: utf-8
 
 # flake8: noqa
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
 
 from __future__ import absolute_import
 
 # import models into model package
 from aspose_barcode_cloud.models.api_error import ApiError
 from aspose_barcode_cloud.models.api_error_response import ApiErrorResponse
 from aspose_barcode_cloud.models.australian_post_params import AustralianPostParams
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/api_error.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/api_error.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/auto_size_mode.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/coupon_params.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,65 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
 
 
-class AutoSizeMode(object):
+class CouponParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
-    allowed enum values
-    """
-    NONE = "None"
-    NEAREST = "Nearest"
-    INTERPOLATION = "Interpolation"
-
-    """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {}
+    swagger_types = {"supplement_space": "float"}
+
+    attribute_map = {"supplement_space": "SupplementSpace"}
 
-    attribute_map = {}
+    def __init__(self, supplement_space=None):  # noqa: E501
+        """CouponParams - a model defined in Swagger"""  # noqa: E501
 
-    def __init__(self):  # noqa: E501
-        """AutoSizeMode - a model defined in Swagger"""  # noqa: E501
+        self._supplement_space = None
         self.discriminator = None
 
+        if supplement_space is not None:
+            self.supplement_space = supplement_space
+
+    @property
+    def supplement_space(self):
+        """Gets the supplement_space of this CouponParams.  # noqa: E501
+
+        Space between main the BarCode and supplement BarCode in Unit value.  # noqa: E501
+
+        :return: The supplement_space of this CouponParams.  # noqa: E501
+        :rtype: float
+        """
+        return self._supplement_space
+
+    @supplement_space.setter
+    def supplement_space(self, supplement_space):
+        """Sets the supplement_space of this CouponParams.
+
+        Space between main the BarCode and supplement BarCode in Unit value.  # noqa: E501
+
+        :param supplement_space: The supplement_space of this CouponParams.  # noqa: E501
+        :type: float
+        """
+
+        self._supplement_space = supplement_space
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -75,15 +71,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(AutoSizeMode, dict):
+        if issubclass(CouponParams, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -91,15 +87,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AutoSizeMode):
+        if not isinstance(other, CouponParams):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/available_graphics_unit.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/preset_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,45 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
 
 
-class AvailableGraphicsUnit(object):
+class PresetType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    PIXEL = "Pixel"
-    POINT = "Point"
-    INCH = "Inch"
-    MILLIMETER = "Millimeter"
+    HIGHPERFORMANCE = "HighPerformance"
+    NORMALQUALITY = "NormalQuality"
+    HIGHQUALITYDETECTION = "HighQualityDetection"
+    MAXQUALITYDETECTION = "MaxQualityDetection"
+    HIGHQUALITY = "HighQuality"
+    MAXBARCODES = "MaxBarCodes"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {}
 
     attribute_map = {}
 
     def __init__(self):  # noqa: E501
-        """AvailableGraphicsUnit - a model defined in Swagger"""  # noqa: E501
+        """PresetType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -76,15 +53,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(AvailableGraphicsUnit, dict):
+        if issubclass(PresetType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -92,15 +69,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AvailableGraphicsUnit):
+        if not isinstance(other, PresetType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/aztec_encode_mode.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/itf14_border_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,44 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
 
 
-class AztecEncodeMode(object):
+class ITF14BorderType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    AUTO = "Auto"
-    BYTES = "Bytes"
-    EXTENDEDCODETEXT = "ExtendedCodetext"
+    NONE = "None"
+    FRAME = "Frame"
+    BAR = "Bar"
+    FRAMEOUT = "FrameOut"
+    BAROUT = "BarOut"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {}
 
     attribute_map = {}
 
     def __init__(self):  # noqa: E501
-        """AztecEncodeMode - a model defined in Swagger"""  # noqa: E501
+        """ITF14BorderType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -75,15 +52,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(AztecEncodeMode, dict):
+        if issubclass(ITF14BorderType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -91,15 +68,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AztecEncodeMode):
+        if not isinstance(other, ITF14BorderType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/aztec_params.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/aztec_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/barcode_response.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/han_xin_params.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,167 +1,152 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
 
 
-class BarcodeResponse(object):
+class HanXinParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {"barcode_value": "str", "type": "str", "region": "list[RegionPoint]", "checksum": "str"}
-
-    attribute_map = {"barcode_value": "BarcodeValue", "type": "Type", "region": "Region", "checksum": "Checksum"}
-
-    def __init__(self, barcode_value=None, type=None, region=None, checksum=None):  # noqa: E501
-        """BarcodeResponse - a model defined in Swagger"""  # noqa: E501
-
-        self._barcode_value = None
-        self._type = None
-        self._region = None
-        self._checksum = None
+    swagger_types = {
+        "encode_mode": "HanXinEncodeMode",
+        "error_level": "HanXinErrorLevel",
+        "version": "HanXinVersion",
+        "eci_encoding": "ECIEncodings",
+    }
+
+    attribute_map = {
+        "encode_mode": "EncodeMode",
+        "error_level": "ErrorLevel",
+        "version": "Version",
+        "eci_encoding": "ECIEncoding",
+    }
+
+    def __init__(self, encode_mode=None, error_level=None, version=None, eci_encoding=None):  # noqa: E501
+        """HanXinParams - a model defined in Swagger"""  # noqa: E501
+
+        self._encode_mode = None
+        self._error_level = None
+        self._version = None
+        self._eci_encoding = None
         self.discriminator = None
 
-        if barcode_value is not None:
-            self.barcode_value = barcode_value
-        if type is not None:
-            self.type = type
-        if region is not None:
-            self.region = region
-        if checksum is not None:
-            self.checksum = checksum
+        if encode_mode is not None:
+            self.encode_mode = encode_mode
+        if error_level is not None:
+            self.error_level = error_level
+        if version is not None:
+            self.version = version
+        if eci_encoding is not None:
+            self.eci_encoding = eci_encoding
 
     @property
-    def barcode_value(self):
-        """Gets the barcode_value of this BarcodeResponse.  # noqa: E501
+    def encode_mode(self):
+        """Gets the encode_mode of this HanXinParams.  # noqa: E501
 
-        Barcode data.  # noqa: E501
+        Encoding mode for XanXin barcodes. Default value: HanXinEncodeMode.Auto.  # noqa: E501
 
-        :return: The barcode_value of this BarcodeResponse.  # noqa: E501
-        :rtype: str
+        :return: The encode_mode of this HanXinParams.  # noqa: E501
+        :rtype: HanXinEncodeMode
         """
-        return self._barcode_value
+        return self._encode_mode
 
-    @barcode_value.setter
-    def barcode_value(self, barcode_value):
-        """Sets the barcode_value of this BarcodeResponse.
+    @encode_mode.setter
+    def encode_mode(self, encode_mode):
+        """Sets the encode_mode of this HanXinParams.
 
-        Barcode data.  # noqa: E501
+        Encoding mode for XanXin barcodes. Default value: HanXinEncodeMode.Auto.  # noqa: E501
 
-        :param barcode_value: The barcode_value of this BarcodeResponse.  # noqa: E501
-        :type: str
+        :param encode_mode: The encode_mode of this HanXinParams.  # noqa: E501
+        :type: HanXinEncodeMode
         """
 
-        self._barcode_value = barcode_value
+        self._encode_mode = encode_mode
 
     @property
-    def type(self):
-        """Gets the type of this BarcodeResponse.  # noqa: E501
+    def error_level(self):
+        """Gets the error_level of this HanXinParams.  # noqa: E501
 
-        Type of the barcode.  # noqa: E501
+        Allowed Han Xin error correction levels from L1 to L4. Default value: HanXinErrorLevel.L1.  # noqa: E501
 
-        :return: The type of this BarcodeResponse.  # noqa: E501
-        :rtype: str
+        :return: The error_level of this HanXinParams.  # noqa: E501
+        :rtype: HanXinErrorLevel
         """
-        return self._type
+        return self._error_level
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this BarcodeResponse.
+    @error_level.setter
+    def error_level(self, error_level):
+        """Sets the error_level of this HanXinParams.
 
-        Type of the barcode.  # noqa: E501
+        Allowed Han Xin error correction levels from L1 to L4. Default value: HanXinErrorLevel.L1.  # noqa: E501
 
-        :param type: The type of this BarcodeResponse.  # noqa: E501
-        :type: str
+        :param error_level: The error_level of this HanXinParams.  # noqa: E501
+        :type: HanXinErrorLevel
         """
 
-        self._type = type
+        self._error_level = error_level
 
     @property
-    def region(self):
-        """Gets the region of this BarcodeResponse.  # noqa: E501
+    def version(self):
+        """Gets the version of this HanXinParams.  # noqa: E501
 
-        Region with barcode.  # noqa: E501
+        Allowed Han Xin versions, Auto and Version01 - Version84. Default value: HanXinVersion.Auto.  # noqa: E501
 
-        :return: The region of this BarcodeResponse.  # noqa: E501
-        :rtype: list[RegionPoint]
+        :return: The version of this HanXinParams.  # noqa: E501
+        :rtype: HanXinVersion
         """
-        return self._region
+        return self._version
 
-    @region.setter
-    def region(self, region):
-        """Sets the region of this BarcodeResponse.
+    @version.setter
+    def version(self, version):
+        """Sets the version of this HanXinParams.
 
-        Region with barcode.  # noqa: E501
+        Allowed Han Xin versions, Auto and Version01 - Version84. Default value: HanXinVersion.Auto.  # noqa: E501
 
-        :param region: The region of this BarcodeResponse.  # noqa: E501
-        :type: list[RegionPoint]
+        :param version: The version of this HanXinParams.  # noqa: E501
+        :type: HanXinVersion
         """
 
-        self._region = region
+        self._version = version
 
     @property
-    def checksum(self):
-        """Gets the checksum of this BarcodeResponse.  # noqa: E501
+    def eci_encoding(self):
+        """Gets the eci_encoding of this HanXinParams.  # noqa: E501
 
-        Checksum of barcode.  # noqa: E501
+        Extended Channel Interpretation Identifiers. It is used to tell the barcode reader details about the used references for encoding the data in the symbol. Current implementation consists all well known charset encodings. Default value: ECIEncodings.ISO_8859_1  # noqa: E501
 
-        :return: The checksum of this BarcodeResponse.  # noqa: E501
-        :rtype: str
+        :return: The eci_encoding of this HanXinParams.  # noqa: E501
+        :rtype: ECIEncodings
         """
-        return self._checksum
+        return self._eci_encoding
 
-    @checksum.setter
-    def checksum(self, checksum):
-        """Sets the checksum of this BarcodeResponse.
+    @eci_encoding.setter
+    def eci_encoding(self, eci_encoding):
+        """Sets the eci_encoding of this HanXinParams.
 
-        Checksum of barcode.  # noqa: E501
+        Extended Channel Interpretation Identifiers. It is used to tell the barcode reader details about the used references for encoding the data in the symbol. Current implementation consists all well known charset encodings. Default value: ECIEncodings.ISO_8859_1  # noqa: E501
 
-        :param checksum: The checksum of this BarcodeResponse.  # noqa: E501
-        :type: str
+        :param eci_encoding: The eci_encoding of this HanXinParams.  # noqa: E501
+        :type: ECIEncodings
         """
 
-        self._checksum = checksum
+        self._eci_encoding = eci_encoding
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -174,15 +159,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(BarcodeResponse, dict):
+        if issubclass(HanXinParams, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -190,15 +175,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, BarcodeResponse):
+        if not isinstance(other, HanXinParams):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/barcode_response_list.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/encode_barcode_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,113 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
 
 
-class BarcodeResponseList(object):
+class EncodeBarcodeType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
+    allowed enum values
+    """
+    CODABAR = "Codabar"
+    CODE11 = "Code11"
+    CODE39STANDARD = "Code39Standard"
+    CODE39EXTENDED = "Code39Extended"
+    CODE93STANDARD = "Code93Standard"
+    CODE93EXTENDED = "Code93Extended"
+    CODE128 = "Code128"
+    GS1CODE128 = "GS1Code128"
+    EAN8 = "EAN8"
+    EAN13 = "EAN13"
+    EAN14 = "EAN14"
+    SCC14 = "SCC14"
+    SSCC18 = "SSCC18"
+    UPCA = "UPCA"
+    UPCE = "UPCE"
+    ISBN = "ISBN"
+    ISSN = "ISSN"
+    ISMN = "ISMN"
+    STANDARD2OF5 = "Standard2of5"
+    INTERLEAVED2OF5 = "Interleaved2of5"
+    MATRIX2OF5 = "Matrix2of5"
+    ITALIANPOST25 = "ItalianPost25"
+    IATA2OF5 = "IATA2of5"
+    ITF14 = "ITF14"
+    ITF6 = "ITF6"
+    MSI = "MSI"
+    VIN = "VIN"
+    DEUTSCHEPOSTIDENTCODE = "DeutschePostIdentcode"
+    DEUTSCHEPOSTLEITCODE = "DeutschePostLeitcode"
+    OPC = "OPC"
+    PZN = "PZN"
+    CODE16K = "Code16K"
+    PHARMACODE = "Pharmacode"
+    DATAMATRIX = "DataMatrix"
+    QR = "QR"
+    AZTEC = "Aztec"
+    PDF417 = "Pdf417"
+    MACROPDF417 = "MacroPdf417"
+    AUSTRALIAPOST = "AustraliaPost"
+    POSTNET = "Postnet"
+    PLANET = "Planet"
+    ONECODE = "OneCode"
+    RM4SCC = "RM4SCC"
+    DATABAROMNIDIRECTIONAL = "DatabarOmniDirectional"
+    DATABARTRUNCATED = "DatabarTruncated"
+    DATABARLIMITED = "DatabarLimited"
+    DATABAREXPANDED = "DatabarExpanded"
+    SINGAPOREPOST = "SingaporePost"
+    GS1DATAMATRIX = "GS1DataMatrix"
+    AUSTRALIANPOSTEPARCEL = "AustralianPosteParcel"
+    SWISSPOSTPARCEL = "SwissPostParcel"
+    PATCHCODE = "PatchCode"
+    DATABAREXPANDEDSTACKED = "DatabarExpandedStacked"
+    DATABARSTACKED = "DatabarStacked"
+    DATABARSTACKEDOMNIDIRECTIONAL = "DatabarStackedOmniDirectional"
+    MICROPDF417 = "MicroPdf417"
+    GS1QR = "GS1QR"
+    MAXICODE = "MaxiCode"
+    CODE32 = "Code32"
+    DATALOGIC2OF5 = "DataLogic2of5"
+    DOTCODE = "DotCode"
+    DUTCHKIX = "DutchKIX"
+    UPCAGS1CODE128COUPON = "UpcaGs1Code128Coupon"
+    UPCAGS1DATABARCOUPON = "UpcaGs1DatabarCoupon"
+    CODABLOCKF = "CodablockF"
+    GS1CODABLOCKF = "GS1CodablockF"
+    MAILMARK = "Mailmark"
+    GS1DOTCODE = "GS1DotCode"
+    HANXIN = "HanXin"
+    GS1HANXIN = "GS1HanXin"
+    GS1AZTEC = "GS1Aztec"
+    GS1MICROPDF417 = "GS1MicroPdf417"
+
+    """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {"barcodes": "list[BarcodeResponse]"}
-
-    attribute_map = {"barcodes": "Barcodes"}
+    swagger_types = {}
 
-    def __init__(self, barcodes=None):  # noqa: E501
-        """BarcodeResponseList - a model defined in Swagger"""  # noqa: E501
+    attribute_map = {}
 
-        self._barcodes = None
+    def __init__(self):  # noqa: E501
+        """EncodeBarcodeType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
-        if barcodes is not None:
-            self.barcodes = barcodes
-
-    @property
-    def barcodes(self):
-        """Gets the barcodes of this BarcodeResponseList.  # noqa: E501
-
-        List of barcodes which are present in image.  # noqa: E501
-
-        :return: The barcodes of this BarcodeResponseList.  # noqa: E501
-        :rtype: list[BarcodeResponse]
-        """
-        return self._barcodes
-
-    @barcodes.setter
-    def barcodes(self, barcodes):
-        """Sets the barcodes of this BarcodeResponseList.
-
-        List of barcodes which are present in image.  # noqa: E501
-
-        :param barcodes: The barcodes of this BarcodeResponseList.  # noqa: E501
-        :type: list[BarcodeResponse]
-        """
-
-        self._barcodes = barcodes
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -96,15 +119,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(BarcodeResponseList, dict):
+        if issubclass(EncodeBarcodeType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -112,15 +135,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, BarcodeResponseList):
+        if not isinstance(other, EncodeBarcodeType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/border_dash_style.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/eci_encodings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,66 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
 
 
-class BorderDashStyle(object):
+class ECIEncodings(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    SOLID = "Solid"
-    DASH = "Dash"
-    DOT = "Dot"
-    DASHDOT = "DashDot"
-    DASHDOTDOT = "DashDotDot"
+    NONE = "NONE"
+    ISO_8859_1 = "ISO_8859_1"
+    ISO_8859_2 = "ISO_8859_2"
+    ISO_8859_3 = "ISO_8859_3"
+    ISO_8859_4 = "ISO_8859_4"
+    ISO_8859_5 = "ISO_8859_5"
+    ISO_8859_6 = "ISO_8859_6"
+    ISO_8859_7 = "ISO_8859_7"
+    ISO_8859_8 = "ISO_8859_8"
+    ISO_8859_9 = "ISO_8859_9"
+    ISO_8859_10 = "ISO_8859_10"
+    ISO_8859_11 = "ISO_8859_11"
+    ISO_8859_13 = "ISO_8859_13"
+    ISO_8859_14 = "ISO_8859_14"
+    ISO_8859_15 = "ISO_8859_15"
+    ISO_8859_16 = "ISO_8859_16"
+    SHIFT_JIS = "Shift_JIS"
+    WIN1250 = "Win1250"
+    WIN1251 = "Win1251"
+    WIN1252 = "Win1252"
+    WIN1256 = "Win1256"
+    UTF16BE = "UTF16BE"
+    UTF8 = "UTF8"
+    US_ASCII = "US_ASCII"
+    BIG5 = "Big5"
+    GB18030 = "GB18030"
+    EUC_KR = "EUC_KR"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {}
 
     attribute_map = {}
 
     def __init__(self):  # noqa: E501
-        """BorderDashStyle - a model defined in Swagger"""  # noqa: E501
+        """ECIEncodings - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -77,15 +74,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(BorderDashStyle, dict):
+        if issubclass(ECIEncodings, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -93,15 +90,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, BorderDashStyle):
+        if not isinstance(other, ECIEncodings):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/caption_params.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/dot_code_params.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,263 +1,216 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
 
 
-class CaptionParams(object):
+class DotCodeParams(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        "text": "str",
-        "alignment": "TextAlignment",
-        "color": "str",
-        "visible": "bool",
-        "font": "FontParams",
-        "padding": "Padding",
-        "no_wrap": "bool",
+        "aspect_ratio": "float",
+        "columns": "int",
+        "encode_mode": "DotCodeEncodeMode",
+        "eci_encoding": "ECIEncodings",
+        "is_reader_initialization": "bool",
+        "rows": "int",
     }
 
     attribute_map = {
-        "text": "Text",
-        "alignment": "Alignment",
-        "color": "Color",
-        "visible": "Visible",
-        "font": "Font",
-        "padding": "Padding",
-        "no_wrap": "NoWrap",
+        "aspect_ratio": "AspectRatio",
+        "columns": "Columns",
+        "encode_mode": "EncodeMode",
+        "eci_encoding": "ECIEncoding",
+        "is_reader_initialization": "IsReaderInitialization",
+        "rows": "Rows",
     }
 
     def __init__(
-        self, text=None, alignment=None, color=None, visible=None, font=None, padding=None, no_wrap=None
+        self,
+        aspect_ratio=None,
+        columns=None,
+        encode_mode=None,
+        eci_encoding=None,
+        is_reader_initialization=None,
+        rows=None,
     ):  # noqa: E501
-        """CaptionParams - a model defined in Swagger"""  # noqa: E501
+        """DotCodeParams - a model defined in Swagger"""  # noqa: E501
 
-        self._text = None
-        self._alignment = None
-        self._color = None
-        self._visible = None
-        self._font = None
-        self._padding = None
-        self._no_wrap = None
+        self._aspect_ratio = None
+        self._columns = None
+        self._encode_mode = None
+        self._eci_encoding = None
+        self._is_reader_initialization = None
+        self._rows = None
         self.discriminator = None
 
-        if text is not None:
-            self.text = text
-        if alignment is not None:
-            self.alignment = alignment
-        if color is not None:
-            self.color = color
-        if visible is not None:
-            self.visible = visible
-        if font is not None:
-            self.font = font
-        if padding is not None:
-            self.padding = padding
-        if no_wrap is not None:
-            self.no_wrap = no_wrap
+        if aspect_ratio is not None:
+            self.aspect_ratio = aspect_ratio
+        if columns is not None:
+            self.columns = columns
+        if encode_mode is not None:
+            self.encode_mode = encode_mode
+        if eci_encoding is not None:
+            self.eci_encoding = eci_encoding
+        if is_reader_initialization is not None:
+            self.is_reader_initialization = is_reader_initialization
+        if rows is not None:
+            self.rows = rows
 
     @property
-    def text(self):
-        """Gets the text of this CaptionParams.  # noqa: E501
+    def aspect_ratio(self):
+        """Gets the aspect_ratio of this DotCodeParams.  # noqa: E501
 
-        Caption text.  # noqa: E501
+        Height/Width ratio of 2D BarCode module.  # noqa: E501
 
-        :return: The text of this CaptionParams.  # noqa: E501
-        :rtype: str
+        :return: The aspect_ratio of this DotCodeParams.  # noqa: E501
+        :rtype: float
         """
-        return self._text
+        return self._aspect_ratio
 
-    @text.setter
-    def text(self, text):
-        """Sets the text of this CaptionParams.
+    @aspect_ratio.setter
+    def aspect_ratio(self, aspect_ratio):
+        """Sets the aspect_ratio of this DotCodeParams.
 
-        Caption text.  # noqa: E501
+        Height/Width ratio of 2D BarCode module.  # noqa: E501
 
-        :param text: The text of this CaptionParams.  # noqa: E501
-        :type: str
+        :param aspect_ratio: The aspect_ratio of this DotCodeParams.  # noqa: E501
+        :type: float
         """
 
-        self._text = text
+        self._aspect_ratio = aspect_ratio
 
     @property
-    def alignment(self):
-        """Gets the alignment of this CaptionParams.  # noqa: E501
+    def columns(self):
+        """Gets the columns of this DotCodeParams.  # noqa: E501
 
-        Text alignment.  # noqa: E501
+        Identifies columns count. Sum of the number of rows plus the number of columns of a DotCode symbol must be odd. Number of columns must be at least 5.  # noqa: E501
 
-        :return: The alignment of this CaptionParams.  # noqa: E501
-        :rtype: TextAlignment
+        :return: The columns of this DotCodeParams.  # noqa: E501
+        :rtype: int
         """
-        return self._alignment
+        return self._columns
 
-    @alignment.setter
-    def alignment(self, alignment):
-        """Sets the alignment of this CaptionParams.
+    @columns.setter
+    def columns(self, columns):
+        """Sets the columns of this DotCodeParams.
 
-        Text alignment.  # noqa: E501
+        Identifies columns count. Sum of the number of rows plus the number of columns of a DotCode symbol must be odd. Number of columns must be at least 5.  # noqa: E501
 
-        :param alignment: The alignment of this CaptionParams.  # noqa: E501
-        :type: TextAlignment
+        :param columns: The columns of this DotCodeParams.  # noqa: E501
+        :type: int
         """
 
-        self._alignment = alignment
+        self._columns = columns
 
     @property
-    def color(self):
-        """Gets the color of this CaptionParams.  # noqa: E501
+    def encode_mode(self):
+        """Gets the encode_mode of this DotCodeParams.  # noqa: E501
 
-        Text color.  # noqa: E501
+        Identifies DotCode encode mode. Default value: Auto.  # noqa: E501
 
-        :return: The color of this CaptionParams.  # noqa: E501
-        :rtype: str
+        :return: The encode_mode of this DotCodeParams.  # noqa: E501
+        :rtype: DotCodeEncodeMode
         """
-        return self._color
+        return self._encode_mode
 
-    @color.setter
-    def color(self, color):
-        """Sets the color of this CaptionParams.
+    @encode_mode.setter
+    def encode_mode(self, encode_mode):
+        """Sets the encode_mode of this DotCodeParams.
 
-        Text color.  # noqa: E501
+        Identifies DotCode encode mode. Default value: Auto.  # noqa: E501
 
-        :param color: The color of this CaptionParams.  # noqa: E501
-        :type: str
+        :param encode_mode: The encode_mode of this DotCodeParams.  # noqa: E501
+        :type: DotCodeEncodeMode
         """
 
-        self._color = color
+        self._encode_mode = encode_mode
 
     @property
-    def visible(self):
-        """Gets the visible of this CaptionParams.  # noqa: E501
+    def eci_encoding(self):
+        """Gets the eci_encoding of this DotCodeParams.  # noqa: E501
 
-        Is caption visible.  # noqa: E501
+        Identifies ECI encoding. Used when DotCodeEncodeMode is Auto. Default value: ISO-8859-1.  # noqa: E501
 
-        :return: The visible of this CaptionParams.  # noqa: E501
-        :rtype: bool
+        :return: The eci_encoding of this DotCodeParams.  # noqa: E501
+        :rtype: ECIEncodings
         """
-        return self._visible
+        return self._eci_encoding
 
-    @visible.setter
-    def visible(self, visible):
-        """Sets the visible of this CaptionParams.
+    @eci_encoding.setter
+    def eci_encoding(self, eci_encoding):
+        """Sets the eci_encoding of this DotCodeParams.
 
-        Is caption visible.  # noqa: E501
+        Identifies ECI encoding. Used when DotCodeEncodeMode is Auto. Default value: ISO-8859-1.  # noqa: E501
 
-        :param visible: The visible of this CaptionParams.  # noqa: E501
-        :type: bool
+        :param eci_encoding: The eci_encoding of this DotCodeParams.  # noqa: E501
+        :type: ECIEncodings
         """
 
-        self._visible = visible
+        self._eci_encoding = eci_encoding
 
     @property
-    def font(self):
-        """Gets the font of this CaptionParams.  # noqa: E501
-
-        Font.  # noqa: E501
-
-        :return: The font of this CaptionParams.  # noqa: E501
-        :rtype: FontParams
-        """
-        return self._font
-
-    @font.setter
-    def font(self, font):
-        """Sets the font of this CaptionParams.
+    def is_reader_initialization(self):
+        """Gets the is_reader_initialization of this DotCodeParams.  # noqa: E501
 
-        Font.  # noqa: E501
+        Indicates whether code is used for instruct reader to interpret the following data as instructions for initialization or reprogramming of the bar code reader. Default value is false.  # noqa: E501
 
-        :param font: The font of this CaptionParams.  # noqa: E501
-        :type: FontParams
-        """
-
-        self._font = font
-
-    @property
-    def padding(self):
-        """Gets the padding of this CaptionParams.  # noqa: E501
-
-        Padding.  # noqa: E501
-
-        :return: The padding of this CaptionParams.  # noqa: E501
-        :rtype: Padding
+        :return: The is_reader_initialization of this DotCodeParams.  # noqa: E501
+        :rtype: bool
         """
-        return self._padding
+        return self._is_reader_initialization
 
-    @padding.setter
-    def padding(self, padding):
-        """Sets the padding of this CaptionParams.
+    @is_reader_initialization.setter
+    def is_reader_initialization(self, is_reader_initialization):
+        """Sets the is_reader_initialization of this DotCodeParams.
 
-        Padding.  # noqa: E501
+        Indicates whether code is used for instruct reader to interpret the following data as instructions for initialization or reprogramming of the bar code reader. Default value is false.  # noqa: E501
 
-        :param padding: The padding of this CaptionParams.  # noqa: E501
-        :type: Padding
+        :param is_reader_initialization: The is_reader_initialization of this DotCodeParams.  # noqa: E501
+        :type: bool
         """
 
-        self._padding = padding
+        self._is_reader_initialization = is_reader_initialization
 
     @property
-    def no_wrap(self):
-        """Gets the no_wrap of this CaptionParams.  # noqa: E501
+    def rows(self):
+        """Gets the rows of this DotCodeParams.  # noqa: E501
 
-        Specify word wraps (line breaks) within text. Default value: false.  # noqa: E501
+        Identifies rows count. Sum of the number of rows plus the number of columns of a DotCode symbol must be odd. Number of rows must be at least 5.  # noqa: E501
 
-        :return: The no_wrap of this CaptionParams.  # noqa: E501
-        :rtype: bool
+        :return: The rows of this DotCodeParams.  # noqa: E501
+        :rtype: int
         """
-        return self._no_wrap
+        return self._rows
 
-    @no_wrap.setter
-    def no_wrap(self, no_wrap):
-        """Sets the no_wrap of this CaptionParams.
+    @rows.setter
+    def rows(self, rows):
+        """Sets the rows of this DotCodeParams.
 
-        Specify word wraps (line breaks) within text. Default value: false.  # noqa: E501
+        Identifies rows count. Sum of the number of rows plus the number of columns of a DotCode symbol must be odd. Number of rows must be at least 5.  # noqa: E501
 
-        :param no_wrap: The no_wrap of this CaptionParams.  # noqa: E501
-        :type: bool
+        :param rows: The rows of this DotCodeParams.  # noqa: E501
+        :type: int
         """
 
-        self._no_wrap = no_wrap
+        self._rows = rows
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -270,15 +223,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(CaptionParams, dict):
+        if issubclass(DotCodeParams, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -286,15 +239,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CaptionParams):
+        if not isinstance(other, DotCodeParams):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/codabar_params.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/codabar_params.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/code128_params.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/decode_barcode_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,126 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
 
 
-class Code128Params(object):
+class DecodeBarcodeType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
+    allowed enum values
+    """
+    ALL = "all"
+    AUSTRALIAPOST = "AustraliaPost"
+    AZTEC = "Aztec"
+    ISBN = "ISBN"
+    CODABAR = "Codabar"
+    CODE11 = "Code11"
+    CODE128 = "Code128"
+    GS1CODE128 = "GS1Code128"
+    CODE39EXTENDED = "Code39Extended"
+    CODE39STANDARD = "Code39Standard"
+    CODE93EXTENDED = "Code93Extended"
+    CODE93STANDARD = "Code93Standard"
+    DATAMATRIX = "DataMatrix"
+    DEUTSCHEPOSTIDENTCODE = "DeutschePostIdentcode"
+    DEUTSCHEPOSTLEITCODE = "DeutschePostLeitcode"
+    EAN13 = "EAN13"
+    EAN14 = "EAN14"
+    EAN8 = "EAN8"
+    IATA2OF5 = "IATA2of5"
+    INTERLEAVED2OF5 = "Interleaved2of5"
+    ISSN = "ISSN"
+    ISMN = "ISMN"
+    ITALIANPOST25 = "ItalianPost25"
+    ITF14 = "ITF14"
+    ITF6 = "ITF6"
+    MACROPDF417 = "MacroPdf417"
+    MATRIX2OF5 = "Matrix2of5"
+    MSI = "MSI"
+    ONECODE = "OneCode"
+    OPC = "OPC"
+    PATCHCODE = "PatchCode"
+    PDF417 = "Pdf417"
+    MICROPDF417 = "MicroPdf417"
+    PLANET = "Planet"
+    POSTNET = "Postnet"
+    PZN = "PZN"
+    QR = "QR"
+    MICROQR = "MicroQR"
+    RM4SCC = "RM4SCC"
+    SCC14 = "SCC14"
+    SSCC18 = "SSCC18"
+    STANDARD2OF5 = "Standard2of5"
+    SUPPLEMENT = "Supplement"
+    UPCA = "UPCA"
+    UPCE = "UPCE"
+    VIN = "VIN"
+    PHARMACODE = "Pharmacode"
+    GS1DATAMATRIX = "GS1DataMatrix"
+    DATABAROMNIDIRECTIONAL = "DatabarOmniDirectional"
+    DATABARTRUNCATED = "DatabarTruncated"
+    DATABARLIMITED = "DatabarLimited"
+    DATABAREXPANDED = "DatabarExpanded"
+    SWISSPOSTPARCEL = "SwissPostParcel"
+    AUSTRALIANPOSTEPARCEL = "AustralianPosteParcel"
+    CODE16K = "Code16K"
+    DATABARSTACKEDOMNIDIRECTIONAL = "DatabarStackedOmniDirectional"
+    DATABARSTACKED = "DatabarStacked"
+    DATABAREXPANDEDSTACKED = "DatabarExpandedStacked"
+    COMPACTPDF417 = "CompactPdf417"
+    GS1QR = "GS1QR"
+    MAXICODE = "MaxiCode"
+    MICRE13B = "MicrE13B"
+    CODE32 = "Code32"
+    DATALOGIC2OF5 = "DataLogic2of5"
+    DOTCODE = "DotCode"
+    DUTCHKIX = "DutchKIX"
+    CODABLOCKF = "CodablockF"
+    MAILMARK = "Mailmark"
+    GS1DOTCODE = "GS1DotCode"
+    HIBCCODE39LIC = "HIBCCode39LIC"
+    HIBCCODE128LIC = "HIBCCode128LIC"
+    HIBCAZTECLIC = "HIBCAztecLIC"
+    HIBCDATAMATRIXLIC = "HIBCDataMatrixLIC"
+    HIBCQRLIC = "HIBCQRLIC"
+    HIBCCODE39PAS = "HIBCCode39PAS"
+    HIBCCODE128PAS = "HIBCCode128PAS"
+    HIBCAZTECPAS = "HIBCAztecPAS"
+    HIBCDATAMATRIXPAS = "HIBCDataMatrixPAS"
+    HIBCQRPAS = "HIBCQRPAS"
+    HANXIN = "HanXin"
+    GS1HANXIN = "GS1HanXin"
+    GS1AZTEC = "GS1Aztec"
+    GS1COMPOSITEBAR = "GS1CompositeBar"
+    GS1MICROPDF417 = "GS1MicroPdf417"
+    MOSTCOMMONLYUSED = "mostCommonlyUsed"
+
+    """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {"encode_mode": "Code128EncodeMode"}
-
-    attribute_map = {"encode_mode": "EncodeMode"}
+    swagger_types = {}
 
-    def __init__(self, encode_mode=None):  # noqa: E501
-        """Code128Params - a model defined in Swagger"""  # noqa: E501
+    attribute_map = {}
 
-        self._encode_mode = None
+    def __init__(self):  # noqa: E501
+        """DecodeBarcodeType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
-        if encode_mode is not None:
-            self.encode_mode = encode_mode
-
-    @property
-    def encode_mode(self):
-        """Gets the encode_mode of this Code128Params.  # noqa: E501
-
-        Encoding mode for Code128 barcodes. Code 128 specification Default value: Code128EncodeMode.Auto.  # noqa: E501
-
-        :return: The encode_mode of this Code128Params.  # noqa: E501
-        :rtype: Code128EncodeMode
-        """
-        return self._encode_mode
-
-    @encode_mode.setter
-    def encode_mode(self, encode_mode):
-        """Sets the encode_mode of this Code128Params.
-
-        Encoding mode for Code128 barcodes. Code 128 specification Default value: Code128EncodeMode.Auto.  # noqa: E501
-
-        :param encode_mode: The encode_mode of this Code128Params.  # noqa: E501
-        :type: Code128EncodeMode
-        """
-
-        self._encode_mode = encode_mode
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -96,15 +132,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(Code128Params, dict):
+        if issubclass(DecodeBarcodeType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -112,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Code128Params):
+        if not isinstance(other, DecodeBarcodeType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/code_location.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_matrix_ecc_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,46 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
 
 
-class CodeLocation(object):
+class DataMatrixEccType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    BELOW = "Below"
-    ABOVE = "Above"
-    NONE = "None"
+    ECCAUTO = "EccAuto"
+    ECC000 = "Ecc000"
+    ECC050 = "Ecc050"
+    ECC080 = "Ecc080"
+    ECC100 = "Ecc100"
+    ECC140 = "Ecc140"
+    ECC200 = "Ecc200"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {}
 
     attribute_map = {}
 
     def __init__(self):  # noqa: E501
-        """CodeLocation - a model defined in Swagger"""  # noqa: E501
+        """DataMatrixEccType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -75,15 +54,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(CodeLocation, dict):
+        if issubclass(DataMatrixEccType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -91,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CodeLocation):
+        if not isinstance(other, DataMatrixEccType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/data_bar_params.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_bar_params.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/data_matrix_params.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_matrix_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/error.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/error.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/file_version.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/file_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/font_mode.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/patch_format.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,44 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
 
 
-class FontMode(object):
+class PatchFormat(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    AUTO = "Auto"
-    MANUAL = "Manual"
+    PATCHONLY = "PatchOnly"
+    A4 = "A4"
+    A4_LANDSCAPE = "A4_LANDSCAPE"
+    US_LETTER = "US_Letter"
+    US_LETTER_LANDSCAPE = "US_Letter_LANDSCAPE"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {}
 
     attribute_map = {}
 
     def __init__(self):  # noqa: E501
-        """FontMode - a model defined in Swagger"""  # noqa: E501
+        """PatchFormat - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -74,15 +52,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(FontMode, dict):
+        if issubclass(PatchFormat, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -90,15 +68,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FontMode):
+        if not isinstance(other, PatchFormat):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/font_params.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/font_params.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/generator_params.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/generator_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/maxi_code_params.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/storage_file.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,141 +1,176 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
 
 
-class MaxiCodeParams(object):
+class StorageFile(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {"aspect_ratio": "float", "mode": "MaxiCodeMode", "encode_mode": "MaxiCodeEncodeMode"}
+    swagger_types = {"name": "str", "is_folder": "bool", "modified_date": "datetime", "size": "int", "path": "str"}
 
-    attribute_map = {"aspect_ratio": "AspectRatio", "mode": "Mode", "encode_mode": "EncodeMode"}
+    attribute_map = {
+        "name": "Name",
+        "is_folder": "IsFolder",
+        "modified_date": "ModifiedDate",
+        "size": "Size",
+        "path": "Path",
+    }
+
+    def __init__(self, name=None, is_folder=None, modified_date=None, size=None, path=None):  # noqa: E501
+        """StorageFile - a model defined in Swagger"""  # noqa: E501
+
+        self._name = None
+        self._is_folder = None
+        self._modified_date = None
+        self._size = None
+        self._path = None
+        self.discriminator = None
 
-    def __init__(self, aspect_ratio=None, mode=None, encode_mode=None):  # noqa: E501
-        """MaxiCodeParams - a model defined in Swagger"""  # noqa: E501
+        if name is not None:
+            self.name = name
+        self.is_folder = is_folder
+        if modified_date is not None:
+            self.modified_date = modified_date
+        self.size = size
+        if path is not None:
+            self.path = path
 
-        self._aspect_ratio = None
-        self._mode = None
-        self._encode_mode = None
-        self.discriminator = None
+    @property
+    def name(self):
+        """Gets the name of this StorageFile.  # noqa: E501
+
+        File or folder name.  # noqa: E501
+
+        :return: The name of this StorageFile.  # noqa: E501
+        :rtype: str
+        """
+        return self._name
+
+    @name.setter
+    def name(self, name):
+        """Sets the name of this StorageFile.
+
+        File or folder name.  # noqa: E501
+
+        :param name: The name of this StorageFile.  # noqa: E501
+        :type: str
+        """
+
+        self._name = name
+
+    @property
+    def is_folder(self):
+        """Gets the is_folder of this StorageFile.  # noqa: E501
+
+        True if it is a folder.  # noqa: E501
+
+        :return: The is_folder of this StorageFile.  # noqa: E501
+        :rtype: bool
+        """
+        return self._is_folder
+
+    @is_folder.setter
+    def is_folder(self, is_folder):
+        """Sets the is_folder of this StorageFile.
+
+        True if it is a folder.  # noqa: E501
+
+        :param is_folder: The is_folder of this StorageFile.  # noqa: E501
+        :type: bool
+        """
+        if is_folder is None:
+            raise ValueError("Invalid value for `is_folder`, must not be `None`")  # noqa: E501
 
-        if aspect_ratio is not None:
-            self.aspect_ratio = aspect_ratio
-        if mode is not None:
-            self.mode = mode
-        if encode_mode is not None:
-            self.encode_mode = encode_mode
+        self._is_folder = is_folder
 
     @property
-    def aspect_ratio(self):
-        """Gets the aspect_ratio of this MaxiCodeParams.  # noqa: E501
+    def modified_date(self):
+        """Gets the modified_date of this StorageFile.  # noqa: E501
 
-        Height/Width ratio of 2D BarCode module.  # noqa: E501
+        File or folder last modified DateTime.  # noqa: E501
 
-        :return: The aspect_ratio of this MaxiCodeParams.  # noqa: E501
-        :rtype: float
+        :return: The modified_date of this StorageFile.  # noqa: E501
+        :rtype: datetime
         """
-        return self._aspect_ratio
+        return self._modified_date
 
-    @aspect_ratio.setter
-    def aspect_ratio(self, aspect_ratio):
-        """Sets the aspect_ratio of this MaxiCodeParams.
+    @modified_date.setter
+    def modified_date(self, modified_date):
+        """Sets the modified_date of this StorageFile.
 
-        Height/Width ratio of 2D BarCode module.  # noqa: E501
+        File or folder last modified DateTime.  # noqa: E501
 
-        :param aspect_ratio: The aspect_ratio of this MaxiCodeParams.  # noqa: E501
-        :type: float
+        :param modified_date: The modified_date of this StorageFile.  # noqa: E501
+        :type: datetime
         """
 
-        self._aspect_ratio = aspect_ratio
+        self._modified_date = modified_date
 
     @property
-    def mode(self):
-        """Gets the mode of this MaxiCodeParams.  # noqa: E501
+    def size(self):
+        """Gets the size of this StorageFile.  # noqa: E501
 
-        Mode for MaxiCode barcodes.  # noqa: E501
+        File or folder size.  # noqa: E501
 
-        :return: The mode of this MaxiCodeParams.  # noqa: E501
-        :rtype: MaxiCodeMode
+        :return: The size of this StorageFile.  # noqa: E501
+        :rtype: int
         """
-        return self._mode
+        return self._size
 
-    @mode.setter
-    def mode(self, mode):
-        """Sets the mode of this MaxiCodeParams.
+    @size.setter
+    def size(self, size):
+        """Sets the size of this StorageFile.
 
-        Mode for MaxiCode barcodes.  # noqa: E501
+        File or folder size.  # noqa: E501
 
-        :param mode: The mode of this MaxiCodeParams.  # noqa: E501
-        :type: MaxiCodeMode
+        :param size: The size of this StorageFile.  # noqa: E501
+        :type: int
         """
+        if size is None:
+            raise ValueError("Invalid value for `size`, must not be `None`")  # noqa: E501
 
-        self._mode = mode
+        self._size = size
 
     @property
-    def encode_mode(self):
-        """Gets the encode_mode of this MaxiCodeParams.  # noqa: E501
+    def path(self):
+        """Gets the path of this StorageFile.  # noqa: E501
 
-        Encoding mode for MaxiCode barcodes.  # noqa: E501
+        File or folder path.  # noqa: E501
 
-        :return: The encode_mode of this MaxiCodeParams.  # noqa: E501
-        :rtype: MaxiCodeEncodeMode
+        :return: The path of this StorageFile.  # noqa: E501
+        :rtype: str
         """
-        return self._encode_mode
+        return self._path
 
-    @encode_mode.setter
-    def encode_mode(self, encode_mode):
-        """Sets the encode_mode of this MaxiCodeParams.
+    @path.setter
+    def path(self, path):
+        """Sets the path of this StorageFile.
 
-        Encoding mode for MaxiCode barcodes.  # noqa: E501
+        File or folder path.  # noqa: E501
 
-        :param encode_mode: The encode_mode of this MaxiCodeParams.  # noqa: E501
-        :type: MaxiCodeEncodeMode
+        :param path: The path of this StorageFile.  # noqa: E501
+        :type: str
         """
 
-        self._encode_mode = encode_mode
+        self._path = path
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -148,15 +183,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(MaxiCodeParams, dict):
+        if issubclass(StorageFile, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -164,15 +199,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MaxiCodeParams):
+        if not isinstance(other, StorageFile):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/patch_code_params.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/patch_code_params.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/pdf417_params.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/pdf417_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/qr_error_level.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/data_matrix_encode_mode.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,48 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
 
 
-class QRErrorLevel(object):
+class DataMatrixEncodeMode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    LEVELL = "LevelL"
-    LEVELM = "LevelM"
-    LEVELQ = "LevelQ"
-    LEVELH = "LevelH"
+    AUTO = "Auto"
+    ASCII = "ASCII"
+    FULL = "Full"
+    CUSTOM = "Custom"
+    C40 = "C40"
+    TEXT = "Text"
+    EDIFACT = "EDIFACT"
+    ANSIX12 = "ANSIX12"
+    EXTENDEDCODETEXT = "ExtendedCodetext"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {}
 
     attribute_map = {}
 
     def __init__(self):  # noqa: E501
-        """QRErrorLevel - a model defined in Swagger"""  # noqa: E501
+        """DataMatrixEncodeMode - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -76,15 +56,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(QRErrorLevel, dict):
+        if issubclass(DataMatrixEncodeMode, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -92,15 +72,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, QRErrorLevel):
+        if not isinstance(other, DataMatrixEncodeMode):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/qr_params.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/qr_params.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/qr_version.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/han_xin_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,17 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
 
 
-class QRVersion(object):
+class HanXinVersion(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
@@ -78,32 +53,72 @@
     VERSION34 = "Version34"
     VERSION35 = "Version35"
     VERSION36 = "Version36"
     VERSION37 = "Version37"
     VERSION38 = "Version38"
     VERSION39 = "Version39"
     VERSION40 = "Version40"
-    VERSIONM1 = "VersionM1"
-    VERSIONM2 = "VersionM2"
-    VERSIONM3 = "VersionM3"
-    VERSIONM4 = "VersionM4"
+    VERSION41 = "Version41"
+    VERSION42 = "Version42"
+    VERSION43 = "Version43"
+    VERSION44 = "Version44"
+    VERSION45 = "Version45"
+    VERSION46 = "Version46"
+    VERSION47 = "Version47"
+    VERSION48 = "Version48"
+    VERSION49 = "Version49"
+    VERSION50 = "Version50"
+    VERSION51 = "Version51"
+    VERSION52 = "Version52"
+    VERSION53 = "Version53"
+    VERSION54 = "Version54"
+    VERSION55 = "Version55"
+    VERSION56 = "Version56"
+    VERSION57 = "Version57"
+    VERSION58 = "Version58"
+    VERSION59 = "Version59"
+    VERSION60 = "Version60"
+    VERSION61 = "Version61"
+    VERSION62 = "Version62"
+    VERSION63 = "Version63"
+    VERSION64 = "Version64"
+    VERSION65 = "Version65"
+    VERSION66 = "Version66"
+    VERSION67 = "Version67"
+    VERSION68 = "Version68"
+    VERSION69 = "Version69"
+    VERSION70 = "Version70"
+    VERSION71 = "Version71"
+    VERSION72 = "Version72"
+    VERSION73 = "Version73"
+    VERSION74 = "Version74"
+    VERSION75 = "Version75"
+    VERSION76 = "Version76"
+    VERSION77 = "Version77"
+    VERSION78 = "Version78"
+    VERSION79 = "Version79"
+    VERSION80 = "Version80"
+    VERSION81 = "Version81"
+    VERSION82 = "Version82"
+    VERSION83 = "Version83"
+    VERSION84 = "Version84"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {}
 
     attribute_map = {}
 
     def __init__(self):  # noqa: E501
-        """QRVersion - a model defined in Swagger"""  # noqa: E501
+        """HanXinVersion - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -117,15 +132,15 @@
                     map(
                         lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
-        if issubclass(QRVersion, dict):
+        if issubclass(HanXinVersion, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -133,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, QRVersion):
+        if not isinstance(other, HanXinVersion):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/reader_params.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/reader_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
 
 
@@ -988,26 +963,26 @@
 
         self._scan_window_sizes = scan_window_sizes
 
     @property
     def similarity(self):
         """Gets the similarity of this ReaderParams.  # noqa: E501
 
-        Similarity coefficient depends on how homogeneous barcodes are. Use high value for for clear barcodes. Use low values to detect barcodes that ara partly damaged or not lighten evenly. Similarity coefficient must be between [0.5, 0.9]  # noqa: E501
+        Similarity coefficient depends on how homogeneous barcodes are. Use high value for clear barcodes. Use low values to detect barcodes that ara partly damaged or not lighten evenly. Similarity coefficient must be between [0.5, 0.9]  # noqa: E501
 
         :return: The similarity of this ReaderParams.  # noqa: E501
         :rtype: float
         """
         return self._similarity
 
     @similarity.setter
     def similarity(self, similarity):
         """Sets the similarity of this ReaderParams.
 
-        Similarity coefficient depends on how homogeneous barcodes are. Use high value for for clear barcodes. Use low values to detect barcodes that ara partly damaged or not lighten evenly. Similarity coefficient must be between [0.5, 0.9]  # noqa: E501
+        Similarity coefficient depends on how homogeneous barcodes are. Use high value for clear barcodes. Use low values to detect barcodes that ara partly damaged or not lighten evenly. Similarity coefficient must be between [0.5, 0.9]  # noqa: E501
 
         :param similarity: The similarity of this ReaderParams.  # noqa: E501
         :type: float
         """
 
         self._similarity = similarity
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/models/result_image_info.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/models/result_image_info.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
-
 import pprint
 import re  # noqa: F401
 import warnings  # noqa: F401
 
 import six
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud/rest.py` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud/rest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,9 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
 from __future__ import absolute_import, division
 
 import io
 import json
 import logging
 import re
 import ssl
@@ -61,14 +37,15 @@
 
     def getheader(self, name, default=None):
         """Returns a given response header."""
         return self.urllib3_response.getheader(name, default)
 
 
 class RESTClientObject(object):
+
     def __init__(self, configuration, pools_size=4, maxsize=None):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680  # noqa: E501
         # maxsize is the number of requests to host that are allowed in parallel  # noqa: E501
         # Custom SSL certificates and client certificates: http://urllib3.readthedocs.io/en/latest/advanced-usage.html  # noqa: E501
 
@@ -380,14 +357,15 @@
         )
 
     def close(self):
         self.pool_manager.clear()
 
 
 class ApiException(Exception):
+
     def __init__(self, status=0, reason=None, http_resp=None):
         # type: (int, str, RESTResponse) -> None
         if http_resp:
             self.status = http_resp.status
             self.reason = http_resp.reason
             self.body = http_resp.data
         else:
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud.egg-info/PKG-INFO` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-barcode-cloud
-Version: 24.3.0
+Version: 24.4.0
 Summary: Aspose.Barcode Cloud API Reference
 Home-page: https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Author: Aspose Barcode Cloud
 License: MIT
 Project-URL: Source With Tests, https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python
 Project-URL: Website, https://www.aspose.cloud
 Project-URL: Product Home, https://products.aspose.cloud/barcode/
@@ -39,15 +39,15 @@
 # Aspose.BarCode Cloud SDK for Python
 
 [![License](https://img.shields.io/github/license/aspose-barcode-cloud/aspose-barcode-cloud-python)](LICENSE)
 [![Python package](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/aspose-barcode-cloud/aspose-barcode-cloud-python/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/aspose-barcode-cloud)](https://pypi.org/project/aspose-barcode-cloud/)
 
 - API version: 3.0
-- Package version: 24.3.0
+- Package version: 24.4.0
 
 ## Demo applications
 
 [Scan QR](https://products.aspose.app/barcode/scanqr) | [Generate Barcode](https://products.aspose.app/barcode/generate) | [Recognize Barcode](https://products.aspose.app/barcode/recognize)
 :---: | :---: | :---:
 [![ScanQR](https://products.aspose.app/barcode/scanqr/img/aspose_scanqr-app-48.png)](https://products.aspose.app/barcode/scanqr) | [![Generate](https://products.aspose.app/barcode/generate/img/aspose_generate-app-48.png)](https://products.aspose.app/barcode/generate) | [![Recognize](https://products.aspose.app/barcode/recognize/img/aspose_recognize-app-48.png)](https://products.aspose.app/barcode/recognize)
 [**Generate Wi-Fi QR**](https://products.aspose.app/barcode/wifi-qr) | [**Embed Barcode**](https://products.aspose.app/barcode/embed) | [**Scan Barcode**](https://products.aspose.app/barcode/scan)
@@ -153,14 +153,15 @@
 *BarcodeApi* | [**get_barcode_generate**](docs/BarcodeApi.md#get_barcode_generate) | **GET** /barcode/generate | Generate barcode.
 *BarcodeApi* | [**get_barcode_recognize**](docs/BarcodeApi.md#get_barcode_recognize) | **GET** /barcode/{name}/recognize | Recognize barcode from a file on server.
 *BarcodeApi* | [**post_barcode_recognize_from_url_or_content**](docs/BarcodeApi.md#post_barcode_recognize_from_url_or_content) | **POST** /barcode/recognize | Recognize barcode from an url or from request body. Request body can contain raw data bytes of the image with content-type \&quot;application/octet-stream\&quot;. An image can also be passed as a form field.
 *BarcodeApi* | [**post_generate_multiple**](docs/BarcodeApi.md#post_generate_multiple) | **POST** /barcode/generateMultiple | Generate multiple barcodes and return in response stream
 *BarcodeApi* | [**put_barcode_generate_file**](docs/BarcodeApi.md#put_barcode_generate_file) | **PUT** /barcode/{name}/generate | Generate barcode and save on server (from query params or from file with json or xml content)
 *BarcodeApi* | [**put_barcode_recognize_from_body**](docs/BarcodeApi.md#put_barcode_recognize_from_body) | **PUT** /barcode/{name}/recognize | Recognition of a barcode from file on server with parameters in body.
 *BarcodeApi* | [**put_generate_multiple**](docs/BarcodeApi.md#put_generate_multiple) | **PUT** /barcode/{name}/generateMultiple | Generate image with multiple barcodes and put new file on server
+*BarcodeApi* | [**scan_barcode**](docs/BarcodeApi.md#scan_barcode) | **POST** /barcode/scan | Quickly scan a barcode from an image.
 *FileApi* | [**copy_file**](docs/FileApi.md#copy_file) | **PUT** /barcode/storage/file/copy/{srcPath} | Copy file
 *FileApi* | [**delete_file**](docs/FileApi.md#delete_file) | **DELETE** /barcode/storage/file/{path} | Delete file
 *FileApi* | [**download_file**](docs/FileApi.md#download_file) | **GET** /barcode/storage/file/{path} | Download file
 *FileApi* | [**move_file**](docs/FileApi.md#move_file) | **PUT** /barcode/storage/file/move/{srcPath} | Move file
 *FileApi* | [**upload_file**](docs/FileApi.md#upload_file) | **PUT** /barcode/storage/file/{path} | Upload file
 *FolderApi* | [**copy_folder**](docs/FolderApi.md#copy_folder) | **PUT** /barcode/storage/folder/copy/{srcPath} | Copy folder
 *FolderApi* | [**create_folder**](docs/FolderApi.md#create_folder) | **PUT** /barcode/storage/folder/{path} | Create the folder
```

### Comparing `aspose-barcode-cloud-24.3.0/aspose_barcode_cloud.egg-info/SOURCES.txt` & `aspose_barcode_cloud-24.4.0/aspose_barcode_cloud.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -101,8 +101,9 @@
 tests/test_configuration.py
 tests/test_generate_and_recognize.py
 tests/test_headers.py
 tests/test_load_configuration.py
 tests/test_recognize_bytes.py
 tests/test_recognize_file.py
 tests/test_recognize_url.py
-tests/test_recognize_with_timeout.py
+tests/test_recognize_with_timeout.py
+tests/test_scan.py
```

### Comparing `aspose-barcode-cloud-24.3.0/setup.py` & `aspose_barcode_cloud-24.4.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,15 @@
 # coding: utf-8
 
-"""
-
-    Copyright (c) 2024 Aspose.BarCode for Cloud
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in all
- copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-"""
-
 import os
 
 from setuptools import setup, find_packages
 
 NAME = "aspose-barcode-cloud"
-VERSION = "24.3.0"
+VERSION = "24.4.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `aspose-barcode-cloud-24.3.0/tests/test_auth.py` & `aspose_barcode_cloud-24.4.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-24.3.0/tests/test_barcode_api.py` & `aspose_barcode_cloud-24.4.0/tests/test_barcode_api.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-24.3.0/tests/test_generate_and_recognize.py` & `aspose_barcode_cloud-24.4.0/tests/test_generate_and_recognize.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-24.3.0/tests/test_headers.py` & `aspose_barcode_cloud-24.4.0/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-24.3.0/tests/test_load_configuration.py` & `aspose_barcode_cloud-24.4.0/tests/test_load_configuration.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-24.3.0/tests/test_recognize_bytes.py` & `aspose_barcode_cloud-24.4.0/tests/test_recognize_bytes.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-24.3.0/tests/test_recognize_file.py` & `aspose_barcode_cloud-24.4.0/tests/test_recognize_file.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-24.3.0/tests/test_recognize_url.py` & `aspose_barcode_cloud-24.4.0/tests/test_recognize_url.py`

 * *Files identical despite different names*

### Comparing `aspose-barcode-cloud-24.3.0/tests/test_recognize_with_timeout.py` & `aspose_barcode_cloud-24.4.0/tests/test_recognize_with_timeout.py`

 * *Files identical despite different names*

