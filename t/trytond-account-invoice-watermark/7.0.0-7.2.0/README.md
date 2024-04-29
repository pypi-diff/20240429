# Comparing `tmp/trytond_account_invoice_watermark-7.0.0.tar.gz` & `tmp/trytond_account_invoice_watermark-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice_watermark-7.0.0.tar", last modified: Mon Oct 30 17:21:41 2023, max compression
+gzip compressed data, was "trytond_account_invoice_watermark-7.2.0.tar", last modified: Mon Apr 29 15:34:21 2024, max compression
```

## Comparing `trytond_account_invoice_watermark-7.0.0.tar` & `trytond_account_invoice_watermark-7.2.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:41.103100 trytond_account_invoice_watermark-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      231 2023-10-22 17:22:52.000000 trytond_account_invoice_watermark-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-10-30 17:02:21.000000 trytond_account_invoice_watermark-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:02:21.000000 trytond_account_invoice_watermark-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2750 2023-10-30 17:21:41.103100 trytond_account_invoice_watermark-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2222 2023-10-07 15:40:36.000000 trytond_account_invoice_watermark-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1167 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:41.099766 trytond_account_invoice_watermark-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2826 2023-10-22 17:22:52.000000 trytond_account_invoice_watermark-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:52.000000 trytond_account_invoice_watermark-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      297 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.0.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    31593 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.0.0/invoice_watermark_draft.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    30602 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.0.0/invoice_watermark_paid.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:41.096433 trytond_account_invoice_watermark-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      479 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      479 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      485 2023-10-30 16:47:45.000000 trytond_account_invoice_watermark-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-28 12:11:20.000000 trytond_account_invoice_watermark-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:21:41.103100 trytond_account_invoice_watermark-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4769 2023-10-27 17:38:49.000000 trytond_account_invoice_watermark-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:41.099766 trytond_account_invoice_watermark-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2931 2023-08-13 15:26:13.000000 trytond_account_invoice_watermark-7.0.0/tests/scenario_account_invoice_watermark.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      708 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.0.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_invoice_watermark-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-10-30 17:02:18.000000 trytond_account_invoice_watermark-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:21:41.099766 trytond_account_invoice_watermark-7.0.0/trytond_account_invoice_watermark.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2750 2023-10-30 17:21:40.000000 trytond_account_invoice_watermark-7.0.0/trytond_account_invoice_watermark.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1740 2023-10-30 17:21:41.000000 trytond_account_invoice_watermark-7.0.0/trytond_account_invoice_watermark.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:21:40.000000 trytond_account_invoice_watermark-7.0.0/trytond_account_invoice_watermark.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-10-30 17:21:40.000000 trytond_account_invoice_watermark-7.0.0/trytond_account_invoice_watermark.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_account_invoice_watermark-7.0.0/trytond_account_invoice_watermark.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       87 2023-10-30 17:21:40.000000 trytond_account_invoice_watermark-7.0.0/trytond_account_invoice_watermark.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:21:40.000000 trytond_account_invoice_watermark-7.0.0/trytond_account_invoice_watermark.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:21.105645 trytond_account_invoice_watermark-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2024-04-29 15:14:53.000000 trytond_account_invoice_watermark-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:14:52.000000 trytond_account_invoice_watermark-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2741 2024-04-29 15:34:21.105645 trytond_account_invoice_watermark-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2222 2024-02-04 18:51:26.000000 trytond_account_invoice_watermark-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1167 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:21.102312 trytond_account_invoice_watermark-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3088 2024-04-27 16:30:39.000000 trytond_account_invoice_watermark-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:56.000000 trytond_account_invoice_watermark-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      297 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    31593 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.2.0/invoice_watermark_draft.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    30602 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.2.0/invoice_watermark_paid.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:21.105645 trytond_account_invoice_watermark-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      479 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      479 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      465 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      471 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-04-29 13:17:17.000000 trytond_account_invoice_watermark-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      485 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-27 16:43:21.000000 trytond_account_invoice_watermark-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:34:21.105645 trytond_account_invoice_watermark-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4760 2024-04-27 16:30:39.000000 trytond_account_invoice_watermark-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:21.105645 trytond_account_invoice_watermark-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2892 2024-04-22 12:14:36.000000 trytond_account_invoice_watermark-7.2.0/tests/scenario_account_invoice_watermark.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      708 2023-04-15 07:12:15.000000 trytond_account_invoice_watermark-7.2.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:56.000000 trytond_account_invoice_watermark-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:14:48.000000 trytond_account_invoice_watermark-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:21.105645 trytond_account_invoice_watermark-7.2.0/trytond_account_invoice_watermark.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2741 2024-04-29 15:34:20.000000 trytond_account_invoice_watermark-7.2.0/trytond_account_invoice_watermark.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1722 2024-04-29 15:34:21.000000 trytond_account_invoice_watermark-7.2.0/trytond_account_invoice_watermark.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:34:20.000000 trytond_account_invoice_watermark-7.2.0/trytond_account_invoice_watermark.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:34:20.000000 trytond_account_invoice_watermark-7.2.0/trytond_account_invoice_watermark.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_account_invoice_watermark-7.2.0/trytond_account_invoice_watermark.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       87 2024-04-29 15:34:20.000000 trytond_account_invoice_watermark-7.2.0/trytond_account_invoice_watermark.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:34:20.000000 trytond_account_invoice_watermark-7.2.0/trytond_account_invoice_watermark.egg-info/top_level.txt
```

### Comparing `trytond_account_invoice_watermark-7.0.0/COPYRIGHT` & `trytond_account_invoice_watermark-7.2.0/COPYRIGHT`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2021-2023 B2CK
-Copyright (C) 2021-2023 Cédric Krier
+Copyright (C) 2021-2024 B2CK
+Copyright (C) 2021-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_invoice_watermark-7.0.0/LICENSE` & `trytond_account_invoice_watermark-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_watermark-7.0.0/PKG-INFO` & `trytond_account_invoice_watermark-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_watermark
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add watermark to invoice
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice-watermark
+Project-URL: Documentation, https://docs.tryton.org/modules-account-invoice-watermark
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice watermark
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,18 +49,18 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pypdf>=3
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ################################
 Account Invoice Watermark Module
 ################################
 
 The *Account Invoice Watermark Module* adds a draft or paid watermark to the
 printed invoice.
```

### Comparing `trytond_account_invoice_watermark-7.0.0/account.py` & `trytond_account_invoice_watermark-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_watermark-7.0.0/account.xml` & `trytond_account_invoice_watermark-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_watermark-7.0.0/doc/conf.py` & `trytond_account_invoice_watermark-7.2.0/doc/conf.py`

 * *Files 10% similar despite different names*

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

### Comparing `trytond_account_invoice_watermark-7.0.0/invoice_watermark_draft.fodt` & `trytond_account_invoice_watermark-7.2.0/invoice_watermark_draft.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_watermark-7.0.0/invoice_watermark_paid.fodt` & `trytond_account_invoice_watermark-7.2.0/invoice_watermark_paid.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_watermark-7.0.0/setup.py` & `trytond_account_invoice_watermark-7.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/'
+            'https://docs.tryton.org/'
             'modules-account-invoice-watermark'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account invoice watermark',
     package_dir={'trytond.modules.account_invoice_watermark': '.'},
     packages=(
```

### Comparing `trytond_account_invoice_watermark-7.0.0/tests/scenario_account_invoice_watermark.rst` & `trytond_account_invoice_watermark-7.2.0/tests/scenario_account_invoice_watermark.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,22 @@
 Account Invoice Watermark Scenario
 ==================================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Report, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from proteus import Model, Report
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
-
-    >>> from trytond.modules.account_invoice_watermark.tests.tools import (
-    ...     pdf_contains)
+    >>> from trytond.modules.account_invoice_watermark.tests.tools import pdf_contains
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice_watermark')
 
     >>> ActionReport = Model.get('ir.action.report')
     >>> Invoice = Model.get('account.invoice')
```

### Comparing `trytond_account_invoice_watermark-7.0.0/tests/tools.py` & `trytond_account_invoice_watermark-7.2.0/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_watermark-7.0.0/tox.ini` & `trytond_account_invoice_watermark-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_watermark-7.0.0/trytond_account_invoice_watermark.egg-info/PKG-INFO` & `trytond_account_invoice_watermark-7.2.0/trytond_account_invoice_watermark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-account-invoice-watermark
-Version: 7.0.0
+Name: trytond_account_invoice_watermark
+Version: 7.2.0
 Summary: Tryton module to add watermark to invoice
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice-watermark
+Project-URL: Documentation, https://docs.tryton.org/modules-account-invoice-watermark
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice watermark
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,18 +49,18 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pypdf>=3
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ################################
 Account Invoice Watermark Module
 ################################
 
 The *Account Invoice Watermark Module* adds a draft or paid watermark to the
 printed invoice.
```

### Comparing `trytond_account_invoice_watermark-7.0.0/trytond_account_invoice_watermark.egg-info/SOURCES.txt` & `trytond_account_invoice_watermark-7.2.0/trytond_account_invoice_watermark.egg-info/SOURCES.txt`

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

