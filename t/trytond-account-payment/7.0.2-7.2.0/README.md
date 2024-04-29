# Comparing `tmp/trytond_account_payment-7.0.2.tar.gz` & `tmp/trytond_account_payment-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment-7.0.2.tar", last modified: Thu Feb 15 18:38:21 2024, max compression
+gzip compressed data, was "trytond_account_payment-7.2.0.tar", last modified: Mon Apr 29 15:34:33 2024, max compression
```

## Comparing `trytond_account_payment-7.0.2.tar` & `trytond_account_payment-7.2.0.tar`

### file list

```diff
@@ -1,93 +1,92 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:38:21.941282 trytond_account_payment-7.0.2/
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     3977 2024-02-15 18:38:19.000000 trytond_account_payment-7.0.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-02-15 18:38:18.000000 trytond_account_payment-7.0.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3124 2024-02-15 18:38:21.941282 trytond_account_payment-7.0.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1421 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27888 2024-02-10 10:20:28.000000 trytond_account_payment-7.0.2/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7877 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:38:21.934615 trytond_account_payment-7.0.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2816 2024-02-05 16:24:27.000000 trytond_account_payment-7.0.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3888 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:38:21.934615 trytond_account_payment-7.0.2/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/icons/tryton-payment.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:38:21.937948 trytond_account_payment-7.0.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    19645 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20283 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18078 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20834 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20160 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17490 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19288 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20582 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18065 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20610 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18536 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18312 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18642 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    21580 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19246 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20382 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18381 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19170 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17121 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19646 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19231 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18065 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16686 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18288 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2212 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5703 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2548 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    24371 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27478 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-02-15 18:38:21.941282 trytond_account_payment-7.0.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4844 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:38:21.937948 trytond_account_payment-7.0.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5501 2024-02-05 16:24:27.000000 trytond_account_payment-7.0.2/tests/scenario_account_payment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2598 2024-02-05 16:24:27.000000 trytond_account_payment-7.0.2/tests/scenario_account_payment_blocked_direct_debit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3132 2024-02-05 16:24:27.000000 trytond_account_payment-7.0.2/tests/scenario_account_payment_direct_debit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3536 2024-02-05 16:24:27.000000 trytond_account_payment-7.0.2/tests/scenario_account_payment_dunning.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4065 2024-02-05 16:24:27.000000 trytond_account_payment-7.0.2/tests/scenario_account_payment_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2564 2024-02-05 16:24:27.000000 trytond_account_payment-7.0.2/tests/scenario_account_payment_planning.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2714 2024-02-05 16:24:27.000000 trytond_account_payment-7.0.2/tests/scenario_account_payment_statement.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4409 2024-02-05 16:24:27.000000 trytond_account_payment-7.0.2/tests/scenario_account_payment_warnings.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-02-05 16:24:27.000000 trytond_account_payment-7.0.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:38:21.941282 trytond_account_payment-7.0.2/trytond_account_payment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3124 2024-02-15 18:38:21.000000 trytond_account_payment-7.0.2/trytond_account_payment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3420 2024-02-15 18:38:21.000000 trytond_account_payment-7.0.2/trytond_account_payment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-02-15 18:38:21.000000 trytond_account_payment-7.0.2/trytond_account_payment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-02-15 18:38:21.000000 trytond_account_payment-7.0.2/trytond_account_payment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:35.000000 trytond_account_payment-7.0.2/trytond_account_payment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-02-15 18:38:21.000000 trytond_account_payment-7.0.2/trytond_account_payment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-02-15 18:38:21.000000 trytond_account_payment-7.0.2/trytond_account_payment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:38:21.941282 trytond_account_payment-7.0.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/move_line_create_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      841 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/move_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/move_line_list_to_pay.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/move_line_pay_ask_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/move_line_pay_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      488 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/party_reception_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/party_reception_direct_debit_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1833 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1029 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/payment_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/payment_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/payment_journal_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-10-30 17:06:38.000000 trytond_account_payment-7.0.2/view/payment_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:33.845312 trytond_account_payment-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3876 2024-04-29 15:15:03.000000 trytond_account_payment-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:15:03.000000 trytond_account_payment-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3115 2024-04-29 15:34:33.845312 trytond_account_payment-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1421 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27997 2024-04-27 16:30:39.000000 trytond_account_payment-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7785 2024-04-27 16:30:39.000000 trytond_account_payment-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:33.838645 trytond_account_payment-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_account_payment-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3888 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:56.000000 trytond_account_payment-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:33.838645 trytond_account_payment-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/icons/tryton-payment.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:33.838645 trytond_account_payment-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19645 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20283 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18078 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20834 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20160 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17490 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19288 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20582 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18065 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20610 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18536 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18312 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18642 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    21580 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19246 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20382 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18381 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19170 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19873 2024-04-29 13:17:17.000000 trytond_account_payment-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19646 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19231 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18065 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16686 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18288 2024-04-27 16:43:21.000000 trytond_account_payment-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2212 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5703 2024-03-08 19:04:12.000000 trytond_account_payment-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2479 2024-04-27 16:30:39.000000 trytond_account_payment-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    24371 2024-02-13 17:30:52.000000 trytond_account_payment-7.2.0/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26995 2024-04-27 16:30:39.000000 trytond_account_payment-7.2.0/payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:34:33.845312 trytond_account_payment-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4835 2024-04-27 16:30:39.000000 trytond_account_payment-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:33.841978 trytond_account_payment-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5477 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2583 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment_blocked_direct_debit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3138 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment_direct_debit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3528 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment_dunning.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4030 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2569 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment_planning.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2714 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment_statement.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4209 2024-04-22 12:14:36.000000 trytond_account_payment-7.2.0/tests/scenario_account_payment_warnings.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:56.000000 trytond_account_payment-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-29 15:14:58.000000 trytond_account_payment-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:33.841978 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3115 2024-04-29 15:34:33.000000 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3402 2024-04-29 15:34:33.000000 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:34:33.000000 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:34:33.000000 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-29 15:34:33.000000 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:34:33.000000 trytond_account_payment-7.2.0/trytond_account_payment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:33.841978 trytond_account_payment-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-01-16 14:00:20.000000 trytond_account_payment-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-01-16 14:00:20.000000 trytond_account_payment-7.2.0/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/view/move_line_create_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2024-01-27 09:58:52.000000 trytond_account_payment-7.2.0/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      841 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/view/move_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-01-27 09:58:52.000000 trytond_account_payment-7.2.0/view/move_line_list_to_pay.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/view/move_line_pay_ask_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/view/move_line_pay_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      488 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-03-08 19:04:12.000000 trytond_account_payment-7.2.0/view/party_reception_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2024-03-08 19:04:12.000000 trytond_account_payment-7.2.0/view/party_reception_direct_debit_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1833 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1029 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/view/payment_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/view/payment_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_account_payment-7.2.0/view/payment_journal_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-02-04 18:51:26.000000 trytond_account_payment-7.2.0/view/payment_list.xml
```

### Comparing `trytond_account_payment-7.0.2/CHANGELOG` & `trytond_account_payment-7.2.0/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 
-Version 7.0.2 - 2024-02-15
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2023-11-17
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_payment-7.0.2/COPYRIGHT` & `trytond_account_payment-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/LICENSE` & `trytond_account_payment-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/PKG-INFO` & `trytond_account_payment-7.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment
-Version: 7.0.2
+Version: 7.2.0
 Summary: Tryton module for payment
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-payment
+Project-URL: Documentation, https://docs.tryton.org/modules-account-payment
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,24 +49,24 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_dunning<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_statement<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_dunning<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_statement<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
 
 ######################
 Account Payment Module
 ######################
 
 The *Account Payment Module* manages the receivable and payable payments.
 A payment is an order to pay an amount to a party or to receive an amount from
```

### Comparing `trytond_account_payment-7.0.2/__init__.py` & `trytond_account_payment-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/account.py` & `trytond_account_payment-7.2.0/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -699,15 +699,17 @@
         super().__setup__()
         cls.related_to.domain['account.payment'] = [
             ('company', '=', Eval('company', -1)),
             If(Bool(Eval('party')),
                 ('party', '=', Eval('party')),
                 ()),
             ('state', 'in', ['processing', 'succeeded', 'failed']),
-            ('currency', '=', Eval('currency', -1)),
+            If(Eval('second_currency'),
+                ('currency', '=', Eval('second_currency', -1)),
+                ('currency', '=', Eval('currency', -1))),
             ('kind', '=',
                 If(Eval('amount', 0) > 0, 'receivable',
                     If(Eval('amount', 0) < 0, 'payable', ''))),
             ]
         cls.related_to.search_order['account.payment'] = [
             ('amount', 'ASC'),
             ('state', 'ASC'),
```

### Comparing `trytond_account_payment-7.0.2/account.xml` & `trytond_account_payment-7.2.0/account.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_account_payment-7.0.2/account.xml` & `trytond_account_payment-7.2.0/account.xml`

```diff
@@ -42,15 +42,15 @@
       <field name="sequence" eval="20"/>
       <field name="domain" eval="['OR', ('debit', '&gt;', 0), ('credit', '&lt;', 0)]" pyson="1"/>
       <field name="count" eval="True"/>
       <field name="act_window" ref="act_move_line_form"/>
     </record>
     <menuitem parent="menu_payments" action="act_move_line_form" sequence="10" id="menu_move_line_form"/>
     <record model="ir.model.access" id="access_move_line_payment">
-      <field name="model" search="[('model', '=', 'account.move.line')]"/>
+      <field name="model">account.move.line</field>
       <field name="group" ref="group_payment"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.action.wizard" id="wizard_create_direct_debit">
@@ -83,35 +83,35 @@
       <field name="model">account.move.line</field>
     </record>
     <record model="ir.action-res.group" id="act_pay_line-group_payment">
       <field name="action" ref="act_pay_line"/>
       <field name="group" ref="group_payment"/>
     </record>
     <record model="ir.model.button" id="move_line_pay_button">
+      <field name="model">account.move.line</field>
       <field name="name">pay</field>
       <field name="string">Pay</field>
-      <field name="model" search="[('model', '=', 'account.move.line')]"/>
     </record>
     <record model="ir.model.button-res.group" id="move_line_pay_button_group_payment">
       <field name="button" ref="move_line_pay_button"/>
       <field name="group" ref="group_payment"/>
     </record>
     <record model="ir.model.button" id="move_line_payment_block_button">
+      <field name="model">account.move.line</field>
       <field name="name">payment_block</field>
       <field name="string">Block</field>
-      <field name="model" search="[('model', '=', 'account.move.line')]"/>
     </record>
     <record model="ir.model.button-res.group" id="move_line_payment_block_button_group_payment">
       <field name="button" ref="move_line_payment_block_button"/>
       <field name="group" ref="group_payment"/>
     </record>
     <record model="ir.model.button" id="move_line_payment_unblock_button">
+      <field name="model">account.move.line</field>
       <field name="name">payment_unblock</field>
       <field name="string">Unblock</field>
-      <field name="model" search="[('model', '=', 'account.move.line')]"/>
     </record>
     <record model="ir.model.button-res.group" id="move_line_payment_unblock_button_group_payment">
       <field name="button" ref="move_line_payment_unblock_button"/>
       <field name="group" ref="group_payment"/>
     </record>
     <record model="ir.ui.view" id="configuration_view_form">
       <field name="model">account.configuration</field>
```

### Comparing `trytond_account_payment-7.0.2/doc/conf.py` & `trytond_account_payment-7.2.0/doc/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 base_url = os.environ.get('DOC_BASE_URL')
 if base_url:
     modules_url = base_url + '/modules-{module}/'
     trytond_url = base_url + '/server/'
 else:
     modules_url = (
-        'https://docs.tryton.org/projects/modules-{module}/en/{series}/')
-    trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
+        'https://docs.tryton.org/${series}/modules-{module}/')
+    trytond_url = 'https://docs.tryton.org/${series}/server/'
 
 
 def get_info():
     import configparser
     import subprocess
     import sys
 
@@ -67,22 +67,33 @@
     }
 html_title = info['description']
 master_doc = 'index'
 project = info['name']
 release = version = info['series']
 default_role = 'ref'
 highlight_language = 'none'
+exclude_patterns = ['**/*.inc.rst']
 extensions = [
     'sphinx_copybutton',
     'sphinx.ext.intersphinx',
     ]
 intersphinx_mapping = {
     'trytond': (trytond_url.format(series=version), None),
     }
 intersphinx_mapping.update({
         m: (modules_url.format(
                 module=m.replace('_', '-'), series=version), None)
         for m in info['modules']
         })
 linkcheck_ignore = [r'/.*', r'https://demo.tryton.org/*']
 
+try:
+    with open(os.path.join(
+                os.path.dirname(__file__),
+                'linkcheck_ignore.json'), 'r') as f:
+        import json
+        linkcheck_ignore.extend(json.load(f))
+        del json
+except FileNotFoundError:
+    pass
+
 del get_info, info, base_url, modules_url, trytond_url
```

### Comparing `trytond_account_payment-7.0.2/doc/design.rst` & `trytond_account_payment-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/exceptions.py` & `trytond_account_payment-7.2.0/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/icons/LICENSE` & `trytond_account_payment-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/bg.po` & `trytond_account_payment-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/ca.po` & `trytond_account_payment-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/cs.po` & `trytond_account_payment-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/de.po` & `trytond_account_payment-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/es.po` & `trytond_account_payment-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/es_419.po` & `trytond_account_payment-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/et.po` & `trytond_account_payment-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/fa.po` & `trytond_account_payment-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/fi.po` & `trytond_account_payment-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/fr.po` & `trytond_account_payment-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/hu.po` & `trytond_account_payment-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/id.po` & `trytond_account_payment-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/it.po` & `trytond_account_payment-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/lo.po` & `trytond_account_payment-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/lt.po` & `trytond_account_payment-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/nl.po` & `trytond_account_payment-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/pl.po` & `trytond_account_payment-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/pt.po` & `trytond_account_payment-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/ro.po` & `trytond_account_payment-7.2.0/locale/tr.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,198 +4,205 @@
 
 msgctxt "field:account.configuration,payment_group_sequence:"
 msgid "Payment Group Sequence"
 msgstr ""
 
 msgctxt "field:account.configuration.payment_group_sequence,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt ""
 "field:account.configuration.payment_group_sequence,payment_group_sequence:"
 msgid "Payment Group Sequence"
 msgstr ""
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
 msgid "Amount to Pay"
-msgstr "Suma"
+msgstr "Lines to Pay"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
 msgid "Payment Currency"
-msgstr "Plată"
+msgstr "Payment Journals"
 
 msgctxt "field:account.move.line,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
 msgctxt "field:account.move.line,payment_kind:"
 msgid "Payment Kind"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.move.line,payments:"
 msgid "Payments"
-msgstr ""
+msgstr "Payments"
 
-#, fuzzy
 msgctxt "field:account.move.line.create_direct_debit.start,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:account.move.line.pay.ask_journal,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:account.move.line.pay.ask_journal,currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr ""
 
 msgctxt "field:account.move.line.pay.ask_journal,journal:"
 msgid "Journal"
-msgstr "Jurnal"
+msgstr ""
 
 msgctxt "field:account.move.line.pay.ask_journal,journals:"
 msgid "Journals"
 msgstr ""
 
 msgctxt "field:account.move.line.pay.start,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:account.payment,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.payment,approved_by:"
 msgid "Approved by"
-msgstr ""
+msgstr "Approved"
 
 msgctxt "field:account.payment,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:account.payment,currency:"
 msgid "Currency"
-msgstr "Valuta"
+msgstr ""
 
 msgctxt "field:account.payment,date:"
 msgid "Date"
-msgstr "Data"
+msgstr ""
 
 msgctxt "field:account.payment,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:account.payment,failed_by:"
 msgid "Failure Noted by"
 msgstr ""
 
 msgctxt "field:account.payment,group:"
 msgid "Group"
-msgstr "Grup"
+msgstr ""
 
 msgctxt "field:account.payment,journal:"
 msgid "Journal"
-msgstr "Jurnal"
+msgstr ""
 
 msgctxt "field:account.payment,kind:"
 msgid "Kind"
 msgstr ""
 
 msgctxt "field:account.payment,line:"
 msgid "Line"
 msgstr ""
 
 msgctxt "field:account.payment,origin:"
 msgid "Origin"
-msgstr "Origine"
+msgstr ""
 
 msgctxt "field:account.payment,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:account.payment,process_method:"
 msgid "Process Method"
-msgstr ""
+msgstr "Process Payments"
 
 msgctxt "field:account.payment,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:account.payment,submitted_by:"
 msgid "Submitted by"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.payment,succeeded_by:"
 msgid "Success Noted by"
-msgstr ""
+msgstr "Succeed"
 
 msgctxt "field:account.payment.group,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:account.payment.group,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Payment Journals"
 
 msgctxt "field:account.payment.group,journal:"
 msgid "Journal"
-msgstr "Jurnal"
+msgstr ""
 
 msgctxt "field:account.payment.group,kind:"
 msgid "Kind"
 msgstr ""
 
 msgctxt "field:account.payment.group,number:"
 msgid "Number"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.payment.group,payment_amount:"
 msgid "Payment Total Amount"
-msgstr ""
+msgstr "Payment Journals"
 
+#, fuzzy
 msgctxt "field:account.payment.group,payment_amount_succeeded:"
 msgid "Payment Succeeded"
-msgstr ""
+msgstr "Succeeded"
 
 #, fuzzy
 msgctxt "field:account.payment.group,payment_complete:"
 msgid "Payment Complete"
-msgstr "Plată"
+msgstr "Payment Groups"
 
 #, fuzzy
 msgctxt "field:account.payment.group,payment_count:"
 msgid "Payment Count"
-msgstr "Plată"
+msgstr "Payment Journals"
 
+#, fuzzy
 msgctxt "field:account.payment.group,payments:"
 msgid "Payments"
-msgstr ""
+msgstr "Payments"
 
+#, fuzzy
 msgctxt "field:account.payment.group,process_method:"
 msgid "Process Method"
-msgstr ""
+msgstr "Process Payments"
 
 msgctxt "field:account.payment.journal,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:account.payment.journal,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr ""
 
 msgctxt "field:account.payment.journal,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:account.payment.journal,process_method:"
 msgid "Process Method"
@@ -215,47 +222,46 @@
 
 msgctxt "field:party.party,reception_direct_debits:"
 msgid "Direct Debits"
 msgstr ""
 
 msgctxt "field:party.party.payment_direct_debit,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:party.party.payment_direct_debit,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:party.party.payment_direct_debit,payment_direct_debit:"
 msgid "Direct Debit"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:party.party.reception_direct_debit,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:party.party.reception_direct_debit,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Payment Journals"
 
 #, fuzzy
 msgctxt "field:party.party.reception_direct_debit,journal:"
 msgid "Journal"
-msgstr "Jurnal"
+msgstr "Payment Journals"
 
-#, fuzzy
 msgctxt "field:party.party.reception_direct_debit,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:party.party.reception_direct_debit,process_method:"
 msgid "Process Method"
-msgstr ""
+msgstr "Process Payments"
 
 msgctxt "help:account.invoice,payment_direct_debit:"
 msgid "Check if the invoice is paid by direct debit."
 msgstr ""
 
 msgctxt "help:account.move.line,payment_direct_debit:"
 msgid "Check if the line will be paid by direct debit."
@@ -303,165 +309,185 @@
 msgid "Account Configuration Payment Group Sequence"
 msgstr ""
 
 msgctxt "model:account.move.line.create_direct_debit.start,name:"
 msgid "Create Direct Debit"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:account.move.line.pay.ask_journal,name:"
 msgid "Pay Line"
-msgstr ""
+msgstr "Pay Lines"
 
+#, fuzzy
 msgctxt "model:account.move.line.pay.start,name:"
 msgid "Pay Line"
-msgstr ""
+msgstr "Pay Lines"
 
+#, fuzzy
 msgctxt "model:account.payment,name:"
 msgid "Payment"
-msgstr "Plată"
+msgstr "Payment"
 
+#, fuzzy
 msgctxt "model:account.payment.group,name:"
 msgid "Payment Group"
-msgstr ""
+msgstr "Payment Groups"
 
+#, fuzzy
 msgctxt "model:account.payment.journal,name:"
 msgid "Payment Journal"
-msgstr ""
+msgstr "Payment Journals"
 
 msgctxt "model:ir.action,name:act_move_line_form"
 msgid "Lines to Pay"
-msgstr ""
+msgstr "Lines to Pay"
 
 msgctxt "model:ir.action,name:act_pay_line"
 msgid "Pay Lines"
-msgstr ""
+msgstr "Pay Lines"
 
 msgctxt "model:ir.action,name:act_payment_form"
 msgid "Payments"
-msgstr ""
+msgstr "Payments"
 
 msgctxt "model:ir.action,name:act_payment_form_group_open"
 msgid "Payments"
-msgstr ""
+msgstr "Payments"
 
 msgctxt "model:ir.action,name:act_payment_form_line_relate"
 msgid "Payments"
-msgstr ""
+msgstr "Payments"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_payment_form_payable"
 msgid "Payable Payments"
-msgstr "Plată"
+msgstr "Process Payments"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_payment_form_receivable"
 msgid "Receivable Payments"
-msgstr ""
+msgstr "Receivable"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_payment_form_relate_party"
 msgid "Payments"
-msgstr "Plată"
+msgstr "Payments"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_payment_group_form"
 msgid "Payment Groups"
-msgstr "Plată"
+msgstr "Payment Groups"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_payment_journal_form"
 msgid "Payment Journals"
-msgstr "Plată"
+msgstr "Payment Journals"
 
 msgctxt "model:ir.action,name:act_process_payments"
 msgid "Process Payments"
-msgstr ""
+msgstr "Process Payments"
 
 msgctxt "model:ir.action,name:wizard_create_direct_debit"
 msgid "Create Direct Debit"
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_move_line_form_domain_payable"
 msgid "Payable"
-msgstr ""
+msgstr "Payable"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_move_line_form_domain_receivable"
 msgid "Receivable"
-msgstr ""
+msgstr "Receivable"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_group_open_domain_all"
 msgid "All"
-msgstr ""
+msgstr "All"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_group_open_domain_failed"
 msgid "Failed"
-msgstr ""
+msgstr "Failed"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_group_open_domain_processing"
 msgid "Processing"
-msgstr ""
+msgstr "Processing"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_group_open_domain_succeeded"
 msgid "Succeeded"
-msgstr ""
+msgstr "Succeeded"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_payable_domain_all"
 msgid "All"
-msgstr ""
+msgstr "All"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_payable_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_payable_domain_processing"
 msgid "Processing"
-msgstr ""
+msgstr "Processing"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_payable_domain_to_approve"
 msgid "To Approve"
-msgstr ""
+msgstr "Approve"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_payable_domain_to_process"
 msgid "To Process"
-msgstr ""
+msgstr "Processing"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_receivable_domain_all"
 msgid "All"
-msgstr ""
+msgstr "All"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_receivable_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_receivable_domain_processing"
 msgid "Processing"
-msgstr ""
+msgstr "Processing"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_receivable_domain_to_process"
 msgid "To Process"
-msgstr ""
+msgstr "Processing"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
 msgid "All"
-msgstr ""
+msgstr "All"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
@@ -516,58 +542,60 @@
 msgid "The line \"%(line)s\" of payment \"%(payment)s\" is already reconciled."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:payment_process_wizard_button"
 msgid "Are you sure you want to process the payments?"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:move_line_pay_button"
 msgid "Pay"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:move_line_payment_block_button"
 msgid "Block"
-msgstr ""
+msgstr "Block"
 
 msgctxt "model:ir.model.button,string:move_line_payment_unblock_button"
 msgid "Unblock"
-msgstr ""
+msgstr "Unblock"
 
 msgctxt "model:ir.model.button,string:payment_approve_button"
 msgid "Approve"
-msgstr ""
+msgstr "Approve"
 
 msgctxt "model:ir.model.button,string:payment_draft_button"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:payment_fail_button"
 msgid "Fail"
-msgstr ""
+msgstr "Fail"
 
+#, fuzzy
 msgctxt "model:ir.model.button,string:payment_group_succeed_button"
 msgid "Succeed"
-msgstr ""
+msgstr "Succeed"
 
+#, fuzzy
 msgctxt "model:ir.model.button,string:payment_proceed_button"
 msgid "Processing"
-msgstr ""
+msgstr "Processing"
 
+#, fuzzy
 msgctxt "model:ir.model.button,string:payment_process_wizard_button"
 msgid "Process"
-msgstr ""
+msgstr "Processing"
 
 msgctxt "model:ir.model.button,string:payment_submit_button"
 msgid "Submit"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:payment_succeed_button"
 msgid "Succeed"
-msgstr ""
+msgstr "Succeed"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_party_reception_direct_debit_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_payment_companies"
@@ -580,130 +608,143 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_payment_journal_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.sequence,name:sequence_account_payment_group"
 msgid "Default Account Payment Group"
-msgstr ""
+msgstr "Default Account Payment Group"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_account_payment_group"
 msgid "Account Payment Group"
-msgstr ""
+msgstr "Account Payment Group"
 
 msgctxt "model:ir.ui.menu,name:menu_create_direct_debit"
 msgid "Create Direct Debit"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_move_line_form"
 msgid "Lines to Pay"
-msgstr ""
+msgstr "Lines to Pay"
 
 msgctxt "model:ir.ui.menu,name:menu_payment_configuration"
 msgid "Payments"
-msgstr ""
+msgstr "Payments"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_payment_form_payable"
 msgid "Payable Payments"
-msgstr "Plată"
+msgstr "Process Payments"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_payment_form_receivable"
 msgid "Receivable Payments"
-msgstr ""
+msgstr "Receivable"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_payment_group_form"
 msgid "Payment Groups"
-msgstr "Plată"
+msgstr "Payment Groups"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_payment_journal_form"
 msgid "Payment Journals"
-msgstr "Plată"
+msgstr "Payment Journals"
 
 msgctxt "model:ir.ui.menu,name:menu_payments"
 msgid "Payments"
-msgstr ""
+msgstr "Payments"
 
 msgctxt "model:party.party.payment_direct_debit,name:"
 msgid "Party Payment Direct Debit"
 msgstr ""
 
 msgctxt "model:party.party.reception_direct_debit,name:"
 msgid "Party Reception Direct Debit"
 msgstr ""
 
 msgctxt "model:res.group,name:group_payment"
 msgid "Payment"
-msgstr "Plată"
+msgstr "Payment"
 
 msgctxt "model:res.group,name:group_payment_approval"
 msgid "Payment Approval"
-msgstr ""
+msgstr "Payment Approval"
 
+#, fuzzy
 msgctxt "selection:account.move.line,payment_kind:"
 msgid "Payable"
-msgstr ""
+msgstr "Payable"
 
+#, fuzzy
 msgctxt "selection:account.move.line,payment_kind:"
 msgid "Receivable"
-msgstr ""
+msgstr "Receivable"
 
+#, fuzzy
 msgctxt "selection:account.payment,kind:"
 msgid "Payable"
-msgstr ""
+msgstr "Payable"
 
+#, fuzzy
 msgctxt "selection:account.payment,kind:"
 msgid "Receivable"
-msgstr ""
+msgstr "Receivable"
 
+#, fuzzy
 msgctxt "selection:account.payment,state:"
 msgid "Approved"
-msgstr ""
+msgstr "Approve"
 
+#, fuzzy
 msgctxt "selection:account.payment,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
+#, fuzzy
 msgctxt "selection:account.payment,state:"
 msgid "Failed"
-msgstr ""
+msgstr "Failed"
 
+#, fuzzy
 msgctxt "selection:account.payment,state:"
 msgid "Processing"
-msgstr ""
+msgstr "Processing"
 
 msgctxt "selection:account.payment,state:"
 msgid "Submitted"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:account.payment,state:"
 msgid "Succeeded"
-msgstr ""
+msgstr "Succeed"
 
+#, fuzzy
 msgctxt "selection:account.payment.group,kind:"
 msgid "Payable"
-msgstr ""
+msgstr "Payable"
 
+#, fuzzy
 msgctxt "selection:account.payment.group,kind:"
 msgid "Receivable"
-msgstr ""
+msgstr "Receivable"
 
 msgctxt "selection:account.payment.journal,process_method:"
 msgid "Manual"
 msgstr ""
 
 msgctxt "view:account.configuration:"
 msgid "Group Sequence"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Payment"
-msgstr "Plată"
+msgstr "Payment"
 
 msgctxt "view:account.move.line.create_direct_debit.start:"
 msgid "Create Direct Debit for date"
 msgstr ""
 
 msgctxt "view:account.payment.group:"
 msgid "Complete"
@@ -712,27 +753,28 @@
 msgctxt "view:account.payment.group:"
 msgid "Count"
 msgstr ""
 
 #, fuzzy
 msgctxt "view:account.payment.group:"
 msgid "Payments Info"
-msgstr "Plată"
+msgstr "Payments"
 
+#, fuzzy
 msgctxt "view:account.payment.group:"
 msgid "Succeeded"
-msgstr ""
+msgstr "Succeeded"
 
 msgctxt "view:account.payment.group:"
 msgid "Total Amount"
 msgstr ""
 
 msgctxt "view:account.payment:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "view:account.payment:"
 msgid "Other Info"
 msgstr ""
 
 msgctxt "wizard_button:account.move.line.create_direct_debit,start,create_:"
 msgid "Create"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_account_payment-7.0.2/locale/ru.po` & `trytond_account_payment-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/sl.po` & `trytond_account_payment-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/tr.po` & `trytond_account_payment-7.2.0/locale/zh_CN.po`

 * *Files 4% similar despite different names*

```diff
@@ -42,17 +42,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.move.line,payments:"
 msgid "Payments"
 msgstr "Payments"
 
+#, fuzzy
 msgctxt "field:account.move.line.create_direct_debit.start,date:"
 msgid "Date"
-msgstr ""
+msgstr "日期格式"
 
 msgctxt "field:account.move.line.pay.ask_journal,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.move.line.pay.ask_journal,currency:"
 msgid "Currency"
@@ -62,17 +63,18 @@
 msgid "Journal"
 msgstr ""
 
 msgctxt "field:account.move.line.pay.ask_journal,journals:"
 msgid "Journals"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.move.line.pay.start,date:"
 msgid "Date"
-msgstr ""
+msgstr "日期格式"
 
 msgctxt "field:account.payment,amount:"
 msgid "Amount"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.payment,approved_by:"
@@ -83,29 +85,33 @@
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.payment,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.payment,date:"
 msgid "Date"
-msgstr ""
+msgstr "日期格式"
 
+#, fuzzy
 msgctxt "field:account.payment,description:"
 msgid "Description"
-msgstr ""
+msgstr "描述"
 
+#, fuzzy
 msgctxt "field:account.payment,failed_by:"
 msgid "Failure Noted by"
-msgstr ""
+msgstr "添加用户"
 
+#, fuzzy
 msgctxt "field:account.payment,group:"
 msgid "Group"
-msgstr ""
+msgstr "用户组"
 
 msgctxt "field:account.payment,journal:"
 msgid "Journal"
 msgstr ""
 
 msgctxt "field:account.payment,kind:"
 msgid "Kind"
@@ -124,17 +130,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.payment,process_method:"
 msgid "Process Method"
 msgstr "Process Payments"
 
+#, fuzzy
 msgctxt "field:account.payment,state:"
 msgid "State"
-msgstr ""
+msgstr "状态"
 
 msgctxt "field:account.payment,submitted_by:"
 msgid "Submitted by"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:account.payment,succeeded_by:"
@@ -196,17 +203,18 @@
 msgid "Company"
 msgstr ""
 
 msgctxt "field:account.payment.journal,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.payment.journal,name:"
 msgid "Name"
-msgstr ""
+msgstr "纳木"
 
 msgctxt "field:account.payment.journal,process_method:"
 msgid "Process Method"
 msgstr ""
 
 msgctxt "field:party.party,payment_direct_debit:"
 msgid "Direct Debit"
@@ -369,15 +377,14 @@
 msgstr "Receivable"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_payment_form_relate_party"
 msgid "Payments"
 msgstr "Payments"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_payment_group_form"
 msgid "Payment Groups"
 msgstr "Payment Groups"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_payment_journal_form"
 msgid "Payment Journals"
@@ -401,15 +408,15 @@
 msgid "Receivable"
 msgstr "Receivable"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_group_open_domain_all"
 msgid "All"
-msgstr "All"
+msgstr "全部"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_group_open_domain_failed"
 msgid "Failed"
 msgstr "Failed"
 
@@ -425,15 +432,15 @@
 msgid "Succeeded"
 msgstr "Succeeded"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_payable_domain_all"
 msgid "All"
-msgstr "All"
+msgstr "全部"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_payable_domain_draft"
 msgid "Draft"
 msgstr "Draft"
 
@@ -455,15 +462,15 @@
 msgid "To Process"
 msgstr "Processing"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_receivable_domain_all"
 msgid "All"
-msgstr "All"
+msgstr "全部"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_receivable_domain_draft"
 msgid "Draft"
 msgstr "Draft"
 
@@ -479,15 +486,15 @@
 msgid "To Process"
 msgstr "Processing"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
 msgid "All"
-msgstr "All"
+msgstr "全部"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
@@ -636,15 +643,14 @@
 msgstr "Process Payments"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_payment_form_receivable"
 msgid "Receivable Payments"
 msgstr "Receivable"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_payment_group_form"
 msgid "Payment Groups"
 msgstr "Payment Groups"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_payment_journal_form"
 msgid "Payment Journals"
@@ -764,38 +770,43 @@
 msgid "Succeeded"
 msgstr "Succeeded"
 
 msgctxt "view:account.payment.group:"
 msgid "Total Amount"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:account.payment:"
 msgid "Description"
-msgstr ""
+msgstr "描述"
 
 msgctxt "view:account.payment:"
 msgid "Other Info"
 msgstr ""
 
+#, fuzzy
 msgctxt "wizard_button:account.move.line.create_direct_debit,start,create_:"
 msgid "Create"
-msgstr ""
+msgstr "创建日期:"
 
+#, fuzzy
 msgctxt "wizard_button:account.move.line.create_direct_debit,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "取消"
 
+#, fuzzy
 msgctxt "wizard_button:account.move.line.pay,ask_journal,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "取消"
 
 msgctxt "wizard_button:account.move.line.pay,ask_journal,next_:"
 msgid "Pay"
 msgstr ""
 
+#, fuzzy
 msgctxt "wizard_button:account.move.line.pay,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "取消"
 
 msgctxt "wizard_button:account.move.line.pay,start,next_:"
 msgid "Pay"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_account_payment-7.0.2/locale/uk.po` & `trytond_account_payment-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/locale/zh_CN.po` & `trytond_account_payment-7.2.0/locale/ro.po`

 * *Files 19% similar despite different names*

```diff
@@ -1,812 +1,757 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.configuration,payment_group_sequence:"
 msgid "Payment Group Sequence"
-msgstr ""
+msgstr "Secventa Grupului de Plati"
 
 msgctxt "field:account.configuration.payment_group_sequence,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt ""
 "field:account.configuration.payment_group_sequence,payment_group_sequence:"
 msgid "Payment Group Sequence"
-msgstr ""
+msgstr "Secventa Grupului de Plati"
 
 msgctxt "field:account.invoice,payment_direct_debit:"
 msgid "Direct Debit"
-msgstr ""
+msgstr "Debit Direct"
 
-#, fuzzy
 msgctxt "field:account.move.line,payment_amount:"
 msgid "Amount to Pay"
-msgstr "Lines to Pay"
+msgstr "Suma de Plata"
 
 msgctxt "field:account.move.line,payment_blocked:"
 msgid "Blocked"
-msgstr ""
+msgstr "Blocat"
 
-#, fuzzy
 msgctxt "field:account.move.line,payment_currency:"
 msgid "Payment Currency"
-msgstr "Payment Journals"
+msgstr "Moneda de Plată"
 
 msgctxt "field:account.move.line,payment_direct_debit:"
 msgid "Direct Debit"
-msgstr ""
+msgstr "Debit Direct"
 
 msgctxt "field:account.move.line,payment_kind:"
 msgid "Payment Kind"
-msgstr ""
+msgstr "Fel de Plata"
 
-#, fuzzy
 msgctxt "field:account.move.line,payments:"
 msgid "Payments"
-msgstr "Payments"
+msgstr "Plati"
 
-#, fuzzy
 msgctxt "field:account.move.line.create_direct_debit.start,date:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Data"
 
 msgctxt "field:account.move.line.pay.ask_journal,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:account.move.line.pay.ask_journal,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Valută"
 
 msgctxt "field:account.move.line.pay.ask_journal,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Jurnal"
 
 msgctxt "field:account.move.line.pay.ask_journal,journals:"
 msgid "Journals"
-msgstr ""
+msgstr "Jurnale"
 
-#, fuzzy
 msgctxt "field:account.move.line.pay.start,date:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Data"
 
 msgctxt "field:account.payment,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
-#, fuzzy
 msgctxt "field:account.payment,approved_by:"
 msgid "Approved by"
-msgstr "Approved"
+msgstr "Aprobat de"
 
 msgctxt "field:account.payment,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:account.payment,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Valuta"
 
-#, fuzzy
 msgctxt "field:account.payment,date:"
 msgid "Date"
-msgstr "日期格式"
+msgstr "Data"
 
-#, fuzzy
 msgctxt "field:account.payment,description:"
 msgid "Description"
-msgstr "描述"
+msgstr "Descriere"
 
-#, fuzzy
 msgctxt "field:account.payment,failed_by:"
 msgid "Failure Noted by"
-msgstr "添加用户"
+msgstr "Eșec Remarcat de"
 
-#, fuzzy
 msgctxt "field:account.payment,group:"
 msgid "Group"
-msgstr "用户组"
+msgstr "Grup"
 
 msgctxt "field:account.payment,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Jurnal"
 
 msgctxt "field:account.payment,kind:"
 msgid "Kind"
-msgstr ""
+msgstr "Fel"
 
 msgctxt "field:account.payment,line:"
 msgid "Line"
-msgstr ""
+msgstr "Rând"
 
 msgctxt "field:account.payment,origin:"
 msgid "Origin"
-msgstr ""
+msgstr "Origine"
 
 msgctxt "field:account.payment,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parte"
 
-#, fuzzy
 msgctxt "field:account.payment,process_method:"
 msgid "Process Method"
-msgstr "Process Payments"
+msgstr "Metoda de Procesare"
 
-#, fuzzy
 msgctxt "field:account.payment,state:"
 msgid "State"
-msgstr "状态"
+msgstr "Stare"
 
 msgctxt "field:account.payment,submitted_by:"
 msgid "Submitted by"
-msgstr ""
+msgstr "Trimis de"
 
-#, fuzzy
 msgctxt "field:account.payment,succeeded_by:"
 msgid "Success Noted by"
-msgstr "Succeed"
+msgstr "Succes Remarcat de"
 
 msgctxt "field:account.payment.group,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
-#, fuzzy
 msgctxt "field:account.payment.group,currency:"
 msgid "Currency"
-msgstr "Payment Journals"
+msgstr "Moneda"
 
 msgctxt "field:account.payment.group,journal:"
 msgid "Journal"
-msgstr ""
+msgstr "Jurnal"
 
 msgctxt "field:account.payment.group,kind:"
 msgid "Kind"
-msgstr ""
+msgstr "Fel"
 
 msgctxt "field:account.payment.group,number:"
 msgid "Number"
-msgstr ""
+msgstr "Numar"
 
-#, fuzzy
 msgctxt "field:account.payment.group,payment_amount:"
 msgid "Payment Total Amount"
-msgstr "Payment Journals"
+msgstr "Suma Totala de Plata"
 
-#, fuzzy
 msgctxt "field:account.payment.group,payment_amount_succeeded:"
 msgid "Payment Succeeded"
-msgstr "Succeeded"
+msgstr "Plata a Reușit"
 
-#, fuzzy
 msgctxt "field:account.payment.group,payment_complete:"
 msgid "Payment Complete"
-msgstr "Payment Groups"
+msgstr "Plata Finalizata"
 
-#, fuzzy
 msgctxt "field:account.payment.group,payment_count:"
 msgid "Payment Count"
-msgstr "Payment Journals"
+msgstr "Numar de Plati"
 
-#, fuzzy
 msgctxt "field:account.payment.group,payments:"
 msgid "Payments"
-msgstr "Payments"
+msgstr "Plati"
 
-#, fuzzy
 msgctxt "field:account.payment.group,process_method:"
 msgid "Process Method"
-msgstr "Process Payments"
+msgstr "Metoda de Procesare"
 
 msgctxt "field:account.payment.journal,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:account.payment.journal,currency:"
 msgid "Currency"
-msgstr ""
+msgstr "Moneda"
 
-#, fuzzy
 msgctxt "field:account.payment.journal,name:"
 msgid "Name"
-msgstr "纳木"
+msgstr "Nume"
 
 msgctxt "field:account.payment.journal,process_method:"
 msgid "Process Method"
-msgstr ""
+msgstr "Metoda de Procesare"
 
 msgctxt "field:party.party,payment_direct_debit:"
 msgid "Direct Debit"
-msgstr ""
+msgstr "Debit Direct"
 
 msgctxt "field:party.party,payment_direct_debits:"
 msgid "Direct Debits"
-msgstr ""
+msgstr "Debite Directe"
 
 msgctxt "field:party.party,payment_identical_parties:"
 msgid "Identical Parties"
-msgstr ""
+msgstr "Parti Identice"
 
 msgctxt "field:party.party,reception_direct_debits:"
 msgid "Direct Debits"
-msgstr ""
+msgstr "Debite Directe"
 
 msgctxt "field:party.party.payment_direct_debit,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
 msgctxt "field:party.party.payment_direct_debit,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parte"
 
 msgctxt "field:party.party.payment_direct_debit,payment_direct_debit:"
 msgid "Direct Debit"
-msgstr ""
+msgstr "Debit Direct"
 
 msgctxt "field:party.party.reception_direct_debit,company:"
 msgid "Company"
-msgstr ""
+msgstr "Companie"
 
-#, fuzzy
 msgctxt "field:party.party.reception_direct_debit,currency:"
 msgid "Currency"
-msgstr "Payment Journals"
+msgstr "Moneda"
 
-#, fuzzy
 msgctxt "field:party.party.reception_direct_debit,journal:"
 msgid "Journal"
-msgstr "Payment Journals"
+msgstr "Jurnal"
 
 msgctxt "field:party.party.reception_direct_debit,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parte"
 
-#, fuzzy
 msgctxt "field:party.party.reception_direct_debit,process_method:"
 msgid "Process Method"
-msgstr "Process Payments"
+msgstr "Metoda de Procesare"
 
 msgctxt "help:account.invoice,payment_direct_debit:"
 msgid "Check if the invoice is paid by direct debit."
-msgstr ""
+msgstr "Verifica daca factura este platita prin debit direct."
 
 msgctxt "help:account.move.line,payment_direct_debit:"
 msgid "Check if the line will be paid by direct debit."
-msgstr ""
+msgstr "Verifica daca linia va fi platita prin debit direct."
 
 msgctxt "help:account.move.line.create_direct_debit.start,date:"
 msgid "Create direct debit for lines due up to this date."
-msgstr ""
+msgstr "Creează debit direct pentru rândurile scadente până în această dată."
 
 msgctxt "help:account.move.line.pay.start,date:"
 msgid ""
 "When the payments are scheduled to happen.\n"
 "Leave empty to use the lines' maturity dates."
 msgstr ""
+"Când plățile sunt programate să aibă loc.\n"
+"Lăsați gol pentru a utiliza datele de scadență ale rândurilor."
 
 msgctxt "help:account.payment.group,payment_amount:"
 msgid "The sum of all payment amounts."
-msgstr ""
+msgstr "Totalul sumelor de plata."
 
 msgctxt "help:account.payment.group,payment_amount_succeeded:"
 msgid "The sum of the amounts of the successful payments."
-msgstr ""
+msgstr "Totalul sumelor platilor reusite."
 
 msgctxt "help:account.payment.group,payment_complete:"
 msgid "All the payments in the group are complete."
-msgstr ""
+msgstr "Toate platile din grup sunt complete."
 
 msgctxt "help:account.payment.group,payment_count:"
 msgid "The number of payments in the group."
-msgstr ""
+msgstr "Numarul de plati din grup."
 
 msgctxt "help:party.party,payment_direct_debit:"
 msgid "Check if supplier does direct debit."
-msgstr ""
+msgstr "Verificați dacă furnizorul efectuează debitare directă."
 
 msgctxt "help:party.party,reception_direct_debits:"
 msgid "Fill to debit automatically the customer."
-msgstr ""
+msgstr "Completați pentru a debita automat clientul."
 
 msgctxt "help:party.party.payment_direct_debit,payment_direct_debit:"
 msgid "Check if supplier does direct debit."
-msgstr ""
+msgstr "Verificați dacă furnizorul efectuează debitare directă."
 
+#, fuzzy
 msgctxt "model:account.configuration.payment_group_sequence,name:"
 msgid "Account Configuration Payment Group Sequence"
-msgstr ""
+msgstr "Secventa Grupului de Plati - Configurare Cont"
 
 msgctxt "model:account.move.line.create_direct_debit.start,name:"
 msgid "Create Direct Debit"
-msgstr ""
+msgstr "Creare Debit Direct"
 
-#, fuzzy
 msgctxt "model:account.move.line.pay.ask_journal,name:"
 msgid "Pay Line"
-msgstr "Pay Lines"
+msgstr "Rând de Plată"
 
-#, fuzzy
 msgctxt "model:account.move.line.pay.start,name:"
 msgid "Pay Line"
-msgstr "Pay Lines"
+msgstr "Rând de Plată"
 
-#, fuzzy
 msgctxt "model:account.payment,name:"
 msgid "Payment"
-msgstr "Payment"
+msgstr "Plată"
 
-#, fuzzy
 msgctxt "model:account.payment.group,name:"
 msgid "Payment Group"
-msgstr "Payment Groups"
+msgstr "Grup de Plati"
 
-#, fuzzy
 msgctxt "model:account.payment.journal,name:"
 msgid "Payment Journal"
-msgstr "Payment Journals"
+msgstr "Jurnal de Plati"
 
 msgctxt "model:ir.action,name:act_move_line_form"
 msgid "Lines to Pay"
-msgstr "Lines to Pay"
+msgstr "Rânduri de Plată"
 
 msgctxt "model:ir.action,name:act_pay_line"
 msgid "Pay Lines"
-msgstr "Pay Lines"
+msgstr "Rânduri de Plată"
 
 msgctxt "model:ir.action,name:act_payment_form"
 msgid "Payments"
-msgstr "Payments"
+msgstr "Plati"
 
 msgctxt "model:ir.action,name:act_payment_form_group_open"
 msgid "Payments"
-msgstr "Payments"
+msgstr "Plati"
 
 msgctxt "model:ir.action,name:act_payment_form_line_relate"
 msgid "Payments"
-msgstr "Payments"
+msgstr "Plati"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_payment_form_payable"
 msgid "Payable Payments"
-msgstr "Process Payments"
+msgstr "Plăţi Furnizor"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_payment_form_receivable"
 msgid "Receivable Payments"
-msgstr "Receivable"
+msgstr "Plăţi Client"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_payment_form_relate_party"
 msgid "Payments"
-msgstr "Payments"
+msgstr "Plati"
 
 msgctxt "model:ir.action,name:act_payment_group_form"
 msgid "Payment Groups"
-msgstr "Payment Groups"
+msgstr "Grupuri de Plati"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_payment_journal_form"
 msgid "Payment Journals"
-msgstr "Payment Journals"
+msgstr "Jurnale de Plati"
 
 msgctxt "model:ir.action,name:act_process_payments"
 msgid "Process Payments"
-msgstr "Process Payments"
+msgstr "Proceseaza Platile"
 
 msgctxt "model:ir.action,name:wizard_create_direct_debit"
 msgid "Create Direct Debit"
-msgstr ""
+msgstr "Creare Debit Direct"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_move_line_form_domain_payable"
 msgid "Payable"
-msgstr "Payable"
+msgstr "Furnizor"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_move_line_form_domain_receivable"
 msgid "Receivable"
-msgstr "Receivable"
+msgstr "Client"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_group_open_domain_all"
 msgid "All"
-msgstr "全部"
+msgstr "Tot"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_group_open_domain_failed"
 msgid "Failed"
-msgstr "Failed"
+msgstr "Esuat"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_group_open_domain_processing"
 msgid "Processing"
-msgstr "Processing"
+msgstr "Procesare"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_group_open_domain_succeeded"
 msgid "Succeeded"
-msgstr "Succeeded"
+msgstr "Reusit"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_payable_domain_all"
 msgid "All"
-msgstr "全部"
+msgstr "Tot"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_payable_domain_draft"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciorna"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_payable_domain_processing"
 msgid "Processing"
-msgstr "Processing"
+msgstr "Procesare"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_payable_domain_to_approve"
 msgid "To Approve"
-msgstr "Approve"
+msgstr "De Aprobat"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_payable_domain_to_process"
 msgid "To Process"
-msgstr "Processing"
+msgstr "De Procesat"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_receivable_domain_all"
 msgid "All"
-msgstr "全部"
+msgstr "Tot"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_receivable_domain_draft"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciorna"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_receivable_domain_processing"
 msgid "Processing"
-msgstr "Processing"
+msgstr "Procesare"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_form_receivable_domain_to_process"
 msgid "To Process"
-msgstr "Processing"
+msgstr "De Procesat"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_group_form_domain_all"
 msgid "All"
-msgstr "全部"
+msgstr "Tot"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_payment_group_form_domain_not_completed"
 msgid "Pending"
-msgstr ""
+msgstr "In derulare"
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_payment"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending payments with "
 "company \"%(company)s\"."
 msgstr ""
+"Nu puteți șterge partea \"%(party)s\" în timp ce aceasta are plăți în "
+"așteptare cu compania \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_move_cancel_payments"
 msgid ""
 "The moves \"%(moves)s\" contain lines with payments, you may want to cancel "
 "them before cancelling."
 msgstr ""
+"Mișcările \"%(moves)s\" conțin rânduri cu plăți, vă recomandăm să le anulați"
+" înainte."
 
 msgctxt "model:ir.message,text:msg_move_line_delegate_payments"
 msgid ""
 "The lines \"%(lines)s\" have payments, you may want to cancel them before "
 "delegating."
 msgstr ""
+"Rândurile \"%(lines)s\" au plăți, vă recomandăm să le anulați înainte de a "
+"delega."
 
 msgctxt "model:ir.message,text:msg_move_line_group_payments"
 msgid ""
 "The lines \"%(lines)s\" have payments, you may want to cancel them before "
 "grouping."
 msgstr ""
+"Rândurile \"%(lines)s\" au plăți, este posibil să doriți să le anulați "
+"înainte de grupare."
 
 msgctxt "model:ir.message,text:msg_move_line_reschedule_payments"
 msgid ""
 "The lines \"%(lines)s\" have payments, you may want to cancel them before "
 "rescheduling."
 msgstr ""
+"Rândurile \"%(lines)s\" au plăți, vă recomandăm să le anulați înainte de a "
+"reprograma."
 
 msgctxt "model:ir.message,text:msg_pay_line_blocked"
 msgid "Line \"%(line)s\" is blocked for payment."
-msgstr ""
+msgstr "Rândul \"%(line)s\" este blocat pentru plată."
 
 msgctxt "model:ir.message,text:msg_pay_line_group"
 msgid ""
 "The lines \"%(names)s\" for %(party)s could be grouped with the line "
 "\"%(line)s\"."
 msgstr ""
+"Rândurile \"%(names)s\" pentru %(party)s pot fi grupate cu rândul "
+"\"%(line)s\"."
 
 msgctxt "model:ir.message,text:msg_payment_delete_draft"
 msgid "To delete payment \"%(payment)s\" you must reset it to draft state."
 msgstr ""
+"Pentru a șterge plata \"%(payment)s\", trebuie să o resetați la starea de "
+"ciornă."
 
 msgctxt "model:ir.message,text:msg_payment_overpay"
 msgid "Payment \"%(payment)s\" overpays line \"%(line)s\"."
-msgstr ""
+msgstr "Plata \"%(payment)s\" plătește în exces linia \"%(line)s\"."
 
 msgctxt "model:ir.message,text:msg_payment_reconciled"
 msgid "The line \"%(line)s\" of payment \"%(payment)s\" is already reconciled."
-msgstr ""
+msgstr "Rândul \"%(line)s\" al plății \"%(payment)s\" este deja reconciliat."
 
 msgctxt "model:ir.model.button,confirm:payment_process_wizard_button"
 msgid "Are you sure you want to process the payments?"
-msgstr ""
+msgstr "Sigur doriți să procesați plățile?"
 
 msgctxt "model:ir.model.button,string:move_line_pay_button"
 msgid "Pay"
-msgstr ""
+msgstr "Plata"
 
 msgctxt "model:ir.model.button,string:move_line_payment_block_button"
 msgid "Block"
-msgstr "Block"
+msgstr "Blocare"
 
 msgctxt "model:ir.model.button,string:move_line_payment_unblock_button"
 msgid "Unblock"
-msgstr "Unblock"
+msgstr "Deblocare"
 
 msgctxt "model:ir.model.button,string:payment_approve_button"
 msgid "Approve"
-msgstr "Approve"
+msgstr "Aproba"
 
 msgctxt "model:ir.model.button,string:payment_draft_button"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciorna"
 
 msgctxt "model:ir.model.button,string:payment_fail_button"
 msgid "Fail"
-msgstr "Fail"
+msgstr "Esuat"
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:payment_group_succeed_button"
 msgid "Succeed"
-msgstr "Succeed"
+msgstr "Reusit"
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:payment_proceed_button"
 msgid "Processing"
-msgstr "Processing"
+msgstr "Procesare"
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:payment_process_wizard_button"
 msgid "Process"
-msgstr "Processing"
+msgstr "Proces"
 
 msgctxt "model:ir.model.button,string:payment_submit_button"
 msgid "Submit"
-msgstr ""
+msgstr "Trimite"
 
 msgctxt "model:ir.model.button,string:payment_succeed_button"
 msgid "Succeed"
-msgstr "Succeed"
+msgstr "Reusit"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_party_reception_direct_debit_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator in Companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_payment_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator in Companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_payment_group_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator in Companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_payment_journal_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator in Companii"
 
 msgctxt "model:ir.sequence,name:sequence_account_payment_group"
 msgid "Default Account Payment Group"
-msgstr "Default Account Payment Group"
+msgstr "Grup de plată implicit pentru cont"
 
 msgctxt "model:ir.sequence.type,name:sequence_type_account_payment_group"
 msgid "Account Payment Group"
-msgstr "Account Payment Group"
+msgstr "Grup de Plata in Cont"
 
 msgctxt "model:ir.ui.menu,name:menu_create_direct_debit"
 msgid "Create Direct Debit"
-msgstr ""
+msgstr "Creare Debit Direct"
 
 msgctxt "model:ir.ui.menu,name:menu_move_line_form"
 msgid "Lines to Pay"
-msgstr "Lines to Pay"
+msgstr "Randuri de Plata"
 
 msgctxt "model:ir.ui.menu,name:menu_payment_configuration"
 msgid "Payments"
-msgstr "Payments"
+msgstr "Plati"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_payment_form_payable"
 msgid "Payable Payments"
-msgstr "Process Payments"
+msgstr "Plăti Furnizor"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_payment_form_receivable"
 msgid "Receivable Payments"
-msgstr "Receivable"
+msgstr "Plati de Creanta"
 
 msgctxt "model:ir.ui.menu,name:menu_payment_group_form"
 msgid "Payment Groups"
-msgstr "Payment Groups"
+msgstr "Grupuri de Plati"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_payment_journal_form"
 msgid "Payment Journals"
-msgstr "Payment Journals"
+msgstr "Jurnale de Plati"
 
 msgctxt "model:ir.ui.menu,name:menu_payments"
 msgid "Payments"
-msgstr "Payments"
+msgstr "Plati"
 
 msgctxt "model:party.party.payment_direct_debit,name:"
 msgid "Party Payment Direct Debit"
-msgstr ""
+msgstr "Debitare Directă de Plată a Părților"
 
 msgctxt "model:party.party.reception_direct_debit,name:"
 msgid "Party Reception Direct Debit"
-msgstr ""
+msgstr "Parte Recepţie Debit Direct"
 
 msgctxt "model:res.group,name:group_payment"
 msgid "Payment"
-msgstr "Payment"
+msgstr "Plată"
 
 msgctxt "model:res.group,name:group_payment_approval"
 msgid "Payment Approval"
-msgstr "Payment Approval"
+msgstr "Aprobare Plata"
 
-#, fuzzy
 msgctxt "selection:account.move.line,payment_kind:"
 msgid "Payable"
-msgstr "Payable"
+msgstr "Furnizor"
 
-#, fuzzy
 msgctxt "selection:account.move.line,payment_kind:"
 msgid "Receivable"
-msgstr "Receivable"
+msgstr "Creanţa"
 
-#, fuzzy
 msgctxt "selection:account.payment,kind:"
 msgid "Payable"
-msgstr "Payable"
+msgstr "Furnizor"
 
-#, fuzzy
 msgctxt "selection:account.payment,kind:"
 msgid "Receivable"
-msgstr "Receivable"
+msgstr "Client"
 
-#, fuzzy
 msgctxt "selection:account.payment,state:"
 msgid "Approved"
-msgstr "Approve"
+msgstr "Aprobat"
 
-#, fuzzy
 msgctxt "selection:account.payment,state:"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciorna"
 
-#, fuzzy
 msgctxt "selection:account.payment,state:"
 msgid "Failed"
-msgstr "Failed"
+msgstr "Esuat"
 
-#, fuzzy
 msgctxt "selection:account.payment,state:"
 msgid "Processing"
-msgstr "Processing"
+msgstr "In Curs de Procesare"
 
 msgctxt "selection:account.payment,state:"
 msgid "Submitted"
-msgstr ""
+msgstr "Depus"
 
-#, fuzzy
 msgctxt "selection:account.payment,state:"
 msgid "Succeeded"
-msgstr "Succeed"
+msgstr "Reusit"
 
-#, fuzzy
 msgctxt "selection:account.payment.group,kind:"
 msgid "Payable"
-msgstr "Payable"
+msgstr "Furnizor"
 
-#, fuzzy
 msgctxt "selection:account.payment.group,kind:"
 msgid "Receivable"
-msgstr "Receivable"
+msgstr "Creanţe"
 
 msgctxt "selection:account.payment.journal,process_method:"
 msgid "Manual"
-msgstr ""
+msgstr "Manual"
 
 msgctxt "view:account.configuration:"
 msgid "Group Sequence"
-msgstr ""
+msgstr "Secventa de Grup"
 
-#, fuzzy
 msgctxt "view:account.configuration:"
 msgid "Payment"
-msgstr "Payment"
+msgstr "Plată"
 
 msgctxt "view:account.move.line.create_direct_debit.start:"
 msgid "Create Direct Debit for date"
-msgstr ""
+msgstr "Creare Debit Direct pentru Data de"
 
 msgctxt "view:account.payment.group:"
 msgid "Complete"
-msgstr ""
+msgstr "Complet"
 
 msgctxt "view:account.payment.group:"
 msgid "Count"
-msgstr ""
+msgstr "Numărare"
 
-#, fuzzy
 msgctxt "view:account.payment.group:"
 msgid "Payments Info"
-msgstr "Payments"
+msgstr "Informatii de Plata"
 
-#, fuzzy
 msgctxt "view:account.payment.group:"
 msgid "Succeeded"
-msgstr "Succeeded"
+msgstr "Reusit"
 
 msgctxt "view:account.payment.group:"
 msgid "Total Amount"
-msgstr ""
+msgstr "Suma Totala"
 
-#, fuzzy
 msgctxt "view:account.payment:"
 msgid "Description"
-msgstr "描述"
+msgstr "Descriere"
 
 msgctxt "view:account.payment:"
 msgid "Other Info"
-msgstr ""
+msgstr "Alte Informatii"
 
-#, fuzzy
 msgctxt "wizard_button:account.move.line.create_direct_debit,start,create_:"
 msgid "Create"
-msgstr "创建日期:"
+msgstr "Creare"
 
-#, fuzzy
 msgctxt "wizard_button:account.move.line.create_direct_debit,start,end:"
 msgid "Cancel"
-msgstr "取消"
+msgstr "Anulare"
 
-#, fuzzy
 msgctxt "wizard_button:account.move.line.pay,ask_journal,end:"
 msgid "Cancel"
-msgstr "取消"
+msgstr "Anulare"
 
 msgctxt "wizard_button:account.move.line.pay,ask_journal,next_:"
 msgid "Pay"
-msgstr ""
+msgstr "Plata"
 
-#, fuzzy
 msgctxt "wizard_button:account.move.line.pay,start,end:"
 msgid "Cancel"
-msgstr "取消"
+msgstr "Anuleaza"
 
 msgctxt "wizard_button:account.move.line.pay,start,next_:"
 msgid "Pay"
-msgstr ""
+msgstr "Plata"
```

### Comparing `trytond_account_payment-7.0.2/message.xml` & `trytond_account_payment-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/party.py` & `trytond_account_payment-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/party.xml` & `trytond_account_payment-7.2.0/party.xml`

 * *Files 13% similar despite different names*

#### Comparing `trytond_account_payment-7.0.2/party.xml` & `trytond_account_payment-7.2.0/party.xml`

```diff
@@ -16,30 +16,30 @@
     <record model="ir.ui.view" id="party_reception_direct_debit_view_list">
       <field name="model">party.party.reception_direct_debit</field>
       <field name="type">tree</field>
       <field name="name">party_reception_direct_debit_list</field>
     </record>
     <record model="ir.rule.group" id="rule_group_party_reception_direct_debit_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'party.party.reception_direct_debit')]"/>
+      <field name="model">party.party.reception_direct_debit</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_party_reception_direct_debit_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_party_reception_direct_debit_companies"/>
     </record>
     <record model="ir.model.access" id="access_party_reception_direct_debit">
-      <field name="model" search="[('model', '=', 'party.party.reception_direct_debit')]"/>
+      <field name="model">party.party.reception_direct_debit</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_party_reception_direct_debit_payment">
-      <field name="model" search="[('model', '=', 'party.party.reception_direct_debit')]"/>
+      <field name="model">party.party.reception_direct_debit</field>
       <field name="group" ref="group_payment"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_account_payment-7.0.2/payment.py` & `trytond_account_payment-7.2.0/payment.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/payment.xml` & `trytond_account_payment-7.2.0/payment.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_account_payment-7.0.2/payment.xml` & `trytond_account_payment-7.2.0/payment.xml`

```diff
@@ -46,38 +46,38 @@
       <field name="sequence" eval="20"/>
       <field name="view" ref="payment_journal_view_form"/>
       <field name="act_window" ref="act_payment_journal_form"/>
     </record>
     <menuitem parent="menu_payment_configuration" action="act_payment_journal_form" sequence="10" id="menu_payment_journal_form"/>
     <record model="ir.rule.group" id="rule_group_payment_journal_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.payment.journal')]"/>
+      <field name="model">account.payment.journal</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_payment_journal_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_payment_journal_companies"/>
     </record>
     <record model="ir.model.access" id="access_payment_journal">
-      <field name="model" search="[('model', '=', 'account.payment.journal')]"/>
+      <field name="model">account.payment.journal</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_payment_journal_account_admin">
-      <field name="model" search="[('model', '=', 'account.payment.journal')]"/>
+      <field name="model">account.payment.journal</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_payment_journal_payment">
-      <field name="model" search="[('model', '=', 'account.payment.journal')]"/>
+      <field name="model">account.payment.journal</field>
       <field name="group" ref="group_payment"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="payment_group_view_form">
@@ -116,48 +116,48 @@
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_payment_group_form"/>
     </record>
     <menuitem parent="menu_payments" action="act_payment_group_form" sequence="30" id="menu_payment_group_form"/>
     <record model="ir.rule.group" id="rule_group_payment_group_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.payment.group')]"/>
+      <field name="model">account.payment.group</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_payment_group_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_payment_group_companies"/>
     </record>
     <record model="ir.model.access" id="access_payment_group">
-      <field name="model" search="[('model', '=', 'account.payment.group')]"/>
+      <field name="model">account.payment.group</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_payment_group_account_admin">
-      <field name="model" search="[('model', '=', 'account.payment.group')]"/>
+      <field name="model">account.payment.group</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_payment_group_payment">
-      <field name="model" search="[('model', '=', 'account.payment.group')]"/>
+      <field name="model">account.payment.group</field>
       <field name="group" ref="group_payment"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.button" id="payment_group_succeed_button">
+      <field name="model">account.payment.group</field>
       <field name="name">succeed</field>
       <field name="string">Succeed</field>
-      <field name="model" search="[('model', '=', 'account.payment.group')]"/>
     </record>
     <record model="ir.sequence.type" id="sequence_type_account_payment_group">
       <field name="name">Account Payment Group</field>
     </record>
     <record model="ir.sequence.type-res.group" id="sequence_type_account_payment_group_group_admin">
       <field name="sequence_type" ref="sequence_type_account_payment_group"/>
       <field name="group" ref="res.group_admin"/>
@@ -284,15 +284,15 @@
     </record>
     <record model="ir.action.act_window.domain" id="act_payment_form_receivable_domain_all">
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_payment_form_receivable"/>
     </record>
-    <menuitem parent="menu_payments" action="act_payment_form_receivable" sequence="10" id="menu_payment_form_receivable"/>
+    <menuitem parent="menu_payments" action="act_payment_form_receivable" sequence="20" id="menu_payment_form_receivable"/>
     <record model="ir.action.act_window" id="act_payment_form_relate_party">
       <field name="name">Payments</field>
       <field name="res_model">account.payment</field>
       <field name="domain" eval="[If(Eval('active_ids', []) == [Eval('active_id')], ('party', '=', Eval('active_id')), ('party', 'in', Eval('active_ids')))]" pyson="1"/>
       <field name="search_value" eval="[('state', 'not in', ['succeeded', 'failed'])]" pyson="1"/>
     </record>
     <record model="ir.action.act_window.view" id="act_payment_form_relate_party_view1">
@@ -312,15 +312,15 @@
     </record>
     <record model="ir.action-res.group" id="act_payment_form_relate_party-group_payment">
       <field name="action" ref="act_payment_form_relate_party"/>
       <field name="group" ref="group_payment"/>
     </record>
     <record model="ir.rule.group" id="rule_group_payment_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
+      <field name="model">account.payment</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_payment_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_payment_companies"/>
     </record>
     <record model="ir.action.act_window" id="act_payment_form_line_relate">
@@ -387,83 +387,83 @@
     </record>
     <record model="ir.action.keyword" id="act_payment_form_group_relate_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">account.payment.group,-1</field>
       <field name="action" ref="act_payment_form_group_open"/>
     </record>
     <record model="ir.model.access" id="access_payment">
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
+      <field name="model">account.payment</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_payment_account_admin">
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
+      <field name="model">account.payment</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_payment_payment">
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
+      <field name="model">account.payment</field>
       <field name="group" ref="group_payment"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_payment_payment_approval">
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
+      <field name="model">account.payment</field>
       <field name="group" ref="group_payment_approval"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.button" id="payment_draft_button">
+      <field name="model">account.payment</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
     </record>
     <record model="ir.model.button" id="payment_submit_button">
+      <field name="model">account.payment</field>
       <field name="name">submit</field>
       <field name="string">Submit</field>
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
     </record>
     <record model="ir.model.button" id="payment_approve_button">
+      <field name="model">account.payment</field>
       <field name="name">approve</field>
       <field name="string">Approve</field>
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
     </record>
     <record model="ir.model.button-res.group" id="payment_approve_button_group_payment_approval">
       <field name="button" ref="payment_approve_button"/>
       <field name="group" ref="group_payment_approval"/>
     </record>
     <record model="ir.model.button" id="payment_process_wizard_button">
+      <field name="model">account.payment</field>
       <field name="name">process_wizard</field>
       <field name="string">Process</field>
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
       <field name="confirm">Are you sure you want to process the payments?</field>
     </record>
     <record model="ir.model.button" id="payment_proceed_button">
+      <field name="model">account.payment</field>
       <field name="name">proceed</field>
       <field name="string">Processing</field>
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
     </record>
     <record model="ir.model.button" id="payment_succeed_button">
+      <field name="model">account.payment</field>
       <field name="name">succeed</field>
       <field name="string">Succeed</field>
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
     </record>
     <record model="ir.model.button" id="payment_fail_button">
+      <field name="model">account.payment</field>
       <field name="name">fail</field>
       <field name="string">Fail</field>
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
     </record>
     <record model="ir.action.wizard" id="act_process_payments">
       <field name="name">Process Payments</field>
       <field name="wiz_name">account.payment.process</field>
       <field name="model">account.payment</field>
     </record>
   </data>
```

### Comparing `trytond_account_payment-7.0.2/setup.py` & `trytond_account_payment-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-account-payment'),
+            'https://docs.tryton.org/modules-account-payment'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account payment',
     package_dir={'trytond.modules.account_payment': '.'},
     packages=(
         ['trytond.modules.account_payment']
```

### Comparing `trytond_account_payment-7.0.2/tests/scenario_account_payment.rst` & `trytond_account_payment-7.2.0/tests/scenario_account_payment.rst`

 * *Files 20% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Payment Scenario
 ================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
     >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('account_payment')
@@ -82,37 +82,31 @@
 Partially pay line::
 
     >>> Payment = Model.get('account.payment')
     >>> line, = [l for l in move.lines if l.account == payable]
     >>> pay_line = Wizard('account.move.line.pay', [line])
     >>> pay_line.form.date = tomorrow
     >>> pay_line.execute('next_')
-    >>> pay_line.form.journal == payment_journal
-    True
+    >>> assertEqual(pay_line.form.journal, payment_journal)
     >>> pay_line.execute('next_')
     >>> payment, = Payment.find()
-    >>> payment.date == tomorrow
-    True
-    >>> payment.party == supplier
-    True
+    >>> assertEqual(payment.date, tomorrow)
+    >>> assertEqual(payment.party, supplier)
     >>> payment.amount
     Decimal('50.00')
     >>> payment.amount = Decimal('20.00')
     >>> payment.click('submit')
-    >>> payment.submitted_by == employee
-    True
+    >>> assertEqual(payment.submitted_by, employee)
     >>> payment.click('approve')
-    >>> payment.approved_by == employee
-    True
+    >>> assertEqual(payment.approved_by, employee)
     >>> payment.state
     'approved'
     >>> process_payment = payment.click('process_wizard')
     >>> group, = process_payment.actions[0]
-    >>> group.payments == [payment]
-    True
+    >>> assertEqual(group.payments, [payment])
     >>> payment.state
     'processing'
     >>> line.reload()
     >>> line.payment_amount
     Decimal('30.00')
 
 Check the properties of the payment group::
@@ -126,32 +120,30 @@
     >>> group.payment_complete
     False
 
 Success the payment and recheck the payment group::
 
     >>> group.click('succeed')
     >>> payment.reload()
-    >>> payment.succeeded_by == employee
-    True
+    >>> assertEqual(payment.succeeded_by, employee)
     >>> payment.state
     'succeeded'
     >>> group.reload()
     >>> group.payment_amount_succeeded
     Decimal('20.00')
     >>> group.payment_complete
     True
 
 Search for the completed payment::
 
     >>> PaymentGroup = Model.get('account.payment.group')
     >>> group, = PaymentGroup.find([('payment_complete', '=', 'True')])
     >>> group.payment_complete
     True
-    >>> group.id == payment.group.id
-    True
+    >>> assertEqual(group, payment.group)
 
 Partially fail to pay the remaining::
 
     >>> pay_line = Wizard('account.move.line.pay', [line])
     >>> pay_line.execute('next_')
     >>> pay_line.execute('next_')
     >>> payment, = Payment.find([('state', '=', 'draft')])
@@ -161,16 +153,15 @@
     >>> payment.click('approve')
     >>> process_payment = payment.click('process_wizard')
     >>> line.reload()
     >>> line.payment_amount
     Decimal('0.00')
     >>> payment.reload()
     >>> payment.click('fail')
-    >>> payment.failed_by == employee
-    True
+    >>> assertEqual(payment.failed_by, employee)
     >>> payment.state
     'failed'
     >>> payment.group.payment_complete
     True
     >>> payment.group.payment_amount_succeeded
     >>> line.reload()
     >>> line.payment_amount
@@ -191,11 +182,11 @@
     >>> len(line.payments)
     0
 
 Try to pay blocked line::
 
     >>> pay_line = Wizard('account.move.line.pay', [line])
     >>> pay_line.execute('next_')
-    >>> pay_line.execute('next_')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> pay_line.execute('next_')
     Traceback (most recent call last):
         ...
     BlockedWarning: ...
```

### Comparing `trytond_account_payment-7.0.2/tests/scenario_account_payment_blocked_direct_debit.rst` & `trytond_account_payment-7.2.0/tests/scenario_account_payment_blocked_direct_debit.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_payment')
```

### Comparing `trytond_account_payment-7.0.2/tests/scenario_account_payment_direct_debit.rst` & `trytond_account_payment-7.2.0/tests/scenario_account_payment_direct_debit.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
     >>> tomorrow = today + dt.timedelta(days=1)
     >>> after_tomorrow = tomorrow + dt.timedelta(days=1)
 
 Activate modules::
 
@@ -86,22 +85,18 @@
     >>> create_direct_debit = Wizard('account.move.line.create_direct_debit')
     >>> create_direct_debit.form.date = after_tomorrow
     >>> create_direct_debit.execute('create_')
 
     >>> payment, = Payment.find([])
     >>> payment.amount
     Decimal('100.00')
-    >>> payment.party == customer1
-    True
-    >>> payment.date == tomorrow
-    True
-    >>> payment.journal == payment_journal
-    True
+    >>> assertEqual(payment.party, customer1)
+    >>> assertEqual(payment.date, tomorrow)
+    >>> assertEqual(payment.journal, payment_journal)
 
 Re-run create direct debit does nothing::
 
     >>> create_direct_debit = Wizard('account.move.line.create_direct_debit')
     >>> create_direct_debit.form.date = after_tomorrow
     >>> create_direct_debit.execute('create_')
 
-    >>> Payment.find([]) == [payment]
-    True
+    >>> assertEqual(Payment.find([]), [payment])
```

### Comparing `trytond_account_payment-7.0.2/tests/scenario_account_payment_dunning.rst` & `trytond_account_payment-7.2.0/tests/scenario_account_payment_dunning.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(['account_payment', 'account_dunning'])
 
@@ -97,30 +96,28 @@
     []
 
 Fail the payment::
 
     >>> payment.click('submit')
     >>> process_payment = payment.click('process_wizard')
     >>> group, = process_payment.actions[0]
-    >>> group.payments == [payment]
-    True
+    >>> assertEqual(group.payments, [payment])
     >>> payment.click('fail')
     >>> payment.state
     'failed'
     >>> line.reload()
     >>> line.payment_amount
     Decimal('50.00')
 
 Create dunning::
 
     >>> create_dunning = Wizard('account.dunning.create')
     >>> create_dunning.execute('create_')
     >>> dunning, = Dunning.find([])
-    >>> dunning.line == line
-    True
+    >>> assertEqual(dunning.line, line)
 
 Recreate a payment::
 
     >>> pay_line = Wizard('account.move.line.pay', [line])
     >>> pay_line.execute('next_')
     >>> pay_line.execute('next_')
     >>> _, payment = line.payments
```

### Comparing `trytond_account_payment-7.0.2/tests/scenario_account_payment_invoice.rst` & `trytond_account_payment-7.2.0/tests/scenario_account_payment_invoice.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 ========================
 Invoice Payment Scenario
 ========================
 
 Imports::
 
-    >>> import datetime
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
 
 Activate modules::
 
     >>> config = activate_modules(['account_payment', 'account_invoice'])
 
 Create company::
```

### Comparing `trytond_account_payment-7.0.2/tests/scenario_account_payment_planning.rst` & `trytond_account_payment-7.2.0/tests/scenario_account_payment_planning.rst`

 * *Files 9% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Payment Planning Scenario
 =========================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
     >>> tomorrow = today + dt.timedelta(days=1)
     >>> next_week = today + dt.timedelta(weeks=1)
 
 Activate modules::
 
@@ -68,20 +68,18 @@
 
     >>> Payment = Model.get('account.payment')
     >>> line, = [l for l in move.lines if l.account == payable]
     >>> pay_line = Wizard('account.move.line.pay', [line])
     >>> pay_line.execute('next_')
     >>> pay_line.execute('next_')
     >>> payment, = Payment.find()
-    >>> payment.date == next_week
-    True
+    >>> assertEqual(payment.date, next_week)
 
 The date on the payment wizard is used for payment date::
 
     >>> payment.delete()
     >>> pay_line = Wizard('account.move.line.pay', [line])
     >>> pay_line.form.date = tomorrow
     >>> pay_line.execute('next_')
     >>> pay_line.execute('next_')
     >>> payment, = Payment.find()
-    >>> payment.date == tomorrow
-    True
+    >>> assertEqual(payment.date, tomorrow)
```

### Comparing `trytond_account_payment-7.0.2/tests/scenario_account_payment_statement.rst` & `trytond_account_payment-7.2.0/tests/scenario_account_payment_statement.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.tests.tools import activate_modules
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(['account_payment', 'account_statement'])
```

### Comparing `trytond_account_payment-7.0.2/tests/scenario_account_payment_warnings.rst` & `trytond_account_payment-7.2.0/tests/scenario_account_payment_warnings.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 =================================
 Account Payment Warnings Scenario
 =================================
 
 Imports::
 
-    >>> from decimal import Decimal
     >>> import datetime as dt
+    >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_payment')
 
@@ -81,46 +80,46 @@
     >>> pay_line.execute('next_')
     >>> pay_line.execute('next_')
     >>> payment, = Payment.find()
 
 Try to cancel move::
 
     >>> cancel_move = Wizard('account.move.cancel', [move])
-    >>> cancel_move.execute('cancel')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> cancel_move.execute('cancel')
     Traceback (most recent call last):
         ...
     CancelWarning: ...
 
 Try to group lines::
 
     >>> line2, = [l for l in move2.lines if l.account == accounts['payable']]
     >>> group_line = Wizard('account.move.line.group', [line, line2])
-    >>> group_line.execute('group')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> group_line.execute('group')
     Traceback (most recent call last):
         ...
     GroupLineWarning: ...
 
 Try to reschedule line::
 
     >>> reschedule_line = Wizard('account.move.line.reschedule', [line])
     >>> reschedule_line.form.start_date = today
     >>> reschedule_line.form.frequency = 'monthly'
     >>> reschedule_line.form.interval = 1
     >>> reschedule_line.form.amount = Decimal('50.00')
     >>> reschedule_line.execute('preview')
-    >>> reschedule_line.execute('reschedule')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> reschedule_line.execute('reschedule')
     Traceback (most recent call last):
         ...
     RescheduleLineWarning: ...
 
 Try to delegate line::
 
     >>> delegate_line = Wizard('account.move.line.delegate', [line])
     >>> delegate_line.form.party = supplier2
-    >>> delegate_line.execute('delegate')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> delegate_line.execute('delegate')
     Traceback (most recent call last):
         ...
     DelegateLineWarning: ...
 
 Reconcile line and try to submit::
 
     >>> move = Move()
@@ -136,11 +135,11 @@
     'posted'
 
     >>> cash_line, = [l for l in move.lines if l.account == accounts['payable']]
     >>> reconcile = Wizard('account.move.reconcile_lines', [payment.line, cash_line])
     >>> reconcile.state
     'end'
 
-    >>> payment.click('submit')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> payment.click('submit')
     Traceback (most recent call last):
         ...
     ReconciledWarning: ...
```

### Comparing `trytond_account_payment-7.0.2/tests/test_module.py` & `trytond_account_payment-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/tox.ini` & `trytond_account_payment-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/trytond_account_payment.egg-info/PKG-INFO` & `trytond_account_payment-7.2.0/trytond_account_payment.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment
-Version: 7.0.2
+Version: 7.2.0
 Summary: Tryton module for payment
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-payment
+Project-URL: Documentation, https://docs.tryton.org/modules-account-payment
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account payment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,24 +49,24 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_dunning<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_statement<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_dunning<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_statement<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
 
 ######################
 Account Payment Module
 ######################
 
 The *Account Payment Module* manages the receivable and payable payments.
 A payment is an order to pay an amount to a party or to receive an amount from
```

### Comparing `trytond_account_payment-7.0.2/trytond_account_payment.egg-info/SOURCES.txt` & `trytond_account_payment-7.2.0/trytond_account_payment.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 account.py
```

### Comparing `trytond_account_payment-7.0.2/view/move_line_form.xml` & `trytond_account_payment-7.2.0/view/move_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/view/move_line_list.xml` & `trytond_account_payment-7.2.0/view/move_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/view/payment_form.xml` & `trytond_account_payment-7.2.0/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/view/payment_group_form.xml` & `trytond_account_payment-7.2.0/view/payment_group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment-7.0.2/view/payment_list.xml` & `trytond_account_payment-7.2.0/view/payment_list.xml`

 * *Files identical despite different names*

