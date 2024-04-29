# Comparing `tmp/trytond_account_payment_braintree-7.0.0.tar.gz` & `tmp/trytond_account_payment_braintree-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment_braintree-7.0.0.tar", last modified: Mon Oct 30 17:22:46 2023, max compression
+gzip compressed data, was "trytond_account_payment_braintree-7.2.0.tar", last modified: Mon Apr 29 15:34:47 2024, max compression
```

## Comparing `trytond_account_payment_braintree-7.0.0.tar` & `trytond_account_payment_braintree-7.2.0.tar`

### file list

```diff
@@ -1,76 +1,75 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:22:46.853413 trytond_account_payment_braintree-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      231 2023-10-22 17:22:53.000000 trytond_account_payment_braintree-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      783 2023-10-30 17:02:35.000000 trytond_account_payment_braintree-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:02:34.000000 trytond_account_payment_braintree-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4933 2023-10-30 17:22:46.853413 trytond_account_payment_braintree-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2359 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1081 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    46420 2023-08-13 15:26:13.000000 trytond_account_payment_braintree-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16889 2023-10-27 17:38:49.000000 trytond_account_payment_braintree-7.0.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1696 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/checkout.html
--rw-r--r--   0 ced       (1000) ced       (1000)     3098 2023-08-13 15:26:13.000000 trytond_account_payment_braintree-7.0.0/common.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:22:46.850080 trytond_account_payment_braintree-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2826 2023-10-22 17:22:53.000000 trytond_account_payment_braintree-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2359 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:53.000000 trytond_account_payment_braintree-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1045 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:22:46.846747 trytond_account_payment_braintree-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13948 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13873 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13949 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14005 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11780 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11779 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13789 2023-10-30 16:47:45.000000 trytond_account_payment_braintree-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11698 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11686 2023-10-28 12:11:20.000000 trytond_account_payment_braintree-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      618 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2238 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2716 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:22:46.853413 trytond_account_payment_braintree-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4639 2023-10-27 17:38:49.000000 trytond_account_payment_braintree-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:22:46.846747 trytond_account_payment_braintree-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8692 2023-10-24 07:56:52.000000 trytond_account_payment_braintree-7.0.0/tests/scenario_account_payment_braintree.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_payment_braintree-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      145 2023-10-30 17:02:31.000000 trytond_account_payment_braintree-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:22:46.850080 trytond_account_payment_braintree-7.0.0/trytond_account_payment_braintree.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4933 2023-10-30 17:22:46.000000 trytond_account_payment_braintree-7.0.0/trytond_account_payment_braintree.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2318 2023-10-30 17:22:46.000000 trytond_account_payment_braintree-7.0.0/trytond_account_payment_braintree.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:22:46.000000 trytond_account_payment_braintree-7.0.0/trytond_account_payment_braintree.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-10-30 17:22:46.000000 trytond_account_payment_braintree-7.0.0/trytond_account_payment_braintree.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_account_payment_braintree-7.0.0/trytond_account_payment_braintree.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      173 2023-10-30 17:22:46.000000 trytond_account_payment_braintree-7.0.0/trytond_account_payment_braintree.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:22:46.000000 trytond_account_payment_braintree-7.0.0/trytond_account_payment_braintree.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:22:46.850080 trytond_account_payment_braintree-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/view/account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      264 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/view/account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      798 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/view/customer_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/view/customer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/view/customer_payment_method_delete_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      634 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/view/party_reception_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2272 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      451 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/view/payment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      760 2023-10-18 13:46:50.000000 trytond_account_payment_braintree-7.0.0/view/refund_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.0.0/view/refund_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:47.554953 trytond_account_payment_braintree-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      884 2024-04-29 15:15:08.000000 trytond_account_payment_braintree-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:15:08.000000 trytond_account_payment_braintree-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4933 2024-04-29 15:34:47.554953 trytond_account_payment_braintree-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2359 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1081 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    46420 2024-03-25 13:26:54.000000 trytond_account_payment_braintree-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16558 2024-04-27 16:30:39.000000 trytond_account_payment_braintree-7.2.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1696 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/checkout.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     3098 2024-01-27 09:58:52.000000 trytond_account_payment_braintree-7.2.0/common.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:47.551620 trytond_account_payment_braintree-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3088 2024-04-27 16:30:39.000000 trytond_account_payment_braintree-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2359 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:57.000000 trytond_account_payment_braintree-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1045 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:47.551620 trytond_account_payment_braintree-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13948 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13873 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13949 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14005 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11780 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11779 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13789 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13292 2024-04-29 13:17:17.000000 trytond_account_payment_braintree-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11686 2024-04-27 16:43:21.000000 trytond_account_payment_braintree-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      618 2024-03-25 13:26:54.000000 trytond_account_payment_braintree-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2238 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2716 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:34:47.554953 trytond_account_payment_braintree-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4639 2024-03-17 11:01:36.000000 trytond_account_payment_braintree-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:47.554953 trytond_account_payment_braintree-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8672 2024-04-22 12:14:36.000000 trytond_account_payment_braintree-7.2.0/tests/scenario_account_payment_braintree.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:57.000000 trytond_account_payment_braintree-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      145 2024-04-29 15:15:03.000000 trytond_account_payment_braintree-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:47.554953 trytond_account_payment_braintree-7.2.0/trytond_account_payment_braintree.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4933 2024-04-29 15:34:47.000000 trytond_account_payment_braintree-7.2.0/trytond_account_payment_braintree.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2300 2024-04-29 15:34:47.000000 trytond_account_payment_braintree-7.2.0/trytond_account_payment_braintree.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:34:47.000000 trytond_account_payment_braintree-7.2.0/trytond_account_payment_braintree.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:34:47.000000 trytond_account_payment_braintree-7.2.0/trytond_account_payment_braintree.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_account_payment_braintree-7.2.0/trytond_account_payment_braintree.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      173 2024-04-29 15:34:47.000000 trytond_account_payment_braintree-7.2.0/trytond_account_payment_braintree.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:34:47.000000 trytond_account_payment_braintree-7.2.0/trytond_account_payment_braintree.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:47.554953 trytond_account_payment_braintree-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      812 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/view/account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      264 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/view/account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      798 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/view/customer_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/view/customer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/view/customer_payment_method_delete_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      634 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/view/party_reception_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2272 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      451 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/view/payment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      863 2024-03-17 11:01:36.000000 trytond_account_payment_braintree-7.2.0/view/refund_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_account_payment_braintree-7.2.0/view/refund_list.xml
```

### Comparing `trytond_account_payment_braintree-7.0.0/CHANGELOG` & `trytond_account_payment_braintree-7.2.0/CHANGELOG`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.2.0 - 2024-04-29
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 
 Version 6.8.0 - 2023-05-01
 --------------------------
```

### Comparing `trytond_account_payment_braintree-7.0.0/COPYRIGHT` & `trytond_account_payment_braintree-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2020-2023 B2CK
-Copyright (C) 2020-2023 Cédric Krier
+Copyright (C) 2020-2024 B2CK
+Copyright (C) 2020-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_payment_braintree-7.0.0/LICENSE` & `trytond_account_payment_braintree-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/PKG-INFO` & `trytond_account_payment_braintree-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_braintree
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for Braintree payment
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,21 +48,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: braintree>=3.38.0
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_payment<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_payment<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Payment Braintree Module
 ################################
 
 The account_payment_braintree module allows receipt of payments using
 `Braintree`_.
 It uses the `Drop-in UI`_ in a checkout form to handle the `payment method
```

### Comparing `trytond_account_payment_braintree-7.0.0/README.rst` & `trytond_account_payment_braintree-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/__init__.py` & `trytond_account_payment_braintree-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/account.py` & `trytond_account_payment_braintree-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/account.xml` & `trytond_account_payment_braintree-7.2.0/account.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_account_payment_braintree-7.0.0/account.xml` & `trytond_account_payment_braintree-7.2.0/account.xml`

```diff
@@ -30,51 +30,53 @@
     <record model="ir.action.act_window.view" id="act_account_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="account_view_form"/>
       <field name="act_window" ref="act_account_form"/>
     </record>
     <menuitem parent="account_payment.menu_payment_configuration" sequence="50" action="act_account_form" id="menu_account_form"/>
     <record model="ir.model.button" id="account_new_identifier_button">
+      <field name="model">account.payment.braintree.account</field>
       <field name="name">new_identifier</field>
       <field name="string">New URL</field>
       <field name="confirm">This action will make the previous URL unusable. Do you want to continue?</field>
-      <field name="model" search="[('model', '=', 'account.payment.braintree.account')]"/>
     </record>
     <record model="ir.model.access" id="access_account">
-      <field name="model" search="[('model', '=', 'account.payment.braintree.account')]"/>
+      <field name="model">account.payment.braintree.account</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_account_account_admin">
-      <field name="model" search="[('model', '=', 'account.payment.braintree.account')]"/>
+      <field name="model">account.payment.braintree.account</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_account_payment">
-      <field name="model" search="[('model', '=', 'account.payment.braintree.account')]"/>
+      <field name="model">account.payment.braintree.account</field>
       <field name="group" ref="account_payment.group_payment"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_account_private_key">
-      <field name="field" search="[('name', '=', 'private_key'), ('model.model', '=', 'account.payment.braintree.account')]"/>
+      <field name="model">account.payment.braintree.account</field>
+      <field name="field">private_key</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_account_private_key_account_admin">
-      <field name="field" search="[('name', '=', 'private_key'), ('model.model', '=', 'account.payment.braintree.account')]"/>
+      <field name="model">account.payment.braintree.account</field>
+      <field name="field">private_key</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="payment_view_form">
@@ -84,27 +86,27 @@
     </record>
     <record model="ir.ui.view" id="payment_view_list">
       <field name="model">account.payment</field>
       <field name="inherit" ref="account_payment.payment_view_list"/>
       <field name="name">payment_list</field>
     </record>
     <record model="ir.model.button" id="payment_braintree_checkout_button">
+      <field name="model">account.payment</field>
       <field name="name">braintree_checkout</field>
       <field name="string">Braintree Checkout</field>
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
     </record>
     <record model="ir.model.button" id="payment_braintree_settle_payment_button">
+      <field name="model">account.payment</field>
       <field name="name">braintree_do_settle_payment</field>
       <field name="string">Braintree Settle Payment</field>
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
     </record>
     <record model="ir.model.button" id="payment_braintree_pull_button">
+      <field name="model">account.payment</field>
       <field name="name">braintree_do_pull</field>
       <field name="string">Braintree Pull</field>
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
     </record>
     <record model="ir.cron" id="cron_transact_payment">
       <field name="method">account.payment|braintree_transact</field>
       <field name="interval_number" eval="15"/>
       <field name="interval_type">minutes</field>
     </record>
     <record model="ir.cron" id="cron_pull_payment">
@@ -180,27 +182,27 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_refund_form"/>
     </record>
     <menuitem parent="account_payment.menu_payments" sequence="20" action="act_refund_form" id="menu_refund_form"/>
     <record model="ir.model.button" id="refund_draft_button">
+      <field name="model">account.payment.braintree.refund</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'account.payment.braintree.refund')]"/>
     </record>
     <record model="ir.model.button" id="refund_submit_button">
+      <field name="model">account.payment.braintree.refund</field>
       <field name="name">submit</field>
       <field name="string">Submit</field>
-      <field name="model" search="[('model', '=', 'account.payment.braintree.refund')]"/>
     </record>
     <record model="ir.model.button" id="refund_approve_button">
+      <field name="model">account.payment.braintree.refund</field>
       <field name="name">approve</field>
       <field name="string">Approve</field>
-      <field name="model" search="[('model', '=', 'account.payment.braintree.refund')]"/>
     </record>
     <record model="ir.cron" id="cron_refund">
       <field name="method">account.payment.braintree.refund|braintree_refund</field>
       <field name="interval_number" eval="15"/>
       <field name="interval_type">minutes</field>
     </record>
     <record model="ir.cron" id="cron_pull_refund">
@@ -230,47 +232,47 @@
     <record model="ir.action.act_window.view" id="act_customer_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="customer_view_form"/>
       <field name="act_window" ref="act_customer_form"/>
     </record>
     <menuitem parent="account_payment.menu_payments" sequence="50" action="act_customer_form" id="menu_customer_form"/>
     <record model="ir.model.access" id="access_customer">
-      <field name="model" search="[('model', '=', 'account.payment.braintree.customer')]"/>
+      <field name="model">account.payment.braintree.customer</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_customer_payment">
-      <field name="model" search="[('model', '=', 'account.payment.braintree.customer')]"/>
+      <field name="model">account.payment.braintree.customer</field>
       <field name="group" ref="account_payment.group_payment"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="customer_braintree_checkout_button">
+      <field name="model">account.payment.braintree.customer</field>
       <field name="name">braintree_checkout</field>
       <field name="string">Add Card</field>
-      <field name="model" search="[('model', '=', 'account.payment.braintree.customer')]"/>
     </record>
     <record model="ir.cron" id="cron_create_customer">
       <field name="method">account.payment.braintree.customer|braintree_create</field>
       <field name="interval_number" eval="1"/>
       <field name="interval_type">hours</field>
     </record>
     <record model="ir.cron" id="cron_delete_customer">
       <field name="method">account.payment.braintree.customer|braintree_delete</field>
       <field name="interval_number" eval="1"/>
       <field name="interval_type">hours</field>
     </record>
     <record model="ir.model.button" id="customer_payment_method_delete_button">
+      <field name="model">account.payment.braintree.customer</field>
       <field name="name">delete_payment_method</field>
       <field name="string">Delete Payment Method</field>
-      <field name="model" search="[('model', '=', 'account.payment.braintree.customer')]"/>
     </record>
     <record model="ir.action.wizard" id="wizard_customer_payment_method_delete">
       <field name="name">Delete Payment Method</field>
       <field name="wiz_name">account.payment.braintree.customer.payment_method.delete</field>
       <field name="model">account.payment.braintree.customer</field>
     </record>
     <record model="ir.ui.view" id="customer_payment_method_delete_ask_view_form">
@@ -284,14 +286,14 @@
     </record>
     <record model="ir.action.url" id="url_checkout">
       <field name="name">Braintree Checkout</field>
       <field name="url">%(http_host)s/%(database)s/account_payment_braintree/checkout/%(model)s/%(id)s</field>
     </record>
     <record model="ir.action.report" id="report_checkout">
       <field name="name">Braintree Checkout</field>
-      <field name="model"/>
+      <field name="model" eval="None"/>
       <field name="report_name">account.payment.braintree.checkout</field>
       <field name="report">account_payment_braintree/checkout.html</field>
       <field name="template_extension">html</field>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_account_payment_braintree-7.0.0/checkout.html` & `trytond_account_payment_braintree-7.2.0/checkout.html`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/common.py` & `trytond_account_payment_braintree-7.2.0/common.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/doc/conf.py` & `trytond_account_payment_braintree-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_payment_braintree-7.0.0/doc/index.rst` & `trytond_account_payment_braintree-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/ir.py` & `trytond_account_payment_braintree-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/bg.po` & `trytond_account_payment_braintree-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/ca.po` & `trytond_account_payment_braintree-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/cs.po` & `trytond_account_payment_braintree-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/de.po` & `trytond_account_payment_braintree-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/es.po` & `trytond_account_payment_braintree-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/es_419.po` & `trytond_account_payment_braintree-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/et.po` & `trytond_account_payment_braintree-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/fa.po` & `trytond_account_payment_braintree-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/fi.po` & `trytond_account_payment_braintree-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/fr.po` & `trytond_account_payment_braintree-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/hu.po` & `trytond_account_payment_braintree-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/id.po` & `trytond_account_payment_braintree-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/it.po` & `trytond_account_payment_braintree-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/lo.po` & `trytond_account_payment_braintree-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/lt.po` & `trytond_account_payment_braintree-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/nl.po` & `trytond_account_payment_braintree-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/pl.po` & `trytond_account_payment_braintree-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/pt.po` & `trytond_account_payment_braintree-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/ro.po` & `trytond_account_payment_braintree-7.2.0/locale/ru.po`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 msgctxt "field:account.payment.braintree.account,webhook_identifier:"
 msgid "Webhook Identifier"
 msgstr ""
 
 msgctxt "field:account.payment.braintree.customer,braintree_account:"
 msgid "Account"
-msgstr "Cont"
+msgstr ""
 
 msgctxt "field:account.payment.braintree.customer,braintree_checkout_id:"
 msgid "Braintree Checkout ID"
 msgstr ""
 
 msgctxt "field:account.payment.braintree.customer,braintree_client_token:"
 msgid "Braintree Client Token"
@@ -154,15 +154,15 @@
 msgctxt ""
 "field:account.payment.braintree.customer.payment_method.delete.ask,payment_method:"
 msgid "Payment Method"
 msgstr ""
 
 msgctxt "field:account.payment.braintree.refund,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "field:account.payment.braintree.refund,approved_by:"
 msgid "Approved by"
 msgstr ""
 
 msgctxt "field:account.payment.braintree.refund,braintree_error_message:"
 msgid "Braintree Error Message"
@@ -190,15 +190,15 @@
 
 msgctxt "field:account.payment.braintree.refund,submitted_by:"
 msgid "Submitted by"
 msgstr ""
 
 msgctxt "field:account.payment.journal,braintree_account:"
 msgid "Account"
-msgstr "Cont"
+msgstr ""
 
 msgctxt "field:party.party,braintree_customers:"
 msgid "Braintree Customers"
 msgstr ""
 
 msgctxt "field:party.party.reception_direct_debit,braintree_account:"
 msgid "Braintree Account"
```

### Comparing `trytond_account_payment_braintree-7.0.0/locale/ru.po` & `trytond_account_payment_braintree-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/sl.po` & `trytond_account_payment_braintree-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/tr.po` & `trytond_account_payment_braintree-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/locale/uk.po` & `trytond_account_payment_braintree-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/message.xml` & `trytond_account_payment_braintree-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/party.py` & `trytond_account_payment_braintree-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/party.xml` & `trytond_account_payment_braintree-7.2.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/routes.py` & `trytond_account_payment_braintree-7.2.0/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/setup.py` & `trytond_account_payment_braintree-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/tests/scenario_account_payment_braintree.rst` & `trytond_account_payment_braintree-7.2.0/tests/scenario_account_payment_braintree.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 ==================================
 
 Imports::
 
     >>> import os
     >>> import random
     >>> from decimal import Decimal
+
     >>> import braintree
     >>> from braintree.test.nonces import Nonces
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, create_fiscalyear
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, assertTrue
 
 Activate modules::
 
     >>> config = activate_modules('account_payment_braintree')
 
 Get cron::
 
@@ -105,34 +105,31 @@
     ...     }, config.context)
 
 Process the payment::
 
     >>> process_payment = payment.click('process_wizard')
     >>> payment.state
     'processing'
-    >>> bool(payment.braintree_payment_settled)
-    True
-    >>> payment.amount == amount
-    True
+    >>> assertTrue(payment.braintree_payment_settled)
+    >>> assertEqual(payment.amount, amount)
 
     >>> _ = gateway.testing.settle_transaction(payment.braintree_transaction_id)
 
 Pull update::
 
     >>> cron_payment_pull, = Cron.find([
     ...     ('method', '=', 'account.payment|braintree_pull'),
     ...     ])
     >>> cron_payment_pull.companies.append(Company(company.id))
     >>> cron_payment_pull.click('run_once')
 
     >>> payment.reload()
     >>> payment.state
     'succeeded'
-    >>> payment.amount == amount
-    True
+    >>> assertEqual(payment.amount, amount)
 
 Create a customer::
 
     >>> Customer = Model.get('account.payment.braintree.customer')
     >>> braintree_customer = Customer()
     >>> braintree_customer.party = customer
     >>> braintree_customer.braintree_account = braintree_account
@@ -256,16 +253,15 @@
     >>> cron_refund.companies.append(Company(company.id))
     >>> cron_refund.click('run_once')
 
     >>> refund.reload()
     >>> refund.state
     'processing'
     >>> payment.reload()
-    >>> payment.amount == amount
-    True
+    >>> assertEqual(payment.amount, amount)
 
     >>> _ = gateway.testing.settle_transaction(refund.braintree_transaction_id)
     >>> cron_refund_pull, = Cron.find([
     ...     ('method', '=', 'account.payment.braintree.refund|braintree_pull'),
     ...     ])
     >>> cron_refund_pull.companies.append(Company(company.id))
     >>> cron_refund_pull.click('run_once')
```

### Comparing `trytond_account_payment_braintree-7.0.0/tox.ini` & `trytond_account_payment_braintree-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/trytond_account_payment_braintree.egg-info/PKG-INFO` & `trytond_account_payment_braintree-7.2.0/trytond_account_payment_braintree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-payment-braintree
-Version: 7.0.0
+Name: trytond_account_payment_braintree
+Version: 7.2.0
 Summary: Tryton module for Braintree payment
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,21 +48,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: braintree>=3.38.0
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_payment<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_payment<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Payment Braintree Module
 ################################
 
 The account_payment_braintree module allows receipt of payments using
 `Braintree`_.
 It uses the `Drop-in UI`_ in a checkout form to handle the `payment method
```

### Comparing `trytond_account_payment_braintree-7.0.0/trytond_account_payment_braintree.egg-info/SOURCES.txt` & `trytond_account_payment_braintree-7.2.0/trytond_account_payment_braintree.egg-info/SOURCES.txt`

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

### Comparing `trytond_account_payment_braintree-7.0.0/view/account_form.xml` & `trytond_account_payment_braintree-7.2.0/view/account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/view/customer_form.xml` & `trytond_account_payment_braintree-7.2.0/view/customer_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/view/party_reception_direct_debit_form.xml` & `trytond_account_payment_braintree-7.2.0/view/party_reception_direct_debit_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/view/payment_form.xml` & `trytond_account_payment_braintree-7.2.0/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_braintree-7.0.0/view/refund_form.xml` & `trytond_account_payment_braintree-7.2.0/view/refund_form.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_account_payment_braintree-7.0.0/view/refund_form.xml` & `trytond_account_payment_braintree-7.2.0/view/refund_form.xml`

```diff
@@ -2,14 +2,16 @@
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <form>
   <label name="payment"/>
   <field name="payment"/>
   <label name="amount"/>
   <field name="amount"/>
+  <label name="braintree_transaction_id"/>
+  <field name="braintree_transaction_id" colspan="3"/>
   <label name="braintree_error_message"/>
   <field name="braintree_error_message" colspan="3" yexpand="0" height="80"/>
   <label name="submitted_by"/>
   <field name="submitted_by"/>
   <label name="approved_by"/>
   <field name="approved_by"/>
   <label name="state"/>
```

