# Comparing `tmp/trytond_account_cash_rounding-7.0.1.tar.gz` & `tmp/trytond_account_cash_rounding-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_cash_rounding-7.0.1.tar", last modified: Sat Feb  3 11:33:27 2024, max compression
+gzip compressed data, was "trytond_account_cash_rounding-7.2.0.tar", last modified: Mon Apr 29 15:32:02 2024, max compression
```

## Comparing `trytond_account_cash_rounding-7.0.1.tar` & `trytond_account_cash_rounding-7.2.0.tar`

### file list

```diff
@@ -1,71 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:33:27.064335 trytond_account_cash_rounding-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      223 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      925 2024-02-03 11:33:24.000000 trytond_account_cash_rounding-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-02-03 11:33:24.000000 trytond_account_cash_rounding-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3231 2024-02-03 11:33:27.064335 trytond_account_cash_rounding-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      543 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      833 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7782 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      832 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      587 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/currency.py
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/currency.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:33:27.061002 trytond_account_cash_rounding-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2822 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      543 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:33:27.061002 trytond_account_cash_rounding-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1756 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1685 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1798 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1384 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1789 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1697 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1643 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2889 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2291 2024-01-26 18:14:18.000000 trytond_account_cash_rounding-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-02-03 11:33:27.064335 trytond_account_cash_rounding-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4736 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:33:27.061002 trytond_account_cash_rounding-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3396 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/tests/scenario_account_cash_rounding.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3251 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/tests/scenario_account_cash_rounding_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2118 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/tests/scenario_account_cash_rounding_purchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2216 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/tests/scenario_account_cash_rounding_sale.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      192 2023-10-30 17:55:12.000000 trytond_account_cash_rounding-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:33:27.064335 trytond_account_cash_rounding-7.0.1/trytond_account_cash_rounding.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3231 2024-02-03 11:33:26.000000 trytond_account_cash_rounding-7.0.1/trytond_account_cash_rounding.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2210 2024-02-03 11:33:27.000000 trytond_account_cash_rounding-7.0.1/trytond_account_cash_rounding.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-02-03 11:33:26.000000 trytond_account_cash_rounding-7.0.1/trytond_account_cash_rounding.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-02-03 11:33:26.000000 trytond_account_cash_rounding-7.0.1/trytond_account_cash_rounding.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:30.000000 trytond_account_cash_rounding-7.0.1/trytond_account_cash_rounding.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      181 2024-02-03 11:33:26.000000 trytond_account_cash_rounding-7.0.1/trytond_account_cash_rounding.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-02-03 11:33:26.000000 trytond_account_cash_rounding-7.0.1/trytond_account_cash_rounding.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:33:27.064335 trytond_account_cash_rounding-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      582 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/view/account_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/view/account_invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/view/currency_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-10-30 17:06:38.000000 trytond_account_cash_rounding-7.0.1/view/purchase_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:02.819262 trytond_account_cash_rounding-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      925 2024-04-29 15:12:57.000000 trytond_account_cash_rounding-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:12:57.000000 trytond_account_cash_rounding-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3231 2024-04-29 15:32:02.819262 trytond_account_cash_rounding-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      543 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      833 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7782 2024-01-14 22:07:45.000000 trytond_account_cash_rounding-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      832 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      587 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/currency.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/currency.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:02.815928 trytond_account_cash_rounding-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3084 2024-04-27 16:30:39.000000 trytond_account_cash_rounding-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      543 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:51.000000 trytond_account_cash_rounding-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:02.815928 trytond_account_cash_rounding-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1756 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1685 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1798 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1754 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1384 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1789 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1697 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1643 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:20.000000 trytond_account_cash_rounding-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2889 2024-04-26 08:56:10.000000 trytond_account_cash_rounding-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2291 2024-04-22 12:14:36.000000 trytond_account_cash_rounding-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:32:02.819262 trytond_account_cash_rounding-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4736 2024-03-17 11:01:36.000000 trytond_account_cash_rounding-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:02.815928 trytond_account_cash_rounding-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3377 2024-04-22 12:14:36.000000 trytond_account_cash_rounding-7.2.0/tests/scenario_account_cash_rounding.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3626 2024-04-22 12:14:36.000000 trytond_account_cash_rounding-7.2.0/tests/scenario_account_cash_rounding_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2341 2024-04-22 12:14:36.000000 trytond_account_cash_rounding-7.2.0/tests/scenario_account_cash_rounding_purchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2435 2024-04-22 12:14:36.000000 trytond_account_cash_rounding-7.2.0/tests/scenario_account_cash_rounding_sale.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:51.000000 trytond_account_cash_rounding-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      192 2024-04-29 15:12:53.000000 trytond_account_cash_rounding-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:02.819262 trytond_account_cash_rounding-7.2.0/trytond_account_cash_rounding.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3231 2024-04-29 15:32:02.000000 trytond_account_cash_rounding-7.2.0/trytond_account_cash_rounding.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2192 2024-04-29 15:32:02.000000 trytond_account_cash_rounding-7.2.0/trytond_account_cash_rounding.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:32:02.000000 trytond_account_cash_rounding-7.2.0/trytond_account_cash_rounding.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:32:02.000000 trytond_account_cash_rounding-7.2.0/trytond_account_cash_rounding.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_account_cash_rounding-7.2.0/trytond_account_cash_rounding.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      181 2024-04-29 15:32:02.000000 trytond_account_cash_rounding-7.2.0/trytond_account_cash_rounding.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:32:02.000000 trytond_account_cash_rounding-7.2.0/trytond_account_cash_rounding.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:02.819262 trytond_account_cash_rounding-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      582 2023-04-15 07:12:15.000000 trytond_account_cash_rounding-7.2.0/view/account_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/view/account_invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/view/currency_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:14.000000 trytond_account_cash_rounding-7.2.0/view/purchase_form.xml
```

### Comparing `trytond_account_cash_rounding-7.0.1/CHANGELOG` & `trytond_account_cash_rounding-7.2.0/CHANGELOG`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-02-03
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_account_cash_rounding-7.0.1/LICENSE` & `trytond_account_cash_rounding-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/PKG-INFO` & `trytond_account_cash_rounding-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_cash_rounding
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to round cash amount
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
@@ -48,22 +48,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
 
 Account Cash Rounding Module
 ############################
 
 The account_cash_rounding module allows cash amounts to be rounded using the
 cash rounding factor of the currency.
```

### Comparing `trytond_account_cash_rounding-7.0.1/README.rst` & `trytond_account_cash_rounding-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/__init__.py` & `trytond_account_cash_rounding-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/account.py` & `trytond_account_cash_rounding-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/account.xml` & `trytond_account_cash_rounding-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/currency.py` & `trytond_account_cash_rounding-7.2.0/currency.py`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/doc/conf.py` & `trytond_account_cash_rounding-7.2.0/doc/conf.py`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_account_cash_rounding-7.0.1/doc/index.rst` & `trytond_account_cash_rounding-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/bg.po` & `trytond_account_cash_rounding-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/ca.po` & `trytond_account_cash_rounding-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/cs.po` & `trytond_account_cash_rounding-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/de.po` & `trytond_account_cash_rounding-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/es.po` & `trytond_account_cash_rounding-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/es_419.po` & `trytond_account_cash_rounding-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/et.po` & `trytond_account_cash_rounding-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/fa.po` & `trytond_account_cash_rounding-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/fi.po` & `trytond_account_cash_rounding-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/fr.po` & `trytond_account_cash_rounding-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/hu.po` & `trytond_account_cash_rounding-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/id.po` & `trytond_account_cash_rounding-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/it.po` & `trytond_account_cash_rounding-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/lo.po` & `trytond_account_cash_rounding-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/lt.po` & `trytond_account_cash_rounding-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/nl.po` & `trytond_account_cash_rounding-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/pl.po` & `trytond_account_cash_rounding-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/pt.po` & `trytond_account_cash_rounding-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/ro.po` & `trytond_account_cash_rounding-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/ru.po` & `trytond_account_cash_rounding-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/sl.po` & `trytond_account_cash_rounding-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/tr.po` & `trytond_account_cash_rounding-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/uk.po` & `trytond_account_cash_rounding-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/locale/zh_CN.po` & `trytond_account_cash_rounding-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/purchase.py` & `trytond_account_cash_rounding-7.2.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/sale.py` & `trytond_account_cash_rounding-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/setup.py` & `trytond_account_cash_rounding-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/tests/scenario_account_cash_rounding.rst` & `trytond_account_cash_rounding-7.2.0/tests/scenario_account_cash_rounding.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ==============================
 Account Cash Rounding Scenario
 ==============================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
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
 
     >>> config = activate_modules(['account_cash_rounding', 'account_invoice'])
 
 Create company::
```

### Comparing `trytond_account_cash_rounding-7.0.1/tests/scenario_account_cash_rounding_alternate_currency.rst` & `trytond_account_cash_rounding-7.2.0/tests/scenario_account_cash_rounding_alternate_currency.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 =================================================
 Account Cash Rounding Alternate Currency Scenario
 =================================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.currency.tests.tools import get_currency
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
+    >>> from trytond.modules.currency.tests.tools import get_currency
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules(['account_cash_rounding', 'account_invoice'])
 
+    >>> Configuration = Model.get('account.configuration')
+
 Set alternate currencies::
 
     >>> currency = get_currency('USD')
     >>> eur = get_currency('EUR')
 
 Create company::
 
@@ -38,14 +40,24 @@
 Create chart of accounts::
 
     >>> Account = Model.get('account.account')
     >>> AccountConfig = Model.get('account.configuration')
     >>> _ = create_chart(company)
     >>> accounts = get_accounts(company)
 
+Configure currency exchange::
+
+    >>> currency_exchange_account, = (
+    ...     accounts['revenue'].duplicate(
+    ...         default={'name': "Currency Exchange"}))
+    >>> configuration = Configuration(1)
+    >>> configuration.currency_exchange_debit_account = (
+    ...     currency_exchange_account)
+    >>> configuration.save()
+
 Set cash rounding::
 
     >>> cash_rounding_credit = Account(name="Cash Rounding")
     >>> cash_rounding_credit.type = accounts['revenue'].type
     >>> cash_rounding_credit.deferral = True
     >>> cash_rounding_credit.save()
     >>> cash_rounding_debit = Account(name="Cash Rounding")
@@ -94,10 +106,10 @@
 
     >>> cash_rounding_credit.reload()
     >>> cash_rounding_credit.credit, cash_rounding_credit.debit
     (Decimal('0.00'), Decimal('0.00'))
 
     >>> line_to_pay, = invoice.lines_to_pay
     >>> line_to_pay.debit, line_to_pay.credit
-    (Decimal('21.03'), Decimal('0'))
+    (Decimal('21.02'), Decimal('0'))
     >>> line_to_pay.amount_second_currency
     Decimal('42.05')
```

### Comparing `trytond_account_cash_rounding-7.0.1/tests/scenario_account_cash_rounding_purchase.rst` & `trytond_account_cash_rounding-7.2.0/tests/scenario_account_cash_rounding_purchase.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 =======================================
 Account Cash Rounding Purchase Scenario
 =======================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.account_invoice.tests.tools import create_payment_term
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
 
 Activate modules::
 
-    >>> config = activate_modules(['account_cash_rounding', 'purchase'])
+    >>> config = activate_modules(
+    ...     ['account_cash_rounding', 'account_invoice', 'purchase'])
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create chart of accounts::
@@ -41,19 +42,25 @@
 
 Create party::
 
     >>> Party = Model.get('party.party')
     >>> party = Party(name='Party')
     >>> party.save()
 
+Create payment term::
+
+    >>> payment_term = create_payment_term()
+    >>> payment_term.save()
+
 Create purchase::
 
     >>> Purchase = Model.get('purchase.purchase')
     >>> purchase = Purchase()
     >>> purchase.party = party
+    >>> purchase.payment_term = payment_term
     >>> line = purchase.lines.new()
     >>> line.quantity = 1
     >>> line.unit_price = Decimal('42.07')
     >>> purchase.untaxed_amount, purchase.tax_amount, purchase.total_amount
     (Decimal('42.07'), Decimal('0.00'), Decimal('42.07'))
     >>> purchase.cash_rounding = True
     >>> purchase.untaxed_amount, purchase.tax_amount, purchase.total_amount
```

### Comparing `trytond_account_cash_rounding-7.0.1/tests/scenario_account_cash_rounding_sale.rst` & `trytond_account_cash_rounding-7.2.0/tests/scenario_account_cash_rounding_sale.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 ===================================
 Account Cash Rounding Sale Scenario
 ===================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.account_invoice.tests.tools import create_payment_term
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
 
 Activate modules::
 
-    >>> config = activate_modules(['account_cash_rounding', 'sale'])
+    >>> config = activate_modules(
+    ...     ['account_cash_rounding', 'account_invoice', 'sale'])
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
 Create chart of accounts::
@@ -50,19 +51,25 @@
 
 Create party::
 
     >>> Party = Model.get('party.party')
     >>> party = Party(name='Party')
     >>> party.save()
 
+Create payment term::
+
+    >>> payment_term = create_payment_term()
+    >>> payment_term.save()
+
 Create sale::
 
     >>> Sale = Model.get('sale.sale')
     >>> sale = Sale()
     >>> sale.party = party
+    >>> sale.payment_term = payment_term
     >>> line = sale.lines.new()
     >>> line.quantity = 1
     >>> line.unit_price = Decimal('42.02')
     >>> sale.untaxed_amount, sale.tax_amount, sale.total_amount
     (Decimal('42.02'), Decimal('0.00'), Decimal('42.00'))
     >>> sale.click('quote')
     >>> sale.untaxed_amount, sale.tax_amount, sale.total_amount
```

### Comparing `trytond_account_cash_rounding-7.0.1/tox.ini` & `trytond_account_cash_rounding-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_cash_rounding-7.0.1/trytond_account_cash_rounding.egg-info/PKG-INFO` & `trytond_account_cash_rounding-7.2.0/trytond_account_cash_rounding.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_cash_rounding
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to round cash amount
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
@@ -48,22 +48,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
 
 Account Cash Rounding Module
 ############################
 
 The account_cash_rounding module allows cash amounts to be rounded using the
 cash rounding factor of the currency.
```

### Comparing `trytond_account_cash_rounding-7.0.1/trytond_account_cash_rounding.egg-info/SOURCES.txt` & `trytond_account_cash_rounding-7.2.0/trytond_account_cash_rounding.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

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

### Comparing `trytond_account_cash_rounding-7.0.1/view/account_configuration_form.xml` & `trytond_account_cash_rounding-7.2.0/view/account_configuration_form.xml`

 * *Files identical despite different names*

