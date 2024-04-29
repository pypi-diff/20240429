# Comparing `tmp/trytond_account_invoice_stock-7.0.1.tar.gz` & `tmp/trytond_account_invoice_stock-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice_stock-7.0.1.tar", last modified: Sat Dec 16 10:05:56 2023, max compression
+gzip compressed data, was "trytond_account_invoice_stock-7.2.0.tar", last modified: Mon Apr 29 15:34:14 2024, max compression
```

## Comparing `trytond_account_invoice_stock-7.0.1.tar` & `trytond_account_invoice_stock-7.2.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:05:56.850410 trytond_account_invoice_stock-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      223 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2744 2023-12-16 10:05:54.000000 trytond_account_invoice_stock-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-12-16 10:05:54.000000 trytond_account_invoice_stock-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2872 2023-12-16 10:05:56.850410 trytond_account_invoice_stock-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5163 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      935 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:05:56.847077 trytond_account_invoice_stock-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2822 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:05:56.850410 trytond_account_invoice_stock-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1302 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1320 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1309 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1317 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1071 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1257 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1298 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1236 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1159 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1291 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1277 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1217 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1255 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1321 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1183 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1246 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-12-16 10:05:56.850410 trytond_account_invoice_stock-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4643 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4506 2023-12-10 12:55:22.000000 trytond_account_invoice_stock-7.0.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:05:56.850410 trytond_account_invoice_stock-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4004 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/tests/scenario_account_invoice_stock.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3792 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/tests/scenario_account_invoice_stock_correction.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      116 2023-10-30 17:55:12.000000 trytond_account_invoice_stock-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:05:56.850410 trytond_account_invoice_stock-7.0.1/trytond_account_invoice_stock.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2872 2023-12-16 10:05:56.000000 trytond_account_invoice_stock-7.0.1/trytond_account_invoice_stock.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1769 2023-12-16 10:05:56.000000 trytond_account_invoice_stock-7.0.1/trytond_account_invoice_stock.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-12-16 10:05:56.000000 trytond_account_invoice_stock-7.0.1/trytond_account_invoice_stock.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-12-16 10:05:56.000000 trytond_account_invoice_stock-7.0.1/trytond_account_invoice_stock.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:34.000000 trytond_account_invoice_stock-7.0.1/trytond_account_invoice_stock.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      128 2023-12-16 10:05:56.000000 trytond_account_invoice_stock-7.0.1/trytond_account_invoice_stock.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-12-16 10:05:56.000000 trytond_account_invoice_stock-7.0.1/trytond_account_invoice_stock.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-16 10:05:56.850410 trytond_account_invoice_stock-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-10-30 17:06:38.000000 trytond_account_invoice_stock-7.0.1/view/move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:14.782477 trytond_account_invoice_stock-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2744 2024-04-29 15:14:47.000000 trytond_account_invoice_stock-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:14:47.000000 trytond_account_invoice_stock-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_invoice_stock-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2863 2024-04-29 15:34:14.782477 trytond_account_invoice_stock-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5163 2024-02-04 18:51:26.000000 trytond_account_invoice_stock-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      912 2024-04-27 16:30:39.000000 trytond_account_invoice_stock-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:14.779144 trytond_account_invoice_stock-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3084 2024-04-27 16:30:39.000000 trytond_account_invoice_stock-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:56.000000 trytond_account_invoice_stock-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:14.779144 trytond_account_invoice_stock-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1302 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1320 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1309 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1317 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1071 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1257 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1298 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1236 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1159 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1291 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1270 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1253 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1277 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1217 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1255 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1321 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1183 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1246 2024-04-27 16:43:21.000000 trytond_account_invoice_stock-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:34:14.782477 trytond_account_invoice_stock-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4634 2024-04-27 16:30:39.000000 trytond_account_invoice_stock-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4506 2024-04-13 17:12:23.000000 trytond_account_invoice_stock-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-01-16 14:00:20.000000 trytond_account_invoice_stock-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:14.779144 trytond_account_invoice_stock-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3980 2024-04-27 16:30:39.000000 trytond_account_invoice_stock-7.2.0/tests/scenario_account_invoice_stock.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3778 2024-04-22 12:14:36.000000 trytond_account_invoice_stock-7.2.0/tests/scenario_account_invoice_stock_correction.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:56.000000 trytond_account_invoice_stock-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      116 2024-04-29 15:14:43.000000 trytond_account_invoice_stock-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:14.782477 trytond_account_invoice_stock-7.2.0/trytond_account_invoice_stock.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2863 2024-04-29 15:34:14.000000 trytond_account_invoice_stock-7.2.0/trytond_account_invoice_stock.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1751 2024-04-29 15:34:14.000000 trytond_account_invoice_stock-7.2.0/trytond_account_invoice_stock.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:34:14.000000 trytond_account_invoice_stock-7.2.0/trytond_account_invoice_stock.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:34:14.000000 trytond_account_invoice_stock-7.2.0/trytond_account_invoice_stock.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account_invoice_stock-7.2.0/trytond_account_invoice_stock.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      128 2024-04-29 15:34:14.000000 trytond_account_invoice_stock-7.2.0/trytond_account_invoice_stock.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:34:14.000000 trytond_account_invoice_stock-7.2.0/trytond_account_invoice_stock.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:34:14.782477 trytond_account_invoice_stock-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-7.2.0/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-7.2.0/view/move_form.xml
```

### Comparing `trytond_account_invoice_stock-7.0.1/CHANGELOG` & `trytond_account_invoice_stock-7.2.0/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2023-12-16
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_invoice_stock-7.0.1/LICENSE` & `trytond_account_invoice_stock-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/PKG-INFO` & `trytond_account_invoice_stock-7.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_stock
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to link stock and invoice
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice-stock/
+Project-URL: Documentation, https://docs.tryton.org/modules-account-invoice-stock/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice stock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ############################
 Account Invoice Stock Module
 ############################
 
 The *Account Invoice Stock Module* links together invoice lines and stock
 moves.
```

### Comparing `trytond_account_invoice_stock-7.0.1/account.py` & `trytond_account_invoice_stock-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/account.xml` & `trytond_account_invoice_stock-7.2.0/account.xml`

 * *Files 13% similar despite different names*

#### Comparing `trytond_account_invoice_stock-7.0.1/account.xml` & `trytond_account_invoice_stock-7.2.0/account.xml`

```diff
@@ -5,15 +5,15 @@
   <data>
     <record model="ir.ui.view" id="invoice_line_view_form">
       <field name="model">account.invoice.line</field>
       <field name="inherit" ref="account_invoice.invoice_line_view_form"/>
       <field name="name">invoice_line_form</field>
     </record>
     <record model="ir.model.access" id="access_stock_move_group_account">
-      <field name="model" search="[('model', '=', 'stock.move')]"/>
+      <field name="model">stock.move</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_account_invoice_stock-7.0.1/doc/conf.py` & `trytond_account_invoice_stock-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_invoice_stock-7.0.1/locale/bg.po` & `trytond_account_invoice_stock-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/ca.po` & `trytond_account_invoice_stock-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/cs.po` & `trytond_account_invoice_stock-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/de.po` & `trytond_account_invoice_stock-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/es.po` & `trytond_account_invoice_stock-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/es_419.po` & `trytond_account_invoice_stock-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/et.po` & `trytond_account_invoice_stock-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/fa.po` & `trytond_account_invoice_stock-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/fi.po` & `trytond_account_invoice_stock-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/fr.po` & `trytond_account_invoice_stock-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/hu.po` & `trytond_account_invoice_stock-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/id.po` & `trytond_account_invoice_stock-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/it.po` & `trytond_account_invoice_stock-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/lo.po` & `trytond_account_invoice_stock-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/lt.po` & `trytond_account_invoice_stock-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/nl.po` & `trytond_account_invoice_stock-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/pl.po` & `trytond_account_invoice_stock-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/pt.po` & `trytond_account_invoice_stock-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/ro.po` & `trytond_account_invoice_stock-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/ru.po` & `trytond_account_invoice_stock-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/sl.po` & `trytond_account_invoice_stock-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/tr.po` & `trytond_account_invoice_stock-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/uk.po` & `trytond_account_invoice_stock-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/locale/zh_CN.po` & `trytond_account_invoice_stock-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/setup.py` & `trytond_account_invoice_stock-7.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation":
-        'https://docs.tryton.org/projects/modules-account-invoice-stock/',
+        'https://docs.tryton.org/modules-account-invoice-stock/',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account invoice stock',
     package_dir={'trytond.modules.account_invoice_stock': '.'},
     packages=(
         ['trytond.modules.account_invoice_stock']
```

### Comparing `trytond_account_invoice_stock-7.0.1/stock.py` & `trytond_account_invoice_stock-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/tests/scenario_account_invoice_stock.rst` & `trytond_account_invoice_stock-7.2.0/tests/scenario_account_invoice_stock.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ========================
 Invoice - Stock Scenario
 ========================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice_stock')
 
 Create company::
 
@@ -108,15 +108,15 @@
     Decimal('40.0000')
 
 Ship the products::
 
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
 Check move unit price has been updated::
 
     >>> move.reload()
     >>> move.unit_price
```

### Comparing `trytond_account_invoice_stock-7.0.1/tests/scenario_account_invoice_stock_correction.rst` & `trytond_account_invoice_stock-7.2.0/tests/scenario_account_invoice_stock_correction.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Invoice - Stock Correction Scenario
 ===================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_invoice_stock')
```

### Comparing `trytond_account_invoice_stock-7.0.1/tox.ini` & `trytond_account_invoice_stock-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-7.0.1/trytond_account_invoice_stock.egg-info/PKG-INFO` & `trytond_account_invoice_stock-7.2.0/trytond_account_invoice_stock.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-account-invoice-stock
-Version: 7.0.1
+Name: trytond_account_invoice_stock
+Version: 7.2.0
 Summary: Tryton module to link stock and invoice
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-invoice-stock/
+Project-URL: Documentation, https://docs.tryton.org/modules-account-invoice-stock/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account invoice stock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ############################
 Account Invoice Stock Module
 ############################
 
 The *Account Invoice Stock Module* links together invoice lines and stock
 moves.
```

### Comparing `trytond_account_invoice_stock-7.0.1/trytond_account_invoice_stock.egg-info/SOURCES.txt` & `trytond_account_invoice_stock-7.2.0/trytond_account_invoice_stock.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_account_invoice_stock-7.0.1/view/invoice_line_form.xml` & `trytond_account_invoice_stock-7.2.0/view/invoice_line_form.xml`

 * *Files identical despite different names*

