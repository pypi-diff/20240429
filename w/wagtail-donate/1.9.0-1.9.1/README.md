# Comparing `tmp/wagtail-donate-1.9.0.tar.gz` & `tmp/wagtail-donate-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-donate-1.9.0.tar", last modified: Wed Mar 13 15:32:00 2024, max compression
+gzip compressed data, was "wagtail-donate-1.9.1.tar", last modified: Mon Apr 29 15:59:56 2024, max compression
```

## Comparing `wagtail-donate-1.9.0.tar` & `wagtail-donate-1.9.1.tar`

### file list

```diff
@@ -1,159 +1,177 @@
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.048167 wagtail-donate-1.9.0/
--rw-r--r--   0 nick       (502) staff       (20)     3823 2024-03-13 15:31:11.000000 wagtail-donate-1.9.0/CHANGELOG.md
--rw-r--r--   0 nick       (502) staff       (20)      230 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/LICENSE.txt
--rw-r--r--   0 nick       (502) staff       (20)      155 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/MANIFEST.in
--rw-r--r--   0 nick       (502) staff       (20)     1997 2024-03-13 15:32:00.048098 wagtail-donate-1.9.0/PKG-INFO
--rw-r--r--   0 nick       (502) staff       (20)      895 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/README.md
--rw-r--r--   0 nick       (502) staff       (20)     1975 2024-03-13 15:32:00.048483 wagtail-donate-1.9.0/setup.cfg
--rw-r--r--   0 nick       (502) staff       (20)       38 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/setup.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.047253 wagtail-donate-1.9.0/wagtail_donate.egg-info/
--rw-r--r--   0 nick       (502) staff       (20)     1997 2024-03-13 15:32:00.000000 wagtail-donate-1.9.0/wagtail_donate.egg-info/PKG-INFO
--rw-r--r--   0 nick       (502) staff       (20)     5920 2024-03-13 15:32:00.000000 wagtail-donate-1.9.0/wagtail_donate.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (502) staff       (20)        1 2024-03-13 15:32:00.000000 wagtail-donate-1.9.0/wagtail_donate.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (502) staff       (20)      423 2024-03-13 15:32:00.000000 wagtail-donate-1.9.0/wagtail_donate.egg-info/requires.txt
--rw-r--r--   0 nick       (502) staff       (20)       14 2024-03-13 15:32:00.000000 wagtail-donate-1.9.0/wagtail_donate.egg-info/top_level.txt
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.033564 wagtail-donate-1.9.0/wagtaildonate/
--rw-r--r--   0 nick       (502) staff       (20)      401 2024-03-13 15:31:11.000000 wagtail-donate-1.9.0/wagtaildonate/__init__.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.034139 wagtail-donate-1.9.0/wagtaildonate/address_lookups/
--rw-r--r--   0 nick       (502) staff       (20)        0 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/address_lookups/__init__.py
--rw-r--r--   0 nick       (502) staff       (20)      429 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/address_lookups/base.py
--rw-r--r--   0 nick       (502) staff       (20)      276 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/address_lookups/generic.py
--rw-r--r--   0 nick       (502) staff       (20)      641 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/address_lookups/loqate.py
--rw-r--r--   0 nick       (502) staff       (20)      469 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/address_lookups/utils.py
--rw-r--r--   0 nick       (502) staff       (20)     2649 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/admin_forms.py
--rw-r--r--   0 nick       (502) staff       (20)      631 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/admin_urls.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.034374 wagtail-donate-1.9.0/wagtaildonate/admin_views/
--rw-r--r--   0 nick       (502) staff       (20)        0 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/admin_views/__init__.py
--rw-r--r--   0 nick       (502) staff       (20)     8724 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/admin_views/export.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.034756 wagtail-donate-1.9.0/wagtaildonate/api/
--rw-r--r--   0 nick       (502) staff       (20)        0 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/__init__.py
--rw-r--r--   0 nick       (502) staff       (20)      150 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/metadata.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.035825 wagtail-donate-1.9.0/wagtaildonate/api/serializers/
--rw-r--r--   0 nick       (502) staff       (20)        0 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/serializers/__init__.py
--rw-r--r--   0 nick       (502) staff       (20)     9336 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/serializers/braintree.py
--rw-r--r--   0 nick       (502) staff       (20)     1396 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/serializers/configuration.py
--rw-r--r--   0 nick       (502) staff       (20)     5025 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/serializers/donations.py
--rw-r--r--   0 nick       (502) staff       (20)     7083 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/serializers/gocardless.py
--rw-r--r--   0 nick       (502) staff       (20)     1759 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/serializers/payment_method.py
--rw-r--r--   0 nick       (502) staff       (20)     1680 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/serializers/recaptcha.py
--rw-r--r--   0 nick       (502) staff       (20)     1885 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/serializers/utils.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.036288 wagtail-donate-1.9.0/wagtaildonate/api/tests/
--rw-r--r--   0 nick       (502) staff       (20)        0 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/tests/__init__.py
--rw-r--r--   0 nick       (502) staff       (20)    25728 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/tests/test_serializers.py
--rw-r--r--   0 nick       (502) staff       (20)      471 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/tests/test_utils.py
--rw-r--r--   0 nick       (502) staff       (20)     3797 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/tests/test_views.py
--rw-r--r--   0 nick       (502) staff       (20)      441 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/urls.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.036613 wagtail-donate-1.9.0/wagtaildonate/api/views/
--rw-r--r--   0 nick       (502) staff       (20)        0 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/views/__init__.py
--rw-r--r--   0 nick       (502) staff       (20)     3013 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/views/configuration.py
--rw-r--r--   0 nick       (502) staff       (20)     6161 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/api/views/donations.py
--rw-r--r--   0 nick       (502) staff       (20)      155 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/apps.py
--rw-r--r--   0 nick       (502) staff       (20)      555 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/blocks.py
--rw-r--r--   0 nick       (502) staff       (20)     2277 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/configuration.py
--rw-r--r--   0 nick       (502) staff       (20)      174 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/constants.py
--rw-r--r--   0 nick       (502) staff       (20)      649 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/countries.py
--rw-r--r--   0 nick       (502) staff       (20)       98 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/exceptions.py
--rw-r--r--   0 nick       (502) staff       (20)     3210 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/factories.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.036762 wagtail-donate-1.9.0/wagtaildonate/management/
--rw-r--r--   0 nick       (502) staff       (20)        0 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/management/__init__.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.036950 wagtail-donate-1.9.0/wagtaildonate/management/commands/
--rw-r--r--   0 nick       (502) staff       (20)        0 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/management/commands/__init__.py
--rw-r--r--   0 nick       (502) staff       (20)     2503 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/management/commands/update_transaction_status.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.041428 wagtail-donate-1.9.0/wagtaildonate/migrations/
--rw-r--r--   0 nick       (502) staff       (20)     9212 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0001_initial.py
--rw-r--r--   0 nick       (502) staff       (20)     1137 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0002_add_fundraising_pay_in_fields.py
--rw-r--r--   0 nick       (502) staff       (20)      982 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0003_donation.py
--rw-r--r--   0 nick       (502) staff       (20)     1682 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0004_thank_you_fields.py
--rw-r--r--   0 nick       (502) staff       (20)     2553 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0005_add_contact_details_fields.py
--rw-r--r--   0 nick       (502) staff       (20)      470 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0006_donation_amount.py
--rw-r--r--   0 nick       (502) staff       (20)      527 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0007_country.py
--rw-r--r--   0 nick       (502) staff       (20)      743 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0008_donation_giftaid_organisation.py
--rw-r--r--   0 nick       (502) staff       (20)      750 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0009_donation_memory.py
--rw-r--r--   0 nick       (502) staff       (20)      446 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0010_donation_payment_method.py
--rw-r--r--   0 nick       (502) staff       (20)      496 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0011_donation_rename_address_lines.py
--rw-r--r--   0 nick       (502) staff       (20)      906 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0012_donation_transaction_status_choices.py
--rw-r--r--   0 nick       (502) staff       (20)     1351 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0013_donation_export_log.py
--rw-r--r--   0 nick       (502) staff       (20)      596 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0014_donation_created_at.py
--rw-r--r--   0 nick       (502) staff       (20)    16647 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0015_recurringdonation.py
--rw-r--r--   0 nick       (502) staff       (20)     2030 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0016_thank_you_emails.py
--rw-r--r--   0 nick       (502) staff       (20)     1049 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0017_donation_donation_page.py
--rw-r--r--   0 nick       (502) staff       (20)     1307 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0018_phonenumber_not_mandatory.py
--rw-r--r--   0 nick       (502) staff       (20)      957 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0019_create_at_to_use_default_timezone_now.py
--rw-r--r--   0 nick       (502) staff       (20)     1057 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0020_add_export_permissions.py
--rw-r--r--   0 nick       (502) staff       (20)     1507 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0021_checkout_hero.py
--rw-r--r--   0 nick       (502) staff       (20)    11550 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0022_thank_you_page_content.py
--rw-r--r--   0 nick       (502) staff       (20)     1870 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0023_optins.py
--rw-r--r--   0 nick       (502) staff       (20)     1253 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0024_donationexportlog_default_permissions.py
--rw-r--r--   0 nick       (502) staff       (20)     1160 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0025_donationexportlog_user_info.py
--rw-r--r--   0 nick       (502) staff       (20)     1236 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0026_thankyouemailcontent_not_mandatory.py
--rw-r--r--   0 nick       (502) staff       (20)      847 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0027_thank_you_email_subject_not_mandatory.py
--rw-r--r--   0 nick       (502) staff       (20)    19042 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0028_payin.py
--rw-r--r--   0 nick       (502) staff       (20)      366 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0029_rename_donation_model_to_single_donation.py
--rw-r--r--   0 nick       (502) staff       (20)      979 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0030_addressline3.py
--rw-r--r--   0 nick       (502) staff       (20)     1787 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0031_remove_conrete_models.py
--rw-r--r--   0 nick       (502) staff       (20)     1549 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0032_payin_events.py
--rw-r--r--   0 nick       (502) staff       (20)     1359 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0033_three_d_secure_fields.py
--rw-r--r--   0 nick       (502) staff       (20)     1436 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/0034_alter_thankyouctasnippet_link.py
--rw-r--r--   0 nick       (502) staff       (20)        0 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/migrations/__init__.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.042406 wagtail-donate-1.9.0/wagtaildonate/models/
--rw-r--r--   0 nick       (502) staff       (20)     1686 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/models/__init__.py
--rw-r--r--   0 nick       (502) staff       (20)     8112 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/models/donations.py
--rw-r--r--   0 nick       (502) staff       (20)     1463 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/models/export.py
--rw-r--r--   0 nick       (502) staff       (20)    15402 2024-03-13 15:22:57.000000 wagtail-donate-1.9.0/wagtaildonate/models/pages.py
--rw-r--r--   0 nick       (502) staff       (20)      719 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/models/pay_in_events.py
--rw-r--r--   0 nick       (502) staff       (20)      362 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/models/query.py
--rw-r--r--   0 nick       (502) staff       (20)     2345 2024-03-13 15:22:57.000000 wagtail-donate-1.9.0/wagtaildonate/models/snippets.py
--rw-r--r--   0 nick       (502) staff       (20)     2265 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/models/utils.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.043008 wagtail-donate-1.9.0/wagtaildonate/payment_methods/
--rw-r--r--   0 nick       (502) staff       (20)        0 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/payment_methods/__init__.py
--rw-r--r--   0 nick       (502) staff       (20)     1598 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/payment_methods/base.py
--rw-r--r--   0 nick       (502) staff       (20)     8557 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/payment_methods/braintree.py
--rw-r--r--   0 nick       (502) staff       (20)      569 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/payment_methods/gocardless.py
--rw-r--r--   0 nick       (502) staff       (20)     1411 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/payment_methods/utils.py
--rw-r--r--   0 nick       (502) staff       (20)     2379 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/settings.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.029833 wagtail-donate-1.9.0/wagtaildonate/templates/
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.043894 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.044010 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/admin/
--rw-r--r--   0 nick       (502) staff       (20)      718 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/admin/export_view.html
--rw-r--r--   0 nick       (502) staff       (20)       84 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/base_donate.html
--rw-r--r--   0 nick       (502) staff       (20)     2051 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/checkout.html
--rw-r--r--   0 nick       (502) staff       (20)     1077 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/donation_campaign_page.html
--rw-r--r--   0 nick       (502) staff       (20)     1096 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/donation_fundraising_pay_in_page.html
--rw-r--r--   0 nick       (502) staff       (20)     1107 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/donation_page.html
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.044245 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/email/
--rw-r--r--   0 nick       (502) staff       (20)      347 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/email/thank_you.html
--rw-r--r--   0 nick       (502) staff       (20)      326 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/email/thank_you.txt
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.044370 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/includes/
--rw-r--r--   0 nick       (502) staff       (20)      671 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/includes/checkout_form.html
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.044615 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/includes/forms/
--rw-r--r--   0 nick       (502) staff       (20)     1068 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/includes/forms/donate_step_one.html
--rw-r--r--   0 nick       (502) staff       (20)      420 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/includes/forms/donate_step_one_fundraising_pay_in.html
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.030277 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/streamfield/
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.045358 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/streamfield/blocks/
--rw-r--r--   0 nick       (502) staff       (20)      113 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/streamfield/blocks/document_block.html
--rw-r--r--   0 nick       (502) staff       (20)       90 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/streamfield/blocks/donate_block.html
--rw-r--r--   0 nick       (502) staff       (20)       21 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/streamfield/blocks/heading_block.html
--rw-r--r--   0 nick       (502) staff       (20)       93 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/streamfield/blocks/image_block.html
--rw-r--r--   0 nick       (502) staff       (20)      121 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/streamfield/blocks/quote_block.html
--rw-r--r--   0 nick       (502) staff       (20)      270 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/streamfield/blocks/thank_you_cta_block.html
--rw-r--r--   0 nick       (502) staff       (20)     1797 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/thank_you.html
--rw-r--r--   0 nick       (502) staff       (20)      624 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/thank_you_fundraising.html
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.045626 wagtail-donate-1.9.0/wagtaildonate/templatetags/
--rw-r--r--   0 nick       (502) staff       (20)        0 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templatetags/__init__.py
--rw-r--r--   0 nick       (502) staff       (20)     1594 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/templatetags/wagtaildonate_tags.py
--rw-r--r--   0 nick       (502) staff       (20)      301 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/transaction_status.py
--rw-r--r--   0 nick       (502) staff       (20)      306 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/urls.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.046514 wagtail-donate-1.9.0/wagtaildonate/utils/
--rw-r--r--   0 nick       (502) staff       (20)        0 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/utils/__init__.py
--rw-r--r--   0 nick       (502) staff       (20)      847 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/utils/assets.py
--rw-r--r--   0 nick       (502) staff       (20)     1495 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/utils/blocks.py
--rw-r--r--   0 nick       (502) staff       (20)     4529 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/utils/braintree.py
--rw-r--r--   0 nick       (502) staff       (20)      354 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/utils/currency.py
--rw-r--r--   0 nick       (502) staff       (20)     3714 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/utils/rich_text.py
--rw-r--r--   0 nick       (502) staff       (20)     7197 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/views.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2024-03-13 15:32:00.047087 wagtail-donate-1.9.0/wagtaildonate/wagtail_hooks/
--rw-r--r--   0 nick       (502) staff       (20)      482 2024-02-27 13:00:18.000000 wagtail-donate-1.9.0/wagtaildonate/wagtail_hooks/__init__.py
--rw-r--r--   0 nick       (502) staff       (20)     2817 2024-03-13 15:31:11.000000 wagtail-donate-1.9.0/wagtaildonate/wagtail_hooks/export.py
--rw-r--r--   0 nick       (502) staff       (20)     2839 2024-03-13 15:31:11.000000 wagtail-donate-1.9.0/wagtaildonate/wagtail_hooks/export_log.py
--rw-r--r--   0 nick       (502) staff       (20)     1166 2024-03-13 15:31:11.000000 wagtail-donate-1.9.0/wagtaildonate/wagtail_hooks/general.py
--rw-r--r--   0 nick       (502) staff       (20)      568 2024-03-13 15:31:11.000000 wagtail-donate-1.9.0/wagtaildonate/wagtail_hooks/pay_in_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.107685 wagtail-donate-1.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)     3881 2024-04-29 11:34:05.000000 wagtail-donate-1.9.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      230 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1190 2024-04-29 15:59:56.107685 wagtail-donate-1.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      895 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1975 2024-04-29 15:59:56.107685 wagtail-donate-1.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.099685 wagtail-donate-1.9.1/wagtail_donate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1190 2024-04-29 15:59:55.000000 wagtail-donate-1.9.1/wagtail_donate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6564 2024-04-29 15:59:55.000000 wagtail-donate-1.9.1/wagtail_donate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 15:59:55.000000 wagtail-donate-1.9.1/wagtail_donate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-29 15:59:55.000000 wagtail-donate-1.9.1/wagtail_donate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-29 15:59:55.000000 wagtail-donate-1.9.1/wagtail_donate.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.099685 wagtail-donate-1.9.1/wagtaildonate/
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-04-29 11:34:05.000000 wagtail-donate-1.9.1/wagtaildonate/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.099685 wagtail-donate-1.9.1/wagtaildonate/address_lookups/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:58:44.000000 wagtail-donate-1.9.1/wagtaildonate/address_lookups/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/address_lookups/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      276 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/address_lookups/generic.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/address_lookups/loqate.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/address_lookups/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2649 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/admin_forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      631 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/admin_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.099685 wagtail-donate-1.9.1/wagtaildonate/admin_views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:58:44.000000 wagtail-donate-1.9.1/wagtaildonate/admin_views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8724 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/admin_views/export.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.099685 wagtail-donate-1.9.1/wagtaildonate/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:58:44.000000 wagtail-donate-1.9.1/wagtaildonate/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      150 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/api/metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.099685 wagtail-donate-1.9.1/wagtaildonate/api/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:58:44.000000 wagtail-donate-1.9.1/wagtaildonate/api/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9336 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/api/serializers/braintree.py
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/api/serializers/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5025 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/api/serializers/donations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7083 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/api/serializers/gocardless.py
+-rw-rw-rw-   0 root         (0) root         (0)     1759 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/api/serializers/payment_method.py
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/api/serializers/recaptcha.py
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/api/serializers/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.099685 wagtail-donate-1.9.1/wagtaildonate/api/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:58:44.000000 wagtail-donate-1.9.1/wagtaildonate/api/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25728 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/api/tests/test_serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/api/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3797 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/api/tests/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/api/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.099685 wagtail-donate-1.9.1/wagtaildonate/api/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:58:44.000000 wagtail-donate-1.9.1/wagtaildonate/api/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3013 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/api/views/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     6161 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/api/views/donations.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      555 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      649 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/countries.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3210 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.099685 wagtail-donate-1.9.1/wagtaildonate/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:58:44.000000 wagtail-donate-1.9.1/wagtaildonate/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.099685 wagtail-donate-1.9.1/wagtaildonate/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:58:44.000000 wagtail-donate-1.9.1/wagtaildonate/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2503 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/management/commands/update_transaction_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.103685 wagtail-donate-1.9.1/wagtaildonate/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     9212 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1137 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0002_add_fundraising_pay_in_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      982 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0003_donation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0004_thank_you_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0005_add_contact_details_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0006_donation_amount.py
+-rw-rw-rw-   0 root         (0) root         (0)      527 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0007_country.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0008_donation_giftaid_organisation.py
+-rw-rw-rw-   0 root         (0) root         (0)      750 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0009_donation_memory.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0010_donation_payment_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      496 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0011_donation_rename_address_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)      906 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0012_donation_transaction_status_choices.py
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0013_donation_export_log.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0014_donation_created_at.py
+-rw-rw-rw-   0 root         (0) root         (0)    16647 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0015_recurringdonation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0016_thank_you_emails.py
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0017_donation_donation_page.py
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0018_phonenumber_not_mandatory.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0019_create_at_to_use_default_timezone_now.py
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0020_add_export_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0021_checkout_hero.py
+-rw-rw-rw-   0 root         (0) root         (0)    11550 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0022_thank_you_page_content.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0023_optins.py
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0024_donationexportlog_default_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0025_donationexportlog_user_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0026_thankyouemailcontent_not_mandatory.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0027_thank_you_email_subject_not_mandatory.py
+-rw-rw-rw-   0 root         (0) root         (0)    19042 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0028_payin.py
+-rw-rw-rw-   0 root         (0) root         (0)      366 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0029_rename_donation_model_to_single_donation.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0030_addressline3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1787 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0031_remove_conrete_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0032_payin_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0033_three_d_secure_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/0034_alter_thankyouctasnippet_link.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:58:44.000000 wagtail-donate-1.9.1/wagtaildonate/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.103685 wagtail-donate-1.9.1/wagtaildonate/models/
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8112 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/models/donations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/models/export.py
+-rw-rw-rw-   0 root         (0) root         (0)    15402 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/models/pages.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/models/pay_in_events.py
+-rw-rw-rw-   0 root         (0) root         (0)      362 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/models/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/models/snippets.py
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/models/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.103685 wagtail-donate-1.9.1/wagtaildonate/payment_methods/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:58:44.000000 wagtail-donate-1.9.1/wagtaildonate/payment_methods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/payment_methods/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8557 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/payment_methods/braintree.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/payment_methods/gocardless.py
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/payment_methods/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2379 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.095685 wagtail-donate-1.9.1/wagtaildonate/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.103685 wagtail-donate-1.9.1/wagtaildonate/static/images/
+-rw-r--r--   0 root         (0) root         (0)     3081 2024-04-29 11:46:15.000000 wagtail-donate-1.9.1/wagtaildonate/static/images/direct-debit.svg
+-rw-r--r--   0 root         (0) root         (0)     4760 2024-04-29 11:46:15.000000 wagtail-donate-1.9.1/wagtaildonate/static/images/fundraising-regulator-logo.svg
+-rw-r--r--   0 root         (0) root         (0)      593 2024-04-29 11:46:15.000000 wagtail-donate-1.9.1/wagtaildonate/static/images/padlock.svg
+-rw-r--r--   0 root         (0) root         (0)     4510 2024-04-29 11:46:15.000000 wagtail-donate-1.9.1/wagtaildonate/static/images/wagtail-logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.095685 wagtail-donate-1.9.1/wagtaildonate/static/wagtaildonate/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.103685 wagtail-donate-1.9.1/wagtaildonate/static/wagtaildonate/css/
+-rw-r--r--   0 root         (0) root         (0)    15716 2024-04-29 11:47:30.000000 wagtail-donate-1.9.1/wagtaildonate/static/wagtaildonate/css/checkout.css
+-rw-r--r--   0 root         (0) root         (0)    15716 2024-04-29 11:47:30.000000 wagtail-donate-1.9.1/wagtaildonate/static/wagtaildonate/css/donate-form.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.103685 wagtail-donate-1.9.1/wagtaildonate/static/wagtaildonate/images/
+-rw-r--r--   0 root         (0) root         (0)     3081 2024-04-29 11:47:30.000000 wagtail-donate-1.9.1/wagtaildonate/static/wagtaildonate/images/direct-debit.svg
+-rw-r--r--   0 root         (0) root         (0)     4760 2024-04-29 11:47:30.000000 wagtail-donate-1.9.1/wagtaildonate/static/wagtaildonate/images/fundraising-regulator-logo.svg
+-rw-r--r--   0 root         (0) root         (0)      593 2024-04-29 11:47:30.000000 wagtail-donate-1.9.1/wagtaildonate/static/wagtaildonate/images/padlock.svg
+-rw-r--r--   0 root         (0) root         (0)     4510 2024-04-29 11:47:30.000000 wagtail-donate-1.9.1/wagtaildonate/static/wagtaildonate/images/wagtail-logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.103685 wagtail-donate-1.9.1/wagtaildonate/static/wagtaildonate/js/
+-rw-r--r--   0 root         (0) root         (0)   316381 2024-04-29 11:47:30.000000 wagtail-donate-1.9.1/wagtaildonate/static/wagtaildonate/js/checkout.js
+-rw-r--r--   0 root         (0) root         (0)   148632 2024-04-29 11:47:30.000000 wagtail-donate-1.9.1/wagtaildonate/static/wagtaildonate/js/donate-form.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.095685 wagtail-donate-1.9.1/wagtaildonate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.103685 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.103685 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/admin/
+-rw-rw-rw-   0 root         (0) root         (0)      718 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/admin/export_view.html
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/base_donate.html
+-rw-rw-rw-   0 root         (0) root         (0)     2051 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/checkout.html
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/donation_campaign_page.html
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/donation_fundraising_pay_in_page.html
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/donation_page.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.103685 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/email/
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/email/thank_you.html
+-rw-rw-rw-   0 root         (0) root         (0)      326 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/email/thank_you.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.103685 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/includes/
+-rw-rw-rw-   0 root         (0) root         (0)      671 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/includes/checkout_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.107685 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/includes/forms/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/includes/forms/donate_step_one.html
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/includes/forms/donate_step_one_fundraising_pay_in.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.095685 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/streamfield/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.107685 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/streamfield/blocks/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/streamfield/blocks/document_block.html
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/streamfield/blocks/donate_block.html
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/streamfield/blocks/heading_block.html
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/streamfield/blocks/image_block.html
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/streamfield/blocks/quote_block.html
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/streamfield/blocks/thank_you_cta_block.html
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/thank_you.html
+-rw-rw-rw-   0 root         (0) root         (0)      624 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/thank_you_fundraising.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.107685 wagtail-donate-1.9.1/wagtaildonate/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:58:44.000000 wagtail-donate-1.9.1/wagtaildonate/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1594 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/templatetags/wagtaildonate_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/transaction_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      306 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.107685 wagtail-donate-1.9.1/wagtaildonate/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:58:44.000000 wagtail-donate-1.9.1/wagtaildonate/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/utils/assets.py
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/utils/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4529 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/utils/braintree.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/utils/currency.py
+-rw-rw-rw-   0 root         (0) root         (0)     3714 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/utils/rich_text.py
+-rw-rw-rw-   0 root         (0) root         (0)     7197 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:59:56.107685 wagtail-donate-1.9.1/wagtaildonate/wagtail_hooks/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/wagtail_hooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2024-04-29 03:51:14.000000 wagtail-donate-1.9.1/wagtaildonate/wagtail_hooks/export.py
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/wagtail_hooks/export_log.py
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2024-04-29 03:51:14.000000 wagtail-donate-1.9.1/wagtaildonate/wagtail_hooks/general.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-03-08 03:13:24.000000 wagtail-donate-1.9.1/wagtaildonate/wagtail_hooks/pay_in_events.py
```

### Comparing `wagtail-donate-1.9.0/CHANGELOG.md` & `wagtail-donate-1.9.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## [1.9.1] - 2024-04-29
+
+-   Fix missing menu item icons
+
 ## [1.9.0] - 2024-03-11
 
 -   Add support for Wagtail 6.0
 -   Add support for Django 5.0
 -   Remove testing for Wagtail 4.1
 -   Drop support for Wagtail < 5.2
```

### Comparing `wagtail-donate-1.9.0/README.md` & `wagtail-donate-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/setup.cfg` & `wagtail-donate-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtail_donate.egg-info/SOURCES.txt` & `wagtail-donate-1.9.1/wagtail_donate.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -95,14 +95,26 @@
 wagtaildonate/models/snippets.py
 wagtaildonate/models/utils.py
 wagtaildonate/payment_methods/__init__.py
 wagtaildonate/payment_methods/base.py
 wagtaildonate/payment_methods/braintree.py
 wagtaildonate/payment_methods/gocardless.py
 wagtaildonate/payment_methods/utils.py
+wagtaildonate/static/images/direct-debit.svg
+wagtaildonate/static/images/fundraising-regulator-logo.svg
+wagtaildonate/static/images/padlock.svg
+wagtaildonate/static/images/wagtail-logo.svg
+wagtaildonate/static/wagtaildonate/css/checkout.css
+wagtaildonate/static/wagtaildonate/css/donate-form.css
+wagtaildonate/static/wagtaildonate/images/direct-debit.svg
+wagtaildonate/static/wagtaildonate/images/fundraising-regulator-logo.svg
+wagtaildonate/static/wagtaildonate/images/padlock.svg
+wagtaildonate/static/wagtaildonate/images/wagtail-logo.svg
+wagtaildonate/static/wagtaildonate/js/checkout.js
+wagtaildonate/static/wagtaildonate/js/donate-form.js
 wagtaildonate/templates/wagtaildonate/base_donate.html
 wagtaildonate/templates/wagtaildonate/checkout.html
 wagtaildonate/templates/wagtaildonate/donation_campaign_page.html
 wagtaildonate/templates/wagtaildonate/donation_fundraising_pay_in_page.html
 wagtaildonate/templates/wagtaildonate/donation_page.html
 wagtaildonate/templates/wagtaildonate/thank_you.html
 wagtaildonate/templates/wagtaildonate/thank_you_fundraising.html
```

### Comparing `wagtail-donate-1.9.0/wagtaildonate/address_lookups/loqate.py` & `wagtail-donate-1.9.1/wagtaildonate/address_lookups/loqate.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/admin_forms.py` & `wagtail-donate-1.9.1/wagtaildonate/admin_forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/admin_urls.py` & `wagtail-donate-1.9.1/wagtaildonate/admin_urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/admin_views/export.py` & `wagtail-donate-1.9.1/wagtaildonate/admin_views/export.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/api/serializers/braintree.py` & `wagtail-donate-1.9.1/wagtaildonate/api/serializers/braintree.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/api/serializers/configuration.py` & `wagtail-donate-1.9.1/wagtaildonate/api/serializers/configuration.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/api/serializers/donations.py` & `wagtail-donate-1.9.1/wagtaildonate/api/serializers/donations.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/api/serializers/gocardless.py` & `wagtail-donate-1.9.1/wagtaildonate/api/serializers/gocardless.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/api/serializers/payment_method.py` & `wagtail-donate-1.9.1/wagtaildonate/api/serializers/payment_method.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/api/serializers/recaptcha.py` & `wagtail-donate-1.9.1/wagtaildonate/api/serializers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/api/serializers/utils.py` & `wagtail-donate-1.9.1/wagtaildonate/api/serializers/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/api/tests/test_serializers.py` & `wagtail-donate-1.9.1/wagtaildonate/api/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/api/tests/test_views.py` & `wagtail-donate-1.9.1/wagtaildonate/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/api/views/configuration.py` & `wagtail-donate-1.9.1/wagtaildonate/api/views/configuration.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/api/views/donations.py` & `wagtail-donate-1.9.1/wagtaildonate/api/views/donations.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/blocks.py` & `wagtail-donate-1.9.1/wagtaildonate/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/configuration.py` & `wagtail-donate-1.9.1/wagtaildonate/configuration.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/countries.py` & `wagtail-donate-1.9.1/wagtaildonate/countries.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/factories.py` & `wagtail-donate-1.9.1/wagtaildonate/factories.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/management/commands/update_transaction_status.py` & `wagtail-donate-1.9.1/wagtaildonate/management/commands/update_transaction_status.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0001_initial.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0002_add_fundraising_pay_in_fields.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0002_add_fundraising_pay_in_fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0003_donation.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0003_donation.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0004_thank_you_fields.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0004_thank_you_fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0005_add_contact_details_fields.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0005_add_contact_details_fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0007_country.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0007_country.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0008_donation_giftaid_organisation.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0008_donation_giftaid_organisation.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0009_donation_memory.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0009_donation_memory.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0012_donation_transaction_status_choices.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0012_donation_transaction_status_choices.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0013_donation_export_log.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0013_donation_export_log.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0014_donation_created_at.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0014_donation_created_at.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0015_recurringdonation.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0015_recurringdonation.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0016_thank_you_emails.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0016_thank_you_emails.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0017_donation_donation_page.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0017_donation_donation_page.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0018_phonenumber_not_mandatory.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0018_phonenumber_not_mandatory.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0019_create_at_to_use_default_timezone_now.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0019_create_at_to_use_default_timezone_now.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0020_add_export_permissions.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0020_add_export_permissions.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0021_checkout_hero.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0021_checkout_hero.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0022_thank_you_page_content.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0022_thank_you_page_content.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0023_optins.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0023_optins.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0024_donationexportlog_default_permissions.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0024_donationexportlog_default_permissions.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0025_donationexportlog_user_info.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0025_donationexportlog_user_info.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0026_thankyouemailcontent_not_mandatory.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0026_thankyouemailcontent_not_mandatory.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0027_thank_you_email_subject_not_mandatory.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0027_thank_you_email_subject_not_mandatory.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0028_payin.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0028_payin.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0030_addressline3.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0030_addressline3.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0031_remove_conrete_models.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0031_remove_conrete_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0032_payin_events.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0032_payin_events.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0033_three_d_secure_fields.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0033_three_d_secure_fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/migrations/0034_alter_thankyouctasnippet_link.py` & `wagtail-donate-1.9.1/wagtaildonate/migrations/0034_alter_thankyouctasnippet_link.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/models/__init__.py` & `wagtail-donate-1.9.1/wagtaildonate/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/models/donations.py` & `wagtail-donate-1.9.1/wagtaildonate/models/donations.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/models/export.py` & `wagtail-donate-1.9.1/wagtaildonate/models/export.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/models/pages.py` & `wagtail-donate-1.9.1/wagtaildonate/models/pages.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/models/pay_in_events.py` & `wagtail-donate-1.9.1/wagtaildonate/models/pay_in_events.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/models/snippets.py` & `wagtail-donate-1.9.1/wagtaildonate/models/snippets.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/models/utils.py` & `wagtail-donate-1.9.1/wagtaildonate/models/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/payment_methods/base.py` & `wagtail-donate-1.9.1/wagtaildonate/payment_methods/base.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/payment_methods/braintree.py` & `wagtail-donate-1.9.1/wagtaildonate/payment_methods/braintree.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/payment_methods/gocardless.py` & `wagtail-donate-1.9.1/wagtaildonate/payment_methods/gocardless.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/payment_methods/utils.py` & `wagtail-donate-1.9.1/wagtaildonate/payment_methods/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/settings.py` & `wagtail-donate-1.9.1/wagtaildonate/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/admin/export_view.html` & `wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/admin/export_view.html`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/checkout.html` & `wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/checkout.html`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/donation_campaign_page.html` & `wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/donation_campaign_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/donation_fundraising_pay_in_page.html` & `wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/donation_fundraising_pay_in_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/donation_page.html` & `wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/donation_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/includes/checkout_form.html` & `wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/includes/checkout_form.html`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/includes/forms/donate_step_one.html` & `wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/includes/forms/donate_step_one.html`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/thank_you.html` & `wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/thank_you.html`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/templates/wagtaildonate/thank_you_fundraising.html` & `wagtail-donate-1.9.1/wagtaildonate/templates/wagtaildonate/thank_you_fundraising.html`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/templatetags/wagtaildonate_tags.py` & `wagtail-donate-1.9.1/wagtaildonate/templatetags/wagtaildonate_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/utils/assets.py` & `wagtail-donate-1.9.1/wagtaildonate/utils/assets.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/utils/blocks.py` & `wagtail-donate-1.9.1/wagtaildonate/utils/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/utils/braintree.py` & `wagtail-donate-1.9.1/wagtaildonate/utils/braintree.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/utils/rich_text.py` & `wagtail-donate-1.9.1/wagtaildonate/utils/rich_text.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/views.py` & `wagtail-donate-1.9.1/wagtaildonate/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/wagtail_hooks/export.py` & `wagtail-donate-1.9.1/wagtaildonate/wagtail_hooks/export.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,43 +38,43 @@
 
 
 def register_export_donations_menu_item():
     return ExportDonationsMenuItem(
         _("Export donations"),
         reverse("wagtaildonate_admin:export"),
         order=1050,
-        classname="icon icon-download",
+        icon_name="download",
     )
 
 
 class ExportRecurringDonationsMenuItem(MenuItem):
     def is_shown(self, request):
         return request.user.has_perm("wagtaildonate.can_export_recurring_donations")
 
 
 def register_export_recurring_donations_menu_item():
     return ExportRecurringDonationsMenuItem(
         _("Export recurring donations"),
         reverse("wagtaildonate_admin:export_recurring"),
         order=1051,
-        classname="icon icon-download",
+        icon_name="download",
     )
 
 
 class ExportPayInsMenuItem(MenuItem):
     def is_shown(self, request):
         return request.user.has_perm("wagtaildonate.can_export_pay_ins")
 
 
 def register_export_pay_ins_menu_item():
     return ExportPayInsMenuItem(
         _("Export pay ins"),
         reverse("wagtaildonate_admin:export_pay_ins"),
         order=1052,
-        classname="icon icon-download",
+        icon_name="download",
     )
 
 
 def register_export_wagtail_hooks():
     if donate_settings.DONATION_EXPORT_ENABLED:
         hooks.register("register_permissions", register_export_permissions)
         hooks.register(
```

### Comparing `wagtail-donate-1.9.0/wagtaildonate/wagtail_hooks/export_log.py` & `wagtail-donate-1.9.1/wagtaildonate/wagtail_hooks/export_log.py`

 * *Files identical despite different names*

### Comparing `wagtail-donate-1.9.0/wagtaildonate/wagtail_hooks/general.py` & `wagtail-donate-1.9.1/wagtaildonate/wagtail_hooks/general.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         return any(request.user.has_perm(perm) for perm in payment_perms)
 
 
 def register_payments_menu():
     return PaymentsMenu(
         _("Payments"),
         Menu(register_hook_name="register_payments_menu_item"),
-        classname="icon icon-cogs",
+        icon_name="cogs",
     )
 
 
 def register_general_wagtail_hooks():
     if donate_settings.DONATION_EXPORT_ENABLED:
         hooks.register("register_admin_urls", register_admin_urls)
         hooks.register("register_admin_menu_item", register_payments_menu)
```

### Comparing `wagtail-donate-1.9.0/wagtaildonate/wagtail_hooks/pay_in_events.py` & `wagtail-donate-1.9.1/wagtaildonate/wagtail_hooks/pay_in_events.py`

 * *Files identical despite different names*

