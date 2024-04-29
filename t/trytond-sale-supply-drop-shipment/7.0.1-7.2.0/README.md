# Comparing `tmp/trytond_sale_supply_drop_shipment-7.0.1.tar.gz` & `tmp/trytond_sale_supply_drop_shipment-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_supply_drop_shipment-7.0.1.tar", last modified: Mon Jan 15 23:15:17 2024, max compression
+gzip compressed data, was "trytond_sale_supply_drop_shipment-7.2.0.tar", last modified: Mon Apr 29 15:50:20 2024, max compression
```

## Comparing `trytond_sale_supply_drop_shipment-7.0.1.tar` & `trytond_sale_supply_drop_shipment-7.2.0.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:15:17.500504 trytond_sale_supply_drop_shipment-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      231 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2516 2024-01-15 23:15:14.000000 trytond_sale_supply_drop_shipment-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-01-15 23:15:14.000000 trytond_sale_supply_drop_shipment-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3725 2024-01-15 23:15:17.500504 trytond_sale_supply_drop_shipment-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      987 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      972 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:15:17.497171 trytond_sale_supply_drop_shipment-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2826 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      987 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:15:17.497171 trytond_sale_supply_drop_shipment-7.0.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/icons/tryton-shipment-drop.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:15:17.497171 trytond_sale_supply_drop_shipment-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7058 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7751 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6627 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7801 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7721 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6547 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6500 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7872 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6627 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7880 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6790 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6470 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7164 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6980 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6710 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7745 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6912 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7279 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6290 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7096 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7083 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6627 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6273 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6653 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      850 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1399 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1156 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8653 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2442 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4729 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1465 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-01-15 23:15:17.500504 trytond_sale_supply_drop_shipment-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4550 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22328 2024-01-08 11:29:26.000000 trytond_sale_supply_drop_shipment-7.0.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13353 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:15:17.497171 trytond_sale_supply_drop_shipment-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10896 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/tests/scenario_sale_supply_drop_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4466 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/tests/scenario_sale_supply_drop_shipment_on_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4053 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/tests/scenario_sale_supply_drop_shipment_remaining_qty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-30 17:55:12.000000 trytond_sale_supply_drop_shipment-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:15:17.500504 trytond_sale_supply_drop_shipment-7.0.1/trytond_sale_supply_drop_shipment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3725 2024-01-15 23:15:17.000000 trytond_sale_supply_drop_shipment-7.0.1/trytond_sale_supply_drop_shipment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2736 2024-01-15 23:15:17.000000 trytond_sale_supply_drop_shipment-7.0.1/trytond_sale_supply_drop_shipment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-01-15 23:15:17.000000 trytond_sale_supply_drop_shipment-7.0.1/trytond_sale_supply_drop_shipment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-01-15 23:15:17.000000 trytond_sale_supply_drop_shipment-7.0.1/trytond_sale_supply_drop_shipment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:12.000000 trytond_sale_supply_drop_shipment-7.0.1/trytond_sale_supply_drop_shipment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      235 2024-01-15 23:15:17.000000 trytond_sale_supply_drop_shipment-7.0.1/trytond_sale_supply_drop_shipment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-01-15 23:15:17.000000 trytond_sale_supply_drop_shipment-7.0.1/trytond_sale_supply_drop_shipment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:15:17.500504 trytond_sale_supply_drop_shipment-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/view/product_supplier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/view/purchase_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      806 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/view/purchase_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/view/purchase_request_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/view/purchase_request_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/view/sale_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1447 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/view/shipment_drop_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      629 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/view/shipment_drop_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/view/stock_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-10-30 17:06:38.000000 trytond_sale_supply_drop_shipment-7.0.1/view/stock_move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:20.090563 trytond_sale_supply_drop_shipment-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2633 2024-04-29 15:27:08.000000 trytond_sale_supply_drop_shipment-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:27:08.000000 trytond_sale_supply_drop_shipment-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3787 2024-04-29 15:50:20.090563 trytond_sale_supply_drop_shipment-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      987 2024-01-27 09:58:52.000000 trytond_sale_supply_drop_shipment-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1282 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:20.087230 trytond_sale_supply_drop_shipment-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3088 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      987 2024-01-27 09:58:52.000000 trytond_sale_supply_drop_shipment-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:30.000000 trytond_sale_supply_drop_shipment-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:20.087230 trytond_sale_supply_drop_shipment-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/icons/tryton-shipment-drop.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:20.087230 trytond_sale_supply_drop_shipment-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7058 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7751 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6627 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7801 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7721 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6547 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6500 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7872 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6627 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7880 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6790 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6470 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7164 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6980 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6710 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7745 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6912 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7279 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6290 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7096 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7083 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6627 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6273 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6653 2024-04-27 16:43:27.000000 trytond_sale_supply_drop_shipment-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1033 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1399 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1156 2024-04-13 17:12:23.000000 trytond_sale_supply_drop_shipment-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8653 2024-01-27 09:58:52.000000 trytond_sale_supply_drop_shipment-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2442 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-7.2.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4729 2024-01-27 09:58:52.000000 trytond_sale_supply_drop_shipment-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1465 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:50:20.090563 trytond_sale_supply_drop_shipment-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4609 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24025 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13541 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:20.087230 trytond_sale_supply_drop_shipment-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10842 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/tests/scenario_sale_supply_drop_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4426 2024-04-22 12:14:36.000000 trytond_sale_supply_drop_shipment-7.2.0/tests/scenario_sale_supply_drop_shipment_on_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4042 2024-04-22 12:14:36.000000 trytond_sale_supply_drop_shipment-7.2.0/tests/scenario_sale_supply_drop_shipment_remaining_qty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4188 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/tests/scenario_sale_supply_drop_shipment_split.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:30.000000 trytond_sale_supply_drop_shipment-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2024-04-29 15:27:04.000000 trytond_sale_supply_drop_shipment-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:20.090563 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3787 2024-04-29 15:50:19.000000 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2892 2024-04-29 15:50:20.000000 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:50:19.000000 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:50:19.000000 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2024-04-29 15:50:19.000000 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:50:19.000000 trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:20.090563 trytond_sale_supply_drop_shipment-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-7.2.0/view/product_supplier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-7.2.0/view/purchase_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      806 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/view/purchase_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-7.2.0/view/purchase_request_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/view/purchase_request_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-01-16 14:00:21.000000 trytond_sale_supply_drop_shipment-7.2.0/view/sale_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1445 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/view/shipment_drop_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      297 2024-04-27 16:30:39.000000 trytond_sale_supply_drop_shipment-7.2.0/view/shipment_drop_split_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      629 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/view/shipment_drop_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/view/stock_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_sale_supply_drop_shipment-7.2.0/view/stock_move_form.xml
```

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/CHANGELOG` & `trytond_sale_supply_drop_shipment-7.2.0/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 
-Version 7.0.1 - 2024-01-15
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
-
+* Support splitting drop shipment
+* Split customer moves when splitting supplier moves
+* Rename 'done' button to 'do'
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 * Check customer product quantities for drop shipment
```

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/COPYRIGHT` & `trytond_sale_supply_drop_shipment-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2011-2023 Cédric Krier.
-Copyright (C) 2011-2023 B2CK SPRL.
+Copyright (C) 2011-2024 Cédric Krier.
+Copyright (C) 2011-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/LICENSE` & `trytond_sale_supply_drop_shipment-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/PKG-INFO` & `trytond_sale_supply_drop_shipment-7.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_supply_drop_shipment
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for sale supply drop shipment
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
@@ -48,24 +48,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond_purchase_request<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_sale_supply<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond_purchase_request<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_sale_supply<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_split<7.3,>=7.2; extra == "test"
 
 Sale Supply Drop Shipment Model
 ###############################
 
 The Sale Supply Drop Shipment module adds a drop shipment option on product
 supplier if "supply on request" is selected.
 When selected, the purchase request and the linked purchase have the address of
```

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/README.rst` & `trytond_sale_supply_drop_shipment-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/doc/conf.py` & `trytond_sale_supply_drop_shipment-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/doc/index.rst` & `trytond_sale_supply_drop_shipment-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/icons/LICENSE` & `trytond_sale_supply_drop_shipment-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/icons/tryton-shipment-drop.svg` & `trytond_sale_supply_drop_shipment-7.2.0/icons/tryton-shipment-drop.svg`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/bg.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/ca.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/cs.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/de.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/es.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/es_419.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/et.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/fa.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/fi.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/fr.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/hu.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/id.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/it.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/lo.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/lt.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/nl.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/pl.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/pt.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/ro.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/ru.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/sl.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/tr.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/uk.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/locale/zh_CN.po` & `trytond_sale_supply_drop_shipment-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/message.xml` & `trytond_sale_supply_drop_shipment-7.2.0/message.xml`

 * *Files 8% similar despite different names*

#### Comparing `trytond_sale_supply_drop_shipment-7.0.1/message.xml` & `trytond_sale_supply_drop_shipment-7.2.0/message.xml`

```diff
@@ -8,9 +8,12 @@
     </record>
     <record model="ir.message" id="msg_reset_move">
       <field name="text">You cannot reset move &quot;%(move)s&quot; to draft because it was generated by a sale or a purchase.</field>
     </record>
     <record model="ir.message" id="msg_drop_shipment_delete_cancel">
       <field name="text">To delete drop shipment &quot;%(shipment)s&quot; you must cancel it.</field>
     </record>
+    <record model="ir.message" id="msg_move_split_drop">
+      <field name="text">To split move from drop shipment, you must use the split wizard.</field>
+    </record>
   </data>
 </tryton>
```

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/party.py` & `trytond_sale_supply_drop_shipment-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/product.py` & `trytond_sale_supply_drop_shipment-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/purchase.py` & `trytond_sale_supply_drop_shipment-7.2.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/purchase.xml` & `trytond_sale_supply_drop_shipment-7.2.0/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/sale.py` & `trytond_sale_supply_drop_shipment-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/sale.xml` & `trytond_sale_supply_drop_shipment-7.2.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/setup.py` & `trytond_sale_supply_drop_shipment-7.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,18 @@
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
-tests_require = [get_require_version('proteus')]
+tests_require = [
+    get_require_version('proteus'),
+    get_require_version('trytond_stock_split'),
+    ]
 
 setup(name=name,
     version=version,
     description='Tryton module for sale supply drop shipment',
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
```

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/stock.py` & `trytond_sale_supply_drop_shipment-7.2.0/stock.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from trytond.model.exceptions import AccessError
 from trytond.modules.product import round_price
 from trytond.modules.purchase.stock import process_purchase
 from trytond.modules.sale.stock import process_sale
 from trytond.modules.stock.shipment import ShipmentCheckQuantity, ShipmentMixin
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval, Id, If
-from trytond.tools import grouped_slice
 from trytond.transaction import Transaction
 
 
 class Configuration(metaclass=PoolMeta):
     __name__ = 'stock.configuration'
 
     shipment_drop_sequence = fields.MultiValue(fields.Many2One(
@@ -200,15 +199,15 @@
                     'invisible': Eval('state') != 'draft',
                     'depends': ['state'],
                     },
                 'ship': {
                     'invisible': Eval('state') != 'waiting',
                     'depends': ['state'],
                     },
-                'done': {
+                'do': {
                     'invisible': Eval('state') != 'shipped',
                     'depends': ['state'],
                     },
                 })
 
     @classmethod
     def order_effective_date(cls, tables):
@@ -298,17 +297,17 @@
         Move = pool.get('stock.move')
 
         cls.cancel(shipments)
         for shipment in shipments:
             if shipment.state != 'cancelled':
                 raise AccessError(
                     gettext('sale_supply_drop_shipment'
-                        '.msg_drop_shipment_delete_cancel') % {
-                        'shipment': shipment.rec_name,
-                        })
+                        '.msg_drop_shipment_delete_cancel',
+                        shipment=shipment.rec_name,
+                        ))
         Move.delete([m for s in shipments for m in s.supplier_moves])
         super(ShipmentDrop, cls).delete(shipments)
 
     @classmethod
     @ModelView.button
     @Workflow.transition('cancelled')
     @process_sale('customer_moves')
@@ -464,45 +463,27 @@
             Move.save(to_save)
 
     @classmethod
     @ModelView.button
     @Workflow.transition('waiting')
     def wait(cls, shipments):
         pool = Pool()
-        PurchaseRequest = pool.get('purchase.request')
-        SaleLine = pool.get('sale.line')
+        PurchaseLine = pool.get('purchase.line')
         Move = pool.get('stock.move')
 
-        requests = []
-        for sub_lines in grouped_slice([m.origin.id for s in shipments
-                    for m in s.supplier_moves if m.origin]):
-            requests += PurchaseRequest.search([
-                    ('purchase_line', 'in', list(sub_lines)),
-                    ])
-        pline2requests = defaultdict(list)
-        for request in requests:
-            pline2requests[request.purchase_line].append(request)
-        sale_lines = []
-        for sub_requests in grouped_slice([r.id for r in requests]):
-            sale_lines += SaleLine.search([
-                    ('purchase_request', 'in', list(sub_requests)),
-                    ])
-        request2slines = defaultdict(list)
-        for sale_line in sale_lines:
-            request2slines[sale_line.purchase_request].append(sale_line)
-
         to_save = []
         for shipment in shipments:
             for s_move in shipment.supplier_moves:
-                if not s_move.origin:
+                if not isinstance(s_move.origin, PurchaseLine):
                     continue
-                for request in pline2requests[s_move.origin]:
-                    for sale_line in request2slines[request]:
+                p_line = s_move.origin
+                for request in p_line.requests:
+                    for sale_line in request.sale_lines:
                         for c_move in sale_line.moves:
-                            if (c_move.state not in ('cancelled', 'done')
+                            if (c_move.state not in {'cancelled', 'done'}
                                     and not c_move.shipment
                                     and c_move.from_location.type == 'drop'):
                                 c_move.shipment = shipment
                                 c_move.origin_drop = s_move
                                 to_save.append(c_move)
         Move.save(to_save)
         Move.draft(to_save)
@@ -519,15 +500,15 @@
         Move.do([m for s in shipments for m in s.supplier_moves])
         cls._synchronize_moves(shipments)
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
     @process_sale('customer_moves')
-    def done(cls, shipments):
+    def do(cls, shipments):
         pool = Pool()
         Move = pool.get('stock.move')
         Date = pool.get('ir.date')
         cls.set_cost(shipments)
         customer_moves, to_delete = [], []
         for shipment in shipments:
             shipment.check_quantity()
@@ -550,14 +531,55 @@
         return self.supplier_moves
 
     @property
     def _check_quantity_target_moves(self):
         return self.customer_moves
 
 
+class ShipmentDropSplit(metaclass=PoolMeta):
+    __name__ = 'stock.shipment.drop'
+
+    @classmethod
+    def __setup__(cls):
+        super().__setup__()
+        cls._buttons.update({
+                'split_wizard': {
+                    'readonly': Eval('state') != 'draft',
+                    'invisible': Eval('state') != 'draft',
+                    'depends': ['state'],
+                    },
+                })
+
+    @classmethod
+    @ModelView.button_action('stock_split.wizard_split_shipment')
+    def split_wizard(cls, shipments):
+        pass
+
+
+class SplitShipment(metaclass=PoolMeta):
+    __name__ = 'stock.shipment.split'
+
+    def get_moves(self, shipment):
+        moves = super().get_moves(shipment)
+        if shipment.__name__ == 'stock.shipment.drop':
+            moves = shipment.supplier_moves
+        return moves
+
+    def transition_split(self):
+        shipment = self.record
+        if shipment.__name__ == 'stock.shipment.drop':
+            customer_moves = []
+            for move in self.start.moves:
+                customer_moves.extend(move.moves_drop)
+            self.start.moves = [*self.start.moves, *customer_moves]
+            self.start.domain_moves = [
+                 *self.start.domain_moves, *customer_moves]
+        return super().transition_split()
+
+
 class Move(metaclass=PoolMeta):
     __name__ = 'stock.move'
 
     origin_drop = fields.Many2One(
         'stock.move', "Drop Origin", readonly=True,
         domain=[
             ('shipment', '=', Eval('shipment', -1)),
@@ -603,10 +625,41 @@
                 *clause[1:3], 'sale.line', *clause[3:]),
             ('origin.purchase.customer' + clause[0][len(name):],
                 *clause[1:3], 'purchase.line', *clause[3:]),
             ]
 
     @classmethod
     def copy(cls, moves, default=None):
+        context = Transaction().context
+        if (context.get('_stock_move_split')
+                and not context.get('_stock_move_split_drop')):
+            for move in moves:
+                if move.moves_drop:
+                    raise AccessError(
+                        gettext('sale_supply_drop_shipment'
+                            '.msg_move_split_drop'))
         default = default.copy() if default is not None else {}
         default.setdefault('moves_drop')
         return super().copy(moves, default=default)
+
+
+class MoveSplit(metaclass=PoolMeta):
+    __name__ = 'stock.move'
+
+    def split(self, quantity, unit, count=None):
+        with Transaction().set_context(_stock_move_split_drop=True):
+            moves = super().split(quantity, unit, count=count)
+        if self.moves_drop:
+            to_save = []
+            moves_drop = list(self.moves_drop)
+            for move in moves:
+                remainder = move.quantity
+                while remainder > 0 and moves_drop:
+                    move_drop = moves_drop.pop(0)
+                    splits = move_drop.split(remainder, move.unit, count=1)
+                    move_drop.origin_drop = move
+                    remainder -= move_drop.quantity
+                    to_save.append(move_drop)
+                    splits.remove(move_drop)
+                    moves_drop.extend(splits)
+            self.__class__.save(to_save)
+        return moves
```

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/stock.xml` & `trytond_sale_supply_drop_shipment-7.2.0/stock.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_sale_supply_drop_shipment-7.0.1/stock.xml` & `trytond_sale_supply_drop_shipment-7.2.0/stock.xml`

```diff
@@ -77,86 +77,86 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_shipment_drop_form"/>
     </record>
     <menuitem parent="stock.menu_shipment" sequence="10" action="act_shipment_drop_form" id="menu_shipment_drop_form"/>
     <record model="ir.model.access" id="access_shipment_drop">
-      <field name="model" search="[('model', '=', 'stock.shipment.drop')]"/>
+      <field name="model">stock.shipment.drop</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_shipment_drop_group_stock">
-      <field name="model" search="[('model', '=', 'stock.shipment.drop')]"/>
+      <field name="model">stock.shipment.drop</field>
       <field name="group" ref="stock.group_stock"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_shipment_drop_group_stock_admin">
-      <field name="model" search="[('model', '=', 'stock.shipment.drop')]"/>
+      <field name="model">stock.shipment.drop</field>
       <field name="group" ref="stock.group_stock_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_shipment_drop_group_sale">
-      <field name="model" search="[('model', '=', 'stock.shipment.drop')]"/>
+      <field name="model">stock.shipment.drop</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_shipment_drop_group_purchase">
-      <field name="model" search="[('model', '=', 'stock.shipment.drop')]"/>
+      <field name="model">stock.shipment.drop</field>
       <field name="group" ref="purchase.group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.button" id="shipment_drop_cancel_button">
+      <field name="model">stock.shipment.drop</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'stock.shipment.drop')]"/>
     </record>
     <record model="ir.model.button-res.group" id="shipment_drop_cancel_button_group_stock">
       <field name="button" ref="shipment_drop_cancel_button"/>
       <field name="group" ref="stock.group_stock"/>
     </record>
     <record model="ir.model.button" id="shipment_drop_draft_button">
+      <field name="model">stock.shipment.drop</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'stock.shipment.drop')]"/>
     </record>
     <record model="ir.model.button" id="shipment_drop_wait_button">
+      <field name="model">stock.shipment.drop</field>
       <field name="name">wait</field>
       <field name="string">Wait</field>
-      <field name="model" search="[('model', '=', 'stock.shipment.drop')]"/>
     </record>
     <record model="ir.model.button" id="shipment_drop_done_button">
-      <field name="name">done</field>
-      <field name="string">Done</field>
+      <field name="model">stock.shipment.drop</field>
+      <field name="name">do</field>
+      <field name="string">Complete</field>
       <field name="confirm">Are you sure you want to complete the shipment?</field>
-      <field name="model" search="[('model', '=', 'stock.shipment.drop')]"/>
     </record>
     <record model="ir.model.button" id="shipment_drop_ship_button">
+      <field name="model">stock.shipment.drop</field>
       <field name="name">ship</field>
       <field name="string">Ship</field>
       <field name="confirm">Are you sure you want to ship the shipment?</field>
-      <field name="model" search="[('model', '=', 'stock.shipment.drop')]"/>
     </record>
     <record model="ir.rule.group" id="rule_group_shipment_drop_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'stock.shipment.drop')]"/>
+      <field name="model">stock.shipment.drop</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_shipment_drop_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_shipment_drop_companies"/>
     </record>
     <record model="ir.action.act_window" id="act_shipment_drop_relate_party">
@@ -216,14 +216,26 @@
     </record>
     <record model="ir.ui.view" id="stock_move_view_form">
       <field name="model">stock.move</field>
       <field name="inherit" ref="stock.move_view_form"/>
       <field name="name">stock_move_form</field>
     </record>
   </data>
+  <data depends="stock_split">
+    <record model="ir.ui.view" id="shipment_drop_view_form_split">
+      <field name="model">stock.shipment.drop</field>
+      <field name="inherit" ref="shipment_drop_view_form"/>
+      <field name="name">shipment_drop_split_form</field>
+    </record>
+    <record model="ir.model.button" id="shipment_drop_split_wizard_button">
+      <field name="model">stock.shipment.drop</field>
+      <field name="name">split_wizard</field>
+      <field name="string">Split</field>
+    </record>
+  </data>
   <data noupdate="1">
     <!-- Default locations -->
     <record model="stock.location" id="location_drop">
       <field name="name">Drop</field>
       <field name="code">DROP</field>
       <field name="type">drop</field>
     </record>
```

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/tests/scenario_sale_supply_drop_shipment.rst` & `trytond_sale_supply_drop_shipment-7.2.0/tests/scenario_sale_supply_drop_shipment.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ==================================
 Sale Supply Drop Shipment Scenario
 ==================================
 
 Imports::
 
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, set_user
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'sale_supply_drop_shipment',
     ...         'sale',
@@ -167,18 +167,16 @@
     >>> PurchaseRequest = Model.get('purchase.request')
     >>> purchase_request, = PurchaseRequest.find()
     >>> purchase_request.quantity
     250.0
     >>> create_purchase = Wizard('purchase.request.create_purchase',
     ...     [purchase_request])
     >>> purchase, = Purchase.find()
-    >>> purchase.customer == customer
-    True
-    >>> purchase.delivery_address == sale.shipment_address
-    True
+    >>> assertEqual(purchase.customer, customer)
+    >>> assertEqual(purchase.delivery_address, sale.shipment_address)
     >>> purchase.payment_term = payment_term
     >>> purchase_line, = purchase.lines
     >>> purchase_line.unit_price = Decimal('3.0000')
     >>> purchase.click('quote')
     >>> purchase.click('confirm')
     >>> purchase.state
     'processing'
@@ -209,15 +207,15 @@
     []
     >>> len(sale.drop_shipments)
     2
     >>> shipment, = [s for s in sale.drop_shipments
     ...     if s.state == 'shipped']
 
     >>> set_user(stock_user)
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
     >>> move, = shipment.customer_moves
     >>> move.cost_price
     Decimal('3.0000')
     >>> set_user(sale_user)
     >>> sale.reload()
@@ -362,13 +360,13 @@
 
     >>> shipment, = sale.shipments
 
     >>> set_user(stock_user)
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
 
     >>> set_user(sale_user)
     >>> sale.reload()
     >>> sale.shipment_state
     'sent'
```

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/tests/scenario_sale_supply_drop_shipment_on_invoice.rst` & `trytond_sale_supply_drop_shipment-7.2.0/tests/scenario_sale_supply_drop_shipment_on_invoice.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Sale Supply Drop Shipment on Invoice Scenario
 =============================================
 
 Imports::
 
     >>> import datetime
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
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
 
 Activate modules::
 
     >>> config = activate_modules('sale_supply_drop_shipment')
 
 Create company::
```

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/tests/scenario_sale_supply_drop_shipment_remaining_qty.rst` & `trytond_sale_supply_drop_shipment-7.2.0/tests/scenario_sale_supply_drop_shipment_remaining_qty.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Sale Supply Drop Shipment Scenario
 ==================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'sale_supply_drop_shipment',
     ...         'sale',
     ...         'purchase',
```

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/tox.ini` & `trytond_sale_supply_drop_shipment-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/trytond_sale_supply_drop_shipment.egg-info/PKG-INFO` & `trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-sale-supply-drop-shipment
-Version: 7.0.1
+Name: trytond_sale_supply_drop_shipment
+Version: 7.2.0
 Summary: Tryton module for sale supply drop shipment
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
@@ -48,24 +48,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond_purchase_request<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_sale_supply<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond_purchase_request<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_sale_supply<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_split<7.3,>=7.2; extra == "test"
 
 Sale Supply Drop Shipment Model
 ###############################
 
 The Sale Supply Drop Shipment module adds a drop shipment option on product
 supplier if "supply on request" is selected.
 When selected, the purchase request and the linked purchase have the address of
```

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/trytond_sale_supply_drop_shipment.egg-info/SOURCES.txt` & `trytond_sale_supply_drop_shipment-7.2.0/trytond_sale_supply_drop_shipment.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 message.xml
@@ -55,25 +54,27 @@
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_sale_supply_drop_shipment.rst
 ./tests/scenario_sale_supply_drop_shipment_on_invoice.rst
 ./tests/scenario_sale_supply_drop_shipment_remaining_qty.rst
+./tests/scenario_sale_supply_drop_shipment_split.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/party_form.xml
 ./view/product_supplier_form.xml
 ./view/purchase_configuration_form.xml
 ./view/purchase_form.xml
 ./view/purchase_request_form.xml
 ./view/purchase_request_tree.xml
 ./view/sale_configuration_form.xml
 ./view/sale_form.xml
 ./view/shipment_drop_form.xml
+./view/shipment_drop_split_form.xml
 ./view/shipment_drop_tree.xml
 ./view/stock_configuration_form.xml
 ./view/stock_move_form.xml
 doc/conf.py
 doc/index.rst
 doc/requirements-doc.txt
 icons/LICENSE
@@ -102,14 +103,15 @@
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_sale_supply_drop_shipment.rst
 tests/scenario_sale_supply_drop_shipment_on_invoice.rst
 tests/scenario_sale_supply_drop_shipment_remaining_qty.rst
+tests/scenario_sale_supply_drop_shipment_split.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_sale_supply_drop_shipment.egg-info/PKG-INFO
 trytond_sale_supply_drop_shipment.egg-info/SOURCES.txt
 trytond_sale_supply_drop_shipment.egg-info/dependency_links.txt
 trytond_sale_supply_drop_shipment.egg-info/entry_points.txt
 trytond_sale_supply_drop_shipment.egg-info/not-zip-safe
@@ -120,10 +122,11 @@
 view/purchase_configuration_form.xml
 view/purchase_form.xml
 view/purchase_request_form.xml
 view/purchase_request_tree.xml
 view/sale_configuration_form.xml
 view/sale_form.xml
 view/shipment_drop_form.xml
+view/shipment_drop_split_form.xml
 view/shipment_drop_tree.xml
 view/stock_configuration_form.xml
 view/stock_move_form.xml
```

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/view/purchase_form.xml` & `trytond_sale_supply_drop_shipment-7.2.0/view/purchase_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/view/sale_form.xml` & `trytond_sale_supply_drop_shipment-7.2.0/view/sale_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/view/shipment_drop_form.xml` & `trytond_sale_supply_drop_shipment-7.2.0/view/shipment_drop_form.xml`

 * *Files 7% similar despite different names*

#### Comparing `trytond_sale_supply_drop_shipment-7.0.1/view/shipment_drop_form.xml` & `trytond_sale_supply_drop_shipment-7.2.0/view/shipment_drop_form.xml`

```diff
@@ -31,10 +31,10 @@
   <label name="state"/>
   <field name="state"/>
   <group col="-1" colspan="2" id="buttons">
     <button name="cancel" icon="tryton-cancel"/>
     <button name="draft"/>
     <button name="wait" icon="tryton-forward"/>
     <button name="ship" icon="tryton-forward"/>
-    <button name="done" icon="tryton-ok"/>
+    <button name="do" icon="tryton-ok"/>
   </group>
 </form>
```

### Comparing `trytond_sale_supply_drop_shipment-7.0.1/view/shipment_drop_tree.xml` & `trytond_sale_supply_drop_shipment-7.2.0/view/shipment_drop_tree.xml`

 * *Files identical despite different names*

