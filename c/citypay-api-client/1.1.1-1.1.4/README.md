# Comparing `tmp/citypay_api_client-1.1.1.tar.gz` & `tmp/citypay_api_client-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citypay_api_client-1.1.1.tar", last modified: Mon Dec 12 12:40:48 2022, max compression
+gzip compressed data, was "citypay_api_client-1.1.4.tar", last modified: Mon Apr 29 15:02:27 2024, max compression
```

## Comparing `citypay_api_client-1.1.1.tar` & `citypay_api_client-1.1.4.tar`

### file list

```diff
@@ -1,194 +1,221 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 12:40:48.736989 citypay_api_client-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2022-12-12 12:40:48.736989 citypay_api_client-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21930 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 12:40:48.720989 citypay_api_client-1.1.1/citypay/
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 12:40:48.720989 citypay_api_client-1.1.1/citypay/api/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58595 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/api/authorisation_and_payment_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19142 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/api/batch_processing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    60578 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/api/card_holder_account_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    32028 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/api/direct_post_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30055 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/api/operational_functions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    61351 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/api/paylink_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40976 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 12:40:48.724989 citypay_api_client-1.1.1/citypay/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19415 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 12:40:48.728989 citypay_api_client-1.1.1/citypay/model/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14250 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/account_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/account_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    14526 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/acknowledgement.py
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/acl_check_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/acl_check_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21249 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/airline_advice.py
--rw-r--r--   0 runner    (1001) docker     (123)    17831 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/airline_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    17813 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/auth_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13435 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/auth_references.py
--rw-r--r--   0 runner    (1001) docker     (123)    31530 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/auth_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    36203 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14266 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/authen_required.py
--rw-r--r--   0 runner    (1001) docker     (123)    15596 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14053 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/batch_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    17206 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/batch_report_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/batch_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20886 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/batch_transaction_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15887 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/bin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13333 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/bin_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/c_res_auth_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/capture_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    19966 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/card.py
--rw-r--r--   0 runner    (1001) docker     (123)    16650 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/card_holder_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/card_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    35555 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/charge_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13851 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/check_batch_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    13418 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/check_batch_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18225 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/contact_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    14125 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/decision.py
--rw-r--r--   0 runner    (1001) docker     (123)    33092 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/direct_post_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14906 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/direct_token_auth_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13504 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/domain_key_check_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13983 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/domain_key_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14600 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/domain_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14832 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    14628 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/event_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13946 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/exists.py
--rw-r--r--   0 runner    (1001) docker     (123)    14843 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/external_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/list_merchants_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14267 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/mcc6012.py
--rw-r--r--   0 runner    (1001) docker     (123)    14388 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/merchant.py
--rw-r--r--   0 runner    (1001) docker     (123)    14359 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/pa_res_auth_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    15613 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    13997 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_adjustment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_attachment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14062 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_attachment_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    16976 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_bill_payment_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    18103 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_card_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16805 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_cart.py
--rw-r--r--   0 runner    (1001) docker     (123)    16818 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_cart_item_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23568 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15958 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_custom_param.py
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_email_notification_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    13603 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    15815 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_field_guard_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14821 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_part_payments.py
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_sms_notification_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_state_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    17767 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_token_created.py
--rw-r--r--   0 runner    (1001) docker     (123)    19250 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_token_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    22514 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_token_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    14665 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_token_status_change_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14265 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_token_status_change_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14558 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/paylink_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    13471 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/process_batch_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13719 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/process_batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    17266 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/refund_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    15216 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/register_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    14910 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/request_challenged.py
--rw-r--r--   0 runner    (1001) docker     (123)    14293 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/retrieve_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    22391 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/three_d_secure.py
--rw-r--r--   0 runner    (1001) docker     (123)    18270 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/tokenisation_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14441 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model/void_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    84409 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 12:40:48.728989 citypay_api_client-1.1.1/citypay/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16103 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 12:40:48.728989 citypay_api_client-1.1.1/citypay/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/utils/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/citypay/utils/direct_post_mac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 12:40:48.728989 citypay_api_client-1.1.1/citypay_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2022-12-12 12:40:48.000000 citypay_api_client-1.1.1/citypay_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2022-12-12 12:40:48.000000 citypay_api_client-1.1.1/citypay_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 12:40:48.000000 citypay_api_client-1.1.1/citypay_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2022-12-12 12:40:48.000000 citypay_api_client-1.1.1/citypay_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-12 12:40:48.000000 citypay_api_client-1.1.1/citypay_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-12 12:40:48.736989 citypay_api_client-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 12:40:48.736989 citypay_api_client-1.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_account_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_account_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_acknowledgement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_acl_check_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_acl_check_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_airline_advice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_airline_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7684 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_auth_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_auth_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_auth_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_authen_required.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_authorisation_and_payment_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_batch_processing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_batch_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_batch_report_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_batch_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_batch_transaction_result_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_bin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_bin_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_c_res_auth_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_capture_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_card_holder_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_card_holder_account_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_card_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_charge_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_check_batch_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_check_batch_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_contact_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_decision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_direct_post_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_direct_post_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_direct_token_auth_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_domain_key_check_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_domain_key_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_domain_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_event_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_external_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_it_api_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_list_merchants_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_mcc6012.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_merchant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_operational_functions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_pa_res_auth_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_adjustment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_attachment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_attachment_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_bill_payment_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_card_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_cart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_cart_item_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_custom_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_email_notification_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_field_guard_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_part_payments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_sms_notification_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_state_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_token_created.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_token_request_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_token_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_token_status_change_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_token_status_change_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_paylink_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_process_batch_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_process_batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_refund_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_register_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_request_challenged.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_retrieve_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_three_d_secure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_tokenisation_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2022-12-12 12:40:37.000000 citypay_api_client-1.1.1/test/test_void_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:02:27.466645 citypay_api_client-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-29 15:02:27.466645 citypay_api_client-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19240 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:02:27.434645 citypay_api_client-1.1.4/citypay/
+-rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:02:27.438645 citypay_api_client-1.1.4/citypay/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113530 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/api/authorisation_and_payment_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38715 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/api/batch_processing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131069 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/api/card_holder_account_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67117 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/api/direct_post_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61984 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/api/operational_functions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   157595 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/api/paylink_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68733 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/api/reporting_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28218 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/api_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:02:27.438645 citypay_api_client-1.1.4/citypay/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19358 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84409 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:02:27.450645 citypay_api_client-1.1.4/citypay/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/account_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/account_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/acknowledgement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/acl_check_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/acl_check_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/airline_advice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/airline_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8850 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/auth_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/auth_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17230 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/auth_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18536 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/authen_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/batch_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/batch_report_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/batch_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/batch_transaction_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/batch_transaction_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10456 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/batch_transaction_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/bin_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/c_res_auth_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/capture_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/card_holder_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/card_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17889 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/charge_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/check_batch_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/check_batch_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/contact_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17115 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/direct_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7033 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/direct_token_auth_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/domain_key_check_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/domain_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/domain_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/event_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/external_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/list_merchants_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/mcc6012.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/merchant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/merchant_batch_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/merchant_batch_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/merchant_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/net_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/pa_res_auth_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_adjustment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_attachment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_attachment_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_bill_payment_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_card_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_cart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_cart_item_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_custom_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_email_notification_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_field_guard_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_part_payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_resend_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_sms_notification_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_state_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_token_created.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_token_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_token_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_token_status_change_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_token_status_change_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/paylink_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/payment_intent_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/process_batch_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/process_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/refund_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/register_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/remittance_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/remittance_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/remittance_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/remitted_client_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/request_challenged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/retrieve_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11269 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/three_d_secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/tokenisation_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/models/void_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:02:27.454645 citypay_api_client-1.1.4/citypay/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/utils/digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/citypay/utils/direct_post_mac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:02:27.454645 citypay_api_client-1.1.4/citypay_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-29 15:02:27.000000 citypay_api_client-1.1.4/citypay_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-29 15:02:27.000000 citypay_api_client-1.1.4/citypay_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:02:27.000000 citypay_api_client-1.1.4/citypay_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-29 15:02:27.000000 citypay_api_client-1.1.4/citypay_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 15:02:27.000000 citypay_api_client-1.1.4/citypay_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 15:02:27.470645 citypay_api_client-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:02:27.466645 citypay_api_client-1.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_account_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_account_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_acknowledgement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_acl_check_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_acl_check_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_airline_advice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_airline_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_auth_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_auth_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_auth_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_authen_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_authorisation_and_payment_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_batch_processing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_batch_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_batch_report_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_batch_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_batch_transaction_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_batch_transaction_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_batch_transaction_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_bin_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_c_res_auth_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_capture_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_card_holder_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_card_holder_account_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_card_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_charge_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_check_batch_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_check_batch_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_contact_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_direct_post_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_direct_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_direct_token_auth_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_domain_key_check_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_domain_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_domain_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_event_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_external_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_it_api_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_list_merchants_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_mcc6012.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_merchant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_merchant_batch_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_merchant_batch_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_merchant_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_net_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_operational_functions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_pa_res_auth_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_adjustment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_attachment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_attachment_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_bill_payment_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_card_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_cart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_cart_item_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_custom_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_email_notification_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_field_guard_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_part_payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_resend_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_sms_notification_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_state_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_token_created.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_token_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_token_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_token_status_change_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_token_status_change_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_paylink_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_payment_intent_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_process_batch_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_process_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_refund_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_register_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_remittance_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_remittance_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_remittance_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_remitted_client_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_reporting_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_request_challenged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_retrieve_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_three_d_secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_tokenisation_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-29 15:02:18.000000 citypay_api_client-1.1.4/test/test_void_request.py
```

### Comparing `citypay_api_client-1.1.1/PKG-INFO` & `citypay_api_client-1.1.4/test/test_domain_key_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,35 @@
-Metadata-Version: 2.1
-Name: citypay_api_client
-Version: 1.1.1
-Summary: CityPay Payment API
-Home-page: 
-Author: CityPay Support
-Author-email: support@citypay.com
-Keywords: OpenAPI,OpenAPI-Generator,CityPay Payment API
-Requires-Python: >=3.6
+"""
+    CityPay Payment API
 
      This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security Your application will need to adhere to PCI-DSS standards to operate safely and to meet requirements set out by  Visa and MasterCard and the PCI Security Standards Council. These include  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
-    
+
+    Contact: support@citypay.com
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import citypay
+from citypay.models.domain_key_request import DomainKeyRequest
+
+
+class TestDomainKeyRequest(unittest.TestCase):
+    """DomainKeyRequest unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testDomainKeyRequest(self):
+        """Test DomainKeyRequest"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = DomainKeyRequest()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `citypay_api_client-1.1.1/citypay/__init__.py` & `citypay_api_client-1.1.4/test/test_direct_token_auth_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,35 @@
-# flake8: noqa
-
 """
     CityPay Payment API
 
      This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security Your application will need to adhere to PCI-DSS standards to operate safely and to meet requirements set out by  Visa and MasterCard and the PCI Security Standards Council. These include  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.1.1"
+import sys
+import unittest
+
+import citypay
+from citypay.models.direct_token_auth_request import DirectTokenAuthRequest
+
+
+class TestDirectTokenAuthRequest(unittest.TestCase):
+    """DirectTokenAuthRequest unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
 
-# import ApiClient
-from citypay.api_client import ApiClient
+    def testDirectTokenAuthRequest(self):
+        """Test DirectTokenAuthRequest"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = DirectTokenAuthRequest()  # noqa: E501
+        pass
 
-# import Configuration
-from citypay.configuration import Configuration
 
-# import exceptions
-from citypay.exceptions import OpenApiException
-from citypay.exceptions import ApiAttributeError
-from citypay.exceptions import ApiTypeError
-from citypay.exceptions import ApiValueError
-from citypay.exceptions import ApiKeyError
-from citypay.exceptions import ApiException
-from citypay.model.api_key import api_key_generate
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `citypay_api_client-1.1.1/citypay/apis/__init__.py` & `citypay_api_client-1.1.4/citypay/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/citypay/configuration.py` & `citypay_api_client-1.1.4/citypay/configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,84 +1,61 @@
+# coding: utf-8
+
 """
     CityPay Payment API
 
-     This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security Your application will need to adhere to PCI-DSS standards to operate safely and to meet requirements set out by  Visa and MasterCard and the PCI Security Standards Council. These include  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
+     Welcome to the CityPay API, a robust HTTP API payment solution designed for seamless server-to-server  transactional processing. Our API facilitates a wide array of payment operations, catering to diverse business needs.  Whether you're integrating Internet payments, handling Mail Order/Telephone Order (MOTO) transactions, managing  Subscriptions with Recurring and Continuous Authority payments, or navigating the complexities of 3-D Secure  authentication, our API is equipped to support your requirements. Additionally, we offer functionalities for  Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids, and Completion processing, alongside the capability  for tokenised payments.  ## Compliance and Security Overview <aside class=\"notice\">   Ensuring the security of payment transactions and compliance with industry standards is paramount. Our API is    designed with stringent security measures and compliance protocols to safeguard sensitive information and meet    the rigorous requirements of Visa, MasterCard, and the PCI Security Standards Council. </aside>  ### Key Compliance and Security Measures  * **TLS Encryption**: All data transmissions must utilise TLS version 1.2 or higher, employing [strong cryptography](#enabled-tls-ciphers). Our infrastructure strictly enforces this requirement to maintain the integrity and confidentiality of data in transit. We conduct regular scans and assessments of our TLS endpoints to identify and mitigate vulnerabilities. * **Data Storage Prohibitions**: Storing sensitive cardholder data (CHD), such as the card security code (CSC) or primary account number (PAN), is strictly prohibited. Our API is designed to minimize your exposure to sensitive data, thereby reducing your compliance burden. * **Data Masking**: For consumer protection and compliance, full card numbers must not be displayed on receipts or any customer-facing materials. Our API automatically masks PANs, displaying only the last four digits to facilitate safe receipt generation. * **Network Scans**: If your application is web-based, regular scans of your hosting environment are mandatory to identify and rectify potential vulnerabilities. This proactive measure is crucial for maintaining a secure and compliant online presence. * **PCI Compliance**: Adherence to PCI DSS standards is not optional; it's a requirement for operating securely and legally in the payments ecosystem. For detailed information on compliance requirements and resources, please visit the PCI Security Standards Council website [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/). * **Request Validation**: Our API includes mechanisms to verify the legitimacy of each request, ensuring it pertains to a valid account and originates from a trusted source. We leverage remote IP address verification alongside sophisticated application firewall technologies to thwart a wide array of common security threats.  ## Getting Started Before integrating with the CityPay API, ensure your application and development practices align with the outlined compliance and security measures. This preparatory step is crucial for a smooth integration process and the long-term success of your payment processing operations.  For further details on API endpoints, request/response formats, and code examples, proceed to the subsequent sections of our documentation. Our aim is to provide you with all the necessary tools and information to integrate our payment processing capabilities seamlessly into your application.  Thank you for choosing CityPay API. We look forward to supporting your payment processing needs with our secure, compliant, and versatile API solution. 
 
     Contact: support@citypay.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
-from http import client as http_client
-from citypay.exceptions import ApiValueError
-
+import http.client as httplib
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
-class Configuration(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-
-    Ref: https://openapi-generator.tech
-    Do not edit the class manually.
+class Configuration:
+    """This class contains various settings of the API client.
 
-    :param host: Base url
+    :param host: Base url.
     :param api_key: Dict to store API key(s).
       Each entry in the dict specifies an API key.
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is the API key secret.
-    :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
+    :param api_key_prefix: Dict to store API prefix (e.g. Bearer).
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is an API key prefix when generating the auth data.
-    :param username: Username for HTTP basic authentication
-    :param password: Password for HTTP basic authentication
-    :param discard_unknown_keys: Boolean value indicating whether to discard
-      unknown properties. A server may send a response that includes additional
-      properties that are not known by the client in the following scenarios:
-      1. The OpenAPI document is incomplete, i.e. it does not match the server
-         implementation.
-      2. The client was generated using an older version of the OpenAPI document
-         and the server has been upgraded since then.
-      If a schema in the OpenAPI document defines the additionalProperties attribute,
-      then all undeclared properties received by the server are injected into the
-      additional properties map. In that case, there are undeclared properties, and
-      nothing to discard.
-    :param disabled_client_side_validations (string): Comma-separated list of
-      JSON schema validation keywords to disable JSON schema structural validation
-      rules. The following keywords may be specified: multipleOf, maximum,
-      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
-      maxItems, minItems.
-      By default, the validation is performed for data generated locally by the client
-      and data received from the server, independent of any validation performed by
-      the server side. If the input data does not satisfy the JSON schema validation
-      rules specified in the OpenAPI document, an exception is raised.
-      If disabled_client_side_validations is set, structural validation is
-      disabled. This can be useful to troubleshoot data validation problem, such as
-      when the OpenAPI document validation rules do not match the actual API data
-      received by the server.
+    :param username: Username for HTTP basic authentication.
+    :param password: Password for HTTP basic authentication.
+    :param access_token: Access token.
     :param server_index: Index to servers configuration.
     :param server_variables: Mapping with string values to replace variables in
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
-      The validation of enums is performed for variables with defined enum values before.
+      The validation of enums is performed for variables with defined enum
+      values before.
     :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
-      in PEM format
+      in PEM format.
 
     :Example:
 
     API Key Authentication Example.
     Given the following security scheme in the OpenAPI specification:
       components:
         securitySchemes:
@@ -98,22 +75,20 @@
        Cookie: JSESSIONID abc123
     """
 
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
-                 access_token=None,
                  username=None, password=None,
-                 discard_unknown_keys=False,
-                 disabled_client_side_validations="",
+                 access_token=None,
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
-                 ):
+                 ) -> None:
         """Constructor
         """
         self._base_path = "https://api.citypay.com" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
@@ -123,15 +98,14 @@
         self.server_operation_variables = server_operation_variables or {}
         """Default server variables
         """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
-        self.access_token = access_token
         self.api_key = {}
         if api_key:
             self.api_key = api_key
         """dict to store API key(s)
         """
         self.api_key_prefix = {}
         if api_key_prefix:
@@ -143,16 +117,17 @@
         """
         self.username = username
         """Username for HTTP basic authentication
         """
         self.password = password
         """Password for HTTP basic authentication
         """
-        self.discard_unknown_keys = discard_unknown_keys
-        self.disabled_client_side_validations = disabled_client_side_validations
+        self.access_token = access_token
+        """Access token
+        """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("citypay")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -183,43 +158,53 @@
         """
         self.key_file = None
         """client key file
         """
         self.assert_hostname = None
         """Set this to True/False to enable/disable SSL hostname verification.
         """
+        self.tls_server_name = None
+        """SSL/TLS Server Name Indication (SNI)
+           Set this to the SNI value expected by the server.
+        """
 
         self.connection_pool_maxsize = multiprocessing.cpu_count() * 5
         """urllib3 connection pool's maximum number of connections saved
            per pool. urllib3 uses 1 connection as default value, but this is
            not the best value when you are making a lot of possibly parallel
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
         """
 
         self.proxy = None
         """Proxy URL
         """
-        self.no_proxy = None
-        """bypass proxy for host in the no_proxy list.
-        """
         self.proxy_headers = None
         """Proxy headers
         """
         self.safe_chars_for_path_param = ''
         """Safe chars for path_param
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
         # Enable client side validation
         self.client_side_validation = True
 
-        # Options to pass down to the underlying urllib3 socket
         self.socket_options = None
+        """Options to pass down to the underlying urllib3 socket
+        """
+
+        self.datetime_format = "%Y-%m-%dT%H:%M:%S.%f%z"
+        """datetime format
+        """
+
+        self.date_format = "%Y-%m-%d"
+        """date format
+        """
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ('logger', 'logger_file_handler'):
@@ -229,46 +214,49 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
-        if name == 'disabled_client_side_validations':
-            s = set(filter(None, value.split(',')))
-            for v in s:
-                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
-                    raise ApiValueError(
-                        "Invalid keyword: '{0}''".format(v))
-            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
 
         :param default: object of Configuration
         """
-        cls._default = copy.deepcopy(default)
+        cls._default = default
 
     @classmethod
     def get_default_copy(cls):
-        """Return new instance of configuration.
+        """Deprecated. Please use `get_default` instead.
+
+        Deprecated. Please use `get_default` instead.
+
+        :return: The configuration object.
+        """
+        return cls.get_default()
+
+    @classmethod
+    def get_default(cls):
+        """Return the default configuration.
 
         This method returns newly created, based on default constructor,
         object of Configuration class or returns a copy of default
-        configuration passed by the set_default method.
+        configuration.
 
         :return: The configuration object.
         """
-        if cls._default is not None:
-            return copy.deepcopy(cls._default)
-        return Configuration()
+        if cls._default is None:
+            cls._default = Configuration()
+        return cls._default
 
     @property
     def logger_file(self):
         """The logger file.
 
         If the logger_file is None, then add stream handler and remove file
         handler. Otherwise, add file handler and remove stream handler.
@@ -314,23 +302,23 @@
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
             for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on http_client debug
-            http_client.HTTPConnection.debuglevel = 1
+            # turn on httplib debug
+            httplib.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
             for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off http_client debug
-            http_client.HTTPConnection.debuglevel = 0
+            # turn off httplib debug
+            httplib.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -413,16 +401,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 6.4.18\n"\
-               "SDK Package Version: 1.1.1".\
+               "Version of the API: 6.6.40\n"\
+               "SDK Package Version: 1.1.4".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `citypay_api_client-1.1.1/citypay/model/acknowledgement.py` & `citypay_api_client-1.1.4/citypay/models/auth_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,283 +1,161 @@
+# coding: utf-8
+
 """
     CityPay Payment API
 
-     This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security Your application will need to adhere to PCI-DSS standards to operate safely and to meet requirements set out by  Visa and MasterCard and the PCI Security Standards Council. These include  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
+     Welcome to the CityPay API, a robust HTTP API payment solution designed for seamless server-to-server  transactional processing. Our API facilitates a wide array of payment operations, catering to diverse business needs.  Whether you're integrating Internet payments, handling Mail Order/Telephone Order (MOTO) transactions, managing  Subscriptions with Recurring and Continuous Authority payments, or navigating the complexities of 3-D Secure  authentication, our API is equipped to support your requirements. Additionally, we offer functionalities for  Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids, and Completion processing, alongside the capability  for tokenised payments.  ## Compliance and Security Overview <aside class=\"notice\">   Ensuring the security of payment transactions and compliance with industry standards is paramount. Our API is    designed with stringent security measures and compliance protocols to safeguard sensitive information and meet    the rigorous requirements of Visa, MasterCard, and the PCI Security Standards Council. </aside>  ### Key Compliance and Security Measures  * **TLS Encryption**: All data transmissions must utilise TLS version 1.2 or higher, employing [strong cryptography](#enabled-tls-ciphers). Our infrastructure strictly enforces this requirement to maintain the integrity and confidentiality of data in transit. We conduct regular scans and assessments of our TLS endpoints to identify and mitigate vulnerabilities. * **Data Storage Prohibitions**: Storing sensitive cardholder data (CHD), such as the card security code (CSC) or primary account number (PAN), is strictly prohibited. Our API is designed to minimize your exposure to sensitive data, thereby reducing your compliance burden. * **Data Masking**: For consumer protection and compliance, full card numbers must not be displayed on receipts or any customer-facing materials. Our API automatically masks PANs, displaying only the last four digits to facilitate safe receipt generation. * **Network Scans**: If your application is web-based, regular scans of your hosting environment are mandatory to identify and rectify potential vulnerabilities. This proactive measure is crucial for maintaining a secure and compliant online presence. * **PCI Compliance**: Adherence to PCI DSS standards is not optional; it's a requirement for operating securely and legally in the payments ecosystem. For detailed information on compliance requirements and resources, please visit the PCI Security Standards Council website [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/). * **Request Validation**: Our API includes mechanisms to verify the legitimacy of each request, ensuring it pertains to a valid account and originates from a trusted source. We leverage remote IP address verification alongside sophisticated application firewall technologies to thwart a wide array of common security threats.  ## Getting Started Before integrating with the CityPay API, ensure your application and development practices align with the outlined compliance and security measures. This preparatory step is crucial for a smooth integration process and the long-term success of your payment processing operations.  For further details on API endpoints, request/response formats, and code examples, proceed to the subsequent sections of our documentation. Our aim is to provide you with all the necessary tools and information to integrate our payment processing capabilities seamlessly into your application.  Thank you for choosing CityPay API. We look forward to supporting your payment processing needs with our secure, compliant, and versatile API solution. 
 
     Contact: support@citypay.com
-    Generated by: https://openapi-generator.tech
-"""
-
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from citypay.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from citypay.exceptions import ApiAttributeError
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class Acknowledgement(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import Field
+from typing_extensions import Annotated
+from citypay.models.airline_advice import AirlineAdvice
+from citypay.models.contact_details import ContactDetails
+from citypay.models.event_data_model import EventDataModel
+from citypay.models.external_mpi import ExternalMPI
+from citypay.models.mcc6012 import MCC6012
+from citypay.models.three_d_secure import ThreeDSecure
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
 
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
+class AuthRequest(BaseModel):
     """
-
-    allowed_values = {
+    AuthRequest
+    """ # noqa: E501
+    airline_data: Optional[AirlineAdvice] = None
+    amount: Annotated[int, Field(strict=True)] = Field(description="The amount to authorise in the lowest unit of currency with a variable length to a maximum of 12 digits.  No decimal points are to be included and no divisional characters such as 1,024.  The amount should be the total amount required for the transaction.  For example with GBP £1,021.95 the amount value is 102195. ")
+    avs_postcode_policy: Optional[StrictStr] = Field(default=None, description="A policy value which determines whether an AVS postcode policy is enforced or bypassed.  Values are:   `0` for the default policy (default value if not supplied). Your default values are determined by your account manager on setup of the account.   `1` for an enforced policy. Transactions that are enforced will be rejected if the AVS postcode numeric value does not match.   `2` to bypass. Transactions that are bypassed will be allowed through even if the postcode did not match.   `3` to ignore. Transactions that are ignored will bypass the result and not send postcode details for authorisation. ")
+    bill_to: Optional[ContactDetails] = None
+    cardnumber: Annotated[str, Field(min_length=12, strict=True, max_length=22)] = Field(description="The card number (PAN) with a variable length to a maximum of 21 digits in numerical form. Any non numeric characters will be stripped out of the card number, this includes whitespace or separators internal of the provided value.  The card number must be treated as sensitive data. We only provide an obfuscated value in logging and reporting.  The plaintext value is encrypted in our database using AES 256 GMC bit encryption for settlement or refund purposes.  When providing the card number to our gateway through the authorisation API you will be handling the card data on your application. This will require further PCI controls to be in place and this value must never be stored. ")
+    csc: Optional[Annotated[str, Field(min_length=3, strict=True, max_length=4)]] = Field(default=None, description="The Card Security Code (CSC) (also known as CV2/CVV2) is normally found on the back of the card (American Express has it on the front). The value helps to identify possession of the card as it is not available within the chip or magnetic swipe.  When forwarding the CSC, please ensure the value is a string as some values start with 0 and this will be stripped out by any integer parsing.  The CSC number aids fraud prevention in Mail Order and Internet payments.  Business rules are available on your account to identify whether to accept or decline transactions based on mismatched results of the CSC.  The Payment Card Industry (PCI) requires that at no stage of a transaction should the CSC be stored.  This applies to all entities handling card data.  It should also not be used in any hashing process.  CityPay do not store the value and have no method of retrieving the value once the transaction has been processed. For this reason, duplicate checking is unable to determine the CSC in its duplication check algorithm. ")
+    csc_policy: Optional[StrictStr] = Field(default=None, description="A policy value which determines whether a CSC policy is enforced or bypassed.  Values are:   `0` for the default policy (default value if not supplied). Your default values are determined by your account manager on setup of the account.   `1` for an enforced policy. Transactions that are enforced will be rejected if the CSC value does not match.   `2` to bypass. Transactions that are bypassed will be allowed through even if the CSC did not match.   `3` to ignore. Transactions that are ignored will bypass the result and not send the CSC details for authorisation. ")
+    currency: Optional[Annotated[str, Field(min_length=3, strict=True, max_length=3)]] = Field(default=None, description="The processing currency for the transaction. Will default to the merchant account currency.")
+    duplicate_policy: Optional[StrictStr] = Field(default=None, description="A policy value which determines whether a duplication policy is enforced or bypassed. A duplication check has a window of time set against your account within which it can action. If a previous transaction with matching values occurred within the window, any subsequent transaction will result in a T001 result.  Values are   `0` for the default policy (default value if not supplied). Your default values are determined by your account manager on setup of the account.   `1` for an enforced policy. Transactions that are enforced will be checked for duplication within the duplication window.   `2` to bypass. Transactions that are bypassed will not be checked for duplication within the duplication window.   `3` to ignore. Transactions that are ignored will have the same affect as bypass. ")
+    event_management: Optional[EventDataModel] = None
+    expmonth: Annotated[int, Field(le=12, strict=True, ge=1)] = Field(description="The month of expiry of the card. The month value should be a numerical value between 1 and 12. ")
+    expyear: Annotated[int, Field(le=2100, strict=True, ge=2000)] = Field(description="The year of expiry of the card. ")
+    external_mpi: Optional[ExternalMPI] = None
+    identifier: Annotated[str, Field(min_length=4, strict=True, max_length=50)] = Field(description="The identifier of the transaction to process. The value should be a valid reference and may be used to perform  post processing actions and to aid in reconciliation of transactions.  The value should be a valid printable string with ASCII character ranges from 0x32 to 0x127.  The identifier is recommended to be distinct for each transaction such as a [random unique identifier](https://en.wikipedia.org/wiki/Universally_unique_identifier) this will aid in ensuring each transaction is identifiable.  When transactions are processed they are also checked for duplicate requests. Changing the identifier on a subsequent request will ensure that a transaction is considered as different. ")
+    match_avsa: Optional[StrictStr] = Field(default=None, description="A policy value which determines whether an AVS address policy is enforced, bypassed or ignored.  Values are:   `0` for the default policy (default value if not supplied). Your default values are determined by your account manager on setup of the account.   `1` for an enforced policy. Transactions that are enforced will be rejected if the AVS address numeric value does not match.   `2` to bypass. Transactions that are bypassed will be allowed through even if the address did not match.   `3` to ignore. Transactions that are ignored will bypass the result and not send address numeric details for authorisation. ")
+    mcc6012: Optional[MCC6012] = None
+    merchantid: StrictInt = Field(description="Identifies the merchant account to perform processing for.")
+    name_on_card: Optional[Annotated[str, Field(min_length=2, strict=True, max_length=45)]] = Field(default=None, description="The card holder name as appears on the card such as MR N E BODY. Required for some acquirers. ")
+    ship_to: Optional[ContactDetails] = None
+    tag: Optional[List[StrictStr]] = None
+    threedsecure: Optional[ThreeDSecure] = None
+    trans_info: Optional[Annotated[str, Field(strict=True, max_length=50)]] = Field(default=None, description="Further information that can be added to the transaction will display in reporting. Can be used for flexible values such as operator id.")
+    trans_type: Optional[Annotated[str, Field(strict=True, max_length=1)]] = Field(default=None, description="The type of transaction being submitted. Normally this value is not required and your account manager may request that you set this field.")
+    __properties: ClassVar[List[str]] = ["airline_data", "amount", "avs_postcode_policy", "bill_to", "cardnumber", "csc", "csc_policy", "currency", "duplicate_policy", "event_management", "expmonth", "expyear", "external_mpi", "identifier", "match_avsa", "mcc6012", "merchantid", "name_on_card", "ship_to", "tag", "threedsecure", "trans_info", "trans_type"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
     }
 
-    validations = {
-        ('code',): {
-            'max_length': 4,
-            'min_length': 3,
-        },
-        ('identifier',): {
-            'max_length': 50,
-            'min_length': 4,
-        },
-    }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
 
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'code': (str,),  # noqa: E501
-            'context': (str,),  # noqa: E501
-            'identifier': (str,),  # noqa: E501
-            'message': (str,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'code': 'code',  # noqa: E501
-        'context': 'context',  # noqa: E501
-        'identifier': 'identifier',  # noqa: E501
-        'message': 'message',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of AuthRequest from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude={
+            },
+            exclude_none=True,
+        )
+        # override the default output from pydantic by calling `to_dict()` of airline_data
+        if self.airline_data:
+            _dict['airline_data'] = self.airline_data.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of bill_to
+        if self.bill_to:
+            _dict['bill_to'] = self.bill_to.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of event_management
+        if self.event_management:
+            _dict['event_management'] = self.event_management.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of external_mpi
+        if self.external_mpi:
+            _dict['external_mpi'] = self.external_mpi.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of mcc6012
+        if self.mcc6012:
+            _dict['mcc6012'] = self.mcc6012.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of ship_to
+        if self.ship_to:
+            _dict['ship_to'] = self.ship_to.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of threedsecure
+        if self.threedsecure:
+            _dict['threedsecure'] = self.threedsecure.to_dict()
+        return _dict
 
     @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Acknowledgement - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            code (str): A response code providing a result of the process.. [optional]  # noqa: E501
-            context (str): A context id of the process used for referencing transactions through support.. [optional]  # noqa: E501
-            identifier (str): An identifier if presented in the original request.. [optional]  # noqa: E501
-            message (str): A response message providing a description of the result of the process.. [optional]  # noqa: E501
-        """
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of AuthRequest from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
+
+        _obj = cls.model_validate({
+            "airline_data": AirlineAdvice.from_dict(obj.get("airline_data")) if obj.get("airline_data") is not None else None,
+            "amount": obj.get("amount"),
+            "avs_postcode_policy": obj.get("avs_postcode_policy"),
+            "bill_to": ContactDetails.from_dict(obj.get("bill_to")) if obj.get("bill_to") is not None else None,
+            "cardnumber": obj.get("cardnumber"),
+            "csc": obj.get("csc"),
+            "csc_policy": obj.get("csc_policy"),
+            "currency": obj.get("currency"),
+            "duplicate_policy": obj.get("duplicate_policy"),
+            "event_management": EventDataModel.from_dict(obj.get("event_management")) if obj.get("event_management") is not None else None,
+            "expmonth": obj.get("expmonth"),
+            "expyear": obj.get("expyear"),
+            "external_mpi": ExternalMPI.from_dict(obj.get("external_mpi")) if obj.get("external_mpi") is not None else None,
+            "identifier": obj.get("identifier"),
+            "match_avsa": obj.get("match_avsa"),
+            "mcc6012": MCC6012.from_dict(obj.get("mcc6012")) if obj.get("mcc6012") is not None else None,
+            "merchantid": obj.get("merchantid"),
+            "name_on_card": obj.get("name_on_card"),
+            "ship_to": ContactDetails.from_dict(obj.get("ship_to")) if obj.get("ship_to") is not None else None,
+            "tag": obj.get("tag"),
+            "threedsecure": ThreeDSecure.from_dict(obj.get("threedsecure")) if obj.get("threedsecure") is not None else None,
+            "trans_info": obj.get("trans_info"),
+            "trans_type": obj.get("trans_type")
+        })
+        return _obj
 
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """Acknowledgement - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            code (str): A response code providing a result of the process.. [optional]  # noqa: E501
-            context (str): A context id of the process used for referencing transactions through support.. [optional]  # noqa: E501
-            identifier (str): An identifier if presented in the original request.. [optional]  # noqa: E501
-            message (str): A response message providing a description of the result of the process.. [optional]  # noqa: E501
-        """
 
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `citypay_api_client-1.1.1/citypay/model/api_key.py` & `citypay_api_client-1.1.4/citypay/models/api_key.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/citypay/model/batch_report_response_model.py` & `citypay_api_client-1.1.4/citypay/models/charge_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,314 +1,124 @@
+# coding: utf-8
+
 """
     CityPay Payment API
 
-     This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security Your application will need to adhere to PCI-DSS standards to operate safely and to meet requirements set out by  Visa and MasterCard and the PCI Security Standards Council. These include  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
+     Welcome to the CityPay API, a robust HTTP API payment solution designed for seamless server-to-server  transactional processing. Our API facilitates a wide array of payment operations, catering to diverse business needs.  Whether you're integrating Internet payments, handling Mail Order/Telephone Order (MOTO) transactions, managing  Subscriptions with Recurring and Continuous Authority payments, or navigating the complexities of 3-D Secure  authentication, our API is equipped to support your requirements. Additionally, we offer functionalities for  Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids, and Completion processing, alongside the capability  for tokenised payments.  ## Compliance and Security Overview <aside class=\"notice\">   Ensuring the security of payment transactions and compliance with industry standards is paramount. Our API is    designed with stringent security measures and compliance protocols to safeguard sensitive information and meet    the rigorous requirements of Visa, MasterCard, and the PCI Security Standards Council. </aside>  ### Key Compliance and Security Measures  * **TLS Encryption**: All data transmissions must utilise TLS version 1.2 or higher, employing [strong cryptography](#enabled-tls-ciphers). Our infrastructure strictly enforces this requirement to maintain the integrity and confidentiality of data in transit. We conduct regular scans and assessments of our TLS endpoints to identify and mitigate vulnerabilities. * **Data Storage Prohibitions**: Storing sensitive cardholder data (CHD), such as the card security code (CSC) or primary account number (PAN), is strictly prohibited. Our API is designed to minimize your exposure to sensitive data, thereby reducing your compliance burden. * **Data Masking**: For consumer protection and compliance, full card numbers must not be displayed on receipts or any customer-facing materials. Our API automatically masks PANs, displaying only the last four digits to facilitate safe receipt generation. * **Network Scans**: If your application is web-based, regular scans of your hosting environment are mandatory to identify and rectify potential vulnerabilities. This proactive measure is crucial for maintaining a secure and compliant online presence. * **PCI Compliance**: Adherence to PCI DSS standards is not optional; it's a requirement for operating securely and legally in the payments ecosystem. For detailed information on compliance requirements and resources, please visit the PCI Security Standards Council website [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/). * **Request Validation**: Our API includes mechanisms to verify the legitimacy of each request, ensuring it pertains to a valid account and originates from a trusted source. We leverage remote IP address verification alongside sophisticated application firewall technologies to thwart a wide array of common security threats.  ## Getting Started Before integrating with the CityPay API, ensure your application and development practices align with the outlined compliance and security measures. This preparatory step is crucial for a smooth integration process and the long-term success of your payment processing operations.  For further details on API endpoints, request/response formats, and code examples, proceed to the subsequent sections of our documentation. Our aim is to provide you with all the necessary tools and information to integrate our payment processing capabilities seamlessly into your application.  Thank you for choosing CityPay API. We look forward to supporting your payment processing needs with our secure, compliant, and versatile API solution. 
 
     Contact: support@citypay.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
+
+from __future__ import annotations
+import pprint
 import re  # noqa: F401
-import sys  # noqa: F401
+import json
 
-from citypay.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from citypay.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from citypay.model.batch_transaction_result_model import BatchTransactionResultModel
-    globals()['BatchTransactionResultModel'] = BatchTransactionResultModel
-
-
-class BatchReportResponseModel(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import Field
+from typing_extensions import Annotated
+from citypay.models.three_d_secure import ThreeDSecure
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
 
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
+class ChargeRequest(BaseModel):
     """
-
-    allowed_values = {
-    }
-
-    validations = {
-        ('amount',): {
-        },
-        ('batch_id',): {
-            'inclusive_minimum': 1,
-        },
-        ('client_account_id',): {
-            'max_length': 20,
-            'min_length': 3,
-        },
+    ChargeRequest
+    """ # noqa: E501
+    amount: Annotated[int, Field(strict=True)] = Field(description="The amount to authorise in the lowest unit of currency with a variable length to a maximum of 12 digits.  No decimal points are to be included and no divisional characters such as 1,024.  The amount should be the total amount required for the transaction.  For example with GBP £1,021.95 the amount value is 102195. ")
+    avs_postcode_policy: Optional[StrictStr] = Field(default=None, description="A policy value which determines whether an AVS postcode policy is enforced or bypassed.  Values are:   `0` for the default policy (default value if not supplied). Your default values are determined by your account manager on setup of the account.   `1` for an enforced policy. Transactions that are enforced will be rejected if the AVS postcode numeric value does not match.   `2` to bypass. Transactions that are bypassed will be allowed through even if the postcode did not match.   `3` to ignore. Transactions that are ignored will bypass the result and not send postcode details for authorisation. ")
+    cardholder_agreement: Optional[Annotated[str, Field(strict=True, max_length=1)]] = Field(default=None, description="Merchant-initiated transactions (MITs) are payments you trigger, where the cardholder has previously consented to you carrying out such payments. These may be scheduled (such as recurring payments and installments) or unscheduled (like account top-ups triggered by balance thresholds and no-show charges).  Scheduled --- These are regular payments using stored card details, like installments or a monthly subscription fee.  - `I` Instalment - A single purchase of goods or services billed to a cardholder in multiple transactions, over a period of time agreed by the cardholder and you.  - `R` Recurring - Transactions processed at fixed, regular intervals not to exceed one year between transactions, representing an agreement between a cardholder and you to purchase goods or services provided over a period of time.  Unscheduled --- These are payments using stored card details that do not occur on a regular schedule, like top-ups for a digital wallet triggered by the balance falling below a certain threshold.  - `A` Reauthorisation - a purchase made after the original purchase. A common scenario is delayed/split shipments.  - `C` Unscheduled Payment - A transaction using a stored credential for a fixed or variable amount that does not occur on a scheduled or regularly occurring transaction date. This includes account top-ups triggered by balance thresholds.  - `D` Delayed Charge - A delayed charge is typically used in hotel, cruise lines and vehicle rental environments to perform a supplemental account charge after original services are rendered.  - `L` Incremental - An incremental authorisation is typically found in hotel and car rental environments, where the cardholder has agreed to pay for any service incurred during the duration of the contract. An incremental authorisation is where you need to seek authorisation of further funds in addition to what you have originally requested. A common scenario is additional services charged to the contract, such as extending a stay in a hotel.  - `S` Resubmission - When the original purchase occurred, but you were not able to get authorisation at the time the goods or services were provided. It should be only used where the goods or services have already been provided, but the authorisation request is declined for insufficient funds.  - `X` No-show - A no-show is a transaction where you are enabled to charge for services which the cardholder entered into an agreement to purchase, but the cardholder did not meet the terms of the agreement. ")
+    csc: Optional[Annotated[str, Field(min_length=3, strict=True, max_length=4)]] = Field(default=None, description="The Card Security Code (CSC) (also known as CV2/CVV2) is normally found on the back of the card (American Express has it on the front). The value helps to identify possession of the card as it is not available within the chip or magnetic swipe.  When forwarding the CSC, please ensure the value is a string as some values start with 0 and this will be stripped out by any integer parsing.  The CSC number aids fraud prevention in Mail Order and Internet payments.  Business rules are available on your account to identify whether to accept or decline transactions based on mismatched results of the CSC.  The Payment Card Industry (PCI) requires that at no stage of a transaction should the CSC be stored.  This applies to all entities handling card data.  It should also not be used in any hashing process.  CityPay do not store the value and have no method of retrieving the value once the transaction has been processed. For this reason, duplicate checking is unable to determine the CSC in its duplication check algorithm. ")
+    csc_policy: Optional[StrictStr] = Field(default=None, description="A policy value which determines whether a CSC policy is enforced or bypassed.  Values are:   `0` for the default policy (default value if not supplied). Your default values are determined by your account manager on setup of the account.   `1` for an enforced policy. Transactions that are enforced will be rejected if the CSC value does not match.   `2` to bypass. Transactions that are bypassed will be allowed through even if the CSC did not match.   `3` to ignore. Transactions that are ignored will bypass the result and not send the CSC details for authorisation. ")
+    currency: Optional[Annotated[str, Field(min_length=3, strict=True, max_length=3)]] = Field(default=None, description="The processing currency for the transaction. Will default to the merchant account currency.")
+    duplicate_policy: Optional[StrictStr] = Field(default=None, description="A policy value which determines whether a duplication policy is enforced or bypassed. A duplication check has a window of time set against your account within which it can action. If a previous transaction with matching values occurred within the window, any subsequent transaction will result in a T001 result.  Values are   `0` for the default policy (default value if not supplied). Your default values are determined by your account manager on setup of the account.   `1` for an enforced policy. Transactions that are enforced will be checked for duplication within the duplication window.   `2` to bypass. Transactions that are bypassed will not be checked for duplication within the duplication window.   `3` to ignore. Transactions that are ignored will have the same affect as bypass. ")
+    identifier: Annotated[str, Field(min_length=4, strict=True, max_length=50)] = Field(description="The identifier of the transaction to process. The value should be a valid reference and may be used to perform  post processing actions and to aid in reconciliation of transactions.  The value should be a valid printable string with ASCII character ranges from 0x32 to 0x127.  The identifier is recommended to be distinct for each transaction such as a [random unique identifier](https://en.wikipedia.org/wiki/Universally_unique_identifier) this will aid in ensuring each transaction is identifiable.  When transactions are processed they are also checked for duplicate requests. Changing the identifier on a subsequent request will ensure that a transaction is considered as different. ")
+    initiation: Optional[Annotated[str, Field(strict=True, max_length=1)]] = Field(default=None, description="Transactions charged using the API are defined as:  **Cardholder Initiated**: A _cardholder initiated transaction_ (CIT) is where the cardholder selects the card for use for a purchase using previously stored details. An example would be a customer buying an item from your website after being present with their saved card details at checkout.  **Merchant Intiated**: A _merchant initiated transaction_ (MIT) is an authorisation initiated where you as the  merchant submit a cardholders previously stored details without the cardholder's participation. An example would  be a subscription to a membership scheme to debit their card monthly.  MITs have different reasons such as reauthorisation, delayed, unscheduled, incremental, recurring, instalment, no-show or resubmission.  The following values apply   - `M` - specifies that the transaction is initiated by the merchant   - `C` - specifies that the transaction is initiated by the cardholder  Where transactions are merchant initiated, a valid cardholder agreement must be defined. ")
+    match_avsa: Optional[StrictStr] = Field(default=None, description="A policy value which determines whether an AVS address policy is enforced, bypassed or ignored.  Values are:   `0` for the default policy (default value if not supplied). Your default values are determined by your account manager on setup of the account.   `1` for an enforced policy. Transactions that are enforced will be rejected if the AVS address numeric value does not match.   `2` to bypass. Transactions that are bypassed will be allowed through even if the address did not match.   `3` to ignore. Transactions that are ignored will bypass the result and not send address numeric details for authorisation. ")
+    merchantid: StrictInt = Field(description="Identifies the merchant account to perform processing for.")
+    tag: Optional[List[StrictStr]] = None
+    threedsecure: Optional[ThreeDSecure] = None
+    token: StrictStr = Field(description="A tokenised form of a card that belongs to a card holder's account and that has been previously registered. The token is time based and will only be active for a short duration. The value is therefore designed not to be stored remotely for future use.   Tokens will start with ct and are resiliently tamper proof using HMacSHA-256. No sensitive card data is stored internally within the token.   Each card will contain a different token and the value may be different on any retrieval call.   The value can be presented for payment as a selection value to an end user in a web application. ")
+    trans_info: Optional[Annotated[str, Field(strict=True, max_length=50)]] = Field(default=None, description="Further information that can be added to the transaction will display in reporting. Can be used for flexible values such as operator id.")
+    trans_type: Optional[Annotated[str, Field(strict=True, max_length=1)]] = Field(default=None, description="The type of transaction being submitted. Normally this value is not required and your account manager may request that you set this field.")
+    __properties: ClassVar[List[str]] = ["amount", "avs_postcode_policy", "cardholder_agreement", "csc", "csc_policy", "currency", "duplicate_policy", "identifier", "initiation", "match_avsa", "merchantid", "tag", "threedsecure", "token", "trans_info", "trans_type"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'amount': (int,),  # noqa: E501
-            'batch_date': (date,),  # noqa: E501
-            'batch_id': (int,),  # noqa: E501
-            'batch_status': (str,),  # noqa: E501
-            'client_account_id': (str,),  # noqa: E501
-            'transactions': ([BatchTransactionResultModel],),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'amount': 'amount',  # noqa: E501
-        'batch_date': 'batch_date',  # noqa: E501
-        'batch_id': 'batch_id',  # noqa: E501
-        'batch_status': 'batch_status',  # noqa: E501
-        'client_account_id': 'client_account_id',  # noqa: E501
-        'transactions': 'transactions',  # noqa: E501
-    }
 
-    read_only_vars = {
-    }
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
 
-    _composed_schemas = {}
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of ChargeRequest from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude={
+            },
+            exclude_none=True,
+        )
+        # override the default output from pydantic by calling `to_dict()` of threedsecure
+        if self.threedsecure:
+            _dict['threedsecure'] = self.threedsecure.to_dict()
+        return _dict
 
     @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, amount, batch_date, batch_id, batch_status, client_account_id, transactions, *args, **kwargs):  # noqa: E501
-        """BatchReportResponseModel - a model defined in OpenAPI
-
-        Args:
-            amount (int): The total amount that the batch contains.
-            batch_date (date): The date and time of the batch in ISO-8601 format.
-            batch_id (int): The batch id specified in the batch processing request.
-            batch_status (str): The status of the batch. Possible values are - CANCELLED. The file has been cancelled by an administrator or server process.  - COMPLETE. The file has passed through the processing cycle and is determined as being complete further information should be obtained on the results of the processing - ERROR_IN_PROCESSING. Errors have occurred in the processing that has deemed that processing can not continue. - INITIALISED. The file has been initialised and no action has yet been performed - LOCKED. The file has been locked for processing - QUEUED. The file has been queued for processing yet no processing has yet been performed - UNKNOWN. The file is of an unknown status, that is the file can either not be determined by the information requested of the file has not yet been received. 
-            client_account_id (str): The batch account id that the batch was processed with.
-            transactions ([BatchTransactionResultModel]):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of ChargeRequest from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
+
+        _obj = cls.model_validate({
+            "amount": obj.get("amount"),
+            "avs_postcode_policy": obj.get("avs_postcode_policy"),
+            "cardholder_agreement": obj.get("cardholder_agreement"),
+            "csc": obj.get("csc"),
+            "csc_policy": obj.get("csc_policy"),
+            "currency": obj.get("currency"),
+            "duplicate_policy": obj.get("duplicate_policy"),
+            "identifier": obj.get("identifier"),
+            "initiation": obj.get("initiation"),
+            "match_avsa": obj.get("match_avsa"),
+            "merchantid": obj.get("merchantid"),
+            "tag": obj.get("tag"),
+            "threedsecure": ThreeDSecure.from_dict(obj.get("threedsecure")) if obj.get("threedsecure") is not None else None,
+            "token": obj.get("token"),
+            "trans_info": obj.get("trans_info"),
+            "trans_type": obj.get("trans_type")
+        })
+        return _obj
 
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.amount = amount
-        self.batch_date = batch_date
-        self.batch_id = batch_id
-        self.batch_status = batch_status
-        self.client_account_id = client_account_id
-        self.transactions = transactions
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, amount, batch_date, batch_id, batch_status, client_account_id, transactions, *args, **kwargs):  # noqa: E501
-        """BatchReportResponseModel - a model defined in OpenAPI
-
-        Args:
-            amount (int): The total amount that the batch contains.
-            batch_date (date): The date and time of the batch in ISO-8601 format.
-            batch_id (int): The batch id specified in the batch processing request.
-            batch_status (str): The status of the batch. Possible values are - CANCELLED. The file has been cancelled by an administrator or server process.  - COMPLETE. The file has passed through the processing cycle and is determined as being complete further information should be obtained on the results of the processing - ERROR_IN_PROCESSING. Errors have occurred in the processing that has deemed that processing can not continue. - INITIALISED. The file has been initialised and no action has yet been performed - LOCKED. The file has been locked for processing - QUEUED. The file has been queued for processing yet no processing has yet been performed - UNKNOWN. The file is of an unknown status, that is the file can either not be determined by the information requested of the file has not yet been received. 
-            client_account_id (str): The batch account id that the batch was processed with.
-            transactions ([BatchTransactionResultModel]):
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-        """
 
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.amount = amount
-        self.batch_date = batch_date
-        self.batch_id = batch_id
-        self.batch_status = batch_status
-        self.client_account_id = client_account_id
-        self.transactions = transactions
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `citypay_api_client-1.1.1/citypay/model/batch_transaction_result_model.py` & `citypay_api_client-1.1.4/citypay/models/auth_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,333 +1,145 @@
+# coding: utf-8
+
 """
     CityPay Payment API
 
-     This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security Your application will need to adhere to PCI-DSS standards to operate safely and to meet requirements set out by  Visa and MasterCard and the PCI Security Standards Council. These include  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
+     Welcome to the CityPay API, a robust HTTP API payment solution designed for seamless server-to-server  transactional processing. Our API facilitates a wide array of payment operations, catering to diverse business needs.  Whether you're integrating Internet payments, handling Mail Order/Telephone Order (MOTO) transactions, managing  Subscriptions with Recurring and Continuous Authority payments, or navigating the complexities of 3-D Secure  authentication, our API is equipped to support your requirements. Additionally, we offer functionalities for  Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids, and Completion processing, alongside the capability  for tokenised payments.  ## Compliance and Security Overview <aside class=\"notice\">   Ensuring the security of payment transactions and compliance with industry standards is paramount. Our API is    designed with stringent security measures and compliance protocols to safeguard sensitive information and meet    the rigorous requirements of Visa, MasterCard, and the PCI Security Standards Council. </aside>  ### Key Compliance and Security Measures  * **TLS Encryption**: All data transmissions must utilise TLS version 1.2 or higher, employing [strong cryptography](#enabled-tls-ciphers). Our infrastructure strictly enforces this requirement to maintain the integrity and confidentiality of data in transit. We conduct regular scans and assessments of our TLS endpoints to identify and mitigate vulnerabilities. * **Data Storage Prohibitions**: Storing sensitive cardholder data (CHD), such as the card security code (CSC) or primary account number (PAN), is strictly prohibited. Our API is designed to minimize your exposure to sensitive data, thereby reducing your compliance burden. * **Data Masking**: For consumer protection and compliance, full card numbers must not be displayed on receipts or any customer-facing materials. Our API automatically masks PANs, displaying only the last four digits to facilitate safe receipt generation. * **Network Scans**: If your application is web-based, regular scans of your hosting environment are mandatory to identify and rectify potential vulnerabilities. This proactive measure is crucial for maintaining a secure and compliant online presence. * **PCI Compliance**: Adherence to PCI DSS standards is not optional; it's a requirement for operating securely and legally in the payments ecosystem. For detailed information on compliance requirements and resources, please visit the PCI Security Standards Council website [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/). * **Request Validation**: Our API includes mechanisms to verify the legitimacy of each request, ensuring it pertains to a valid account and originates from a trusted source. We leverage remote IP address verification alongside sophisticated application firewall technologies to thwart a wide array of common security threats.  ## Getting Started Before integrating with the CityPay API, ensure your application and development practices align with the outlined compliance and security measures. This preparatory step is crucial for a smooth integration process and the long-term success of your payment processing operations.  For further details on API endpoints, request/response formats, and code examples, proceed to the subsequent sections of our documentation. Our aim is to provide you with all the necessary tools and information to integrate our payment processing capabilities seamlessly into your application.  Thank you for choosing CityPay API. We look forward to supporting your payment processing needs with our secure, compliant, and versatile API solution. 
 
     Contact: support@citypay.com
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from citypay.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from citypay.exceptions import ApiAttributeError
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
-class BatchTransactionResultModel(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-    Do not edit the class manually.
+from datetime import datetime as DateTime
+from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, StrictBool, StrictInt, StrictStr
+from pydantic import Field
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
 
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
+class AuthResponse(BaseModel):
     """
-
-    allowed_values = {
-    }
-
-    validations = {
-        ('account_id',): {
-            'max_length': 50,
-            'min_length': 5,
-        },
-        ('identifier',): {
-            'max_length': 50,
-            'min_length': 4,
-        },
-        ('amount',): {
-        },
+    AuthResponse
+    """ # noqa: E501
+    amount: Optional[StrictInt] = Field(default=None, description="The amount of the transaction processed.")
+    atrn: Optional[StrictStr] = Field(default=None, description="A reference number provided by the acquirer for a transaction it can be used to cross reference transactions with an Acquirers reporting panel. ")
+    atsd: Optional[StrictStr] = Field(default=None, description="Additional Transaction Security Data used for ecommerce transactions to decipher security capabilities and attempts against a transaction.")
+    authcode: Optional[StrictStr] = Field(default=None, description="The authorisation code as returned by the card issuer or acquiring bank when a transaction has successfully   been authorised. Authorisation codes contain alphanumeric values. Whilst the code confirms authorisation it   should not be used to determine whether a transaction was successfully processed. For instance an auth code   may be returned when a transaction has been subsequently declined due to a CSC mismatch. ")
+    authen_result: Optional[StrictStr] = Field(default=None, description="The result of any authentication using 3d_secure authorisation against ecommerce transactions. Values are:  <table> <tr> <th>Value</th> <th>Description</th> </tr> <tr> <td>Y</td> <td>Authentication Successful. The Cardholder's password was successfully validated.</td> </tr> <tr> <td>N</td> <td>Authentication Failed. Customer failed or cancelled authentication, transaction denied.</td> </tr> <tr> <td>A</td> <td>Attempts Processing Performed Authentication could not be completed but a proof of authentication attempt (CAVV) was generated.</td> </tr> <tr> <td>U</td> <td>Authentication Could Not Be Performed Authentication could not be completed, due to technical or other problem.</td> </tr> </table> ")
+    authorised: Optional[StrictBool] = Field(default=None, description="A boolean definition that indicates that the transaction was authorised. It will return false if the transaction  was declined, rejected or cancelled due to CSC matching failures.  Attention should be referenced to the AuthResult and Response code for accurate determination of the result. ")
+    avs_result: Optional[StrictStr] = Field(default=None, description="The AVS result codes determine the result of checking the AVS values within the Address Verification fraud system. If a transaction is declined due to the AVS code not matching, this value can help determine the reason for the decline.  <table> <tr> <th>Code</th> <th>Description</th> </tr> <tr><td>Y</td><td>Address and 5 digit post code match</td></tr> <tr><td>M</td><td>Street address and Postal codes match for international transaction</td></tr> <tr><td>U</td><td>No AVS data available from issuer auth system</td></tr> <tr><td>A</td><td>Addres matches, post code does not</td></tr> <tr><td>I</td><td>Address information verified for international transaction</td></tr> <tr><td>Z</td><td>5 digit post code matches, Address does not</td></tr> <tr><td>W</td><td>9 digit post code matches, Address does not</td></tr> <tr><td>X</td><td>Postcode and address match</td></tr> <tr><td>B</td><td>Postal code not verified due to incompatible formats</td></tr> <tr><td>P</td><td>Postal codes match. Street address not verified due to to incompatible formats</td></tr> <tr><td>E</td><td>AVS Error</td></tr> <tr><td>C</td><td>Street address and Postal code not verified due to incompatible formats</td></tr> <tr><td>D</td><td>Street address and postal codes match</td></tr> <tr><td> </td><td>No information</td></tr> <tr><td>N</td><td>Neither postcode nor address match</td></tr> <tr><td>R</td><td>Retry, System unavailble or Timed Out</td></tr> <tr><td>S</td><td>AVS Service not supported by issuer or processor</td></tr> <tr><td>G</td><td>Issuer does not participate in AVS</td></tr> </table> ")
+    bin_commercial: Optional[StrictBool] = Field(default=None, description="Determines whether the bin range was found to be a commercial or business card.")
+    bin_debit: Optional[StrictBool] = Field(default=None, description="Determines whether the bin range was found to be a debit card. If false the card was considered as a credit card.")
+    bin_description: Optional[StrictStr] = Field(default=None, description="A description of the bin range found for the card.")
+    cavv: Optional[StrictStr] = Field(default=None, description="The cardholder authentication verification value which can be returned for verification purposes of the authenticated  transaction for dispute realisation. ")
+    context: Optional[StrictStr] = Field(default=None, description="The context which processed the transaction, can be used for support purposes to trace transactions.")
+    csc_result: Optional[StrictStr] = Field(default=None, description="The CSC result codes determine the result of checking the provided CSC value within the Card Security Code fraud system. If a transaction is declined due to the CSC code not matching, this value can help determine the reason for the decline.  <table> <tr> <th>Code</th> <th>Description</th> </tr> <tr><td> </td><td>No information</td></tr> <tr><td>M</td><td>Card verification data matches</td></tr> <tr><td>N</td><td>Card verification data was checked but did not match</td></tr> <tr><td>P</td><td>Card verification was not processed</td></tr> <tr><td>S</td><td>The card verification data should be on the card but the merchant indicates that it is not</td></tr> <tr><td>U</td><td>The card issuer is not certified</td></tr> </table> ")
+    currency: Optional[StrictStr] = Field(default=None, description="The currency the transaction was processed in. This is an `ISO4217` alpha currency value.")
+    datetime: Optional[DateTime] = Field(default=None, description="The UTC date time of the transaction in ISO data time format. ")
+    eci: Optional[StrictStr] = Field(default=None, description="An Electronic Commerce Indicator (ECI) used to identify the result of authentication using 3DSecure. ")
+    identifier: Optional[StrictStr] = Field(default=None, description="The identifier provided within the request.")
+    live: Optional[StrictBool] = Field(default=None, description="Used to identify that a transaction was processed on a live authorisation platform.")
+    maskedpan: Optional[StrictStr] = Field(default=None, description="A masked value of the card number used for processing displaying limited values that can be used on a receipt. ")
+    merchantid: StrictInt = Field(description="The merchant id that processed this transaction.")
+    result: StrictInt = Field(description="An integer result that indicates the outcome of the transaction. The Code value below maps to the result value  <table> <tr> <th>Code</th> <th>Abbrev</th> <th>Description</th> </tr> <tr><td>0</td><td>Declined</td><td>Declined</td></tr> <tr><td>1</td><td>Accepted</td><td>Accepted</td></tr> <tr><td>2</td><td>Rejected</td><td>Rejected</td></tr> <tr><td>3</td><td>Not Attempted</td><td>Not Attempted</td></tr> <tr><td>4</td><td>Referred</td><td>Referred</td></tr> <tr><td>5</td><td>PinRetry</td><td>Perform PIN Retry</td></tr> <tr><td>6</td><td>ForSigVer</td><td>Force Signature Verification</td></tr> <tr><td>7</td><td>Hold</td><td>Hold</td></tr> <tr><td>8</td><td>SecErr</td><td>Security Error</td></tr> <tr><td>9</td><td>CallAcq</td><td>Call Acquirer</td></tr> <tr><td>10</td><td>DNH</td><td>Do Not Honour</td></tr> <tr><td>11</td><td>RtnCrd</td><td>Retain Card</td></tr> <tr><td>12</td><td>ExprdCrd</td><td>Expired Card</td></tr> <tr><td>13</td><td>InvldCrd</td><td>Invalid Card No</td></tr> <tr><td>14</td><td>PinExcd</td><td>Pin Tries Exceeded</td></tr> <tr><td>15</td><td>PinInvld</td><td>Pin Invalid</td></tr> <tr><td>16</td><td>AuthReq</td><td>Authentication Required</td></tr> <tr><td>17</td><td>AuthenFail</td><td>Authentication Failed</td></tr> <tr><td>18</td><td>Verified</td><td>Card Verified</td></tr> <tr><td>19</td><td>Cancelled</td><td>Cancelled</td></tr> <tr><td>20</td><td>Un</td><td>Unknown</td></tr> <tr><td>21</td><td>Challenged</td><td>Challenged</td></tr> <tr><td>22</td><td>Decoupled</td><td>Decoupled</td></tr> <tr><td>23</td><td>Denied</td><td>Permission Denied</td></tr> </table> ")
+    result_code: StrictStr = Field(description="The result code as defined in the Response Codes Reference for example 000 is an accepted live transaction whilst 001 is an accepted test transaction. Result codes identify the source of success and failure.  Codes may start with an alpha character i.e. C001 indicating a type of error such as a card validation error. ")
+    result_message: StrictStr = Field(description="The message regarding the result which provides further narrative to the result code. ")
+    scheme: Optional[StrictStr] = Field(default=None, description="The name of the card scheme of the transaction that processed the transaction such as Visa or MasterCard. ")
+    scheme_id: Optional[StrictStr] = Field(default=None, description="The name of the card scheme of the transaction such as VI or MC. ")
+    scheme_logo: Optional[StrictStr] = Field(default=None, description="A url containing a logo of the card scheme. ")
+    sha256: Optional[StrictStr] = Field(default=None, description="A SHA256 digest value of the transaction used to validate the response data The digest is calculated by concatenating   * authcode   * amount   * response_code   * merchant_id   * trans_no   * identifier   * licence_key - which is not provided in the response. ")
+    trans_status: Optional[StrictStr] = Field(default=None, description="Used to identify the status of a transaction. The status is used to track a transaction through its life cycle.  <table> <tr> <th>Id</th> <th>Description</th> </tr> <tr> <td>O</td> <td>Transaction is open for settlement</td> </tr> <tr> <td>A</td> <td>Transaction is assigned for settlement and can no longer be voided</td> </tr> <tr> <td>S</td> <td>Transaction has been settled</td> </tr> <tr> <td>D</td> <td>Transaction has been declined</td> </tr> <tr> <td>R</td> <td>Transaction has been rejected</td> </tr> <tr> <td>P</td> <td>Transaction has been authorised only and awaiting a capture. Used in pre-auth situations</td> </tr> <tr> <td>C</td> <td>Transaction has been cancelled</td> </tr> <tr> <td>E</td> <td>Transaction has expired</td> </tr> <tr> <td>I</td> <td>Transaction has been initialised but no action was able to be carried out</td> </tr> <tr> <td>H</td> <td>Transaction is awaiting authorisation</td> </tr> <tr> <td>.</td> <td>Transaction is on hold</td> </tr> <tr> <td>V</td> <td>Transaction has been verified</td> </tr> </table> ")
+    transno: Optional[StrictInt] = Field(default=None, description="The resulting transaction number, ordered incrementally from 1 for every merchant_id. The value will default to less than 1 for transactions that do not have a transaction number issued. ")
+    __properties: ClassVar[List[str]] = ["amount", "atrn", "atsd", "authcode", "authen_result", "authorised", "avs_result", "bin_commercial", "bin_debit", "bin_description", "cavv", "context", "csc_result", "currency", "datetime", "eci", "identifier", "live", "maskedpan", "merchantid", "result", "result_code", "result_message", "scheme", "scheme_id", "scheme_logo", "sha256", "trans_status", "transno"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        return {
-            'account_id': (str,),  # noqa: E501
-            'identifier': (str,),  # noqa: E501
-            'merchantid': (int,),  # noqa: E501
-            'message': (str,),  # noqa: E501
-            'result': (int,),  # noqa: E501
-            'result_code': (str,),  # noqa: E501
-            'amount': (int,),  # noqa: E501
-            'authcode': (str,),  # noqa: E501
-            'datetime': (datetime,),  # noqa: E501
-            'maskedpan': (str,),  # noqa: E501
-            'scheme': (str,),  # noqa: E501
-            'transno': (int,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'account_id': 'account_id',  # noqa: E501
-        'identifier': 'identifier',  # noqa: E501
-        'merchantid': 'merchantid',  # noqa: E501
-        'message': 'message',  # noqa: E501
-        'result': 'result',  # noqa: E501
-        'result_code': 'result_code',  # noqa: E501
-        'amount': 'amount',  # noqa: E501
-        'authcode': 'authcode',  # noqa: E501
-        'datetime': 'datetime',  # noqa: E501
-        'maskedpan': 'maskedpan',  # noqa: E501
-        'scheme': 'scheme',  # noqa: E501
-        'transno': 'transno',  # noqa: E501
-    }
 
-    read_only_vars = {
-    }
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
 
-    _composed_schemas = {}
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of AuthResponse from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude={
+            },
+            exclude_none=True,
+        )
+        return _dict
 
     @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, account_id, identifier, merchantid, message, result, result_code, *args, **kwargs):  # noqa: E501
-        """BatchTransactionResultModel - a model defined in OpenAPI
-
-        Args:
-            account_id (str): The card holder account id used for the transaction.
-            identifier (str): The identifier of the transaction.
-            merchantid (int): The merchant id of the transaction.
-            message (str): A response message pertaining to the transaction.
-            result (int): An integer result that indicates the outcome of the transaction. The Code value below maps to the result value  <table> <tr> <th>Code</th> <th>Abbrev</th> <th>Description</th> </tr> <tr><td>0</td><td>Declined</td><td>Declined</td></tr> <tr><td>1</td><td>Accepted</td><td>Accepted</td></tr> <tr><td>2</td><td>Rejected</td><td>Rejected</td></tr> <tr><td>3</td><td>Not Attempted</td><td>Not Attempted</td></tr> <tr><td>4</td><td>Referred</td><td>Referred</td></tr> <tr><td>5</td><td>PinRetry</td><td>Perform PIN Retry</td></tr> <tr><td>6</td><td>ForSigVer</td><td>Force Signature Verification</td></tr> <tr><td>7</td><td>Hold</td><td>Hold</td></tr> <tr><td>8</td><td>SecErr</td><td>Security Error</td></tr> <tr><td>9</td><td>CallAcq</td><td>Call Acquirer</td></tr> <tr><td>10</td><td>DNH</td><td>Do Not Honour</td></tr> <tr><td>11</td><td>RtnCrd</td><td>Retain Card</td></tr> <tr><td>12</td><td>ExprdCrd</td><td>Expired Card</td></tr> <tr><td>13</td><td>InvldCrd</td><td>Invalid Card No</td></tr> <tr><td>14</td><td>PinExcd</td><td>Pin Tries Exceeded</td></tr> <tr><td>15</td><td>PinInvld</td><td>Pin Invalid</td></tr> <tr><td>16</td><td>AuthReq</td><td>Authentication Required</td></tr> <tr><td>17</td><td>AuthenFail</td><td>Authentication Failed</td></tr> <tr><td>18</td><td>Verified</td><td>Card Verified</td></tr> <tr><td>19</td><td>Cancelled</td><td>Cancelled</td></tr> <tr><td>20</td><td>Un</td><td>Unknown</td></tr> <tr><td>21</td><td>Challenged</td><td>Challenged</td></tr> <tr><td>22</td><td>Decoupled</td><td>Decoupled</td></tr> <tr><td>23</td><td>Denied</td><td>Permission Denied</td></tr> </table> 
-            result_code (str): A result code of the transaction identifying the result of the transaction for success, rejection or decline.
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            amount (int): The amount of the transaction processed.. [optional]  # noqa: E501
-            authcode (str): The authorisation code of a successful transaction.. [optional]  # noqa: E501
-            datetime (datetime): The datetime that the transaction was processed.. [optional]  # noqa: E501
-            maskedpan (str): A masked value of the card number used for processing displaying limited values that can be used on a receipt. . [optional]  # noqa: E501
-            scheme (str): A name of the card scheme of the transaction that processed the transaction such as Visa or MasterCard. . [optional]  # noqa: E501
-            transno (int): The resulting transaction number, ordered incrementally from 1 for every merchant_id. The value will default to less than 1 for transactions that do not have a transaction number issued. . [optional]  # noqa: E501
-        """
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of AuthResponse from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
+
+        _obj = cls.model_validate({
+            "amount": obj.get("amount"),
+            "atrn": obj.get("atrn"),
+            "atsd": obj.get("atsd"),
+            "authcode": obj.get("authcode"),
+            "authen_result": obj.get("authen_result"),
+            "authorised": obj.get("authorised"),
+            "avs_result": obj.get("avs_result"),
+            "bin_commercial": obj.get("bin_commercial"),
+            "bin_debit": obj.get("bin_debit"),
+            "bin_description": obj.get("bin_description"),
+            "cavv": obj.get("cavv"),
+            "context": obj.get("context"),
+            "csc_result": obj.get("csc_result"),
+            "currency": obj.get("currency"),
+            "datetime": obj.get("datetime"),
+            "eci": obj.get("eci"),
+            "identifier": obj.get("identifier"),
+            "live": obj.get("live"),
+            "maskedpan": obj.get("maskedpan"),
+            "merchantid": obj.get("merchantid"),
+            "result": obj.get("result"),
+            "result_code": obj.get("result_code"),
+            "result_message": obj.get("result_message"),
+            "scheme": obj.get("scheme"),
+            "scheme_id": obj.get("scheme_id"),
+            "scheme_logo": obj.get("scheme_logo"),
+            "sha256": obj.get("sha256"),
+            "trans_status": obj.get("trans_status"),
+            "transno": obj.get("transno")
+        })
+        return _obj
 
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.account_id = account_id
-        self.identifier = identifier
-        self.merchantid = merchantid
-        self.message = message
-        self.result = result
-        self.result_code = result_code
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, account_id, identifier, merchantid, message, result, result_code, *args, **kwargs):  # noqa: E501
-        """BatchTransactionResultModel - a model defined in OpenAPI
-
-        Args:
-            account_id (str): The card holder account id used for the transaction.
-            identifier (str): The identifier of the transaction.
-            merchantid (int): The merchant id of the transaction.
-            message (str): A response message pertaining to the transaction.
-            result (int): An integer result that indicates the outcome of the transaction. The Code value below maps to the result value  <table> <tr> <th>Code</th> <th>Abbrev</th> <th>Description</th> </tr> <tr><td>0</td><td>Declined</td><td>Declined</td></tr> <tr><td>1</td><td>Accepted</td><td>Accepted</td></tr> <tr><td>2</td><td>Rejected</td><td>Rejected</td></tr> <tr><td>3</td><td>Not Attempted</td><td>Not Attempted</td></tr> <tr><td>4</td><td>Referred</td><td>Referred</td></tr> <tr><td>5</td><td>PinRetry</td><td>Perform PIN Retry</td></tr> <tr><td>6</td><td>ForSigVer</td><td>Force Signature Verification</td></tr> <tr><td>7</td><td>Hold</td><td>Hold</td></tr> <tr><td>8</td><td>SecErr</td><td>Security Error</td></tr> <tr><td>9</td><td>CallAcq</td><td>Call Acquirer</td></tr> <tr><td>10</td><td>DNH</td><td>Do Not Honour</td></tr> <tr><td>11</td><td>RtnCrd</td><td>Retain Card</td></tr> <tr><td>12</td><td>ExprdCrd</td><td>Expired Card</td></tr> <tr><td>13</td><td>InvldCrd</td><td>Invalid Card No</td></tr> <tr><td>14</td><td>PinExcd</td><td>Pin Tries Exceeded</td></tr> <tr><td>15</td><td>PinInvld</td><td>Pin Invalid</td></tr> <tr><td>16</td><td>AuthReq</td><td>Authentication Required</td></tr> <tr><td>17</td><td>AuthenFail</td><td>Authentication Failed</td></tr> <tr><td>18</td><td>Verified</td><td>Card Verified</td></tr> <tr><td>19</td><td>Cancelled</td><td>Cancelled</td></tr> <tr><td>20</td><td>Un</td><td>Unknown</td></tr> <tr><td>21</td><td>Challenged</td><td>Challenged</td></tr> <tr><td>22</td><td>Decoupled</td><td>Decoupled</td></tr> <tr><td>23</td><td>Denied</td><td>Permission Denied</td></tr> </table> 
-            result_code (str): A result code of the transaction identifying the result of the transaction for success, rejection or decline.
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            amount (int): The amount of the transaction processed.. [optional]  # noqa: E501
-            authcode (str): The authorisation code of a successful transaction.. [optional]  # noqa: E501
-            datetime (datetime): The datetime that the transaction was processed.. [optional]  # noqa: E501
-            maskedpan (str): A masked value of the card number used for processing displaying limited values that can be used on a receipt. . [optional]  # noqa: E501
-            scheme (str): A name of the card scheme of the transaction that processed the transaction such as Visa or MasterCard. . [optional]  # noqa: E501
-            transno (int): The resulting transaction number, ordered incrementally from 1 for every merchant_id. The value will default to less than 1 for transactions that do not have a transaction number issued. . [optional]  # noqa: E501
-        """
 
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            for arg in args:
-                if isinstance(arg, dict):
-                    kwargs.update(arg)
-                else:
-                    raise ApiTypeError(
-                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                            args,
-                            self.__class__.__name__,
-                        ),
-                        path_to_item=_path_to_item,
-                        valid_classes=(self.__class__,),
-                    )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.account_id = account_id
-        self.identifier = identifier
-        self.merchantid = merchantid
-        self.message = message
-        self.result = result
-        self.result_code = result_code
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
```

### Comparing `citypay_api_client-1.1.1/citypay/model_utils.py` & `citypay_api_client-1.1.4/citypay/model_utils.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/citypay/utils/digest.py` & `citypay_api_client-1.1.4/citypay/utils/digest.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/citypay/utils/direct_post_mac.py` & `citypay_api_client-1.1.4/citypay/utils/direct_post_mac.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/citypay_api_client.egg-info/PKG-INFO` & `citypay_api_client-1.1.4/test/test_paylink_custom_param.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,35 @@
-Metadata-Version: 2.1
-Name: citypay-api-client
-Version: 1.1.1
-Summary: CityPay Payment API
-Home-page: 
-Author: CityPay Support
-Author-email: support@citypay.com
-Keywords: OpenAPI,OpenAPI-Generator,CityPay Payment API
-Requires-Python: >=3.6
+"""
+    CityPay Payment API
 
      This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security Your application will need to adhere to PCI-DSS standards to operate safely and to meet requirements set out by  Visa and MasterCard and the PCI Security Standards Council. These include  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
-    
+
+    Contact: support@citypay.com
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import sys
+import unittest
+
+import citypay
+from citypay.models.paylink_custom_param import PaylinkCustomParam
+
+
+class TestPaylinkCustomParam(unittest.TestCase):
+    """PaylinkCustomParam unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testPaylinkCustomParam(self):
+        """Test PaylinkCustomParam"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = PaylinkCustomParam()  # noqa: E501
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `citypay_api_client-1.1.1/citypay_api_client.egg-info/SOURCES.txt` & `citypay_api_client-1.1.4/citypay_api_client.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,115 @@
 README.md
 setup.cfg
 setup.py
 citypay/__init__.py
 citypay/api_client.py
+citypay/api_response.py
 citypay/configuration.py
 citypay/exceptions.py
 citypay/model_utils.py
 citypay/rest.py
 citypay/api/__init__.py
 citypay/api/authorisation_and_payment_api.py
 citypay/api/batch_processing_api.py
 citypay/api/card_holder_account_api.py
 citypay/api/direct_post_api.py
 citypay/api/operational_functions_api.py
 citypay/api/paylink_api.py
+citypay/api/reporting_api.py
 citypay/apis/__init__.py
-citypay/model/__init__.py
-citypay/model/account_create.py
-citypay/model/account_status.py
-citypay/model/acknowledgement.py
-citypay/model/acl_check_request.py
-citypay/model/acl_check_response_model.py
-citypay/model/airline_advice.py
-citypay/model/airline_segment.py
-citypay/model/api_key.py
-citypay/model/auth_reference.py
-citypay/model/auth_references.py
-citypay/model/auth_request.py
-citypay/model/auth_response.py
-citypay/model/authen_required.py
-citypay/model/batch.py
-citypay/model/batch_report_request.py
-citypay/model/batch_report_response_model.py
-citypay/model/batch_transaction.py
-citypay/model/batch_transaction_result_model.py
-citypay/model/bin.py
-citypay/model/bin_lookup.py
-citypay/model/c_res_auth_request.py
-citypay/model/capture_request.py
-citypay/model/card.py
-citypay/model/card_holder_account.py
-citypay/model/card_status.py
-citypay/model/charge_request.py
-citypay/model/check_batch_status.py
-citypay/model/check_batch_status_response.py
-citypay/model/contact_details.py
-citypay/model/decision.py
-citypay/model/direct_post_request.py
-citypay/model/direct_token_auth_request.py
-citypay/model/domain_key_check_request.py
-citypay/model/domain_key_request.py
-citypay/model/domain_key_response.py
-citypay/model/error.py
-citypay/model/event_data_model.py
-citypay/model/exists.py
-citypay/model/external_mpi.py
-citypay/model/list_merchants_response.py
-citypay/model/mcc6012.py
-citypay/model/merchant.py
-citypay/model/pa_res_auth_request.py
-citypay/model/paylink_address.py
-citypay/model/paylink_adjustment_request.py
-citypay/model/paylink_attachment_request.py
-citypay/model/paylink_attachment_result.py
-citypay/model/paylink_bill_payment_token_request.py
-citypay/model/paylink_card_holder.py
-citypay/model/paylink_cart.py
-citypay/model/paylink_cart_item_model.py
-citypay/model/paylink_config.py
-citypay/model/paylink_custom_param.py
-citypay/model/paylink_email_notification_path.py
-citypay/model/paylink_error_code.py
-citypay/model/paylink_field_guard_model.py
-citypay/model/paylink_part_payments.py
-citypay/model/paylink_sms_notification_path.py
-citypay/model/paylink_state_event.py
-citypay/model/paylink_token_created.py
-citypay/model/paylink_token_request_model.py
-citypay/model/paylink_token_status.py
-citypay/model/paylink_token_status_change_request.py
-citypay/model/paylink_token_status_change_response.py
-citypay/model/paylink_ui.py
-citypay/model/ping.py
-citypay/model/process_batch_request.py
-citypay/model/process_batch_response.py
-citypay/model/refund_request.py
-citypay/model/register_card.py
-citypay/model/request_challenged.py
-citypay/model/retrieve_request.py
-citypay/model/three_d_secure.py
-citypay/model/tokenisation_response_model.py
-citypay/model/void_request.py
 citypay/models/__init__.py
+citypay/models/account_create.py
+citypay/models/account_status.py
+citypay/models/acknowledgement.py
+citypay/models/acl_check_request.py
+citypay/models/acl_check_response_model.py
+citypay/models/airline_advice.py
+citypay/models/airline_segment.py
+citypay/models/api_key.py
+citypay/models/auth_reference.py
+citypay/models/auth_references.py
+citypay/models/auth_request.py
+citypay/models/auth_response.py
+citypay/models/authen_required.py
+citypay/models/batch.py
+citypay/models/batch_report_request.py
+citypay/models/batch_report_response_model.py
+citypay/models/batch_transaction.py
+citypay/models/batch_transaction_report_request.py
+citypay/models/batch_transaction_report_response.py
+citypay/models/batch_transaction_result_model.py
+citypay/models/bin.py
+citypay/models/bin_lookup.py
+citypay/models/c_res_auth_request.py
+citypay/models/capture_request.py
+citypay/models/card.py
+citypay/models/card_holder_account.py
+citypay/models/card_status.py
+citypay/models/charge_request.py
+citypay/models/check_batch_status.py
+citypay/models/check_batch_status_response.py
+citypay/models/contact_details.py
+citypay/models/decision.py
+citypay/models/direct_post_request.py
+citypay/models/direct_token_auth_request.py
+citypay/models/domain_key_check_request.py
+citypay/models/domain_key_request.py
+citypay/models/domain_key_response.py
+citypay/models/error.py
+citypay/models/event_data_model.py
+citypay/models/exists.py
+citypay/models/external_mpi.py
+citypay/models/list_merchants_response.py
+citypay/models/mcc6012.py
+citypay/models/merchant.py
+citypay/models/merchant_batch_report_request.py
+citypay/models/merchant_batch_report_response.py
+citypay/models/merchant_batch_response.py
+citypay/models/net_summary_response.py
+citypay/models/pa_res_auth_request.py
+citypay/models/paylink_address.py
+citypay/models/paylink_adjustment_request.py
+citypay/models/paylink_attachment_request.py
+citypay/models/paylink_attachment_result.py
+citypay/models/paylink_bill_payment_token_request.py
+citypay/models/paylink_card_holder.py
+citypay/models/paylink_cart.py
+citypay/models/paylink_cart_item_model.py
+citypay/models/paylink_config.py
+citypay/models/paylink_custom_param.py
+citypay/models/paylink_email_notification_path.py
+citypay/models/paylink_error_code.py
+citypay/models/paylink_field_guard_model.py
+citypay/models/paylink_part_payments.py
+citypay/models/paylink_resend_notification_request.py
+citypay/models/paylink_sms_notification_path.py
+citypay/models/paylink_state_event.py
+citypay/models/paylink_token_created.py
+citypay/models/paylink_token_request_model.py
+citypay/models/paylink_token_status.py
+citypay/models/paylink_token_status_change_request.py
+citypay/models/paylink_token_status_change_response.py
+citypay/models/paylink_ui.py
+citypay/models/payment_intent.py
+citypay/models/payment_intent_reference.py
+citypay/models/ping.py
+citypay/models/process_batch_request.py
+citypay/models/process_batch_response.py
+citypay/models/refund_request.py
+citypay/models/register_card.py
+citypay/models/remittance_data.py
+citypay/models/remittance_report_request.py
+citypay/models/remittance_report_response.py
+citypay/models/remitted_client_data.py
+citypay/models/request_challenged.py
+citypay/models/retrieve_request.py
+citypay/models/three_d_secure.py
+citypay/models/tokenisation_response_model.py
+citypay/models/void_request.py
 citypay/utils/__init__.py
 citypay/utils/digest.py
 citypay/utils/direct_post_mac.py
 citypay_api_client.egg-info/PKG-INFO
 citypay_api_client.egg-info/SOURCES.txt
 citypay_api_client.egg-info/dependency_links.txt
 citypay_api_client.egg-info/requires.txt
@@ -115,14 +129,16 @@
 test/test_authen_required.py
 test/test_authorisation_and_payment_api.py
 test/test_batch.py
 test/test_batch_processing_api.py
 test/test_batch_report_request.py
 test/test_batch_report_response_model.py
 test/test_batch_transaction.py
+test/test_batch_transaction_report_request.py
+test/test_batch_transaction_report_response.py
 test/test_batch_transaction_result_model.py
 test/test_bin.py
 test/test_bin_lookup.py
 test/test_c_res_auth_request.py
 test/test_capture_request.py
 test/test_card.py
 test/test_card_holder_account.py
@@ -143,14 +159,18 @@
 test/test_event_data_model.py
 test/test_exists.py
 test/test_external_mpi.py
 test/test_it_api_sandbox.py
 test/test_list_merchants_response.py
 test/test_mcc6012.py
 test/test_merchant.py
+test/test_merchant_batch_report_request.py
+test/test_merchant_batch_report_response.py
+test/test_merchant_batch_response.py
+test/test_net_summary_response.py
 test/test_operational_functions_api.py
 test/test_pa_res_auth_request.py
 test/test_paylink_address.py
 test/test_paylink_adjustment_request.py
 test/test_paylink_api.py
 test/test_paylink_attachment_request.py
 test/test_paylink_attachment_result.py
@@ -160,25 +180,33 @@
 test/test_paylink_cart_item_model.py
 test/test_paylink_config.py
 test/test_paylink_custom_param.py
 test/test_paylink_email_notification_path.py
 test/test_paylink_error_code.py
 test/test_paylink_field_guard_model.py
 test/test_paylink_part_payments.py
+test/test_paylink_resend_notification_request.py
 test/test_paylink_sms_notification_path.py
 test/test_paylink_state_event.py
 test/test_paylink_token_created.py
 test/test_paylink_token_request_model.py
 test/test_paylink_token_status.py
 test/test_paylink_token_status_change_request.py
 test/test_paylink_token_status_change_response.py
 test/test_paylink_ui.py
+test/test_payment_intent.py
+test/test_payment_intent_reference.py
 test/test_ping.py
 test/test_process_batch_request.py
 test/test_process_batch_response.py
 test/test_refund_request.py
 test/test_register_card.py
+test/test_remittance_data.py
+test/test_remittance_report_request.py
+test/test_remittance_report_response.py
+test/test_remitted_client_data.py
+test/test_reporting_api.py
 test/test_request_challenged.py
 test/test_retrieve_request.py
 test/test_three_d_secure.py
 test/test_tokenisation_response_model.py
 test/test_void_request.py
```

### Comparing `citypay_api_client-1.1.1/setup.py` & `citypay_api_client-1.1.4/citypay/models/authen_required.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,93 @@
+# coding: utf-8
+
 """
     CityPay Payment API
 
-     This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security Your application will need to adhere to PCI-DSS standards to operate safely and to meet requirements set out by  Visa and MasterCard and the PCI Security Standards Council. These include  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
+     This CityPay API is an HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokenized payments using cardholder Accounts.  ## Compliance and Security Your application will need to adhere to PCI-DSS standards to operate safely and to meet requirements set out by  Visa and MasterCard and the PCI Security Standards Council. These include  * Data must be collected using TLS version 1.2 using [strong cryptography](https://citypay.github.io/api-docs/payment-api/#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive cardholder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities. 
 
-    The version of the OpenAPI document: 6.4.18
     Contact: support@citypay.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-from setuptools import setup, find_packages  # noqa: H301
 
-NAME = "citypay_api_client"
-VERSION = "1.1.1"
-# To install the library, run the following
-#
-# python setup.py install
-#
-# prerequisite: setuptools
-# http://pypi.python.org/pypi/setuptools
-
-REQUIRES = [
-  "urllib3 >= 1.25.3",
-  "python-dateutil",
-]
-
-setup(
-    name=NAME,
-    version=VERSION,
-    description="CityPay Payment API",
-    author="CityPay Support",
-    author_email="support@citypay.com",
-    url="",
-    keywords=["OpenAPI", "OpenAPI-Generator", "CityPay Payment API"],
-    python_requires=">=3.6",
-    install_requires=REQUIRES,
-    packages=find_packages(exclude=["test", "tests"]),
-    include_package_data=True,
-    long_description="""\
-     This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security Your application will need to adhere to PCI-DSS standards to operate safely and to meet requirements set out by  Visa and MasterCard and the PCI Security Standards Council. These include  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
+from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, StrictStr
+from pydantic import Field
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
+
+class AuthenRequired(BaseModel):
     """
-)
+    AuthenRequired
+    """ # noqa: E501
+    acs_url: Optional[StrictStr] = Field(default=None, description="The url of the Access Control Server (ACS) to forward the user to. ")
+    md: Optional[StrictStr] = Field(default=None, description="Merchant Data (MD) which should be sent to the ACS to establish and reference the authentication session. ")
+    pareq: Optional[StrictStr] = Field(default=None, description="The Payer Authentication Request packet which should be `POSTed` to the Url of the ACS to establish the authentication session. Data should be sent untouched. ")
+    __properties: ClassVar[List[str]] = ["acs_url", "md", "pareq"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of AuthenRequired from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude={
+            },
+            exclude_none=True,
+        )
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of AuthenRequired from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
+
+        _obj = cls.model_validate({
+            "acs_url": obj.get("acs_url"),
+            "md": obj.get("md"),
+            "pareq": obj.get("pareq")
+        })
+        return _obj
+
+
```

### Comparing `citypay_api_client-1.1.1/test/test_account_create.py` & `citypay_api_client-1.1.4/test/test_account_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import unittest
 
-from citypay.model.account_create import AccountCreate  # noqa: E501
-from citypay.model.contact_details import ContactDetails
+from citypay.models.account_create import AccountCreate  # noqa: E501
+from citypay.models.contact_details import ContactDetails
 
 
 class TestAccountCreate(unittest.TestCase):
     """AccountCreate unit test stubs"""
 
     def setUp(self):
         pass
@@ -53,13 +53,13 @@
         else:
             return AccountCreate(
                 account_id='aaabbb-cccddd-eee',
             )
 
     def testAccountCreate(self):
         """Test AccountCreate"""
-        inst_req_only = self.make_instance(include_optional=False)
-        inst_req_and_optional = self.make_instance(include_optional=True)
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_account_status.py` & `citypay_api_client-1.1.4/test/test_account_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.account_status import AccountStatus  # noqa: E501
+from citypay.models.account_status import AccountStatus  # noqa: E501
 
 
 class TestAccountStatus(unittest.TestCase):
     """AccountStatus unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_acknowledgement.py` & `citypay_api_client-1.1.4/test/test_acknowledgement.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
 from citypay import ApiClient
-from citypay.model.acknowledgement import Acknowledgement  # noqa: E501
+from citypay.models.acknowledgement import Acknowledgement  # noqa: E501
 
 
 class TestAcknowledgement(unittest.TestCase):
     """Acknowledgement unit test stubs"""
 
     def setUp(self):
         self.data = """
@@ -24,15 +24,15 @@
             "code": "000",
             "context": "1B12WmDZB3EYSbb",
             "identifier": "testIdentifier",
             "message": "System: Accepted Transaction"
         }        
         """
 
-        self.instance = ApiClient().deserialize(self, (Acknowledgement,), True)
+        self.instance = ApiClient().deserialize(self.data, Acknowledgement)
 
     def tearDown(self):
         # run after each test
         pass
 
     def testAcknowledgement(self):
         """Test Acknowledgement"""
```

### Comparing `citypay_api_client-1.1.1/test/test_acl_check_request.py` & `citypay_api_client-1.1.4/test/test_acl_check_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.acl_check_request import AclCheckRequest
+from citypay.models.acl_check_request import AclCheckRequest
 
 
 class TestAclCheckRequest(unittest.TestCase):
     """AclCheckRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_acl_check_response_model.py` & `citypay_api_client-1.1.4/test/test_acl_check_response_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.acl_check_response_model import AclCheckResponseModel
+from citypay.models.acl_check_response_model import AclCheckResponseModel
 
 
 class TestAclCheckResponseModel(unittest.TestCase):
     """AclCheckResponseModel unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_airline_advice.py` & `citypay_api_client-1.1.4/test/test_airline_advice.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
 from datetime import date
-from citypay.model.airline_advice import AirlineAdvice  # noqa: E501
-from citypay.model.airline_segment import AirlineSegment  # noqa: E501
+from citypay.models.airline_advice import AirlineAdvice  # noqa: E501
+from citypay.models.airline_segment import AirlineSegment  # noqa: E501
 
 
 class TestAirlineAdvice(unittest.TestCase):
     """AirlineAdvice unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_airline_segment.py` & `citypay_api_client-1.1.4/test/test_airline_segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
 from datetime import date
-from citypay.model.airline_segment import AirlineSegment  # noqa: E501
+from citypay.models.airline_segment import AirlineSegment  # noqa: E501
 
 
 class TestAirlineSegment(unittest.TestCase):
     """AirlineSegment unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_api_key.py` & `citypay_api_client-1.1.4/test/test_api_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from citypay.model.api_key import *
+from citypay.models.api_key import *
 
 
 class TestApiKey(unittest.TestCase):
 
     def testGenerate(self):
         dt = datetime.strptime("2020-01-01T09:23:12", "%Y-%m-%dT%H:%M:%S")
         key = api_key_generate_for("PC2", "7G79TG62BAJTK669", bytearray.fromhex("acb875aef083de292299bd69fcdeb5c5"), dt)
```

### Comparing `citypay_api_client-1.1.1/test/test_auth_reference.py` & `citypay_api_client-1.1.4/test/test_auth_reference.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
 from datetime import datetime
-from citypay.model.auth_reference import AuthReference  # noqa: E501
+from citypay.models.auth_reference import AuthReference  # noqa: E501
 
 
 class TestAuthReference(unittest.TestCase):
     """AuthReference unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_auth_references.py` & `citypay_api_client-1.1.4/test/test_auth_references.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.auth_references import AuthReferences  # noqa: E501
+from citypay.models.auth_references import AuthReferences  # noqa: E501
 from citypay import ApiClient
 
 
 class TestAuthReferences(unittest.TestCase):
     """AuthReferences unit test stubs"""
 
     def setUp(self):
@@ -35,15 +35,15 @@
               "result": "Accepted",
               "trans_status": "O",
               "trans_type": "S",
               "transno": 88
           }
         ]}       
         """
-        self.instance = ApiClient().deserialize(self, (AuthReferences,), True)
+        self.instance = ApiClient().deserialize(self.data, AuthReferences)
 
     def tearDown(self):
         pass
 
     def testAuthReferences(self):
         """Test AuthReferences"""
         self.assertEqual(self.instance.auths[0].amount, "0.12")
```

### Comparing `citypay_api_client-1.1.1/test/test_auth_request.py` & `citypay_api_client-1.1.4/test/test_auth_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
 from datetime import date
 import citypay
-from citypay.model.airline_advice import AirlineAdvice
-from citypay.model.airline_segment import AirlineSegment
-from citypay.model.auth_request import AuthRequest  # noqa: E501
-from citypay.model.contact_details import ContactDetails
-from citypay.model.external_mpi import ExternalMPI
-from citypay.model.mcc6012 import MCC6012
-from citypay.model.three_d_secure import ThreeDSecure
+from citypay.models.airline_advice import AirlineAdvice
+from citypay.models.airline_segment import AirlineSegment
+from citypay.models.auth_request import AuthRequest  # noqa: E501
+from citypay.models.contact_details import ContactDetails
+from citypay.models.external_mpi import ExternalMPI
+from citypay.models.mcc6012 import MCC6012
+from citypay.models.three_d_secure import ThreeDSecure
 
 
 class TestAuthRequest(unittest.TestCase):
     """AuthRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_auth_response.py` & `citypay_api_client-1.1.4/test/test_auth_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import unittest
-from citypay.model.auth_response import AuthResponse  # noqa: E501
+from citypay.models.auth_response import AuthResponse  # noqa: E501
 from citypay import ApiClient
 
 
 class TestAuthResponse(unittest.TestCase):
     """AuthResponse unit test stubs"""
 
     def setUp(self):
@@ -48,15 +48,48 @@
           "scheme": "VISA_BUSINESS",
           "sha256": "abcdefg",
           "trans_status": "P",
           "transno": 74875
         }
         """
 
-        self.instance = ApiClient().deserialize(self, (AuthResponse,), True)
+        self.data_no_ident = """
+        {
+            "amount": 0,
+            "atrn": "",
+            "atsd": "",
+            "authcode": "",
+            "authen_result": "",
+            "authorised": false,
+            "avs_result": " ",
+            "bin_commercial": false,
+            "bin_debit": false,
+            "bin_description": "",
+            "cavv": "",
+            "context": "PC.0.A5298ef695b",
+            "csc_result": " ",
+            "currency": "---",
+            "datetime": "1969-12-31T23:59:59Z",
+            "eci": "0",
+            "identifier": "",
+            "live": true,
+            "maskedpan": "N/A",
+            "merchantid": 0,
+            "result": 3,
+            "result_code": "P030",
+            "result_message": "Request Error: Authorisation invalid (203: Data element not in the required format or value is invalid as defined in Table A.1. threeDSSessionData)",
+            "scheme": "",
+            "sha256": "",
+            "trans_status": "_",
+            "transno": -1
+        }
+        """
+
+        self.instance = ApiClient().deserialize(self.data, AuthResponse)
+        self.instance_no_ident = ApiClient().deserialize(self.data_no_ident, AuthResponse)
 
     def tearDown(self):
         pass
 
     def testAuthResponse(self):
         """Test AuthResponse"""
         self.assertEqual(self.instance.amount, 5500)
@@ -82,11 +115,13 @@
         self.assertEqual(self.instance.result, 1)
         self.assertEqual(self.instance.result_code, "000")
         self.assertEqual(self.instance.result_message, "System: Accepted Transaction")
         self.assertEqual(self.instance.scheme, "VISA_BUSINESS")
         self.assertEqual(self.instance.sha256, "abcdefg")
         self.assertEqual(self.instance.trans_status, "P")
         self.assertEqual(self.instance.transno, 74875)
+        self.assertEqual(self.instance_no_ident.result_code, "P030")
+        self.assertEqual(self.instance_no_ident.result, 3)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_authen_required.py` & `citypay_api_client-1.1.4/test/test_authen_required.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.authen_required import AuthenRequired  # noqa: E501
+from citypay.models.authen_required import AuthenRequired  # noqa: E501
 from citypay.api_client import ApiClient
 
 
 class TestAuthenRequired(unittest.TestCase):
     """AuthenRequired unit test stubs"""
 
     def setUp(self):
@@ -24,15 +24,15 @@
         {
            "acs_url": "https://www.acs.com/tdsecure/opt_in_dispatcher.jsp?partner=debit&VAA=B",
             "md": "0000000000000000000022",
             "pareq": "eJxVUm1v2yAQ/itWv8dg/B5dmJyfw=="
         }
         """
 
-        self.instance = ApiClient().deserialize(self, (AuthenRequired,), True)
+        self.instance = ApiClient().deserialize(self.data, AuthenRequired)
 
     def tearDown(self):
         pass
 
     def testAuthenRequired(self):
         """Test AuthenRequired"""
         self.assertEqual(self.instance.acs_url, "https://www.acs.com/tdsecure/opt_in_dispatcher.jsp?partner=debit&VAA=B")
```

### Comparing `citypay_api_client-1.1.1/test/test_authorisation_and_payment_api.py` & `citypay_api_client-1.1.4/test/test_authorisation_and_payment_api.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/test/test_batch.py` & `citypay_api_client-1.1.4/test/test_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.batch import Batch
+from citypay.models.batch import Batch
 
 
 class TestBatch(unittest.TestCase):
     """Batch unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_batch_processing_api.py` & `citypay_api_client-1.1.4/test/test_batch_processing_api.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/test/test_batch_report_request.py` & `citypay_api_client-1.1.4/test/test_batch_report_request.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/test/test_batch_report_response_model.py` & `citypay_api_client-1.1.4/test/test_batch_report_response_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
-from citypay.model.batch_transaction_result_model import BatchTransactionResultModel
+from citypay.models.batch_transaction_result_model import BatchTransactionResultModel
 
 globals()['BatchTransactionResultModel'] = BatchTransactionResultModel
 
 
 class TestBatchReportResponseModel(unittest.TestCase):
     """BatchReportResponseModel unit test stubs"""
```

### Comparing `citypay_api_client-1.1.1/test/test_batch_transaction.py` & `citypay_api_client-1.1.4/test/test_batch_transaction.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/test/test_batch_transaction_result_model.py` & `citypay_api_client-1.1.4/test/test_batch_transaction_result_model.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/test/test_bin.py` & `citypay_api_client-1.1.4/test/test_bin.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/test/test_bin_lookup.py` & `citypay_api_client-1.1.4/test/test_bin_lookup.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/test/test_c_res_auth_request.py` & `citypay_api_client-1.1.4/test/test_c_res_auth_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.c_res_auth_request import CResAuthRequest  # noqa: E501
+from citypay.models.c_res_auth_request import CResAuthRequest  # noqa: E501
 
 
 class TestCResAuthRequest(unittest.TestCase):
     """CResAuthRequest unit test stubs"""
 
     def setUp(self):
         pass
@@ -24,15 +24,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test CResAuthRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.c_res_auth_request.CResAuthRequest()  # noqa: E501
+        # model = citypay.models.c_res_auth_request.CResAuthRequest()  # noqa: E501
 
         if include_optional:
             return CResAuthRequest(
                 cres='x90+vZ/7Ll05Vid/jPfQn8adw+4D/vRDUGT19kndW97Hfirbv66ycfSp8jNlvy7PkHbx44NEt3vo...'
             )
         else:
             return CResAuthRequest(
```

### Comparing `citypay_api_client-1.1.1/test/test_capture_request.py` & `citypay_api_client-1.1.4/test/test_capture_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
 from datetime import date
 import citypay
-from citypay.model.airline_advice import AirlineAdvice
-from citypay.model.airline_segment import AirlineSegment
-from citypay.model.capture_request import CaptureRequest  # noqa: E501
+from citypay.models.airline_advice import AirlineAdvice
+from citypay.models.airline_segment import AirlineSegment
+from citypay.models.capture_request import CaptureRequest  # noqa: E501
 
 
 class TestCaptureRequest(unittest.TestCase):
     """CaptureRequest unit test stubs"""
 
     def setUp(self):
         pass
@@ -28,15 +28,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test CaptureRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.capture_request.CaptureRequest()  # noqa: E501
+        # model = citypay.models.capture_request.CaptureRequest()  # noqa: E501
 
         if include_optional:
             return CaptureRequest(
                 airline_data=AirlineAdvice(
                     carrier_name='EG Air',
                     conjunction_ticket_indicator=False,
                     eticket_indicator=True,
```

### Comparing `citypay_api_client-1.1.1/test/test_card.py` & `citypay_api_client-1.1.4/test/test_card.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.card import Card  # noqa: E501
+from citypay.models.card import Card  # noqa: E501
 
 
 class TestCard(unittest.TestCase):
     """Card unit test stubs"""
 
     def setUp(self):
         pass
@@ -24,15 +24,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test Card
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.card.Card()  # noqa: E501
+        # model = citypay.models.card.Card()  # noqa: E501
 
         if include_optional:
             return Card(
                 bin_commercial=True,
                 bin_corporate=True,
                 bin_country_issued='0',
                 bin_credit=True,
```

### Comparing `citypay_api_client-1.1.1/test/test_card_holder_account.py` & `citypay_api_client-1.1.4/test/test_card_holder_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.card_holder_account import CardHolderAccount  # noqa: E501
+from citypay.models.card_holder_account import CardHolderAccount  # noqa: E501
 from citypay.api_client import ApiClient
 
 
 class TestCardHolderAccount(unittest.TestCase):
     """CardHolderAccount unit test stubs"""
 
     def setUp(self):
@@ -58,15 +58,15 @@
             "default_card_id": "2U1XV3PJSeUXFNzXidACn2TyCzAK",
             "default_card_index": 0,
             "status": "ACTIVE",
             "unique_id": "Ew3BKeWNdL3qKQU7XK7Sbt2eAL5WFW4AfoASDSA"
         }
         """
 
-        self.instance = ApiClient().deserialize(self, (CardHolderAccount,), True)
+        self.instance = ApiClient().deserialize(self.data, CardHolderAccount)
 
     def tearDown(self):
         pass
 
     def testCardHolderAccount(self):
         """Test CardHolderAccount"""
         self.assertEqual(self.instance.account_id, "abc123")
```

### Comparing `citypay_api_client-1.1.1/test/test_card_holder_account_api.py` & `citypay_api_client-1.1.4/test/test_card_holder_account_api.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/test/test_card_status.py` & `citypay_api_client-1.1.4/test/test_card_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.card_status import CardStatus  # noqa: E501
+from citypay.models.card_status import CardStatus  # noqa: E501
 
 
 class TestCardStatus(unittest.TestCase):
     """CardStatus unit test stubs"""
 
     def setUp(self):
         pass
@@ -25,15 +25,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test CardStatus
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.card_status.CardStatus()  # noqa: E501
+        # model = citypay.models.card_status.CardStatus()  # noqa: E501
 
         if include_optional :
             return CardStatus(
                 card_status = '0', 
                 default = True
             )
         else :
```

### Comparing `citypay_api_client-1.1.1/test/test_charge_request.py` & `citypay_api_client-1.1.4/test/test_charge_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.charge_request import ChargeRequest  # noqa: E501
+from citypay.models.charge_request import ChargeRequest  # noqa: E501
 
 
 class TestChargeRequest(unittest.TestCase):
     """ChargeRequest unit test stubs"""
 
     def setUp(self):
         pass
@@ -24,15 +24,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test ChargeRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.charge_request.ChargeRequest()  # noqa: E501
+        # model = citypay.models.charge_request.ChargeRequest()  # noqa: E501
 
         if include_optional:
             return ChargeRequest(
                 amount=3600,
                 avs_postcode_policy='0',
                 csc='123',
                 csc_policy='0',
```

### Comparing `citypay_api_client-1.1.1/test/test_check_batch_status.py` & `citypay_api_client-1.1.4/test/test_check_batch_status.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/test/test_check_batch_status_response.py` & `citypay_api_client-1.1.4/test/test_check_batch_status_response.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/test/test_contact_details.py` & `citypay_api_client-1.1.4/test/test_contact_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.contact_details import ContactDetails  # noqa: E501
+from citypay.models.contact_details import ContactDetails  # noqa: E501
 
 
 class TestContactDetails(unittest.TestCase):
     """ContactDetails unit test stubs"""
 
     def setUp(self):
         pass
@@ -24,15 +24,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test ContactDetails
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.contact_details.ContactDetails()  # noqa: E501
+        # model = citypay.models.contact_details.ContactDetails()  # noqa: E501
 
         if include_optional:
             return ContactDetails(
                 address1='79 Parliament St',
                 address2='Westminster',
                 address3='0',
                 area='London',
```

### Comparing `citypay_api_client-1.1.1/test/test_decision.py` & `citypay_api_client-1.1.4/test/test_decision.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.decision import Decision  # noqa: E501
+from citypay.models.decision import Decision  # noqa: E501
 from citypay.api_client import ApiClient
 
 
 class TestDecision(unittest.TestCase):
     """Decision unit test stubs"""
 
     def setUp(self):
@@ -49,27 +49,26 @@
         "scheme": "VISA_BUSINESS",
         "sha256": "abcdefg",
         "trans_status": "P",
         "transno": 74875
     }
 }
                    """
-        self.instance = ApiClient().deserialize(self, (Decision,), True)
+        self.instance = ApiClient().deserialize(self.data, Decision)
 
     def tearDown(self):
         pass
 
     def testDecisionType(self):
-        self.assertTrue(self.instance.auth_response())
-        self.assertFalse(self.instance.authen_required())
-        self.assertFalse(self.instance.request_challenged())
+        self.assertTrue(self.instance.auth_response)
+        self.assertFalse(self.instance.request_challenged)
 
     def testDecision(self):
         """Test Decision"""
-        response = self.instance.auth_response()
+        response = self.instance.auth_response
         self.assertEqual(response.amount, 5500)
         self.assertEqual(response.atrn, "atrn1")
         self.assertEqual(response.atsd, "a")
         self.assertEqual(response.authcode, "12345")
         self.assertEqual(response.authen_result, "R")
         self.assertEqual(response.authorised, True)
         self.assertEqual(response.avs_result, "G")
```

### Comparing `citypay_api_client-1.1.1/test/test_direct_post_api.py` & `citypay_api_client-1.1.4/test/test_direct_post_api.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/test/test_direct_post_request.py` & `citypay_api_client-1.1.4/test/test_direct_post_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.contact_details import ContactDetails
-from citypay.model.three_d_secure import ThreeDSecure
+from citypay.models.contact_details import ContactDetails
+from citypay.models.three_d_secure import ThreeDSecure
 globals()['ContactDetails'] = ContactDetails
 globals()['ThreeDSecure'] = ThreeDSecure
-from citypay.model.direct_post_request import DirectPostRequest
+from citypay.models.direct_post_request import DirectPostRequest
 
 
 class TestDirectPostRequest(unittest.TestCase):
     """DirectPostRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_direct_token_auth_request.py` & `citypay_api_client-1.1.4/test/test_paylink_ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.direct_token_auth_request import DirectTokenAuthRequest
+from citypay.models.paylink_ui import PaylinkUI
 
 
-class TestDirectTokenAuthRequest(unittest.TestCase):
-    """DirectTokenAuthRequest unit test stubs"""
+class TestPaylinkUI(unittest.TestCase):
+    """PaylinkUI unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDirectTokenAuthRequest(self):
-        """Test DirectTokenAuthRequest"""
+    def testPaylinkUI(self):
+        """Test PaylinkUI"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = DirectTokenAuthRequest()  # noqa: E501
+        # model = PaylinkUI()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_domain_key_check_request.py` & `citypay_api_client-1.1.4/test/test_domain_key_check_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.domain_key_check_request import DomainKeyCheckRequest
+from citypay.models.domain_key_check_request import DomainKeyCheckRequest
 
 
 class TestDomainKeyCheckRequest(unittest.TestCase):
     """DomainKeyCheckRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_domain_key_request.py` & `citypay_api_client-1.1.4/test/test_domain_key_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.domain_key_request import DomainKeyRequest
+from citypay.models.domain_key_response import DomainKeyResponse
 
 
-class TestDomainKeyRequest(unittest.TestCase):
-    """DomainKeyRequest unit test stubs"""
+class TestDomainKeyResponse(unittest.TestCase):
+    """DomainKeyResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDomainKeyRequest(self):
-        """Test DomainKeyRequest"""
+    def testDomainKeyResponse(self):
+        """Test DomainKeyResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = DomainKeyRequest()  # noqa: E501
+        # model = DomainKeyResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_domain_key_response.py` & `citypay_api_client-1.1.4/test/test_event_data_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.domain_key_response import DomainKeyResponse
+from citypay.models.event_data_model import EventDataModel
 
 
-class TestDomainKeyResponse(unittest.TestCase):
-    """DomainKeyResponse unit test stubs"""
+class TestEventDataModel(unittest.TestCase):
+    """EventDataModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDomainKeyResponse(self):
-        """Test DomainKeyResponse"""
+    def testEventDataModel(self):
+        """Test EventDataModel"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = DomainKeyResponse()  # noqa: E501
+        # model = EventDataModel()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_error.py` & `citypay_api_client-1.1.4/test/test_error.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.error import Error  # noqa: E501
+from citypay.models.error import Error  # noqa: E501
 from citypay.api_client import ApiClient
 
 
 class TestError(unittest.TestCase):
     """Error unit test stubs"""
 
     def setUp(self):
@@ -23,15 +23,15 @@
         {
             "code": "000",
             "context": "aspiu352908ns47n343598bads",
             "identifier": "95b857a1-5955-4b86-963c-5a6dbfc4fb95",
             "message": "Approved 044332"
         }
         """
-        self.instance = ApiClient().deserialize(self, (Error,), True)
+        self.instance = ApiClient().deserialize(self.data, Error)
 
     def tearDown(self):
         pass
 
     def testError(self):
         """Test Error"""
         self.assertEqual(self.instance.code, "000")
```

### Comparing `citypay_api_client-1.1.1/test/test_event_data_model.py` & `citypay_api_client-1.1.4/test/test_paylink_address.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.event_data_model import EventDataModel
+from citypay.models.paylink_address import PaylinkAddress
 
 
-class TestEventDataModel(unittest.TestCase):
-    """EventDataModel unit test stubs"""
+class TestPaylinkAddress(unittest.TestCase):
+    """PaylinkAddress unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testEventDataModel(self):
-        """Test EventDataModel"""
+    def testPaylinkAddress(self):
+        """Test PaylinkAddress"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = EventDataModel()  # noqa: E501
+        # model = PaylinkAddress()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_exists.py` & `citypay_api_client-1.1.4/test/test_exists.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
 from datetime import datetime
-from citypay.model.exists import Exists  # noqa: E501
+from citypay.models.exists import Exists  # noqa: E501
 
 
 class TestExists(unittest.TestCase):
     """Exists unit test stubs"""
 
     def setUp(self):
         pass
@@ -25,15 +25,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test Exists
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.exists.Exists()  # noqa: E501
+        # model = citypay.models.exists.Exists()  # noqa: E501
 
         if include_optional:
             return Exists(
                 active=True,
                 exists=True,
                 last_modified=datetime(2020, 1, 2, 18, 32, 28)
             )
```

### Comparing `citypay_api_client-1.1.1/test/test_external_mpi.py` & `citypay_api_client-1.1.4/test/test_external_mpi.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.external_mpi import ExternalMPI  # noqa: E501
+from citypay.models.external_mpi import ExternalMPI  # noqa: E501
 from citypay.rest import ApiException
 
 
 class TestExternalMPI(unittest.TestCase):
     """ExternalMPI unit test stubs"""
 
     def setUp(self):
@@ -26,15 +26,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test ExternalMPI
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.external_mpi.ExternalMPI()  # noqa: E501
+        # model = citypay.models.external_mpi.ExternalMPI()  # noqa: E501
 
         if include_optional :
             return ExternalMPI(
                 authen_result = '0', 
                 cavv = '0', 
                 eci = 56, 
                 enrolled = '0',
```

### Comparing `citypay_api_client-1.1.1/test/test_it_api_sandbox.py` & `citypay_api_client-1.1.4/test/test_it_api_sandbox.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 import unittest
 import uuid
 import citypay
 from citypay import Configuration
 from citypay.api.card_holder_account_api import CardHolderAccountApi
 from citypay.api.operational_functions_api import OperationalFunctionsApi
 from citypay.api.authorisation_and_payment_api import AuthorisationAndPaymentApi
-from citypay.model.account_create import AccountCreate
-from citypay.model.api_key import *
+from citypay.models.account_create import AccountCreate
+from citypay.models.api_key import *
 import requests
 import base64
 
-from citypay.model.auth_request import AuthRequest
-from citypay.model.c_res_auth_request import CResAuthRequest
-from citypay.model.charge_request import ChargeRequest
-from citypay.model.contact_details import ContactDetails
-from citypay.model.ping import Ping
-from citypay.model.register_card import RegisterCard
-from citypay.model.three_d_secure import ThreeDSecure
+from citypay.models.auth_request import AuthRequest
+from citypay.models.c_res_auth_request import CResAuthRequest
+from citypay.models.charge_request import ChargeRequest
+from citypay.models.contact_details import ContactDetails
+from citypay.models.ping import Ping
+from citypay.models.register_card import RegisterCard
+from citypay.models.three_d_secure import ThreeDSecure
 from citypay.utils.digest import validate_digest
 
 
 class TestApiIntegration(unittest.TestCase):
     """Error unit test stubs"""
 
     @classmethod
@@ -77,19 +77,18 @@
             identifier=id,
             merchantid=int(self.merchant_id),
             threedsecure=ThreeDSecure(
                 tds_policy="2"
             )
         ))
 
-        self.assertIsNone(decision.authen_required())
-        self.assertIsNone(decision.request_challenged())
-        self.assertIsNotNone(decision.auth_response())
+        self.assertIsNone(decision.request_challenged)
+        self.assertIsNotNone(decision.auth_response)
 
-        response = decision.auth_response()
+        response = decision.auth_response
         self.assertEqual(response.result_code, "001")
         self.assertEqual(response.identifier, id)
         self.assertEqual(response.authcode, "A12345")
         self.assertEqual(response.amount, 1395)
         self.assertTrue(validate_digest(response, self.licence_key))
 
     def testAuthorise3DSv2Test(self):
@@ -105,19 +104,18 @@
             trans_type="A",
             threedsecure=ThreeDSecure(
                 cp_bx="eyJhIjoiRkFwSCIsImMiOjI0LCJpIjoid3dIOTExTlBKSkdBRVhVZCIsImoiOmZhbHNlLCJsIjoiZW4tVVMiLCJoIjoxNDQwLCJ3IjoyNTYwLCJ0IjowLCJ1IjoiTW96aWxsYS81LjAgKE1hY2ludG9zaDsgSW50ZWwgTWFjIE9TIFggMTFfMl8zKSBBcHBsZVdlYktpdC81MzcuMzYgKEtIVE1MLCBsaWtlIEdlY2tvKSBDaHJvbWUvODkuMC40Mzg5LjgyIFNhZmFyaS81MzcuMzYiLCJ2IjoiMS4wLjAifQ",
                 merchant_termurl="https://citypay.com/acs/return"
             )
         ))
 
-        self.assertIsNone(decision.authen_required())
-        self.assertIsNotNone(decision.request_challenged())
-        self.assertIsNone(decision.auth_response())
+        self.assertIsNotNone(decision.request_challenged)
+        self.assertIsNone(decision.auth_response)
 
-        response = decision.request_challenged()
+        response = decision.request_challenged
         self.assertIsNotNone(response.creq)
         self.assertIsNotNone(response.acs_url)
         self.assertIsNotNone(response.threedserver_trans_id)
 
         content = {
             "threeDSSessionData": response.threedserver_trans_id,
             "creq": response.creq
@@ -125,21 +123,15 @@
 
         url = "https://sandbox.citypay.com/3dsv2/acs"
         headers = {'Content-type': 'application/json'}
 
         res = requests.post(url, data=json.dumps(content), headers=headers)
         res_obj = json.loads(res.text)
 
-        self.assertIsNotNone(res_obj['acsTransID'])
-        self.assertIsNotNone(res_obj['messageType'])
-        self.assertIsNotNone(res_obj['messageVersion'])
-        self.assertIsNotNone(res_obj['threeDSServerTransID'])
-        self.assertIsNotNone(res_obj['transStatus'])
-
-        c_res_auth_request = CResAuthRequest(cres=base64.b64encode(res.text.encode("ascii")).decode("ascii"))
+        c_res_auth_request = CResAuthRequest(cres=res_obj['cres'])
 
         c_res_request_response =  AuthorisationAndPaymentApi(self.api_client).c_res_request(c_res_auth_request)
 
         self.assertEqual(c_res_request_response.amount, 1396)
         self.assertEqual(c_res_request_response.authcode, "A12345")
         self.assertEqual(c_res_request_response.authen_result, "Y")
         self.assertEqual(c_res_request_response.authorised, True)
@@ -190,19 +182,18 @@
             token=result.cards[0].token,
             csc="012",
             threedsecure=ThreeDSecure(
                 tds_policy="2"
             )
         ))
 
-        self.assertIsNone(decision.authen_required())
-        self.assertIsNone(decision.request_challenged())
-        self.assertIsNotNone(decision.auth_response())
+        self.assertIsNone(decision.request_challenged)
+        self.assertIsNotNone(decision.auth_response)
 
-        response = decision.auth_response()
+        response = decision.auth_response
         self.assertEqual("001", response.result_code)
         self.assertEqual(identifier, response.identifier)
         self.assertEqual("A12345", response.authcode)
         self.assertEqual(7801, response.amount)
 
         # attempt with 3dsv1
         identifier = uuid.uuid4().hex
@@ -217,24 +208,17 @@
                 accept_headers="text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
                 merchant_termurl="https://citypay.com/example-url",
                 user_agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.121 Safari/537.36",
                 downgrade1=True
             )
         ))
 
-        self.assertIsNotNone(decision.authen_required())
-        self.assertIsNone(decision.request_challenged())
-        self.assertIsNone(decision.auth_response())
-
-        self.assertIsNotNone(decision.authen_required().acs_url)
-        self.assertIsNotNone(decision.authen_required().md)
-        self.assertIsNotNone(decision.authen_required().pareq)
+        self.assertIsNotNone(decision.request_challenged)
+        self.assertIsNone(decision.auth_response)
+
+        self.assertIsNotNone(decision.request_challenged.acs_url)
 
         result = api.account_delete_request(cha_id)
         self.assertEqual(result.code, "001")
 
-    def tearDown(self):
-        self.api_client.close()
-
-
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_list_merchants_response.py` & `citypay_api_client-1.1.4/test/test_list_merchants_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 import unittest
 import citypay
-from citypay.model.list_merchants_response import ListMerchantsResponse  # noqa: E501
-from citypay.model.merchant import Merchant
+from citypay.models.list_merchants_response import ListMerchantsResponse  # noqa: E501
+from citypay.models.merchant import Merchant
 
 
 class TestListMerchantsResponse(unittest.TestCase):
     """ListMerchantsResponse unit test stubs"""
 
     def setUp(self):
         pass
@@ -27,15 +27,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test ListMerchantsResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.list_merchants_response.ListMerchantsResponse()  # noqa: E501
+        # model = citypay.models.list_merchants_response.ListMerchantsResponse()  # noqa: E501
 
         if include_optional :
             return ListMerchantsResponse(
                 client_name = '0', 
                 clientid = 'PC12345', 
                 merchants = [
                     Merchant(
```

### Comparing `citypay_api_client-1.1.1/test/test_mcc6012.py` & `citypay_api_client-1.1.4/test/test_mcc6012.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.mcc6012 import MCC6012  # noqa: E501
+from citypay.models.mcc6012 import MCC6012  # noqa: E501
 
 
 class TestMCC6012(unittest.TestCase):
     """MCC6012 unit test stubs"""
 
     def setUp(self):
         pass
@@ -25,15 +25,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test MCC6012
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.mcc6012.MCC6012()  # noqa: E501
+        # model = citypay.models.mcc6012.MCC6012()  # noqa: E501
 
         if include_optional :
             return MCC6012(
                 recipient_account = '0', 
                 recipient_dob = '0', 
                 recipient_lastname = '0', 
                 recipient_postcode = '0'
```

### Comparing `citypay_api_client-1.1.1/test/test_merchant.py` & `citypay_api_client-1.1.4/test/test_merchant.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.merchant import Merchant  # noqa: E501
+from citypay.models.merchant import Merchant  # noqa: E501
 from citypay.rest import ApiException
 
 
 class TestMerchant(unittest.TestCase):
     """Merchant unit test stubs"""
 
     def setUp(self):
@@ -25,15 +25,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test Merchant
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.merchant.Merchant()  # noqa: E501
+        # model = citypay.models.merchant.Merchant()  # noqa: E501
 
         if include_optional:
             return Merchant(
                 currency='GBP',
                 merchantid=11223344,
                 name='Merchant 1',
                 status='A',
```

### Comparing `citypay_api_client-1.1.1/test/test_operational_functions_api.py` & `citypay_api_client-1.1.4/test/test_operational_functions_api.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/test/test_pa_res_auth_request.py` & `citypay_api_client-1.1.4/test/test_pa_res_auth_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.pa_res_auth_request import PaResAuthRequest  # noqa: E501
+from citypay.models.pa_res_auth_request import PaResAuthRequest  # noqa: E501
 
 
 class TestPaResAuthRequest(unittest.TestCase):
     """PaResAuthRequest unit test stubs"""
 
     def setUp(self):
         pass
@@ -24,15 +24,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test PaResAuthRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.pa_res_auth_request.PaResAuthRequest()  # noqa: E501
+        # model = citypay.models.pa_res_auth_request.PaResAuthRequest()  # noqa: E501
 
         if include_optional:
             return PaResAuthRequest(
                 md='0',
                 pares='v66ycfSp8jNlvy7PkHbx44NEt3vox90+vZ/7Ll05Vid/jPfQn8adw+4D/vRDUGT19kndW97Hfirb...'
             )
         else:
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_address.py` & `citypay_api_client-1.1.4/test/test_paylink_attachment_result.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_address import PaylinkAddress
+from citypay.models.paylink_attachment_result import PaylinkAttachmentResult
 
 
-class TestPaylinkAddress(unittest.TestCase):
-    """PaylinkAddress unit test stubs"""
+class TestPaylinkAttachmentResult(unittest.TestCase):
+    """PaylinkAttachmentResult unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPaylinkAddress(self):
-        """Test PaylinkAddress"""
+    def testPaylinkAttachmentResult(self):
+        """Test PaylinkAttachmentResult"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PaylinkAddress()  # noqa: E501
+        # model = PaylinkAttachmentResult()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_adjustment_request.py` & `citypay_api_client-1.1.4/test/test_paylink_adjustment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_adjustment_request import PaylinkAdjustmentRequest
+from citypay.models.paylink_adjustment_request import PaylinkAdjustmentRequest
 
 
 class TestPaylinkAdjustmentRequest(unittest.TestCase):
     """PaylinkAdjustmentRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_api.py` & `citypay_api_client-1.1.4/test/test_paylink_api.py`

 * *Files identical despite different names*

### Comparing `citypay_api_client-1.1.1/test/test_paylink_attachment_request.py` & `citypay_api_client-1.1.4/test/test_paylink_attachment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_attachment_request import PaylinkAttachmentRequest
+from citypay.models.paylink_attachment_request import PaylinkAttachmentRequest
 
 
 class TestPaylinkAttachmentRequest(unittest.TestCase):
     """PaylinkAttachmentRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_attachment_result.py` & `citypay_api_client-1.1.4/test/test_paylink_token_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_attachment_result import PaylinkAttachmentResult
+from citypay.models.paylink_state_event import PaylinkStateEvent
+globals()['PaylinkStateEvent'] = PaylinkStateEvent
+from citypay.models.paylink_token_status import PaylinkTokenStatus
 
 
-class TestPaylinkAttachmentResult(unittest.TestCase):
-    """PaylinkAttachmentResult unit test stubs"""
+class TestPaylinkTokenStatus(unittest.TestCase):
+    """PaylinkTokenStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPaylinkAttachmentResult(self):
-        """Test PaylinkAttachmentResult"""
+    def testPaylinkTokenStatus(self):
+        """Test PaylinkTokenStatus"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PaylinkAttachmentResult()  # noqa: E501
+        # model = PaylinkTokenStatus()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_bill_payment_token_request.py` & `citypay_api_client-1.1.4/test/test_paylink_bill_payment_token_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_attachment_request import PaylinkAttachmentRequest
-from citypay.model.paylink_email_notification_path import PaylinkEmailNotificationPath
-from citypay.model.paylink_sms_notification_path import PaylinkSMSNotificationPath
-from citypay.model.paylink_token_request_model import PaylinkTokenRequestModel
+from citypay.models.paylink_attachment_request import PaylinkAttachmentRequest
+from citypay.models.paylink_email_notification_path import PaylinkEmailNotificationPath
+from citypay.models.paylink_sms_notification_path import PaylinkSMSNotificationPath
+from citypay.models.paylink_token_request_model import PaylinkTokenRequestModel
 globals()['PaylinkAttachmentRequest'] = PaylinkAttachmentRequest
 globals()['PaylinkEmailNotificationPath'] = PaylinkEmailNotificationPath
 globals()['PaylinkSMSNotificationPath'] = PaylinkSMSNotificationPath
 globals()['PaylinkTokenRequestModel'] = PaylinkTokenRequestModel
-from citypay.model.paylink_bill_payment_token_request import PaylinkBillPaymentTokenRequest
+from citypay.models.paylink_bill_payment_token_request import PaylinkBillPaymentTokenRequest
 
 
 class TestPaylinkBillPaymentTokenRequest(unittest.TestCase):
     """PaylinkBillPaymentTokenRequest unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_card_holder.py` & `citypay_api_client-1.1.4/test/test_paylink_card_holder.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_address import PaylinkAddress
+from citypay.models.paylink_address import PaylinkAddress
 globals()['PaylinkAddress'] = PaylinkAddress
-from citypay.model.paylink_card_holder import PaylinkCardHolder
+from citypay.models.paylink_card_holder import PaylinkCardHolder
 
 
 class TestPaylinkCardHolder(unittest.TestCase):
     """PaylinkCardHolder unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_cart.py` & `citypay_api_client-1.1.4/test/test_paylink_cart.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_cart_item_model import PaylinkCartItemModel
+from citypay.models.paylink_cart_item_model import PaylinkCartItemModel
 globals()['PaylinkCartItemModel'] = PaylinkCartItemModel
-from citypay.model.paylink_cart import PaylinkCart
+from citypay.models.paylink_cart import PaylinkCart
 
 
 class TestPaylinkCart(unittest.TestCase):
     """PaylinkCart unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_cart_item_model.py` & `citypay_api_client-1.1.4/test/test_paylink_cart_item_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_cart_item_model import PaylinkCartItemModel
+from citypay.models.paylink_cart_item_model import PaylinkCartItemModel
 
 
 class TestPaylinkCartItemModel(unittest.TestCase):
     """PaylinkCartItemModel unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_config.py` & `citypay_api_client-1.1.4/test/test_paylink_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_custom_param import PaylinkCustomParam
-from citypay.model.paylink_field_guard_model import PaylinkFieldGuardModel
-from citypay.model.paylink_part_payments import PaylinkPartPayments
-from citypay.model.paylink_ui import PaylinkUI
+from citypay.models.paylink_custom_param import PaylinkCustomParam
+from citypay.models.paylink_field_guard_model import PaylinkFieldGuardModel
+from citypay.models.paylink_part_payments import PaylinkPartPayments
+from citypay.models.paylink_ui import PaylinkUI
 globals()['PaylinkCustomParam'] = PaylinkCustomParam
 globals()['PaylinkFieldGuardModel'] = PaylinkFieldGuardModel
 globals()['PaylinkPartPayments'] = PaylinkPartPayments
 globals()['PaylinkUI'] = PaylinkUI
-from citypay.model.paylink_config import PaylinkConfig
+from citypay.models.paylink_config import PaylinkConfig
 
 
 class TestPaylinkConfig(unittest.TestCase):
     """PaylinkConfig unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_custom_param.py` & `citypay_api_client-1.1.4/test/test_paylink_email_notification_path.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_custom_param import PaylinkCustomParam
+from citypay.models.paylink_email_notification_path import PaylinkEmailNotificationPath
 
 
-class TestPaylinkCustomParam(unittest.TestCase):
-    """PaylinkCustomParam unit test stubs"""
+class TestPaylinkEmailNotificationPath(unittest.TestCase):
+    """PaylinkEmailNotificationPath unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPaylinkCustomParam(self):
-        """Test PaylinkCustomParam"""
+    def testPaylinkEmailNotificationPath(self):
+        """Test PaylinkEmailNotificationPath"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PaylinkCustomParam()  # noqa: E501
+        # model = PaylinkEmailNotificationPath()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_email_notification_path.py` & `citypay_api_client-1.1.4/test/test_paylink_sms_notification_path.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_email_notification_path import PaylinkEmailNotificationPath
+from citypay.models.paylink_sms_notification_path import PaylinkSMSNotificationPath
 
 
-class TestPaylinkEmailNotificationPath(unittest.TestCase):
-    """PaylinkEmailNotificationPath unit test stubs"""
+class TestPaylinkSMSNotificationPath(unittest.TestCase):
+    """PaylinkSMSNotificationPath unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPaylinkEmailNotificationPath(self):
-        """Test PaylinkEmailNotificationPath"""
+    def testPaylinkSMSNotificationPath(self):
+        """Test PaylinkSMSNotificationPath"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PaylinkEmailNotificationPath()  # noqa: E501
+        # model = PaylinkSMSNotificationPath()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_error_code.py` & `citypay_api_client-1.1.4/test/test_paylink_error_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_error_code import PaylinkErrorCode
+from citypay.models.paylink_error_code import PaylinkErrorCode
 
 
 class TestPaylinkErrorCode(unittest.TestCase):
     """PaylinkErrorCode unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_field_guard_model.py` & `citypay_api_client-1.1.4/test/test_paylink_field_guard_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_field_guard_model import PaylinkFieldGuardModel
+from citypay.models.paylink_field_guard_model import PaylinkFieldGuardModel
 
 
 class TestPaylinkFieldGuardModel(unittest.TestCase):
     """PaylinkFieldGuardModel unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_part_payments.py` & `citypay_api_client-1.1.4/test/test_paylink_part_payments.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_part_payments import PaylinkPartPayments
+from citypay.models.paylink_part_payments import PaylinkPartPayments
 
 
 class TestPaylinkPartPayments(unittest.TestCase):
     """PaylinkPartPayments unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_sms_notification_path.py` & `citypay_api_client-1.1.4/test/test_paylink_token_created.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,28 +8,32 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_sms_notification_path import PaylinkSMSNotificationPath
+from citypay.models.paylink_attachment_result import PaylinkAttachmentResult
+from citypay.models.paylink_error_code import PaylinkErrorCode
+globals()['PaylinkAttachmentResult'] = PaylinkAttachmentResult
+globals()['PaylinkErrorCode'] = PaylinkErrorCode
+from citypay.models.paylink_token_created import PaylinkTokenCreated
 
 
-class TestPaylinkSMSNotificationPath(unittest.TestCase):
-    """PaylinkSMSNotificationPath unit test stubs"""
+class TestPaylinkTokenCreated(unittest.TestCase):
+    """PaylinkTokenCreated unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPaylinkSMSNotificationPath(self):
-        """Test PaylinkSMSNotificationPath"""
+    def testPaylinkTokenCreated(self):
+        """Test PaylinkTokenCreated"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PaylinkSMSNotificationPath()  # noqa: E501
+        # model = PaylinkTokenCreated()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_state_event.py` & `citypay_api_client-1.1.4/test/test_paylink_state_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_state_event import PaylinkStateEvent
+from citypay.models.paylink_state_event import PaylinkStateEvent
 
 
 class TestPaylinkStateEvent(unittest.TestCase):
     """PaylinkStateEvent unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_token_created.py` & `citypay_api_client-1.1.4/test/test_paylink_token_status_change_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,32 +8,30 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_attachment_result import PaylinkAttachmentResult
-from citypay.model.paylink_error_code import PaylinkErrorCode
-globals()['PaylinkAttachmentResult'] = PaylinkAttachmentResult
-globals()['PaylinkErrorCode'] = PaylinkErrorCode
-from citypay.model.paylink_token_created import PaylinkTokenCreated
+from citypay.models.paylink_token_status import PaylinkTokenStatus
+globals()['PaylinkTokenStatus'] = PaylinkTokenStatus
+from citypay.models.paylink_token_status_change_response import PaylinkTokenStatusChangeResponse
 
 
-class TestPaylinkTokenCreated(unittest.TestCase):
-    """PaylinkTokenCreated unit test stubs"""
+class TestPaylinkTokenStatusChangeResponse(unittest.TestCase):
+    """PaylinkTokenStatusChangeResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPaylinkTokenCreated(self):
-        """Test PaylinkTokenCreated"""
+    def testPaylinkTokenStatusChangeResponse(self):
+        """Test PaylinkTokenStatusChangeResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PaylinkTokenCreated()  # noqa: E501
+        # model = PaylinkTokenStatusChangeResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_token_request_model.py` & `citypay_api_client-1.1.4/test/test_paylink_token_request_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_card_holder import PaylinkCardHolder
-from citypay.model.paylink_cart import PaylinkCart
-from citypay.model.paylink_config import PaylinkConfig
+from citypay.models.paylink_card_holder import PaylinkCardHolder
+from citypay.models.paylink_cart import PaylinkCart
+from citypay.models.paylink_config import PaylinkConfig
 globals()['PaylinkCardHolder'] = PaylinkCardHolder
 globals()['PaylinkCart'] = PaylinkCart
 globals()['PaylinkConfig'] = PaylinkConfig
-from citypay.model.paylink_token_request_model import PaylinkTokenRequestModel
+from citypay.models.paylink_token_request_model import PaylinkTokenRequestModel
 
 
 class TestPaylinkTokenRequestModel(unittest.TestCase):
     """PaylinkTokenRequestModel unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_token_status.py` & `citypay_api_client-1.1.4/test/test_paylink_token_status_change_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,30 +8,28 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_state_event import PaylinkStateEvent
-globals()['PaylinkStateEvent'] = PaylinkStateEvent
-from citypay.model.paylink_token_status import PaylinkTokenStatus
+from citypay.models.paylink_token_status_change_request import PaylinkTokenStatusChangeRequest
 
 
-class TestPaylinkTokenStatus(unittest.TestCase):
-    """PaylinkTokenStatus unit test stubs"""
+class TestPaylinkTokenStatusChangeRequest(unittest.TestCase):
+    """PaylinkTokenStatusChangeRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPaylinkTokenStatus(self):
-        """Test PaylinkTokenStatus"""
+    def testPaylinkTokenStatusChangeRequest(self):
+        """Test PaylinkTokenStatusChangeRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PaylinkTokenStatus()  # noqa: E501
+        # model = PaylinkTokenStatusChangeRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_token_status_change_request.py` & `citypay_api_client-1.1.4/test/test_process_batch_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 """
     CityPay Payment API
 
-     This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security Your application will need to adhere to PCI-DSS standards to operate safely and to meet requirements set out by  Visa and MasterCard and the PCI Security Standards Council. These include  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
+     This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security <aside class=\"notice\">   Before we begin a reminder that your application will need to adhere to PCI-DSS standards to operate safely   and to meet requirements set out by Visa and MasterCard and the PCI Security Standards Council including: </aside>  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
-
-import citypay
-from citypay.model.paylink_token_status_change_request import PaylinkTokenStatusChangeRequest
+from citypay.models.batch_transaction import BatchTransaction
+globals()['BatchTransaction'] = BatchTransaction
 
 
-class TestPaylinkTokenStatusChangeRequest(unittest.TestCase):
-    """PaylinkTokenStatusChangeRequest unit test stubs"""
+class TestProcessBatchRequest(unittest.TestCase):
+    """ProcessBatchRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPaylinkTokenStatusChangeRequest(self):
-        """Test PaylinkTokenStatusChangeRequest"""
+    def testProcessBatchRequest(self):
+        """Test ProcessBatchRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PaylinkTokenStatusChangeRequest()  # noqa: E501
+        # model = ProcessBatchRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_token_status_change_response.py` & `citypay_api_client-1.1.4/test/test_process_batch_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 """
     CityPay Payment API
 
-     This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security Your application will need to adhere to PCI-DSS standards to operate safely and to meet requirements set out by  Visa and MasterCard and the PCI Security Standards Council. These include  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
+     This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security <aside class=\"notice\">   Before we begin a reminder that your application will need to adhere to PCI-DSS standards to operate safely   and to meet requirements set out by Visa and MasterCard and the PCI Security Standards Council including: </aside>  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
-
-import sys
 import unittest
 
-import citypay
-from citypay.model.paylink_token_status import PaylinkTokenStatus
-globals()['PaylinkTokenStatus'] = PaylinkTokenStatus
-from citypay.model.paylink_token_status_change_response import PaylinkTokenStatusChangeResponse
-
 
-class TestPaylinkTokenStatusChangeResponse(unittest.TestCase):
-    """PaylinkTokenStatusChangeResponse unit test stubs"""
+class TestProcessBatchResponse(unittest.TestCase):
+    """ProcessBatchResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPaylinkTokenStatusChangeResponse(self):
-        """Test PaylinkTokenStatusChangeResponse"""
+    def testProcessBatchResponse(self):
+        """Test ProcessBatchResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PaylinkTokenStatusChangeResponse()  # noqa: E501
+        # model = ProcessBatchResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_paylink_ui.py` & `citypay_api_client-1.1.4/test/test_tokenisation_response_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 """
 
 
 import sys
 import unittest
 
 import citypay
-from citypay.model.paylink_ui import PaylinkUI
+from citypay.models.tokenisation_response_model import TokenisationResponseModel
 
 
-class TestPaylinkUI(unittest.TestCase):
-    """PaylinkUI unit test stubs"""
+class TestTokenisationResponseModel(unittest.TestCase):
+    """TokenisationResponseModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPaylinkUI(self):
-        """Test PaylinkUI"""
+    def testTokenisationResponseModel(self):
+        """Test TokenisationResponseModel"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PaylinkUI()  # noqa: E501
+        # model = TokenisationResponseModel()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_ping.py` & `citypay_api_client-1.1.4/test/test_ping.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.ping import Ping  # noqa: E501
+from citypay.models.ping import Ping  # noqa: E501
 
 
 class TestPing(unittest.TestCase):
     """Ping unit test stubs"""
 
     def setUp(self):
         pass
@@ -24,15 +24,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test Ping
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.ping.Ping()  # noqa: E501
+        # model = citypay.models.ping.Ping()  # noqa: E501
 
         if include_optional:
             return Ping(
                 identifier='95b857a1-5955-4b86-963c-5a6dbfc4fb95'
             )
         else:
             return Ping(
```

### Comparing `citypay_api_client-1.1.1/test/test_process_batch_request.py` & `citypay_api_client-1.1.4/test/test_void_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,51 @@
+# coding: utf-8
+
 """
     CityPay Payment API
 
      This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security <aside class=\"notice\">   Before we begin a reminder that your application will need to adhere to PCI-DSS standards to operate safely   and to meet requirements set out by Visa and MasterCard and the PCI Security Standards Council including: </aside>  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
+from __future__ import absolute_import
 import unittest
-from citypay.model.batch_transaction import BatchTransaction
-globals()['BatchTransaction'] = BatchTransaction
+from citypay.models.void_request import VoidRequest  # noqa: E501
 
 
-class TestProcessBatchRequest(unittest.TestCase):
-    """ProcessBatchRequest unit test stubs"""
+class TestVoidRequest(unittest.TestCase):
+    """VoidRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProcessBatchRequest(self):
-        """Test ProcessBatchRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ProcessBatchRequest()  # noqa: E501
-        pass
+    def make_instance(self, include_optional):
+        """Test VoidRequest
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # model = citypay.models.void_request.VoidRequest()  # noqa: E501
+
+        if include_optional:
+            return VoidRequest(
+                identifier='95b857a1-5955-4b86-963c-5a6dbfc4fb95',
+                merchantid=11223344,
+                transno=78416
+            )
+        else:
+            return VoidRequest(
+                merchantid=11223344,
+            )
+
+    def testVoidRequest(self):
+        """Test VoidRequest"""
+        inst_req_only = self.make_instance(include_optional=False)
+        inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_process_batch_response.py` & `citypay_api_client-1.1.4/test/test_refund_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,57 @@
+# coding: utf-8
+
 """
     CityPay Payment API
 
      This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security <aside class=\"notice\">   Before we begin a reminder that your application will need to adhere to PCI-DSS standards to operate safely   and to meet requirements set out by Visa and MasterCard and the PCI Security Standards Council including: </aside>  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
+
+from __future__ import absolute_import
 import unittest
+from citypay.models.refund_request import RefundRequest  # noqa: E501
 
 
-class TestProcessBatchResponse(unittest.TestCase):
-    """ProcessBatchResponse unit test stubs"""
+class TestRefundRequest(unittest.TestCase):
+    """RefundRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProcessBatchResponse(self):
-        """Test ProcessBatchResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ProcessBatchResponse()  # noqa: E501
-        pass
+    def make_instance(self, include_optional):
+        """Test RefundRequest
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # model = citypay.models.refund_request.RefundRequest()  # noqa: E501
+
+        if include_optional :
+            return RefundRequest(
+                amount = 3600, 
+                identifier = '95b857a1-5955-4b86-963c-5a6dbfc4fb95', 
+                merchantid = 11223344, 
+                refund_ref = 8322, 
+                trans_info = '0'
+            )
+        else :
+            return RefundRequest(
+                amount = 3600,
+                identifier = '95b857a1-5955-4b86-963c-5a6dbfc4fb95',
+                merchantid = 11223344,
+                refund_ref = 8322,
+        )
+
+    def testRefundRequest(self):
+        """Test RefundRequest"""
+        inst_req_only = self.make_instance(include_optional=False)
+        inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_refund_request.py` & `citypay_api_client-1.1.4/test/test_three_d_secure.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,53 +5,48 @@
 
      This CityPay API is a HTTP RESTful payment API used for direct server to server transactional processing. It provides a number of payment mechanisms including: Internet, MOTO, Continuous Authority transaction processing, 3-D Secure decision handling using RFA Secure, Authorisation, Refunding, Pre-Authorisation, Cancellation/Voids and Completion processing. The API is also capable of tokinsed payments using Card Holder Accounts.  ## Compliance and Security <aside class=\"notice\">   Before we begin a reminder that your application will need to adhere to PCI-DSS standards to operate safely   and to meet requirements set out by Visa and MasterCard and the PCI Security Standards Council including: </aside>  * Data must be collected using TLS version 1.2 using [strong cryptography](#enabled-tls-ciphers). We will not accept calls to our API at   lower grade encryption levels. We regularly scan our TLS endpoints for vulnerabilities and perform TLS assessments   as part of our compliance program. * The application must not store sensitive card holder data (CHD) such as the card security code (CSC) or   primary access number (PAN) * The application must not display the full card number on receipts, it is recommended to mask the PAN   and show the last 4 digits. The API will return this for you for ease of receipt creation * If you are developing a website, you will be required to perform regular scans on the network where you host the   application to meet your compliance obligations * You will be required to be PCI Compliant and the application must adhere to the security standard. Further information   is available from [https://www.pcisecuritystandards.org/](https://www.pcisecuritystandards.org/) * The API verifies that the request is for a valid account and originates from a trusted source using the remote IP   address. Our application firewalls analyse data that may be an attempt to break a large number of security common   security vulnerabilities.   # noqa: E501
 
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
-
 from __future__ import absolute_import
 import unittest
-from citypay.model.refund_request import RefundRequest  # noqa: E501
+from citypay.models.three_d_secure import ThreeDSecure  # noqa: E501
 
 
-class TestRefundRequest(unittest.TestCase):
-    """RefundRequest unit test stubs"""
+class TestThreeDSecure(unittest.TestCase):
+    """ThreeDSecure unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test RefundRequest
+        """Test ThreeDSecure
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.refund_request.RefundRequest()  # noqa: E501
+        # model = citypay.models.three_d_secure.ThreeDSecure()  # noqa: E501
 
-        if include_optional :
-            return RefundRequest(
-                amount = 3600, 
-                identifier = '95b857a1-5955-4b86-963c-5a6dbfc4fb95', 
-                merchantid = 11223344, 
-                refund_ref = 8322, 
-                trans_info = '0'
+        if include_optional:
+            return ThreeDSecure(
+                accept_headers='text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
+                downgrade1=True,
+                merchant_termurl='0',
+                tds_policy='0',
+                user_agent='Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.149 Safari/537.36'
+            )
+        else:
+            return ThreeDSecure(
             )
-        else :
-            return RefundRequest(
-                amount = 3600,
-                identifier = '95b857a1-5955-4b86-963c-5a6dbfc4fb95',
-                merchantid = 11223344,
-                refund_ref = 8322,
-        )
 
-    def testRefundRequest(self):
-        """Test RefundRequest"""
+    def testThreeDSecure(self):
+        """Test ThreeDSecure"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `citypay_api_client-1.1.1/test/test_register_card.py` & `citypay_api_client-1.1.4/test/test_register_card.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 import unittest
-from citypay.model.register_card import RegisterCard  # noqa: E501
+from citypay.models.register_card import RegisterCard  # noqa: E501
 
 
 class TestRegisterCard(unittest.TestCase):
     """RegisterCard unit test stubs"""
 
     def setUp(self):
         pass
@@ -25,15 +25,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test RegisterCard
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.register_card.RegisterCard()  # noqa: E501
+        # model = citypay.models.register_card.RegisterCard()  # noqa: E501
         if include_optional :
             return RegisterCard(
                 cardnumber = '4000 0000 0000 0002', 
                 default = True, 
                 expmonth = 9, 
                 expyear = 2023
             )
```

### Comparing `citypay_api_client-1.1.1/test/test_request_challenged.py` & `citypay_api_client-1.1.4/test/test_request_challenged.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import unittest
-from citypay.model.request_challenged import RequestChallenged  # noqa: E501
+from citypay.models.request_challenged import RequestChallenged  # noqa: E501
 
 
 class TestRequestChallenged(unittest.TestCase):
     """RequestChallenged unit test stubs"""
 
     def setUp(self):
         pass
@@ -25,15 +25,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test RequestChallenged
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.request_challenged.RequestChallenged()  # noqa: E501
+        # model = citypay.models.request_challenged.RequestChallenged()  # noqa: E501
 
         if include_optional:
             return RequestChallenged(
                 acs_url='https://acs.cardissuer.com/3dsv1',
                 creq='0',
                 merchantid=11223344,
                 threedserver_trans_id='0',
```

### Comparing `citypay_api_client-1.1.1/test/test_retrieve_request.py` & `citypay_api_client-1.1.4/test/test_retrieve_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Contact: support@citypay.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import unittest
-from citypay.model.retrieve_request import RetrieveRequest  # noqa: E501
+from citypay.models.retrieve_request import RetrieveRequest  # noqa: E501
 
 
 class TestRetrieveRequest(unittest.TestCase):
     """RetrieveRequest unit test stubs"""
 
     def setUp(self):
         pass
@@ -25,15 +25,15 @@
         pass
 
     def make_instance(self, include_optional):
         """Test RetrieveRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = citypay.model.retrieve_request.RetrieveRequest()  # noqa: E501
+        # model = citypay.models.retrieve_request.RetrieveRequest()  # noqa: E501
         if include_optional:
             return RetrieveRequest(
                 identifier='95b857a1-5955-4b86-963c-5a6dbfc4fb95',
                 merchantid=11223344,
                 transno=78416
             )
         else:
```

