# Comparing `tmp/songtradr-api-client-python-2.0.0.tar.gz` & `tmp/songtradr_api_client_python-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "songtradr-api-client-python-2.0.0.tar", last modified: Mon Mar  4 15:31:14 2024, max compression
+gzip compressed data, was "songtradr_api_client_python-2.1.0.tar", last modified: Mon Apr 29 09:02:16 2024, max compression
```

## Comparing `songtradr-api-client-python-2.0.0.tar` & `songtradr_api_client_python-2.1.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:31:14.743080 songtradr-api-client-python-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-03-04 15:31:14.743080 songtradr-api-client-python-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11671 2024-03-04 15:31:04.000000 songtradr-api-client-python-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-04 15:31:04.000000 songtradr-api-client-python-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-04 15:31:14.743080 songtradr-api-client-python-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-03-04 15:31:04.000000 songtradr-api-client-python-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:31:14.727080 songtradr-api-client-python-2.0.0/songtradr_api_client_python/
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-03-04 15:31:04.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:31:14.727080 songtradr-api-client-python-2.0.0/songtradr_api_client_python/api/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-04 15:31:04.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34873 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/api/allowed_values_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   123358 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/api/recording_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   289639 2024-03-04 15:31:04.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27486 2024-03-04 15:31:04.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-04 15:31:04.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16424 2024-03-04 15:31:04.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-03-04 15:31:04.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:31:14.735080 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-03-04 15:31:04.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/category_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/category_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/config_access_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/config_identifier_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/contributor_type_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/field_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/file_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/file_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/file_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/file_upload_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/file_w_ith_url_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/files_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/forgot_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/genre_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/genre_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/genres_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/image_recognition_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/init_put_recording_audio_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/jwt_token_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/login_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    43771 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/party_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_for_similarity_search_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_genre_prediction_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/save_user_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     9340 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/search_filter_values_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/sign_up_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/tag_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/taggram_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/tags_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/tagstrength_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/title_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/track_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/update_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/user_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/video_recognition_response.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 15:31:04.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-03-04 15:31:04.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:31:14.739080 songtradr-api-client-python-2.0.0/songtradr_api_client_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-03-04 15:31:14.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-04 15:31:14.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:31:14.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-04 15:31:14.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-04 15:31:14.000000 songtradr-api-client-python-2.0.0/songtradr_api_client_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:31:14.739080 songtradr-api-client-python-2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_allowed_values_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_category_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_category_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_config_access_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_config_identifier_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_contributor_type_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_field_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_file_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    23419 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_file_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_file_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_file_upload_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    21995 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_file_w_ith_url_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_files_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_forgot_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_genre_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_genre_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_genres_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_image_recognition_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_init_put_recording_audio_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_jwt_token_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_login_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_party_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_recording_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_recording_for_similarity_search_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_recording_genre_prediction_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    19737 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_recording_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_recording_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_recording_minimal_with_musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_recording_minimal_with_taggrams_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_recording_minimal_with_tagstrengths_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_recording_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_recording_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_recording_tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_save_user_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_search_filter_values_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_sign_up_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_tag_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_taggram_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_tags_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_tagstrength_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_title_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_track_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_update_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-03-04 15:31:04.000000 songtradr-api-client-python-2.0.0/test/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_user_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-03-04 15:31:03.000000 songtradr-api-client-python-2.0.0/test/test_video_recognition_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:16.147219 songtradr_api_client_python-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-29 09:02:16.147219 songtradr_api_client_python-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12601 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 09:02:16.147219 songtradr_api_client_python-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:16.123218 songtradr_api_client_python-2.1.0/songtradr_api_client_python/
+-rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:16.127218 songtradr_api_client_python-2.1.0/songtradr_api_client_python/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34921 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/api/allowed_values_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126485 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/api/recording_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   347657 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28037 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16424 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:16.135218 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/category_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/category_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/config_access_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/config_identifier_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/contributor_type_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/field_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_upload_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_w_ith_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/files_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/forgot_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/genre_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/genres_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/image_recognition_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/init_put_recording_audio_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/jwt_token_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/login_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46483 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/party_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_for_similarity_search_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_genre_prediction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/save_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/search_filter_values_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/sign_up_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/taggram_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/tags_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/tagstrength_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/title_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/track_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/update_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/video_recognition_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:16.147219 songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-29 09:02:16.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-29 09:02:16.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:02:16.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-29 09:02:16.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 09:02:16.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:16.147219 songtradr_api_client_python-2.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/test/test_allowed_values_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_category_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_category_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_config_access_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_config_identifier_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_contributor_type_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_field_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_file_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23731 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_file_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_file_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_file_upload_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22291 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_file_w_ith_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_files_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_forgot_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_genre_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_genres_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_image_recognition_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_init_put_recording_audio_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_jwt_token_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_login_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_party_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/test/test_recording_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_for_similarity_search_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_genre_prediction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20033 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_minimal_with_musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_minimal_with_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_minimal_with_tagstrengths_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_save_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_search_filter_values_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_sign_up_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_taggram_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_tags_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_tagstrength_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_title_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_track_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_update_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/test/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_video_recognition_response.py
```

### Comparing `songtradr-api-client-python-2.0.0/PKG-INFO` & `songtradr_api_client_python-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songtradr-api-client-python
-Version: 2.0.0
+Version: 2.1.0
 Summary: Songtradr API
 Home-page: https://github.com/songtradr/songtradr-python-api-client-docs
 Author: Songtradr Inc.
 Author-email: info@songtradr.com
 Keywords: OpenAPI,OpenAPI-Generator,Songtradr API
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
```

### Comparing `songtradr-api-client-python-2.0.0/README.md` & `songtradr_api_client_python-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.
 
 1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters.
 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2.0.0
-- Package version: 2.0.0
+- API version: 2.1.0
+- Package version: 2.1.0
+- Generator version: 7.6.0-SNAPSHOT
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://songtradr.com](https://songtradr.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -113,30 +114,34 @@
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AllowedValuesApi* | [**allowed_musical_features**](docs/AllowedValuesApi.md#allowed_musical_features) | **GET** /api/v1/allowedValues/musicalFeatures | Allowed values for music descriptive parameters to be used in the searchAll endpoint.
 *AllowedValuesApi* | [**genres**](docs/AllowedValuesApi.md#genres) | **GET** /api/v1/allowedValues/genre | Allowed values for genres.
 *AllowedValuesApi* | [**tags**](docs/AllowedValuesApi.md#tags) | **GET** /api/v1/allowedValues/tag | All descriptive tags inside of tag-categories.
 *RecordingApi* | [**prompt_search_recordings**](docs/RecordingApi.md#prompt_search_recordings) | **GET** /api/v1/public/recording/promptSearch | Recordings for query.
 *RecordingApi* | [**recordings_by_ids_with_musical_features**](docs/RecordingApi.md#recordings_by_ids_with_musical_features) | **GET** /api/v1/public/recording/{ids}/musicalFeatures | AI generated moods, musical features and more for recordings.
-*RecordingApi* | [**recordings_by_ids_with_similarities**](docs/RecordingApi.md#recordings_by_ids_with_similarities) | **GET** /api/v1/public/recording/{ids}/similarities | Similar recordings for a list of recordings.
-*RecordingApi* | [**recordings_by_ids_with_taggrams**](docs/RecordingApi.md#recordings_by_ids_with_taggrams) | **GET** /api/v1/public/recording/{ids}/taggrams | Timeseries of AI generated moods, musical features and more for a list of recordings.
-*RecordingApi* | [**recordings_by_ids_with_tagstrengths**](docs/RecordingApi.md#recordings_by_ids_with_tagstrengths) | **GET** /api/v1/public/recording/{ids}/tagstrengths | Strengths as numerical representations for AI generated moods, musical features and more for recordings.
-*RecordingApi* | [**recordings_medium_by_ids**](docs/RecordingApi.md#recordings_medium_by_ids) | **GET** /api/v1/public/recording/m/{ids} | Recordings by IDs with a medium sized response.
+*RecordingApi* | [**recordings_by_ids_with_similarities1**](docs/RecordingApi.md#recordings_by_ids_with_similarities1) | **GET** /api/v1/public/recording/{ids}/similarities | Similar recordings for a list of recordings.
+*RecordingApi* | [**recordings_by_ids_with_taggrams1**](docs/RecordingApi.md#recordings_by_ids_with_taggrams1) | **GET** /api/v1/public/recording/{ids}/taggrams | Timeseries of AI generated moods, musical features and more for a list of recordings.
+*RecordingApi* | [**recordings_by_ids_with_tagstrengths1**](docs/RecordingApi.md#recordings_by_ids_with_tagstrengths1) | **GET** /api/v1/public/recording/{ids}/tagstrengths | Strengths as numerical representations for AI generated moods, musical features and more for recordings.
+*RecordingApi* | [**recordings_medium_by_ids1**](docs/RecordingApi.md#recordings_medium_by_ids1) | **GET** /api/v1/public/recording/m/{ids} | Recordings by IDs with a medium sized response.
 *RecordingApi* | [**search_recordings**](docs/RecordingApi.md#search_recordings) | **GET** /api/v1/public/recording/search | Recordings by contributors, moods, musical features and more.
 *UserApi* | [**delete_user_file**](docs/UserApi.md#delete_user_file) | **DELETE** /api/v1/user/file/{objectKey} | Delete file.
 *UserApi* | [**edit_me**](docs/UserApi.md#edit_me) | **POST** /api/v1/user/me | Edit details for a logged-in user
 *UserApi* | [**forgot_password**](docs/UserApi.md#forgot_password) | **POST** /api/v1/user/forgot-password | Send a password reset email
 *UserApi* | [**init_video_upload**](docs/UserApi.md#init_video_upload) | **POST** /api/v1/user/file/{name}/initVideoUpload | Recognise and upload video. Responds with an object with recognition result.
 *UserApi* | [**initiate_user_file_upload**](docs/UserApi.md#initiate_user_file_upload) | **POST** /api/v1/user/file/{name}/initUpload | Initialize a file upload. Responds with an URL where the file can be uploaded.
 *UserApi* | [**initiate_user_image_upload**](docs/UserApi.md#initiate_user_image_upload) | **POST** /api/v1/user/file/{name}/initImageUpload | Recognise and upload image. Responds with an object with recognition result.
 *UserApi* | [**login**](docs/UserApi.md#login) | **POST** /api/v1/user/login | Login to generate a bearer token.
 *UserApi* | [**me**](docs/UserApi.md#me) | **GET** /api/v1/user/me | Details for a logged-in user
 *UserApi* | [**prompt_search_user_files**](docs/UserApi.md#prompt_search_user_files) | **GET** /api/v1/user/promptSearch | Files for query.
 *UserApi* | [**recordings_by_folder_with_taggrams**](docs/UserApi.md#recordings_by_folder_with_taggrams) | **GET** /api/v1/user/folder/{folderName}/taggrams | Timeseries of AI generated moods, musical features and more for recordings in your folder.
 *UserApi* | [**recordings_by_folder_with_tagstrengths**](docs/UserApi.md#recordings_by_folder_with_tagstrengths) | **GET** /api/v1/user/folder/{folderName}/tagstrengths | Strengths as numerical representations for AI generated moods, musical features and more for recordings in your folder.
+*UserApi* | [**recordings_by_ids_with_similarities**](docs/UserApi.md#recordings_by_ids_with_similarities) | **GET** /api/v1/user/recording/{ids}/similarities | Similar recordings for a list of user recordings.
+*UserApi* | [**recordings_by_ids_with_taggrams**](docs/UserApi.md#recordings_by_ids_with_taggrams) | **GET** /api/v1/user/recording/{ids}/taggrams | Timeseries of AI generated moods, musical features and more for a list of recordings.
+*UserApi* | [**recordings_by_ids_with_tagstrengths**](docs/UserApi.md#recordings_by_ids_with_tagstrengths) | **GET** /api/v1/user/recording/{ids}/tagstrengths | Strengths as numerical representations for AI generated moods, musical features and more for recordings.
+*UserApi* | [**recordings_medium_by_ids**](docs/UserApi.md#recordings_medium_by_ids) | **GET** /api/v1/user/recording/{ids} | Recordings by IDs with a medium sized response.
 *UserApi* | [**sign_up**](docs/UserApi.md#sign_up) | **POST** /api/v1/user/sign-up | Sign up a new user.
 *UserApi* | [**token**](docs/UserApi.md#token) | **POST** /api/v1/user/token | Generates a new JWT token for the given refresh token
 *UserApi* | [**update_password**](docs/UserApi.md#update_password) | **POST** /api/v1/user/update-password | Update password by using the password reset token
 *UserApi* | [**user_file**](docs/UserApi.md#user_file) | **GET** /api/v1/user/file/{objectKey} | Details and a download link for a file.
 *UserApi* | [**user_files**](docs/UserApi.md#user_files) | **GET** /api/v1/user/files | List and search your own files.
 *UserApi* | [**user_files_status**](docs/UserApi.md#user_files_status) | **GET** /api/v1/user/filesStatus | Status details for files.
 *UserApi* | [**user_files_summary**](docs/UserApi.md#user_files_summary) | **GET** /api/v1/user/filesSummary | Summary fo your files.
```

### Comparing `songtradr-api-client-python-2.0.0/pyproject.toml` & `songtradr_api_client_python-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "songtradr_api_client_python"
-version = "2.0.0"
+version = "2.1.0"
 description = "Songtradr API"
 authors = ["Songtradr Inc. <info@songtradr.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Songtradr API"]
 include = ["songtradr_api_client_python/py.typed"]
```

### Comparing `songtradr-api-client-python-2.0.0/setup.py` & `songtradr_api_client_python-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "songtradr-api-client-python"
-VERSION = "2.0.0"
+VERSION = "2.1.0"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/__init__.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 
 # import apis into sdk package
 from songtradr_api_client_python.api.allowed_values_api import AllowedValuesApi
 from songtradr_api_client_python.api.recording_api import RecordingApi
 from songtradr_api_client_python.api.user_api import UserApi
 
 # import ApiClient
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/api/allowed_values_api.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/api/allowed_values_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr, field_validator
-from typing import Optional
+from typing import List, Optional
 from typing_extensions import Annotated
 from songtradr_api_client_python.models.category_medium_dto import CategoryMediumDTO
 from songtradr_api_client_python.models.genre_dto import GenreDTO
 from songtradr_api_client_python.models.search_filter_values_dto import SearchFilterValuesDTO
 
 from songtradr_api_client_python.api_client import ApiClient, RequestSerialized
 from songtradr_api_client_python.api_response import ApiResponse
@@ -259,15 +259,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_size is not None:
             
             _query_params.append(('responseSize', response_size))
@@ -524,15 +524,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if genre_type is not None:
             
             _query_params.append(('genreType', genre_type))
@@ -792,15 +792,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if category_name is not None:
             
             _query_params.append(('categoryName', category_name))
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/api/recording_api.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/api/recording_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
@@ -262,15 +262,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if query is not None:
             
             _query_params.append(('query', query))
@@ -324,15 +324,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> List[RecordingMinimalWithMusicalFeaturesDTO]:
-        """AI generated moods, musical features and more for recordings.
+        """(Deprecated) AI generated moods, musical features and more for recordings.
 
 
         :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
         :type ids: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -350,14 +350,15 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("GET /api/v1/public/recording/{ids}/musicalFeatures is deprecated.", DeprecationWarning)
 
         _param = self._recordings_by_ids_with_musical_features_serialize(
             ids=ids,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
@@ -393,15 +394,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[List[RecordingMinimalWithMusicalFeaturesDTO]]:
-        """AI generated moods, musical features and more for recordings.
+        """(Deprecated) AI generated moods, musical features and more for recordings.
 
 
         :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
         :type ids: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -419,14 +420,15 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("GET /api/v1/public/recording/{ids}/musicalFeatures is deprecated.", DeprecationWarning)
 
         _param = self._recordings_by_ids_with_musical_features_serialize(
             ids=ids,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
@@ -462,15 +464,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """AI generated moods, musical features and more for recordings.
+        """(Deprecated) AI generated moods, musical features and more for recordings.
 
 
         :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
         :type ids: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -488,14 +490,15 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("GET /api/v1/public/recording/{ids}/musicalFeatures is deprecated.", DeprecationWarning)
 
         _param = self._recordings_by_ids_with_musical_features_serialize(
             ids=ids,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
@@ -528,15 +531,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if ids is not None:
             _path_params['ids'] = ids
         # process the query parameters
         # process the header parameters
@@ -572,15 +575,15 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def recordings_by_ids_with_similarities(
+    def recordings_by_ids_with_similarities1(
         self,
         ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
         identical_only: Annotated[Optional[StrictBool], Field(description="Whether a result list shall include only identical recordings.")] = None,
         usage: Annotated[Optional[StrictStr], Field(description="Filter by recording usage.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
@@ -590,15 +593,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> List[RecordingForSimilaritySearchDTO]:
-        """Similar recordings for a list of recordings.
+        """(Deprecated) Similar recordings for a list of recordings.
 
 
         :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
         :type ids: str
         :param identical_only: Whether a result list shall include only identical recordings.
         :type identical_only: bool
         :param usage: Filter by recording usage.
@@ -620,16 +623,17 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("GET /api/v1/public/recording/{ids}/similarities is deprecated.", DeprecationWarning)
 
-        _param = self._recordings_by_ids_with_similarities_serialize(
+        _param = self._recordings_by_ids_with_similarities1_serialize(
             ids=ids,
             identical_only=identical_only,
             usage=usage,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
@@ -649,15 +653,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def recordings_by_ids_with_similarities_with_http_info(
+    def recordings_by_ids_with_similarities1_with_http_info(
         self,
         ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
         identical_only: Annotated[Optional[StrictBool], Field(description="Whether a result list shall include only identical recordings.")] = None,
         usage: Annotated[Optional[StrictStr], Field(description="Filter by recording usage.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
@@ -667,15 +671,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[List[RecordingForSimilaritySearchDTO]]:
-        """Similar recordings for a list of recordings.
+        """(Deprecated) Similar recordings for a list of recordings.
 
 
         :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
         :type ids: str
         :param identical_only: Whether a result list shall include only identical recordings.
         :type identical_only: bool
         :param usage: Filter by recording usage.
@@ -697,16 +701,17 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("GET /api/v1/public/recording/{ids}/similarities is deprecated.", DeprecationWarning)
 
-        _param = self._recordings_by_ids_with_similarities_serialize(
+        _param = self._recordings_by_ids_with_similarities1_serialize(
             ids=ids,
             identical_only=identical_only,
             usage=usage,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
@@ -726,15 +731,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def recordings_by_ids_with_similarities_without_preload_content(
+    def recordings_by_ids_with_similarities1_without_preload_content(
         self,
         ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
         identical_only: Annotated[Optional[StrictBool], Field(description="Whether a result list shall include only identical recordings.")] = None,
         usage: Annotated[Optional[StrictStr], Field(description="Filter by recording usage.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
@@ -744,15 +749,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Similar recordings for a list of recordings.
+        """(Deprecated) Similar recordings for a list of recordings.
 
 
         :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
         :type ids: str
         :param identical_only: Whether a result list shall include only identical recordings.
         :type identical_only: bool
         :param usage: Filter by recording usage.
@@ -774,16 +779,17 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("GET /api/v1/public/recording/{ids}/similarities is deprecated.", DeprecationWarning)
 
-        _param = self._recordings_by_ids_with_similarities_serialize(
+        _param = self._recordings_by_ids_with_similarities1_serialize(
             ids=ids,
             identical_only=identical_only,
             usage=usage,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
@@ -798,15 +804,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _recordings_by_ids_with_similarities_serialize(
+    def _recordings_by_ids_with_similarities1_serialize(
         self,
         ids,
         identical_only,
         usage,
         _request_auth,
         _content_type,
         _headers,
@@ -818,15 +824,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if ids is not None:
             _path_params['ids'] = ids
         # process the query parameters
         if identical_only is not None:
@@ -870,15 +876,15 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def recordings_by_ids_with_taggrams(
+    def recordings_by_ids_with_taggrams1(
         self,
         ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
         category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
         tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
         genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
         from_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data starting from from this timestamp in seconds.")] = None,
         to_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data before this timestamp in seconds.")] = None,
@@ -892,15 +898,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> List[RecordingMinimalWithTaggramsDTO]:
-        """Timeseries of AI generated moods, musical features and more for a list of recordings.
+        """(Deprecated) Timeseries of AI generated moods, musical features and more for a list of recordings.
 
 
         :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
         :type ids: str
         :param category_name: Show only taggrams for one category.
         :type category_name: str
         :param tag_name: Show only taggrams for one tag.
@@ -930,16 +936,17 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("GET /api/v1/public/recording/{ids}/taggrams is deprecated.", DeprecationWarning)
 
-        _param = self._recordings_by_ids_with_taggrams_serialize(
+        _param = self._recordings_by_ids_with_taggrams1_serialize(
             ids=ids,
             category_name=category_name,
             tag_name=tag_name,
             genre_name=genre_name,
             from_timestamp=from_timestamp,
             to_timestamp=to_timestamp,
             fill_with_zero=fill_with_zero,
@@ -963,15 +970,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def recordings_by_ids_with_taggrams_with_http_info(
+    def recordings_by_ids_with_taggrams1_with_http_info(
         self,
         ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
         category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
         tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
         genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
         from_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data starting from from this timestamp in seconds.")] = None,
         to_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data before this timestamp in seconds.")] = None,
@@ -985,15 +992,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[List[RecordingMinimalWithTaggramsDTO]]:
-        """Timeseries of AI generated moods, musical features and more for a list of recordings.
+        """(Deprecated) Timeseries of AI generated moods, musical features and more for a list of recordings.
 
 
         :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
         :type ids: str
         :param category_name: Show only taggrams for one category.
         :type category_name: str
         :param tag_name: Show only taggrams for one tag.
@@ -1023,16 +1030,17 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("GET /api/v1/public/recording/{ids}/taggrams is deprecated.", DeprecationWarning)
 
-        _param = self._recordings_by_ids_with_taggrams_serialize(
+        _param = self._recordings_by_ids_with_taggrams1_serialize(
             ids=ids,
             category_name=category_name,
             tag_name=tag_name,
             genre_name=genre_name,
             from_timestamp=from_timestamp,
             to_timestamp=to_timestamp,
             fill_with_zero=fill_with_zero,
@@ -1056,15 +1064,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def recordings_by_ids_with_taggrams_without_preload_content(
+    def recordings_by_ids_with_taggrams1_without_preload_content(
         self,
         ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
         category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
         tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
         genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
         from_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data starting from from this timestamp in seconds.")] = None,
         to_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data before this timestamp in seconds.")] = None,
@@ -1078,15 +1086,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Timeseries of AI generated moods, musical features and more for a list of recordings.
+        """(Deprecated) Timeseries of AI generated moods, musical features and more for a list of recordings.
 
 
         :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
         :type ids: str
         :param category_name: Show only taggrams for one category.
         :type category_name: str
         :param tag_name: Show only taggrams for one tag.
@@ -1116,16 +1124,17 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("GET /api/v1/public/recording/{ids}/taggrams is deprecated.", DeprecationWarning)
 
-        _param = self._recordings_by_ids_with_taggrams_serialize(
+        _param = self._recordings_by_ids_with_taggrams1_serialize(
             ids=ids,
             category_name=category_name,
             tag_name=tag_name,
             genre_name=genre_name,
             from_timestamp=from_timestamp,
             to_timestamp=to_timestamp,
             fill_with_zero=fill_with_zero,
@@ -1144,15 +1153,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _recordings_by_ids_with_taggrams_serialize(
+    def _recordings_by_ids_with_taggrams1_serialize(
         self,
         ids,
         category_name,
         tag_name,
         genre_name,
         from_timestamp,
         to_timestamp,
@@ -1168,15 +1177,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if ids is not None:
             _path_params['ids'] = ids
         # process the query parameters
         if category_name is not None:
@@ -1236,15 +1245,15 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def recordings_by_ids_with_tagstrengths(
+    def recordings_by_ids_with_tagstrengths1(
         self,
         ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
         category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
         tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
         genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
         _request_timeout: Union[
             None,
@@ -1255,15 +1264,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> List[RecordingMinimalWithTagstrengthsDTO]:
-        """Strengths as numerical representations for AI generated moods, musical features and more for recordings.
+        """(Deprecated) Strengths as numerical representations for AI generated moods, musical features and more for recordings.
 
 
         :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
         :type ids: str
         :param category_name: Show only taggrams for one category.
         :type category_name: str
         :param tag_name: Show only taggrams for one tag.
@@ -1287,16 +1296,17 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("GET /api/v1/public/recording/{ids}/tagstrengths is deprecated.", DeprecationWarning)
 
-        _param = self._recordings_by_ids_with_tagstrengths_serialize(
+        _param = self._recordings_by_ids_with_tagstrengths1_serialize(
             ids=ids,
             category_name=category_name,
             tag_name=tag_name,
             genre_name=genre_name,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -1317,15 +1327,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def recordings_by_ids_with_tagstrengths_with_http_info(
+    def recordings_by_ids_with_tagstrengths1_with_http_info(
         self,
         ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
         category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
         tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
         genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
         _request_timeout: Union[
             None,
@@ -1336,15 +1346,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[List[RecordingMinimalWithTagstrengthsDTO]]:
-        """Strengths as numerical representations for AI generated moods, musical features and more for recordings.
+        """(Deprecated) Strengths as numerical representations for AI generated moods, musical features and more for recordings.
 
 
         :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
         :type ids: str
         :param category_name: Show only taggrams for one category.
         :type category_name: str
         :param tag_name: Show only taggrams for one tag.
@@ -1368,16 +1378,17 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("GET /api/v1/public/recording/{ids}/tagstrengths is deprecated.", DeprecationWarning)
 
-        _param = self._recordings_by_ids_with_tagstrengths_serialize(
+        _param = self._recordings_by_ids_with_tagstrengths1_serialize(
             ids=ids,
             category_name=category_name,
             tag_name=tag_name,
             genre_name=genre_name,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -1398,15 +1409,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def recordings_by_ids_with_tagstrengths_without_preload_content(
+    def recordings_by_ids_with_tagstrengths1_without_preload_content(
         self,
         ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
         category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
         tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
         genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
         _request_timeout: Union[
             None,
@@ -1417,15 +1428,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Strengths as numerical representations for AI generated moods, musical features and more for recordings.
+        """(Deprecated) Strengths as numerical representations for AI generated moods, musical features and more for recordings.
 
 
         :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
         :type ids: str
         :param category_name: Show only taggrams for one category.
         :type category_name: str
         :param tag_name: Show only taggrams for one tag.
@@ -1449,16 +1460,17 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("GET /api/v1/public/recording/{ids}/tagstrengths is deprecated.", DeprecationWarning)
 
-        _param = self._recordings_by_ids_with_tagstrengths_serialize(
+        _param = self._recordings_by_ids_with_tagstrengths1_serialize(
             ids=ids,
             category_name=category_name,
             tag_name=tag_name,
             genre_name=genre_name,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -1474,15 +1486,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _recordings_by_ids_with_tagstrengths_serialize(
+    def _recordings_by_ids_with_tagstrengths1_serialize(
         self,
         ids,
         category_name,
         tag_name,
         genre_name,
         _request_auth,
         _content_type,
@@ -1495,15 +1507,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if ids is not None:
             _path_params['ids'] = ids
         # process the query parameters
         if category_name is not None:
@@ -1551,15 +1563,15 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def recordings_medium_by_ids(
+    def recordings_medium_by_ids1(
         self,
         ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
         page: Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None,
         size: Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None,
         sort: Annotated[Optional[List[StrictStr]], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None,
         _request_timeout: Union[
             None,
@@ -1570,15 +1582,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> List[RecordingMediumDTO]:
-        """Recordings by IDs with a medium sized response.
+        """(Deprecated) Recordings by IDs with a medium sized response.
 
 
         :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
         :type ids: str
         :param page: Zero-based page index (0..N)
         :type page: int
         :param size: The size of the page to be returned
@@ -1602,16 +1614,17 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("GET /api/v1/public/recording/m/{ids} is deprecated.", DeprecationWarning)
 
-        _param = self._recordings_medium_by_ids_serialize(
+        _param = self._recordings_medium_by_ids1_serialize(
             ids=ids,
             page=page,
             size=size,
             sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -1632,15 +1645,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def recordings_medium_by_ids_with_http_info(
+    def recordings_medium_by_ids1_with_http_info(
         self,
         ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
         page: Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None,
         size: Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None,
         sort: Annotated[Optional[List[StrictStr]], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None,
         _request_timeout: Union[
             None,
@@ -1651,15 +1664,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[List[RecordingMediumDTO]]:
-        """Recordings by IDs with a medium sized response.
+        """(Deprecated) Recordings by IDs with a medium sized response.
 
 
         :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
         :type ids: str
         :param page: Zero-based page index (0..N)
         :type page: int
         :param size: The size of the page to be returned
@@ -1683,16 +1696,17 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("GET /api/v1/public/recording/m/{ids} is deprecated.", DeprecationWarning)
 
-        _param = self._recordings_medium_by_ids_serialize(
+        _param = self._recordings_medium_by_ids1_serialize(
             ids=ids,
             page=page,
             size=size,
             sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -1713,15 +1727,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def recordings_medium_by_ids_without_preload_content(
+    def recordings_medium_by_ids1_without_preload_content(
         self,
         ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
         page: Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None,
         size: Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None,
         sort: Annotated[Optional[List[StrictStr]], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None,
         _request_timeout: Union[
             None,
@@ -1732,15 +1746,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Recordings by IDs with a medium sized response.
+        """(Deprecated) Recordings by IDs with a medium sized response.
 
 
         :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
         :type ids: str
         :param page: Zero-based page index (0..N)
         :type page: int
         :param size: The size of the page to be returned
@@ -1764,16 +1778,17 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("GET /api/v1/public/recording/m/{ids} is deprecated.", DeprecationWarning)
 
-        _param = self._recordings_medium_by_ids_serialize(
+        _param = self._recordings_medium_by_ids1_serialize(
             ids=ids,
             page=page,
             size=size,
             sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -1789,15 +1804,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _recordings_medium_by_ids_serialize(
+    def _recordings_medium_by_ids1_serialize(
         self,
         ids,
         page,
         size,
         sort,
         _request_auth,
         _content_type,
@@ -1811,15 +1826,15 @@
             'sort': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if ids is not None:
             _path_params['ids'] = ids
         # process the query parameters
         if page is not None:
@@ -1905,14 +1920,15 @@
         loudness: Annotated[Optional[StrictStr], Field(description="Search for loudness.")] = None,
         origin_decade: Annotated[Optional[StrictStr], Field(description="Search for origin decade.")] = None,
         curateability: Annotated[Optional[StrictStr], Field(description="Search for curateability.")] = None,
         use_case: Annotated[Optional[StrictStr], Field(description="Search for use case.")] = None,
         channel_suitability: Annotated[Optional[StrictStr], Field(description="Search for channel suitability.")] = None,
         songtradr_track_id: Annotated[Optional[StrictStr], Field(description="Search for Songtradr track id.")] = None,
         usage: Annotated[Optional[StrictStr], Field(description="Search for recording usage.")] = None,
+        pretzel_station_suitability: Annotated[Optional[StrictStr], Field(description="Search for Pretzel station suitability.")] = None,
         similar_to_songtradr_track_id: Annotated[Optional[StrictStr], Field(description="Search for songs similar to a recording by songtradr Track Id.")] = None,
         shuffled: Annotated[Optional[StrictStr], Field(description="Sort the results randomly.")] = None,
         sort: Annotated[Optional[StrictStr], Field(description="Sort the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None,
         size: Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None,
         _request_timeout: Union[
             None,
@@ -1998,14 +2014,16 @@
         :type use_case: str
         :param channel_suitability: Search for channel suitability.
         :type channel_suitability: str
         :param songtradr_track_id: Search for Songtradr track id.
         :type songtradr_track_id: str
         :param usage: Search for recording usage.
         :type usage: str
+        :param pretzel_station_suitability: Search for Pretzel station suitability.
+        :type pretzel_station_suitability: str
         :param similar_to_songtradr_track_id: Search for songs similar to a recording by songtradr Track Id.
         :type similar_to_songtradr_track_id: str
         :param shuffled: Sort the results randomly.
         :type shuffled: str
         :param sort: Sort the results.
         :type sort: str
         :param page: Zero-based page index (0..N)
@@ -2067,14 +2085,15 @@
             loudness=loudness,
             origin_decade=origin_decade,
             curateability=curateability,
             use_case=use_case,
             channel_suitability=channel_suitability,
             songtradr_track_id=songtradr_track_id,
             usage=usage,
+            pretzel_station_suitability=pretzel_station_suitability,
             similar_to_songtradr_track_id=similar_to_songtradr_track_id,
             shuffled=shuffled,
             sort=sort,
             page=page,
             size=size,
             _request_auth=_request_auth,
             _content_type=_content_type,
@@ -2134,14 +2153,15 @@
         loudness: Annotated[Optional[StrictStr], Field(description="Search for loudness.")] = None,
         origin_decade: Annotated[Optional[StrictStr], Field(description="Search for origin decade.")] = None,
         curateability: Annotated[Optional[StrictStr], Field(description="Search for curateability.")] = None,
         use_case: Annotated[Optional[StrictStr], Field(description="Search for use case.")] = None,
         channel_suitability: Annotated[Optional[StrictStr], Field(description="Search for channel suitability.")] = None,
         songtradr_track_id: Annotated[Optional[StrictStr], Field(description="Search for Songtradr track id.")] = None,
         usage: Annotated[Optional[StrictStr], Field(description="Search for recording usage.")] = None,
+        pretzel_station_suitability: Annotated[Optional[StrictStr], Field(description="Search for Pretzel station suitability.")] = None,
         similar_to_songtradr_track_id: Annotated[Optional[StrictStr], Field(description="Search for songs similar to a recording by songtradr Track Id.")] = None,
         shuffled: Annotated[Optional[StrictStr], Field(description="Sort the results randomly.")] = None,
         sort: Annotated[Optional[StrictStr], Field(description="Sort the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None,
         size: Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None,
         _request_timeout: Union[
             None,
@@ -2227,14 +2247,16 @@
         :type use_case: str
         :param channel_suitability: Search for channel suitability.
         :type channel_suitability: str
         :param songtradr_track_id: Search for Songtradr track id.
         :type songtradr_track_id: str
         :param usage: Search for recording usage.
         :type usage: str
+        :param pretzel_station_suitability: Search for Pretzel station suitability.
+        :type pretzel_station_suitability: str
         :param similar_to_songtradr_track_id: Search for songs similar to a recording by songtradr Track Id.
         :type similar_to_songtradr_track_id: str
         :param shuffled: Sort the results randomly.
         :type shuffled: str
         :param sort: Sort the results.
         :type sort: str
         :param page: Zero-based page index (0..N)
@@ -2296,14 +2318,15 @@
             loudness=loudness,
             origin_decade=origin_decade,
             curateability=curateability,
             use_case=use_case,
             channel_suitability=channel_suitability,
             songtradr_track_id=songtradr_track_id,
             usage=usage,
+            pretzel_station_suitability=pretzel_station_suitability,
             similar_to_songtradr_track_id=similar_to_songtradr_track_id,
             shuffled=shuffled,
             sort=sort,
             page=page,
             size=size,
             _request_auth=_request_auth,
             _content_type=_content_type,
@@ -2363,14 +2386,15 @@
         loudness: Annotated[Optional[StrictStr], Field(description="Search for loudness.")] = None,
         origin_decade: Annotated[Optional[StrictStr], Field(description="Search for origin decade.")] = None,
         curateability: Annotated[Optional[StrictStr], Field(description="Search for curateability.")] = None,
         use_case: Annotated[Optional[StrictStr], Field(description="Search for use case.")] = None,
         channel_suitability: Annotated[Optional[StrictStr], Field(description="Search for channel suitability.")] = None,
         songtradr_track_id: Annotated[Optional[StrictStr], Field(description="Search for Songtradr track id.")] = None,
         usage: Annotated[Optional[StrictStr], Field(description="Search for recording usage.")] = None,
+        pretzel_station_suitability: Annotated[Optional[StrictStr], Field(description="Search for Pretzel station suitability.")] = None,
         similar_to_songtradr_track_id: Annotated[Optional[StrictStr], Field(description="Search for songs similar to a recording by songtradr Track Id.")] = None,
         shuffled: Annotated[Optional[StrictStr], Field(description="Sort the results randomly.")] = None,
         sort: Annotated[Optional[StrictStr], Field(description="Sort the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None,
         size: Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None,
         _request_timeout: Union[
             None,
@@ -2456,14 +2480,16 @@
         :type use_case: str
         :param channel_suitability: Search for channel suitability.
         :type channel_suitability: str
         :param songtradr_track_id: Search for Songtradr track id.
         :type songtradr_track_id: str
         :param usage: Search for recording usage.
         :type usage: str
+        :param pretzel_station_suitability: Search for Pretzel station suitability.
+        :type pretzel_station_suitability: str
         :param similar_to_songtradr_track_id: Search for songs similar to a recording by songtradr Track Id.
         :type similar_to_songtradr_track_id: str
         :param shuffled: Sort the results randomly.
         :type shuffled: str
         :param sort: Sort the results.
         :type sort: str
         :param page: Zero-based page index (0..N)
@@ -2525,14 +2551,15 @@
             loudness=loudness,
             origin_decade=origin_decade,
             curateability=curateability,
             use_case=use_case,
             channel_suitability=channel_suitability,
             songtradr_track_id=songtradr_track_id,
             usage=usage,
+            pretzel_station_suitability=pretzel_station_suitability,
             similar_to_songtradr_track_id=similar_to_songtradr_track_id,
             shuffled=shuffled,
             sort=sort,
             page=page,
             size=size,
             _request_auth=_request_auth,
             _content_type=_content_type,
@@ -2587,14 +2614,15 @@
         loudness,
         origin_decade,
         curateability,
         use_case,
         channel_suitability,
         songtradr_track_id,
         usage,
+        pretzel_station_suitability,
         similar_to_songtradr_track_id,
         shuffled,
         sort,
         page,
         size,
         _request_auth,
         _content_type,
@@ -2607,15 +2635,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if similar_to_recording is not None:
             
             _query_params.append(('similarToRecording', similar_to_recording))
@@ -2756,14 +2784,18 @@
             
             _query_params.append(('songtradrTrackId', songtradr_track_id))
             
         if usage is not None:
             
             _query_params.append(('usage', usage))
             
+        if pretzel_station_suitability is not None:
+            
+            _query_params.append(('pretzelStationSuitability', pretzel_station_suitability))
+            
         if similar_to_songtradr_track_id is not None:
             
             _query_params.append(('similarToSongtradrTrackId', similar_to_songtradr_track_id))
             
         if shuffled is not None:
             
             _query_params.append(('shuffled', shuffled))
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/api/user_api.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/api/user_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from datetime import datetime
 from pydantic import Field, StrictBool, StrictFloat, StrictInt, StrictStr, field_validator
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 from typing_extensions import Annotated
 from songtradr_api_client_python.models.file_list_dto import FileListDTO
 from songtradr_api_client_python.models.file_small_dto import FileSmallDTO
 from songtradr_api_client_python.models.file_upload_dto import FileUploadDTO
 from songtradr_api_client_python.models.file_w_ith_url_dto import FileWIthUrlDTO
 from songtradr_api_client_python.models.files_summary_dto import FilesSummaryDTO
 from songtradr_api_client_python.models.forgot_password_dto import ForgotPasswordDTO
 from songtradr_api_client_python.models.image_recognition_response import ImageRecognitionResponse
 from songtradr_api_client_python.models.init_put_recording_audio_dto import InitPutRecordingAudioDTO
 from songtradr_api_client_python.models.jwt_token_dto import JwtTokenDTO
 from songtradr_api_client_python.models.login_dto import LoginDTO
+from songtradr_api_client_python.models.recording_for_similarity_search_dto import RecordingForSimilaritySearchDTO
+from songtradr_api_client_python.models.recording_medium_dto import RecordingMediumDTO
 from songtradr_api_client_python.models.recording_minimal_with_taggrams_dto import RecordingMinimalWithTaggramsDTO
 from songtradr_api_client_python.models.recording_minimal_with_tagstrengths_dto import RecordingMinimalWithTagstrengthsDTO
 from songtradr_api_client_python.models.save_user_dto import SaveUserDTO
 from songtradr_api_client_python.models.sign_up_dto import SignUpDTO
 from songtradr_api_client_python.models.token_request import TokenRequest
 from songtradr_api_client_python.models.update_password_dto import UpdatePasswordDTO
 from songtradr_api_client_python.models.user_dto import UserDTO
@@ -275,15 +277,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if object_key is not None:
             _path_params['objectKey'] = object_key
         # process the query parameters
         # process the header parameters
@@ -543,15 +545,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -823,15 +825,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -1117,15 +1119,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if name is not None:
             _path_params['name'] = name
         # process the query parameters
         if url is not None:
@@ -1414,15 +1416,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if name is not None:
             _path_params['name'] = name
         # process the query parameters
         if folder is not None:
@@ -1713,15 +1715,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if name is not None:
             _path_params['name'] = name
         # process the query parameters
         if url is not None:
@@ -1984,15 +1986,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -2248,15 +2250,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -2510,15 +2512,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if query is not None:
             
             _query_params.append(('query', query))
@@ -2894,15 +2896,15 @@
             'sort': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if folder_name is not None:
             _path_params['folderName'] = folder_name
         # process the query parameters
         if category_name is not None:
@@ -3273,15 +3275,15 @@
             'sort': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if folder_name is not None:
             _path_params['folderName'] = folder_name
         # process the query parameters
         if category_name is not None:
@@ -3341,14 +3343,1309 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
+    def recordings_by_ids_with_similarities(
+        self,
+        ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
+        identical_only: Annotated[Optional[StrictBool], Field(description="Whether a result list shall include only identical recordings.")] = None,
+        usage: Annotated[Optional[StrictStr], Field(description="Filter by recording usage.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> List[RecordingForSimilaritySearchDTO]:
+        """Similar recordings for a list of user recordings.
+
+
+        :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
+        :type ids: str
+        :param identical_only: Whether a result list shall include only identical recordings.
+        :type identical_only: bool
+        :param usage: Filter by recording usage.
+        :type usage: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._recordings_by_ids_with_similarities_serialize(
+            ids=ids,
+            identical_only=identical_only,
+            usage=usage,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[RecordingForSimilaritySearchDTO]",
+            '401': "ErrorResponse",
+            '429': "ErrorResponse",
+            '500': "ErrorResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def recordings_by_ids_with_similarities_with_http_info(
+        self,
+        ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
+        identical_only: Annotated[Optional[StrictBool], Field(description="Whether a result list shall include only identical recordings.")] = None,
+        usage: Annotated[Optional[StrictStr], Field(description="Filter by recording usage.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[List[RecordingForSimilaritySearchDTO]]:
+        """Similar recordings for a list of user recordings.
+
+
+        :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
+        :type ids: str
+        :param identical_only: Whether a result list shall include only identical recordings.
+        :type identical_only: bool
+        :param usage: Filter by recording usage.
+        :type usage: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._recordings_by_ids_with_similarities_serialize(
+            ids=ids,
+            identical_only=identical_only,
+            usage=usage,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[RecordingForSimilaritySearchDTO]",
+            '401': "ErrorResponse",
+            '429': "ErrorResponse",
+            '500': "ErrorResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def recordings_by_ids_with_similarities_without_preload_content(
+        self,
+        ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
+        identical_only: Annotated[Optional[StrictBool], Field(description="Whether a result list shall include only identical recordings.")] = None,
+        usage: Annotated[Optional[StrictStr], Field(description="Filter by recording usage.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Similar recordings for a list of user recordings.
+
+
+        :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
+        :type ids: str
+        :param identical_only: Whether a result list shall include only identical recordings.
+        :type identical_only: bool
+        :param usage: Filter by recording usage.
+        :type usage: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._recordings_by_ids_with_similarities_serialize(
+            ids=ids,
+            identical_only=identical_only,
+            usage=usage,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[RecordingForSimilaritySearchDTO]",
+            '401': "ErrorResponse",
+            '429': "ErrorResponse",
+            '500': "ErrorResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _recordings_by_ids_with_similarities_serialize(
+        self,
+        ids,
+        identical_only,
+        usage,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, Union[str, bytes]] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if ids is not None:
+            _path_params['ids'] = ids
+        # process the query parameters
+        if identical_only is not None:
+            
+            _query_params.append(('identicalOnly', identical_only))
+            
+        if usage is not None:
+            
+            _query_params.append(('usage', usage))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'bearer-jwt'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/api/v1/user/recording/{ids}/similarities',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def recordings_by_ids_with_taggrams(
+        self,
+        ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
+        category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
+        tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
+        genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
+        from_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data starting from from this timestamp in seconds.")] = None,
+        to_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data before this timestamp in seconds.")] = None,
+        fill_with_zero: Annotated[Optional[StrictBool], Field(description="If set to true, empty timeseries are filled with timeseries of 0.0 values.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> List[RecordingMinimalWithTaggramsDTO]:
+        """Timeseries of AI generated moods, musical features and more for a list of recordings.
+
+
+        :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
+        :type ids: str
+        :param category_name: Show only taggrams for one category.
+        :type category_name: str
+        :param tag_name: Show only taggrams for one tag.
+        :type tag_name: str
+        :param genre_name: Show only taggrams for one genre.
+        :type genre_name: str
+        :param from_timestamp: Show only taggrams data starting from from this timestamp in seconds.
+        :type from_timestamp: float
+        :param to_timestamp: Show only taggrams data before this timestamp in seconds.
+        :type to_timestamp: float
+        :param fill_with_zero: If set to true, empty timeseries are filled with timeseries of 0.0 values.
+        :type fill_with_zero: bool
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._recordings_by_ids_with_taggrams_serialize(
+            ids=ids,
+            category_name=category_name,
+            tag_name=tag_name,
+            genre_name=genre_name,
+            from_timestamp=from_timestamp,
+            to_timestamp=to_timestamp,
+            fill_with_zero=fill_with_zero,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[RecordingMinimalWithTaggramsDTO]",
+            '401': "ErrorResponse",
+            '429': "ErrorResponse",
+            '500': "ErrorResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def recordings_by_ids_with_taggrams_with_http_info(
+        self,
+        ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
+        category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
+        tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
+        genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
+        from_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data starting from from this timestamp in seconds.")] = None,
+        to_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data before this timestamp in seconds.")] = None,
+        fill_with_zero: Annotated[Optional[StrictBool], Field(description="If set to true, empty timeseries are filled with timeseries of 0.0 values.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[List[RecordingMinimalWithTaggramsDTO]]:
+        """Timeseries of AI generated moods, musical features and more for a list of recordings.
+
+
+        :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
+        :type ids: str
+        :param category_name: Show only taggrams for one category.
+        :type category_name: str
+        :param tag_name: Show only taggrams for one tag.
+        :type tag_name: str
+        :param genre_name: Show only taggrams for one genre.
+        :type genre_name: str
+        :param from_timestamp: Show only taggrams data starting from from this timestamp in seconds.
+        :type from_timestamp: float
+        :param to_timestamp: Show only taggrams data before this timestamp in seconds.
+        :type to_timestamp: float
+        :param fill_with_zero: If set to true, empty timeseries are filled with timeseries of 0.0 values.
+        :type fill_with_zero: bool
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._recordings_by_ids_with_taggrams_serialize(
+            ids=ids,
+            category_name=category_name,
+            tag_name=tag_name,
+            genre_name=genre_name,
+            from_timestamp=from_timestamp,
+            to_timestamp=to_timestamp,
+            fill_with_zero=fill_with_zero,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[RecordingMinimalWithTaggramsDTO]",
+            '401': "ErrorResponse",
+            '429': "ErrorResponse",
+            '500': "ErrorResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def recordings_by_ids_with_taggrams_without_preload_content(
+        self,
+        ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
+        category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
+        tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
+        genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
+        from_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data starting from from this timestamp in seconds.")] = None,
+        to_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data before this timestamp in seconds.")] = None,
+        fill_with_zero: Annotated[Optional[StrictBool], Field(description="If set to true, empty timeseries are filled with timeseries of 0.0 values.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Timeseries of AI generated moods, musical features and more for a list of recordings.
+
+
+        :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
+        :type ids: str
+        :param category_name: Show only taggrams for one category.
+        :type category_name: str
+        :param tag_name: Show only taggrams for one tag.
+        :type tag_name: str
+        :param genre_name: Show only taggrams for one genre.
+        :type genre_name: str
+        :param from_timestamp: Show only taggrams data starting from from this timestamp in seconds.
+        :type from_timestamp: float
+        :param to_timestamp: Show only taggrams data before this timestamp in seconds.
+        :type to_timestamp: float
+        :param fill_with_zero: If set to true, empty timeseries are filled with timeseries of 0.0 values.
+        :type fill_with_zero: bool
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._recordings_by_ids_with_taggrams_serialize(
+            ids=ids,
+            category_name=category_name,
+            tag_name=tag_name,
+            genre_name=genre_name,
+            from_timestamp=from_timestamp,
+            to_timestamp=to_timestamp,
+            fill_with_zero=fill_with_zero,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[RecordingMinimalWithTaggramsDTO]",
+            '401': "ErrorResponse",
+            '429': "ErrorResponse",
+            '500': "ErrorResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _recordings_by_ids_with_taggrams_serialize(
+        self,
+        ids,
+        category_name,
+        tag_name,
+        genre_name,
+        from_timestamp,
+        to_timestamp,
+        fill_with_zero,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, Union[str, bytes]] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if ids is not None:
+            _path_params['ids'] = ids
+        # process the query parameters
+        if category_name is not None:
+            
+            _query_params.append(('categoryName', category_name))
+            
+        if tag_name is not None:
+            
+            _query_params.append(('tagName', tag_name))
+            
+        if genre_name is not None:
+            
+            _query_params.append(('genreName', genre_name))
+            
+        if from_timestamp is not None:
+            
+            _query_params.append(('fromTimestamp', from_timestamp))
+            
+        if to_timestamp is not None:
+            
+            _query_params.append(('toTimestamp', to_timestamp))
+            
+        if fill_with_zero is not None:
+            
+            _query_params.append(('fillWithZero', fill_with_zero))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'bearer-jwt'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/api/v1/user/recording/{ids}/taggrams',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def recordings_by_ids_with_tagstrengths(
+        self,
+        ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
+        category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
+        tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
+        genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> List[RecordingMinimalWithTagstrengthsDTO]:
+        """Strengths as numerical representations for AI generated moods, musical features and more for recordings.
+
+
+        :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
+        :type ids: str
+        :param category_name: Show only taggrams for one category.
+        :type category_name: str
+        :param tag_name: Show only taggrams for one tag.
+        :type tag_name: str
+        :param genre_name: Show only taggrams for one genre.
+        :type genre_name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._recordings_by_ids_with_tagstrengths_serialize(
+            ids=ids,
+            category_name=category_name,
+            tag_name=tag_name,
+            genre_name=genre_name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[RecordingMinimalWithTagstrengthsDTO]",
+            '401': "ErrorResponse",
+            '429': "ErrorResponse",
+            '500': "ErrorResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def recordings_by_ids_with_tagstrengths_with_http_info(
+        self,
+        ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
+        category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
+        tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
+        genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[List[RecordingMinimalWithTagstrengthsDTO]]:
+        """Strengths as numerical representations for AI generated moods, musical features and more for recordings.
+
+
+        :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
+        :type ids: str
+        :param category_name: Show only taggrams for one category.
+        :type category_name: str
+        :param tag_name: Show only taggrams for one tag.
+        :type tag_name: str
+        :param genre_name: Show only taggrams for one genre.
+        :type genre_name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._recordings_by_ids_with_tagstrengths_serialize(
+            ids=ids,
+            category_name=category_name,
+            tag_name=tag_name,
+            genre_name=genre_name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[RecordingMinimalWithTagstrengthsDTO]",
+            '401': "ErrorResponse",
+            '429': "ErrorResponse",
+            '500': "ErrorResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def recordings_by_ids_with_tagstrengths_without_preload_content(
+        self,
+        ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
+        category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
+        tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
+        genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Strengths as numerical representations for AI generated moods, musical features and more for recordings.
+
+
+        :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
+        :type ids: str
+        :param category_name: Show only taggrams for one category.
+        :type category_name: str
+        :param tag_name: Show only taggrams for one tag.
+        :type tag_name: str
+        :param genre_name: Show only taggrams for one genre.
+        :type genre_name: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._recordings_by_ids_with_tagstrengths_serialize(
+            ids=ids,
+            category_name=category_name,
+            tag_name=tag_name,
+            genre_name=genre_name,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[RecordingMinimalWithTagstrengthsDTO]",
+            '401': "ErrorResponse",
+            '429': "ErrorResponse",
+            '500': "ErrorResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _recordings_by_ids_with_tagstrengths_serialize(
+        self,
+        ids,
+        category_name,
+        tag_name,
+        genre_name,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, Union[str, bytes]] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if ids is not None:
+            _path_params['ids'] = ids
+        # process the query parameters
+        if category_name is not None:
+            
+            _query_params.append(('categoryName', category_name))
+            
+        if tag_name is not None:
+            
+            _query_params.append(('tagName', tag_name))
+            
+        if genre_name is not None:
+            
+            _query_params.append(('genreName', genre_name))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'bearer-jwt'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/api/v1/user/recording/{ids}/tagstrengths',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def recordings_medium_by_ids(
+        self,
+        ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
+        page: Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None,
+        size: Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None,
+        sort: Annotated[Optional[List[StrictStr]], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> List[RecordingMediumDTO]:
+        """Recordings by IDs with a medium sized response.
+
+
+        :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
+        :type ids: str
+        :param page: Zero-based page index (0..N)
+        :type page: int
+        :param size: The size of the page to be returned
+        :type size: int
+        :param sort: Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.
+        :type sort: List[str]
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._recordings_medium_by_ids_serialize(
+            ids=ids,
+            page=page,
+            size=size,
+            sort=sort,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[RecordingMediumDTO]",
+            '401': "ErrorResponse",
+            '429': "ErrorResponse",
+            '500': "ErrorResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def recordings_medium_by_ids_with_http_info(
+        self,
+        ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
+        page: Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None,
+        size: Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None,
+        sort: Annotated[Optional[List[StrictStr]], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[List[RecordingMediumDTO]]:
+        """Recordings by IDs with a medium sized response.
+
+
+        :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
+        :type ids: str
+        :param page: Zero-based page index (0..N)
+        :type page: int
+        :param size: The size of the page to be returned
+        :type size: int
+        :param sort: Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.
+        :type sort: List[str]
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._recordings_medium_by_ids_serialize(
+            ids=ids,
+            page=page,
+            size=size,
+            sort=sort,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[RecordingMediumDTO]",
+            '401': "ErrorResponse",
+            '429': "ErrorResponse",
+            '500': "ErrorResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def recordings_medium_by_ids_without_preload_content(
+        self,
+        ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
+        page: Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None,
+        size: Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None,
+        sort: Annotated[Optional[List[StrictStr]], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Recordings by IDs with a medium sized response.
+
+
+        :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
+        :type ids: str
+        :param page: Zero-based page index (0..N)
+        :type page: int
+        :param size: The size of the page to be returned
+        :type size: int
+        :param sort: Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.
+        :type sort: List[str]
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._recordings_medium_by_ids_serialize(
+            ids=ids,
+            page=page,
+            size=size,
+            sort=sort,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[RecordingMediumDTO]",
+            '401': "ErrorResponse",
+            '429': "ErrorResponse",
+            '500': "ErrorResponse",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _recordings_medium_by_ids_serialize(
+        self,
+        ids,
+        page,
+        size,
+        sort,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+            'sort': 'multi',
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, Union[str, bytes]] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if ids is not None:
+            _path_params['ids'] = ids
+        # process the query parameters
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if size is not None:
+            
+            _query_params.append(('size', size))
+            
+        if sort is not None:
+            
+            _query_params.append(('sort', sort))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'bearer-jwt'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/api/v1/user/recording/{ids}',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def sign_up(
         self,
         save_user_dto: SaveUserDTO,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -3393,17 +4690,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "SignUpDTO",
             '409': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "SignUpDTO",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -3465,17 +4762,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "SignUpDTO",
             '409': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "SignUpDTO",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -3537,17 +4834,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "SignUpDTO",
             '409': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "SignUpDTO",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -3570,15 +4867,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -3850,15 +5147,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -4130,15 +5427,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -4411,15 +5708,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if object_key is not None:
             _path_params['objectKey'] = object_key
         # process the query parameters
         # process the header parameters
@@ -4503,14 +5800,15 @@
         audience_age: Optional[StrictStr] = None,
         audience_region: Optional[StrictStr] = None,
         audience_gender: Optional[StrictStr] = None,
         origin_decade: Optional[StrictStr] = None,
         curateability: Optional[StrictStr] = None,
         use_case: Optional[StrictStr] = None,
         channel_suitability: Optional[StrictStr] = None,
+        pretzel_station_suitability: Optional[StrictStr] = None,
         similar_to_recording: Optional[StrictStr] = None,
         songtradr_track_id: Optional[StrictStr] = None,
         usage_name: Optional[StrictStr] = None,
         bpm_min: Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None,
         bpm_max: Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None,
         name: Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None,
         folder: Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None,
@@ -4627,14 +5925,16 @@
         :type origin_decade: str
         :param curateability:
         :type curateability: str
         :param use_case:
         :type use_case: str
         :param channel_suitability:
         :type channel_suitability: str
+        :param pretzel_station_suitability:
+        :type pretzel_station_suitability: str
         :param similar_to_recording:
         :type similar_to_recording: str
         :param songtradr_track_id:
         :type songtradr_track_id: str
         :param usage_name:
         :type usage_name: str
         :param bpm_min: Search for a minimal bpm.
@@ -4728,14 +6028,15 @@
             audience_age=audience_age,
             audience_region=audience_region,
             audience_gender=audience_gender,
             origin_decade=origin_decade,
             curateability=curateability,
             use_case=use_case,
             channel_suitability=channel_suitability,
+            pretzel_station_suitability=pretzel_station_suitability,
             similar_to_recording=similar_to_recording,
             songtradr_track_id=songtradr_track_id,
             usage_name=usage_name,
             bpm_min=bpm_min,
             bpm_max=bpm_max,
             name=name,
             folder=folder,
@@ -4816,14 +6117,15 @@
         audience_age: Optional[StrictStr] = None,
         audience_region: Optional[StrictStr] = None,
         audience_gender: Optional[StrictStr] = None,
         origin_decade: Optional[StrictStr] = None,
         curateability: Optional[StrictStr] = None,
         use_case: Optional[StrictStr] = None,
         channel_suitability: Optional[StrictStr] = None,
+        pretzel_station_suitability: Optional[StrictStr] = None,
         similar_to_recording: Optional[StrictStr] = None,
         songtradr_track_id: Optional[StrictStr] = None,
         usage_name: Optional[StrictStr] = None,
         bpm_min: Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None,
         bpm_max: Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None,
         name: Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None,
         folder: Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None,
@@ -4940,14 +6242,16 @@
         :type origin_decade: str
         :param curateability:
         :type curateability: str
         :param use_case:
         :type use_case: str
         :param channel_suitability:
         :type channel_suitability: str
+        :param pretzel_station_suitability:
+        :type pretzel_station_suitability: str
         :param similar_to_recording:
         :type similar_to_recording: str
         :param songtradr_track_id:
         :type songtradr_track_id: str
         :param usage_name:
         :type usage_name: str
         :param bpm_min: Search for a minimal bpm.
@@ -5041,14 +6345,15 @@
             audience_age=audience_age,
             audience_region=audience_region,
             audience_gender=audience_gender,
             origin_decade=origin_decade,
             curateability=curateability,
             use_case=use_case,
             channel_suitability=channel_suitability,
+            pretzel_station_suitability=pretzel_station_suitability,
             similar_to_recording=similar_to_recording,
             songtradr_track_id=songtradr_track_id,
             usage_name=usage_name,
             bpm_min=bpm_min,
             bpm_max=bpm_max,
             name=name,
             folder=folder,
@@ -5129,14 +6434,15 @@
         audience_age: Optional[StrictStr] = None,
         audience_region: Optional[StrictStr] = None,
         audience_gender: Optional[StrictStr] = None,
         origin_decade: Optional[StrictStr] = None,
         curateability: Optional[StrictStr] = None,
         use_case: Optional[StrictStr] = None,
         channel_suitability: Optional[StrictStr] = None,
+        pretzel_station_suitability: Optional[StrictStr] = None,
         similar_to_recording: Optional[StrictStr] = None,
         songtradr_track_id: Optional[StrictStr] = None,
         usage_name: Optional[StrictStr] = None,
         bpm_min: Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None,
         bpm_max: Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None,
         name: Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None,
         folder: Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None,
@@ -5253,14 +6559,16 @@
         :type origin_decade: str
         :param curateability:
         :type curateability: str
         :param use_case:
         :type use_case: str
         :param channel_suitability:
         :type channel_suitability: str
+        :param pretzel_station_suitability:
+        :type pretzel_station_suitability: str
         :param similar_to_recording:
         :type similar_to_recording: str
         :param songtradr_track_id:
         :type songtradr_track_id: str
         :param usage_name:
         :type usage_name: str
         :param bpm_min: Search for a minimal bpm.
@@ -5354,14 +6662,15 @@
             audience_age=audience_age,
             audience_region=audience_region,
             audience_gender=audience_gender,
             origin_decade=origin_decade,
             curateability=curateability,
             use_case=use_case,
             channel_suitability=channel_suitability,
+            pretzel_station_suitability=pretzel_station_suitability,
             similar_to_recording=similar_to_recording,
             songtradr_track_id=songtradr_track_id,
             usage_name=usage_name,
             bpm_min=bpm_min,
             bpm_max=bpm_max,
             name=name,
             folder=folder,
@@ -5437,14 +6746,15 @@
         audience_age,
         audience_region,
         audience_gender,
         origin_decade,
         curateability,
         use_case,
         channel_suitability,
+        pretzel_station_suitability,
         similar_to_recording,
         songtradr_track_id,
         usage_name,
         bpm_min,
         bpm_max,
         name,
         folder,
@@ -5471,15 +6781,15 @@
             'sort': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if isrc is not None:
             
             _query_params.append(('ISRC', isrc))
@@ -5669,14 +6979,18 @@
             
             _query_params.append(('useCase', use_case))
             
         if channel_suitability is not None:
             
             _query_params.append(('channelSuitability', channel_suitability))
             
+        if pretzel_station_suitability is not None:
+            
+            _query_params.append(('pretzelStationSuitability', pretzel_station_suitability))
+            
         if similar_to_recording is not None:
             
             _query_params.append(('similarToRecording', similar_to_recording))
             
         if songtradr_track_id is not None:
             
             _query_params.append(('songtradrTrackId', songtradr_track_id))
@@ -6020,15 +7334,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if object_keys is not None:
             
             _query_params.append(('objectKeys', object_keys))
@@ -6113,14 +7427,15 @@
         audience_age: Optional[StrictStr] = None,
         audience_region: Optional[StrictStr] = None,
         audience_gender: Optional[StrictStr] = None,
         origin_decade: Optional[StrictStr] = None,
         curateability: Optional[StrictStr] = None,
         use_case: Optional[StrictStr] = None,
         channel_suitability: Optional[StrictStr] = None,
+        pretzel_station_suitability: Optional[StrictStr] = None,
         similar_to_recording: Optional[StrictStr] = None,
         songtradr_track_id: Optional[StrictStr] = None,
         usage_name: Optional[StrictStr] = None,
         bpm_min: Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None,
         bpm_max: Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None,
         name: Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None,
         folder: Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None,
@@ -6232,14 +7547,16 @@
         :type origin_decade: str
         :param curateability:
         :type curateability: str
         :param use_case:
         :type use_case: str
         :param channel_suitability:
         :type channel_suitability: str
+        :param pretzel_station_suitability:
+        :type pretzel_station_suitability: str
         :param similar_to_recording:
         :type similar_to_recording: str
         :param songtradr_track_id:
         :type songtradr_track_id: str
         :param usage_name:
         :type usage_name: str
         :param bpm_min: Search for a minimal bpm.
@@ -6326,14 +7643,15 @@
             audience_age=audience_age,
             audience_region=audience_region,
             audience_gender=audience_gender,
             origin_decade=origin_decade,
             curateability=curateability,
             use_case=use_case,
             channel_suitability=channel_suitability,
+            pretzel_station_suitability=pretzel_station_suitability,
             similar_to_recording=similar_to_recording,
             songtradr_track_id=songtradr_track_id,
             usage_name=usage_name,
             bpm_min=bpm_min,
             bpm_max=bpm_max,
             name=name,
             folder=folder,
@@ -6410,14 +7728,15 @@
         audience_age: Optional[StrictStr] = None,
         audience_region: Optional[StrictStr] = None,
         audience_gender: Optional[StrictStr] = None,
         origin_decade: Optional[StrictStr] = None,
         curateability: Optional[StrictStr] = None,
         use_case: Optional[StrictStr] = None,
         channel_suitability: Optional[StrictStr] = None,
+        pretzel_station_suitability: Optional[StrictStr] = None,
         similar_to_recording: Optional[StrictStr] = None,
         songtradr_track_id: Optional[StrictStr] = None,
         usage_name: Optional[StrictStr] = None,
         bpm_min: Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None,
         bpm_max: Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None,
         name: Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None,
         folder: Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None,
@@ -6529,14 +7848,16 @@
         :type origin_decade: str
         :param curateability:
         :type curateability: str
         :param use_case:
         :type use_case: str
         :param channel_suitability:
         :type channel_suitability: str
+        :param pretzel_station_suitability:
+        :type pretzel_station_suitability: str
         :param similar_to_recording:
         :type similar_to_recording: str
         :param songtradr_track_id:
         :type songtradr_track_id: str
         :param usage_name:
         :type usage_name: str
         :param bpm_min: Search for a minimal bpm.
@@ -6623,14 +7944,15 @@
             audience_age=audience_age,
             audience_region=audience_region,
             audience_gender=audience_gender,
             origin_decade=origin_decade,
             curateability=curateability,
             use_case=use_case,
             channel_suitability=channel_suitability,
+            pretzel_station_suitability=pretzel_station_suitability,
             similar_to_recording=similar_to_recording,
             songtradr_track_id=songtradr_track_id,
             usage_name=usage_name,
             bpm_min=bpm_min,
             bpm_max=bpm_max,
             name=name,
             folder=folder,
@@ -6707,14 +8029,15 @@
         audience_age: Optional[StrictStr] = None,
         audience_region: Optional[StrictStr] = None,
         audience_gender: Optional[StrictStr] = None,
         origin_decade: Optional[StrictStr] = None,
         curateability: Optional[StrictStr] = None,
         use_case: Optional[StrictStr] = None,
         channel_suitability: Optional[StrictStr] = None,
+        pretzel_station_suitability: Optional[StrictStr] = None,
         similar_to_recording: Optional[StrictStr] = None,
         songtradr_track_id: Optional[StrictStr] = None,
         usage_name: Optional[StrictStr] = None,
         bpm_min: Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None,
         bpm_max: Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None,
         name: Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None,
         folder: Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None,
@@ -6826,14 +8149,16 @@
         :type origin_decade: str
         :param curateability:
         :type curateability: str
         :param use_case:
         :type use_case: str
         :param channel_suitability:
         :type channel_suitability: str
+        :param pretzel_station_suitability:
+        :type pretzel_station_suitability: str
         :param similar_to_recording:
         :type similar_to_recording: str
         :param songtradr_track_id:
         :type songtradr_track_id: str
         :param usage_name:
         :type usage_name: str
         :param bpm_min: Search for a minimal bpm.
@@ -6920,14 +8245,15 @@
             audience_age=audience_age,
             audience_region=audience_region,
             audience_gender=audience_gender,
             origin_decade=origin_decade,
             curateability=curateability,
             use_case=use_case,
             channel_suitability=channel_suitability,
+            pretzel_station_suitability=pretzel_station_suitability,
             similar_to_recording=similar_to_recording,
             songtradr_track_id=songtradr_track_id,
             usage_name=usage_name,
             bpm_min=bpm_min,
             bpm_max=bpm_max,
             name=name,
             folder=folder,
@@ -6999,14 +8325,15 @@
         audience_age,
         audience_region,
         audience_gender,
         origin_decade,
         curateability,
         use_case,
         channel_suitability,
+        pretzel_station_suitability,
         similar_to_recording,
         songtradr_track_id,
         usage_name,
         bpm_min,
         bpm_max,
         name,
         folder,
@@ -7029,15 +8356,15 @@
             'tagNames': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if isrc is not None:
             
             _query_params.append(('ISRC', isrc))
@@ -7223,14 +8550,18 @@
             
             _query_params.append(('useCase', use_case))
             
         if channel_suitability is not None:
             
             _query_params.append(('channelSuitability', channel_suitability))
             
+        if pretzel_station_suitability is not None:
+            
+            _query_params.append(('pretzelStationSuitability', pretzel_station_suitability))
+            
         if similar_to_recording is not None:
             
             _query_params.append(('similarToRecording', similar_to_recording))
             
         if songtradr_track_id is not None:
             
             _query_params.append(('songtradrTrackId', songtradr_track_id))
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/api_client.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/api_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -19,15 +19,16 @@
 import json
 import mimetypes
 import os
 import re
 import tempfile
 
 from urllib.parse import quote
-from typing import Tuple, Optional, List, Dict
+from typing import Tuple, Optional, List, Dict, Union
+from pydantic import SecretStr
 
 from songtradr_api_client_python.configuration import Configuration
 from songtradr_api_client_python.api_response import ApiResponse, T as ApiResponseT
 import songtradr_api_client_python.models
 from songtradr_api_client_python import rest
 from songtradr_api_client_python.exceptions import (
     ApiValueError,
@@ -84,15 +85,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/2.1.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
@@ -204,15 +205,16 @@
         if post_params or files:
             post_params = post_params if post_params else []
             post_params = self.sanitize_for_serialization(post_params)
             post_params = self.parameters_to_tuples(
                 post_params,
                 collection_formats
             )
-            post_params.extend(self.files_parameters(files))
+            if files:
+                post_params.extend(self.files_parameters(files))
 
         # auth setting
         self.update_params_for_auth(
             header_params,
             query_params,
             auth_settings,
             resource_path,
@@ -309,15 +311,18 @@
             elif response_type is not None:
                 match = None
                 content_type = response_data.getheader('content-type')
                 if content_type is not None:
                     match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?", content_type)
                 encoding = match.group(1) if match else "utf-8"
                 response_text = response_data.data.decode(encoding)
-                return_data = self.deserialize(response_text, response_type)
+                if response_type in ["bytearray", "str"]:
+                    return_data = self.__deserialize_primitive(response_text, response_type)
+                else:
+                    return_data = self.deserialize(response_text, response_type)
         finally:
             if not 200 <= response_data.status <= 299:
                 raise ApiException.from_response(
                     http_resp=response_data,
                     body=response_text,
                     data=return_data,
                 )
@@ -329,26 +334,31 @@
             raw_data = response_data.data
         )
 
     def sanitize_for_serialization(self, obj):
         """Builds a JSON POST object.
 
         If obj is None, return None.
+        If obj is SecretStr, return obj.get_secret_value()
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
             convert to string in iso8601 format.
         If obj is list, sanitize each element in the list.
         If obj is dict, return the dict.
         If obj is OpenAPI model, return the properties dict.
 
         :param obj: The data to serialize.
         :return: The serialized form of data.
         """
         if obj is None:
             return None
+        elif isinstance(obj, Enum):
+            return obj.value
+        elif isinstance(obj, SecretStr):
+            return obj.get_secret_value()
         elif isinstance(obj, self.PRIMITIVE_TYPES):
             return obj
         elif isinstance(obj, list):
             return [
                 self.sanitize_for_serialization(sub_obj) for sub_obj in obj
             ]
         elif isinstance(obj, tuple):
@@ -362,15 +372,18 @@
             obj_dict = obj
         else:
             # Convert model obj to dict except
             # attributes `openapi_types`, `attribute_map`
             # and attributes which value is not None.
             # Convert attribute name to json key in
             # model definition for request.
-            obj_dict = obj.to_dict()
+            if hasattr(obj, 'to_dict') and callable(getattr(obj, 'to_dict')):
+                obj_dict = obj.to_dict()
+            else:
+                obj_dict = obj.__dict__
 
         return {
             key: self.sanitize_for_serialization(val)
             for key, val in obj_dict.items()
         }
 
     def deserialize(self, response_text, response_type):
@@ -501,39 +514,38 @@
                         (k, delimiter.join(quote(str(value)) for value in v))
                     )
             else:
                 new_params.append((k, quote(str(v))))
 
         return "&".join(["=".join(map(str, item)) for item in new_params])
 
-    def files_parameters(self, files=None):
+    def files_parameters(self, files: Dict[str, Union[str, bytes]]):
         """Builds form parameters.
 
         :param files: File parameters.
         :return: Form parameters with files.
         """
         params = []
-
-        if files:
-            for k, v in files.items():
-                if not v:
-                    continue
-                file_names = v if type(v) is list else [v]
-                for n in file_names:
-                    with open(n, 'rb') as f:
-                        filename = os.path.basename(f.name)
-                        filedata = f.read()
-                        mimetype = (
-                            mimetypes.guess_type(filename)[0]
-                            or 'application/octet-stream'
-                        )
-                        params.append(
-                            tuple([k, tuple([filename, filedata, mimetype])])
-                        )
-
+        for k, v in files.items():
+            if isinstance(v, str):
+                with open(v, 'rb') as f:
+                    filename = os.path.basename(f.name)
+                    filedata = f.read()
+            elif isinstance(v, bytes):
+                filename = k
+                filedata = v
+            else:
+                raise ValueError("Unsupported file value")
+            mimetype = (
+                mimetypes.guess_type(filename)[0]
+                or 'application/octet-stream'
+            )
+            params.append(
+                tuple([k, tuple([filename, filedata, mimetype])])
+            )
         return params
 
     def select_header_accept(self, accepts: List[str]) -> Optional[str]:
         """Returns `Accept` based on an array of accepts provided.
 
         :param accepts: List of headers.
         :return: Accept (e.g. application/json).
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/api_response.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/api_response.py`

 * *Files identical despite different names*

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/configuration.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -375,16 +375,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.0.0\n"\
-               "SDK Package Version: 2.0.0".\
+               "Version of the API: 2.1.0\n"\
+               "SDK Package Version: 2.1.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/exceptions.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/__init__.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/category_medium_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/category_medium_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/category_minimal_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/category_minimal_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/config_access_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/config_access_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/config_identifier_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/config_identifier_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/contributor_type_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/contributor_type_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/error_response.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/field_summary_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/field_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/file_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/file_list_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_list_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/file_small_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -24,30 +24,30 @@
 from typing import Optional, Set
 from typing_extensions import Self
 
 class FileSmallDTO(BaseModel):
     """
     Reduced details on a file that has been uploaded for auto-tagging or audio-recognition purposes.
     """ # noqa: E501
+    folder: StrictStr
     name: StrictStr
     id: StrictInt
     extension: StrictStr = Field(description="extension of the file")
     error_message: Optional[StrictStr] = None
-    folder: StrictStr
     fingerprint_status: Optional[StrictStr] = Field(default=None, description="status of the audio recognition", alias="fingerprintStatus")
     object_key: StrictStr = Field(alias="objectKey")
     upload_start_time: Optional[datetime] = Field(default=None, alias="uploadStartTime")
     upload_end_time: Optional[datetime] = Field(default=None, alias="uploadEndTime")
     fingerprint_start_time: Optional[datetime] = Field(default=None, alias="fingerprintStartTime")
     fingerprint_end_time: Optional[datetime] = Field(default=None, alias="fingerprintEndTime")
     inference_status: Optional[StrictStr] = Field(default=None, description="status of the auto-tagging", alias="inferenceStatus")
     inference_start_time: Optional[datetime] = Field(default=None, alias="inferenceStartTime")
     inference_end_time: Optional[datetime] = Field(default=None, alias="inferenceEndTime")
     error_time: Optional[datetime] = None
-    __properties: ClassVar[List[str]] = ["name", "id", "extension", "error_message", "folder", "fingerprintStatus", "objectKey", "uploadStartTime", "uploadEndTime", "fingerprintStartTime", "fingerprintEndTime", "inferenceStatus", "inferenceStartTime", "inferenceEndTime", "error_time"]
+    __properties: ClassVar[List[str]] = ["folder", "name", "id", "extension", "error_message", "fingerprintStatus", "objectKey", "uploadStartTime", "uploadEndTime", "fingerprintStartTime", "fingerprintEndTime", "inferenceStatus", "inferenceStartTime", "inferenceEndTime", "error_time"]
 
     @field_validator('extension')
     def extension_validate_enum(cls, value):
         """Validates the enum"""
         if value not in set(['mp3', 'wav', 'flac']):
             raise ValueError("must be one of enum values ('mp3', 'wav', 'flac')")
         return value
@@ -119,19 +119,19 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "folder": obj.get("folder"),
             "name": obj.get("name"),
             "id": obj.get("id"),
             "extension": obj.get("extension"),
             "error_message": obj.get("error_message"),
-            "folder": obj.get("folder"),
             "fingerprintStatus": obj.get("fingerprintStatus"),
             "objectKey": obj.get("objectKey"),
             "uploadStartTime": obj.get("uploadStartTime"),
             "uploadEndTime": obj.get("uploadEndTime"),
             "fingerprintStartTime": obj.get("fingerprintStartTime"),
             "fingerprintEndTime": obj.get("fingerprintEndTime"),
             "inferenceStatus": obj.get("inferenceStatus"),
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/file_upload_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_upload_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/file_w_ith_url_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_w_ith_url_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/files_summary_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/files_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/forgot_password_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/forgot_password_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/genre_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/genre_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/genre_minimal_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/genre_minimal_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/genres_summary_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/genres_summary_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/image_recognition_response.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/image_recognition_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/init_put_recording_audio_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/init_put_recording_audio_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/jwt_token_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/jwt_token_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/login_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/login_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/musical_features_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/musical_features_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -24,32 +24,32 @@
 from typing_extensions import Self
 
 class MusicalFeaturesDTO(BaseModel):
     """
     AI generated musical features of a recording.
     """ # noqa: E501
     space: Optional[StrictStr] = Field(default=None, description="Search for space")
-    arousal: Optional[StrictStr] = Field(default=None, description="Search for an arousal")
     valence_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="valenceAffinity")
-    arousal_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="arousalAffinity")
-    pleasantness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="pleasantnessAffinity")
-    engagement_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="engagementAffinity")
-    energy_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="energyAffinity")
     tempo_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="tempoAffinity")
     scale_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="scaleAffinity")
     timbre_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="timbreAffinity")
     roughness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="roughnessAffinity")
     harmony_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="harmonyAffinity")
     texture_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="textureAffinity")
     groovyness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="groovynessAffinity")
     space_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="spaceAffinity")
     loudness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="loudnessAffinity")
     key_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="keyAffinity")
     channel_suitability_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="channelSuitabilityAffinity")
+    arousal_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="arousalAffinity")
+    pleasantness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="pleasantnessAffinity")
+    engagement_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="engagementAffinity")
+    energy_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="energyAffinity")
     language_of_performance: Optional[StrictStr] = Field(default=None, alias="languageOfPerformance")
+    arousal: Optional[StrictStr] = Field(default=None, description="Search for an arousal")
     dominant_instrument: Optional[StrictStr] = Field(default=None, description="Search for a dominant instrument", alias="dominantInstrument")
     energy: Optional[StrictStr] = Field(default=None, description="Search for energy")
     engagement: Optional[StrictStr] = Field(default=None, description="Search for an engagement")
     groovyness: Optional[StrictStr] = Field(default=None, description="Search for groovyness")
     harmony: Optional[StrictStr] = Field(default=None, description="Search for a degree of harmoniousness")
     pleasantness: Optional[StrictStr] = Field(default=None, description="Search for pleasantness")
     primary_mood_cluster: Optional[StrictStr] = Field(default=None, description="Search for a language of the lyrics", alias="primaryMoodCluster")
@@ -65,15 +65,17 @@
     tonality: Optional[StrictStr] = Field(default=None, description="Search for tonality")
     valence: Optional[StrictStr] = Field(default=None, description="Search for a valence")
     vocals: Optional[StrictStr] = Field(default=None, description="Search for a vocal gender or instrumental songs")
     origin_decade: Optional[StrictStr] = Field(default=None, description="Search for origin decade", alias="originDecade")
     curateability: Optional[StrictStr] = Field(default=None, description="Search for curatebility")
     use_case: Optional[StrictStr] = Field(default=None, description="Search for use case", alias="useCase")
     channel_suitability: Optional[StrictStr] = Field(default=None, description="Search for social media suitability", alias="channelSuitability")
+    pretzel_station_suitability: Optional[StrictStr] = Field(default=None, description="Search for pretzel station suitability", alias="pretzelStationSuitability")
     loudness: Optional[StrictStr] = Field(default=None, description="Search for loudness")
+    bpm: Optional[Union[StrictFloat, StrictInt]] = None
     primary_mood_cluster_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="primaryMoodClusterAffinity")
     secondary_mood_cluster: Optional[StrictStr] = Field(default=None, description="Search for a language of the lyrics", alias="secondaryMoodCluster")
     secondary_mood_cluster_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="secondaryMoodClusterAffinity")
     tertiary_mood_cluster: Optional[StrictStr] = Field(default=None, description="Search for a language of the lyrics", alias="tertiaryMoodCluster")
     tertiary_mood_cluster_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="tertiaryMoodClusterAffinity")
     vocals_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="vocalsAffinity")
     dominant_instrument_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="dominantInstrumentAffinity")
@@ -81,15 +83,14 @@
     secondary_instrument_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="secondaryInstrumentAffinity")
     tertiary_instrument: Optional[StrictStr] = Field(default=None, description="Search for a dominant instrument", alias="tertiaryInstrument")
     tertiary_instrument_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="tertiaryInstrumentAffinity")
     sound_generation_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="soundGenerationAffinity")
     rhythm_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="rhythmAffinity")
     primary_sound_character_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="primarySoundCharacterAffinity")
     tonality_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="tonalityAffinity")
-    bpm: Optional[Union[StrictFloat, StrictInt]] = None
     production_rating: Optional[StrictStr] = Field(default=None, alias="productionRating")
     production_rating_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="productionRatingAffinity")
     performance_rating: Optional[StrictStr] = Field(default=None, alias="performanceRating")
     performance_rating_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="performanceRatingAffinity")
     song_rating: Optional[StrictStr] = Field(default=None, alias="songRating")
     song_rating_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="songRatingAffinity")
     audience_age: Optional[StrictStr] = Field(default=None, alias="audienceAge")
@@ -109,45 +110,46 @@
     origin_region_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="originRegionAffinity")
     origin_decade_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="originDecadeAffinity")
     language_of_performance_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="languageOfPerformanceAffinity")
     curateability_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="curateabilityAffinity")
     use_case_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="useCaseAffinity")
     industry_suitability: Optional[StrictStr] = Field(default=None, description="Search for Industry suitability", alias="industrySuitability")
     industry_suitability_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="industrySuitabilityAffinity")
+    pretzel_station_suitability_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="pretzelStationSuitabilityAffinity")
     audience_region: Optional[StrictStr] = Field(default=None, alias="audienceRegion")
-    __properties: ClassVar[List[str]] = ["space", "arousal", "valenceAffinity", "arousalAffinity", "pleasantnessAffinity", "engagementAffinity", "energyAffinity", "tempoAffinity", "scaleAffinity", "timbreAffinity", "roughnessAffinity", "harmonyAffinity", "textureAffinity", "groovynessAffinity", "spaceAffinity", "loudnessAffinity", "keyAffinity", "channelSuitabilityAffinity", "languageOfPerformance", "dominantInstrument", "energy", "engagement", "groovyness", "harmony", "pleasantness", "primaryMoodCluster", "primarySoundCharacter", "rhythm", "roughness", "scale", "key", "soundGeneration", "tempo", "texture", "timbre", "tonality", "valence", "vocals", "originDecade", "curateability", "useCase", "channelSuitability", "loudness", "primaryMoodClusterAffinity", "secondaryMoodCluster", "secondaryMoodClusterAffinity", "tertiaryMoodCluster", "tertiaryMoodClusterAffinity", "vocalsAffinity", "dominantInstrumentAffinity", "secondaryInstrument", "secondaryInstrumentAffinity", "tertiaryInstrument", "tertiaryInstrumentAffinity", "soundGenerationAffinity", "rhythmAffinity", "primarySoundCharacterAffinity", "tonalityAffinity", "bpm", "productionRating", "productionRatingAffinity", "performanceRating", "performanceRatingAffinity", "songRating", "songRatingAffinity", "audienceAge", "audienceAgeAffinity", "secondaryAudienceAge", "secondaryAudienceAgeAffinity", "tertiaryAudienceAge", "tertiaryAudienceAgeAffinity", "audienceGender", "audienceGenderAffinity", "audienceRegionAffinity", "secondaryAudienceRegion", "secondaryAudienceRegionAffinity", "tertiaryAudienceRegion", "tertiaryAudienceRegionAffinity", "originRegion", "originRegionAffinity", "originDecadeAffinity", "languageOfPerformanceAffinity", "curateabilityAffinity", "useCaseAffinity", "industrySuitability", "industrySuitabilityAffinity", "audienceRegion"]
+    __properties: ClassVar[List[str]] = ["space", "valenceAffinity", "tempoAffinity", "scaleAffinity", "timbreAffinity", "roughnessAffinity", "harmonyAffinity", "textureAffinity", "groovynessAffinity", "spaceAffinity", "loudnessAffinity", "keyAffinity", "channelSuitabilityAffinity", "arousalAffinity", "pleasantnessAffinity", "engagementAffinity", "energyAffinity", "languageOfPerformance", "arousal", "dominantInstrument", "energy", "engagement", "groovyness", "harmony", "pleasantness", "primaryMoodCluster", "primarySoundCharacter", "rhythm", "roughness", "scale", "key", "soundGeneration", "tempo", "texture", "timbre", "tonality", "valence", "vocals", "originDecade", "curateability", "useCase", "channelSuitability", "pretzelStationSuitability", "loudness", "bpm", "primaryMoodClusterAffinity", "secondaryMoodCluster", "secondaryMoodClusterAffinity", "tertiaryMoodCluster", "tertiaryMoodClusterAffinity", "vocalsAffinity", "dominantInstrumentAffinity", "secondaryInstrument", "secondaryInstrumentAffinity", "tertiaryInstrument", "tertiaryInstrumentAffinity", "soundGenerationAffinity", "rhythmAffinity", "primarySoundCharacterAffinity", "tonalityAffinity", "productionRating", "productionRatingAffinity", "performanceRating", "performanceRatingAffinity", "songRating", "songRatingAffinity", "audienceAge", "audienceAgeAffinity", "secondaryAudienceAge", "secondaryAudienceAgeAffinity", "tertiaryAudienceAge", "tertiaryAudienceAgeAffinity", "audienceGender", "audienceGenderAffinity", "audienceRegionAffinity", "secondaryAudienceRegion", "secondaryAudienceRegionAffinity", "tertiaryAudienceRegion", "tertiaryAudienceRegionAffinity", "originRegion", "originRegionAffinity", "originDecadeAffinity", "languageOfPerformanceAffinity", "curateabilityAffinity", "useCaseAffinity", "industrySuitability", "industrySuitabilityAffinity", "pretzelStationSuitabilityAffinity", "audienceRegion"]
 
     @field_validator('space')
     def space_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
         if value not in set(['very compact', 'compact', 'moderate space', 'wide', 'very wide']):
             raise ValueError("must be one of enum values ('very compact', 'compact', 'moderate space', 'wide', 'very wide')")
         return value
 
-    @field_validator('arousal')
-    def arousal_validate_enum(cls, value):
+    @field_validator('language_of_performance')
+    def language_of_performance_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in set(['very calm', 'calm', 'moderate arousal', 'energetic', 'very energetic', 'varying arousal']):
-            raise ValueError("must be one of enum values ('very calm', 'calm', 'moderate arousal', 'energetic', 'very energetic', 'varying arousal')")
+        if value not in set(['en', 'de', 'no', 'fr', 'es', 'pt', 'fi', 'ru', 'it', 'la', 'el', 'ar', 'nl', 'ja', 'pl', 'sv', 'zu', 'da', 'cs', 'hu', 'af', 'hi', 'tr', 'zh', 'ms', 'pa', 'id', 'ko', 'vi']):
+            raise ValueError("must be one of enum values ('en', 'de', 'no', 'fr', 'es', 'pt', 'fi', 'ru', 'it', 'la', 'el', 'ar', 'nl', 'ja', 'pl', 'sv', 'zu', 'da', 'cs', 'hu', 'af', 'hi', 'tr', 'zh', 'ms', 'pa', 'id', 'ko', 'vi')")
         return value
 
-    @field_validator('language_of_performance')
-    def language_of_performance_validate_enum(cls, value):
+    @field_validator('arousal')
+    def arousal_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in set(['en', 'de', 'no', 'fr', 'es', 'pt', 'fi', 'ru', 'it', 'la', 'el', 'ar', 'nl', 'ja', 'pl', 'sv', 'zu', 'da', 'cs', 'hu', 'af', 'hi', 'tr', 'zh', 'ms', 'pa', 'id', 'ko', 'vi']):
-            raise ValueError("must be one of enum values ('en', 'de', 'no', 'fr', 'es', 'pt', 'fi', 'ru', 'it', 'la', 'el', 'ar', 'nl', 'ja', 'pl', 'sv', 'zu', 'da', 'cs', 'hu', 'af', 'hi', 'tr', 'zh', 'ms', 'pa', 'id', 'ko', 'vi')")
+        if value not in set(['very calm', 'calm', 'moderate arousal', 'energetic', 'very energetic', 'varying arousal']):
+            raise ValueError("must be one of enum values ('very calm', 'calm', 'moderate arousal', 'energetic', 'very energetic', 'varying arousal')")
         return value
 
     @field_validator('dominant_instrument')
     def dominant_instrument_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -372,14 +374,24 @@
         if value is None:
             return value
 
         if value not in set(['Spotify', 'TikTok', 'Unfitting', 'YouTube']):
             raise ValueError("must be one of enum values ('Spotify', 'TikTok', 'Unfitting', 'YouTube')")
         return value
 
+    @field_validator('pretzel_station_suitability')
+    def pretzel_station_suitability_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in set(['Afro Beats', 'Alternative', 'Ambient', 'Apex Legends', 'Baten Kaitos', 'Blues', 'Call of Duty', 'Calming Cinematics', 'Chess', 'Chill Bass', 'Chill EDM', 'Chill Guitars', 'Chill Jazz', 'Chill Piano', 'Chill Pop', 'Chill', 'Chiptune', 'Classic Rock', 'Classical', 'Country', 'Drum _ Bass', 'Dungeons _ Dragons', 'EDM', 'Electro-Swing', 'Emo', 'Epic', 'Fifa', 'Final Fantasy', 'Folk', 'Fortnite', 'Forza Horizon', 'Funk', 'GTA', 'Happy EDM', 'Happy Holidays!', 'Hard Dance', 'Hip Hop', 'House Grooves', 'Hype Bangers!', 'Hype Bass!', 'Indie', 'Industrial', 'Jazz', 'Latin Pop', 'League of Legends', 'Lofi', 'Love Bug', 'Main Character', 'Meditation', 'Melodic Bass', 'Metal', 'Minecraft', 'Polka', 'Pop', 'Punk', 'R_B', 'Reggae', 'Rock', 'Ska', 'Spooky', 'Synthwave', 'Techno', 'The Elevator', 'The Lounge', 'Traditional Latin', 'Tran', 'Upbeat Dance', 'VHS', 'Valorant', 'World of Warcraft', 'World', 'Yacht Rock', 'Disco']):
+            raise ValueError("must be one of enum values ('Afro Beats', 'Alternative', 'Ambient', 'Apex Legends', 'Baten Kaitos', 'Blues', 'Call of Duty', 'Calming Cinematics', 'Chess', 'Chill Bass', 'Chill EDM', 'Chill Guitars', 'Chill Jazz', 'Chill Piano', 'Chill Pop', 'Chill', 'Chiptune', 'Classic Rock', 'Classical', 'Country', 'Drum _ Bass', 'Dungeons _ Dragons', 'EDM', 'Electro-Swing', 'Emo', 'Epic', 'Fifa', 'Final Fantasy', 'Folk', 'Fortnite', 'Forza Horizon', 'Funk', 'GTA', 'Happy EDM', 'Happy Holidays!', 'Hard Dance', 'Hip Hop', 'House Grooves', 'Hype Bangers!', 'Hype Bass!', 'Indie', 'Industrial', 'Jazz', 'Latin Pop', 'League of Legends', 'Lofi', 'Love Bug', 'Main Character', 'Meditation', 'Melodic Bass', 'Metal', 'Minecraft', 'Polka', 'Pop', 'Punk', 'R_B', 'Reggae', 'Rock', 'Ska', 'Spooky', 'Synthwave', 'Techno', 'The Elevator', 'The Lounge', 'Traditional Latin', 'Tran', 'Upbeat Dance', 'VHS', 'Valorant', 'World of Warcraft', 'World', 'Yacht Rock', 'Disco')")
+        return value
+
     @field_validator('loudness')
     def loudness_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
         if value not in set(['very low', 'low', 'moderate', 'high', 'very high']):
@@ -594,32 +606,32 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "space": obj.get("space"),
-            "arousal": obj.get("arousal"),
             "valenceAffinity": obj.get("valenceAffinity"),
-            "arousalAffinity": obj.get("arousalAffinity"),
-            "pleasantnessAffinity": obj.get("pleasantnessAffinity"),
-            "engagementAffinity": obj.get("engagementAffinity"),
-            "energyAffinity": obj.get("energyAffinity"),
             "tempoAffinity": obj.get("tempoAffinity"),
             "scaleAffinity": obj.get("scaleAffinity"),
             "timbreAffinity": obj.get("timbreAffinity"),
             "roughnessAffinity": obj.get("roughnessAffinity"),
             "harmonyAffinity": obj.get("harmonyAffinity"),
             "textureAffinity": obj.get("textureAffinity"),
             "groovynessAffinity": obj.get("groovynessAffinity"),
             "spaceAffinity": obj.get("spaceAffinity"),
             "loudnessAffinity": obj.get("loudnessAffinity"),
             "keyAffinity": obj.get("keyAffinity"),
             "channelSuitabilityAffinity": obj.get("channelSuitabilityAffinity"),
+            "arousalAffinity": obj.get("arousalAffinity"),
+            "pleasantnessAffinity": obj.get("pleasantnessAffinity"),
+            "engagementAffinity": obj.get("engagementAffinity"),
+            "energyAffinity": obj.get("energyAffinity"),
             "languageOfPerformance": obj.get("languageOfPerformance"),
+            "arousal": obj.get("arousal"),
             "dominantInstrument": obj.get("dominantInstrument"),
             "energy": obj.get("energy"),
             "engagement": obj.get("engagement"),
             "groovyness": obj.get("groovyness"),
             "harmony": obj.get("harmony"),
             "pleasantness": obj.get("pleasantness"),
             "primaryMoodCluster": obj.get("primaryMoodCluster"),
@@ -635,15 +647,17 @@
             "tonality": obj.get("tonality"),
             "valence": obj.get("valence"),
             "vocals": obj.get("vocals"),
             "originDecade": obj.get("originDecade"),
             "curateability": obj.get("curateability"),
             "useCase": obj.get("useCase"),
             "channelSuitability": obj.get("channelSuitability"),
+            "pretzelStationSuitability": obj.get("pretzelStationSuitability"),
             "loudness": obj.get("loudness"),
+            "bpm": obj.get("bpm"),
             "primaryMoodClusterAffinity": obj.get("primaryMoodClusterAffinity"),
             "secondaryMoodCluster": obj.get("secondaryMoodCluster"),
             "secondaryMoodClusterAffinity": obj.get("secondaryMoodClusterAffinity"),
             "tertiaryMoodCluster": obj.get("tertiaryMoodCluster"),
             "tertiaryMoodClusterAffinity": obj.get("tertiaryMoodClusterAffinity"),
             "vocalsAffinity": obj.get("vocalsAffinity"),
             "dominantInstrumentAffinity": obj.get("dominantInstrumentAffinity"),
@@ -651,15 +665,14 @@
             "secondaryInstrumentAffinity": obj.get("secondaryInstrumentAffinity"),
             "tertiaryInstrument": obj.get("tertiaryInstrument"),
             "tertiaryInstrumentAffinity": obj.get("tertiaryInstrumentAffinity"),
             "soundGenerationAffinity": obj.get("soundGenerationAffinity"),
             "rhythmAffinity": obj.get("rhythmAffinity"),
             "primarySoundCharacterAffinity": obj.get("primarySoundCharacterAffinity"),
             "tonalityAffinity": obj.get("tonalityAffinity"),
-            "bpm": obj.get("bpm"),
             "productionRating": obj.get("productionRating"),
             "productionRatingAffinity": obj.get("productionRatingAffinity"),
             "performanceRating": obj.get("performanceRating"),
             "performanceRatingAffinity": obj.get("performanceRatingAffinity"),
             "songRating": obj.get("songRating"),
             "songRatingAffinity": obj.get("songRatingAffinity"),
             "audienceAge": obj.get("audienceAge"),
@@ -679,12 +692,13 @@
             "originRegionAffinity": obj.get("originRegionAffinity"),
             "originDecadeAffinity": obj.get("originDecadeAffinity"),
             "languageOfPerformanceAffinity": obj.get("languageOfPerformanceAffinity"),
             "curateabilityAffinity": obj.get("curateabilityAffinity"),
             "useCaseAffinity": obj.get("useCaseAffinity"),
             "industrySuitability": obj.get("industrySuitability"),
             "industrySuitabilityAffinity": obj.get("industrySuitabilityAffinity"),
+            "pretzelStationSuitabilityAffinity": obj.get("pretzelStationSuitabilityAffinity"),
             "audienceRegion": obj.get("audienceRegion")
         })
         return _obj
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/party_small_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/party_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_for_similarity_search_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_for_similarity_search_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_genre_prediction_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_genre_prediction_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_list_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_list_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_medium_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_medium_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -35,22 +35,22 @@
     """
     Recording with a mid-sized field set.
     """ # noqa: E501
     isrc: StrictStr
     genres: Optional[List[GenreDTO]] = None
     language_of_performance: Optional[StrictStr] = Field(default=None, alias="languageOfPerformance")
     release_date: Optional[datetime] = Field(default=None, alias="releaseDate")
+    recording_party_entities: Optional[List[RecordingPartyDTO]] = Field(default=None, alias="recordingPartyEntities")
     titles: Optional[List[TitleDTO]] = None
     tracks: Optional[List[TrackDTO]] = None
     musical_features: Optional[MusicalFeaturesDTO] = Field(default=None, alias="musicalFeatures")
-    recording_party_entities: Optional[List[RecordingPartyDTO]] = Field(default=None, alias="recordingPartyEntities")
     spotify_id: Optional[StrictStr] = Field(default=None, alias="spotifyId")
     tags: Optional[List[RecordingTagSmallDTO]] = None
     genre_predictions: Optional[List[RecordingGenrePredictionDTO]] = Field(default=None, alias="genrePredictions")
-    __properties: ClassVar[List[str]] = ["isrc", "genres", "languageOfPerformance", "releaseDate", "titles", "tracks", "musicalFeatures", "recordingPartyEntities", "spotifyId", "tags", "genrePredictions"]
+    __properties: ClassVar[List[str]] = ["isrc", "genres", "languageOfPerformance", "releaseDate", "recordingPartyEntities", "titles", "tracks", "musicalFeatures", "spotifyId", "tags", "genrePredictions"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -90,14 +90,21 @@
         # override the default output from pydantic by calling `to_dict()` of each item in genres (list)
         _items = []
         if self.genres:
             for _item in self.genres:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['genres'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in recording_party_entities (list)
+        _items = []
+        if self.recording_party_entities:
+            for _item in self.recording_party_entities:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['recordingPartyEntities'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in titles (list)
         _items = []
         if self.titles:
             for _item in self.titles:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['titles'] = _items
@@ -107,21 +114,14 @@
             for _item in self.tracks:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['tracks'] = _items
         # override the default output from pydantic by calling `to_dict()` of musical_features
         if self.musical_features:
             _dict['musicalFeatures'] = self.musical_features.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in recording_party_entities (list)
-        _items = []
-        if self.recording_party_entities:
-            for _item in self.recording_party_entities:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['recordingPartyEntities'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in tags (list)
         _items = []
         if self.tags:
             for _item in self.tags:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['tags'] = _items
@@ -144,18 +144,18 @@
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "isrc": obj.get("isrc"),
             "genres": [GenreDTO.from_dict(_item) for _item in obj["genres"]] if obj.get("genres") is not None else None,
             "languageOfPerformance": obj.get("languageOfPerformance"),
             "releaseDate": obj.get("releaseDate"),
+            "recordingPartyEntities": [RecordingPartyDTO.from_dict(_item) for _item in obj["recordingPartyEntities"]] if obj.get("recordingPartyEntities") is not None else None,
             "titles": [TitleDTO.from_dict(_item) for _item in obj["titles"]] if obj.get("titles") is not None else None,
             "tracks": [TrackDTO.from_dict(_item) for _item in obj["tracks"]] if obj.get("tracks") is not None else None,
             "musicalFeatures": MusicalFeaturesDTO.from_dict(obj["musicalFeatures"]) if obj.get("musicalFeatures") is not None else None,
-            "recordingPartyEntities": [RecordingPartyDTO.from_dict(_item) for _item in obj["recordingPartyEntities"]] if obj.get("recordingPartyEntities") is not None else None,
             "spotifyId": obj.get("spotifyId"),
             "tags": [RecordingTagSmallDTO.from_dict(_item) for _item in obj["tags"]] if obj.get("tags") is not None else None,
             "genrePredictions": [RecordingGenrePredictionDTO.from_dict(_item) for _item in obj["genrePredictions"]] if obj.get("genrePredictions") is not None else None
         })
         return _obj
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_party_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_party_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_small_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_small_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -28,18 +28,18 @@
 
 class RecordingSmallDTO(BaseModel):
     """
     Recording with a small field set.
     """ # noqa: E501
     duration: Optional[StrictInt] = None
     isrc: StrictStr
+    parties: Optional[List[RecordingPartyDTO]] = None
     titles: Optional[List[TitleDTO]] = None
     tracks: Optional[List[TrackDTO]] = None
-    parties: Optional[List[RecordingPartyDTO]] = None
-    __properties: ClassVar[List[str]] = ["duration", "isrc", "titles", "tracks", "parties"]
+    __properties: ClassVar[List[str]] = ["duration", "isrc", "parties", "titles", "tracks"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -72,49 +72,49 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in parties (list)
+        _items = []
+        if self.parties:
+            for _item in self.parties:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['parties'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in titles (list)
         _items = []
         if self.titles:
             for _item in self.titles:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['titles'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in tracks (list)
         _items = []
         if self.tracks:
             for _item in self.tracks:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['tracks'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in parties (list)
-        _items = []
-        if self.parties:
-            for _item in self.parties:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['parties'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of RecordingSmallDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "duration": obj.get("duration"),
             "isrc": obj.get("isrc"),
+            "parties": [RecordingPartyDTO.from_dict(_item) for _item in obj["parties"]] if obj.get("parties") is not None else None,
             "titles": [TitleDTO.from_dict(_item) for _item in obj["titles"]] if obj.get("titles") is not None else None,
-            "tracks": [TrackDTO.from_dict(_item) for _item in obj["tracks"]] if obj.get("tracks") is not None else None,
-            "parties": [RecordingPartyDTO.from_dict(_item) for _item in obj["parties"]] if obj.get("parties") is not None else None
+            "tracks": [TrackDTO.from_dict(_item) for _item in obj["tracks"]] if obj.get("tracks") is not None else None
         })
         return _obj
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/recording_tag_small_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_tag_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/save_user_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/save_user_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/search_filter_values_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/search_filter_values_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -65,15 +65,16 @@
     tertiary_audience_region: List[StrictStr] = Field(alias="tertiaryAudienceRegion")
     origin_decade: List[StrictStr] = Field(alias="originDecade")
     origin_region: List[StrictStr] = Field(alias="originRegion")
     language_of_performance: List[StrictStr] = Field(alias="languageOfPerformance")
     curateability: List[StrictStr]
     use_case: List[StrictStr] = Field(alias="useCase")
     channel_suitability: List[StrictStr] = Field(alias="channelSuitability")
-    __properties: ClassVar[List[str]] = ["primaryMoodCluster", "secondaryMoodCluster", "tertiaryMoodCluster", "valence", "arousal", "pleasantness", "engagement", "vocals", "dominantInstrument", "secondaryInstrument", "tertiaryInstrument", "energy", "soundGeneration", "tempo", "scale", "key", "rhythm", "primarySoundCharacter", "timbre", "roughness", "tonality", "harmony", "texture", "groovyness", "space", "loudness", "productionRating", "performanceRating", "songRating", "audienceAge", "secondaryAudienceAge", "tertiaryAudienceAge", "audienceGender", "audienceRegion", "secondaryAudienceRegion", "tertiaryAudienceRegion", "originDecade", "originRegion", "languageOfPerformance", "curateability", "useCase", "channelSuitability"]
+    pretzel_station_suitability: List[StrictStr] = Field(alias="pretzelStationSuitability")
+    __properties: ClassVar[List[str]] = ["primaryMoodCluster", "secondaryMoodCluster", "tertiaryMoodCluster", "valence", "arousal", "pleasantness", "engagement", "vocals", "dominantInstrument", "secondaryInstrument", "tertiaryInstrument", "energy", "soundGeneration", "tempo", "scale", "key", "rhythm", "primarySoundCharacter", "timbre", "roughness", "tonality", "harmony", "texture", "groovyness", "space", "loudness", "productionRating", "performanceRating", "songRating", "audienceAge", "secondaryAudienceAge", "tertiaryAudienceAge", "audienceGender", "audienceRegion", "secondaryAudienceRegion", "tertiaryAudienceRegion", "originDecade", "originRegion", "languageOfPerformance", "curateability", "useCase", "channelSuitability", "pretzelStationSuitability"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -159,12 +160,13 @@
             "secondaryAudienceRegion": obj.get("secondaryAudienceRegion"),
             "tertiaryAudienceRegion": obj.get("tertiaryAudienceRegion"),
             "originDecade": obj.get("originDecade"),
             "originRegion": obj.get("originRegion"),
             "languageOfPerformance": obj.get("languageOfPerformance"),
             "curateability": obj.get("curateability"),
             "useCase": obj.get("useCase"),
-            "channelSuitability": obj.get("channelSuitability")
+            "channelSuitability": obj.get("channelSuitability"),
+            "pretzelStationSuitability": obj.get("pretzelStationSuitability")
         })
         return _obj
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/sign_up_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/sign_up_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/tag_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/tag_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/tag_small_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/tag_small_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/taggram_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/taggram_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/tags_summary_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/tags_summary_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/tagstrength_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/tagstrength_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/title_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/title_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/token_request.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/track_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/track_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/update_password_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/update_password_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/user_dto.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/user_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/models/video_recognition_response.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/video_recognition_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python/rest.py` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -199,14 +199,16 @@
                         preload_content=False
                     )
                 elif content_type == 'multipart/form-data':
                     # must del headers['Content-Type'], or the correct
                     # Content-Type which generated by urllib3 will be
                     # overwritten.
                     del headers['Content-Type']
+                    # Ensures that dict objects are serialized
+                    post_params = [(a, json.dumps(b)) if isinstance(b, dict) else (a,b) for a, b in post_params]
                     r = self.pool_manager.request(
                         method,
                         url,
                         fields=post_params,
                         encode_multipart=True,
                         timeout=timeout,
                         headers=headers,
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python.egg-info/PKG-INFO` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songtradr-api-client-python
-Version: 2.0.0
+Version: 2.1.0
 Summary: Songtradr API
 Home-page: https://github.com/songtradr/songtradr-python-api-client-docs
 Author: Songtradr Inc.
 Author-email: info@songtradr.com
 Keywords: OpenAPI,OpenAPI-Generator,Songtradr API
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
```

### Comparing `songtradr-api-client-python-2.0.0/songtradr_api_client_python.egg-info/SOURCES.txt` & `songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `songtradr-api-client-python-2.0.0/test/test_allowed_values_api.py` & `songtradr_api_client_python-2.1.0/test/test_allowed_values_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_category_medium_dto.py` & `songtradr_api_client_python-2.1.0/test/test_category_medium_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_category_minimal_dto.py` & `songtradr_api_client_python-2.1.0/test/test_category_minimal_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_config_access_dto.py` & `songtradr_api_client_python-2.1.0/test/test_config_access_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_config_identifier_dto.py` & `songtradr_api_client_python-2.1.0/test/test_config_identifier_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_contributor_type_dto.py` & `songtradr_api_client_python-2.1.0/test/test_contributor_type_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_error_response.py` & `songtradr_api_client_python-2.1.0/test/test_error_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_field_summary_dto.py` & `songtradr_api_client_python-2.1.0/test/test_field_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_file_dto.py` & `songtradr_api_client_python-2.1.0/test/test_file_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -55,42 +55,52 @@
                     genres = [
                         songtradr_api_client_python.models.genre_dto.GenreDTO(
                             id = 56, 
                             name = '', )
                         ], 
                     language_of_performance = '', 
                     release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    recording_party_entities = [
+                        songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                            party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                id = '', 
+                                full_name = '', ), 
+                            contributor_types = [
+                                songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
+                                    type_name = '', )
+                                ], )
+                        ], 
                     titles = [
                         songtradr_api_client_python.models.title_dto.TitleDTO(
                             title_text = '', )
                         ], 
                     tracks = [
                         songtradr_api_client_python.models.track_dto.TrackDTO(
                             songtradr_track_id = '', )
                         ], 
                     musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                         space = 'very compact', 
-                        arousal = 'very calm', 
                         valence_affinity = 1.337, 
-                        arousal_affinity = 1.337, 
-                        pleasantness_affinity = 1.337, 
-                        engagement_affinity = 1.337, 
-                        energy_affinity = 1.337, 
                         tempo_affinity = 1.337, 
                         scale_affinity = 1.337, 
                         timbre_affinity = 1.337, 
                         roughness_affinity = 1.337, 
                         harmony_affinity = 1.337, 
                         texture_affinity = 1.337, 
                         groovyness_affinity = 1.337, 
                         space_affinity = 1.337, 
                         loudness_affinity = 1.337, 
                         key_affinity = 1.337, 
                         channel_suitability_affinity = 1.337, 
+                        arousal_affinity = 1.337, 
+                        pleasantness_affinity = 1.337, 
+                        engagement_affinity = 1.337, 
+                        energy_affinity = 1.337, 
                         language_of_performance = 'en', 
+                        arousal = 'very calm', 
                         dominant_instrument = 'piano', 
                         energy = 'very quiet', 
                         engagement = 'very unengaging', 
                         groovyness = 'very steady', 
                         harmony = 'very dissonant', 
                         pleasantness = 'very unpleasant', 
                         primary_mood_cluster = 'aggressive', 
@@ -106,15 +116,17 @@
                         tonality = 'monotonous', 
                         valence = 'very sad', 
                         vocals = 'instrumental', 
                         origin_decade = 'pre-1950s', 
                         curateability = 'curateable', 
                         use_case = 'background', 
                         channel_suitability = 'Spotify', 
+                        pretzel_station_suitability = 'Afro Beats', 
                         loudness = 'very low', 
+                        bpm = 1.337, 
                         primary_mood_cluster_affinity = 1.337, 
                         secondary_mood_cluster = 'aggressive', 
                         secondary_mood_cluster_affinity = 1.337, 
                         tertiary_mood_cluster = 'aggressive', 
                         tertiary_mood_cluster_affinity = 1.337, 
                         vocals_affinity = 1.337, 
                         dominant_instrument_affinity = 1.337, 
@@ -122,15 +134,14 @@
                         secondary_instrument_affinity = 1.337, 
                         tertiary_instrument = 'piano', 
                         tertiary_instrument_affinity = 1.337, 
                         sound_generation_affinity = 1.337, 
                         rhythm_affinity = 1.337, 
                         primary_sound_character_affinity = 1.337, 
                         tonality_affinity = 1.337, 
-                        bpm = 1.337, 
                         production_rating = 'low production quality', 
                         production_rating_affinity = 1.337, 
                         performance_rating = 'low performance quality', 
                         performance_rating_affinity = 1.337, 
                         song_rating = 'low song quality', 
                         song_rating_affinity = 1.337, 
                         audience_age = 'Generation Z', 
@@ -150,25 +161,16 @@
                         origin_region_affinity = 1.337, 
                         origin_decade_affinity = 1.337, 
                         language_of_performance_affinity = 1.337, 
                         curateability_affinity = 1.337, 
                         use_case_affinity = 1.337, 
                         industry_suitability = 'Automobiles and Parts', 
                         industry_suitability_affinity = 1.337, 
+                        pretzel_station_suitability_affinity = 1.337, 
                         audience_region = 'Australia and New Zealand', ), 
-                    recording_party_entities = [
-                        songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
-                            party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                id = '', 
-                                full_name = '', ), 
-                            contributor_types = [
-                                songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
-                                    type_name = '', )
-                                ], )
-                        ], 
                     spotify_id = '', 
                     tags = [
                         songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
                             tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                                 id = 56, 
                                 name = '', 
                                 categories = [
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_file_list_dto.py` & `songtradr_api_client_python-2.1.0/test/test_file_list_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -57,42 +57,52 @@
                             genres = [
                                 songtradr_api_client_python.models.genre_dto.GenreDTO(
                                     id = 56, 
                                     name = '', )
                                 ], 
                             language_of_performance = '', 
                             release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            recording_party_entities = [
+                                songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                                    party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                        id = '', 
+                                        full_name = '', ), 
+                                    contributor_types = [
+                                        songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
+                                            type_name = '', )
+                                        ], )
+                                ], 
                             titles = [
                                 songtradr_api_client_python.models.title_dto.TitleDTO(
                                     title_text = '', )
                                 ], 
                             tracks = [
                                 songtradr_api_client_python.models.track_dto.TrackDTO(
                                     songtradr_track_id = '', )
                                 ], 
                             musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                                 space = 'very compact', 
-                                arousal = 'very calm', 
                                 valence_affinity = 1.337, 
-                                arousal_affinity = 1.337, 
-                                pleasantness_affinity = 1.337, 
-                                engagement_affinity = 1.337, 
-                                energy_affinity = 1.337, 
                                 tempo_affinity = 1.337, 
                                 scale_affinity = 1.337, 
                                 timbre_affinity = 1.337, 
                                 roughness_affinity = 1.337, 
                                 harmony_affinity = 1.337, 
                                 texture_affinity = 1.337, 
                                 groovyness_affinity = 1.337, 
                                 space_affinity = 1.337, 
                                 loudness_affinity = 1.337, 
                                 key_affinity = 1.337, 
                                 channel_suitability_affinity = 1.337, 
+                                arousal_affinity = 1.337, 
+                                pleasantness_affinity = 1.337, 
+                                engagement_affinity = 1.337, 
+                                energy_affinity = 1.337, 
                                 language_of_performance = 'en', 
+                                arousal = 'very calm', 
                                 dominant_instrument = 'piano', 
                                 energy = 'very quiet', 
                                 engagement = 'very unengaging', 
                                 groovyness = 'very steady', 
                                 harmony = 'very dissonant', 
                                 pleasantness = 'very unpleasant', 
                                 primary_mood_cluster = 'aggressive', 
@@ -108,15 +118,17 @@
                                 tonality = 'monotonous', 
                                 valence = 'very sad', 
                                 vocals = 'instrumental', 
                                 origin_decade = 'pre-1950s', 
                                 curateability = 'curateable', 
                                 use_case = 'background', 
                                 channel_suitability = 'Spotify', 
+                                pretzel_station_suitability = 'Afro Beats', 
                                 loudness = 'very low', 
+                                bpm = 1.337, 
                                 primary_mood_cluster_affinity = 1.337, 
                                 secondary_mood_cluster = 'aggressive', 
                                 secondary_mood_cluster_affinity = 1.337, 
                                 tertiary_mood_cluster = 'aggressive', 
                                 tertiary_mood_cluster_affinity = 1.337, 
                                 vocals_affinity = 1.337, 
                                 dominant_instrument_affinity = 1.337, 
@@ -124,15 +136,14 @@
                                 secondary_instrument_affinity = 1.337, 
                                 tertiary_instrument = 'piano', 
                                 tertiary_instrument_affinity = 1.337, 
                                 sound_generation_affinity = 1.337, 
                                 rhythm_affinity = 1.337, 
                                 primary_sound_character_affinity = 1.337, 
                                 tonality_affinity = 1.337, 
-                                bpm = 1.337, 
                                 production_rating = 'low production quality', 
                                 production_rating_affinity = 1.337, 
                                 performance_rating = 'low performance quality', 
                                 performance_rating_affinity = 1.337, 
                                 song_rating = 'low song quality', 
                                 song_rating_affinity = 1.337, 
                                 audience_age = 'Generation Z', 
@@ -152,25 +163,16 @@
                                 origin_region_affinity = 1.337, 
                                 origin_decade_affinity = 1.337, 
                                 language_of_performance_affinity = 1.337, 
                                 curateability_affinity = 1.337, 
                                 use_case_affinity = 1.337, 
                                 industry_suitability = 'Automobiles and Parts', 
                                 industry_suitability_affinity = 1.337, 
+                                pretzel_station_suitability_affinity = 1.337, 
                                 audience_region = 'Australia and New Zealand', ), 
-                            recording_party_entities = [
-                                songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
-                                    party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                        id = '', 
-                                        full_name = '', ), 
-                                    contributor_types = [
-                                        songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
-                                            type_name = '', )
-                                        ], )
-                                ], 
                             spotify_id = '', 
                             tags = [
                                 songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
                                     tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                                         id = 56, 
                                         name = '', 
                                         categories = [
@@ -215,42 +217,52 @@
                             genres = [
                                 songtradr_api_client_python.models.genre_dto.GenreDTO(
                                     id = 56, 
                                     name = '', )
                                 ], 
                             language_of_performance = '', 
                             release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            recording_party_entities = [
+                                songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                                    party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                        id = '', 
+                                        full_name = '', ), 
+                                    contributor_types = [
+                                        songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
+                                            type_name = '', )
+                                        ], )
+                                ], 
                             titles = [
                                 songtradr_api_client_python.models.title_dto.TitleDTO(
                                     title_text = '', )
                                 ], 
                             tracks = [
                                 songtradr_api_client_python.models.track_dto.TrackDTO(
                                     songtradr_track_id = '', )
                                 ], 
                             musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                                 space = 'very compact', 
-                                arousal = 'very calm', 
                                 valence_affinity = 1.337, 
-                                arousal_affinity = 1.337, 
-                                pleasantness_affinity = 1.337, 
-                                engagement_affinity = 1.337, 
-                                energy_affinity = 1.337, 
                                 tempo_affinity = 1.337, 
                                 scale_affinity = 1.337, 
                                 timbre_affinity = 1.337, 
                                 roughness_affinity = 1.337, 
                                 harmony_affinity = 1.337, 
                                 texture_affinity = 1.337, 
                                 groovyness_affinity = 1.337, 
                                 space_affinity = 1.337, 
                                 loudness_affinity = 1.337, 
                                 key_affinity = 1.337, 
                                 channel_suitability_affinity = 1.337, 
+                                arousal_affinity = 1.337, 
+                                pleasantness_affinity = 1.337, 
+                                engagement_affinity = 1.337, 
+                                energy_affinity = 1.337, 
                                 language_of_performance = 'en', 
+                                arousal = 'very calm', 
                                 dominant_instrument = 'piano', 
                                 energy = 'very quiet', 
                                 engagement = 'very unengaging', 
                                 groovyness = 'very steady', 
                                 harmony = 'very dissonant', 
                                 pleasantness = 'very unpleasant', 
                                 primary_mood_cluster = 'aggressive', 
@@ -266,15 +278,17 @@
                                 tonality = 'monotonous', 
                                 valence = 'very sad', 
                                 vocals = 'instrumental', 
                                 origin_decade = 'pre-1950s', 
                                 curateability = 'curateable', 
                                 use_case = 'background', 
                                 channel_suitability = 'Spotify', 
+                                pretzel_station_suitability = 'Afro Beats', 
                                 loudness = 'very low', 
+                                bpm = 1.337, 
                                 primary_mood_cluster_affinity = 1.337, 
                                 secondary_mood_cluster = 'aggressive', 
                                 secondary_mood_cluster_affinity = 1.337, 
                                 tertiary_mood_cluster = 'aggressive', 
                                 tertiary_mood_cluster_affinity = 1.337, 
                                 vocals_affinity = 1.337, 
                                 dominant_instrument_affinity = 1.337, 
@@ -282,15 +296,14 @@
                                 secondary_instrument_affinity = 1.337, 
                                 tertiary_instrument = 'piano', 
                                 tertiary_instrument_affinity = 1.337, 
                                 sound_generation_affinity = 1.337, 
                                 rhythm_affinity = 1.337, 
                                 primary_sound_character_affinity = 1.337, 
                                 tonality_affinity = 1.337, 
-                                bpm = 1.337, 
                                 production_rating = 'low production quality', 
                                 production_rating_affinity = 1.337, 
                                 performance_rating = 'low performance quality', 
                                 performance_rating_affinity = 1.337, 
                                 song_rating = 'low song quality', 
                                 song_rating_affinity = 1.337, 
                                 audience_age = 'Generation Z', 
@@ -310,25 +323,16 @@
                                 origin_region_affinity = 1.337, 
                                 origin_decade_affinity = 1.337, 
                                 language_of_performance_affinity = 1.337, 
                                 curateability_affinity = 1.337, 
                                 use_case_affinity = 1.337, 
                                 industry_suitability = 'Automobiles and Parts', 
                                 industry_suitability_affinity = 1.337, 
+                                pretzel_station_suitability_affinity = 1.337, 
                                 audience_region = 'Australia and New Zealand', ), 
-                            recording_party_entities = [
-                                songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
-                                    party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                        id = '', 
-                                        full_name = '', ), 
-                                    contributor_types = [
-                                        songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
-                                            type_name = '', )
-                                        ], )
-                                ], 
                             spotify_id = '', 
                             tags = [
                                 songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
                                     tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                                         id = 56, 
                                         name = '', 
                                         categories = [
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_file_small_dto.py` & `songtradr_api_client_python-2.1.0/test/test_file_small_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -32,36 +32,36 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `FileSmallDTO`
         """
         model = FileSmallDTO()
         if include_optional:
             return FileSmallDTO(
+                folder = '',
                 name = '',
                 id = 56,
                 extension = 'mp3',
                 error_message = '',
-                folder = '',
                 fingerprint_status = 'processing',
                 object_key = '',
                 upload_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 upload_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 inference_status = 'processing',
                 inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 error_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
             )
         else:
             return FileSmallDTO(
+                folder = '',
                 name = '',
                 id = 56,
                 extension = 'mp3',
-                folder = '',
                 object_key = '',
         )
         """
 
     def testFileSmallDTO(self):
         """Test FileSmallDTO"""
         # inst_req_only = self.make_instance(include_optional=False)
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_file_upload_dto.py` & `songtradr_api_client_python-2.1.0/test/test_file_upload_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_file_w_ith_url_dto.py` & `songtradr_api_client_python-2.1.0/test/test_file_w_ith_url_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -56,42 +56,52 @@
                         genres = [
                             songtradr_api_client_python.models.genre_dto.GenreDTO(
                                 id = 56, 
                                 name = '', )
                             ], 
                         language_of_performance = '', 
                         release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        recording_party_entities = [
+                            songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                    id = '', 
+                                    full_name = '', ), 
+                                contributor_types = [
+                                    songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
+                                        type_name = '', )
+                                    ], )
+                            ], 
                         titles = [
                             songtradr_api_client_python.models.title_dto.TitleDTO(
                                 title_text = '', )
                             ], 
                         tracks = [
                             songtradr_api_client_python.models.track_dto.TrackDTO(
                                 songtradr_track_id = '', )
                             ], 
                         musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                             space = 'very compact', 
-                            arousal = 'very calm', 
                             valence_affinity = 1.337, 
-                            arousal_affinity = 1.337, 
-                            pleasantness_affinity = 1.337, 
-                            engagement_affinity = 1.337, 
-                            energy_affinity = 1.337, 
                             tempo_affinity = 1.337, 
                             scale_affinity = 1.337, 
                             timbre_affinity = 1.337, 
                             roughness_affinity = 1.337, 
                             harmony_affinity = 1.337, 
                             texture_affinity = 1.337, 
                             groovyness_affinity = 1.337, 
                             space_affinity = 1.337, 
                             loudness_affinity = 1.337, 
                             key_affinity = 1.337, 
                             channel_suitability_affinity = 1.337, 
+                            arousal_affinity = 1.337, 
+                            pleasantness_affinity = 1.337, 
+                            engagement_affinity = 1.337, 
+                            energy_affinity = 1.337, 
                             language_of_performance = 'en', 
+                            arousal = 'very calm', 
                             dominant_instrument = 'piano', 
                             energy = 'very quiet', 
                             engagement = 'very unengaging', 
                             groovyness = 'very steady', 
                             harmony = 'very dissonant', 
                             pleasantness = 'very unpleasant', 
                             primary_mood_cluster = 'aggressive', 
@@ -107,15 +117,17 @@
                             tonality = 'monotonous', 
                             valence = 'very sad', 
                             vocals = 'instrumental', 
                             origin_decade = 'pre-1950s', 
                             curateability = 'curateable', 
                             use_case = 'background', 
                             channel_suitability = 'Spotify', 
+                            pretzel_station_suitability = 'Afro Beats', 
                             loudness = 'very low', 
+                            bpm = 1.337, 
                             primary_mood_cluster_affinity = 1.337, 
                             secondary_mood_cluster = 'aggressive', 
                             secondary_mood_cluster_affinity = 1.337, 
                             tertiary_mood_cluster = 'aggressive', 
                             tertiary_mood_cluster_affinity = 1.337, 
                             vocals_affinity = 1.337, 
                             dominant_instrument_affinity = 1.337, 
@@ -123,15 +135,14 @@
                             secondary_instrument_affinity = 1.337, 
                             tertiary_instrument = 'piano', 
                             tertiary_instrument_affinity = 1.337, 
                             sound_generation_affinity = 1.337, 
                             rhythm_affinity = 1.337, 
                             primary_sound_character_affinity = 1.337, 
                             tonality_affinity = 1.337, 
-                            bpm = 1.337, 
                             production_rating = 'low production quality', 
                             production_rating_affinity = 1.337, 
                             performance_rating = 'low performance quality', 
                             performance_rating_affinity = 1.337, 
                             song_rating = 'low song quality', 
                             song_rating_affinity = 1.337, 
                             audience_age = 'Generation Z', 
@@ -151,25 +162,16 @@
                             origin_region_affinity = 1.337, 
                             origin_decade_affinity = 1.337, 
                             language_of_performance_affinity = 1.337, 
                             curateability_affinity = 1.337, 
                             use_case_affinity = 1.337, 
                             industry_suitability = 'Automobiles and Parts', 
                             industry_suitability_affinity = 1.337, 
+                            pretzel_station_suitability_affinity = 1.337, 
                             audience_region = 'Australia and New Zealand', ), 
-                        recording_party_entities = [
-                            songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
-                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                    id = '', 
-                                    full_name = '', ), 
-                                contributor_types = [
-                                    songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
-                                        type_name = '', )
-                                    ], )
-                            ], 
                         spotify_id = '', 
                         tags = [
                             songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
                                 tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                                     id = 56, 
                                     name = '', 
                                     categories = [
@@ -210,42 +212,52 @@
                         genres = [
                             songtradr_api_client_python.models.genre_dto.GenreDTO(
                                 id = 56, 
                                 name = '', )
                             ], 
                         language_of_performance = '', 
                         release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        recording_party_entities = [
+                            songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                    id = '', 
+                                    full_name = '', ), 
+                                contributor_types = [
+                                    songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
+                                        type_name = '', )
+                                    ], )
+                            ], 
                         titles = [
                             songtradr_api_client_python.models.title_dto.TitleDTO(
                                 title_text = '', )
                             ], 
                         tracks = [
                             songtradr_api_client_python.models.track_dto.TrackDTO(
                                 songtradr_track_id = '', )
                             ], 
                         musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                             space = 'very compact', 
-                            arousal = 'very calm', 
                             valence_affinity = 1.337, 
-                            arousal_affinity = 1.337, 
-                            pleasantness_affinity = 1.337, 
-                            engagement_affinity = 1.337, 
-                            energy_affinity = 1.337, 
                             tempo_affinity = 1.337, 
                             scale_affinity = 1.337, 
                             timbre_affinity = 1.337, 
                             roughness_affinity = 1.337, 
                             harmony_affinity = 1.337, 
                             texture_affinity = 1.337, 
                             groovyness_affinity = 1.337, 
                             space_affinity = 1.337, 
                             loudness_affinity = 1.337, 
                             key_affinity = 1.337, 
                             channel_suitability_affinity = 1.337, 
+                            arousal_affinity = 1.337, 
+                            pleasantness_affinity = 1.337, 
+                            engagement_affinity = 1.337, 
+                            energy_affinity = 1.337, 
                             language_of_performance = 'en', 
+                            arousal = 'very calm', 
                             dominant_instrument = 'piano', 
                             energy = 'very quiet', 
                             engagement = 'very unengaging', 
                             groovyness = 'very steady', 
                             harmony = 'very dissonant', 
                             pleasantness = 'very unpleasant', 
                             primary_mood_cluster = 'aggressive', 
@@ -261,15 +273,17 @@
                             tonality = 'monotonous', 
                             valence = 'very sad', 
                             vocals = 'instrumental', 
                             origin_decade = 'pre-1950s', 
                             curateability = 'curateable', 
                             use_case = 'background', 
                             channel_suitability = 'Spotify', 
+                            pretzel_station_suitability = 'Afro Beats', 
                             loudness = 'very low', 
+                            bpm = 1.337, 
                             primary_mood_cluster_affinity = 1.337, 
                             secondary_mood_cluster = 'aggressive', 
                             secondary_mood_cluster_affinity = 1.337, 
                             tertiary_mood_cluster = 'aggressive', 
                             tertiary_mood_cluster_affinity = 1.337, 
                             vocals_affinity = 1.337, 
                             dominant_instrument_affinity = 1.337, 
@@ -277,15 +291,14 @@
                             secondary_instrument_affinity = 1.337, 
                             tertiary_instrument = 'piano', 
                             tertiary_instrument_affinity = 1.337, 
                             sound_generation_affinity = 1.337, 
                             rhythm_affinity = 1.337, 
                             primary_sound_character_affinity = 1.337, 
                             tonality_affinity = 1.337, 
-                            bpm = 1.337, 
                             production_rating = 'low production quality', 
                             production_rating_affinity = 1.337, 
                             performance_rating = 'low performance quality', 
                             performance_rating_affinity = 1.337, 
                             song_rating = 'low song quality', 
                             song_rating_affinity = 1.337, 
                             audience_age = 'Generation Z', 
@@ -305,25 +318,16 @@
                             origin_region_affinity = 1.337, 
                             origin_decade_affinity = 1.337, 
                             language_of_performance_affinity = 1.337, 
                             curateability_affinity = 1.337, 
                             use_case_affinity = 1.337, 
                             industry_suitability = 'Automobiles and Parts', 
                             industry_suitability_affinity = 1.337, 
+                            pretzel_station_suitability_affinity = 1.337, 
                             audience_region = 'Australia and New Zealand', ), 
-                        recording_party_entities = [
-                            songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
-                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                    id = '', 
-                                    full_name = '', ), 
-                                contributor_types = [
-                                    songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
-                                        type_name = '', )
-                                    ], )
-                            ], 
                         spotify_id = '', 
                         tags = [
                             songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
                                 tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                                     id = 56, 
                                     name = '', 
                                     categories = [
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_files_summary_dto.py` & `songtradr_api_client_python-2.1.0/test/test_files_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_forgot_password_dto.py` & `songtradr_api_client_python-2.1.0/test/test_forgot_password_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_genre_dto.py` & `songtradr_api_client_python-2.1.0/test/test_genre_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_genre_minimal_dto.py` & `songtradr_api_client_python-2.1.0/test/test_genre_minimal_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_genres_summary_dto.py` & `songtradr_api_client_python-2.1.0/test/test_genres_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_image_recognition_response.py` & `songtradr_api_client_python-2.1.0/test/test_image_recognition_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_init_put_recording_audio_dto.py` & `songtradr_api_client_python-2.1.0/test/test_init_put_recording_audio_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_jwt_token_dto.py` & `songtradr_api_client_python-2.1.0/test/test_jwt_token_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_login_dto.py` & `songtradr_api_client_python-2.1.0/test/test_login_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_musical_features_dto.py` & `songtradr_api_client_python-2.1.0/test/test_musical_features_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -33,32 +33,32 @@
             optional params are included """
         # uncomment below to create an instance of `MusicalFeaturesDTO`
         """
         model = MusicalFeaturesDTO()
         if include_optional:
             return MusicalFeaturesDTO(
                 space = 'very compact',
-                arousal = 'very calm',
                 valence_affinity = 1.337,
-                arousal_affinity = 1.337,
-                pleasantness_affinity = 1.337,
-                engagement_affinity = 1.337,
-                energy_affinity = 1.337,
                 tempo_affinity = 1.337,
                 scale_affinity = 1.337,
                 timbre_affinity = 1.337,
                 roughness_affinity = 1.337,
                 harmony_affinity = 1.337,
                 texture_affinity = 1.337,
                 groovyness_affinity = 1.337,
                 space_affinity = 1.337,
                 loudness_affinity = 1.337,
                 key_affinity = 1.337,
                 channel_suitability_affinity = 1.337,
+                arousal_affinity = 1.337,
+                pleasantness_affinity = 1.337,
+                engagement_affinity = 1.337,
+                energy_affinity = 1.337,
                 language_of_performance = 'en',
+                arousal = 'very calm',
                 dominant_instrument = 'piano',
                 energy = 'very quiet',
                 engagement = 'very unengaging',
                 groovyness = 'very steady',
                 harmony = 'very dissonant',
                 pleasantness = 'very unpleasant',
                 primary_mood_cluster = 'aggressive',
@@ -74,15 +74,17 @@
                 tonality = 'monotonous',
                 valence = 'very sad',
                 vocals = 'instrumental',
                 origin_decade = 'pre-1950s',
                 curateability = 'curateable',
                 use_case = 'background',
                 channel_suitability = 'Spotify',
+                pretzel_station_suitability = 'Afro Beats',
                 loudness = 'very low',
+                bpm = 1.337,
                 primary_mood_cluster_affinity = 1.337,
                 secondary_mood_cluster = 'aggressive',
                 secondary_mood_cluster_affinity = 1.337,
                 tertiary_mood_cluster = 'aggressive',
                 tertiary_mood_cluster_affinity = 1.337,
                 vocals_affinity = 1.337,
                 dominant_instrument_affinity = 1.337,
@@ -90,15 +92,14 @@
                 secondary_instrument_affinity = 1.337,
                 tertiary_instrument = 'piano',
                 tertiary_instrument_affinity = 1.337,
                 sound_generation_affinity = 1.337,
                 rhythm_affinity = 1.337,
                 primary_sound_character_affinity = 1.337,
                 tonality_affinity = 1.337,
-                bpm = 1.337,
                 production_rating = 'low production quality',
                 production_rating_affinity = 1.337,
                 performance_rating = 'low performance quality',
                 performance_rating_affinity = 1.337,
                 song_rating = 'low song quality',
                 song_rating_affinity = 1.337,
                 audience_age = 'Generation Z',
@@ -118,14 +119,15 @@
                 origin_region_affinity = 1.337,
                 origin_decade_affinity = 1.337,
                 language_of_performance_affinity = 1.337,
                 curateability_affinity = 1.337,
                 use_case_affinity = 1.337,
                 industry_suitability = 'Automobiles and Parts',
                 industry_suitability_affinity = 1.337,
+                pretzel_station_suitability_affinity = 1.337,
                 audience_region = 'Australia and New Zealand'
             )
         else:
             return MusicalFeaturesDTO(
         )
         """
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_party_small_dto.py` & `songtradr_api_client_python-2.1.0/test/test_party_small_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_recording_api.py` & `songtradr_api_client_python-2.1.0/test/test_recording_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -37,37 +37,37 @@
     def test_recordings_by_ids_with_musical_features(self) -> None:
         """Test case for recordings_by_ids_with_musical_features
 
         AI generated moods, musical features and more for recordings.
         """
         pass
 
-    def test_recordings_by_ids_with_similarities(self) -> None:
-        """Test case for recordings_by_ids_with_similarities
+    def test_recordings_by_ids_with_similarities1(self) -> None:
+        """Test case for recordings_by_ids_with_similarities1
 
         Similar recordings for a list of recordings.
         """
         pass
 
-    def test_recordings_by_ids_with_taggrams(self) -> None:
-        """Test case for recordings_by_ids_with_taggrams
+    def test_recordings_by_ids_with_taggrams1(self) -> None:
+        """Test case for recordings_by_ids_with_taggrams1
 
         Timeseries of AI generated moods, musical features and more for a list of recordings.
         """
         pass
 
-    def test_recordings_by_ids_with_tagstrengths(self) -> None:
-        """Test case for recordings_by_ids_with_tagstrengths
+    def test_recordings_by_ids_with_tagstrengths1(self) -> None:
+        """Test case for recordings_by_ids_with_tagstrengths1
 
         Strengths as numerical representations for AI generated moods, musical features and more for recordings.
         """
         pass
 
-    def test_recordings_medium_by_ids(self) -> None:
-        """Test case for recordings_medium_by_ids
+    def test_recordings_medium_by_ids1(self) -> None:
+        """Test case for recordings_medium_by_ids1
 
         Recordings by IDs with a medium sized response.
         """
         pass
 
     def test_search_recordings(self) -> None:
         """Test case for search_recordings
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_recording_for_similarity_search_dto.py` & `songtradr_api_client_python-2.1.0/test/test_recording_for_similarity_search_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -35,56 +35,56 @@
         """
         model = RecordingForSimilaritySearchDTO()
         if include_optional:
             return RecordingForSimilaritySearchDTO(
                 recording = songtradr_api_client_python.models.recording_small_dto.RecordingSmallDTO(
                     duration = 56, 
                     isrc = '', 
-                    titles = [
-                        songtradr_api_client_python.models.title_dto.TitleDTO(
-                            title_text = '', )
-                        ], 
-                    tracks = [
-                        songtradr_api_client_python.models.track_dto.TrackDTO(
-                            songtradr_track_id = '', )
-                        ], 
                     parties = [
                         songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                             party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                 id = '', 
                                 full_name = '', ), 
                             contributor_types = [
                                 songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                     type_name = '', )
                                 ], )
+                        ], 
+                    titles = [
+                        songtradr_api_client_python.models.title_dto.TitleDTO(
+                            title_text = '', )
+                        ], 
+                    tracks = [
+                        songtradr_api_client_python.models.track_dto.TrackDTO(
+                            songtradr_track_id = '', )
                         ], ),
                 score = 1.337
             )
         else:
             return RecordingForSimilaritySearchDTO(
                 recording = songtradr_api_client_python.models.recording_small_dto.RecordingSmallDTO(
                     duration = 56, 
                     isrc = '', 
-                    titles = [
-                        songtradr_api_client_python.models.title_dto.TitleDTO(
-                            title_text = '', )
-                        ], 
-                    tracks = [
-                        songtradr_api_client_python.models.track_dto.TrackDTO(
-                            songtradr_track_id = '', )
-                        ], 
                     parties = [
                         songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                             party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                 id = '', 
                                 full_name = '', ), 
                             contributor_types = [
                                 songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                     type_name = '', )
                                 ], )
+                        ], 
+                    titles = [
+                        songtradr_api_client_python.models.title_dto.TitleDTO(
+                            title_text = '', )
+                        ], 
+                    tracks = [
+                        songtradr_api_client_python.models.track_dto.TrackDTO(
+                            songtradr_track_id = '', )
                         ], ),
                 score = 1.337,
         )
         """
 
     def testRecordingForSimilaritySearchDTO(self):
         """Test RecordingForSimilaritySearchDTO"""
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_recording_genre_prediction_dto.py` & `songtradr_api_client_python-2.1.0/test/test_recording_genre_prediction_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_recording_list_dto.py` & `songtradr_api_client_python-2.1.0/test/test_recording_list_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -42,42 +42,52 @@
                         genres = [
                             songtradr_api_client_python.models.genre_dto.GenreDTO(
                                 id = 56, 
                                 name = '', )
                             ], 
                         language_of_performance = '', 
                         release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        recording_party_entities = [
+                            songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                    id = '', 
+                                    full_name = '', ), 
+                                contributor_types = [
+                                    songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
+                                        type_name = '', )
+                                    ], )
+                            ], 
                         titles = [
                             songtradr_api_client_python.models.title_dto.TitleDTO(
                                 title_text = '', )
                             ], 
                         tracks = [
                             songtradr_api_client_python.models.track_dto.TrackDTO(
                                 songtradr_track_id = '', )
                             ], 
                         musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                             space = 'very compact', 
-                            arousal = 'very calm', 
                             valence_affinity = 1.337, 
-                            arousal_affinity = 1.337, 
-                            pleasantness_affinity = 1.337, 
-                            engagement_affinity = 1.337, 
-                            energy_affinity = 1.337, 
                             tempo_affinity = 1.337, 
                             scale_affinity = 1.337, 
                             timbre_affinity = 1.337, 
                             roughness_affinity = 1.337, 
                             harmony_affinity = 1.337, 
                             texture_affinity = 1.337, 
                             groovyness_affinity = 1.337, 
                             space_affinity = 1.337, 
                             loudness_affinity = 1.337, 
                             key_affinity = 1.337, 
                             channel_suitability_affinity = 1.337, 
+                            arousal_affinity = 1.337, 
+                            pleasantness_affinity = 1.337, 
+                            engagement_affinity = 1.337, 
+                            energy_affinity = 1.337, 
                             language_of_performance = 'en', 
+                            arousal = 'very calm', 
                             dominant_instrument = 'piano', 
                             energy = 'very quiet', 
                             engagement = 'very unengaging', 
                             groovyness = 'very steady', 
                             harmony = 'very dissonant', 
                             pleasantness = 'very unpleasant', 
                             primary_mood_cluster = 'aggressive', 
@@ -93,15 +103,17 @@
                             tonality = 'monotonous', 
                             valence = 'very sad', 
                             vocals = 'instrumental', 
                             origin_decade = 'pre-1950s', 
                             curateability = 'curateable', 
                             use_case = 'background', 
                             channel_suitability = 'Spotify', 
+                            pretzel_station_suitability = 'Afro Beats', 
                             loudness = 'very low', 
+                            bpm = 1.337, 
                             primary_mood_cluster_affinity = 1.337, 
                             secondary_mood_cluster = 'aggressive', 
                             secondary_mood_cluster_affinity = 1.337, 
                             tertiary_mood_cluster = 'aggressive', 
                             tertiary_mood_cluster_affinity = 1.337, 
                             vocals_affinity = 1.337, 
                             dominant_instrument_affinity = 1.337, 
@@ -109,15 +121,14 @@
                             secondary_instrument_affinity = 1.337, 
                             tertiary_instrument = 'piano', 
                             tertiary_instrument_affinity = 1.337, 
                             sound_generation_affinity = 1.337, 
                             rhythm_affinity = 1.337, 
                             primary_sound_character_affinity = 1.337, 
                             tonality_affinity = 1.337, 
-                            bpm = 1.337, 
                             production_rating = 'low production quality', 
                             production_rating_affinity = 1.337, 
                             performance_rating = 'low performance quality', 
                             performance_rating_affinity = 1.337, 
                             song_rating = 'low song quality', 
                             song_rating_affinity = 1.337, 
                             audience_age = 'Generation Z', 
@@ -137,25 +148,16 @@
                             origin_region_affinity = 1.337, 
                             origin_decade_affinity = 1.337, 
                             language_of_performance_affinity = 1.337, 
                             curateability_affinity = 1.337, 
                             use_case_affinity = 1.337, 
                             industry_suitability = 'Automobiles and Parts', 
                             industry_suitability_affinity = 1.337, 
+                            pretzel_station_suitability_affinity = 1.337, 
                             audience_region = 'Australia and New Zealand', ), 
-                        recording_party_entities = [
-                            songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
-                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                    id = '', 
-                                    full_name = '', ), 
-                                contributor_types = [
-                                    songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
-                                        type_name = '', )
-                                    ], )
-                            ], 
                         spotify_id = '', 
                         tags = [
                             songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
                                 tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                                     id = 56, 
                                     name = '', 
                                     categories = [
@@ -183,42 +185,52 @@
                         genres = [
                             songtradr_api_client_python.models.genre_dto.GenreDTO(
                                 id = 56, 
                                 name = '', )
                             ], 
                         language_of_performance = '', 
                         release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        recording_party_entities = [
+                            songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                                    id = '', 
+                                    full_name = '', ), 
+                                contributor_types = [
+                                    songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
+                                        type_name = '', )
+                                    ], )
+                            ], 
                         titles = [
                             songtradr_api_client_python.models.title_dto.TitleDTO(
                                 title_text = '', )
                             ], 
                         tracks = [
                             songtradr_api_client_python.models.track_dto.TrackDTO(
                                 songtradr_track_id = '', )
                             ], 
                         musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                             space = 'very compact', 
-                            arousal = 'very calm', 
                             valence_affinity = 1.337, 
-                            arousal_affinity = 1.337, 
-                            pleasantness_affinity = 1.337, 
-                            engagement_affinity = 1.337, 
-                            energy_affinity = 1.337, 
                             tempo_affinity = 1.337, 
                             scale_affinity = 1.337, 
                             timbre_affinity = 1.337, 
                             roughness_affinity = 1.337, 
                             harmony_affinity = 1.337, 
                             texture_affinity = 1.337, 
                             groovyness_affinity = 1.337, 
                             space_affinity = 1.337, 
                             loudness_affinity = 1.337, 
                             key_affinity = 1.337, 
                             channel_suitability_affinity = 1.337, 
+                            arousal_affinity = 1.337, 
+                            pleasantness_affinity = 1.337, 
+                            engagement_affinity = 1.337, 
+                            energy_affinity = 1.337, 
                             language_of_performance = 'en', 
+                            arousal = 'very calm', 
                             dominant_instrument = 'piano', 
                             energy = 'very quiet', 
                             engagement = 'very unengaging', 
                             groovyness = 'very steady', 
                             harmony = 'very dissonant', 
                             pleasantness = 'very unpleasant', 
                             primary_mood_cluster = 'aggressive', 
@@ -234,15 +246,17 @@
                             tonality = 'monotonous', 
                             valence = 'very sad', 
                             vocals = 'instrumental', 
                             origin_decade = 'pre-1950s', 
                             curateability = 'curateable', 
                             use_case = 'background', 
                             channel_suitability = 'Spotify', 
+                            pretzel_station_suitability = 'Afro Beats', 
                             loudness = 'very low', 
+                            bpm = 1.337, 
                             primary_mood_cluster_affinity = 1.337, 
                             secondary_mood_cluster = 'aggressive', 
                             secondary_mood_cluster_affinity = 1.337, 
                             tertiary_mood_cluster = 'aggressive', 
                             tertiary_mood_cluster_affinity = 1.337, 
                             vocals_affinity = 1.337, 
                             dominant_instrument_affinity = 1.337, 
@@ -250,15 +264,14 @@
                             secondary_instrument_affinity = 1.337, 
                             tertiary_instrument = 'piano', 
                             tertiary_instrument_affinity = 1.337, 
                             sound_generation_affinity = 1.337, 
                             rhythm_affinity = 1.337, 
                             primary_sound_character_affinity = 1.337, 
                             tonality_affinity = 1.337, 
-                            bpm = 1.337, 
                             production_rating = 'low production quality', 
                             production_rating_affinity = 1.337, 
                             performance_rating = 'low performance quality', 
                             performance_rating_affinity = 1.337, 
                             song_rating = 'low song quality', 
                             song_rating_affinity = 1.337, 
                             audience_age = 'Generation Z', 
@@ -278,25 +291,16 @@
                             origin_region_affinity = 1.337, 
                             origin_decade_affinity = 1.337, 
                             language_of_performance_affinity = 1.337, 
                             curateability_affinity = 1.337, 
                             use_case_affinity = 1.337, 
                             industry_suitability = 'Automobiles and Parts', 
                             industry_suitability_affinity = 1.337, 
+                            pretzel_station_suitability_affinity = 1.337, 
                             audience_region = 'Australia and New Zealand', ), 
-                        recording_party_entities = [
-                            songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
-                                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                                    id = '', 
-                                    full_name = '', ), 
-                                contributor_types = [
-                                    songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
-                                        type_name = '', )
-                                    ], )
-                            ], 
                         spotify_id = '', 
                         tags = [
                             songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
                                 tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                                     id = 56, 
                                     name = '', 
                                     categories = [
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_recording_medium_dto.py` & `songtradr_api_client_python-2.1.0/test/test_recording_medium_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -40,42 +40,52 @@
                 genres = [
                     songtradr_api_client_python.models.genre_dto.GenreDTO(
                         id = 56, 
                         name = '', )
                     ],
                 language_of_performance = '',
                 release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                recording_party_entities = [
+                    songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
+                        party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                            id = '', 
+                            full_name = '', ), 
+                        contributor_types = [
+                            songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
+                                type_name = '', )
+                            ], )
+                    ],
                 titles = [
                     songtradr_api_client_python.models.title_dto.TitleDTO(
                         title_text = '', )
                     ],
                 tracks = [
                     songtradr_api_client_python.models.track_dto.TrackDTO(
                         songtradr_track_id = '', )
                     ],
                 musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                     space = 'very compact', 
-                    arousal = 'very calm', 
                     valence_affinity = 1.337, 
-                    arousal_affinity = 1.337, 
-                    pleasantness_affinity = 1.337, 
-                    engagement_affinity = 1.337, 
-                    energy_affinity = 1.337, 
                     tempo_affinity = 1.337, 
                     scale_affinity = 1.337, 
                     timbre_affinity = 1.337, 
                     roughness_affinity = 1.337, 
                     harmony_affinity = 1.337, 
                     texture_affinity = 1.337, 
                     groovyness_affinity = 1.337, 
                     space_affinity = 1.337, 
                     loudness_affinity = 1.337, 
                     key_affinity = 1.337, 
                     channel_suitability_affinity = 1.337, 
+                    arousal_affinity = 1.337, 
+                    pleasantness_affinity = 1.337, 
+                    engagement_affinity = 1.337, 
+                    energy_affinity = 1.337, 
                     language_of_performance = 'en', 
+                    arousal = 'very calm', 
                     dominant_instrument = 'piano', 
                     energy = 'very quiet', 
                     engagement = 'very unengaging', 
                     groovyness = 'very steady', 
                     harmony = 'very dissonant', 
                     pleasantness = 'very unpleasant', 
                     primary_mood_cluster = 'aggressive', 
@@ -91,15 +101,17 @@
                     tonality = 'monotonous', 
                     valence = 'very sad', 
                     vocals = 'instrumental', 
                     origin_decade = 'pre-1950s', 
                     curateability = 'curateable', 
                     use_case = 'background', 
                     channel_suitability = 'Spotify', 
+                    pretzel_station_suitability = 'Afro Beats', 
                     loudness = 'very low', 
+                    bpm = 1.337, 
                     primary_mood_cluster_affinity = 1.337, 
                     secondary_mood_cluster = 'aggressive', 
                     secondary_mood_cluster_affinity = 1.337, 
                     tertiary_mood_cluster = 'aggressive', 
                     tertiary_mood_cluster_affinity = 1.337, 
                     vocals_affinity = 1.337, 
                     dominant_instrument_affinity = 1.337, 
@@ -107,15 +119,14 @@
                     secondary_instrument_affinity = 1.337, 
                     tertiary_instrument = 'piano', 
                     tertiary_instrument_affinity = 1.337, 
                     sound_generation_affinity = 1.337, 
                     rhythm_affinity = 1.337, 
                     primary_sound_character_affinity = 1.337, 
                     tonality_affinity = 1.337, 
-                    bpm = 1.337, 
                     production_rating = 'low production quality', 
                     production_rating_affinity = 1.337, 
                     performance_rating = 'low performance quality', 
                     performance_rating_affinity = 1.337, 
                     song_rating = 'low song quality', 
                     song_rating_affinity = 1.337, 
                     audience_age = 'Generation Z', 
@@ -135,25 +146,16 @@
                     origin_region_affinity = 1.337, 
                     origin_decade_affinity = 1.337, 
                     language_of_performance_affinity = 1.337, 
                     curateability_affinity = 1.337, 
                     use_case_affinity = 1.337, 
                     industry_suitability = 'Automobiles and Parts', 
                     industry_suitability_affinity = 1.337, 
+                    pretzel_station_suitability_affinity = 1.337, 
                     audience_region = 'Australia and New Zealand', ),
-                recording_party_entities = [
-                    songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
-                        party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                            id = '', 
-                            full_name = '', ), 
-                        contributor_types = [
-                            songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
-                                type_name = '', )
-                            ], )
-                    ],
                 spotify_id = '',
                 tags = [
                     songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
                         tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                             id = 56, 
                             name = '', 
                             categories = [
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_recording_minimal_with_musical_features_dto.py` & `songtradr_api_client_python-2.1.0/test/test_recording_minimal_with_musical_features_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -36,32 +36,32 @@
         model = RecordingMinimalWithMusicalFeaturesDTO()
         if include_optional:
             return RecordingMinimalWithMusicalFeaturesDTO(
                 isrc = '',
                 musical_features = [
                     songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                         space = 'very compact', 
-                        arousal = 'very calm', 
                         valence_affinity = 1.337, 
-                        arousal_affinity = 1.337, 
-                        pleasantness_affinity = 1.337, 
-                        engagement_affinity = 1.337, 
-                        energy_affinity = 1.337, 
                         tempo_affinity = 1.337, 
                         scale_affinity = 1.337, 
                         timbre_affinity = 1.337, 
                         roughness_affinity = 1.337, 
                         harmony_affinity = 1.337, 
                         texture_affinity = 1.337, 
                         groovyness_affinity = 1.337, 
                         space_affinity = 1.337, 
                         loudness_affinity = 1.337, 
                         key_affinity = 1.337, 
                         channel_suitability_affinity = 1.337, 
+                        arousal_affinity = 1.337, 
+                        pleasantness_affinity = 1.337, 
+                        engagement_affinity = 1.337, 
+                        energy_affinity = 1.337, 
                         language_of_performance = 'en', 
+                        arousal = 'very calm', 
                         dominant_instrument = 'piano', 
                         energy = 'very quiet', 
                         engagement = 'very unengaging', 
                         groovyness = 'very steady', 
                         harmony = 'very dissonant', 
                         pleasantness = 'very unpleasant', 
                         primary_mood_cluster = 'aggressive', 
@@ -77,15 +77,17 @@
                         tonality = 'monotonous', 
                         valence = 'very sad', 
                         vocals = 'instrumental', 
                         origin_decade = 'pre-1950s', 
                         curateability = 'curateable', 
                         use_case = 'background', 
                         channel_suitability = 'Spotify', 
+                        pretzel_station_suitability = 'Afro Beats', 
                         loudness = 'very low', 
+                        bpm = 1.337, 
                         primary_mood_cluster_affinity = 1.337, 
                         secondary_mood_cluster = 'aggressive', 
                         secondary_mood_cluster_affinity = 1.337, 
                         tertiary_mood_cluster = 'aggressive', 
                         tertiary_mood_cluster_affinity = 1.337, 
                         vocals_affinity = 1.337, 
                         dominant_instrument_affinity = 1.337, 
@@ -93,15 +95,14 @@
                         secondary_instrument_affinity = 1.337, 
                         tertiary_instrument = 'piano', 
                         tertiary_instrument_affinity = 1.337, 
                         sound_generation_affinity = 1.337, 
                         rhythm_affinity = 1.337, 
                         primary_sound_character_affinity = 1.337, 
                         tonality_affinity = 1.337, 
-                        bpm = 1.337, 
                         production_rating = 'low production quality', 
                         production_rating_affinity = 1.337, 
                         performance_rating = 'low performance quality', 
                         performance_rating_affinity = 1.337, 
                         song_rating = 'low song quality', 
                         song_rating_affinity = 1.337, 
                         audience_age = 'Generation Z', 
@@ -121,14 +122,15 @@
                         origin_region_affinity = 1.337, 
                         origin_decade_affinity = 1.337, 
                         language_of_performance_affinity = 1.337, 
                         curateability_affinity = 1.337, 
                         use_case_affinity = 1.337, 
                         industry_suitability = 'Automobiles and Parts', 
                         industry_suitability_affinity = 1.337, 
+                        pretzel_station_suitability_affinity = 1.337, 
                         audience_region = 'Australia and New Zealand', )
                     ]
             )
         else:
             return RecordingMinimalWithMusicalFeaturesDTO(
                 isrc = '',
         )
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_recording_minimal_with_taggrams_dto.py` & `songtradr_api_client_python-2.1.0/test/test_recording_minimal_with_taggrams_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_recording_minimal_with_tagstrengths_dto.py` & `songtradr_api_client_python-2.1.0/test/test_recording_minimal_with_tagstrengths_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_recording_party_dto.py` & `songtradr_api_client_python-2.1.0/test/test_recording_party_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_recording_small_dto.py` & `songtradr_api_client_python-2.1.0/test/test_recording_small_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -34,31 +34,31 @@
         # uncomment below to create an instance of `RecordingSmallDTO`
         """
         model = RecordingSmallDTO()
         if include_optional:
             return RecordingSmallDTO(
                 duration = 56,
                 isrc = '',
-                titles = [
-                    songtradr_api_client_python.models.title_dto.TitleDTO(
-                        title_text = '', )
-                    ],
-                tracks = [
-                    songtradr_api_client_python.models.track_dto.TrackDTO(
-                        songtradr_track_id = '', )
-                    ],
                 parties = [
                     songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                         party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                             id = '', 
                             full_name = '', ), 
                         contributor_types = [
                             songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                 type_name = '', )
                             ], )
+                    ],
+                titles = [
+                    songtradr_api_client_python.models.title_dto.TitleDTO(
+                        title_text = '', )
+                    ],
+                tracks = [
+                    songtradr_api_client_python.models.track_dto.TrackDTO(
+                        songtradr_track_id = '', )
                     ]
             )
         else:
             return RecordingSmallDTO(
                 isrc = '',
         )
         """
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_recording_tag_small_dto.py` & `songtradr_api_client_python-2.1.0/test/test_recording_tag_small_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_save_user_dto.py` & `songtradr_api_client_python-2.1.0/test/test_save_user_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_search_filter_values_dto.py` & `songtradr_api_client_python-2.1.0/test/test_search_filter_values_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -157,14 +157,17 @@
                     ''
                     ],
                 use_case = [
                     ''
                     ],
                 channel_suitability = [
                     ''
+                    ],
+                pretzel_station_suitability = [
+                    ''
                     ]
             )
         else:
             return SearchFilterValuesDTO(
                 primary_mood_cluster = [
                     ''
                     ],
@@ -287,14 +290,17 @@
                     ],
                 use_case = [
                     ''
                     ],
                 channel_suitability = [
                     ''
                     ],
+                pretzel_station_suitability = [
+                    ''
+                    ],
         )
         """
 
     def testSearchFilterValuesDTO(self):
         """Test SearchFilterValuesDTO"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_sign_up_dto.py` & `songtradr_api_client_python-2.1.0/test/test_sign_up_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_tag_dto.py` & `songtradr_api_client_python-2.1.0/test/test_tag_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_tag_small_dto.py` & `songtradr_api_client_python-2.1.0/test/test_tag_small_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_taggram_dto.py` & `songtradr_api_client_python-2.1.0/test/test_taggram_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_tags_summary_dto.py` & `songtradr_api_client_python-2.1.0/test/test_tags_summary_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_tagstrength_dto.py` & `songtradr_api_client_python-2.1.0/test/test_tagstrength_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_title_dto.py` & `songtradr_api_client_python-2.1.0/test/test_title_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_token_request.py` & `songtradr_api_client_python-2.1.0/test/test_token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_track_dto.py` & `songtradr_api_client_python-2.1.0/test/test_track_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_update_password_dto.py` & `songtradr_api_client_python-2.1.0/test/test_update_password_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_user_api.py` & `songtradr_api_client_python-2.1.0/test/test_user_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -100,14 +100,42 @@
     def test_recordings_by_folder_with_tagstrengths(self) -> None:
         """Test case for recordings_by_folder_with_tagstrengths
 
         Strengths as numerical representations for AI generated moods, musical features and more for recordings in your folder.
         """
         pass
 
+    def test_recordings_by_ids_with_similarities(self) -> None:
+        """Test case for recordings_by_ids_with_similarities
+
+        Similar recordings for a list of user recordings.
+        """
+        pass
+
+    def test_recordings_by_ids_with_taggrams(self) -> None:
+        """Test case for recordings_by_ids_with_taggrams
+
+        Timeseries of AI generated moods, musical features and more for a list of recordings.
+        """
+        pass
+
+    def test_recordings_by_ids_with_tagstrengths(self) -> None:
+        """Test case for recordings_by_ids_with_tagstrengths
+
+        Strengths as numerical representations for AI generated moods, musical features and more for recordings.
+        """
+        pass
+
+    def test_recordings_medium_by_ids(self) -> None:
+        """Test case for recordings_medium_by_ids
+
+        Recordings by IDs with a medium sized response.
+        """
+        pass
+
     def test_sign_up(self) -> None:
         """Test case for sign_up
 
         Sign up a new user.
         """
         pass
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_user_dto.py` & `songtradr_api_client_python-2.1.0/test/test_user_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr-api-client-python-2.0.0/test/test_video_recognition_response.py` & `songtradr_api_client_python-2.1.0/test/test_video_recognition_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.1.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

