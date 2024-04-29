# Comparing `tmp/trytond_purchase_shipment_cost-7.0.0.tar.gz` & `tmp/trytond_purchase_shipment_cost-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_shipment_cost-7.0.0.tar", last modified: Mon Oct 30 17:36:25 2023, max compression
+gzip compressed data, was "trytond_purchase_shipment_cost-7.2.0.tar", last modified: Mon Apr 29 15:46:39 2024, max compression
```

## Comparing `trytond_purchase_shipment_cost-7.0.0.tar` & `trytond_purchase_shipment_cost-7.2.0.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:25.343984 trytond_purchase_shipment_cost-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-22 17:23:15.000000 trytond_purchase_shipment_cost-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2114 2023-10-30 17:11:09.000000 trytond_purchase_shipment_cost-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      769 2023-10-30 17:11:09.000000 trytond_purchase_shipment_cost-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_shipment_cost-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3637 2023-10-30 17:36:25.343984 trytond_purchase_shipment_cost-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-01-16 14:00:21.000000 trytond_purchase_shipment_cost-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.0.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-01-16 14:00:21.000000 trytond_purchase_shipment_cost-7.0.0/carrier.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:25.340650 trytond_purchase_shipment_cost-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2823 2023-10-22 17:23:15.000000 trytond_purchase_shipment_cost-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-01-16 14:00:21.000000 trytond_purchase_shipment_cost-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:15.000000 trytond_purchase_shipment_cost-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:25.337317 trytond_purchase_shipment_cost-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1462 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1217 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1248 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1223 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1226 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1190 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1316 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1259 2023-10-30 16:47:45.000000 trytond_purchase_shipment_cost-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1263 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1502 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1079 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1126 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1252 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1142 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1248 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1034 2023-10-28 12:11:25.000000 trytond_purchase_shipment_cost-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:36:25.343984 trytond_purchase_shipment_cost-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4702 2023-10-27 17:38:49.000000 trytond_purchase_shipment_cost-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7130 2023-10-07 17:14:58.000000 trytond_purchase_shipment_cost-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      773 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:25.340650 trytond_purchase_shipment_cost-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4504 2023-08-13 15:26:13.000000 trytond_purchase_shipment_cost-7.0.0/tests/scenario_purchase_shipment_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4117 2023-06-10 11:39:56.000000 trytond_purchase_shipment_cost-7.0.0/tests/scenario_purchase_shipment_cost_invoice_stock.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6698 2023-08-13 15:26:13.000000 trytond_purchase_shipment_cost-7.0.0/tests/scenario_purchase_shipment_cost_with_account_stock.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6339 2023-10-07 17:14:58.000000 trytond_purchase_shipment_cost-7.0.0/tests/scenario_purchase_shipment_cost_with_account_stock_anglo_saxon.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_purchase_shipment_cost-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-10-30 17:11:05.000000 trytond_purchase_shipment_cost-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:25.343984 trytond_purchase_shipment_cost-7.0.0/trytond_purchase_shipment_cost.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3637 2023-10-30 17:36:24.000000 trytond_purchase_shipment_cost-7.0.0/trytond_purchase_shipment_cost.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2097 2023-10-30 17:36:25.000000 trytond_purchase_shipment_cost-7.0.0/trytond_purchase_shipment_cost.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:36:24.000000 trytond_purchase_shipment_cost-7.0.0/trytond_purchase_shipment_cost.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-10-30 17:36:24.000000 trytond_purchase_shipment_cost-7.0.0/trytond_purchase_shipment_cost.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_purchase_shipment_cost-7.0.0/trytond_purchase_shipment_cost.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-10-30 17:36:24.000000 trytond_purchase_shipment_cost-7.0.0/trytond_purchase_shipment_cost.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:36:24.000000 trytond_purchase_shipment_cost-7.0.0/trytond_purchase_shipment_cost.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:25.340650 trytond_purchase_shipment_cost-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-01-16 14:00:21.000000 trytond_purchase_shipment_cost-7.0.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.0.0/view/shipment_in_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.0.0/view/stock_move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:39.722993 trytond_purchase_shipment_cost-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2215 2024-04-29 15:24:21.000000 trytond_purchase_shipment_cost-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      769 2024-04-29 15:24:21.000000 trytond_purchase_shipment_cost-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase_shipment_cost-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3637 2024-04-29 15:46:39.722993 trytond_purchase_shipment_cost-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-01-16 14:00:21.000000 trytond_purchase_shipment_cost-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.2.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-01-16 14:00:21.000000 trytond_purchase_shipment_cost-7.2.0/carrier.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:39.719660 trytond_purchase_shipment_cost-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_purchase_shipment_cost-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-01-16 14:00:21.000000 trytond_purchase_shipment_cost-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:22.000000 trytond_purchase_shipment_cost-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:39.722993 trytond_purchase_shipment_cost-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1462 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1217 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1248 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1223 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1226 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1190 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1316 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1259 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1263 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1502 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1079 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1126 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1252 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1142 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1248 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1034 2024-04-27 16:43:26.000000 trytond_purchase_shipment_cost-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:46:39.722993 trytond_purchase_shipment_cost-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4702 2024-03-17 11:01:36.000000 trytond_purchase_shipment_cost-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7130 2024-02-04 18:51:26.000000 trytond_purchase_shipment_cost-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      773 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:39.722993 trytond_purchase_shipment_cost-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4476 2024-04-22 12:14:36.000000 trytond_purchase_shipment_cost-7.2.0/tests/scenario_purchase_shipment_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4094 2024-04-22 12:14:36.000000 trytond_purchase_shipment_cost-7.2.0/tests/scenario_purchase_shipment_cost_invoice_stock.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6429 2024-04-22 12:14:36.000000 trytond_purchase_shipment_cost-7.2.0/tests/scenario_purchase_shipment_cost_with_account_stock.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6335 2024-04-27 16:30:39.000000 trytond_purchase_shipment_cost-7.2.0/tests/scenario_purchase_shipment_cost_with_account_stock_anglo_saxon.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:22.000000 trytond_purchase_shipment_cost-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2024-04-29 15:24:16.000000 trytond_purchase_shipment_cost-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:39.722993 trytond_purchase_shipment_cost-7.2.0/trytond_purchase_shipment_cost.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3637 2024-04-29 15:46:39.000000 trytond_purchase_shipment_cost-7.2.0/trytond_purchase_shipment_cost.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2079 2024-04-29 15:46:39.000000 trytond_purchase_shipment_cost-7.2.0/trytond_purchase_shipment_cost.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:46:39.000000 trytond_purchase_shipment_cost-7.2.0/trytond_purchase_shipment_cost.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:46:39.000000 trytond_purchase_shipment_cost-7.2.0/trytond_purchase_shipment_cost.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_purchase_shipment_cost-7.2.0/trytond_purchase_shipment_cost.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2024-04-29 15:46:39.000000 trytond_purchase_shipment_cost-7.2.0/trytond_purchase_shipment_cost.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:46:39.000000 trytond_purchase_shipment_cost-7.2.0/trytond_purchase_shipment_cost.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:39.722993 trytond_purchase_shipment_cost-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-01-16 14:00:21.000000 trytond_purchase_shipment_cost-7.2.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      738 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.2.0/view/shipment_in_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-04-15 07:12:15.000000 trytond_purchase_shipment_cost-7.2.0/view/stock_move_form.xml
```

### Comparing `trytond_purchase_shipment_cost-7.0.0/CHANGELOG` & `trytond_purchase_shipment_cost-7.2.0/CHANGELOG`

 * *Files 0% similar despite different names*

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

### Comparing `trytond_purchase_shipment_cost-7.0.0/COPYRIGHT` & `trytond_purchase_shipment_cost-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Copyright (C) 2011-2023 Cédric Krier.
+Copyright (C) 2011-2024 Cédric Krier.
 Copyright (C) 2011-2020 Bertrand Chenal.
 Copyright (C) 2011-2023 Nicolas Évrard.
-Copyright (C) 2011-2023 B2CK SPRL.
+Copyright (C) 2011-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_purchase_shipment_cost-7.0.0/LICENSE` & `trytond_purchase_shipment_cost-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/PKG-INFO` & `trytond_purchase_shipment_cost-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_shipment_cost
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for purchase shipment cost
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
@@ -48,26 +48,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_cost<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_cost<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_stock_continental<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_stock_anglo_saxon<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_stock_continental<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_stock_anglo_saxon<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
 
 Purchase Shipment Cost Module
 #############################
 
 The purchase_shipment_cost module adds shipment cost to *Supplier Shipment*.
 
 One field is added to *Carrier*:
```

### Comparing `trytond_purchase_shipment_cost-7.0.0/README.rst` & `trytond_purchase_shipment_cost-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/carrier.py` & `trytond_purchase_shipment_cost-7.2.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/doc/conf.py` & `trytond_purchase_shipment_cost-7.2.0/doc/conf.py`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_purchase_shipment_cost-7.0.0/doc/index.rst` & `trytond_purchase_shipment_cost-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/bg.po` & `trytond_purchase_shipment_cost-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/ca.po` & `trytond_purchase_shipment_cost-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/cs.po` & `trytond_purchase_shipment_cost-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/de.po` & `trytond_purchase_shipment_cost-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/es.po` & `trytond_purchase_shipment_cost-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/es_419.po` & `trytond_purchase_shipment_cost-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/et.po` & `trytond_purchase_shipment_cost-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/fa.po` & `trytond_purchase_shipment_cost-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/fi.po` & `trytond_purchase_shipment_cost-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/fr.po` & `trytond_purchase_shipment_cost-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/hu.po` & `trytond_purchase_shipment_cost-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/id.po` & `trytond_purchase_shipment_cost-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/it.po` & `trytond_purchase_shipment_cost-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/lo.po` & `trytond_purchase_shipment_cost-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/lt.po` & `trytond_purchase_shipment_cost-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/nl.po` & `trytond_purchase_shipment_cost-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/pl.po` & `trytond_purchase_shipment_cost-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/pt.po` & `trytond_purchase_shipment_cost-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/ro.po` & `trytond_purchase_shipment_cost-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/ru.po` & `trytond_purchase_shipment_cost-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/sl.po` & `trytond_purchase_shipment_cost-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/tr.po` & `trytond_purchase_shipment_cost-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/uk.po` & `trytond_purchase_shipment_cost-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/locale/zh_CN.po` & `trytond_purchase_shipment_cost-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/setup.py` & `trytond_purchase_shipment_cost-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/stock.py` & `trytond_purchase_shipment_cost-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/stock.xml` & `trytond_purchase_shipment_cost-7.2.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/tests/scenario_purchase_shipment_cost.rst` & `trytond_purchase_shipment_cost-7.2.0/tests/scenario_purchase_shipment_cost.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ===============================
 Purchase Shipment Cost Scenario
 ===============================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('purchase_shipment_cost')
 
 Create company::
 
@@ -78,16 +78,15 @@
     >>> move.product = product
     >>> move.quantity = 50
     >>> move.unit_price = Decimal('8')
     >>> move.currency = company.currency
     >>> shipment.carrier = carrier
     >>> shipment.cost_used
     Decimal('3.0000')
-    >>> shipment.cost_currency_used == company.currency
-    True
+    >>> assertEqual(shipment.cost_currency_used, company.currency)
     >>> shipment.click('receive')
     >>> shipment.state
     'received'
     >>> move, = shipment.incoming_moves
     >>> move.unit_price
     Decimal('8.0600')
 
@@ -106,17 +105,16 @@
     ...     move.currency = company.currency
     >>> shipment.carrier = carrier
     >>> shipment.cost_used
     Decimal('3.0000')
     >>> shipment.click('receive')
     >>> shipment.state
     'received'
-    >>> [move.unit_price for move in shipment.incoming_moves] == \
-    ...     [Decimal('8.3334'), Decimal('8.3333'), Decimal('8.3333')]
-    True
+    >>> [move.unit_price for move in shipment.incoming_moves]
+    [Decimal('8.3334'), Decimal('8.3333'), Decimal('8.3333')]
 
 Receive a two lines with no cost::
 
     >>> shipment = ShipmentIn()
     >>> shipment.supplier = supplier
     >>> move = shipment.incoming_moves.new()
     >>> move.from_location = supplier_location
```

### Comparing `trytond_purchase_shipment_cost-7.0.0/tests/scenario_purchase_shipment_cost_invoice_stock.rst` & `trytond_purchase_shipment_cost-7.2.0/tests/scenario_purchase_shipment_cost_invoice_stock.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 ==================================================
 
 Imports::
 
     >>> import datetime as dt
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
+    >>> from trytond.tests.tools import activate_modules
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'purchase_shipment_cost',
```

### Comparing `trytond_purchase_shipment_cost-7.0.0/tests/scenario_purchase_shipment_cost_with_account_stock.rst` & `trytond_purchase_shipment_cost-7.2.0/tests/scenario_purchase_shipment_cost_with_account_stock.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 ==================================================
 Purchase Shipment Cost with Account Stock Scenario
 ==================================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
-    >>> from trytond.modules.account_stock_continental.tests.tools import \
-    ...     add_stock_accounts
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_stock_continental.tests.tools import (
+    ...     add_stock_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'purchase_shipment_cost',
     ...         'account_stock_continental',
     ...         ])
@@ -135,36 +133,32 @@
     >>> move.product = product_average
     >>> move.quantity = 20
     >>> move.unit_price = Decimal('8')
     >>> move.currency = company.currency
     >>> shipment.carrier = carrier
     >>> shipment.cost_used
     Decimal('3.0000')
-    >>> shipment.cost_currency_used == company.currency
-    True
+    >>> assertEqual(shipment.cost_currency_used, company.currency)
     >>> shipment.click('receive')
     >>> shipment.state
     'received'
     >>> move, move_average = shipment.incoming_moves
     >>> move.unit_price
     Decimal('8.0600')
     >>> move_average.unit_price
     Decimal('8.0600')
     >>> stock_in.reload()
-    >>> (stock_in.debit, stock_in.credit) == \
-    ...     (Decimal('0.00'), Decimal('398.20'))
-    True
+    >>> (stock_in.debit, stock_in.credit)
+    (Decimal('0.00'), Decimal('398.20'))
     >>> expense.reload()
-    >>> (expense.debit, expense.credit) == \
-    ...     (Decimal('0.00'), Decimal('3.00'))
-    True
+    >>> (expense.debit, expense.credit)
+    (Decimal('0.00'), Decimal('3.00'))
     >>> stock.reload()
-    >>> (stock.debit, stock.credit) == \
-    ...     (Decimal('401.20'), Decimal('0.00'))
-    True
+    >>> (stock.debit, stock.credit)
+    (Decimal('401.20'), Decimal('0.00'))
 
 Receive many product lines::
 
     >>> shipment = ShipmentIn()
     >>> shipment.supplier = supplier
     >>> for quantity in (1, 3, 5):
     ...     move = Move()
@@ -177,22 +171,18 @@
     ...     move.currency = company.currency
     >>> shipment.carrier = carrier
     >>> shipment.cost_used
     Decimal('3.0000')
     >>> shipment.click('receive')
     >>> shipment.state
     'received'
-    >>> [move.unit_price for move in shipment.incoming_moves] == \
-    ...     [Decimal('8.3334'), Decimal('8.3333'), Decimal('8.3333')]
-    True
+    >>> [move.unit_price for move in shipment.incoming_moves]
+    [Decimal('8.3334'), Decimal('8.3333'), Decimal('8.3333')]
     >>> stock_in.reload()
-    >>> (stock_in.debit, stock_in.credit) == \
-    ...     (Decimal('0.00'), Decimal('467.20'))
-    True
+    >>> (stock_in.debit, stock_in.credit)
+    (Decimal('0.00'), Decimal('467.20'))
     >>> expense.reload()
-    >>> (expense.debit, expense.credit) == \
-    ...     (Decimal('0.00'), Decimal('6.00'))
-    True
+    >>> (expense.debit, expense.credit)
+    (Decimal('0.00'), Decimal('6.00'))
     >>> stock.reload()
-    >>> (stock.debit, stock.credit) == \
-    ...     (Decimal('473.20'), Decimal('0.00'))
-    True
+    >>> (stock.debit, stock.credit)
+    (Decimal('473.20'), Decimal('0.00'))
```

### Comparing `trytond_purchase_shipment_cost-7.0.0/tests/scenario_purchase_shipment_cost_with_account_stock_anglo_saxon.rst` & `trytond_purchase_shipment_cost-7.2.0/tests/scenario_purchase_shipment_cost_with_account_stock_anglo_saxon.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 Purchase Shipment Cost with Account Stock Anglo-Saxon Scenario
 ==============================================================
 
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
-    >>> from trytond.modules.account_stock_continental.tests.tools import \
-    ...     add_stock_accounts
-    >>> from trytond.modules.account_stock_anglo_saxon.tests.tools import \
-    ...     add_cogs_accounts
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.account_stock_anglo_saxon.tests.tools import (
+    ...     add_cogs_accounts)
+    >>> from trytond.modules.account_stock_continental.tests.tools import (
+    ...     add_stock_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'purchase_shipment_cost',
@@ -146,23 +146,22 @@
     >>> shipment = ShipmentIn(supplier=supplier)
     >>> move = Move(purchase.moves[0].id)
     >>> move.quantity = 4.0
     >>> shipment.incoming_moves.append(move)
     >>> shipment.carrier = carrier
     >>> shipment.cost_used
     Decimal('3.0000')
-    >>> shipment.cost_currency_used == company.currency
-    True
+    >>> assertEqual(shipment.cost_currency_used, company.currency)
     >>> shipment.click('receive')
     >>> shipment.state
     'received'
     >>> move, = shipment.incoming_moves
     >>> move.unit_price
     Decimal('5.7500')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
     >>> stock_in.reload()
     >>> stock.reload()
     >>> stock_in.debit
     Decimal('0.00')
     >>> stock_in.credit
```

### Comparing `trytond_purchase_shipment_cost-7.0.0/tox.ini` & `trytond_purchase_shipment_cost-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_shipment_cost-7.0.0/trytond_purchase_shipment_cost.egg-info/PKG-INFO` & `trytond_purchase_shipment_cost-7.2.0/trytond_purchase_shipment_cost.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-purchase-shipment-cost
-Version: 7.0.0
+Name: trytond_purchase_shipment_cost
+Version: 7.2.0
 Summary: Tryton module for purchase shipment cost
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
@@ -48,26 +48,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_cost<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_cost<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_stock_continental<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_stock_anglo_saxon<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_stock_continental<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_stock_anglo_saxon<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
 
 Purchase Shipment Cost Module
 #############################
 
 The purchase_shipment_cost module adds shipment cost to *Supplier Shipment*.
 
 One field is added to *Carrier*:
```

### Comparing `trytond_purchase_shipment_cost-7.0.0/trytond_purchase_shipment_cost.egg-info/SOURCES.txt` & `trytond_purchase_shipment_cost-7.2.0/trytond_purchase_shipment_cost.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 carrier.py
```

### Comparing `trytond_purchase_shipment_cost-7.0.0/view/shipment_in_form.xml` & `trytond_purchase_shipment_cost-7.2.0/view/shipment_in_form.xml`

 * *Files identical despite different names*

