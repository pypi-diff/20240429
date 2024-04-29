# Comparing `tmp/trytond_account_payment_clearing-7.0.2.tar.gz` & `tmp/trytond_account_payment_clearing-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_payment_clearing-7.0.2.tar", last modified: Wed Apr 17 10:45:14 2024, max compression
+gzip compressed data, was "trytond_account_payment_clearing-7.2.0.tar", last modified: Mon Apr 29 15:34:54 2024, max compression
```

## Comparing `trytond_account_payment_clearing-7.0.2.tar` & `trytond_account_payment_clearing-7.2.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:14.984990 trytond_account_payment_clearing-7.0.2/
--rw-r--r--   0 ced       (1000) ced       (1000)     3005 2024-04-17 10:45:12.000000 trytond_account_payment_clearing-7.0.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-17 10:45:11.000000 trytond_account_payment_clearing-7.0.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3049 2024-04-17 10:45:14.984990 trytond_account_payment_clearing-7.0.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      992 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1794 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:14.981656 trytond_account_payment_clearing-7.0.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2803 2024-03-03 16:24:20.000000 trytond_account_payment_clearing-7.0.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1331 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:14.981656 trytond_account_payment_clearing-7.0.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2638 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2669 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2636 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2248 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2424 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2557 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2654 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2049 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2248 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2456 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2161 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2564 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2140 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2297 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2033 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2125 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16668 2024-04-12 22:39:25.000000 trytond_account_payment_clearing-7.0.2/payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2402 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:45:14.984990 trytond_account_payment_clearing-7.0.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4889 2024-03-03 16:24:03.000000 trytond_account_payment_clearing-7.0.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8612 2024-02-05 16:24:27.000000 trytond_account_payment_clearing-7.0.2/statement.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:14.981656 trytond_account_payment_clearing-7.0.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3317 2024-02-05 16:24:27.000000 trytond_account_payment_clearing-7.0.2/tests/scenario_account_negative_payment_clearing.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    14076 2024-02-05 16:24:27.000000 trytond_account_payment_clearing-7.0.2/tests/scenario_account_payment_clearing.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5337 2024-02-05 16:24:27.000000 trytond_account_payment_clearing-7.0.2/tests/scenario_account_payment_clearing_invoice_amount_to_pay.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-02-05 16:24:27.000000 trytond_account_payment_clearing-7.0.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:14.984990 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3049 2024-04-17 10:45:14.000000 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2127 2024-04-17 10:45:14.000000 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:45:14.000000 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       86 2024-04-17 10:45:14.000000 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:36.000000 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2024-04-17 10:45:14.000000 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:45:14.000000 trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:45:14.984990 trytond_account_payment_clearing-7.0.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/view/payment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/view/payment_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/view/payment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-10-30 17:06:38.000000 trytond_account_payment_clearing-7.0.2/view/succeed_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:54.884761 trytond_account_payment_clearing-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2904 2024-04-29 15:15:13.000000 trytond_account_payment_clearing-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:15:13.000000 trytond_account_payment_clearing-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_payment_clearing-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3049 2024-04-29 15:34:54.884761 trytond_account_payment_clearing-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-02-04 18:51:26.000000 trytond_account_payment_clearing-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      992 2024-03-08 19:04:12.000000 trytond_account_payment_clearing-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1794 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-7.2.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:54.881428 trytond_account_payment_clearing-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3087 2024-04-27 16:30:39.000000 trytond_account_payment_clearing-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1331 2024-02-04 18:51:26.000000 trytond_account_payment_clearing-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-02-04 18:51:26.000000 trytond_account_payment_clearing-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-02-04 18:51:26.000000 trytond_account_payment_clearing-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:57.000000 trytond_account_payment_clearing-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:54.881428 trytond_account_payment_clearing-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2638 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2669 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2636 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2248 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2424 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2557 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2654 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2049 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2248 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2456 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2161 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2564 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2140 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2348 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2130 2024-04-29 13:17:17.000000 trytond_account_payment_clearing-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2297 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2033 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2125 2024-04-27 16:43:21.000000 trytond_account_payment_clearing-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16668 2024-04-27 16:30:39.000000 trytond_account_payment_clearing-7.2.0/payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2379 2024-04-27 16:30:39.000000 trytond_account_payment_clearing-7.2.0/payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:34:54.884761 trytond_account_payment_clearing-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4889 2024-04-27 16:30:39.000000 trytond_account_payment_clearing-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8721 2024-04-27 16:30:39.000000 trytond_account_payment_clearing-7.2.0/statement.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:54.884761 trytond_account_payment_clearing-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3306 2024-04-22 12:14:36.000000 trytond_account_payment_clearing-7.2.0/tests/scenario_account_negative_payment_clearing.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    14093 2024-04-22 12:14:36.000000 trytond_account_payment_clearing-7.2.0/tests/scenario_account_payment_clearing.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5253 2024-04-22 12:14:36.000000 trytond_account_payment_clearing-7.2.0/tests/scenario_account_payment_clearing_invoice_amount_to_pay.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:57.000000 trytond_account_payment_clearing-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      156 2024-04-29 15:15:09.000000 trytond_account_payment_clearing-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:54.884761 trytond_account_payment_clearing-7.2.0/trytond_account_payment_clearing.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3049 2024-04-29 15:34:54.000000 trytond_account_payment_clearing-7.2.0/trytond_account_payment_clearing.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2127 2024-04-29 15:34:54.000000 trytond_account_payment_clearing-7.2.0/trytond_account_payment_clearing.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:34:54.000000 trytond_account_payment_clearing-7.2.0/trytond_account_payment_clearing.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       86 2024-04-29 15:34:54.000000 trytond_account_payment_clearing-7.2.0/trytond_account_payment_clearing.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_account_payment_clearing-7.2.0/trytond_account_payment_clearing.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      215 2024-04-29 15:34:54.000000 trytond_account_payment_clearing-7.2.0/trytond_account_payment_clearing.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:34:54.000000 trytond_account_payment_clearing-7.2.0/trytond_account_payment_clearing.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:54.884761 trytond_account_payment_clearing-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-01-16 14:00:20.000000 trytond_account_payment_clearing-7.2.0/view/payment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-04-15 07:12:15.000000 trytond_account_payment_clearing-7.2.0/view/payment_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2024-02-04 18:51:26.000000 trytond_account_payment_clearing-7.2.0/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-02-04 18:51:26.000000 trytond_account_payment_clearing-7.2.0/view/payment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:20.000000 trytond_account_payment_clearing-7.2.0/view/succeed_start_form.xml
```

### Comparing `trytond_account_payment_clearing-7.0.2/CHANGELOG` & `trytond_account_payment_clearing-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 
-Version 7.0.2 - 2024-04-17
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2024-01-15
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_payment_clearing-7.0.2/COPYRIGHT` & `trytond_account_payment_clearing-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/LICENSE` & `trytond_account_payment_clearing-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/PKG-INFO` & `trytond_account_payment_clearing-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_clearing
-Version: 7.0.2
+Version: 7.2.0
 Summary: Tryton module for payment clearing
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-account-payment-clearing
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,22 +48,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_payment<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_payment<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_statement<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_statement_rule<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_statement<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_statement_rule<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
 
 ###############################
 Account Payment Clearing Module
 ###############################
 
 The *Account Payment Clearing Module* allows to generate account move when a
 payment is succeeded between the receivable/payable account to a clearing
```

### Comparing `trytond_account_payment_clearing-7.0.2/__init__.py` & `trytond_account_payment_clearing-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/account.py` & `trytond_account_payment_clearing-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/doc/conf.py` & `trytond_account_payment_clearing-7.2.0/doc/conf.py`

 * *Files 4% similar despite different names*

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

### Comparing `trytond_account_payment_clearing-7.0.2/doc/design.rst` & `trytond_account_payment_clearing-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/bg.po` & `trytond_account_payment_clearing-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/ca.po` & `trytond_account_payment_clearing-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/cs.po` & `trytond_account_payment_clearing-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/de.po` & `trytond_account_payment_clearing-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/es.po` & `trytond_account_payment_clearing-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/es_419.po` & `trytond_account_payment_clearing-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/et.po` & `trytond_account_payment_clearing-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/fa.po` & `trytond_account_payment_clearing-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/fi.po` & `trytond_account_payment_clearing-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/fr.po` & `trytond_account_payment_clearing-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/hu.po` & `trytond_account_payment_clearing-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/id.po` & `trytond_account_payment_clearing-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/it.po` & `trytond_account_payment_clearing-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/lo.po` & `trytond_account_payment_clearing-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/lt.po` & `trytond_account_payment_clearing-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/nl.po` & `trytond_account_payment_clearing-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/pl.po` & `trytond_account_payment_clearing-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/pt.po` & `trytond_account_payment_clearing-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/ro.po` & `trytond_account_payment_clearing-7.2.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.payment,account:"
 msgid "Account"
 msgstr "Cont"
 
+#, fuzzy
 msgctxt "field:account.payment,clearing_move:"
 msgid "Clearing Move"
-msgstr ""
+msgstr "Ștergerea Mișcării"
 
 msgctxt "field:account.payment,clearing_reconciled:"
 msgid "Clearing Reconciled"
 msgstr ""
 
 msgctxt "field:account.payment,statement_lines:"
 msgid "Statement Lines"
@@ -46,17 +47,18 @@
 msgid "Define the account to use for clearing move."
 msgstr ""
 
 msgctxt "help:account.payment,clearing_reconciled:"
 msgid "Checked if clearing line is reconciled."
 msgstr ""
 
+#, fuzzy
 msgctxt "help:account.payment.group,clearing_reconciled:"
 msgid "All payments in the group are reconciled."
-msgstr ""
+msgstr "Toate plățile din grup sunt reconciliate."
 
 msgctxt "help:account.payment.journal,clearing_posting_delay:"
 msgid ""
 "Post automatically the clearing moves after the delay.\n"
 "Leave empty for no posting."
 msgstr ""
 
@@ -78,12 +80,12 @@
 
 msgctxt "view:account.payment.journal:"
 msgid "Clearing"
 msgstr ""
 
 msgctxt "wizard_button:account.payment.succeed,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Anulare"
 
 msgctxt "wizard_button:account.payment.succeed,start,succeed:"
 msgid "Succeed"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_account_payment_clearing-7.0.2/locale/ru.po` & `trytond_account_payment_clearing-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/sl.po` & `trytond_account_payment_clearing-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/tr.po` & `trytond_account_payment_clearing-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/uk.po` & `trytond_account_payment_clearing-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/locale/zh_CN.po` & `trytond_account_payment_clearing-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/payment.py` & `trytond_account_payment_clearing-7.2.0/payment.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/payment.xml` & `trytond_account_payment_clearing-7.2.0/payment.xml`

 * *Files 5% similar despite different names*

#### Comparing `trytond_account_payment_clearing-7.0.2/payment.xml` & `trytond_account_payment_clearing-7.2.0/payment.xml`

```diff
@@ -30,17 +30,17 @@
     </record>
     <record model="ir.ui.view" id="succeed_start_view_form">
       <field name="model">account.payment.succeed.start</field>
       <field name="type">form</field>
       <field name="name">succeed_start_form</field>
     </record>
     <record model="ir.model.button" id="payment_succeed_wizard_button">
+      <field name="model">account.payment</field>
       <field name="name">succeed_wizard</field>
       <field name="string">Succeed</field>
-      <field name="model" search="[('model', '=', 'account.payment')]"/>
     </record>
     <record model="ir.cron" id="cron_post_clearing_moves">
       <field name="method">account.payment.journal|cron_post_clearing_moves</field>
       <field name="interval_number" eval="1"/>
       <field name="interval_type">days</field>
     </record>
   </data>
```

### Comparing `trytond_account_payment_clearing-7.0.2/setup.py` & `trytond_account_payment_clearing-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/statement.py` & `trytond_account_payment_clearing-7.2.0/statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,17 @@
             cls.related_to.domain.get('account.payment', []),
             If(Eval('statement_state') == 'draft',
                 ('clearing_reconciled', '!=', True),
                 ()),
             ]
         cls.related_to.domain['account.payment.group'] = [
             ('company', '=', Eval('company', -1)),
-            ('currency', '=', Eval('currency', -1)),
+            If(Eval('second_currency'),
+                ('currency', '=', Eval('second_currency', -1)),
+                ('currency', '=', Eval('currency', -1))),
             If(Eval('statement_state') == 'draft',
                 ('clearing_reconciled', '!=', True),
                 ()),
             ]
 
     @classmethod
     def __register__(cls, module):
```

### Comparing `trytond_account_payment_clearing-7.0.2/tests/scenario_account_negative_payment_clearing.rst` & `trytond_account_payment_clearing-7.2.0/tests/scenario_account_negative_payment_clearing.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 Negative Payment Clearing Scenario
 ==================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(['account_payment_clearing'])
 
 Create company::
```

### Comparing `trytond_account_payment_clearing-7.0.2/tests/scenario_account_payment_clearing.rst` & `trytond_account_payment_clearing-7.2.0/tests/scenario_account_payment_clearing.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 Payment Clearing Scenario
 =========================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+
     >>> today = dt.date.today()
     >>> yesterday = today - dt.timedelta(days=1)
     >>> first = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules(['account_payment_clearing', 'account_statement'])
@@ -108,16 +109,15 @@
 Succeed payment::
 
     >>> succeed = payment.click('succeed_wizard')
     >>> succeed.form.date = first
     >>> succeed.execute('succeed')
     >>> payment.state
     'succeeded'
-    >>> payment.clearing_move.date == first
-    True
+    >>> assertEqual(payment.clearing_move.date, first)
     >>> payment.clearing_move.state
     'draft'
     >>> bool(payment.clearing_reconciled)
     False
     >>> payable.reload()
     >>> payable.balance
     Decimal('-20.00')
@@ -248,18 +248,16 @@
     ... )
 
 Create a line for the payment::
 
     >>> line = statement.lines.new(date=today)
     >>> line.amount = Decimal('-50.00')
     >>> line.related_to = payment
-    >>> line.party == supplier
-    True
-    >>> line.account == bank_clearing
-    True
+    >>> assertEqual(line.party, supplier)
+    >>> assertEqual(line.account, bank_clearing)
 
 Remove the party must remove payment::
 
     >>> line.party = None
     >>> line.related_to
 
     >>> line.related_to = payment
@@ -305,16 +303,15 @@
     >>> statement = Statement(name='test',
     ...     journal=statement_journal,
     ...     start_balance=Decimal('-50.00'),
     ...     end_balance=Decimal('0.00'),
     ...     )
     >>> line = statement.lines.new(date=today)
     >>> line.related_to = payment.group
-    >>> line.account == bank_clearing
-    True
+    >>> assertEqual(line.account, bank_clearing)
     >>> line.amount = Decimal('50.00')
 
     >>> statement.click('validate_statement')
     >>> statement.state
     'validated'
 
 Payment must be failed::
@@ -449,18 +446,16 @@
     >>> statement = Statement(name='test',
     ...     journal=statement_journal,
     ...     start_balance=Decimal('0.00'),
     ...     end_balance=Decimal('-50.00'))
     >>> line = statement.lines.new(date=yesterday)
     >>> line.amount = Decimal('-50.00')
     >>> line.related_to = payment
-    >>> line.party == supplier
-    True
-    >>> line.account == bank_clearing
-    True
+    >>> assertEqual(line.party, supplier)
+    >>> assertEqual(line.account, bank_clearing)
     >>> statement.save()
 
 Validate statement and check the payment is confirmed::
 
     >>> statement.click('validate_statement')
     >>> statement.state
     'validated'
@@ -473,9 +468,8 @@
     >>> payment.state
     'succeeded'
     >>> bool(payment.clearing_reconciled)
     True
     >>> debit_line, = [l for l in payment.clearing_move.lines if l.debit > 0]
     >>> debit_line.debit
     Decimal('50.00')
-    >>> debit_line.date == yesterday
-    True
+    >>> assertEqual(debit_line.date, yesterday)
```

### Comparing `trytond_account_payment_clearing-7.0.2/tests/scenario_account_payment_clearing_invoice_amount_to_pay.rst` & `trytond_account_payment_clearing-7.2.0/tests/scenario_account_payment_clearing_invoice_amount_to_pay.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 ======================================
 Payment Clearing Invoice Amount to Pay
 ======================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules(
     ...     ['account_payment_clearing', 'account_invoice'])
 
 Create company::
```

### Comparing `trytond_account_payment_clearing-7.0.2/tox.ini` & `trytond_account_payment_clearing-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/PKG-INFO` & `trytond_account_payment_clearing-7.2.0/trytond_account_payment_clearing.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_payment_clearing
-Version: 7.0.2
+Version: 7.2.0
 Summary: Tryton module for payment clearing
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-account-payment-clearing
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,22 +48,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_payment<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_payment<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_statement<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_statement_rule<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_statement<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_statement_rule<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
 
 ###############################
 Account Payment Clearing Module
 ###############################
 
 The *Account Payment Clearing Module* allows to generate account move when a
 payment is succeeded between the receivable/payable account to a clearing
```

### Comparing `trytond_account_payment_clearing-7.0.2/trytond_account_payment_clearing.egg-info/SOURCES.txt` & `trytond_account_payment_clearing-7.2.0/trytond_account_payment_clearing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/view/payment_form.xml` & `trytond_account_payment_clearing-7.2.0/view/payment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_payment_clearing-7.0.2/view/payment_journal_form.xml` & `trytond_account_payment_clearing-7.2.0/view/payment_journal_form.xml`

 * *Files identical despite different names*

