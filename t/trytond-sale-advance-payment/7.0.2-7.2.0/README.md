# Comparing `tmp/trytond_sale_advance_payment-7.0.2.tar.gz` & `tmp/trytond_sale_advance_payment-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_advance_payment-7.0.2.tar", last modified: Wed Apr 17 10:37:38 2024, max compression
+gzip compressed data, was "trytond_sale_advance_payment-7.2.0.tar", last modified: Mon Apr 29 15:47:10 2024, max compression
```

## Comparing `trytond_sale_advance_payment-7.0.2.tar` & `trytond_sale_advance_payment-7.2.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:37:38.483596 trytond_sale_advance_payment-7.0.2/
--rw-r--r--   0 ced       (1000) ced       (1000)     1633 2024-04-17 10:37:35.000000 trytond_sale_advance_payment-7.0.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-17 10:37:35.000000 trytond_sale_advance_payment-7.0.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4361 2024-04-17 10:37:38.483596 trytond_sale_advance_payment-7.0.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1718 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      754 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3343 2024-04-12 20:29:30.000000 trytond_sale_advance_payment-7.0.2/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      787 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:37:38.476929 trytond_sale_advance_payment-7.0.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2799 2024-03-03 16:24:20.000000 trytond_sale_advance_payment-7.0.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1718 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:37:38.480263 trytond_sale_advance_payment-7.0.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6416 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6304 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6360 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4871 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5335 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6830 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6343 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4957 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5144 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5349 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6356 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5212 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6073 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4993 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5750 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4871 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2242 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1238 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1213 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1212 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1205 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1212 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1209 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1210 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1214 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1211 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    17135 2024-02-05 16:24:27.000000 trytond_sale_advance_payment-7.0.2/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5721 2024-02-05 16:24:27.000000 trytond_sale_advance_payment-7.0.2/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:37:38.483596 trytond_sale_advance_payment-7.0.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4621 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1036 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:37:38.480263 trytond_sale_advance_payment-7.0.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12088 2024-02-05 16:24:27.000000 trytond_sale_advance_payment-7.0.2/tests/scenario_advance_payment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4581 2024-02-05 16:24:27.000000 trytond_sale_advance_payment-7.0.2/tests/scenario_sale_advance_payment_on_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2024-02-05 16:24:27.000000 trytond_sale_advance_payment-7.0.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1290 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2024-02-05 16:24:27.000000 trytond_sale_advance_payment-7.0.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:37:38.480263 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4361 2024-04-17 10:37:38.000000 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2749 2024-04-17 10:37:38.000000 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:37:38.000000 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-17 10:37:38.000000 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:04.000000 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      168 2024-04-17 10:37:38.000000 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:37:38.000000 trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:37:38.480263 trytond_sale_advance_payment-7.0.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      735 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/advance_payment_condition_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/advance_payment_condition_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/advance_payment_term_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/advance_payment_term_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/advance_payment_term_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/advance_payment_term_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      630 2023-10-30 17:06:38.000000 trytond_sale_advance_payment-7.0.2/view/sale_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:10.552187 trytond_sale_advance_payment-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-29 15:24:37.000000 trytond_sale_advance_payment-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:24:36.000000 trytond_sale_advance_payment-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_advance_payment-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4402 2024-04-29 15:47:10.552187 trytond_sale_advance_payment-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1718 2023-01-16 14:00:21.000000 trytond_sale_advance_payment-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      754 2023-12-21 15:24:43.000000 trytond_sale_advance_payment-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3343 2024-04-27 16:30:39.000000 trytond_sale_advance_payment-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      787 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:10.545521 trytond_sale_advance_payment-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-27 16:30:39.000000 trytond_sale_advance_payment-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1718 2023-01-16 14:00:21.000000 trytond_sale_advance_payment-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:23.000000 trytond_sale_advance_payment-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:10.548854 trytond_sale_advance_payment-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6416 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6304 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6360 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4871 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5335 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6830 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6343 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4957 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5144 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5349 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6356 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5212 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6073 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6184 2024-04-29 13:17:17.000000 trytond_sale_advance_payment-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5750 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4871 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2024-04-27 16:43:26.000000 trytond_sale_advance_payment-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      645 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2242 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1238 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1213 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1212 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1205 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1212 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1209 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1210 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1214 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1211 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    17700 2024-04-27 16:30:39.000000 trytond_sale_advance_payment-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4730 2024-04-27 16:30:39.000000 trytond_sale_advance_payment-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:47:10.552187 trytond_sale_advance_payment-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4621 2024-03-17 11:01:36.000000 trytond_sale_advance_payment-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1036 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:10.548854 trytond_sale_advance_payment-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12064 2024-04-22 12:14:36.000000 trytond_sale_advance_payment-7.2.0/tests/scenario_advance_payment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4554 2024-04-27 16:30:39.000000 trytond_sale_advance_payment-7.2.0/tests/scenario_sale_advance_payment_on_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2024-04-22 12:14:36.000000 trytond_sale_advance_payment-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1290 2024-01-27 09:58:52.000000 trytond_sale_advance_payment-7.2.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:23.000000 trytond_sale_advance_payment-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2024-04-29 15:24:32.000000 trytond_sale_advance_payment-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:10.552187 trytond_sale_advance_payment-7.2.0/trytond_sale_advance_payment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4402 2024-04-29 15:47:10.000000 trytond_sale_advance_payment-7.2.0/trytond_sale_advance_payment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2749 2024-04-29 15:47:10.000000 trytond_sale_advance_payment-7.2.0/trytond_sale_advance_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:47:10.000000 trytond_sale_advance_payment-7.2.0/trytond_sale_advance_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:47:10.000000 trytond_sale_advance_payment-7.2.0/trytond_sale_advance_payment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_sale_advance_payment-7.2.0/trytond_sale_advance_payment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      194 2024-04-29 15:47:10.000000 trytond_sale_advance_payment-7.2.0/trytond_sale_advance_payment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:47:10.000000 trytond_sale_advance_payment-7.2.0/trytond_sale_advance_payment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:47:10.552187 trytond_sale_advance_payment-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      735 2023-12-21 15:24:43.000000 trytond_sale_advance_payment-7.2.0/view/advance_payment_condition_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-12-21 15:24:43.000000 trytond_sale_advance_payment-7.2.0/view/advance_payment_condition_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2023-01-16 14:00:21.000000 trytond_sale_advance_payment-7.2.0/view/advance_payment_term_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-01-16 14:00:21.000000 trytond_sale_advance_payment-7.2.0/view/advance_payment_term_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/view/advance_payment_term_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_sale_advance_payment-7.2.0/view/advance_payment_term_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      630 2023-12-21 15:24:43.000000 trytond_sale_advance_payment-7.2.0/view/sale_form.xml
```

### Comparing `trytond_sale_advance_payment-7.0.2/CHANGELOG` & `trytond_sale_advance_payment-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 
-Version 7.0.2 - 2024-04-17
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

### Comparing `trytond_sale_advance_payment-7.0.2/COPYRIGHT` & `trytond_sale_advance_payment-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/LICENSE` & `trytond_sale_advance_payment-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/PKG-INFO` & `trytond_sale_advance_payment-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_advance_payment
-Version: 7.0.2
+Version: 7.2.0
 Summary: Tryton module for sale advance payment
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
@@ -49,21 +49,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: simpleeval
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_supply<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_supply<7.3,>=7.2; extra == "test"
 
 Sale Advance Payment Module
 ###########################
 
 The sale_advance_payment module adds support for advance payment management on
 the sale.
```

### Comparing `trytond_sale_advance_payment-7.0.2/README.rst` & `trytond_sale_advance_payment-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/__init__.py` & `trytond_sale_advance_payment-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/account.py` & `trytond_sale_advance_payment-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/account.xml` & `trytond_sale_advance_payment-7.2.0/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/doc/conf.py` & `trytond_sale_advance_payment-7.2.0/doc/conf.py`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_sale_advance_payment-7.0.2/doc/index.rst` & `trytond_sale_advance_payment-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/bg.po` & `trytond_sale_advance_payment-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/ca.po` & `trytond_sale_advance_payment-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/cs.po` & `trytond_sale_advance_payment-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/de.po` & `trytond_sale_advance_payment-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/es.po` & `trytond_sale_advance_payment-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/es_419.po` & `trytond_sale_advance_payment-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/et.po` & `trytond_sale_advance_payment-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/fa.po` & `trytond_sale_advance_payment-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/fi.po` & `trytond_sale_advance_payment-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/fr.po` & `trytond_sale_advance_payment-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/hu.po` & `trytond_sale_advance_payment-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/id.po` & `trytond_sale_advance_payment-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/it.po` & `trytond_sale_advance_payment-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/lo.po` & `trytond_sale_advance_payment-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/lt.po` & `trytond_sale_advance_payment-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/nl.po` & `trytond_sale_advance_payment-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/pl.po` & `trytond_sale_advance_payment-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/pt.po` & `trytond_sale_advance_payment-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/ro.po` & `trytond_sale_advance_payment-7.2.0/locale/uk.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 msgid "Unearned Revenue"
 msgstr ""
 
 msgctxt "field:account.account.type.template,unearned_revenue:"
 msgid "Unearned Revenue"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.invoice.line,advance_payment_recalled_lines:"
 msgid "Advance Payment Recalled Lines"
-msgstr "Termen de plata in avans"
+msgstr ""
 
 msgctxt "field:sale.advance_payment.condition,account:"
 msgid "Account"
-msgstr "Cont"
+msgstr ""
 
 msgctxt "field:sale.advance_payment.condition,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "field:sale.advance_payment.condition,block_shipping:"
 msgid "Block Shipping"
 msgstr ""
 
 msgctxt "field:sale.advance_payment.condition,block_supply:"
 msgid "Block Supply"
@@ -37,15 +36,15 @@
 
 msgctxt "field:sale.advance_payment.condition,currency:"
 msgid "Currency"
 msgstr ""
 
 msgctxt "field:sale.advance_payment.condition,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:sale.advance_payment.condition,invoice_delay:"
 msgid "Invoice Delay"
 msgstr ""
 
 msgctxt "field:sale.advance_payment.condition,invoice_lines:"
 msgid "Invoice Lines"
@@ -53,67 +52,67 @@
 
 msgctxt "field:sale.advance_payment.condition,sale:"
 msgid "Sale"
 msgstr ""
 
 msgctxt "field:sale.advance_payment.condition,sale_company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:sale.advance_payment.condition,sale_state:"
 msgid "Sale State"
 msgstr ""
 
 msgctxt "field:sale.advance_payment_term,lines:"
 msgid "Lines"
-msgstr "Rânduri"
+msgstr ""
 
 msgctxt "field:sale.advance_payment_term,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:sale.advance_payment_term.line,account:"
 msgid "Account"
-msgstr "Cont"
+msgstr ""
 
 msgctxt "field:sale.advance_payment_term.line,accounts:"
 msgid "Accounts"
-msgstr "Conturi"
+msgstr ""
 
 msgctxt "field:sale.advance_payment_term.line,advance_payment_term:"
 msgid "Advance Payment Term"
-msgstr "Termen de plata in avans"
+msgstr ""
 
 msgctxt "field:sale.advance_payment_term.line,block_shipping:"
 msgid "Block Shipping"
 msgstr ""
 
 msgctxt "field:sale.advance_payment_term.line,block_supply:"
 msgid "Block Supply"
 msgstr ""
 
 msgctxt "field:sale.advance_payment_term.line,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:sale.advance_payment_term.line,formula:"
 msgid "Formula"
 msgstr ""
 
 msgctxt "field:sale.advance_payment_term.line,invoice_delay:"
 msgid "Invoice Delay"
 msgstr ""
 
 msgctxt "field:sale.advance_payment_term.line.account,account:"
 msgid "Account"
-msgstr "Cont"
+msgstr ""
 
 msgctxt "field:sale.advance_payment_term.line.account,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:sale.advance_payment_term.line.account,line:"
 msgid "Line"
 msgstr ""
 
 msgctxt "field:sale.sale,advance_payment_conditions:"
 msgid "Advance Payment Conditions"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_sale_advance_payment-7.0.2/locale/ru.po` & `trytond_sale_advance_payment-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/sl.po` & `trytond_sale_advance_payment-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/tr.po` & `trytond_sale_advance_payment-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/locale/uk.po` & `trytond_sale_advance_payment-7.2.0/locale/zh_CN.po`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 msgid "Unearned Revenue"
 msgstr ""
 
 msgctxt "field:account.account.type.template,unearned_revenue:"
 msgid "Unearned Revenue"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.invoice.line,advance_payment_recalled_lines:"
 msgid "Advance Payment Recalled Lines"
-msgstr ""
+msgstr "Advance Payment Terms"
 
 msgctxt "field:sale.advance_payment.condition,account:"
 msgid "Account"
 msgstr ""
 
 msgctxt "field:sale.advance_payment.condition,amount:"
 msgid "Amount"
@@ -74,17 +75,18 @@
 msgid "Account"
 msgstr ""
 
 msgctxt "field:sale.advance_payment_term.line,accounts:"
 msgid "Accounts"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.advance_payment_term.line,advance_payment_term:"
 msgid "Advance Payment Term"
-msgstr ""
+msgstr "Advance Payment Terms"
 
 msgctxt "field:sale.advance_payment_term.line,block_shipping:"
 msgid "Block Shipping"
 msgstr ""
 
 msgctxt "field:sale.advance_payment_term.line,block_supply:"
 msgid "Block Supply"
@@ -118,17 +120,18 @@
 msgid "Advance Payment Conditions"
 msgstr ""
 
 msgctxt "field:sale.sale,advance_payment_invoices:"
 msgid "Advance Payment Invoices"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.sale,advance_payment_term:"
 msgid "Advance Payment Term"
-msgstr ""
+msgstr "Advance Payment Terms"
 
 msgctxt "help:sale.advance_payment_term.line,account:"
 msgid "Used for the line of advance payment invoice."
 msgstr ""
 
 msgctxt "help:sale.advance_payment_term.line,block_shipping:"
 msgid "Check to prevent the packing of the shipment before advance payment."
@@ -152,19 +155,19 @@
 msgctxt "help:sale.advance_payment_term.line,invoice_delay:"
 msgid ""
 "Delta to apply on the sale date for the date of the advance payment invoice."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_advance_invoice_form"
 msgid "Advance Invoices"
-msgstr ""
+msgstr "Advance Invoices"
 
 msgctxt "model:ir.action,name:act_advance_payment_term_form"
 msgid "Advance Payment Terms"
-msgstr ""
+msgstr "Advance Payment Terms"
 
 msgctxt "model:ir.message,text:msg_shipping_blocked"
 msgid ""
 "To pack shipments the customer must paid the advance payment for sale "
 "\"%(sale)s\"."
 msgstr ""
 
@@ -172,24 +175,27 @@
 msgid ""
 "Invalid formula \"%(formula)s\" in term line \"%(term_line)s\" with "
 "exception \"%(exception)s\"."
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_advance_payment_term"
 msgid "Advance Payment Terms"
-msgstr ""
+msgstr "Advance Payment Terms"
 
 msgctxt "model:sale.advance_payment.condition,name:"
 msgid "Advance Payment Condition"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:sale.advance_payment_term,name:"
 msgid "Advance Payment Term"
-msgstr ""
+msgstr "Advance Payment Terms"
 
+#, fuzzy
 msgctxt "model:sale.advance_payment_term.line,name:"
 msgid "Advance Payment Term Line"
-msgstr ""
+msgstr "Advance Payment Terms"
 
+#, fuzzy
 msgctxt "model:sale.advance_payment_term.line.account,name:"
 msgid "Advance Payment Term Line Account"
-msgstr ""
+msgstr "Advance Payment Terms"
```

### Comparing `trytond_sale_advance_payment-7.0.2/message.xml` & `trytond_sale_advance_payment-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/minimal_chart.xml` & `trytond_sale_advance_payment-7.2.0/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/minimal_chart_bg.xml` & `trytond_sale_advance_payment-7.2.0/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/minimal_chart_ca.xml` & `trytond_sale_advance_payment-7.2.0/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/minimal_chart_de.xml` & `trytond_sale_advance_payment-7.2.0/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/minimal_chart_en.xml` & `trytond_sale_advance_payment-7.2.0/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/minimal_chart_es.xml` & `trytond_sale_advance_payment-7.2.0/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/minimal_chart_fr.xml` & `trytond_sale_advance_payment-7.2.0/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/minimal_chart_nl.xml` & `trytond_sale_advance_payment-7.2.0/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/minimal_chart_pt.xml` & `trytond_sale_advance_payment-7.2.0/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/minimal_chart_ru.xml` & `trytond_sale_advance_payment-7.2.0/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/minimal_chart_sl.xml` & `trytond_sale_advance_payment-7.2.0/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/sale.py` & `trytond_sale_advance_payment-7.2.0/sale.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,18 @@
 
 class AdvancePaymentTermLineAccount(ModelSQL, CompanyValueMixin):
     "Advance Payment Term Line Account"
     __name__ = 'sale.advance_payment_term.line.account'
 
     line = fields.Many2One(
         'sale.advance_payment_term.line', "Line",
-        required=True, ondelete='CASCADE')
+        required=True, ondelete='CASCADE',
+        context={
+            'company': Eval('company', -1),
+            })
     account = fields.Many2One(
         'account.account', "Account", required=True,
         domain=[
             ('type.unearned_revenue', '=', True),
             ('company', '=', Eval('company', -1)),
             ])
 
@@ -182,14 +185,15 @@
 
     del _states
 
     @classmethod
     def __setup__(cls):
         super(AdvancePaymentCondition, cls).__setup__()
         cls._order.insert(0, ('amount', 'ASC'))
+        cls.__access__.add('sale')
 
     @classmethod
     def get_sale_states(cls):
         pool = Pool()
         Sale = pool.get('sale.sale')
         return Sale.fields_get(['state'])['state']['selection']
 
@@ -213,24 +217,22 @@
         else:
             default = default.copy()
         default.setdefault('invoice_lines', [])
         return super(AdvancePaymentCondition, cls).copy(conditions, default)
 
     def create_invoice(self):
         invoice = self.sale._get_invoice_sale()
-        invoice.invoice_date = self.sale.sale_date
-        if self.invoice_delay:
-            invoice.invoice_date += self.invoice_delay
+        if self.invoice_delay is not None:
+            invoice.invoice_date = self.sale.sale_date + self.invoice_delay
         invoice.payment_term = None
 
         invoice_lines = self.get_invoice_advance_payment_lines(invoice)
         if not invoice_lines:
             return None
         invoice.lines = invoice_lines
-        invoice.save()
         return invoice
 
     def get_invoice_advance_payment_lines(self, invoice):
         pool = Pool()
         InvoiceLine = pool.get('account.invoice.line')
 
         advance_amount = self._get_advance_amount()
@@ -287,14 +289,24 @@
             })
     advance_payment_invoices = fields.Function(fields.Many2Many(
             'account.invoice', None, None, "Advance Payment Invoices"),
         'get_advance_payment_invoices',
         searcher='search_advance_payment_invoices')
 
     @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        cls.invoices_ignored.domain = [
+            'OR', cls.invoices_ignored.domain, [
+                ('id', 'in', Eval('advance_payment_invoices', [])),
+                ('state', '=', 'cancelled'),
+                ],
+            ]
+
+    @classmethod
     @ModelView.button
     @Workflow.transition('quotation')
     def quote(cls, sales):
         pool = Pool()
         AdvancePaymentCondition = pool.get('sale.advance_payment.condition')
 
         super(Sale, cls).quote(sales)
@@ -371,33 +383,39 @@
                     origin=advance_line,
                     taxes=advance_line.taxes,
                     taxes_date=advance_line.tax_date,
                     )
                 recall_lines.append(line)
         return recall_lines
 
-    def create_invoice(self):
+    @classmethod
+    def _process_invoice(cls, sales):
         pool = Pool()
-        InvoiceLine = pool.get('account.invoice.line')
+        Invoice = pool.get('account.invoice')
+        invoices = []
+        for sale in sales:
+            if (sale.advance_payment_eligible()
+                    and not sale.advance_payment_completed):
+                for condition in sale.advance_payment_conditions:
+                    invoice = condition.create_invoice()
+                    if invoice:
+                        invoices.append(invoice)
+        Invoice.save(invoices)
 
-        invoice = super(Sale, self).create_invoice()
+        super()._process_invoice(sales)
 
-        if self.advance_payment_eligible():
-            if not self.advance_payment_completed:
-                for condition in self.advance_payment_conditions:
-                    condition.create_invoice()
-            elif invoice is not None:
-                invoice.save()
-                recall_lines = self.get_recall_lines(invoice)
-                if recall_lines:
-                    for line in recall_lines:
-                        line.invoice = invoice
-                    InvoiceLine.save(recall_lines)
-                    invoice.update_taxes()
+    def create_invoice(self):
+        invoice = super(Sale, self).create_invoice()
 
+        if (invoice is not None
+                and self.advance_payment_eligible()
+                and self.advance_payment_completed):
+            invoice.lines = (
+                list(getattr(invoice, 'lines', ()))
+                + self.get_recall_lines(invoice))
         return invoice
 
     def advance_payment_eligible(self, shipment_type=None):
         """
         Returns True when the shipment_type is eligible to further processing
         of the sale's advance payment.
         """
```

### Comparing `trytond_sale_advance_payment-7.0.2/sale.xml` & `trytond_sale_advance_payment-7.2.0/sale.xml`

 * *Files 11% similar despite different names*

#### Comparing `trytond_sale_advance_payment-7.0.2/sale.xml` & `trytond_sale_advance_payment-7.2.0/sale.xml`

```diff
@@ -59,38 +59,23 @@
       <field name="name">advance_payment_term_line_form</field>
     </record>
     <record model="ir.ui.view" id="advance_payment_term_line_list">
       <field name="model">sale.advance_payment_term.line</field>
       <field name="type">tree</field>
       <field name="name">advance_payment_term_line_list</field>
     </record>
-    <record model="ir.model.access" id="access_advance_payment_condition">
-      <field name="model" search="[('model', '=', 'sale.advance_payment.condition')]"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="False"/>
-      <field name="perm_create" eval="False"/>
-      <field name="perm_delete" eval="False"/>
-    </record>
-    <record model="ir.model.access" id="access_advance_payment_condition_sale_admin">
-      <field name="model" search="[('model', '=', 'sale.advance_payment.condition')]"/>
-      <field name="group" ref="sale.group_sale_admin"/>
-      <field name="perm_read" eval="True"/>
-      <field name="perm_write" eval="True"/>
-      <field name="perm_create" eval="True"/>
-      <field name="perm_delete" eval="True"/>
-    </record>
     <record model="ir.model.access" id="access_advance_payment_term">
-      <field name="model" search="[('model', '=', 'sale.advance_payment_term')]"/>
+      <field name="model">sale.advance_payment_term</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_advance_payment_term_sale_admin">
-      <field name="model" search="[('model', '=', 'sale.advance_payment_term')]"/>
+      <field name="model">sale.advance_payment_term</field>
       <field name="group" ref="sale.group_sale_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_sale_advance_payment-7.0.2/setup.py` & `trytond_sale_advance_payment-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/stock.py` & `trytond_sale_advance_payment-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/tests/scenario_advance_payment.rst` & `trytond_sale_advance_payment-7.2.0/tests/scenario_advance_payment.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 Sale Advance Payment Scenario
 ==============================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> from trytond.modules.sale_advance_payment.tests.tools import \
-    ...     create_advance_payment_term, add_advance_payment_accounts
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.modules.sale_advance_payment.tests.tools import (
+    ...     add_advance_payment_accounts, create_advance_payment_term)
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
     >>> next_week = today + dt.timedelta(days=7)
 
 Activate sale_advance_payment::
 
     >>> config = activate_modules(['sale_advance_payment', 'sale_supply'])
@@ -131,16 +131,15 @@
     >>> sale.state
     'processing'
 
 As usual an invoice and a shipment has been created::
 
     >>> invoice, = sale.invoices
     >>> invoice_line, = invoice.lines
-    >>> invoice_line.account == revenue
-    True
+    >>> assertEqual(invoice_line.account, revenue)
     >>> invoice.total_amount
     Decimal('20.00')
     >>> len(sale.shipments)
     1
 
 Create a sale with advance payment::
 
@@ -160,20 +159,18 @@
     >>> sale.state
     'processing'
 
 The advance payment invoice has been created::
 
     >>> invoice, = sale.advance_payment_invoices
     >>> invoice_line, = invoice.lines
-    >>> invoice_line.account == advance_payment_account
-    True
+    >>> assertEqual(invoice_line.account, advance_payment_account)
     >>> invoice.total_amount
     Decimal('10.00')
-    >>> invoice.invoice_date == next_week
-    True
+    >>> assertEqual(invoice.invoice_date, next_week)
     >>> invoice.invoice_date = None
     >>> invoice.click('post')
     >>> sale.reload()
     >>> len(sale.invoices)
     0
     >>> len(sale.shipments)
     0
@@ -195,24 +192,21 @@
     >>> invoice, = sale.invoices
     >>> invoice.total_amount
     Decimal('90.00')
     >>> len(invoice.lines)
     2
     >>> il1, il2 = sorted([il for il in invoice.lines],
     ...     key=lambda il: 1 if il.product else 0)
-    >>> il1.account == advance_payment_account
-    True
+    >>> assertEqual(il1.account, advance_payment_account)
     >>> il1.unit_price
     Decimal('10.00')
-    >>> il1.taxes_date == today
-    True
+    >>> assertEqual(il1.taxes_date, today)
     >>> il1.quantity
     -1.0
-    >>> il2.product == product
-    True
+    >>> assertEqual(il2.product, product)
     >>> il2.unit_price
     Decimal('20.0000')
     >>> il2.quantity
     5.0
 
 Create another advance payment term preventing the packing stage::
 
@@ -244,24 +238,23 @@
     >>> shipment, = sale.shipments
 
 Let's try to pack it::
 
     >>> shipment.click('wait')
     >>> shipment.click('assign_try')
     >>> shipment.click('pick')
-    >>> shipment.click('pack')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> shipment.click('pack')
     Traceback (most recent call last):
         ...
     ShippingBlocked: ...
 
 Let's pay the advance payment invoice::
 
     >>> invoice, = sale.advance_payment_invoices
-    >>> invoice.invoice_date == next_week
-    True
+    >>> assertEqual(invoice.invoice_date, next_week)
     >>> invoice.invoice_date = None
     >>> invoice.click('post')
     >>> pay = invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> sale.reload()
     >>> sale.state
@@ -312,16 +305,15 @@
     >>> PurchaseRequest = Model.get('purchase.request')
     >>> PurchaseRequest.find()
     []
 
 The advance payment invoice has been created, now pay it::
 
     >>> invoice, = sale.advance_payment_invoices
-    >>> invoice.invoice_date == next_week
-    True
+    >>> assertEqual(invoice.invoice_date, next_week)
     >>> invoice.invoice_date = None
     >>> invoice.click('post')
     >>> pay = invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> sale.reload()
     >>> sale.state
@@ -400,16 +392,15 @@
 
     >>> handle_exception = sale.click('handle_invoice_exception')
     >>> handle_exception.execute('handle')
     >>> sale.reload()
     >>> _, inv_recreated = sale.advance_payment_invoices
     >>> inv_recreated.total_amount
     Decimal('10.00')
-    >>> inv_recreated.invoice_date == next_week
-    True
+    >>> assertEqual(inv_recreated.invoice_date, next_week)
     >>> inv_recreated.invoice_date = None
     >>> inv_recreated.click('post')
     >>> pay = inv_recreated.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> sale.reload()
     >>> last_invoice, = sale.invoices
```

### Comparing `trytond_sale_advance_payment-7.0.2/tests/scenario_sale_advance_payment_on_shipment.rst` & `trytond_sale_advance_payment-7.2.0/tests/scenario_sale_advance_payment_on_shipment.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 Sale Advance Payment On Shipment Scenario
 =========================================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.modules.sale_advance_payment.tests.tools import (
-    ...     create_advance_payment_term, add_advance_payment_accounts)
+    ...     add_advance_payment_accounts, create_advance_payment_term)
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('sale_advance_payment')
 
     >>> Journal = Model.get('account.journal')
     >>> Party = Model.get('party.party')
@@ -131,15 +130,15 @@
 
     >>> shipment, = sale.shipments
     >>> move, = shipment.inventory_moves
     >>> move.quantity = 5
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
 
     >>> sale.reload()
     >>> len(sale.shipments)
     2
     >>> len(sale.invoices)
     1
 
@@ -149,15 +148,15 @@
 
 Ship backorder::
 
     >>> _, shipment = sale.shipments
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
 
     >>> sale.reload()
     >>> len(sale.shipments)
     2
     >>> len(sale.invoices)
     2
```

### Comparing `trytond_sale_advance_payment-7.0.2/tests/tools.py` & `trytond_sale_advance_payment-7.2.0/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/tox.ini` & `trytond_sale_advance_payment-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/PKG-INFO` & `trytond_sale_advance_payment-7.2.0/trytond_sale_advance_payment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_advance_payment
-Version: 7.0.2
+Version: 7.2.0
 Summary: Tryton module for sale advance payment
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
@@ -49,21 +49,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: simpleeval
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_supply<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_supply<7.3,>=7.2; extra == "test"
 
 Sale Advance Payment Module
 ###########################
 
 The sale_advance_payment module adds support for advance payment management on
 the sale.
```

### Comparing `trytond_sale_advance_payment-7.0.2/trytond_sale_advance_payment.egg-info/SOURCES.txt` & `trytond_sale_advance_payment-7.2.0/trytond_sale_advance_payment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/view/advance_payment_condition_form.xml` & `trytond_sale_advance_payment-7.2.0/view/advance_payment_condition_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/view/advance_payment_term_line_form.xml` & `trytond_sale_advance_payment-7.2.0/view/advance_payment_term_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_advance_payment-7.0.2/view/sale_form.xml` & `trytond_sale_advance_payment-7.2.0/view/sale_form.xml`

 * *Files identical despite different names*

