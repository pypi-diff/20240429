# Comparing `tmp/docusign-maestro-1.0.0.tar.gz` & `tmp/docusign-maestro-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/docusign-maestro-1.0.0.tar", last modified: Mon Apr 29 15:05:08 2024, max compression
+gzip compressed data, was "dist/docusign-maestro-1.0.0rc1.tar", last modified: Wed Apr  3 17:28:58 2024, max compression
```

## Comparing `docusign-maestro-1.0.0.tar` & `docusign-maestro-1.0.0rc1.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:05:08.000000 docusign-maestro-1.0.0/
--rw-r--r--   0 root         (0) root         (0)    13462 2024-04-29 15:05:08.000000 docusign-maestro-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13261 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:05:08.000000 docusign-maestro-1.0.0/docusign_maestro/
--rw-r--r--   0 root         (0) root         (0)    11477 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:05:08.000000 docusign-maestro-1.0.0/docusign_maestro/apis/
--rw-r--r--   0 root         (0) root         (0)      275 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23097 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/apis/workflow_instance_management_api.py
--rw-r--r--   0 root         (0) root         (0)    40216 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/apis/workflow_management_api.py
--rw-r--r--   0 root         (0) root         (0)     6926 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/apis/workflow_trigger_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:05:08.000000 docusign-maestro-1.0.0/docusign_maestro/client/
--rw-r--r--   0 root         (0) root         (0)      696 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35473 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/client/api_client.py
--rw-r--r--   0 root         (0) root         (0)     1884 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/client/api_exception.py
--rw-r--r--   0 root         (0) root         (0)    13591 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/client/api_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:05:08.000000 docusign-maestro-1.0.0/docusign_maestro/client/auth/
--rw-r--r--   0 root         (0) root         (0)      632 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/client/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14856 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/client/auth/oauth.py
--rw-r--r--   0 root         (0) root         (0)     8976 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/client/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:05:08.000000 docusign-maestro-1.0.0/docusign_maestro/models/
--rw-r--r--   0 root         (0) root         (0)    10851 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5331 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/access_token_response.py
--rw-r--r--   0 root         (0) root         (0)     3064 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/access_token_token_types.py
--rw-r--r--   0 root         (0) root         (0)     2883 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/account_id.py
--rw-r--r--   0 root         (0) root         (0)     2873 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/aow_uuid.py
--rw-r--r--   0 root         (0) root         (0)     2903 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/aow_uuid_string.py
--rw-r--r--   0 root         (0) root         (0)     4303 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/cancel_response.py
--rw-r--r--   0 root         (0) root         (0)     4069 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/create_or_update_workflow_definition_request_body.py
--rw-r--r--   0 root         (0) root         (0)     3934 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/deploy_request.py
--rw-r--r--   0 root         (0) root         (0)     5929 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/deploy_response.py
--rw-r--r--   0 root         (0) root         (0)     3015 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/deploy_status.py
--rw-r--r--   0 root         (0) root         (0)     3249 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/deployment_status.py
--rw-r--r--   0 root         (0) root         (0)     7518 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_do_until_step.py
--rw-r--r--   0 root         (0) root         (0)     7780 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_doc_gen_step.py
--rw-r--r--   0 root         (0) root         (0)     9249 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_doc_gen_step_input.py
--rw-r--r--   0 root         (0) root         (0)     7675 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_idv_step.py
--rw-r--r--   0 root         (0) root         (0)     9267 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_idv_step_input.py
--rw-r--r--   0 root         (0) root         (0)     8928 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_if_else_step.py
--rw-r--r--   0 root         (0) root         (0)     7474 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_loop_step.py
--rw-r--r--   0 root         (0) root         (0)     6966 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_parallel_step.py
--rw-r--r--   0 root         (0) root         (0)     2903 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_service_step.py
--rw-r--r--   0 root         (0) root         (0)     7710 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_sign_step.py
--rw-r--r--   0 root         (0) root         (0)     8848 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_sign_step_input.py
--rw-r--r--   0 root         (0) root         (0)     2878 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_step_id.py
--rw-r--r--   0 root         (0) root         (0)    10152 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_transformation_step.py
--rw-r--r--   0 root         (0) root         (0)     8055 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_web_forms_step.py
--rw-r--r--   0 root         (0) root         (0)     3790 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_web_forms_step_config.py
--rw-r--r--   0 root         (0) root         (0)     6368 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_boolean_expression.py
--rw-r--r--   0 root         (0) root         (0)     7727 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_comparison_expression.py
--rw-r--r--   0 root         (0) root         (0)     3416 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_comparison_operator_types.py
--rw-r--r--   0 root         (0) root         (0)     5256 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_concat_expression.py
--rw-r--r--   0 root         (0) root         (0)     3068 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_doc_gen_doc_output_format.py
--rw-r--r--   0 root         (0) root         (0)     3133 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_expression_types_boolean_expression.py
--rw-r--r--   0 root         (0) root         (0)     3154 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_expression_types_comparison_expression.py
--rw-r--r--   0 root         (0) root         (0)     3140 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_expression_types_parallel_expression.py
--rw-r--r--   0 root         (0) root         (0)     6912 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_index_of_expression.py
--rw-r--r--   0 root         (0) root         (0)     5165 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_lane.py
--rw-r--r--   0 root         (0) root         (0)     2943 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_lanes_record.py
--rw-r--r--   0 root         (0) root         (0)     6992 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_last_index_of_expression.py
--rw-r--r--   0 root         (0) root         (0)     3059 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_logical_operator_types.py
--rw-r--r--   0 root         (0) root         (0)     5222 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_parallel_expression.py
--rw-r--r--   0 root         (0) root         (0)     2973 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_participant_record.py
--rw-r--r--   0 root         (0) root         (0)     8351 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_replace_expression.py
--rw-r--r--   0 root         (0) root         (0)     2908 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step.py
--rw-r--r--   0 root         (0) root         (0)     3039 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_do_until.py
--rw-r--r--   0 root         (0) root         (0)     3042 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_ds_doc_gen.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_ds_idv.py
--rw-r--r--   0 root         (0) root         (0)     3042 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_ds_if_else.py
--rw-r--r--   0 root         (0) root         (0)     3028 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_ds_sign.py
--rw-r--r--   0 root         (0) root         (0)     3098 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_ds_transformation.py
--rw-r--r--   0 root         (0) root         (0)     3056 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_ds_web_forms.py
--rw-r--r--   0 root         (0) root         (0)     3018 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_loop.py
--rw-r--r--   0 root         (0) root         (0)     3046 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_parallel.py
--rw-r--r--   0 root         (0) root         (0)     7909 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_substring_expression.py
--rw-r--r--   0 root         (0) root         (0)     5353 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_to_lower_expression.py
--rw-r--r--   0 root         (0) root         (0)     5353 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_to_upper_expression.py
--rw-r--r--   0 root         (0) root         (0)     3008 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression.py
--rw-r--r--   0 root         (0) root         (0)     3196 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression_types_concat_expression.py
--rw-r--r--   0 root         (0) root         (0)     3203 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression_types_index_of_expression.py
--rw-r--r--   0 root         (0) root         (0)     3231 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression_types_last_index_of_expression.py
--rw-r--r--   0 root         (0) root         (0)     3203 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression_types_replace_expression.py
--rw-r--r--   0 root         (0) root         (0)     3217 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression_types_substring_expression.py
--rw-r--r--   0 root         (0) root         (0)     3203 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression_types_to_lower_expression.py
--rw-r--r--   0 root         (0) root         (0)     3203 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression_types_to_upper_expression.py
--rw-r--r--   0 root         (0) root         (0)     8701 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_trigger.py
--rw-r--r--   0 root         (0) root         (0)     3033 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_trigger_types.py
--rw-r--r--   0 root         (0) root         (0)     2928 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable.py
--rw-r--r--   0 root         (0) root         (0)     3003 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable_from_participant.py
--rw-r--r--   0 root         (0) root         (0)     6504 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable_from_step.py
--rw-r--r--   0 root         (0) root         (0)     6600 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable_from_variable.py
--rw-r--r--   0 root         (0) root         (0)     2958 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable_record.py
--rw-r--r--   0 root         (0) root         (0)     3111 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable_source_types_participant.py
--rw-r--r--   0 root         (0) root         (0)     3062 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable_source_types_step.py
--rw-r--r--   0 root         (0) root         (0)     3090 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable_source_types_variable.py
--rw-r--r--   0 root         (0) root         (0)     7506 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/e_sign_document_from_e_sign_template.py
--rw-r--r--   0 root         (0) root         (0)     7862 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/e_sign_document_from_previous_step.py
--rw-r--r--   0 root         (0) root         (0)     3077 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/e_sign_document_types_from_ds_template.py
--rw-r--r--   0 root         (0) root         (0)     3091 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/e_sign_document_types_from_previous_step.py
--rw-r--r--   0 root         (0) root         (0)     2908 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/e_sign_documents.py
--rw-r--r--   0 root         (0) root         (0)     2923 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/e_sign_locale_policy.py
--rw-r--r--   0 root         (0) root         (0)     8769 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/e_sign_signer.py
--rw-r--r--   0 root         (0) root         (0)    20733 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/e_sign_tabs.py
--rw-r--r--   0 root         (0) root         (0)     8578 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/e_sign_tabs_record.py
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/error_codes.py
--rw-r--r--   0 root         (0) root         (0)     4249 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/error_response.py
--rw-r--r--   0 root         (0) root         (0)     3579 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/event_types.py
--rw-r--r--   0 root         (0) root         (0)     5499 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/get_configuration_instance_response.py
--rw-r--r--   0 root         (0) root         (0)     5703 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/get_configuration_instances_response.py
--rw-r--r--   0 root         (0) root         (0)     4727 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/get_configuration_instances_response_config_instances.py
--rw-r--r--   0 root         (0) root         (0)     2996 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/http_types.py
--rw-r--r--   0 root         (0) root         (0)     4899 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/invalid_workflow_response.py
--rw-r--r--   0 root         (0) root         (0)     2908 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/last_deployed_id.py
--rw-r--r--   0 root         (0) root         (0)     7906 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/new_or_updated_workflow_definition_response.py
--rw-r--r--   0 root         (0) root         (0)     2918 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/number_or_variable.py
--rw-r--r--   0 root         (0) root         (0)     7035 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/participant.py
--rw-r--r--   0 root         (0) root         (0)     3094 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/participant_keys.py
--rw-r--r--   0 root         (0) root         (0)     5855 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/progress_instance.py
--rw-r--r--   0 root         (0) root         (0)     2933 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/record_string_boolean.py
--rw-r--r--   0 root         (0) root         (0)     3028 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/record_string_or_variable_or_transformation.py
--rw-r--r--   0 root         (0) root         (0)     2903 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/record_to_never.py
--rw-r--r--   0 root         (0) root         (0)     3542 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/replication_status.py
--rw-r--r--   0 root         (0) root         (0)     5835 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/started_by_instance.py
--rw-r--r--   0 root         (0) root         (0)     2998 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/string_or_variable_or_transformation.py
--rw-r--r--   0 root         (0) root         (0)     3620 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/success_message_response.py
--rw-r--r--   0 root         (0) root         (0)     2888 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/template_id.py
--rw-r--r--   0 root         (0) root         (0)     5710 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/trigger_payload.py
--rw-r--r--   0 root         (0) root         (0)     4919 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/trigger_workflow_via_post_response.py
--rw-r--r--   0 root         (0) root         (0)     2868 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/user_id.py
--rw-r--r--   0 root         (0) root         (0)     4492 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/validation_errors.py
--rw-r--r--   0 root         (0) root         (0)     2903 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/version_string.py
--rw-r--r--   0 root         (0) root         (0)     2923 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_creator_id.py
--rw-r--r--   0 root         (0) root         (0)     2918 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_date_time.py
--rw-r--r--   0 root         (0) root         (0)    12923 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_definition.py
--rw-r--r--   0 root         (0) root         (0)     4551 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_definition_list.py
--rw-r--r--   0 root         (0) root         (0)    10987 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_definition_metadata.py
--rw-r--r--   0 root         (0) root         (0)    13317 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_definition_with_id.py
--rw-r--r--   0 root         (0) root         (0)     4947 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_delete_response.py
--rw-r--r--   0 root         (0) root         (0)    12160 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_instance.py
--rw-r--r--   0 root         (0) root         (0)     2928 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_instance_id.py
--rw-r--r--   0 root         (0) root         (0)     2933 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_instance_map.py
--rw-r--r--   0 root         (0) root         (0)     3116 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_instance_state.py
--rw-r--r--   0 root         (0) root         (0)     2943 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_instances_list.py
--rw-r--r--   0 root         (0) root         (0)     3155 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_metadata_status.py
--rw-r--r--   0 root         (0) root         (0)     6680 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_step_error.py
--rw-r--r--   0 root         (0) root         (0)     4452 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_step_error_error.py
--rw-r--r--   0 root         (0) root         (0)    12061 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_step_history.py
--rw-r--r--   0 root         (0) root         (0)     2953 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_step_history_list.py
--rw-r--r--   0 root         (0) root         (0)     3107 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/docusign_maestro/models/workflow_step_history_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:05:08.000000 docusign-maestro-1.0.0/docusign_maestro.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13462 2024-04-29 15:05:07.000000 docusign-maestro-1.0.0/docusign_maestro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7703 2024-04-29 15:05:08.000000 docusign-maestro-1.0.0/docusign_maestro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 15:05:07.000000 docusign-maestro-1.0.0/docusign_maestro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      128 2024-04-29 15:05:08.000000 docusign-maestro-1.0.0/docusign_maestro.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-29 15:05:08.000000 docusign-maestro-1.0.0/docusign_maestro.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 15:05:08.000000 docusign-maestro-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1725 2024-04-29 15:05:03.000000 docusign-maestro-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:28:58.000000 docusign-maestro-1.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    13610 2024-04-03 17:28:58.000000 docusign-maestro-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13406 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:28:58.000000 docusign-maestro-1.0.0rc1/docusign_maestro/
+-rw-r--r--   0 root         (0) root         (0)    11669 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:28:58.000000 docusign-maestro-1.0.0rc1/docusign_maestro/apis/
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23097 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/apis/workflow_instance_management_api.py
+-rw-r--r--   0 root         (0) root         (0)    40216 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/apis/workflow_management_api.py
+-rw-r--r--   0 root         (0) root         (0)     6926 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/apis/workflow_trigger_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:28:58.000000 docusign-maestro-1.0.0rc1/docusign_maestro/client/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35473 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/client/api_client.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/client/api_exception.py
+-rw-r--r--   0 root         (0) root         (0)    13591 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/client/api_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:28:58.000000 docusign-maestro-1.0.0rc1/docusign_maestro/client/auth/
+-rw-r--r--   0 root         (0) root         (0)      632 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/client/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14856 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/client/auth/oauth.py
+-rw-r--r--   0 root         (0) root         (0)     8985 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/client/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:28:58.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/
+-rw-r--r--   0 root         (0) root         (0)    11043 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/access_token_response.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/access_token_token_types.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/account_id.py
+-rw-r--r--   0 root         (0) root         (0)     2873 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/aow_uuid.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/aow_uuid_string.py
+-rw-r--r--   0 root         (0) root         (0)     4303 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/cancel_response.py
+-rw-r--r--   0 root         (0) root         (0)     4069 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/create_or_update_workflow_definition_request_body.py
+-rw-r--r--   0 root         (0) root         (0)     3934 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/deploy_request.py
+-rw-r--r--   0 root         (0) root         (0)     5929 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/deploy_response.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/deploy_status.py
+-rw-r--r--   0 root         (0) root         (0)     3165 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)     7518 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_do_until_step.py
+-rw-r--r--   0 root         (0) root         (0)     7780 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_doc_gen_step.py
+-rw-r--r--   0 root         (0) root         (0)     9249 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_doc_gen_step_input.py
+-rw-r--r--   0 root         (0) root         (0)     7675 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_idv_step.py
+-rw-r--r--   0 root         (0) root         (0)     9267 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_idv_step_input.py
+-rw-r--r--   0 root         (0) root         (0)     8928 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_if_else_step.py
+-rw-r--r--   0 root         (0) root         (0)     7474 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_loop_step.py
+-rw-r--r--   0 root         (0) root         (0)     6966 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_parallel_step.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_service_step.py
+-rw-r--r--   0 root         (0) root         (0)     7710 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_sign_step.py
+-rw-r--r--   0 root         (0) root         (0)     8848 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_sign_step_input.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_step_id.py
+-rw-r--r--   0 root         (0) root         (0)    10152 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_transformation_step.py
+-rw-r--r--   0 root         (0) root         (0)     8055 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_web_forms_step.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_web_forms_step_config.py
+-rw-r--r--   0 root         (0) root         (0)     6368 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_boolean_expression.py
+-rw-r--r--   0 root         (0) root         (0)     7727 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_comparison_expression.py
+-rw-r--r--   0 root         (0) root         (0)     3416 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_comparison_operator_types.py
+-rw-r--r--   0 root         (0) root         (0)     5256 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_concat_expression.py
+-rw-r--r--   0 root         (0) root         (0)     3068 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_doc_gen_doc_output_format.py
+-rw-r--r--   0 root         (0) root         (0)     3133 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_expression_types_boolean_expression.py
+-rw-r--r--   0 root         (0) root         (0)     3154 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_expression_types_comparison_expression.py
+-rw-r--r--   0 root         (0) root         (0)     3140 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_expression_types_parallel_expression.py
+-rw-r--r--   0 root         (0) root         (0)     6912 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_index_of_expression.py
+-rw-r--r--   0 root         (0) root         (0)     5165 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_lane.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_lanes_record.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_last_index_of_expression.py
+-rw-r--r--   0 root         (0) root         (0)     3059 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_logical_operator_types.py
+-rw-r--r--   0 root         (0) root         (0)     5222 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_parallel_expression.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_participant_record.py
+-rw-r--r--   0 root         (0) root         (0)     8351 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_replace_expression.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_do_until.py
+-rw-r--r--   0 root         (0) root         (0)     3042 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_ds_doc_gen.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_ds_idv.py
+-rw-r--r--   0 root         (0) root         (0)     3042 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_ds_if_else.py
+-rw-r--r--   0 root         (0) root         (0)     3028 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_ds_sign.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_ds_transformation.py
+-rw-r--r--   0 root         (0) root         (0)     3056 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_ds_web_forms.py
+-rw-r--r--   0 root         (0) root         (0)     3018 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_loop.py
+-rw-r--r--   0 root         (0) root         (0)     3046 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_parallel.py
+-rw-r--r--   0 root         (0) root         (0)     7909 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_substring_expression.py
+-rw-r--r--   0 root         (0) root         (0)     5353 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_to_lower_expression.py
+-rw-r--r--   0 root         (0) root         (0)     5353 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_to_upper_expression.py
+-rw-r--r--   0 root         (0) root         (0)     3008 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression_types_concat_expression.py
+-rw-r--r--   0 root         (0) root         (0)     3203 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression_types_index_of_expression.py
+-rw-r--r--   0 root         (0) root         (0)     3231 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression_types_last_index_of_expression.py
+-rw-r--r--   0 root         (0) root         (0)     3203 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression_types_replace_expression.py
+-rw-r--r--   0 root         (0) root         (0)     3217 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression_types_substring_expression.py
+-rw-r--r--   0 root         (0) root         (0)     3203 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression_types_to_lower_expression.py
+-rw-r--r--   0 root         (0) root         (0)     3203 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression_types_to_upper_expression.py
+-rw-r--r--   0 root         (0) root         (0)     8701 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_trigger.py
+-rw-r--r--   0 root         (0) root         (0)     3033 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_trigger_types.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_variable.py
+-rw-r--r--   0 root         (0) root         (0)     5844 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_variable_from_participant.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_variable_from_step.py
+-rw-r--r--   0 root         (0) root         (0)     6600 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_variable_from_variable.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_variable_record.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_variable_source_types_participant.py
+-rw-r--r--   0 root         (0) root         (0)     3062 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_variable_source_types_step.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_variable_source_types_variable.py
+-rw-r--r--   0 root         (0) root         (0)     7506 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_document_from_e_sign_template.py
+-rw-r--r--   0 root         (0) root         (0)     7862 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_document_from_previous_step.py
+-rw-r--r--   0 root         (0) root         (0)     3077 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_document_types_from_ds_template.py
+-rw-r--r--   0 root         (0) root         (0)     3091 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_document_types_from_previous_step.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_documents.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_locale_policy.py
+-rw-r--r--   0 root         (0) root         (0)     8769 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_signer.py
+-rw-r--r--   0 root         (0) root         (0)    20733 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_tabs.py
+-rw-r--r--   0 root         (0) root         (0)     8578 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_tabs_record.py
+-rw-r--r--   0 root         (0) root         (0)     3354 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/error_codes.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/error_response.py
+-rw-r--r--   0 root         (0) root         (0)     3025 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/event_types.py
+-rw-r--r--   0 root         (0) root         (0)     5499 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/get_configuration_instance_response.py
+-rw-r--r--   0 root         (0) root         (0)     5703 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/get_configuration_instances_response.py
+-rw-r--r--   0 root         (0) root         (0)     4727 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/get_configuration_instances_response_config_instances.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/http_types.py
+-rw-r--r--   0 root         (0) root         (0)     4899 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/invalid_workflow_response.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/last_deployed_id.py
+-rw-r--r--   0 root         (0) root         (0)     7906 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/new_or_updated_workflow_definition_response.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/number_or_variable.py
+-rw-r--r--   0 root         (0) root         (0)     7035 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/participant.py
+-rw-r--r--   0 root         (0) root         (0)     3094 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/participant_keys.py
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/progress_instance.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/record_string_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     3028 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/record_string_or_variable_or_transformation.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/record_to_never.py
+-rw-r--r--   0 root         (0) root         (0)     3542 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/replication_status.py
+-rw-r--r--   0 root         (0) root         (0)     5821 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/started_by_instance.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/string_or_variable_or_transformation.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/success_message_response.py
+-rw-r--r--   0 root         (0) root         (0)     2888 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/template_id.py
+-rw-r--r--   0 root         (0) root         (0)     5710 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/trigger_payload.py
+-rw-r--r--   0 root         (0) root         (0)     4919 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/trigger_workflow_via_post_response.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/user_id.py
+-rw-r--r--   0 root         (0) root         (0)     4492 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/validation_errors.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/version_string.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_creator_id.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_date_time.py
+-rw-r--r--   0 root         (0) root         (0)    12923 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_definition.py
+-rw-r--r--   0 root         (0) root         (0)     4551 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_definition_list.py
+-rw-r--r--   0 root         (0) root         (0)    10987 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_definition_metadata.py
+-rw-r--r--   0 root         (0) root         (0)    13317 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_definition_with_id.py
+-rw-r--r--   0 root         (0) root         (0)     4947 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_delete_response.py
+-rw-r--r--   0 root         (0) root         (0)    12026 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_instance.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_instance_id.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_instance_map.py
+-rw-r--r--   0 root         (0) root         (0)     3066 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_instance_state.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_instances_list.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_metadata_status.py
+-rw-r--r--   0 root         (0) root         (0)     6680 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_step_error.py
+-rw-r--r--   0 root         (0) root         (0)     4452 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_step_error_error.py
+-rw-r--r--   0 root         (0) root         (0)    12061 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_step_history.py
+-rw-r--r--   0 root         (0) root         (0)     2953 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_step_history_list.py
+-rw-r--r--   0 root         (0) root         (0)     3081 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_step_history_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:28:58.000000 docusign-maestro-1.0.0rc1/docusign_maestro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13610 2024-04-03 17:28:58.000000 docusign-maestro-1.0.0rc1/docusign_maestro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7703 2024-04-03 17:28:58.000000 docusign-maestro-1.0.0rc1/docusign_maestro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 17:28:58.000000 docusign-maestro-1.0.0rc1/docusign_maestro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      128 2024-04-03 17:28:58.000000 docusign-maestro-1.0.0rc1/docusign_maestro.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-03 17:28:58.000000 docusign-maestro-1.0.0rc1/docusign_maestro.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 17:28:58.000000 docusign-maestro-1.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1728 2024-04-03 17:28:55.000000 docusign-maestro-1.0.0rc1/setup.py
```

### Comparing `docusign-maestro-1.0.0/PKG-INFO` & `docusign-maestro-1.0.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,14 @@
-Metadata-Version: 2.1
-Name: docusign-maestro
-Version: 1.0.0
-Summary: Maestro API
-Home-page: 
-Author-email: devcenter@docusign.com
-Keywords: Swagger,Maestro API
-Description-Content-Type: text/markdown
-
 # docusign-maestro
 Maestro authors and executes experiences that allow non-coders the ability to define Simple Business Process without having to write code and to deploy them seamlessly without having to have development expertise
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0.0
-- Package version: 1.0.0
+- Package version: 1.0.0rc1
 - Build package: io.swagger.codegen.languages.PythonClientCodegen
 For more information, please visit [https://developers.docusign.com/](https://developers.docusign.com/)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -159,14 +150,15 @@
  - [DSWorkflowTrigger](docs/DSWorkflowTrigger.md)
  - [DSWorkflowTriggerTypes](docs/DSWorkflowTriggerTypes.md)
  - [DSWorkflowVariable](docs/DSWorkflowVariable.md)
  - [DSWorkflowVariableFromParticipant](docs/DSWorkflowVariableFromParticipant.md)
  - [DSWorkflowVariableFromStep](docs/DSWorkflowVariableFromStep.md)
  - [DSWorkflowVariableFromVariable](docs/DSWorkflowVariableFromVariable.md)
  - [DSWorkflowVariableRecord](docs/DSWorkflowVariableRecord.md)
+ - [DSWorkflowVariableSourceTypesParticipant](docs/DSWorkflowVariableSourceTypesParticipant.md)
  - [DSWorkflowVariableSourceTypesStep](docs/DSWorkflowVariableSourceTypesStep.md)
  - [DSWorkflowVariableSourceTypesVariable](docs/DSWorkflowVariableSourceTypesVariable.md)
  - [DeployRequest](docs/DeployRequest.md)
  - [DeployResponse](docs/DeployResponse.md)
  - [DeployStatus](docs/DeployStatus.md)
  - [DeploymentStatus](docs/DeploymentStatus.md)
  - [ESignDocumentFromESignTemplate](docs/ESignDocumentFromESignTemplate.md)
@@ -185,14 +177,15 @@
  - [GetConfigurationInstancesResponse](docs/GetConfigurationInstancesResponse.md)
  - [GetConfigurationInstancesResponseConfigInstances](docs/GetConfigurationInstancesResponseConfigInstances.md)
  - [HttpTypes](docs/HttpTypes.md)
  - [InvalidWorkflowResponse](docs/InvalidWorkflowResponse.md)
  - [NewOrUpdatedWorkflowDefinitionResponse](docs/NewOrUpdatedWorkflowDefinitionResponse.md)
  - [NumberOrVariable](docs/NumberOrVariable.md)
  - [Participant](docs/Participant.md)
+ - [ParticipantKeys](docs/ParticipantKeys.md)
  - [ProgressInstance](docs/ProgressInstance.md)
  - [RecordStringBoolean](docs/RecordStringBoolean.md)
  - [RecordStringOrVariableOrTransformation](docs/RecordStringOrVariableOrTransformation.md)
  - [RecordToNever](docs/RecordToNever.md)
  - [ReplicationStatus](docs/ReplicationStatus.md)
  - [StartedByInstance](docs/StartedByInstance.md)
  - [StringOrVariableOrTransformation](docs/StringOrVariableOrTransformation.md)
```

### Comparing `docusign-maestro-1.0.0/README.md` & `docusign-maestro-1.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,23 @@
+Metadata-Version: 2.1
+Name: docusign-maestro
+Version: 1.0.0rc1
+Summary: Maestro API
+Home-page: 
+Author-email: devcenter@docusign.com
+Keywords: Swagger,Maestro API
+Description-Content-Type: text/markdown
+
 # docusign-maestro
 Maestro authors and executes experiences that allow non-coders the ability to define Simple Business Process without having to write code and to deploy them seamlessly without having to have development expertise
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0.0
-- Package version: 1.0.0
+- Package version: 1.0.0rc1
 - Build package: io.swagger.codegen.languages.PythonClientCodegen
 For more information, please visit [https://developers.docusign.com/](https://developers.docusign.com/)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -150,14 +159,15 @@
  - [DSWorkflowTrigger](docs/DSWorkflowTrigger.md)
  - [DSWorkflowTriggerTypes](docs/DSWorkflowTriggerTypes.md)
  - [DSWorkflowVariable](docs/DSWorkflowVariable.md)
  - [DSWorkflowVariableFromParticipant](docs/DSWorkflowVariableFromParticipant.md)
  - [DSWorkflowVariableFromStep](docs/DSWorkflowVariableFromStep.md)
  - [DSWorkflowVariableFromVariable](docs/DSWorkflowVariableFromVariable.md)
  - [DSWorkflowVariableRecord](docs/DSWorkflowVariableRecord.md)
+ - [DSWorkflowVariableSourceTypesParticipant](docs/DSWorkflowVariableSourceTypesParticipant.md)
  - [DSWorkflowVariableSourceTypesStep](docs/DSWorkflowVariableSourceTypesStep.md)
  - [DSWorkflowVariableSourceTypesVariable](docs/DSWorkflowVariableSourceTypesVariable.md)
  - [DeployRequest](docs/DeployRequest.md)
  - [DeployResponse](docs/DeployResponse.md)
  - [DeployStatus](docs/DeployStatus.md)
  - [DeploymentStatus](docs/DeploymentStatus.md)
  - [ESignDocumentFromESignTemplate](docs/ESignDocumentFromESignTemplate.md)
@@ -176,14 +186,15 @@
  - [GetConfigurationInstancesResponse](docs/GetConfigurationInstancesResponse.md)
  - [GetConfigurationInstancesResponseConfigInstances](docs/GetConfigurationInstancesResponseConfigInstances.md)
  - [HttpTypes](docs/HttpTypes.md)
  - [InvalidWorkflowResponse](docs/InvalidWorkflowResponse.md)
  - [NewOrUpdatedWorkflowDefinitionResponse](docs/NewOrUpdatedWorkflowDefinitionResponse.md)
  - [NumberOrVariable](docs/NumberOrVariable.md)
  - [Participant](docs/Participant.md)
+ - [ParticipantKeys](docs/ParticipantKeys.md)
  - [ProgressInstance](docs/ProgressInstance.md)
  - [RecordStringBoolean](docs/RecordStringBoolean.md)
  - [RecordStringOrVariableOrTransformation](docs/RecordStringOrVariableOrTransformation.md)
  - [RecordToNever](docs/RecordToNever.md)
  - [ReplicationStatus](docs/ReplicationStatus.md)
  - [StartedByInstance](docs/StartedByInstance.md)
  - [StringOrVariableOrTransformation](docs/StringOrVariableOrTransformation.md)
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/__init__.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 from docusign_maestro.models.ds_workflow_trigger import DSWorkflowTrigger
 from docusign_maestro.models.ds_workflow_trigger_types import DSWorkflowTriggerTypes
 from docusign_maestro.models.ds_workflow_variable import DSWorkflowVariable
 from docusign_maestro.models.ds_workflow_variable_from_participant import DSWorkflowVariableFromParticipant
 from docusign_maestro.models.ds_workflow_variable_from_step import DSWorkflowVariableFromStep
 from docusign_maestro.models.ds_workflow_variable_from_variable import DSWorkflowVariableFromVariable
 from docusign_maestro.models.ds_workflow_variable_record import DSWorkflowVariableRecord
+from docusign_maestro.models.ds_workflow_variable_source_types_participant import DSWorkflowVariableSourceTypesParticipant
 from docusign_maestro.models.ds_workflow_variable_source_types_step import DSWorkflowVariableSourceTypesStep
 from docusign_maestro.models.ds_workflow_variable_source_types_variable import DSWorkflowVariableSourceTypesVariable
 from docusign_maestro.models.deploy_request import DeployRequest
 from docusign_maestro.models.deploy_response import DeployResponse
 from docusign_maestro.models.deploy_status import DeployStatus
 from docusign_maestro.models.deployment_status import DeploymentStatus
 from docusign_maestro.models.e_sign_document_from_e_sign_template import ESignDocumentFromESignTemplate
@@ -116,14 +117,15 @@
 from docusign_maestro.models.get_configuration_instances_response import GetConfigurationInstancesResponse
 from docusign_maestro.models.get_configuration_instances_response_config_instances import GetConfigurationInstancesResponseConfigInstances
 from docusign_maestro.models.http_types import HttpTypes
 from docusign_maestro.models.invalid_workflow_response import InvalidWorkflowResponse
 from docusign_maestro.models.new_or_updated_workflow_definition_response import NewOrUpdatedWorkflowDefinitionResponse
 from docusign_maestro.models.number_or_variable import NumberOrVariable
 from docusign_maestro.models.participant import Participant
+from docusign_maestro.models.participant_keys import ParticipantKeys
 from docusign_maestro.models.progress_instance import ProgressInstance
 from docusign_maestro.models.record_string_boolean import RecordStringBoolean
 from docusign_maestro.models.record_string_or_variable_or_transformation import RecordStringOrVariableOrTransformation
 from docusign_maestro.models.record_to_never import RecordToNever
 from docusign_maestro.models.replication_status import ReplicationStatus
 from docusign_maestro.models.started_by_instance import StartedByInstance
 from docusign_maestro.models.string_or_variable_or_transformation import StringOrVariableOrTransformation
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/apis/workflow_instance_management_api.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/apis/workflow_instance_management_api.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/apis/workflow_management_api.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/apis/workflow_management_api.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/apis/workflow_trigger_api.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/apis/workflow_trigger_api.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/client/__init__.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/client/__init__.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/client/api_client.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/client/api_client.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/client/api_exception.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/client/api_exception.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/client/api_response.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/client/api_response.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/client/auth/__init__.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/client/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/client/auth/oauth.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/client/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/client/configuration.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,17 +115,17 @@
 
         # Disable client side validation
         self.client_side_validation = True
 
         python_version = platform.python_version()
 
         if six.PY3:
-            self.user_agent = "Swagger-Codegen/1.0.0/1.0.0/python3/" + f"{python_version}"
+            self.user_agent = "Swagger-Codegen/1.0.0/1.0.0rc1/python3/" + f"{python_version}"
         else:
-            self.user_agent = "Swagger-Codegen/1.0.0/1.0.0/python2/" + f"{python_version}"
+            self.user_agent = "Swagger-Codegen/1.0.0/1.0.0rc1/python2/" + f"{python_version}"
 
 
     @classmethod
     def set_default(cls, default):
         cls._default = default
 
     @property
@@ -273,9 +273,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.0.0".\
+               "SDK Package Version: 1.0.0rc1".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/__init__.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 from docusign_maestro.models.ds_workflow_trigger import DSWorkflowTrigger
 from docusign_maestro.models.ds_workflow_trigger_types import DSWorkflowTriggerTypes
 from docusign_maestro.models.ds_workflow_variable import DSWorkflowVariable
 from docusign_maestro.models.ds_workflow_variable_from_participant import DSWorkflowVariableFromParticipant
 from docusign_maestro.models.ds_workflow_variable_from_step import DSWorkflowVariableFromStep
 from docusign_maestro.models.ds_workflow_variable_from_variable import DSWorkflowVariableFromVariable
 from docusign_maestro.models.ds_workflow_variable_record import DSWorkflowVariableRecord
+from docusign_maestro.models.ds_workflow_variable_source_types_participant import DSWorkflowVariableSourceTypesParticipant
 from docusign_maestro.models.ds_workflow_variable_source_types_step import DSWorkflowVariableSourceTypesStep
 from docusign_maestro.models.ds_workflow_variable_source_types_variable import DSWorkflowVariableSourceTypesVariable
 from docusign_maestro.models.deploy_request import DeployRequest
 from docusign_maestro.models.deploy_response import DeployResponse
 from docusign_maestro.models.deploy_status import DeployStatus
 from docusign_maestro.models.deployment_status import DeploymentStatus
 from docusign_maestro.models.e_sign_document_from_e_sign_template import ESignDocumentFromESignTemplate
@@ -99,14 +100,15 @@
 from docusign_maestro.models.get_configuration_instances_response import GetConfigurationInstancesResponse
 from docusign_maestro.models.get_configuration_instances_response_config_instances import GetConfigurationInstancesResponseConfigInstances
 from docusign_maestro.models.http_types import HttpTypes
 from docusign_maestro.models.invalid_workflow_response import InvalidWorkflowResponse
 from docusign_maestro.models.new_or_updated_workflow_definition_response import NewOrUpdatedWorkflowDefinitionResponse
 from docusign_maestro.models.number_or_variable import NumberOrVariable
 from docusign_maestro.models.participant import Participant
+from docusign_maestro.models.participant_keys import ParticipantKeys
 from docusign_maestro.models.progress_instance import ProgressInstance
 from docusign_maestro.models.record_string_boolean import RecordStringBoolean
 from docusign_maestro.models.record_string_or_variable_or_transformation import RecordStringOrVariableOrTransformation
 from docusign_maestro.models.record_to_never import RecordToNever
 from docusign_maestro.models.replication_status import ReplicationStatus
 from docusign_maestro.models.started_by_instance import StartedByInstance
 from docusign_maestro.models.string_or_variable_or_transformation import StringOrVariableOrTransformation
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/access_token_response.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/access_token_response.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/access_token_token_types.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/access_token_token_types.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/account_id.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/account_id.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/aow_uuid.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/aow_uuid.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/aow_uuid_string.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/aow_uuid_string.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/cancel_response.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/cancel_response.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/create_or_update_workflow_definition_request_body.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/create_or_update_workflow_definition_request_body.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/deploy_request.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/deploy_request.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/deploy_response.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/deploy_response.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/deploy_status.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/deploy_status.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/deployment_status.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/deployment_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,14 @@
     """
     DEPLOYMENT_IN_PROGRESS = "Deployment In Progress"
     DEPLOYED = "Deployed"
     FAILED = "Failed"
     DELETE_IN_PROGRESS = "Delete in Progress"
     DELETED = "Deleted"
     NOT_DEPLOYED = "Not Deployed"
-    UNPUBLISH_IN_PROGRESS = "Unpublish in Progress"
-    UNPUBLISHED = "Unpublished"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_do_until_step.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_do_until_step.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_doc_gen_step.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_doc_gen_step.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_doc_gen_step_input.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_doc_gen_step_input.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_idv_step.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_idv_step.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_idv_step_input.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_idv_step_input.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_if_else_step.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_if_else_step.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_loop_step.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_loop_step.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_parallel_step.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_parallel_step.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_service_step.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_service_step.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_sign_step.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_sign_step.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_sign_step_input.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_sign_step_input.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_step_id.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_step_id.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_transformation_step.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_transformation_step.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_web_forms_step.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_web_forms_step.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_web_forms_step_config.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_web_forms_step_config.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_boolean_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_boolean_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_comparison_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_comparison_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_comparison_operator_types.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_comparison_operator_types.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_concat_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_concat_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_doc_gen_doc_output_format.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_doc_gen_doc_output_format.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_expression_types_boolean_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_expression_types_boolean_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_expression_types_comparison_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_expression_types_comparison_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_expression_types_parallel_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_expression_types_parallel_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_index_of_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_index_of_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_lane.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_lane.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_lanes_record.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_lanes_record.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_last_index_of_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_last_index_of_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_logical_operator_types.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_logical_operator_types.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_parallel_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_parallel_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_participant_record.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_participant_record.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_replace_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_replace_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_do_until.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_do_until.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_ds_doc_gen.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_ds_doc_gen.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_ds_idv.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_ds_idv.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_ds_if_else.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_ds_if_else.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_ds_sign.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_ds_sign.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_ds_transformation.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_ds_transformation.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_ds_web_forms.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_ds_web_forms.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_loop.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_loop.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_step_types_parallel.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_step_types_parallel.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_substring_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_substring_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_to_lower_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_to_lower_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_to_upper_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_to_upper_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression_types_concat_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression_types_concat_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression_types_index_of_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression_types_index_of_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression_types_last_index_of_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression_types_last_index_of_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression_types_replace_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression_types_replace_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression_types_substring_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression_types_substring_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression_types_to_lower_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression_types_to_lower_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_transformation_expression_types_to_upper_expression.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_transformation_expression_types_to_upper_expression.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_trigger.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_trigger.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_trigger_types.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_trigger_types.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_variable.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable_from_participant.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/http_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,35 +15,43 @@
 import re  # noqa: F401
 
 import six
 
 from docusign_maestro.client.configuration import Configuration
 
 
-class DSWorkflowVariableFromParticipant(object):
+class HttpTypes(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
+    allowed enum values
+    """
+    GET = "Get"
+    POST = "Post"
+    PUT = "Put"
+    DELETE = "Delete"
+
+    """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None, **kwargs):  # noqa: E501
-        """DSWorkflowVariableFromParticipant - a model defined in Swagger"""  # noqa: E501
+        """HttpTypes - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -62,15 +70,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(DSWorkflowVariableFromParticipant, dict):
+        if issubclass(HttpTypes, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,18 +86,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DSWorkflowVariableFromParticipant):
+        if not isinstance(other, HttpTypes):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, DSWorkflowVariableFromParticipant):
+        if not isinstance(other, HttpTypes):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable_from_step.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_variable_from_step.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable_from_variable.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_variable_from_variable.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable_record.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_variable_record.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable_source_types_participant.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_variable_source_types_participant.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable_source_types_step.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_variable_source_types_step.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/ds_workflow_variable_source_types_variable.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/ds_workflow_variable_source_types_variable.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/e_sign_document_from_e_sign_template.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_document_from_e_sign_template.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/e_sign_document_from_previous_step.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_document_from_previous_step.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/e_sign_document_types_from_ds_template.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_document_types_from_ds_template.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/e_sign_document_types_from_previous_step.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_document_types_from_previous_step.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/e_sign_documents.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_documents.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/e_sign_locale_policy.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_locale_policy.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/e_sign_signer.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_signer.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/e_sign_tabs.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_tabs.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/e_sign_tabs_record.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/e_sign_tabs_record.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/error_codes.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/error_codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     _10008 = "ERR_10008"
     _10009 = "ERR_10009"
     _10101 = "ERR_10101"
     _10201 = "ERR_10201"
     _10202 = "ERR_10202"
     _10301 = "ERR_10301"
     _10302 = "ERR_10302"
-    _10401 = "ERR_10401"
     _10801 = "ERR_10801"
     _10802 = "ERR_10802"
     _10999 = "ERR_10999"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/error_response.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/error_response.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/event_types.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/replication_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,40 +15,33 @@
 import re  # noqa: F401
 
 import six
 
 from docusign_maestro.client.configuration import Configuration
 
 
-class EventTypes(object):
+class ReplicationStatus(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    ENVELOPE_SENT = "envelope-sent"
-    ENVELOPE_DELIVERED = "envelope-delivered"
-    ENVELOPE_COMPLETED = "envelope-completed"
-    ENVELOPE_DECLINED = "envelope-declined"
-    ENVELOPE_VOIDED = "envelope-voided"
-    ENVELOPE_CREATED = "envelope-created"
-    ENVELOPE_RESENT = "envelope-resent"
-    ENVELOPE_CORRECTED = "envelope-corrected"
-    ENVELOPE_PURGE = "envelope-purge"
-    ENVELOPE_DELETED = "envelope-deleted"
-    ENVELOPE_DISCARD = "envelope-discard"
-    DELIVERY_FAILED = "Delivery Failed"
-    AUTHENTICATION_FAILED = "Authentication Failed"
-    SENT = "Sent"
-    DELIVERED = "Delivered"
-    SIGNED = "Signed"
-    COMPLETED = "Completed"
+    DEPLOY_REPLICATION_IN_PROGRESS = "Deploy Replication In Progress"
+    DEPLOY_REPLICATED = "Deploy Replicated"
+    DEPLOY_REPLICATION_FAILED = "Deploy Replication Failed"
+    NOT_REPLICATED = "Not Replicated"
+    DELETE_REPLICATION_IN_PROGRESS = "Delete Replication in Progress"
+    DELETE_REPLICATED = "Delete Replicated"
+    DELETE_REPLICATION_FAILED = "Delete Replication Failed"
+    UNPUBLISH_REPLICATION_IN_PROGRESS = "Unpublish replication in Progress"
+    UNPUBLISH_REPLICATED = "Unpublish Replicated"
+    UNPUBLISH_REPLICATION_FAILED = "Unpublish Replication Failed"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -56,15 +49,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None, **kwargs):  # noqa: E501
-        """EventTypes - a model defined in Swagger"""  # noqa: E501
+        """ReplicationStatus - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -83,15 +76,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(EventTypes, dict):
+        if issubclass(ReplicationStatus, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -99,18 +92,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, EventTypes):
+        if not isinstance(other, ReplicationStatus):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, EventTypes):
+        if not isinstance(other, ReplicationStatus):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/get_configuration_instance_response.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/get_configuration_instance_response.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/get_configuration_instances_response.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/get_configuration_instances_response.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/get_configuration_instances_response_config_instances.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/get_configuration_instances_response_config_instances.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/http_types.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/user_id.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,43 +15,35 @@
 import re  # noqa: F401
 
 import six
 
 from docusign_maestro.client.configuration import Configuration
 
 
-class HttpTypes(object):
+class UserId(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
-    allowed enum values
-    """
-    GET = "Get"
-    POST = "Post"
-    PUT = "Put"
-    DELETE = "Delete"
-
-    """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None, **kwargs):  # noqa: E501
-        """HttpTypes - a model defined in Swagger"""  # noqa: E501
+        """UserId - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -70,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(HttpTypes, dict):
+        if issubclass(UserId, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -86,18 +78,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, HttpTypes):
+        if not isinstance(other, UserId):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, HttpTypes):
+        if not isinstance(other, UserId):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/invalid_workflow_response.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/invalid_workflow_response.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/last_deployed_id.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/last_deployed_id.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/new_or_updated_workflow_definition_response.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/new_or_updated_workflow_definition_response.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/number_or_variable.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/number_or_variable.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/participant.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/participant.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/participant_keys.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/participant_keys.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/progress_instance.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/progress_instance.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/record_string_boolean.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/record_string_boolean.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/record_string_or_variable_or_transformation.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/record_string_or_variable_or_transformation.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/record_to_never.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/record_to_never.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/replication_status.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_metadata_status.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,33 +15,29 @@
 import re  # noqa: F401
 
 import six
 
 from docusign_maestro.client.configuration import Configuration
 
 
-class ReplicationStatus(object):
+class WorkflowMetadataStatus(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    DEPLOY_REPLICATION_IN_PROGRESS = "Deploy Replication In Progress"
-    DEPLOY_REPLICATED = "Deploy Replicated"
-    DEPLOY_REPLICATION_FAILED = "Deploy Replication Failed"
-    NOT_REPLICATED = "Not Replicated"
-    DELETE_REPLICATION_IN_PROGRESS = "Delete Replication in Progress"
-    DELETE_REPLICATED = "Delete Replicated"
-    DELETE_REPLICATION_FAILED = "Delete Replication Failed"
-    UNPUBLISH_REPLICATION_IN_PROGRESS = "Unpublish replication in Progress"
-    UNPUBLISH_REPLICATED = "Unpublish Replicated"
-    UNPUBLISH_REPLICATION_FAILED = "Unpublish Replication Failed"
+    ACTIVE = "active"
+    INACTIVE = "inactive"
+    PUBLISHING = "publishing"
+    UNPUBLISHING = "unpublishing"
+    ARCHIVED = "archived"
+    ARCHIVING = "archiving"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -49,15 +45,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None, **kwargs):  # noqa: E501
-        """ReplicationStatus - a model defined in Swagger"""  # noqa: E501
+        """WorkflowMetadataStatus - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -76,15 +72,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ReplicationStatus, dict):
+        if issubclass(WorkflowMetadataStatus, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -92,18 +88,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ReplicationStatus):
+        if not isinstance(other, WorkflowMetadataStatus):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ReplicationStatus):
+        if not isinstance(other, WorkflowMetadataStatus):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/started_by_instance.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/started_by_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     def started_by_type(self, started_by_type):
         """Sets the started_by_type of this StartedByInstance.
 
 
         :param started_by_type: The started_by_type of this StartedByInstance.  # noqa: E501
         :type: str
         """
-        allowed_values = ["Anonymous", "Preparer", "Participant", "OnBehalfOf"]  # noqa: E501
+        allowed_values = ["Anonymous", "Preparer", "Participant"]  # noqa: E501
         if (self._configuration.client_side_validation and
                 started_by_type not in allowed_values):
             raise ValueError(
                 "Invalid value for `started_by_type` ({0}), must be one of {1}"  # noqa: E501
                 .format(started_by_type, allowed_values)
             )
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/string_or_variable_or_transformation.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/string_or_variable_or_transformation.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/success_message_response.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/success_message_response.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/template_id.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/template_id.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/trigger_payload.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/trigger_payload.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/trigger_workflow_via_post_response.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/trigger_workflow_via_post_response.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/user_id.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/version_string.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import re  # noqa: F401
 
 import six
 
 from docusign_maestro.client.configuration import Configuration
 
 
-class UserId(object):
+class VersionString(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
@@ -35,15 +35,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None, **kwargs):  # noqa: E501
-        """UserId - a model defined in Swagger"""  # noqa: E501
+        """VersionString - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -62,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UserId, dict):
+        if issubclass(VersionString, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,18 +78,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UserId):
+        if not isinstance(other, VersionString):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, UserId):
+        if not isinstance(other, VersionString):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/validation_errors.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/validation_errors.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/version_string.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_instance_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import re  # noqa: F401
 
 import six
 
 from docusign_maestro.client.configuration import Configuration
 
 
-class VersionString(object):
+class WorkflowInstanceId(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
@@ -35,15 +35,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None, **kwargs):  # noqa: E501
-        """VersionString - a model defined in Swagger"""  # noqa: E501
+        """WorkflowInstanceId - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -62,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(VersionString, dict):
+        if issubclass(WorkflowInstanceId, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,18 +78,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, VersionString):
+        if not isinstance(other, WorkflowInstanceId):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, VersionString):
+        if not isinstance(other, WorkflowInstanceId):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_creator_id.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_creator_id.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_date_time.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_date_time.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_definition.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_definition.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_definition_list.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_definition_list.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_definition_metadata.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_definition_metadata.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_definition_with_id.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_definition_with_id.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_delete_response.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_delete_response.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_instance.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,26 +315,24 @@
 
         self._template_id = template_id
 
     @property
     def users(self):
         """Gets the users of this WorkflowInstance.  # noqa: E501
 
-        Contains the list of Users and Steps mapping  # noqa: E501
 
         :return: The users of this WorkflowInstance.  # noqa: E501
         :rtype: dict(str, str)
         """
         return self._users
 
     @users.setter
     def users(self, users):
         """Sets the users of this WorkflowInstance.
 
-        Contains the list of Users and Steps mapping  # noqa: E501
 
         :param users: The users of this WorkflowInstance.  # noqa: E501
         :type: dict(str, str)
         """
         if self._configuration.client_side_validation and users is None:
             raise ValueError("Invalid value for `users`, must not be `None`")  # noqa: E501
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_instance_id.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_instances_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import re  # noqa: F401
 
 import six
 
 from docusign_maestro.client.configuration import Configuration
 
 
-class WorkflowInstanceId(object):
+class WorkflowInstancesList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
@@ -35,15 +35,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None, **kwargs):  # noqa: E501
-        """WorkflowInstanceId - a model defined in Swagger"""  # noqa: E501
+        """WorkflowInstancesList - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -62,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(WorkflowInstanceId, dict):
+        if issubclass(WorkflowInstancesList, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,18 +78,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WorkflowInstanceId):
+        if not isinstance(other, WorkflowInstancesList):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, WorkflowInstanceId):
+        if not isinstance(other, WorkflowInstancesList):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_instance_map.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_instance_map.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_instance_state.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_instance_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,17 @@
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    CREATED = "Created"
     IN_PROGRESS = "In Progress"
     COMPLETED = "Completed"
     FAILED = "Failed"
-    CANCELED = "Canceled"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_instances_list.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/event_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,35 +15,43 @@
 import re  # noqa: F401
 
 import six
 
 from docusign_maestro.client.configuration import Configuration
 
 
-class WorkflowInstancesList(object):
+class EventTypes(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
+    allowed enum values
+    """
+    SENT = "Sent"
+    DELIVERED = "Delivered"
+    SIGNED = "Signed"
+    COMPLETED = "Completed"
+
+    """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None, **kwargs):  # noqa: E501
-        """WorkflowInstancesList - a model defined in Swagger"""  # noqa: E501
+        """EventTypes - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -62,15 +70,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(WorkflowInstancesList, dict):
+        if issubclass(EventTypes, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,18 +86,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WorkflowInstancesList):
+        if not isinstance(other, EventTypes):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, WorkflowInstancesList):
+        if not isinstance(other, EventTypes):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_metadata_status.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_step_history_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,29 +15,26 @@
 import re  # noqa: F401
 
 import six
 
 from docusign_maestro.client.configuration import Configuration
 
 
-class WorkflowMetadataStatus(object):
+class WorkflowStepHistoryState(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    ACTIVE = "active"
-    INACTIVE = "inactive"
-    PUBLISHING = "publishing"
-    UNPUBLISHING = "unpublishing"
-    ARCHIVED = "archived"
-    ARCHIVING = "archiving"
+    IN_PROGRESS = "In Progress"
+    COMPLETED = "Completed"
+    FAILED = "Failed"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -45,15 +42,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None, **kwargs):  # noqa: E501
-        """WorkflowMetadataStatus - a model defined in Swagger"""  # noqa: E501
+        """WorkflowStepHistoryState - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -72,15 +69,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(WorkflowMetadataStatus, dict):
+        if issubclass(WorkflowStepHistoryState, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -88,18 +85,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WorkflowMetadataStatus):
+        if not isinstance(other, WorkflowStepHistoryState):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, WorkflowMetadataStatus):
+        if not isinstance(other, WorkflowStepHistoryState):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_step_error.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_step_error.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_step_error_error.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_step_error_error.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_step_history.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_step_history.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro/models/workflow_step_history_list.py` & `docusign-maestro-1.0.0rc1/docusign_maestro/models/workflow_step_history_list.py`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/docusign_maestro.egg-info/PKG-INFO` & `docusign-maestro-1.0.0rc1/docusign_maestro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: docusign-maestro
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Maestro API
 Home-page: 
 Author-email: devcenter@docusign.com
 Keywords: Swagger,Maestro API
 Description-Content-Type: text/markdown
 
 # docusign-maestro
 Maestro authors and executes experiences that allow non-coders the ability to define Simple Business Process without having to write code and to deploy them seamlessly without having to have development expertise
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0.0
-- Package version: 1.0.0
+- Package version: 1.0.0rc1
 - Build package: io.swagger.codegen.languages.PythonClientCodegen
 For more information, please visit [https://developers.docusign.com/](https://developers.docusign.com/)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -159,14 +159,15 @@
  - [DSWorkflowTrigger](docs/DSWorkflowTrigger.md)
  - [DSWorkflowTriggerTypes](docs/DSWorkflowTriggerTypes.md)
  - [DSWorkflowVariable](docs/DSWorkflowVariable.md)
  - [DSWorkflowVariableFromParticipant](docs/DSWorkflowVariableFromParticipant.md)
  - [DSWorkflowVariableFromStep](docs/DSWorkflowVariableFromStep.md)
  - [DSWorkflowVariableFromVariable](docs/DSWorkflowVariableFromVariable.md)
  - [DSWorkflowVariableRecord](docs/DSWorkflowVariableRecord.md)
+ - [DSWorkflowVariableSourceTypesParticipant](docs/DSWorkflowVariableSourceTypesParticipant.md)
  - [DSWorkflowVariableSourceTypesStep](docs/DSWorkflowVariableSourceTypesStep.md)
  - [DSWorkflowVariableSourceTypesVariable](docs/DSWorkflowVariableSourceTypesVariable.md)
  - [DeployRequest](docs/DeployRequest.md)
  - [DeployResponse](docs/DeployResponse.md)
  - [DeployStatus](docs/DeployStatus.md)
  - [DeploymentStatus](docs/DeploymentStatus.md)
  - [ESignDocumentFromESignTemplate](docs/ESignDocumentFromESignTemplate.md)
@@ -185,14 +186,15 @@
  - [GetConfigurationInstancesResponse](docs/GetConfigurationInstancesResponse.md)
  - [GetConfigurationInstancesResponseConfigInstances](docs/GetConfigurationInstancesResponseConfigInstances.md)
  - [HttpTypes](docs/HttpTypes.md)
  - [InvalidWorkflowResponse](docs/InvalidWorkflowResponse.md)
  - [NewOrUpdatedWorkflowDefinitionResponse](docs/NewOrUpdatedWorkflowDefinitionResponse.md)
  - [NumberOrVariable](docs/NumberOrVariable.md)
  - [Participant](docs/Participant.md)
+ - [ParticipantKeys](docs/ParticipantKeys.md)
  - [ProgressInstance](docs/ProgressInstance.md)
  - [RecordStringBoolean](docs/RecordStringBoolean.md)
  - [RecordStringOrVariableOrTransformation](docs/RecordStringOrVariableOrTransformation.md)
  - [RecordToNever](docs/RecordToNever.md)
  - [ReplicationStatus](docs/ReplicationStatus.md)
  - [StartedByInstance](docs/StartedByInstance.md)
  - [StringOrVariableOrTransformation](docs/StringOrVariableOrTransformation.md)
```

### Comparing `docusign-maestro-1.0.0/docusign_maestro.egg-info/SOURCES.txt` & `docusign-maestro-1.0.0rc1/docusign_maestro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docusign-maestro-1.0.0/setup.py` & `docusign-maestro-1.0.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages, Command, os  # noqa: H301	
 
 NAME = "docusign-maestro"
-VERSION = "1.0.0"
+VERSION = "1.0.0rc1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

