# Comparing `tmp/trytond_account_payment_stripe-7.0.3.tar.gz` & `tmp/trytond_account_payment_stripe-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment_stripe-7.0.3.tar", last modified: Wed Apr 17 10:42:05 2024, max compression
+gzip compressed data, was "trytond_account_payment_stripe-7.2.0.tar", last modified: Mon Apr 29 15:35:15 2024, max compression
```

## Comparing `trytond_account_payment_stripe-7.0.3.tar` & `trytond_account_payment_stripe-7.2.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:42:05.739939 trytond_account_payment_stripe-7.0.3/
--rw-r--r--   0 ced       (1000) ced       (1000)     2336 2024-04-17 10:42:02.000000 trytond_account_payment_stripe-7.0.3/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-17 10:42:02.000000 trytond_account_payment_stripe-7.0.3/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     5117 2024-04-17 10:42:05.739939 trytond_account_payment_stripe-7.0.3/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2533 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      953 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5183 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/checkout.html
--rw-r--r--   0 ced       (1000) ced       (1000)     5064 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/common.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:42:05.733273 trytond_account_payment_stripe-7.0.3/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2801 2024-03-03 16:24:20.000000 trytond_account_payment_stripe-7.0.3/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2533 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1274 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/email_checkout.html
--rw-r--r--   0 ced       (1000) ced       (1000)     1091 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:42:05.736606 trytond_account_payment_stripe-7.0.3/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17701 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17557 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17713 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14745 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14708 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17994 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17665 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14826 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16182 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16208 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17330 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16207 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16909 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14655 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16624 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14625 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16196 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      780 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2285 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    70748 2024-04-12 20:15:59.000000 trytond_account_payment_stripe-7.0.3/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17754 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2861 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:42:05.739939 trytond_account_payment_stripe-7.0.3/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4553 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:42:05.736606 trytond_account_payment_stripe-7.0.3/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10828 2024-02-29 11:47:00.000000 trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8962 2024-02-29 11:47:00.000000 trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe_dispute.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3211 2024-02-05 16:24:27.000000 trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe_identical.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5579 2024-02-29 11:47:00.000000 trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe_intent.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      132 2024-03-03 12:25:53.000000 trytond_account_payment_stripe-7.0.3/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:42:05.739939 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     5117 2024-04-17 10:42:05.000000 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2607 2024-04-17 10:42:05.000000 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:42:05.000000 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-17 10:42:05.000000 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:36.000000 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      143 2024-04-17 10:42:05.000000 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:42:05.000000 trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:42:05.739939 trytond_account_payment_stripe-7.0.3/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/customer_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/customer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/customer_source_detach_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/party_reception_direct_debit_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2519 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      439 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/payment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      955 2024-02-05 16:24:27.000000 trytond_account_payment_stripe-7.0.3/view/refund_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-10-30 17:06:38.000000 trytond_account_payment_stripe-7.0.3/view/refund_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:15.390892 trytond_account_payment_stripe-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2134 2024-04-29 15:15:29.000000 trytond_account_payment_stripe-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:15:29.000000 trytond_account_payment_stripe-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment_stripe-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     5117 2024-04-29 15:35:15.390892 trytond_account_payment_stripe-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2533 2024-02-04 18:51:26.000000 trytond_account_payment_stripe-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      953 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5183 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/checkout.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     5064 2024-01-27 09:58:52.000000 trytond_account_payment_stripe-7.2.0/common.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:15.387559 trytond_account_payment_stripe-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_account_payment_stripe-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2533 2024-02-04 18:51:26.000000 trytond_account_payment_stripe-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:58.000000 trytond_account_payment_stripe-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1274 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/email_checkout.html
+-rw-r--r--   0 ced       (1000) ced       (1000)     1091 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:15.387559 trytond_account_payment_stripe-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17701 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17557 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17713 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14745 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14708 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17994 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17665 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14826 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16182 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16208 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17330 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16207 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16909 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14891 2024-04-29 13:17:17.000000 trytond_account_payment_stripe-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16624 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14625 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16196 2024-04-27 16:43:21.000000 trytond_account_payment_stripe-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      780 2024-03-25 13:26:54.000000 trytond_account_payment_stripe-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2285 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      556 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    70679 2024-04-27 16:30:39.000000 trytond_account_payment_stripe-7.2.0/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17311 2024-04-27 16:30:39.000000 trytond_account_payment_stripe-7.2.0/payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2861 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:35:15.390892 trytond_account_payment_stripe-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4553 2024-03-17 11:01:36.000000 trytond_account_payment_stripe-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:15.387559 trytond_account_payment_stripe-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10754 2024-04-27 16:30:39.000000 trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8914 2024-04-27 16:30:39.000000 trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe_dispute.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3149 2024-04-22 12:14:36.000000 trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe_identical.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5531 2024-04-27 16:30:39.000000 trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe_intent.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:58.000000 trytond_account_payment_stripe-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      132 2024-04-29 15:15:24.000000 trytond_account_payment_stripe-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:15.390892 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5117 2024-04-29 15:35:14.000000 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2607 2024-04-29 15:35:15.000000 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:35:14.000000 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:35:14.000000 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      143 2024-04-29 15:35:14.000000 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:35:14.000000 trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:35:15.390892 trytond_account_payment_stripe-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      717 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-01-16 14:00:20.000000 trytond_account_payment_stripe-7.2.0/view/account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/customer_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/customer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/customer_source_detach_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      871 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/party_reception_direct_debit_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2519 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      439 2023-01-16 14:00:20.000000 trytond_account_payment_stripe-7.2.0/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/payment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1039 2024-03-17 11:01:36.000000 trytond_account_payment_stripe-7.2.0/view/refund_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-04-15 07:12:15.000000 trytond_account_payment_stripe-7.2.0/view/refund_list.xml
```

### Comparing `trytond_account_payment_stripe-7.0.3/CHANGELOG` & `trytond_account_payment_stripe-7.2.0/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,9 @@
 
-Version 7.0.3 - 2024-04-17
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.2 - 2024-03-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2024-02-03
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_payment_stripe-7.0.3/COPYRIGHT` & `trytond_account_payment_stripe-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/LICENSE` & `trytond_account_payment_stripe-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/PKG-INFO` & `trytond_account_payment_stripe-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_stripe
-Version: 7.0.3
+Version: 7.2.0
 Summary: Tryton module for Stripe payment
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
@@ -49,20 +49,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: stripe>=2.32.0
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_payment<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_payment<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Payment Stripe Module
 #############################
 
 The account_payment_stripe module allows to receive payment from `Stripe`_.
 It uses `Stripe.js and Stripe Elements`_ in a checkout form to handle `Setup
 Intent`_ and `Payment Intent`_ by card.
```

### Comparing `trytond_account_payment_stripe-7.0.3/README.rst` & `trytond_account_payment_stripe-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/__init__.py` & `trytond_account_payment_stripe-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/checkout.html` & `trytond_account_payment_stripe-7.2.0/checkout.html`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/common.py` & `trytond_account_payment_stripe-7.2.0/common.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/doc/conf.py` & `trytond_account_payment_stripe-7.2.0/doc/conf.py`

 * *Files 8% similar despite different names*

```diff
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

### Comparing `trytond_account_payment_stripe-7.0.3/doc/index.rst` & `trytond_account_payment_stripe-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/email_checkout.html` & `trytond_account_payment_stripe-7.2.0/email_checkout.html`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/ir.py` & `trytond_account_payment_stripe-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/bg.po` & `trytond_account_payment_stripe-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/ca.po` & `trytond_account_payment_stripe-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/cs.po` & `trytond_account_payment_stripe-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/de.po` & `trytond_account_payment_stripe-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/es.po` & `trytond_account_payment_stripe-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/es_419.po` & `trytond_account_payment_stripe-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/et.po` & `trytond_account_payment_stripe-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/fa.po` & `trytond_account_payment_stripe-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/fi.po` & `trytond_account_payment_stripe-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/fr.po` & `trytond_account_payment_stripe-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/hu.po` & `trytond_account_payment_stripe-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/id.po` & `trytond_account_payment_stripe-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/it.po` & `trytond_account_payment_stripe-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/lo.po` & `trytond_account_payment_stripe-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/lt.po` & `trytond_account_payment_stripe-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/nl.po` & `trytond_account_payment_stripe-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/pl.po` & `trytond_account_payment_stripe-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/pt.po` & `trytond_account_payment_stripe-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/ro.po` & `trytond_account_payment_stripe-7.2.0/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 msgctxt "field:account.payment,stripe_token:"
 msgid "Stripe Token"
 msgstr ""
 
 msgctxt "field:account.payment.journal,stripe_account:"
 msgid "Account"
-msgstr "Cont"
+msgstr ""
 
 msgctxt "field:account.payment.stripe.account,last_event:"
 msgid "Last Event"
 msgstr ""
 
 msgctxt "field:account.payment.stripe.account,name:"
 msgid "Name"
@@ -140,19 +140,19 @@
 
 msgctxt "field:account.payment.stripe.customer,identical_customers:"
 msgid "Identical Customers"
 msgstr ""
 
 msgctxt "field:account.payment.stripe.customer,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:account.payment.stripe.customer,stripe_account:"
 msgid "Account"
-msgstr "Cont"
+msgstr ""
 
 msgctxt "field:account.payment.stripe.customer,stripe_checkout_id:"
 msgid "Stripe Checkout ID"
 msgstr ""
 
 msgctxt "field:account.payment.stripe.customer,stripe_checkout_needed:"
 msgid "Stripe Checkout Needed"
@@ -204,15 +204,15 @@
 
 msgctxt "field:account.payment.stripe.customer.source.detach.ask,source:"
 msgid "Source"
 msgstr ""
 
 msgctxt "field:account.payment.stripe.refund,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "field:account.payment.stripe.refund,approved_by:"
 msgid "Approved by"
 msgstr ""
 
 msgctxt "field:account.payment.stripe.refund,company:"
 msgid "Company"
@@ -262,18 +262,17 @@
 msgid "Submitted by"
 msgstr ""
 
 msgctxt "field:party.party,stripe_customers:"
 msgid "Stripe Customers"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:party.party.reception_direct_debit,stripe_account:"
 msgid "Stripe Account"
-msgstr "Cont"
+msgstr ""
 
 msgctxt "field:party.party.reception_direct_debit,stripe_customer:"
 msgid "Stripe Customer"
 msgstr ""
 
 msgctxt ""
 "field:party.party.reception_direct_debit,stripe_customer_payment_method:"
```

### Comparing `trytond_account_payment_stripe-7.0.3/locale/ru.po` & `trytond_account_payment_stripe-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/sl.po` & `trytond_account_payment_stripe-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/tr.po` & `trytond_account_payment_stripe-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/locale/uk.po` & `trytond_account_payment_stripe-7.2.0/locale/ro.po`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 msgctxt "field:account.payment,stripe_token:"
 msgid "Stripe Token"
 msgstr ""
 
 msgctxt "field:account.payment.journal,stripe_account:"
 msgid "Account"
-msgstr ""
+msgstr "Cont"
 
 msgctxt "field:account.payment.stripe.account,last_event:"
 msgid "Last Event"
 msgstr ""
 
 msgctxt "field:account.payment.stripe.account,name:"
 msgid "Name"
@@ -140,19 +140,19 @@
 
 msgctxt "field:account.payment.stripe.customer,identical_customers:"
 msgid "Identical Customers"
 msgstr ""
 
 msgctxt "field:account.payment.stripe.customer,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parte"
 
 msgctxt "field:account.payment.stripe.customer,stripe_account:"
 msgid "Account"
-msgstr ""
+msgstr "Cont"
 
 msgctxt "field:account.payment.stripe.customer,stripe_checkout_id:"
 msgid "Stripe Checkout ID"
 msgstr ""
 
 msgctxt "field:account.payment.stripe.customer,stripe_checkout_needed:"
 msgid "Stripe Checkout Needed"
@@ -204,15 +204,15 @@
 
 msgctxt "field:account.payment.stripe.customer.source.detach.ask,source:"
 msgid "Source"
 msgstr ""
 
 msgctxt "field:account.payment.stripe.refund,amount:"
 msgid "Amount"
-msgstr ""
+msgstr "Suma"
 
 msgctxt "field:account.payment.stripe.refund,approved_by:"
 msgid "Approved by"
 msgstr ""
 
 msgctxt "field:account.payment.stripe.refund,company:"
 msgid "Company"
@@ -262,17 +262,18 @@
 msgid "Submitted by"
 msgstr ""
 
 msgctxt "field:party.party,stripe_customers:"
 msgid "Stripe Customers"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:party.party.reception_direct_debit,stripe_account:"
 msgid "Stripe Account"
-msgstr ""
+msgstr "Cont"
 
 msgctxt "field:party.party.reception_direct_debit,stripe_customer:"
 msgid "Stripe Customer"
 msgstr ""
 
 msgctxt ""
 "field:party.party.reception_direct_debit,stripe_customer_payment_method:"
@@ -363,39 +364,39 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_refund_form_domain_all"
 msgid "All"
 msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_refund_form_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Ciorna"
 
 msgctxt "model:ir.action.act_window.domain,name:act_refund_form_domain_failed"
 msgid "Failed"
-msgstr ""
+msgstr "Esuat"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_refund_form_domain_processing"
 msgid "Processing"
-msgstr ""
+msgstr "In Curs de Procesare"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_refund_form_domain_suceeded"
 msgid "Succeeded"
-msgstr ""
+msgstr "Reusit"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_refund_form_domain_to_approve"
 msgid "To Approve"
-msgstr ""
+msgstr "De Aprobat"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_refund_form_domain_to_process"
 msgid "To Process"
-msgstr ""
+msgstr "De Procesat"
 
 msgctxt "model:ir.message,text:msg_customer_fingerprint_unique"
 msgid "The fingerprint must be unique by customer."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_no_stripe_token"
 msgid ""
@@ -406,18 +407,20 @@
 msgid "To pay \"%(payment)s\", you cannot use a stripe journal \"%(journal)s\"."
 msgstr ""
 
 msgctxt "model:ir.model.button,confirm:account_new_identifier_button"
 msgid ""
 "This action will make the previous URL unusable. Do you want to continue?"
 msgstr ""
+"Această acțiune va face ca adresa URL anterioară să fie inutilizabilă. "
+"Doriți să continuați?"
 
 msgctxt "model:ir.model.button,string:account_new_identifier_button"
 msgid "New URL"
-msgstr ""
+msgstr "URL Nou"
 
 msgctxt "model:ir.model.button,string:customer_find_identical_button"
 msgid "Find Identical"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:customer_source_detach_button"
 msgid "Detach Source"
@@ -433,23 +436,23 @@
 
 msgctxt "model:ir.model.button,string:payment_stripe_checkout_button"
 msgid "Stripe Checkout"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:refund_approve_button"
 msgid "Approve"
-msgstr ""
+msgstr "Aproba"
 
 msgctxt "model:ir.model.button,string:refund_draft_button"
 msgid "Draft"
-msgstr ""
+msgstr "Ciorna"
 
 msgctxt "model:ir.model.button,string:refund_submit_button"
 msgid "Submit"
-msgstr ""
+msgstr "Trimite"
 
 msgctxt "model:ir.ui.menu,name:menu_account_form"
 msgid "Stripe Accounts"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_customer_form"
 msgid "Stripe Customers"
@@ -581,23 +584,23 @@
 
 msgctxt "view:account.payment:"
 msgid "Chargeable:"
 msgstr ""
 
 msgctxt "view:account.payment:"
 msgid "Customer:"
-msgstr ""
+msgstr "Client:"
 
 msgctxt "view:account.payment:"
 msgid "Payment Intent:"
 msgstr ""
 
 msgctxt "view:account.payment:"
 msgid "Payment Method:"
-msgstr ""
+msgstr "Metoda de Plata:"
 
 msgctxt "view:account.payment:"
 msgid "Source:"
 msgstr ""
 
 msgctxt "view:account.payment:"
 msgid "Stripe"
@@ -605,19 +608,19 @@
 
 msgctxt "view:account.payment:"
 msgid "Token:"
 msgstr ""
 
 msgctxt "view:party.party.reception_direct_debit:"
 msgid "Customer:"
-msgstr ""
+msgstr "Client:"
 
 msgctxt "view:party.party.reception_direct_debit:"
 msgid "Payment Method:"
-msgstr ""
+msgstr "Metoda de Plata:"
 
 msgctxt "view:party.party.reception_direct_debit:"
 msgid "Source:"
 msgstr ""
 
 msgctxt ""
 "wizard_button:account.payment.stripe.customer.source.detach,ask,detach:"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_account_payment_stripe-7.0.3/locale/zh_CN.po` & `trytond_account_payment_stripe-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/message.xml` & `trytond_account_payment_stripe-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/party.py` & `trytond_account_payment_stripe-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/party.xml` & `trytond_account_payment_stripe-7.2.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/payment.py` & `trytond_account_payment_stripe-7.2.0/payment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime as dt
 import logging
 import urllib.parse
 import uuid
 from decimal import Decimal
-from email.header import Header
 from itertools import groupby
 from operator import attrgetter
 
 import stripe
 from sql import Literal
 
 from trytond.cache import Cache
@@ -23,15 +22,15 @@
 from trytond.modules.company.model import (
     employee_field, reset_employee, set_employee)
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval, TimeDelta
 from trytond.report import Report, get_email
 from trytond.rpc import RPC
-from trytond.sendmail import sendmail_transactional
+from trytond.sendmail import send_message_transactional
 from trytond.tools import sql_pairing
 from trytond.tools.email_ import set_from_header
 from trytond.transaction import Transaction
 from trytond.url import http_host
 from trytond.wizard import (
     Button, StateAction, StateTransition, StateView, Wizard)
 
@@ -386,17 +385,17 @@
         if not emails:
             logger.warning("Could not send checkout email for %d", self.id)
             return
         languages = [self.party.lang or Language.get()]
         msg, title = get_email(
             'account.payment.stripe.email_checkout', self, languages)
         set_from_header(msg, from_cfg, from_ or from_cfg)
-        msg['To'] = ','.join(emails)
-        msg['Subject'] = Header(title, 'utf-8')
-        sendmail_transactional(from_cfg, emails, msg)
+        msg['To'] = emails
+        msg['Subject'] = title
+        send_message_transactional(msg)
 
     def _emails_checkout(self):
         emails = []
         if self.party.email:
             emails.append(self.party.email)
         return emails
```

### Comparing `trytond_account_payment_stripe-7.0.3/payment.xml` & `trytond_account_payment_stripe-7.2.0/payment.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_account_payment_stripe-7.0.3/payment.xml` & `trytond_account_payment_stripe-7.2.0/payment.xml`

```diff
@@ -86,27 +86,27 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_refund_form"/>
     </record>
     <menuitem parent="account_payment.menu_payments" sequence="20" action="act_refund_form" id="menu_refund_form"/>
     <record model="ir.model.button" id="refund_draft_button">
+      <field name="model">account.payment.stripe.refund</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'account.payment.stripe.refund')]"/>
     </record>
     <record model="ir.model.button" id="refund_submit_button">
+      <field name="model">account.payment.stripe.refund</field>
       <field name="name">submit</field>
       <field name="string">Submit</field>
-      <field name="model" search="[('model', '=', 'account.payment.stripe.refund')]"/>
     </record>
     <record model="ir.model.button" id="refund_approve_button">
+      <field name="model">account.payment.stripe.refund</field>
       <field name="name">approve</field>
       <field name="string">Approve</field>
-      <field name="model" search="[('model', '=', 'account.payment.stripe.refund')]"/>
     </record>
     <record model="ir.model.button-res.group" id="refund_approve_button_group_payment_approval">
       <field name="button" ref="refund_approve_button"/>
       <field name="group" ref="account_payment.group_payment_approval"/>
     </record>
     <record model="ir.ui.view" id="account_view_form">
       <field name="model">account.payment.stripe.account</field>
@@ -115,18 +115,18 @@
     </record>
     <record model="ir.ui.view" id="account_view_list">
       <field name="model">account.payment.stripe.account</field>
       <field name="type">tree</field>
       <field name="name">account_list</field>
     </record>
     <record model="ir.model.button" id="account_new_identifier_button">
+      <field name="model">account.payment.stripe.account</field>
       <field name="name">new_identifier</field>
       <field name="string">New URL</field>
       <field name="confirm">This action will make the previous URL unusable. Do you want to continue?</field>
-      <field name="model" search="[('model', '=', 'account.payment.stripe.account')]"/>
     </record>
     <record model="ir.action.act_window" id="act_account_form">
       <field name="name">Stripe Accounts</field>
       <field name="res_model">account.payment.stripe.account</field>
     </record>
     <record model="ir.action.act_window.view" id="act_account_form_view1">
       <field name="sequence" eval="10"/>
@@ -136,60 +136,62 @@
     <record model="ir.action.act_window.view" id="act_account_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="account_view_form"/>
       <field name="act_window" ref="act_account_form"/>
     </record>
     <menuitem parent="account_payment.menu_payment_configuration" action="act_account_form" sequence="20" id="menu_account_form"/>
     <record model="ir.model.access" id="access_account">
-      <field name="model" search="[('model', '=', 'account.payment.stripe.account')]"/>
+      <field name="model">account.payment.stripe.account</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_account_account_admin">
-      <field name="model" search="[('model', '=', 'account.payment.stripe.account')]"/>
+      <field name="model">account.payment.stripe.account</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_account_payment">
-      <field name="model" search="[('model', '=', 'account.payment.stripe.account')]"/>
+      <field name="model">account.payment.stripe.account</field>
       <field name="group" ref="account_payment.group_payment"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_account_secret_key">
-      <field name="field" search="[('name', '=', 'secret_key'), ('model.model', '=', 'account.payment.stripe.account')]"/>
+      <field name="model">account.payment.stripe.account</field>
+      <field name="field">secret_key</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_account_secret_key_account_admin">
-      <field name="field" search="[('name', '=', 'secret_key'), ('model.model', '=', 'account.payment.stripe.account')]"/>
+      <field name="model">account.payment.stripe.account</field>
+      <field name="field">secret_key</field>
       <field name="group" ref="account.group_account_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="payment_stripe_checkout_button">
+      <field name="model">account.payment</field>
       <field name="name">stripe_checkout</field>
       <field name="string">Stripe Checkout</field>
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
     </record>
     <record model="ir.model.button" id="payment_stripe_capture_button">
+      <field name="model">account.payment</field>
       <field name="name">stripe_do_capture</field>
       <field name="string">Stripe Capture</field>
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
     </record>
     <record model="ir.ui.view" id="customer_view_form">
       <field name="model">account.payment.stripe.customer</field>
       <field name="type">form</field>
       <field name="name">customer_form</field>
     </record>
     <record model="ir.ui.view" id="customer_view_list">
@@ -209,51 +211,51 @@
     <record model="ir.action.act_window.view" id="act_customer_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="customer_view_form"/>
       <field name="act_window" ref="act_customer_form"/>
     </record>
     <menuitem parent="account_payment.menu_payments" action="act_customer_form" sequence="50" id="menu_customer_form"/>
     <record model="ir.model.access" id="access_customer">
-      <field name="model" search="[('model', '=', 'account.payment.stripe.customer')]"/>
+      <field name="model">account.payment.stripe.customer</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_customer_payment">
-      <field name="model" search="[('model', '=', 'account.payment.stripe.customer')]"/>
+      <field name="model">account.payment.stripe.customer</field>
       <field name="group" ref="account_payment.group_payment"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="customer_stripe_checkout_button">
+      <field name="model">account.payment.stripe.customer</field>
       <field name="name">stripe_checkout</field>
       <field name="string">Add Card</field>
-      <field name="model" search="[('model', '=', 'account.payment.stripe.customer')]"/>
     </record>
     <record model="ir.model.button" id="customer_source_detach_button">
+      <field name="model">account.payment.stripe.customer</field>
       <field name="name">detach_source</field>
       <field name="string">Detach Source</field>
-      <field name="model" search="[('model', '=', 'account.payment.stripe.customer')]"/>
     </record>
     <record model="ir.model.button" id="customer_find_identical_button">
+      <field name="model">account.payment.stripe.customer</field>
       <field name="name">find_identical</field>
       <field name="string">Find Identical</field>
-      <field name="model" search="[('model', '=', 'account.payment.stripe.customer')]"/>
     </record>
     <record model="ir.action.wizard" id="wizard_checkout">
       <field name="name">Stripe Checkout</field>
       <field name="wiz_name">account.payment.stripe.checkout</field>
       <field name="model" eval="None"/>
     </record>
     <record model="ir.action.report" id="report_checkout">
       <field name="name">Stripe Checkout</field>
-      <field name="model"/>
+      <field name="model" eval="None"/>
       <field name="report_name">account.payment.stripe.checkout</field>
       <field name="report">account_payment_stripe/checkout.html</field>
       <field name="template_extension">html</field>
     </record>
     <record model="ir.action.report" id="report_email_checkout">
       <field name="name">Checkout</field>
       <field name="model">account.payment</field>
```

### Comparing `trytond_account_payment_stripe-7.0.3/routes.py` & `trytond_account_payment_stripe-7.2.0/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/setup.py` & `trytond_account_payment_stripe-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe.rst` & `trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ===============================
 Account Payment Stripe Scenario
 ===============================
 
 Imports::
 
-    >>> import os
     >>> import datetime as dt
+    >>> import os
     >>> import time
     >>> from decimal import Decimal
+
     >>> import stripe
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, create_fiscalyear
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
 
     >>> today = dt.date.today()
 
     >>> FETCH_SLEEP, MAX_SLEEP = 1, 100
 
 Activate modules::
 
@@ -215,16 +215,16 @@
 Make payment with customer::
 
     >>> payment, = payment.duplicate()
     >>> payment.stripe_customer = stripe_customer
     >>> payment.save()
     >>> _, source = Payment.get_stripe_customer_sources(payment.id, config.context)
     >>> source_id, source_name = source
-    >>> source_name == 'Visa ****1881 12/%s' % (today.year + 1)
-    True
+    >>> source_name
+    'Visa ****1881 12/...'
     >>> payment.stripe_customer_source = source_id
     >>> payment.click('submit')
     >>> payment.state
     'submitted'
     >>> process_payment = payment.click('process_wizard')
     >>> payment.state
     'processing'
```

### Comparing `trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe_dispute.rst` & `trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe_dispute.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 =======================================
 Account Payment Stripe Dispute Scenario
 =======================================
 
 Imports::
 
-    >>> import os
     >>> import datetime as dt
+    >>> import os
     >>> import time
     >>> from decimal import Decimal
+
     >>> import stripe
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, create_fiscalyear
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
 
     >>> today = dt.date.today()
 
     >>> FETCH_SLEEP, MAX_SLEEP = 1, 100
 
 Activate modules::
```

### Comparing `trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe_identical.rst` & `trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe_identical.rst`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,20 @@
 Account Payment Stripe Identical
 ================================
 
 Imports::
 
     >>> import datetime as dt
     >>> import os
-    >>> import time
-    >>> from decimal import Decimal
 
     >>> import stripe
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_payment_stripe')
 
@@ -100,12 +97,10 @@
     ...     [stripe_customer2.id], {'stripe_token': token.id}, config.context)
 
 Run cron::
 
     >>> cron_customer_create.click('run_once')
 
     >>> stripe_customer2.reload()
-    >>> stripe_customer2.identical_customers == [stripe_customer1]
-    True
+    >>> assertEqual(stripe_customer2.identical_customers, [stripe_customer1])
     >>> stripe_customer1.reload()
-    >>> stripe_customer1.identical_customers == [stripe_customer2]
-    True
+    >>> assertEqual(stripe_customer1.identical_customers, [stripe_customer2])
```

### Comparing `trytond_account_payment_stripe-7.0.3/tests/scenario_account_payment_stripe_intent.rst` & `trytond_account_payment_stripe-7.2.0/tests/scenario_account_payment_stripe_intent.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ======================================
 Account Payment Stripe Intent Scenario
 ======================================
 
 Imports::
 
-    >>> import os
     >>> import datetime as dt
+    >>> import os
     >>> import time
     >>> from decimal import Decimal
+
     >>> import stripe
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, create_fiscalyear
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
 
     >>> today = dt.date.today()
 
     >>> FETCH_SLEEP, MAX_SLEEP = 1, 100
 
 Activate modules::
```

### Comparing `trytond_account_payment_stripe-7.0.3/tox.ini` & `trytond_account_payment_stripe-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/PKG-INFO` & `trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_stripe
-Version: 7.0.3
+Version: 7.2.0
 Summary: Tryton module for Stripe payment
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
@@ -49,20 +49,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: stripe>=2.32.0
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_payment<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_payment<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Account Payment Stripe Module
 #############################
 
 The account_payment_stripe module allows to receive payment from `Stripe`_.
 It uses `Stripe.js and Stripe Elements`_ in a checkout form to handle `Setup
 Intent`_ and `Payment Intent`_ by card.
```

### Comparing `trytond_account_payment_stripe-7.0.3/trytond_account_payment_stripe.egg-info/SOURCES.txt` & `trytond_account_payment_stripe-7.2.0/trytond_account_payment_stripe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/view/account_form.xml` & `trytond_account_payment_stripe-7.2.0/view/account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/view/customer_form.xml` & `trytond_account_payment_stripe-7.2.0/view/customer_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/view/party_reception_direct_debit_form.xml` & `trytond_account_payment_stripe-7.2.0/view/party_reception_direct_debit_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/view/payment_form.xml` & `trytond_account_payment_stripe-7.2.0/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_stripe-7.0.3/view/refund_form.xml` & `trytond_account_payment_stripe-7.2.0/view/refund_form.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_account_payment_stripe-7.0.3/view/refund_form.xml` & `trytond_account_payment_stripe-7.2.0/view/refund_form.xml`

```diff
@@ -4,17 +4,18 @@
 <form>
   <label name="payment"/>
   <field name="payment" colspan="3"/>
   <label name="amount"/>
   <field name="amount"/>
   <label name="reason"/>
   <field name="reason"/>
+  <label name="stripe_refund_id"/>
+  <field name="stripe_refund_id" colspan="3"/>
   <label name="stripe_error_message"/>
-  <field name="stripe_error_message"/>
-  <newline/>
+  <field name="stripe_error_message" colspan="3"/>
   <label name="stripe_error_code"/>
   <field name="stripe_error_code"/>
   <label name="stripe_error_param"/>
   <field name="stripe_error_param"/>
   <label name="submitted_by"/>
   <field name="submitted_by"/>
   <label name="approved_by"/>
```

