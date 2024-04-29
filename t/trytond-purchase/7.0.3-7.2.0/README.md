# Comparing `tmp/trytond_purchase-7.0.3.tar.gz` & `tmp/trytond_purchase-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase-7.0.3.tar", last modified: Wed Apr 17 10:40:49 2024, max compression
+gzip compressed data, was "trytond_purchase-7.2.0.tar", last modified: Mon Apr 29 15:45:08 2024, max compression
```

## Comparing `trytond_purchase-7.0.3.tar` & `trytond_purchase-7.2.0.tar`

### file list

```diff
@@ -1,121 +1,123 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.381936 trytond_purchase-7.0.3/
--rw-r--r--   0 ced       (1000) ced       (1000)     7291 2024-04-17 10:40:46.000000 trytond_purchase-7.0.3/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-17 10:40:46.000000 trytond_purchase-7.0.3/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-17 10:40:49.381936 trytond_purchase-7.0.3/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1909 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3581 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2554 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.371937 trytond_purchase-7.0.3/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2787 2024-03-03 16:24:20.000000 trytond_purchase-7.0.3/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7482 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.375270 trytond_purchase-7.0.3/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      208 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2000 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/doc/usage/prepurchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4855 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2027 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/doc/usage/returns.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.375270 trytond_purchase-7.0.3/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/icons/tryton-purchase.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     5622 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1761 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.375270 trytond_purchase-7.0.3/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    37669 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37866 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32868 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38333 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38062 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32388 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34581 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39805 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32855 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38221 2024-01-26 17:57:52.000000 trytond_purchase-7.0.3/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36910 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33506 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36150 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37669 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35653 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38239 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34203 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35891 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32093 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38224 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37603 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32846 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31183 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36322 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4337 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3677 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1160 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    21315 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    77930 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/purchase.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    83768 2024-04-12 17:44:57.000000 trytond_purchase-7.0.3/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    30912 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11639 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/purchase_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24226 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/purchase_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:40:49.381936 trytond_purchase-7.0.3/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4577 2024-03-03 16:24:03.000000 trytond_purchase-7.0.3/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8582 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4823 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.378603 trytond_purchase-7.0.3/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19200 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1676 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase_copy_product_suppliers.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1564 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase_default_taxes.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1332 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase_empty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2463 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase_manual_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3064 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase_modify_header.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5191 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2999 2024-02-05 16:24:27.000000 trytond_purchase-7.0.3/tests/scenario_purchase_return_wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5595 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2024-04-04 07:50:42.000000 trytond_purchase-7.0.3/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.381936 trytond_purchase-7.0.3/trytond_purchase.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-17 10:40:48.000000 trytond_purchase-7.0.3/trytond_purchase.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     4959 2024-04-17 10:40:49.000000 trytond_purchase-7.0.3/trytond_purchase.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:40:48.000000 trytond_purchase-7.0.3/trytond_purchase.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-04-17 10:40:48.000000 trytond_purchase-7.0.3/trytond_purchase.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:00.000000 trytond_purchase-7.0.3/trytond_purchase.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-17 10:40:48.000000 trytond_purchase-7.0.3/trytond_purchase.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:40:48.000000 trytond_purchase-7.0.3/trytond_purchase.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:49.381936 trytond_purchase-7.0.3/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/handle_invoice_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/handle_shipment_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/modify_header_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      482 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/move_list_shipment_in.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/product_list_purchase_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/product_supplier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/product_supplier_price_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/product_supplier_price_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/product_supplier_price_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/product_supplier_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/product_supplier_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3543 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1818 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      741 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      544 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_main_graph_expense.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_main_time_series_graph_expense.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_reporting_supplier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/purchase_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/return_purchase_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-10-30 17:06:38.000000 trytond_purchase-7.0.3/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.278719 trytond_purchase-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7140 2024-04-29 15:23:24.000000 trytond_purchase-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:23:23.000000 trytond_purchase-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_purchase-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-29 15:45:08.278719 trytond_purchase-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1909 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3581 2024-01-27 09:58:52.000000 trytond_purchase-7.2.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2508 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.272052 trytond_purchase-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7482 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:20.000000 trytond_purchase-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.272052 trytond_purchase-7.2.0/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      232 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2000 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/doc/usage/prepurchase.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5036 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/doc/usage/process.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2027 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/doc/usage/returns.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      460 2024-02-04 18:51:26.000000 trytond_purchase-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.272052 trytond_purchase-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      471 2023-01-16 14:00:21.000000 trytond_purchase-7.2.0/icons/tryton-purchase.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5999 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1715 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.272052 trytond_purchase-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    37791 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37990 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32968 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38450 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38189 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32498 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34685 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39922 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32955 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38334 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37020 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33611 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36267 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37779 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35762 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38352 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34308 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36009 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38395 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38348 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37703 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32946 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31266 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36435 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4336 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3698 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1146 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    20794 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2024-01-27 09:58:52.000000 trytond_purchase-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    77247 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/purchase.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    87914 2024-04-29 13:17:17.000000 trytond_purchase-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31720 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11639 2024-03-17 11:01:36.000000 trytond_purchase-7.2.0/purchase_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23812 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/purchase_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:45:08.278719 trytond_purchase-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4577 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8934 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4754 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.275385 trytond_purchase-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19177 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/tests/scenario_purchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1678 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_copy_product_suppliers.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1581 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_default_taxes.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1285 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_empty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2794 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_line_cancelled.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2509 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_line_cancelled_on_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2448 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_manual_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3040 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_modify_header.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5169 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3003 2024-04-22 12:14:36.000000 trytond_purchase-7.2.0/tests/scenario_purchase_return_wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5595 2024-02-04 18:51:26.000000 trytond_purchase-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:20.000000 trytond_purchase-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2024-04-29 15:23:19.000000 trytond_purchase-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.278719 trytond_purchase-7.2.0/trytond_purchase.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-29 15:45:07.000000 trytond_purchase-7.2.0/trytond_purchase.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     5171 2024-04-29 15:45:08.000000 trytond_purchase-7.2.0/trytond_purchase.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:45:07.000000 trytond_purchase-7.2.0/trytond_purchase.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-04-29 15:45:07.000000 trytond_purchase-7.2.0/trytond_purchase.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_purchase-7.2.0/trytond_purchase.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-29 15:45:07.000000 trytond_purchase-7.2.0/trytond_purchase.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:45:07.000000 trytond_purchase-7.2.0/trytond_purchase.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:45:08.278719 trytond_purchase-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2023-01-16 14:00:21.000000 trytond_purchase-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/handle_invoice_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/handle_shipment_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-01-16 14:00:21.000000 trytond_purchase-7.2.0/view/modify_header_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      482 2024-02-04 18:51:26.000000 trytond_purchase-7.2.0/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/move_list_shipment_in.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-01-27 09:58:52.000000 trytond_purchase-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2023-01-16 14:00:21.000000 trytond_purchase-7.2.0/view/product_list_purchase_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-02-04 18:51:26.000000 trytond_purchase-7.2.0/view/product_supplier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-02-04 18:51:26.000000 trytond_purchase-7.2.0/view/product_supplier_price_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-02-04 18:51:26.000000 trytond_purchase-7.2.0/view/product_supplier_price_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2024-02-04 18:51:26.000000 trytond_purchase-7.2.0/view/product_supplier_price_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/product_supplier_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/product_supplier_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3651 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/view/purchase_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1860 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      918 2024-04-27 16:30:39.000000 trytond_purchase-7.2.0/view/purchase_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      589 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      544 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_reporting_main_graph_expense.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-01-27 09:58:52.000000 trytond_purchase-7.2.0/view/purchase_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_reporting_main_time_series_graph_expense.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-01-27 09:58:52.000000 trytond_purchase-7.2.0/view/purchase_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_reporting_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_reporting_supplier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      656 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/purchase_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/return_purchase_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2024-01-27 09:58:52.000000 trytond_purchase-7.2.0/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-04-15 07:12:15.000000 trytond_purchase-7.2.0/view/template_tree.xml
```

### Comparing `trytond_purchase-7.0.3/CHANGELOG` & `trytond_purchase-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,12 @@
 
-Version 7.0.3 - 2024-04-17
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.2 - 2024-04-04
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2024-02-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
+* Permit to remove ignored invoices and stock moves
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 * Add warning when receiving too much goods from purchase
 * Require unit price only for confirmed purchase
```

### Comparing `trytond_purchase-7.0.3/COPYRIGHT` & `trytond_purchase-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/LICENSE` & `trytond_purchase-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/PKG-INFO` & `trytond_purchase-7.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_purchase
-Version: 7.0.3
+Version: 7.2.0
 Summary: Tryton module for purchase
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-purchase/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -49,28 +49,28 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: sparklines
 Requires-Dist: pygal; extra == "sparklines"
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ###############
 Purchase Module
 ###############
 
 The *Purchase Module* provides everything that is required to create and
 manage purchases made by the company.
```

### Comparing `trytond_purchase-7.0.3/__init__.py` & `trytond_purchase-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/configuration.py` & `trytond_purchase-7.2.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/configuration.xml` & `trytond_purchase-7.2.0/configuration.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_purchase-7.0.3/configuration.xml` & `trytond_purchase-7.2.0/configuration.xml`

```diff
@@ -21,22 +21,22 @@
     <record model="ir.action.act_window.view" id="act_purchase_configuration_view1">
       <field name="sequence" eval="1"/>
       <field name="view" ref="purchase_configuration_view_form"/>
       <field name="act_window" ref="act_purchase_configuration_form"/>
     </record>
     <menuitem parent="menu_configuration" action="act_purchase_configuration_form" sequence="10" id="menu_purchase_configuration" icon="tryton-list"/>
     <record model="ir.model.access" id="access_purchase_configuration">
-      <field name="model" search="[('model', '=', 'purchase.configuration')]"/>
+      <field name="model">purchase.configuration</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_purchase_configuration_purchase_admin">
-      <field name="model" search="[('model', '=', 'purchase.configuration')]"/>
+      <field name="model">purchase.configuration</field>
       <field name="group" ref="group_purchase_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_purchase-7.0.3/doc/conf.py` & `trytond_purchase-7.2.0/doc/conf.py`

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

### Comparing `trytond_purchase-7.0.3/doc/design.rst` & `trytond_purchase-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/doc/usage/prepurchase.rst` & `trytond_purchase-7.2.0/doc/usage/prepurchase.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/doc/usage/process.rst` & `trytond_purchase-7.2.0/doc/usage/process.inc.rst`

 * *Files 3% similar despite different names*

```diff
@@ -109,14 +109,20 @@
 
 .. tip::
 
    When using the wizard the moves and invoices to recreate will, by default,
    already be selected.
    This means you will need to deselect any that you do not want to recreate.
 
+.. note::
+
+   If you have ignored by mistake a move or an invoice, you can remove them
+   from the corresponding ignored list and after click on the
+   :guilabel:`Process` button.
+
 .. _Finishing a purchase:
 
 Finishing a purchase
 ====================
 
 In Tryton once a `Purchase <model-purchase.purchase>` is being processed there
 is no button that moves the purchase into a done state.
```

### Comparing `trytond_purchase-7.0.3/doc/usage/returns.rst` & `trytond_purchase-7.2.0/doc/usage/returns.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/icons/LICENSE` & `trytond_purchase-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/invoice.py` & `trytond_purchase-7.2.0/invoice.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from functools import wraps
 
 from trytond.i18n import gettext
 from trytond.model import ModelView, Workflow, fields
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval
+from trytond.tools import cached_property
 from trytond.transaction import Transaction, without_check_access
 
 
 def process_purchase(func):
     @wraps(func)
     def wrapper(cls, invoices):
         pool = Pool()
@@ -106,14 +107,24 @@
         super().__setup__()
         if not cls.origin.domain:
             cls.origin.domain = {}
         cls.origin.domain['purchase.line'] = [
             ('type', '=', Eval('type')),
             ]
 
+    @cached_property
+    def product_name(self):
+        pool = Pool()
+        PurchaseLine = pool.get('purchase.line')
+        name = super().product_name
+        if (isinstance(self.origin, PurchaseLine)
+                and self.origin.product_supplier):
+            name = self.origin.product_supplier.rec_name
+        return name
+
     @fields.depends('origin')
     def on_change_with_product_uom_category(self, name=None):
         pool = Pool()
         PurchaseLine = pool.get('purchase.line')
         category = super().on_change_with_product_uom_category(name=name)
         # Enforce the same unit category as they are used to compute the
         # remaining quantity to invoice and the quantity to receive.
```

### Comparing `trytond_purchase-7.0.3/invoice.xml` & `trytond_purchase-7.2.0/invoice.xml`

 * *Files 7% similar despite different names*

#### Comparing `trytond_purchase-7.0.3/invoice.xml` & `trytond_purchase-7.2.0/invoice.xml`

```diff
@@ -11,23 +11,23 @@
     </record>
     <record model="ir.action.keyword" id="act_open_invoice_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">purchase.purchase,-1</field>
       <field name="action" ref="act_invoice_form"/>
     </record>
     <record model="ir.model.access" id="access_invoice_purchase">
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
+      <field name="model">account.invoice</field>
       <field name="group" ref="group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_invoice_line_purchase">
-      <field name="model" search="[('model', '=', 'account.invoice.line')]"/>
+      <field name="model">account.invoice.line</field>
       <field name="group" ref="group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_purchase-7.0.3/locale/bg.po` & `trytond_purchase-7.2.0/locale/bg.po`

 * *Files 0% similar despite different names*

```diff
@@ -195,14 +195,19 @@
 msgid "From Location"
 msgstr "От местонахождение"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Редове от фактура"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Адрес за фактура"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Движения"
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -878,16 +883,16 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/ca.po` & `trytond_purchase-7.2.0/locale/ca.po`

 * *Files 0% similar despite different names*

```diff
@@ -175,14 +175,19 @@
 msgid "From Location"
 msgstr "Des de la ubicació"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Línies de factura"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Adreça de facturació"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Moviments"
 
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
 msgstr "Moviments en excepció"
@@ -804,18 +809,19 @@
 msgid "Done"
 msgstr "Finalitzada"
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr "Pendent"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 "Esteu intentar modificar la unitat de mesura de compra en la que es basen "
 "els preus de compra."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
@@ -865,15 +871,15 @@
 msgstr "Un impost només es pot afegir una vegada a una línia de compra."
 
 msgctxt "model:ir.message,text:msg_purchase_missing_account_expense"
 msgid ""
 "To invoice purchase \"%(purchase)s\" you must configure a default account "
 "expense."
 msgstr ""
-"Per facturar la compra \"%(purchase)\" heu de configurar un compte de "
+"Per facturar la compra \"%(purchase)s\" heu de configurar un compte de "
 "despeses per defecte."
 
 msgctxt "model:ir.message,text:msg_purchase_modify_header_draft"
 msgid ""
 "To modify the header of purchase \"%(purchase)s\", it must be in draft "
 "state."
 msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/cs.po` & `trytond_purchase-7.2.0/locale/cs.po`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,19 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Invoices"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -838,16 +843,16 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/de.po` & `trytond_purchase-7.2.0/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,19 @@
 msgid "From Location"
 msgstr "Von Lagerort"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Rechnungspositionen"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Rechnungsadresse"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Warenbewegungen"
 
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
 msgstr "Warenbewegungen mit Vorbehalt"
@@ -809,18 +814,19 @@
 msgid "Done"
 msgstr "Erledigt"
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr "Ausstehend"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 "Sie versuchen die Einkaufsmaßeinheit zu ändern, auf der die Einkaufspreise "
 "basieren."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
```

### Comparing `trytond_purchase-7.0.3/locale/es.po` & `trytond_purchase-7.2.0/locale/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -175,14 +175,19 @@
 msgid "From Location"
 msgstr "Desde ubicación"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Líneas de factura"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Dirección de facturación"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Movimientos"
 
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
 msgstr "Movimientos en excepción"
@@ -807,18 +812,19 @@
 msgid "Done"
 msgstr "Finalizada"
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr "Pendiente"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 "Está intentando modificar la unidad media de compra en la que se basan los "
 "precios de compra."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
```

### Comparing `trytond_purchase-7.0.3/locale/es_419.po` & `trytond_purchase-7.2.0/locale/es_419.po`

 * *Files 0% similar despite different names*

```diff
@@ -183,14 +183,19 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Líneas de factura"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Líneas de factura"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -824,16 +829,16 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/et.po` & `trytond_purchase-7.2.0/locale/et.po`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,19 @@
 msgid "From Location"
 msgstr "Asukohast"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Arveread"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Arve aadress"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Liikumised"
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -851,16 +856,16 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/fa.po` & `trytond_purchase-7.2.0/locale/fa.po`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,19 @@
 msgid "From Location"
 msgstr "از مکان"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "خطوط صورتحساب"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "آدرس صورتحساب"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "جابجایی ها"
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -862,16 +867,16 @@
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 "شما در حال تلاش برای تغییرواحد قیمت خرید هستید، که قیمت خرید بر مبنای آن "
 "متکی است."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
```

### Comparing `trytond_purchase-7.0.3/locale/fi.po` & `trytond_purchase-7.2.0/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,19 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Invoices"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -837,16 +842,16 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/fr.po` & `trytond_purchase-7.2.0/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,18 @@
 msgid "From Location"
 msgstr "Emplacement d'origine"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Lignes de facture"
 
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Progression de la facturation"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Mouvements"
 
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
 msgstr "Mouvements en exception"
@@ -809,18 +813,18 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr "En attentes"
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
-"Vous essayez de modifier l'unité de mesure d'achat sur laquelle est basée "
+"Vous essayez de modifier l'unité de mesure d'achat sur laquelle sont basés "
 "les prix d'achat."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/hu.po` & `trytond_purchase-7.2.0/locale/hu.po`

 * *Files 0% similar despite different names*

```diff
@@ -183,14 +183,19 @@
 msgid "From Location"
 msgstr "Induló tárhely"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Számlasorok"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Számlázási cím"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Mozgások"
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -847,16 +852,16 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/id.po` & `trytond_purchase-7.2.0/locale/id.po`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,19 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Baris Faktur"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Alamat Faktur"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Perpindahan"
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -833,16 +838,16 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/it.po` & `trytond_purchase-7.2.0/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,19 @@
 msgid "From Location"
 msgstr "Da locazione"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Righe fattura"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Indirizzo di fatturazione"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Movimenti"
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -857,16 +862,16 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/lo.po` & `trytond_purchase-7.2.0/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -196,14 +196,19 @@
 
 #, fuzzy
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "ລາຍການເກັບເງິນ"
 
 #, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "ທີ່ຢູ່"
+
+#, fuzzy
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "ຕັດບັນຊີສາງ"
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -899,16 +904,16 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/lt.po` & `trytond_purchase-7.2.0/locale/lt.po`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,19 @@
 msgid "From Location"
 msgstr "Išsiuntimo vieta"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Sąskaitos faktūros eilutės"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Juridinis adresas"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Operacijos"
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -854,16 +859,16 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/nl.po` & `trytond_purchase-7.2.0/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,19 @@
 msgid "From Location"
 msgstr "Van locatie"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Factuurregels"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Factuuradres"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Voorraad bewegingen"
 
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
 msgstr "Voorraad Mutaties Uitzondering"
@@ -809,18 +814,19 @@
 msgid "Done"
 msgstr "Afgerond"
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr "In behandeling"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 "U probeert de inkoop maateenheid waarop de inkoopprijzen zijn gebaseerd te "
 "wijzigen."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
```

### Comparing `trytond_purchase-7.0.3/locale/pl.po` & `trytond_purchase-7.2.0/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,19 @@
 msgid "From Location"
 msgstr "Z lokalizacji"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Wiersze faktury"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Adres faktury"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Ruchy"
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -866,16 +871,16 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/pt.po` & `trytond_purchase-7.2.0/locale/pt.po`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,19 @@
 msgid "From Location"
 msgstr "Origem"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Linhas da fatura"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Endereço para faturamento"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Movimentações"
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -874,16 +879,16 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/ro.po` & `trytond_purchase-7.2.0/locale/tr.po`

 * *Files 4% similar despite different names*

```diff
@@ -2,84 +2,82 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.invoice,purchase_exception_state:"
 msgid "Exception State"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:account.invoice,purchases:"
 msgid "Purchases"
-msgstr ""
+msgstr "Purchases"
 
 msgctxt "field:party.party,customer_code:"
 msgid "Customer Code"
 msgstr ""
 
 msgctxt "field:party.party,customer_codes:"
 msgid "Customer Codes"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:party.party,supplier_currencies:"
 msgid "Supplier Currencies"
-msgstr "Furnizor"
+msgstr "Product Suppliers"
 
 #, fuzzy
 msgctxt "field:party.party,supplier_currency:"
 msgid "Supplier Currency"
-msgstr "Moneda"
+msgstr "Product Suppliers"
 
 msgctxt "field:party.party,supplier_lead_time:"
 msgid "Lead Time"
 msgstr ""
 
 msgctxt "field:party.party,supplier_lead_times:"
 msgid "Lead Times"
 msgstr ""
 
 msgctxt "field:party.party.customer_code,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:party.party.customer_code,customer_code:"
 msgid "Customer Code"
 msgstr ""
 
 msgctxt "field:party.party.customer_code,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:party.party.supplier_currency,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:party.party.supplier_currency,supplier_currency:"
 msgid "Supplier Currency"
-msgstr "Moneda"
+msgstr "Product Suppliers"
 
-#, fuzzy
 msgctxt "field:party.party.supplier_lead_time,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:party.party.supplier_lead_time,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:party.party.supplier_lead_time,supplier_lead_time:"
 msgid "Lead Time"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,last_purchase_price_uom:"
 msgid "Last Purchase Price"
-msgstr "Achiziții"
+msgstr "Purchases"
 
 msgctxt "field:product.product,product_suppliers:"
 msgid "Suppliers"
 msgstr ""
 
 msgctxt "field:product.product,purchasable:"
 msgid "Purchasable"
@@ -88,28 +86,28 @@
 msgctxt "field:product.product,purchase_price_uom:"
 msgid "Purchase Price"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,purchase_uom:"
 msgid "Purchase UoM"
-msgstr "Achiziții"
+msgstr "Purchases"
 
 msgctxt "field:product.template,product_suppliers:"
 msgid "Suppliers"
 msgstr ""
 
 msgctxt "field:product.template,purchasable:"
 msgid "Purchasable"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,purchase_uom:"
 msgid "Purchase UoM"
-msgstr "Achiziții"
+msgstr "Purchases"
 
 msgctxt "field:purchase.configuration,purchase_invoice_method:"
 msgid "Invoice Method"
 msgstr ""
 
 msgctxt "field:purchase.configuration,purchase_process_after:"
 msgid "Process Purchase after"
@@ -122,15 +120,15 @@
 msgctxt ""
 "field:purchase.configuration.purchase_method,purchase_invoice_method:"
 msgid "Invoice Method"
 msgstr ""
 
 msgctxt "field:purchase.configuration.sequence,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:purchase.configuration.sequence,purchase_sequence:"
 msgid "Purchase Sequence"
 msgstr ""
 
 msgctxt "field:purchase.handle.invoice.exception.ask,domain_invoices:"
 msgid "Domain Invoices"
@@ -150,56 +148,61 @@
 
 msgctxt "field:purchase.line,actual_quantity:"
 msgid "Actual Quantity"
 msgstr ""
 
 msgctxt "field:purchase.line,amount:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "field:purchase.line,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:purchase.line,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr ""
 
 msgctxt "field:purchase.line,delivery_date:"
 msgid "Delivery Date"
-msgstr "Data de livrare"
+msgstr ""
 
 msgctxt "field:purchase.line,delivery_date_edit:"
 msgid "Edit Delivery Date"
 msgstr ""
 
 msgctxt "field:purchase.line,delivery_date_store:"
 msgid "Delivery Date"
 msgstr ""
 
 msgctxt "field:purchase.line,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:purchase.line,from_location:"
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Invoices"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
-msgstr "Gestionare Excepție Factura"
+msgstr "Handle Invoice Exception"
 
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
 msgctxt "field:purchase.line,moves_progress:"
 msgid "Moves Progress"
@@ -211,32 +214,33 @@
 
 msgctxt "field:purchase.line,note:"
 msgid "Note"
 msgstr ""
 
 msgctxt "field:purchase.line,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "field:purchase.line,product_supplier:"
 msgid "Supplier's Product"
 msgstr ""
 
 msgctxt "field:purchase.line,product_uom_category:"
 msgid "Product UoM Category"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
-msgstr ""
+msgstr "Purchases"
 
 #, fuzzy
 msgctxt "field:purchase.line,purchase_date:"
 msgid "Purchase Date"
-msgstr "Achiziții"
+msgstr "Purchases"
 
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr ""
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
@@ -245,23 +249,23 @@
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.line,supplier:"
 msgid "Supplier"
-msgstr "Furnizor"
+msgstr "Product Suppliers"
 
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
-msgstr "Spre Locație"
+msgstr ""
 
 msgctxt "field:purchase.line,type:"
 msgid "Type"
 msgstr ""
 
 msgctxt "field:purchase.line,unit:"
 msgid "Unit"
@@ -277,19 +281,19 @@
 
 msgctxt "field:purchase.line-account.tax,line:"
 msgid "Purchase Line"
 msgstr ""
 
 msgctxt "field:purchase.line-account.tax,tax:"
 msgid "Tax"
-msgstr "Impozit"
+msgstr ""
 
 msgctxt "field:purchase.line-ignored-stock.move,move:"
 msgid "Move"
-msgstr "Mișcare"
+msgstr ""
 
 msgctxt "field:purchase.line-ignored-stock.move,purchase_line:"
 msgid "Purchase Line"
 msgstr ""
 
 msgctxt "field:purchase.line-recreated-stock.move,move:"
 msgid "Move"
@@ -297,59 +301,60 @@
 
 msgctxt "field:purchase.line-recreated-stock.move,purchase_line:"
 msgid "Purchase Line"
 msgstr ""
 
 msgctxt "field:purchase.product_supplier,code:"
 msgid "Code"
-msgstr "Cod"
+msgstr ""
 
 msgctxt "field:purchase.product_supplier,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:purchase.product_supplier,currency:"
 msgid "Currency"
-msgstr "Moneda"
+msgstr ""
 
 msgctxt "field:purchase.product_supplier,lead_time:"
 msgid "Lead Time"
 msgstr ""
 
 msgctxt "field:purchase.product_supplier,name:"
 msgid "Name"
 msgstr ""
 
 msgctxt "field:purchase.product_supplier,party:"
 msgid "Supplier"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:purchase.product_supplier,prices:"
 msgid "Prices"
-msgstr ""
+msgstr "Prices"
 
 msgctxt "field:purchase.product_supplier,product:"
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:purchase.product_supplier,template:"
 msgid "Product"
-msgstr "Produs"
+msgstr ""
 
 msgctxt "field:purchase.product_supplier,unit:"
 msgid "Unit"
 msgstr ""
 
 msgctxt "field:purchase.product_supplier.price,currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr ""
 
 msgctxt "field:purchase.product_supplier.price,product_supplier:"
 msgid "Supplier"
-msgstr "Furnizor"
+msgstr ""
 
 msgctxt "field:purchase.product_supplier.price,quantity:"
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:purchase.product_supplier.price,unit:"
 msgid "Unit"
@@ -361,123 +366,128 @@
 
 msgctxt "field:purchase.purchase,comment:"
 msgid "Comment"
 msgstr ""
 
 msgctxt "field:purchase.purchase,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:purchase.purchase,confirmed_by:"
 msgid "Confirmed By"
-msgstr ""
+msgstr "Confirmed"
 
 msgctxt "field:purchase.purchase,contact:"
 msgid "Contact"
 msgstr ""
 
 msgctxt "field:purchase.purchase,currency:"
 msgid "Currency"
-msgstr "Valută"
+msgstr ""
 
 msgctxt "field:purchase.purchase,delivery_date:"
 msgid "Delivery Date"
-msgstr "Data de livrare"
+msgstr ""
 
 msgctxt "field:purchase.purchase,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "field:purchase.purchase,invoice_address:"
 msgid "Invoice Address"
 msgstr ""
 
 msgctxt "field:purchase.purchase,invoice_method:"
 msgid "Invoice Method"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:purchase.purchase,invoice_party:"
 msgid "Invoice Party"
-msgstr "Parte Facturata"
+msgstr "Invoices"
 
 msgctxt "field:purchase.purchase,invoice_state:"
 msgid "Invoice State"
-msgstr "Stare Factura"
+msgstr ""
 
+#, fuzzy
 msgctxt "field:purchase.purchase,invoices:"
 msgid "Invoices"
-msgstr "Facturi"
+msgstr "Invoices"
 
 msgctxt "field:purchase.purchase,invoices_ignored:"
 msgid "Ignored Invoices"
-msgstr "Facturi ignorate"
+msgstr ""
 
 msgctxt "field:purchase.purchase,invoices_recreated:"
 msgid "Recreated Invoices"
 msgstr ""
 
 msgctxt "field:purchase.purchase,lines:"
 msgid "Lines"
-msgstr "Rânduri"
+msgstr ""
 
 msgctxt "field:purchase.purchase,moves:"
 msgid "Moves"
-msgstr "Mișcări"
+msgstr ""
 
 msgctxt "field:purchase.purchase,number:"
 msgid "Number"
-msgstr "Număr"
+msgstr ""
 
 msgctxt "field:purchase.purchase,origin:"
 msgid "Origin"
 msgstr ""
 
 msgctxt "field:purchase.purchase,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:purchase.purchase,party_lang:"
 msgid "Party Language"
-msgstr "Limba Părții"
+msgstr ""
 
 msgctxt "field:purchase.purchase,payment_term:"
 msgid "Payment Term"
-msgstr "Termen de plata"
+msgstr ""
 
 msgctxt "field:purchase.purchase,purchase_date:"
 msgid "Purchase Date"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:purchase.purchase,quoted_by:"
 msgid "Quoted By"
-msgstr ""
+msgstr "Quote"
 
 msgctxt "field:purchase.purchase,reference:"
 msgid "Reference"
 msgstr ""
 
 msgctxt "field:purchase.purchase,shipment_returns:"
 msgid "Shipment Returns"
 msgstr ""
 
 msgctxt "field:purchase.purchase,shipment_state:"
 msgid "Shipment State"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:purchase.purchase,shipments:"
 msgid "Shipments"
-msgstr "Expedieri"
+msgstr "Shipments"
 
 msgctxt "field:purchase.purchase,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:purchase.purchase,tax_amount:"
 msgid "Tax"
-msgstr "Impozit"
+msgstr ""
 
 msgctxt "field:purchase.purchase,tax_amount_cache:"
 msgid "Tax Cache"
 msgstr ""
 
 msgctxt "field:purchase.purchase,total_amount:"
 msgid "Total"
@@ -495,34 +505,37 @@
 msgid "Untaxed Cache"
 msgstr ""
 
 msgctxt "field:purchase.purchase,warehouse:"
 msgid "Warehouse"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:purchase.purchase-ignored-account.invoice,invoice:"
 msgid "Invoice"
-msgstr ""
+msgstr "Invoices"
 
+#, fuzzy
 msgctxt "field:purchase.purchase-ignored-account.invoice,purchase:"
 msgid "Purchase"
-msgstr ""
+msgstr "Purchases"
 
+#, fuzzy
 msgctxt "field:purchase.purchase-recreated-account.invoice,invoice:"
 msgid "Invoice"
-msgstr ""
+msgstr "Invoices"
 
+#, fuzzy
 msgctxt "field:purchase.purchase-recreated-account.invoice,purchase:"
 msgid "Purchase"
-msgstr ""
+msgstr "Purchases"
 
-#, fuzzy
 msgctxt "field:purchase.reporting.context,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:purchase.reporting.context,from_date:"
 msgid "From Date"
 msgstr ""
 
 msgctxt "field:purchase.reporting.context,period:"
 msgid "Period"
@@ -535,48 +548,49 @@
 msgctxt "field:purchase.reporting.context,warehouse:"
 msgid "Warehouse"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.reporting.product,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr "Product Suppliers"
 
 #, fuzzy
 msgctxt "field:purchase.reporting.product,product_supplier:"
 msgid "Supplier's Product"
-msgstr "Furnizor"
+msgstr "Product Suppliers"
 
 #, fuzzy
 msgctxt "field:purchase.reporting.product.time_series,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr "Product Suppliers"
 
 #, fuzzy
 msgctxt "field:purchase.reporting.product.time_series,product_supplier:"
 msgid "Supplier's Product"
-msgstr "Furnizor"
+msgstr "Product Suppliers"
 
 #, fuzzy
 msgctxt "field:purchase.reporting.supplier,supplier:"
 msgid "Supplier"
-msgstr "Furnizor"
+msgstr "Product Suppliers"
 
 #, fuzzy
 msgctxt "field:purchase.reporting.supplier.time_series,supplier:"
 msgid "Supplier"
-msgstr "Furnizor"
+msgstr "Product Suppliers"
 
 msgctxt "field:stock.location,supplier_return_location:"
 msgid "Supplier Return"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:stock.move,purchase:"
 msgid "Purchase"
-msgstr ""
+msgstr "Purchases"
 
 msgctxt "field:stock.move,purchase_exception_state:"
 msgid "Exception State"
 msgstr ""
 
 msgctxt "field:stock.move,supplier:"
 msgid "Supplier"
@@ -664,174 +678,180 @@
 
 msgctxt "help:stock.location,supplier_return_location:"
 msgid "If empty the Storage location is used."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
-msgstr "Facturi"
+msgstr "Invoices"
 
 msgctxt "model:ir.action,name:act_open_supplier"
 msgid "Parties associated to Purchases"
-msgstr ""
+msgstr "Parties associated to Purchases"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_product_supplier_form"
 msgid "Suppliers"
-msgstr "Furnizor"
+msgstr "Product Suppliers"
 
 msgctxt "model:ir.action,name:act_product_supplier_price_form"
 msgid "Prices"
-msgstr ""
+msgstr "Prices"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_configuration_form"
 msgid "Configuration"
-msgstr "Configurație"
+msgstr "Configuration"
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
-msgstr ""
+msgstr "Purchases"
 
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
-msgstr ""
+msgstr "Purchases"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_line_relate"
 msgid "Purchase Lines"
-msgstr "Achiziții"
+msgstr "Purchases"
 
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
-msgstr "Achiziții"
+msgstr "Purchases"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
-msgstr "Achiziții"
+msgstr "Purchases"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
-msgstr "Achiziții"
+msgstr "Purchases"
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main_time_series"
 msgid "Purchases"
-msgstr "Achiziții"
+msgstr "Purchases"
 
 msgctxt "model:ir.action,name:act_reporting_product"
 msgid "Purchases per Product"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_reporting_product_time_series"
 msgid "Purchases per Product"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_supplier"
 msgid "Purchases per Supplier"
-msgstr ""
+msgstr "Product Suppliers"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_supplier_time_series"
 msgid "Purchases per Supplier"
-msgstr ""
+msgstr "Product Suppliers"
 
 msgctxt "model:ir.action,name:act_return_form"
 msgid "Returns"
-msgstr "Retururi"
+msgstr "Returns"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
-msgstr "Expedieri"
+msgstr "Shipments"
 
+#, fuzzy
 msgctxt "model:ir.action,name:report_purchase"
 msgid "Purchase"
-msgstr ""
+msgstr "Purchase"
 
 msgctxt "model:ir.action,name:wizard_invoice_handle_exception"
 msgid "Handle Invoice Exception"
-msgstr "Gestionare Excepție Factura"
+msgstr "Handle Invoice Exception"
 
 msgctxt "model:ir.action,name:wizard_modify_header"
 msgid "Modify Header"
-msgstr "Modificați antetul"
+msgstr "Modify Header"
 
 #, fuzzy
 msgctxt "model:ir.action,name:wizard_return_purchase"
 msgid "Return Purchase"
-msgstr "Returnări"
+msgstr "Purchases"
 
 msgctxt "model:ir.action,name:wizard_shipment_handle_exception"
 msgid "Handle Shipment Exception"
-msgstr "Gestioneaza Excepție de expediere"
+msgstr "Handle Shipment Exception"
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_form_domain_all"
 msgid "All"
-msgstr ""
+msgstr "All"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_confirmed"
 msgid "Confirmed"
-msgstr ""
+msgstr "Confirmed"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_exception"
 msgid "Exception"
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_processing"
 msgid "Processing"
-msgstr ""
+msgstr "Processing"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
-msgstr ""
+msgstr "Quotation"
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
 msgid "All"
-msgstr ""
+msgstr "All"
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
 msgid "Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
 msgid "Pending"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
 msgid "All"
-msgstr ""
+msgstr "All"
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
 msgid "Done"
 msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
@@ -888,23 +908,22 @@
 
 msgctxt "model:ir.message,text:msg_purchase_product_missing_account_expense"
 msgid ""
 "To invoice purchase \"%(purchase)s\" you must define an account expense for "
 "product \"%(product)s\"."
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_purchase_reporting_company"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_purchase_reporting_currency"
 msgid "Currency"
-msgstr "Moneda"
+msgstr "Product Suppliers"
 
 msgctxt "model:ir.message,text:msg_purchase_reporting_date"
 msgid "Date"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_reporting_expense"
 msgid "Expense"
@@ -935,49 +954,49 @@
 msgctxt "model:ir.message,text:msg_warehouse_required_for_quotation"
 msgid ""
 "To get a quote for the purchase \"%(purchase)s\" you must enter a warehouse."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:purchase_cancel_button"
 msgid "Cancel"
-msgstr ""
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:purchase_confirm_button"
 msgid "Confirm"
-msgstr ""
+msgstr "Confirm"
 
 msgctxt "model:ir.model.button,string:purchase_draft_button"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:purchase_hande_invoice_exception_button"
 msgid "Handle Invoice Exception"
-msgstr ""
+msgstr "Handle Invoice Exception"
 
 msgctxt ""
 "model:ir.model.button,string:purchase_hande_shipment_exception_button"
 msgid "Handle Shipment Exception"
-msgstr ""
+msgstr "Handle Shipment Exception"
 
 #, fuzzy
 msgctxt "model:ir.model.button,string:purchase_manual_invoice_button"
 msgid "Create Invoice"
-msgstr "Facturi ignorate"
+msgstr "Invoices"
 
 msgctxt "model:ir.model.button,string:purchase_modify_header_button"
 msgid "Modify Header"
-msgstr ""
+msgstr "Modify Header"
 
 msgctxt "model:ir.model.button,string:purchase_process_button"
 msgid "Process"
-msgstr ""
+msgstr "Process"
 
 msgctxt "model:ir.model.button,string:purchase_quote_button"
 msgid "Quote"
-msgstr ""
+msgstr "Quote"
 
 msgctxt "model:ir.rule.group,name:rule_group_product_supplier_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_purchase_companies"
 msgid "User in companies"
@@ -1006,88 +1025,97 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_supplier_time_series_companies"
 msgid "User in companies"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.sequence,name:sequence_purchase"
 msgid "Purchase"
-msgstr ""
+msgstr "Purchase"
 
+#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_purchase"
 msgid "Purchase"
-msgstr ""
+msgstr "Purchase"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configurare"
+msgstr "Configuration"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_product_supplier"
 msgid "Suppliers"
-msgstr "Furnizor"
+msgstr "Product Suppliers"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_purchase"
 msgid "Purchases"
-msgstr "Achiziții"
+msgstr "Purchases"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_purchase_configuration"
 msgid "Configuration"
-msgstr "Configurare"
+msgstr "Configuration"
 
 msgctxt "model:ir.ui.menu,name:menu_purchase_form"
 msgid "Purchases"
-msgstr ""
+msgstr "Purchases"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "Raportare"
+msgstr "Reporting"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_reporting_purchase"
 msgid "Purchases"
-msgstr "Achiziții"
+msgstr "Purchases"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_supplier"
 msgid "Associated to Purchases"
-msgstr ""
+msgstr "Parties associated to Purchases"
 
 msgctxt "model:party.party.customer_code,name:"
 msgid "Party Customer Code"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:party.party.supplier_currency,name:"
 msgid "Party Supplier Currency"
-msgstr ""
+msgstr "Product Suppliers"
 
 #, fuzzy
 msgctxt "model:party.party.supplier_lead_time,name:"
 msgid "Supplier Lead Time"
-msgstr "Furnizor"
+msgstr "Product Suppliers"
 
+#, fuzzy
 msgctxt "model:purchase.configuration,name:"
 msgid "Purchase Configuration"
-msgstr ""
+msgstr "Purchase Configuration"
 
 msgctxt "model:purchase.configuration.purchase_method,name:"
 msgid "Purchase Configuration Purchase Method"
 msgstr ""
 
 msgctxt "model:purchase.configuration.sequence,name:"
 msgid "Purchase Configuration Sequence"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:purchase.handle.invoice.exception.ask,name:"
 msgid "Handle Invoice Exception"
-msgstr ""
+msgstr "Handle Invoice Exception"
 
+#, fuzzy
 msgctxt "model:purchase.handle.shipment.exception.ask,name:"
 msgid "Handle Shipment Exception"
-msgstr ""
+msgstr "Handle Shipment Exception"
 
 msgctxt "model:purchase.line,name:"
 msgid "Purchase Line"
 msgstr ""
 
 msgctxt "model:purchase.line-account.tax,name:"
 msgid "Purchase Line - Tax"
@@ -1097,47 +1125,50 @@
 msgid "Purchase Line - Ignored Move"
 msgstr ""
 
 msgctxt "model:purchase.line-recreated-stock.move,name:"
 msgid "Purchase Line - Ignored Move"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:purchase.product_supplier,name:"
 msgid "Product Supplier"
-msgstr ""
+msgstr "Product Suppliers"
 
 msgctxt "model:purchase.product_supplier.price,name:"
 msgid "Product Supplier Price"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:purchase.purchase,name:"
 msgid "Purchase"
-msgstr ""
+msgstr "Purchases"
 
 msgctxt "model:purchase.purchase-ignored-account.invoice,name:"
 msgid "Purchase - Ignored Invoice"
 msgstr ""
 
 msgctxt "model:purchase.purchase-recreated-account.invoice,name:"
 msgid "Purchase - Recreated Invoice"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:purchase.reporting.context,name:"
 msgid "Purchase Reporting Context"
-msgstr ""
+msgstr "Purchase Configuration"
 
 #, fuzzy
 msgctxt "model:purchase.reporting.main,name:"
 msgid "Purchase Reporting"
-msgstr "Raportare"
+msgstr "Purchase Configuration"
 
 #, fuzzy
 msgctxt "model:purchase.reporting.main.time_series,name:"
 msgid "Purchase Reporting"
-msgstr "Raportare"
+msgstr "Purchase Configuration"
 
 msgctxt "model:purchase.reporting.product,name:"
 msgid "Purchase Reporting per Product"
 msgstr ""
 
 msgctxt "model:purchase.reporting.product.time_series,name:"
 msgid "Purchase Reporting per Product"
@@ -1150,31 +1181,32 @@
 msgctxt "model:purchase.reporting.supplier.time_series,name:"
 msgid "Purchase Reporting per Supplier"
 msgstr ""
 
 #, fuzzy
 msgctxt "model:purchase.return_purchase.start,name:"
 msgid "Return Purchase"
-msgstr "Returnări"
+msgstr "Purchases"
 
+#, fuzzy
 msgctxt "model:res.group,name:group_purchase"
 msgid "Purchase"
-msgstr ""
+msgstr "Purchase"
 
 msgctxt "model:res.group,name:group_purchase_admin"
 msgid "Purchase Administrator"
-msgstr ""
+msgstr "Purchase Administrator"
 
 msgctxt "report:purchase.purchase:"
 msgid ":"
-msgstr ""
+msgstr ":"
 
 msgctxt "report:purchase.purchase:"
 msgid "Amount"
-msgstr "Suma"
+msgstr ""
 
 msgctxt "report:purchase.purchase:"
 msgid "Customer Code:"
 msgstr ""
 
 msgctxt "report:purchase.purchase:"
 msgid "Date:"
@@ -1182,19 +1214,19 @@
 
 msgctxt "report:purchase.purchase:"
 msgid "Delivery Address:"
 msgstr ""
 
 msgctxt "report:purchase.purchase:"
 msgid "Description"
-msgstr "Descriere"
+msgstr ""
 
 msgctxt "report:purchase.purchase:"
 msgid "Description:"
-msgstr "Descriere:"
+msgstr ""
 
 msgctxt "report:purchase.purchase:"
 msgid "Draft Purchase Order"
 msgstr ""
 
 msgctxt "report:purchase.purchase:"
 msgid "Purchase Order N°:"
@@ -1308,37 +1340,42 @@
 msgid "Received"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:purchase.purchase,state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Cancel"
 
+#, fuzzy
 msgctxt "selection:purchase.purchase,state:"
 msgid "Confirmed"
-msgstr ""
+msgstr "Confirm"
 
 msgctxt "selection:purchase.purchase,state:"
 msgid "Done"
 msgstr ""
 
+#, fuzzy
 msgctxt "selection:purchase.purchase,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
+#, fuzzy
 msgctxt "selection:purchase.purchase,state:"
 msgid "Processing"
-msgstr ""
+msgstr "Processing"
 
+#, fuzzy
 msgctxt "selection:purchase.purchase,state:"
 msgid "Quotation"
-msgstr ""
+msgstr "Quotation"
 
 msgctxt "selection:purchase.reporting.context,period:"
 msgid "Day"
 msgstr ""
 
 msgctxt "selection:purchase.reporting.context,period:"
 msgid "Month"
@@ -1352,17 +1389,18 @@
 msgid "Ignored"
 msgstr ""
 
 msgctxt "selection:stock.move,purchase_exception_state:"
 msgid "Recreated"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:party.party:"
 msgid "Supplier"
-msgstr ""
+msgstr "Product Suppliers"
 
 msgctxt "view:product.template:"
 msgid "Suppliers"
 msgstr ""
 
 msgctxt "view:purchase.handle.invoice.exception.ask:"
 msgid "Choose invoices to recreate:"
@@ -1388,47 +1426,52 @@
 msgid "Taxes"
 msgstr ""
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr ""
 
+#, fuzzy
 msgctxt "view:purchase.purchase:"
 msgid "Purchase"
-msgstr ""
+msgstr "Purchases"
 
 msgctxt "view:purchase.return_purchase.start:"
 msgid "Are you sure to return these/this purchase(s)?"
 msgstr ""
 
+#, fuzzy
 msgctxt "wizard_button:purchase.handle.invoice.exception,ask,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Cancel"
 
 msgctxt "wizard_button:purchase.handle.invoice.exception,ask,handle:"
 msgid "OK"
 msgstr ""
 
+#, fuzzy
 msgctxt "wizard_button:purchase.handle.shipment.exception,ask,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Cancel"
 
 msgctxt "wizard_button:purchase.handle.shipment.exception,ask,handle:"
 msgid "OK"
 msgstr ""
 
+#, fuzzy
 msgctxt "wizard_button:purchase.modify_header,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Cancel"
 
 msgctxt "wizard_button:purchase.modify_header,start,modify:"
 msgid "Modify"
 msgstr ""
 
+#, fuzzy
 msgctxt "wizard_button:purchase.return_purchase,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Cancel"
 
 #, fuzzy
 msgctxt "wizard_button:purchase.return_purchase,start,return_:"
 msgid "Return"
-msgstr "Returnări"
+msgstr "Returns"
```

### Comparing `trytond_purchase-7.0.3/locale/ru.po` & `trytond_purchase-7.2.0/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,19 @@
 msgid "From Location"
 msgstr "Из местоположения"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Строки инвойса"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Адрес для инвойса"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Перемещения"
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -877,16 +882,16 @@
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/sl.po` & `trytond_purchase-7.2.0/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -178,14 +178,19 @@
 msgid "From Location"
 msgstr "Iz lokacije"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Postavke računa"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Plačnik"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "Promet"
 
 #, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
@@ -818,16 +823,16 @@
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr "V teku"
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 "Poskušate spremeniti mersko enoto na podlagi katere so določene nabavne "
 "cene."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
```

### Comparing `trytond_purchase-7.0.3/locale/tr.po` & `trytond_purchase-7.2.0/locale/uk.po`

 * *Files 19% similar despite different names*

```diff
@@ -2,36 +2,33 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.invoice,purchase_exception_state:"
 msgid "Exception State"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:account.invoice,purchases:"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr ""
 
 msgctxt "field:party.party,customer_code:"
 msgid "Customer Code"
 msgstr ""
 
 msgctxt "field:party.party,customer_codes:"
 msgid "Customer Codes"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:party.party,supplier_currencies:"
 msgid "Supplier Currencies"
-msgstr "Product Suppliers"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:party.party,supplier_currency:"
 msgid "Supplier Currency"
-msgstr "Product Suppliers"
+msgstr ""
 
 msgctxt "field:party.party,supplier_lead_time:"
 msgid "Lead Time"
 msgstr ""
 
 msgctxt "field:party.party,supplier_lead_times:"
 msgid "Lead Times"
@@ -49,18 +46,17 @@
 msgid "Party"
 msgstr ""
 
 msgctxt "field:party.party.supplier_currency,party:"
 msgid "Party"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:party.party.supplier_currency,supplier_currency:"
 msgid "Supplier Currency"
-msgstr "Product Suppliers"
+msgstr ""
 
 msgctxt "field:party.party.supplier_lead_time,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:party.party.supplier_lead_time,party:"
 msgid "Party"
@@ -69,15 +65,15 @@
 msgctxt "field:party.party.supplier_lead_time,supplier_lead_time:"
 msgid "Lead Time"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,last_purchase_price_uom:"
 msgid "Last Purchase Price"
-msgstr "Purchases"
+msgstr "Звітність"
 
 msgctxt "field:product.product,product_suppliers:"
 msgid "Suppliers"
 msgstr ""
 
 msgctxt "field:product.product,purchasable:"
 msgid "Purchasable"
@@ -86,28 +82,28 @@
 msgctxt "field:product.product,purchase_price_uom:"
 msgid "Purchase Price"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.product,purchase_uom:"
 msgid "Purchase UoM"
-msgstr "Purchases"
+msgstr "Звітність"
 
 msgctxt "field:product.template,product_suppliers:"
 msgid "Suppliers"
 msgstr ""
 
 msgctxt "field:product.template,purchasable:"
 msgid "Purchasable"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:product.template,purchase_uom:"
 msgid "Purchase UoM"
-msgstr "Purchases"
+msgstr "Звітність"
 
 msgctxt "field:purchase.configuration,purchase_invoice_method:"
 msgid "Invoice Method"
 msgstr ""
 
 msgctxt "field:purchase.configuration,purchase_process_after:"
 msgid "Process Purchase after"
@@ -182,22 +178,25 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr ""
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
-msgstr "Handle Invoice Exception"
+msgstr ""
 
 msgctxt "field:purchase.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr ""
 
 msgctxt "field:purchase.line,moves_progress:"
 msgid "Moves Progress"
@@ -219,40 +218,38 @@
 msgid "Supplier's Product"
 msgstr ""
 
 msgctxt "field:purchase.line,product_uom_category:"
 msgid "Product UoM Category"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.line,purchase:"
 msgid "Purchase"
-msgstr "Purchases"
+msgstr ""
 
 #, fuzzy
 msgctxt "field:purchase.line,purchase_date:"
 msgid "Purchase Date"
-msgstr "Purchases"
+msgstr "Звітність"
 
 msgctxt "field:purchase.line,purchase_state:"
 msgid "Purchase State"
 msgstr ""
 
 msgctxt "field:purchase.line,quantity:"
 msgid "Quantity"
 msgstr ""
 
 msgctxt "field:purchase.line,summary:"
 msgid "Summary"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.line,supplier:"
 msgid "Supplier"
-msgstr "Product Suppliers"
+msgstr ""
 
 msgctxt "field:purchase.line,taxes:"
 msgid "Taxes"
 msgstr ""
 
 msgctxt "field:purchase.line,to_location:"
 msgid "To Location"
@@ -318,18 +315,17 @@
 msgid "Name"
 msgstr ""
 
 msgctxt "field:purchase.product_supplier,party:"
 msgid "Supplier"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.product_supplier,prices:"
 msgid "Prices"
-msgstr "Prices"
+msgstr ""
 
 msgctxt "field:purchase.product_supplier,product:"
 msgid "Variant"
 msgstr ""
 
 msgctxt "field:purchase.product_supplier,template:"
 msgid "Product"
@@ -363,18 +359,17 @@
 msgid "Comment"
 msgstr ""
 
 msgctxt "field:purchase.purchase,company:"
 msgid "Company"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.purchase,confirmed_by:"
 msgid "Confirmed By"
-msgstr "Confirmed"
+msgstr ""
 
 msgctxt "field:purchase.purchase,contact:"
 msgid "Contact"
 msgstr ""
 
 msgctxt "field:purchase.purchase,currency:"
 msgid "Currency"
@@ -392,27 +387,25 @@
 msgid "Invoice Address"
 msgstr ""
 
 msgctxt "field:purchase.purchase,invoice_method:"
 msgid "Invoice Method"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.purchase,invoice_party:"
 msgid "Invoice Party"
-msgstr "Invoices"
+msgstr ""
 
 msgctxt "field:purchase.purchase,invoice_state:"
 msgid "Invoice State"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.purchase,invoices:"
 msgid "Invoices"
-msgstr "Invoices"
+msgstr ""
 
 msgctxt "field:purchase.purchase,invoices_ignored:"
 msgid "Ignored Invoices"
 msgstr ""
 
 msgctxt "field:purchase.purchase,invoices_recreated:"
 msgid "Recreated Invoices"
@@ -446,35 +439,33 @@
 msgid "Payment Term"
 msgstr ""
 
 msgctxt "field:purchase.purchase,purchase_date:"
 msgid "Purchase Date"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.purchase,quoted_by:"
 msgid "Quoted By"
-msgstr "Quote"
+msgstr ""
 
 msgctxt "field:purchase.purchase,reference:"
 msgid "Reference"
 msgstr ""
 
 msgctxt "field:purchase.purchase,shipment_returns:"
 msgid "Shipment Returns"
 msgstr ""
 
 msgctxt "field:purchase.purchase,shipment_state:"
 msgid "Shipment State"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.purchase,shipments:"
 msgid "Shipments"
-msgstr "Shipments"
+msgstr ""
 
 msgctxt "field:purchase.purchase,state:"
 msgid "State"
 msgstr ""
 
 msgctxt "field:purchase.purchase,tax_amount:"
 msgid "Tax"
@@ -500,33 +491,29 @@
 msgid "Untaxed Cache"
 msgstr ""
 
 msgctxt "field:purchase.purchase,warehouse:"
 msgid "Warehouse"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.purchase-ignored-account.invoice,invoice:"
 msgid "Invoice"
-msgstr "Invoices"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.purchase-ignored-account.invoice,purchase:"
 msgid "Purchase"
-msgstr "Purchases"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.purchase-recreated-account.invoice,invoice:"
 msgid "Invoice"
-msgstr "Invoices"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.purchase-recreated-account.invoice,purchase:"
 msgid "Purchase"
-msgstr "Purchases"
+msgstr ""
 
 msgctxt "field:purchase.reporting.context,company:"
 msgid "Company"
 msgstr ""
 
 msgctxt "field:purchase.reporting.context,from_date:"
 msgid "From Date"
@@ -540,52 +527,45 @@
 msgid "To Date"
 msgstr ""
 
 msgctxt "field:purchase.reporting.context,warehouse:"
 msgid "Warehouse"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.reporting.product,product:"
 msgid "Product"
-msgstr "Product Suppliers"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.reporting.product,product_supplier:"
 msgid "Supplier's Product"
-msgstr "Product Suppliers"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.reporting.product.time_series,product:"
 msgid "Product"
-msgstr "Product Suppliers"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.reporting.product.time_series,product_supplier:"
 msgid "Supplier's Product"
-msgstr "Product Suppliers"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.reporting.supplier,supplier:"
 msgid "Supplier"
-msgstr "Product Suppliers"
+msgstr ""
 
-#, fuzzy
 msgctxt "field:purchase.reporting.supplier.time_series,supplier:"
 msgid "Supplier"
-msgstr "Product Suppliers"
+msgstr ""
 
 msgctxt "field:stock.location,supplier_return_location:"
 msgid "Supplier Return"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:stock.move,purchase:"
 msgid "Purchase"
-msgstr "Purchases"
+msgstr ""
 
 msgctxt "field:stock.move,purchase_exception_state:"
 msgid "Exception State"
 msgstr ""
 
 msgctxt "field:stock.move,supplier:"
 msgid "Supplier"
@@ -673,180 +653,167 @@
 
 msgctxt "help:stock.location,supplier_return_location:"
 msgid "If empty the Storage location is used."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
-msgstr "Invoices"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_open_supplier"
 msgid "Parties associated to Purchases"
-msgstr "Parties associated to Purchases"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_product_supplier_form"
 msgid "Suppliers"
-msgstr "Product Suppliers"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_product_supplier_price_form"
 msgid "Prices"
-msgstr "Prices"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_configuration_form"
 msgid "Configuration"
-msgstr "Configuration"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_purchase_form"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_purchase_invoice_relate"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.action,name:act_purchase_line_relate"
 msgid "Purchase Lines"
-msgstr "Purchases"
+msgstr "Звітність"
 
 msgctxt "model:ir.action,name:act_purchase_move_relate"
 msgid "Moves"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_relate"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_purchase_relate_simple"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_main_time_series"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_reporting_product"
 msgid "Purchases per Product"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_reporting_product_time_series"
 msgid "Purchases per Product"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_supplier"
 msgid "Purchases per Supplier"
-msgstr "Product Suppliers"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_supplier_time_series"
 msgid "Purchases per Supplier"
-msgstr "Product Suppliers"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_return_form"
 msgid "Returns"
-msgstr "Returns"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
-msgstr "Shipments"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:report_purchase"
 msgid "Purchase"
-msgstr "Purchase"
+msgstr ""
 
 msgctxt "model:ir.action,name:wizard_invoice_handle_exception"
 msgid "Handle Invoice Exception"
-msgstr "Handle Invoice Exception"
+msgstr ""
 
 msgctxt "model:ir.action,name:wizard_modify_header"
 msgid "Modify Header"
-msgstr "Modify Header"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action,name:wizard_return_purchase"
 msgid "Return Purchase"
-msgstr "Purchases"
+msgstr ""
 
 msgctxt "model:ir.action,name:wizard_shipment_handle_exception"
 msgid "Handle Shipment Exception"
-msgstr "Handle Shipment Exception"
+msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_form_domain_all"
 msgid "All"
-msgstr "All"
+msgstr ""
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_confirmed"
 msgid "Confirmed"
-msgstr "Confirmed"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_draft"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_exception"
 msgid "Exception"
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_processing"
 msgid "Processing"
-msgstr "Processing"
+msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_form_domain_quotation"
 msgid "Quotation"
-msgstr "Quotation"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_all"
 msgid "All"
-msgstr "All"
+msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_line_relate_done"
 msgid "Done"
 msgstr ""
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_purchase_line_relate_pending"
 msgid "Pending"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_all"
 msgid "All"
-msgstr "All"
+msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_done"
 msgid "Done"
 msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr ""
@@ -907,18 +874,17 @@
 "product \"%(product)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_reporting_company"
 msgid "Company"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_purchase_reporting_currency"
 msgid "Currency"
-msgstr "Product Suppliers"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_reporting_date"
 msgid "Date"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_purchase_reporting_expense"
 msgid "Expense"
@@ -949,49 +915,48 @@
 msgctxt "model:ir.message,text:msg_warehouse_required_for_quotation"
 msgid ""
 "To get a quote for the purchase \"%(purchase)s\" you must enter a warehouse."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:purchase_cancel_button"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:purchase_confirm_button"
 msgid "Confirm"
-msgstr "Confirm"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:purchase_draft_button"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:purchase_hande_invoice_exception_button"
 msgid "Handle Invoice Exception"
-msgstr "Handle Invoice Exception"
+msgstr ""
 
 msgctxt ""
 "model:ir.model.button,string:purchase_hande_shipment_exception_button"
 msgid "Handle Shipment Exception"
-msgstr "Handle Shipment Exception"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:purchase_manual_invoice_button"
 msgid "Create Invoice"
-msgstr "Invoices"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:purchase_modify_header_button"
 msgid "Modify Header"
-msgstr "Modify Header"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:purchase_process_button"
 msgid "Process"
-msgstr "Process"
+msgstr ""
 
 msgctxt "model:ir.model.button,string:purchase_quote_button"
 msgid "Quote"
-msgstr "Quote"
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_product_supplier_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_purchase_companies"
 msgid "User in companies"
@@ -1020,97 +985,85 @@
 msgstr ""
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_supplier_time_series_companies"
 msgid "User in companies"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.sequence,name:sequence_purchase"
 msgid "Purchase"
-msgstr "Purchase"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_purchase"
 msgid "Purchase"
-msgstr "Purchase"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configuration"
+msgstr "Налаштування"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_product_supplier"
 msgid "Suppliers"
-msgstr "Product Suppliers"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_purchase"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_purchase_configuration"
 msgid "Configuration"
-msgstr "Configuration"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_purchase_form"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "Reporting"
+msgstr "Звітність"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_reporting_purchase"
 msgid "Purchases"
-msgstr "Purchases"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_supplier"
 msgid "Associated to Purchases"
-msgstr "Parties associated to Purchases"
+msgstr ""
 
 msgctxt "model:party.party.customer_code,name:"
 msgid "Party Customer Code"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:party.party.supplier_currency,name:"
 msgid "Party Supplier Currency"
-msgstr "Product Suppliers"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:party.party.supplier_lead_time,name:"
 msgid "Supplier Lead Time"
-msgstr "Product Suppliers"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:purchase.configuration,name:"
 msgid "Purchase Configuration"
-msgstr "Purchase Configuration"
+msgstr ""
 
 msgctxt "model:purchase.configuration.purchase_method,name:"
 msgid "Purchase Configuration Purchase Method"
 msgstr ""
 
 msgctxt "model:purchase.configuration.sequence,name:"
 msgid "Purchase Configuration Sequence"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:purchase.handle.invoice.exception.ask,name:"
 msgid "Handle Invoice Exception"
-msgstr "Handle Invoice Exception"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:purchase.handle.shipment.exception.ask,name:"
 msgid "Handle Shipment Exception"
-msgstr "Handle Shipment Exception"
+msgstr ""
 
 msgctxt "model:purchase.line,name:"
 msgid "Purchase Line"
 msgstr ""
 
 msgctxt "model:purchase.line-account.tax,name:"
 msgid "Purchase Line - Tax"
@@ -1120,50 +1073,47 @@
 msgid "Purchase Line - Ignored Move"
 msgstr ""
 
 msgctxt "model:purchase.line-recreated-stock.move,name:"
 msgid "Purchase Line - Ignored Move"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:purchase.product_supplier,name:"
 msgid "Product Supplier"
-msgstr "Product Suppliers"
+msgstr ""
 
 msgctxt "model:purchase.product_supplier.price,name:"
 msgid "Product Supplier Price"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:purchase.purchase,name:"
 msgid "Purchase"
-msgstr "Purchases"
+msgstr ""
 
 msgctxt "model:purchase.purchase-ignored-account.invoice,name:"
 msgid "Purchase - Ignored Invoice"
 msgstr ""
 
 msgctxt "model:purchase.purchase-recreated-account.invoice,name:"
 msgid "Purchase - Recreated Invoice"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:purchase.reporting.context,name:"
 msgid "Purchase Reporting Context"
-msgstr "Purchase Configuration"
+msgstr ""
 
 #, fuzzy
 msgctxt "model:purchase.reporting.main,name:"
 msgid "Purchase Reporting"
-msgstr "Purchase Configuration"
+msgstr "Звітність"
 
 #, fuzzy
 msgctxt "model:purchase.reporting.main.time_series,name:"
 msgid "Purchase Reporting"
-msgstr "Purchase Configuration"
+msgstr "Звітність"
 
 msgctxt "model:purchase.reporting.product,name:"
 msgid "Purchase Reporting per Product"
 msgstr ""
 
 msgctxt "model:purchase.reporting.product.time_series,name:"
 msgid "Purchase Reporting per Product"
@@ -1173,31 +1123,29 @@
 msgid "Purchase Reporting per Supplier"
 msgstr ""
 
 msgctxt "model:purchase.reporting.supplier.time_series,name:"
 msgid "Purchase Reporting per Supplier"
 msgstr ""
 
-#, fuzzy
 msgctxt "model:purchase.return_purchase.start,name:"
 msgid "Return Purchase"
-msgstr "Purchases"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:res.group,name:group_purchase"
 msgid "Purchase"
-msgstr "Purchase"
+msgstr ""
 
 msgctxt "model:res.group,name:group_purchase_admin"
 msgid "Purchase Administrator"
-msgstr "Purchase Administrator"
+msgstr ""
 
 msgctxt "report:purchase.purchase:"
 msgid ":"
-msgstr ":"
+msgstr ""
 
 msgctxt "report:purchase.purchase:"
 msgid "Amount"
 msgstr ""
 
 msgctxt "report:purchase.purchase:"
 msgid "Customer Code:"
@@ -1335,42 +1283,37 @@
 msgid "Received"
 msgstr ""
 
 msgctxt "selection:purchase.purchase,shipment_state:"
 msgid "Waiting"
 msgstr ""
 
-#, fuzzy
 msgctxt "selection:purchase.purchase,state:"
 msgid "Cancelled"
-msgstr "Cancel"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:purchase.purchase,state:"
 msgid "Confirmed"
-msgstr "Confirm"
+msgstr ""
 
 msgctxt "selection:purchase.purchase,state:"
 msgid "Done"
 msgstr ""
 
-#, fuzzy
 msgctxt "selection:purchase.purchase,state:"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:purchase.purchase,state:"
 msgid "Processing"
-msgstr "Processing"
+msgstr ""
 
-#, fuzzy
 msgctxt "selection:purchase.purchase,state:"
 msgid "Quotation"
-msgstr "Quotation"
+msgstr ""
 
 msgctxt "selection:purchase.reporting.context,period:"
 msgid "Day"
 msgstr ""
 
 msgctxt "selection:purchase.reporting.context,period:"
 msgid "Month"
@@ -1384,18 +1327,17 @@
 msgid "Ignored"
 msgstr ""
 
 msgctxt "selection:stock.move,purchase_exception_state:"
 msgid "Recreated"
 msgstr ""
 
-#, fuzzy
 msgctxt "view:party.party:"
 msgid "Supplier"
-msgstr "Product Suppliers"
+msgstr ""
 
 msgctxt "view:product.template:"
 msgid "Suppliers"
 msgstr ""
 
 msgctxt "view:purchase.handle.invoice.exception.ask:"
 msgid "Choose invoices to recreate:"
@@ -1421,52 +1363,46 @@
 msgid "Taxes"
 msgstr ""
 
 msgctxt "view:purchase.purchase:"
 msgid "Other Info"
 msgstr ""
 
-#, fuzzy
 msgctxt "view:purchase.purchase:"
 msgid "Purchase"
-msgstr "Purchases"
+msgstr ""
 
 msgctxt "view:purchase.return_purchase.start:"
 msgid "Are you sure to return these/this purchase(s)?"
 msgstr ""
 
-#, fuzzy
 msgctxt "wizard_button:purchase.handle.invoice.exception,ask,end:"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr ""
 
 msgctxt "wizard_button:purchase.handle.invoice.exception,ask,handle:"
 msgid "OK"
 msgstr ""
 
-#, fuzzy
 msgctxt "wizard_button:purchase.handle.shipment.exception,ask,end:"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr ""
 
 msgctxt "wizard_button:purchase.handle.shipment.exception,ask,handle:"
 msgid "OK"
 msgstr ""
 
-#, fuzzy
 msgctxt "wizard_button:purchase.modify_header,start,end:"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr ""
 
 msgctxt "wizard_button:purchase.modify_header,start,modify:"
 msgid "Modify"
 msgstr ""
 
-#, fuzzy
 msgctxt "wizard_button:purchase.return_purchase,start,end:"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr ""
 
-#, fuzzy
 msgctxt "wizard_button:purchase.return_purchase,start,return_:"
 msgid "Return"
-msgstr "Returns"
+msgstr ""
```

### Comparing `trytond_purchase-7.0.3/locale/zh_CN.po` & `trytond_purchase-7.2.0/locale/zh_CN.po`

 * *Files 0% similar despite different names*

```diff
@@ -175,14 +175,19 @@
 msgid "From Location"
 msgstr "从位置"
 
 msgctxt "field:purchase.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "发票明细"
 
+#, fuzzy
+msgctxt "field:purchase.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "发票地址"
+
 msgctxt "field:purchase.line,moves:"
 msgid "Moves"
 msgstr "移动"
 
 msgctxt "field:purchase.line,moves_exception:"
 msgid "Moves Exception"
 msgstr "移动异常"
@@ -803,18 +808,19 @@
 msgid "Done"
 msgstr "完成"
 
 msgctxt "model:ir.action.act_window.domain,name:act_purchase_relate_pending"
 msgid "Pending"
 msgstr "待定"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_change_purchase_uom"
 msgid ""
-"You are trying to change the purchase unit of measurer on which the purchase"
-" prices are based."
+"You are trying to change the purchase unit of measure on which the purchase "
+"prices are based."
 msgstr "您正在试图更改采购价格依赖的采购计量单位."
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_purchase"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending purchases with "
 "company \"%(company)s\"."
 msgstr "你不能删除参与者 \"%(party)s\" ， 因为它与公司 \"%(company)s\" 有未完成的采购."
```

### Comparing `trytond_purchase-7.0.3/message.xml` & `trytond_purchase-7.2.0/message.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_purchase-7.0.3/message.xml` & `trytond_purchase-7.2.0/message.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
 <tryton>
   <data grouped="1">
     <record model="ir.message" id="msg_change_purchase_uom">
-      <field name="text">You are trying to change the purchase unit of measurer on which the purchase prices are based.</field>
+      <field name="text">You are trying to change the purchase unit of measure on which the purchase prices are based.</field>
     </record>
     <record model="ir.message" id="msg_erase_party_pending_purchase">
       <field name="text">You cannot erase party &quot;%(party)s&quot; while they have pending purchases with company &quot;%(company)s&quot;.</field>
     </record>
     <record model="ir.message" id="msg_warehouse_required_for_quotation">
       <field name="text">To get a quote for the purchase &quot;%(purchase)s&quot; you must enter a warehouse.</field>
     </record>
```

### Comparing `trytond_purchase-7.0.3/party.py` & `trytond_purchase-7.2.0/party.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from trytond.modules.company.model import (
     CompanyMultiValueMixin, CompanyValueMixin)
 from trytond.modules.party.exceptions import EraseError
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval, TimeDelta
 
 supplier_currency = fields.Many2One(
-    'currency.currency', "Supplier Currency",
+    'currency.currency', "Supplier Currency", ondelete='RESTRICT',
     help="Default currency for purchases from this party.")
 supplier_lead_time = fields.TimeDelta(
     "Lead Time",
     domain=['OR',
         ('supplier_lead_time', '=', None),
         ('supplier_lead_time', '>=', TimeDelta()),
         ],
```

### Comparing `trytond_purchase-7.0.3/party.xml` & `trytond_purchase-7.2.0/party.xml`

 * *Files 22% similar despite different names*

#### Comparing `trytond_purchase-7.0.3/party.xml` & `trytond_purchase-7.2.0/party.xml`

```diff
@@ -5,19 +5,21 @@
   <data>
     <record model="ir.ui.view" id="party_view_form">
       <field name="model">party.party</field>
       <field name="inherit" ref="party.party_view_form"/>
       <field name="name">party_form</field>
     </record>
     <record model="ir.model.field.access" id="access_party_supplier_currency">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'supplier_currency')]"/>
+      <field name="model">party.party</field>
+      <field name="field">supplier_currency</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_supplier_currency_group_sale">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'supplier_currency')]"/>
+      <field name="model">party.party</field>
+      <field name="field">supplier_currency</field>
       <field name="group" ref="group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_purchase-7.0.3/product.py` & `trytond_purchase-7.2.0/product.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from collections import defaultdict
 
 from sql import Literal
 from sql.aggregate import Count, Max
 
 from trytond.i18n import gettext
 from trytond.model import (
-    DeactivableMixin, Index, MatchMixin, ModelSQL, ModelView, fields,
-    sequence_ordered)
+    Index, MatchMixin, ModelSQL, ModelView, fields, sequence_ordered)
 from trytond.modules.currency.fields import Monetary
-from trytond.modules.product import price_digits, round_price
+from trytond.modules.product import (
+    ProductDeactivatableMixin, price_digits, round_price)
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Bool, Eval, If, TimeDelta
 from trytond.tools import (
     grouped_slice, is_full_text, lstrip_wildcard, reduce_ids)
 from trytond.transaction import Transaction
 
 from .exceptions import PurchaseUOMWarning
@@ -25,18 +25,15 @@
     __name__ = "product.template"
     purchasable = fields.Boolean("Purchasable")
     product_suppliers = fields.One2Many(
         'purchase.product_supplier', 'template', "Suppliers",
         states={
             'invisible': (~Eval('purchasable', False)
                 | ~Eval('context', {}).get('company')),
-            },
-        domain=[
-            If(~Eval('active'), ('active', '=', False), ()),
-            ])
+            })
     purchase_uom = fields.Many2One(
         'product.uom', "Purchase UoM",
         states={
             'invisible': ~Eval('purchasable'),
             'required': Eval('purchasable', False),
             },
         domain=[('category', '=', Eval('default_uom_category'))],
@@ -59,18 +56,15 @@
     def view_attributes(cls):
         return super(Template, cls).view_attributes() + [
             ('//page[@id="suppliers"]', 'states', {
                     'invisible': ~Eval('purchasable'),
                     })]
 
     def product_suppliers_used(self, **pattern):
-        # Skip rules to test pattern on all records
-        with Transaction().set_user(0):
-            template = self.__class__(self)
-        for product_supplier in template.product_suppliers:
+        for product_supplier in self.product_suppliers:
             if product_supplier.match(pattern):
                 yield product_supplier
 
     @classmethod
     def write(cls, *args):
         pool = Pool()
         Warning = pool.get('res.user.warning')
@@ -121,15 +115,14 @@
 class Product(metaclass=PoolMeta):
     __name__ = 'product.product'
 
     product_suppliers = fields.One2Many(
         'purchase.product_supplier', 'product', "Suppliers",
         domain=[
             ('template', '=', Eval('template')),
-            If(~Eval('active'), ('active', '=', False), ()),
             ],
         states={
             'invisible': (~Eval('purchasable', False)
                 | ~Eval('context', {}).get('company')),
             })
     purchase_price_uom = fields.Function(fields.Numeric(
             "Purchase Price", digits=price_digits), 'get_purchase_price_uom')
@@ -200,18 +193,15 @@
                     unit_price = Currency.compute(
                         line.purchase.currency, unit_price, currency,
                         round=False)
             prices[line.product.id] = round_price(unit_price)
         return prices
 
     def product_suppliers_used(self, **pattern):
-        # Skip rules to test pattern on all records
-        with Transaction().set_user(0):
-            product = self.__class__(self)
-        for product_supplier in product.product_suppliers:
+        for product_supplier in self.product_suppliers:
             if product_supplier.match(pattern):
                 yield product_supplier
         pattern['product'] = None
         yield from self.template.product_suppliers_used(**pattern)
 
     def _get_purchase_unit_price(self, quantity=0):
         return
@@ -314,40 +304,39 @@
                         'product': lambda d: product2new[d['product']],
                         'template': lambda d: template2new[d['template']],
                         })
         return new_products
 
 
 class ProductSupplier(
-        sequence_ordered(), DeactivableMixin, ModelSQL, ModelView, MatchMixin):
+        sequence_ordered(), ProductDeactivatableMixin, MatchMixin,
+        ModelSQL, ModelView):
     'Product Supplier'
     __name__ = 'purchase.product_supplier'
     template = fields.Many2One(
         'product.template', "Product",
         required=True, ondelete='CASCADE',
         domain=[
             If(Bool(Eval('product')),
                 ('products', '=', Eval('product')),
                 ()),
-            If(Eval('active'), ('active', '=', True), ()),
             ],
         states={
             'readonly': Eval('id', -1) >= 0,
             },
         context={
             'company': Eval('company', -1),
             },
         depends={'company'})
     product = fields.Many2One(
         'product.product', "Variant",
         domain=[
             If(Bool(Eval('template')),
                 ('template', '=', Eval('template')),
                 ()),
-            If(Eval('active'), ('active', '=', True), ()),
             ],
         states={
             'readonly': Eval('id', -1) >= 0,
             },
         context={
             'company': Eval('company', -1),
             },
```

### Comparing `trytond_purchase-7.0.3/product.xml` & `trytond_purchase-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/purchase.fodt` & `trytond_purchase-7.2.0/purchase.fodt`

 * *Files 2% similar despite different names*

#### Comparing `trytond_purchase-7.0.3/purchase.fodt` & `trytond_purchase-7.2.0/purchase.fodt`

```diff
@@ -609,15 +609,15 @@
   <office:master-styles>
     <style:master-page style:name="Standard" style:page-layout-name="pm1" draw:style-name="dp1">
       <style:header>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;if test=&quot;company and company.header&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
-          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.header.split('\n')&quot;&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.header_used.split('\n')&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;line&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P1">
           <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
         </text:p>
@@ -629,15 +629,15 @@
         </text:p>
       </style:header>
       <style:footer>
         <text:p text:style-name="P2">
           <text:placeholder text:placeholder-type="text">&lt;if test=&quot;company and company.footer&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
-          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.footer.split('\n')&quot;&gt;</text:placeholder>
+          <text:placeholder text:placeholder-type="text">&lt;for each=&quot;line in company.footer_used.split('\n')&quot;&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
           <text:placeholder text:placeholder-type="text">&lt;line&gt;</text:placeholder>
         </text:p>
         <text:p text:style-name="P2">
           <text:placeholder text:placeholder-type="text">&lt;/for&gt;</text:placeholder>
         </text:p>
@@ -802,37 +802,22 @@
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
         </table:table-row>
         <table:table-row>
           <table:table-cell table:style-name="Table1.A5" office:value-type="string">
-            <text:p text:style-name="P26">
-              <text:placeholder text:placeholder-type="text">&lt;choose&gt;</text:placeholder>
-            </text:p>
-            <text:p text:style-name="P26">
-              <text:placeholder text:placeholder-type="text">&lt;when test=&quot;line.product_supplier&quot;&gt;</text:placeholder>
-            </text:p>
-            <text:p text:style-name="P25">
-              <text:placeholder text:placeholder-type="text">&lt;line.product_supplier.rec_name&gt;</text:placeholder>
-            </text:p>
-            <text:p text:style-name="P25">
-              <text:placeholder text:placeholder-type="text">&lt;/when&gt;</text:placeholder>
-            </text:p>
-            <text:p text:style-name="P25">
-              <text:placeholder text:placeholder-type="text">&lt;when test=&quot;line.product&quot;&gt;</text:placeholder>
-            </text:p>
             <text:p text:style-name="P25">
-              <text:placeholder text:placeholder-type="text">&lt;line.product.rec_name&gt;</text:placeholder>
+              <text:placeholder text:placeholder-type="text">&lt;if test=&quot;line.product_name&quot;&gt;</text:placeholder>
             </text:p>
             <text:p text:style-name="P25">
-              <text:placeholder text:placeholder-type="text">&lt;/when&gt;</text:placeholder>
+              <text:placeholder text:placeholder-type="text">&lt;line.product_name&gt;</text:placeholder>
             </text:p>
             <text:p text:style-name="P25">
-              <text:placeholder text:placeholder-type="text">&lt;/choose&gt;</text:placeholder>
+              <text:placeholder text:placeholder-type="text">&lt;/if&gt;</text:placeholder>
             </text:p>
             <text:p text:style-name="P25">
               <text:placeholder text:placeholder-type="text">&lt;if test=&quot;line.description&quot;&gt;</text:placeholder>
             </text:p>
             <text:p text:style-name="P25">
               <text:placeholder text:placeholder-type="text">&lt;for each=&quot;description in line.description.split('\n')&quot;&gt;</text:placeholder>
             </text:p>
```

### Comparing `trytond_purchase-7.0.3/purchase.py` & `trytond_purchase-7.2.0/purchase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
+import math
 from collections import defaultdict
 from decimal import Decimal
 from itertools import chain, groupby
 
-from sql import Literal
+from sql import Literal, Null
 from sql.aggregate import Count
 from sql.functions import CharLength
 
+from trytond import backend
 from trytond.i18n import gettext
 from trytond.ir.attachment import AttachmentCopyMixin
 from trytond.ir.note import NoteCopyMixin
 from trytond.model import (
     Index, Model, ModelSQL, ModelView, Unique, Workflow, fields,
     sequence_ordered)
 from trytond.model.exceptions import AccessError
@@ -21,15 +23,15 @@
 from trytond.modules.company import CompanyReport
 from trytond.modules.company.model import (
     employee_field, reset_employee, set_employee)
 from trytond.modules.currency.fields import Monetary
 from trytond.modules.product import price_digits
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, If, PYSONEncoder
-from trytond.tools import firstline
+from trytond.tools import cached_property, firstline
 from trytond.transaction import Transaction
 from trytond.wizard import (
     Button, StateAction, StateTransition, StateView, Wizard)
 
 from .exceptions import (
     PartyLocationError, PurchaseMoveQuantity, PurchaseQuotationError)
 
@@ -119,14 +121,15 @@
     invoice_party = fields.Many2One('party.party', "Invoice Party",
         states={
             'readonly': ((Eval('state') != 'draft')
                 | Eval('lines', [0])),
             },
         context={
             'company': Eval('company', -1),
+            'party_contact_mechanism_usage': 'invoice',
             },
         search_context={
             'related_party': Eval('party'),
             },
         depends={'company'})
     invoice_address = fields.Many2One('party.address', 'Invoice Address',
         domain=[
@@ -176,16 +179,23 @@
             ('paid', 'Paid'),
             ('exception', 'Exception'),
             ], 'Invoice State', readonly=True, required=True, sort=False)
     invoices = fields.Function(fields.Many2Many(
             'account.invoice', None, None, "Invoices"),
         'get_invoices', searcher='search_invoices')
     invoices_ignored = fields.Many2Many(
-            'purchase.purchase-ignored-account.invoice',
-            'purchase', 'invoice', 'Ignored Invoices', readonly=True)
+        'purchase.purchase-ignored-account.invoice',
+        'purchase', 'invoice', "Ignored Invoices",
+        domain=[
+            ('id', 'in', Eval('invoices', [])),
+            ('state', '=', 'cancelled'),
+            ],
+        states={
+            'invisible': ~Eval('invoices_ignored', []),
+            })
     invoices_recreated = fields.Many2Many(
             'purchase.purchase-recreated-account.invoice',
             'purchase', 'invoice', 'Recreated Invoices', readonly=True)
     origin = fields.Reference(
         "Origin", selection='get_origin',
         states={
             'readonly': Eval('state') != 'draft',
@@ -295,15 +305,15 @@
                             ()),
                         ],
                     'invisible': Eval('state') != 'quotation',
                     'depends': ['state'],
                     },
                 'process': {
                     'invisible': ~Eval('state').in_(
-                        ['confirmed', 'processing']),
+                        ['confirmed', 'processing', 'done']),
                     'icon': If(Eval('state') == 'confirmed',
                         'tryton-forward', 'tryton-refresh'),
                     'depends': ['state'],
                     },
                 'manual_invoice': {
                     'invisible': (
                         (Eval('invoice_method') != 'manual')
@@ -345,15 +355,17 @@
         cursor.execute(*sql_table.update(
                 [sql_table.invoice_state], ['pending'],
                 where=sql_table.invoice_state == 'waiting'))
 
     @classmethod
     def order_number(cls, tables):
         table, _ = tables[None]
-        return [CharLength(table.number), table.number]
+        return [
+            ~((table.state == 'cancelled') & (table.number == Null)),
+            CharLength(table.number), table.number]
 
     @classmethod
     def default_warehouse(cls):
         Location = Pool().get('stock.location')
         return Location.get_default_warehouse()
 
     @staticmethod
@@ -598,18 +610,18 @@
     search_shipment_returns = search_shipments_returns(
         'stock.shipment.in.return')
 
     def get_shipment_state(self):
         '''
         Return the shipment state for the purchase.
         '''
-        if self.moves:
-            if any(l.moves_exception for l in self.lines):
-                return 'exception'
-            elif all(l.moves_progress >= 1 for l in self.lines
+        if any(l.moves_exception for l in self.lines):
+            return 'exception'
+        elif any(m.state != 'cancelled' for m in self.moves):
+            if all(l.moves_progress >= 1 for l in self.lines
                     if l.moves_progress is not None):
                 return 'received'
             elif any(l.moves_progress for l in self.lines):
                 return 'partially shipped'
             else:
                 return 'waiting'
         return 'none'
@@ -832,19 +844,24 @@
         return_shipment = self._get_return_shipment()
         return_shipment.moves = return_moves
         return return_shipment
 
     def is_done(self):
         return ((self.invoice_state == 'paid'
                 or (self.invoice_state == 'none'
-                    and self.invoice_method != 'manual'))
+                    and all(
+                        l.invoice_progress >= 1
+                        for l in self.lines
+                        if l.invoice_progress is not None)))
             and (self.shipment_state == 'received'
-                or self.shipment_state == 'none'
-                or all(l.product.type == 'service'
-                    for l in self.lines if l.product)))
+                or (self.shipment_state == 'none'
+                    and all(
+                        l.moves_progress >= 1
+                        for l in self.lines
+                        if l.moves_progress is not None))))
 
     @classmethod
     def delete(cls, purchases):
         # Cancel before delete
         cls.cancel(purchases)
         for purchase in purchases:
             if purchase.state != 'cancelled':
@@ -1031,29 +1048,49 @@
     def modify_header(cls, purchases):
         pass
 
 
 class PurchaseIgnoredInvoice(ModelSQL):
     'Purchase - Ignored Invoice'
     __name__ = 'purchase.purchase-ignored-account.invoice'
-    _table = 'purchase_invoice_ignored_rel'
     purchase = fields.Many2One(
         'purchase.purchase', "Purchase", ondelete='CASCADE', required=True)
     invoice = fields.Many2One(
-        'account.invoice', "Invoice", ondelete='RESTRICT', required=True)
+        'account.invoice', "Invoice", ondelete='RESTRICT', required=True,
+        domain=[
+            ('purchases', '=', Eval('purchase', -1)),
+            ('state', '=', 'cancelled'),
+            ])
+
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'purchase_invoice_ignored_rel', cls._table)
+        super().__register__(module)
 
 
 class PurchaseRecreatedInvoice(ModelSQL):
     'Purchase - Recreated Invoice'
     __name__ = 'purchase.purchase-recreated-account.invoice'
-    _table = 'purchase_invoice_recreated_rel'
     purchase = fields.Many2One(
         'purchase.purchase', "Purchase", ondelete='CASCADE', required=True)
     invoice = fields.Many2One(
-        'account.invoice', "Invoice", ondelete='RESTRICT', required=True)
+        'account.invoice', "Invoice", ondelete='RESTRICT', required=True,
+        domain=[
+            ('purchases', '=', Eval('purchase', -1)),
+            ('state', '=', 'cancelled'),
+            ])
+
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'purchase_invoice_recreated_rel', cls._table)
+        super().__register__(module)
 
 
 class Line(sequence_ordered(), ModelSQL, ModelView):
     'Purchase Line'
     __name__ = 'purchase.line'
     purchase = fields.Many2One(
         'purchase.purchase', "Purchase", ondelete='CASCADE', required=True,
@@ -1213,21 +1250,32 @@
             'readonly': Eval('purchase_state') != 'draft',
             })
     invoice_lines = fields.One2Many(
         'account.invoice.line', 'origin', "Invoice Lines", readonly=True,
         states={
             'invisible': ~Eval('invoice_lines'),
             })
+    invoice_progress = fields.Function(
+        fields.Float("Invoice Progress", digits=(1, 4)),
+        'get_invoice_progress')
     moves = fields.One2Many(
         'stock.move', 'origin', "Moves", readonly=True,
         states={
             'invisible': ~Eval('moves'),
             })
-    moves_ignored = fields.Many2Many('purchase.line-ignored-stock.move',
-            'purchase_line', 'move', 'Ignored Moves', readonly=True)
+    moves_ignored = fields.Many2Many(
+        'purchase.line-ignored-stock.move', 'purchase_line', 'move',
+        "Ignored Moves",
+        domain=[
+            ('id', 'in', Eval('moves', [])),
+            ('state', '=', 'cancelled'),
+            ],
+        states={
+            'invisible': ~Eval('moves_ignored'),
+            })
     moves_recreated = fields.Many2Many('purchase.line-recreated-stock.move',
             'purchase_line', 'move', 'Recreated Moves', readonly=True)
     moves_exception = fields.Function(
         fields.Boolean("Moves Exception"), 'get_moves_exception')
     moves_progress = fields.Function(
         fields.Float("Moves Progress", digits=(1, 4)),
         'get_moves_progress')
@@ -1305,27 +1353,61 @@
         cls._order.insert(0, ('purchase.purchase_date', 'DESC NULLS FIRST'))
         cls._order.insert(1, ('purchase.id', 'DESC'))
 
     @staticmethod
     def default_type():
         return 'line'
 
-    @fields.depends('type')
+    @fields.depends('type', 'taxes')
     def on_change_type(self):
         if self.type != 'line':
             self.product = None
             self.product_supplier = None
             self.unit = None
             self.taxes = None
 
     @classmethod
     def default_delivery_date_edit(cls):
         return False
 
     @property
+    def _invoice_remaining_quantity(self):
+        "Compute the remaining quantity to be paid"
+        pool = Pool()
+        UoM = pool.get('product.uom')
+        if self.type != 'line':
+            return
+        skips = set(self.purchase.invoices_ignored)
+        quantity = self.quantity
+        if self.purchase.invoice_method == 'shipment':
+            moves_ignored = set(self.moves_ignored)
+            for move in self.moves:
+                if move in moves_ignored:
+                    quantity -= UoM.compute_qty(
+                        move.unit, math.copysign(move.quantity, self.quantity),
+                        self.unit)
+        for invoice_line in self.invoice_lines:
+            if invoice_line.type != 'line':
+                continue
+            if (invoice_line.invoice.state == 'paid'
+                    or invoice_line.invoice in skips):
+                quantity -= UoM.compute_qty(
+                    invoice_line.unit or self.unit, invoice_line.quantity,
+                    self.unit)
+        return quantity
+
+    def get_invoice_progress(self, name):
+        progress = None
+        quantity = self._invoice_remaining_quantity
+        if quantity is not None and self.quantity:
+            progress = round((self.quantity - quantity) / self.quantity, 4)
+            progress = max(0., min(1., progress))
+        return progress
+
+    @property
     def _move_remaining_quantity(self):
         "Compute the remaining quantity to receive"
         pool = Pool()
         Uom = pool.get('product.uom')
         if self.type != 'line' or not self.product:
             return
         if self.product.type == 'service':
@@ -1346,15 +1428,15 @@
 
     def get_moves_progress(self, name):
         progress = None
         quantity = self._move_remaining_quantity
         if quantity is not None and self.quantity:
             progress = round(
                 (abs(self.quantity) - quantity) / abs(self.quantity), 4)
-            progress = max(0, min(1, progress))
+            progress = max(0., min(1., progress))
         return progress
 
     def _get_tax_rule_pattern(self):
         '''
         Get tax rule pattern
         '''
         return {}
@@ -1388,24 +1470,26 @@
             'party': (
                 self.purchase.party.id
                 if self.purchase and self.purchase.party else -1),
             'company': (self.company.id if self.company else -1),
             }
 
     @fields.depends(
-        'purchase', '_parent_purchase.party', '_parent_purchase.invoice_party',
+        'purchase', 'taxes',
+        '_parent_purchase.party', '_parent_purchase.invoice_party',
         methods=['compute_taxes', 'on_change_with_amount'])
     def on_change_purchase(self):
         party = None
         if self.purchase:
             party = self.purchase.invoice_party or self.purchase.party
         self.taxes = self.compute_taxes(party)
         self.amount = self.on_change_with_amount()
 
-    @fields.depends('product', 'unit', 'purchase',
+    @fields.depends(
+        'product', 'unit', 'purchase', 'taxes',
         '_parent_purchase.party', '_parent_purchase.invoice_party',
         'product_supplier', methods=['compute_taxes', 'compute_unit_price',
             '_get_product_supplier_pattern'])
     def on_change_product(self):
         party = None
         if self.purchase:
             party = self.purchase.invoice_party or self.purchase.party
@@ -1427,14 +1511,23 @@
                     and self.product_supplier not in product_suppliers):
                 self.product_supplier = None
 
             self.unit_price = self.compute_unit_price()
 
         self.amount = self.on_change_with_amount()
 
+    @cached_property
+    def product_name(self):
+        if self.product_supplier:
+            return self.product_supplier.rec_name
+        elif self.product:
+            return self.product.rec_name
+        else:
+            return ''
+
     @fields.depends(
         'type', 'product',
         methods=['on_change_with_company', '_get_tax_rule_pattern'])
     def compute_taxes(self, party):
         pool = Pool()
         AccountConfiguration = pool.get('account.configuration')
 
@@ -1962,15 +2055,14 @@
         default.setdefault('actual_quantity')
         return super().copy(lines, default=default)
 
 
 class LineTax(ModelSQL):
     'Purchase Line - Tax'
     __name__ = 'purchase.line-account.tax'
-    _table = 'purchase_line_account_tax'
     line = fields.Many2One(
         'purchase.line', "Purchase Line", ondelete='CASCADE', required=True,
         domain=[('type', '=', 'line')])
     tax = fields.Many2One(
         'account.tax', "Tax", ondelete='RESTRICT', required=True,
         domain=[('parent', '=', None)])
 
@@ -1979,33 +2071,60 @@
         super().__setup__()
         t = cls.__table__()
         cls._sql_constraints += [
             ('line_tax_unique', Unique(t, t.line, t.tax),
                 'purchase.msg_purchase_line_tax_unique'),
             ]
 
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'purchase_line_account_tax', cls._table)
+        super().__register__(module)
+
 
 class LineIgnoredMove(ModelSQL):
     'Purchase Line - Ignored Move'
     __name__ = 'purchase.line-ignored-stock.move'
-    _table = 'purchase_line_moves_ignored_rel'
     purchase_line = fields.Many2One(
         'purchase.line', "Purchase Line", ondelete='CASCADE', required=True)
     move = fields.Many2One(
-        'stock.move', "Move", ondelete='RESTRICT', required=True)
+        'stock.move', "Move", ondelete='RESTRICT', required=True,
+        domain=[
+            ('origin.id', '=', Eval('purchase_line', -1), 'purchase.line'),
+            ('state', '=', 'cancelled'),
+            ])
+
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'purchase_line_moves_ignored_rel', cls._table)
+        super().__register__(module)
 
 
 class LineRecreatedMove(ModelSQL):
     'Purchase Line - Ignored Move'
     __name__ = 'purchase.line-recreated-stock.move'
-    _table = 'purchase_line_moves_recreated_rel'
     purchase_line = fields.Many2One(
         'purchase.line', "Purchase Line", ondelete='CASCADE', required=True)
     move = fields.Many2One(
-        'stock.move', "Move", ondelete='RESTRICT', required=True)
+        'stock.move', "Move", ondelete='RESTRICT', required=True,
+        domain=[
+            ('origin.id', '=', Eval('purchase_line', -1), 'purchase.line'),
+            ('state', '=', 'cancelled'),
+            ])
+
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'purchase_line_moves_recreated_rel', cls._table)
+        super().__register__(module)
 
 
 class PurchaseReport(CompanyReport):
     __name__ = 'purchase.purchase'
 
     @classmethod
     def execute(cls, ids, data):
```

### Comparing `trytond_purchase-7.0.3/purchase.xml` & `trytond_purchase-7.2.0/purchase.xml`

 * *Files 8% similar despite different names*

#### Comparing `trytond_purchase-7.0.3/purchase.xml` & `trytond_purchase-7.2.0/purchase.xml`

```diff
@@ -197,100 +197,112 @@
     </record>
     <record model="ir.action.keyword" id="act_purchase_relate_simple_keyword_shipment_in_return">
       <field name="keyword">form_relate</field>
       <field name="model">stock.shipment.in.return,-1</field>
       <field name="action" ref="act_purchase_relate_simple"/>
     </record>
     <record model="ir.model.access" id="access_purchase">
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
+      <field name="model">purchase.purchase</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_purchase_purchase">
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
+      <field name="model">purchase.purchase</field>
       <field name="group" ref="group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.access" id="access_purchase_account">
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
+      <field name="model">purchase.purchase</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_purchase_group_stock">
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
+      <field name="model">purchase.purchase</field>
       <field name="group" ref="stock.group_stock"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
+    <record model="ir.model.field.access" id="access_purchase_purchase_invoices_ignored">
+      <field name="model">purchase.purchase</field>
+      <field name="field">invoices_ignored</field>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="False"/>
+    </record>
+    <record model="ir.model.field.access" id="access_purchase_purchase_invoices_ignored_purchase_admin">
+      <field name="model">purchase.purchase</field>
+      <field name="field">invoices_ignored</field>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="True"/>
+    </record>
     <record model="ir.model.button" id="purchase_cancel_button">
+      <field name="model">purchase.purchase</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
     </record>
     <record model="ir.model.button" id="purchase_draft_button">
+      <field name="model">purchase.purchase</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
     </record>
     <record model="ir.model.button" id="purchase_quote_button">
+      <field name="model">purchase.purchase</field>
       <field name="name">quote</field>
       <field name="string">Quote</field>
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
     </record>
     <record model="ir.model.button" id="purchase_confirm_button">
+      <field name="model">purchase.purchase</field>
       <field name="name">confirm</field>
       <field name="string">Confirm</field>
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
     </record>
     <record model="ir.model.button" id="purchase_process_button">
+      <field name="model">purchase.purchase</field>
       <field name="name">process</field>
       <field name="string">Process</field>
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
     </record>
     <record model="ir.model.button-res.group" id="purchase_process_button_group_purchase_admin">
       <field name="button" ref="purchase_process_button"/>
       <field name="group" ref="group_purchase_admin"/>
     </record>
     <record model="ir.model.button" id="purchase_manual_invoice_button">
+      <field name="model">purchase.purchase</field>
       <field name="name">manual_invoice</field>
       <field name="string">Create Invoice</field>
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
     </record>
     <record model="ir.model.button-res.group" id="purchase_manual_button_group_purchase">
       <field name="button" ref="purchase_manual_invoice_button"/>
       <field name="group" ref="group_purchase"/>
     </record>
     <record model="ir.model.button-res.group" id="purchase_manual_button_group_account">
       <field name="button" ref="purchase_manual_invoice_button"/>
       <field name="group" ref="account.group_account"/>
     </record>
     <record model="ir.model.button" id="purchase_modify_header_button">
+      <field name="model">purchase.purchase</field>
       <field name="name">modify_header</field>
       <field name="string">Modify Header</field>
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
     </record>
     <record model="ir.model.button" id="purchase_hande_invoice_exception_button">
+      <field name="model">purchase.purchase</field>
       <field name="name">handle_invoice_exception</field>
       <field name="string">Handle Invoice Exception</field>
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
     </record>
     <record model="ir.model.button" id="purchase_hande_shipment_exception_button">
+      <field name="model">purchase.purchase</field>
       <field name="name">handle_shipment_exception</field>
       <field name="string">Handle Shipment Exception</field>
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
     </record>
     <record model="ir.sequence.type" id="sequence_type_purchase">
       <field name="name">Purchase</field>
     </record>
     <record model="ir.sequence.type-res.group" id="sequence_type_purchase_group_admin">
       <field name="sequence_type" ref="sequence_type_purchase"/>
       <field name="group" ref="res.group_admin"/>
@@ -383,21 +395,33 @@
     </record>
     <record model="ir.action.keyword" id="act_purchase_line_relate_keyword_party">
       <field name="keyword">form_relate</field>
       <field name="model">party.party,-1</field>
       <field name="action" ref="act_purchase_line_relate"/>
     </record>
     <record model="ir.model.access" id="access_purchase_line_group_stock">
-      <field name="model" search="[('model', '=', 'purchase.line')]"/>
+      <field name="model">purchase.line</field>
       <field name="group" ref="stock.group_stock"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
+    <record model="ir.model.field.access" id="access_purchase_line_moves_ignored">
+      <field name="model">purchase.line</field>
+      <field name="field">moves_ignored</field>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="False"/>
+    </record>
+    <record model="ir.model.field.access" id="access_purchase_line_moves_ignored_purchase_admin">
+      <field name="model">purchase.line</field>
+      <field name="field">moves_ignored</field>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="True"/>
+    </record>
     <record model="ir.ui.view" id="product_supplier_view_form">
       <field name="model">purchase.product_supplier</field>
       <field name="type">form</field>
       <field name="name">product_supplier_form</field>
     </record>
     <record model="ir.ui.view" id="product_supplier_view_tree">
       <field name="model">purchase.product_supplier</field>
@@ -423,31 +447,31 @@
     <record model="ir.action.act_window.view" id="act_product_supplier_form_view">
       <field name="sequence" eval="20"/>
       <field name="view" ref="product_supplier_view_form"/>
       <field name="act_window" ref="act_product_supplier_form"/>
     </record>
     <menuitem parent="product.menu_template" sequence="20" action="act_product_supplier_form" id="menu_product_supplier"/>
     <record model="ir.model.access" id="access_product_supplier">
-      <field name="model" search="[('model', '=', 'purchase.product_supplier')]"/>
+      <field name="model">purchase.product_supplier</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_product_supplier_purchase">
-      <field name="model" search="[('model', '=', 'purchase.product_supplier')]"/>
+      <field name="model">purchase.product_supplier</field>
       <field name="group" ref="group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_product_supplier_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'purchase.product_supplier')]"/>
+      <field name="model">purchase.product_supplier</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_product_supplier_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_product_supplier_companies"/>
     </record>
     <record model="ir.ui.view" id="product_supplier_price_view_form">
@@ -504,15 +528,15 @@
       <field name="model">purchase.purchase</field>
       <field name="inherit" ref="purchase.purchase_view_form"/>
       <field name="name">modify_header_form</field>
       <field name="domain" eval="Eval('context', {}).get('modify_header', False)" pyson="1"/>
     </record>
     <record model="ir.rule.group" id="rule_group_purchase_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'purchase.purchase')]"/>
+      <field name="model">purchase.purchase</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_purchase_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_purchase_companies"/>
     </record>
   </data>
```

### Comparing `trytond_purchase-7.0.3/purchase_reporting.py` & `trytond_purchase-7.2.0/purchase_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/purchase_reporting.xml` & `trytond_purchase-7.2.0/purchase_reporting.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_purchase-7.0.3/purchase_reporting.xml` & `trytond_purchase-7.2.0/purchase_reporting.xml`

```diff
@@ -37,30 +37,30 @@
     <record model="ir.action.keyword" id="act_reporting_main_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model" ref="menu_reporting_purchase"/>
       <field name="action" ref="act_reporting_main"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_main_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'purchase.reporting.main')]"/>
+      <field name="model">purchase.reporting.main</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_main_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_main_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_main">
-      <field name="model" search="[('model', '=', 'purchase.reporting.main')]"/>
+      <field name="model">purchase.reporting.main</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_main_purchase">
-      <field name="model" search="[('model', '=', 'purchase.reporting.main')]"/>
+      <field name="model">purchase.reporting.main</field>
       <field name="group" ref="group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="reporting_main_time_series_view_list">
@@ -102,30 +102,30 @@
     <record model="ir.action.keyword" id="act_reporting_main_time_series_list_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">purchase.reporting.main,-1</field>
       <field name="action" ref="act_reporting_main_time_series"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_main_time_series_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'purchase.reporting.main.time_series')]"/>
+      <field name="model">purchase.reporting.main.time_series</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_main_time_series_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_main_time_series_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_main_time_series">
-      <field name="model" search="[('model', '=', 'purchase.reporting.main.time_series')]"/>
+      <field name="model">purchase.reporting.main.time_series</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_main_time_series_purchase">
-      <field name="model" search="[('model', '=', 'purchase.reporting.main.time_series')]"/>
+      <field name="model">purchase.reporting.main.time_series</field>
       <field name="group" ref="group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <!-- Supplier -->
@@ -167,30 +167,30 @@
     <record model="ir.action.keyword" id="act_reporting_supplier_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model" ref="menu_reporting_purchase"/>
       <field name="action" ref="act_reporting_supplier"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_supplier_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'purchase.reporting.supplier')]"/>
+      <field name="model">purchase.reporting.supplier</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_supplier_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_supplier_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_supplier">
-      <field name="model" search="[('model', '=', 'purchase.reporting.supplier')]"/>
+      <field name="model">purchase.reporting.supplier</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_supplier_purchase">
-      <field name="model" search="[('model', '=', 'purchase.reporting.supplier')]"/>
+      <field name="model">purchase.reporting.supplier</field>
       <field name="group" ref="group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="reporting_supplier_time_series_view_list">
@@ -233,30 +233,30 @@
     <record model="ir.action.keyword" id="act_reporting_supplier_time_series_list_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">purchase.reporting.supplier,-1</field>
       <field name="action" ref="act_reporting_supplier_time_series"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_supplier_time_series_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'purchase.reporting.supplier.time_series')]"/>
+      <field name="model">purchase.reporting.supplier.time_series</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_supplier_time_series_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_supplier_time_series_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_supplier_time_series">
-      <field name="model" search="[('model', '=', 'purchase.reporting.supplier.time_series')]"/>
+      <field name="model">purchase.reporting.supplier.time_series</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_supplier_time_series_purchase">
-      <field name="model" search="[('model', '=', 'purchase.reporting.supplier.time_series')]"/>
+      <field name="model">purchase.reporting.supplier.time_series</field>
       <field name="group" ref="group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <!-- Product -->
@@ -299,30 +299,30 @@
     <record model="ir.action.keyword" id="act_reporting_product_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">purchase.reporting.supplier,-1</field>
       <field name="action" ref="act_reporting_product"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_product_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'purchase.reporting.product')]"/>
+      <field name="model">purchase.reporting.product</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_product_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_product_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_product">
-      <field name="model" search="[('model', '=', 'purchase.reporting.product')]"/>
+      <field name="model">purchase.reporting.product</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_product_purchase">
-      <field name="model" search="[('model', '=', 'purchase.reporting.product')]"/>
+      <field name="model">purchase.reporting.product</field>
       <field name="group" ref="group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="reporting_product_time_series_view_list">
@@ -365,30 +365,30 @@
     <record model="ir.action.keyword" id="act_reporting_product_time_series_list_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">purchase.reporting.product,-1</field>
       <field name="action" ref="act_reporting_product_time_series"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_product_time_series_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'purchase.reporting.product.time_series')]"/>
+      <field name="model">purchase.reporting.product.time_series</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_product_time_series_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_product_time_series_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_product_time_series">
-      <field name="model" search="[('model', '=', 'purchase.reporting.product.time_series')]"/>
+      <field name="model">purchase.reporting.product.time_series</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_product_time_series_purchase">
-      <field name="model" search="[('model', '=', 'purchase.reporting.product.time_series')]"/>
+      <field name="model">purchase.reporting.product.time_series</field>
       <field name="group" ref="group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_purchase-7.0.3/setup.py` & `trytond_purchase-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/stock.py` & `trytond_purchase-7.2.0/stock.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from functools import wraps
 
 from trytond.i18n import gettext
 from trytond.model import ModelView, Workflow, fields
 from trytond.model.exceptions import AccessError
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval
+from trytond.tools import cached_property
 from trytond.transaction import Transaction, without_check_access
 
 
 def process_purchase(moves_field):
     def _process_purchase(func):
         @wraps(func)
         def wrapper(cls, shipments):
@@ -102,16 +103,16 @@
 
         return super(ShipmentInReturn, cls).draft(shipments)
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
     @process_purchase('moves')
-    def done(cls, shipments):
-        super(ShipmentInReturn, cls).done(shipments)
+    def do(cls, shipments):
+        super().do(shipments)
 
 
 def process_purchase_move(without_shipment=False):
     def _process_purchase_move(func):
         @wraps(func)
         def wrapper(cls, moves):
             pool = Pool()
@@ -182,14 +183,24 @@
             return 'ignored'
 
     def get_supplier(self, name):
         PurchaseLine = Pool().get('purchase.line')
         if isinstance(self.origin, PurchaseLine):
             return self.origin.purchase.party.id
 
+    @cached_property
+    def product_name(self):
+        pool = Pool()
+        PurchaseLine = pool.get('purchase.line')
+        name = super().product_name
+        if (isinstance(self.origin, PurchaseLine)
+                and self.origin.product_supplier):
+            name = self.origin.product_supplier.rec_name
+        return name
+
     @fields.depends('origin')
     def on_change_with_product_uom_category(self, name=None):
         pool = Pool()
         PurchaseLine = pool.get('purchase.line')
         category = super(Move, self).on_change_with_product_uom_category(
             name=name)
         # Enforce the same unit category as they are used to compute the
```

### Comparing `trytond_purchase-7.0.3/stock.xml` & `trytond_purchase-7.2.0/stock.xml`

 * *Files 3% similar despite different names*

#### Comparing `trytond_purchase-7.0.3/stock.xml` & `trytond_purchase-7.2.0/stock.xml`

```diff
@@ -6,15 +6,15 @@
     <record model="ir.ui.view" id="move_view_list_shipment">
       <field name="model">stock.move</field>
       <field name="type">tree</field>
       <field name="priority" eval="20"/>
       <field name="name">move_list_shipment</field>
     </record>
     <record model="ir.model.access" id="access_move_group_purchase">
-      <field name="model" search="[('model', '=', 'stock.move')]"/>
+      <field name="model">stock.move</field>
       <field name="group" ref="group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="location_view_form">
@@ -54,15 +54,15 @@
     </record>
     <record model="ir.action.keyword" id="act_open_shipment_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">purchase.purchase,-1</field>
       <field name="action" ref="act_shipment_form"/>
     </record>
     <record model="ir.model.access" id="access_shipment_in_group_purchase">
-      <field name="model" search="[('model', '=', 'stock.shipment.in')]"/>
+      <field name="model">stock.shipment.in</field>
       <field name="group" ref="group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.action.act_window" id="act_return_form">
@@ -72,15 +72,15 @@
     </record>
     <record model="ir.action.keyword" id="act_open_shipment_return_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">purchase.purchase,-1</field>
       <field name="action" ref="act_return_form"/>
     </record>
     <record model="ir.model.access" id="access_shipment_in_return_group_purchase">
-      <field name="model" search="[('model', '=', 'stock.shipment.in.return')]"/>
+      <field name="model">stock.shipment.in.return</field>
       <field name="group" ref="group_purchase"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_purchase-7.0.3/tests/scenario_purchase.rst` & `trytond_purchase-7.2.0/tests/scenario_purchase.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 Purchase Scenario
 =================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from operator import attrgetter
-    >>> from proteus import Model, Wizard, Report
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
+
+    >>> from proteus import Model, Report
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, create_tax, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, set_user
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('purchase')
 
@@ -164,54 +163,47 @@
     >>> purchase.lines.append(purchase_line)
     >>> purchase_line.product = product
     >>> purchase_line.quantity = 3.0
     >>> purchase_line.unit_price = Decimal('5.0000')
     >>> purchase.click('quote')
     >>> purchase.untaxed_amount, purchase.tax_amount, purchase.total_amount
     (Decimal('25.00'), Decimal('2.50'), Decimal('27.50'))
-    >>> purchase.quoted_by == employee
-    True
+    >>> assertEqual(purchase.quoted_by, employee)
     >>> purchase.click('confirm')
     >>> purchase.untaxed_amount, purchase.tax_amount, purchase.total_amount
     (Decimal('25.00'), Decimal('2.50'), Decimal('27.50'))
-    >>> purchase.confirmed_by == employee
-    True
+    >>> assertEqual(purchase.confirmed_by, employee)
     >>> purchase.state
     'processing'
     >>> purchase.shipment_state
     'waiting'
     >>> purchase.invoice_state
     'pending'
     >>> len(purchase.moves), len(purchase.shipment_returns), len(purchase.invoices)
     (2, 0, 1)
     >>> invoice, = purchase.invoices
-    >>> invoice.origins == purchase.rec_name
-    True
+    >>> assertEqual(invoice.origins, purchase.rec_name)
     >>> invoice.untaxed_amount, invoice.tax_amount, invoice.total_amount
     (Decimal('25.00'), Decimal('2.50'), Decimal('27.50'))
 
 Invoice line must be linked to stock move::
 
     >>> invoice_line1, invoice_line2 = sorted(
     ...     invoice.lines, key=lambda l: l.quantity or 0)
     >>> stock_move1, stock_move2 = sorted(purchase.moves,
     ...     key=lambda m: m.quantity)
-    >>> invoice_line1.stock_moves == [stock_move1]
-    True
-    >>> stock_move1.invoice_lines == [invoice_line1]
-    True
-    >>> invoice_line2.stock_moves == [stock_move2]
-    True
-    >>> stock_move2.invoice_lines == [invoice_line2]
-    True
+    >>> assertEqual(invoice_line1.stock_moves, [stock_move1])
+    >>> assertEqual(stock_move1.invoice_lines, [invoice_line1])
+    >>> assertEqual(invoice_line2.stock_moves, [stock_move2])
+    >>> assertEqual(stock_move2.invoice_lines, [invoice_line2])
 
 Check actual quantity::
 
-    >>> all(l.quantity == l.actual_quantity for l in purchase.lines)
-    True
+    >>> for line in purchase.lines:
+    ...     assertEqual(line.quantity, line.actual_quantity)
 
 Post invoice and check no new invoices::
 
     >>> invoice.invoice_date = today
     >>> invoice.click('post')
     >>> purchase.reload()
     >>> purchase.shipment_state
@@ -265,18 +257,17 @@
     >>> ShipmentIn = Model.get('stock.shipment.in')
     >>> shipment = ShipmentIn()
     >>> shipment.supplier = supplier
     >>> for move in purchase.moves:
     ...     incoming_move = Move(id=move.id)
     ...     shipment.incoming_moves.append(incoming_move)
     >>> shipment.save()
-    >>> shipment.origins == purchase.rec_name
-    True
+    >>> assertEqual(shipment.origins, purchase.rec_name)
     >>> shipment.click('receive')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> purchase.reload()
     >>> purchase.shipment_state
     'received'
     >>> len(purchase.shipments), len(purchase.shipment_returns)
     (1, 0)
 
 Open supplier invoice::
@@ -292,18 +283,16 @@
     ...     line.quantity = 1
     ...     line.save()
     >>> invoice.invoice_date = today
     >>> invoice.click('post')
 
 Invoice lines must be linked to each stock moves::
 
-    >>> invoice_line1.stock_moves == [stock_move1]
-    True
-    >>> invoice_line2.stock_moves == [stock_move2]
-    True
+    >>> assertEqual(invoice_line1.stock_moves, [stock_move1])
+    >>> assertEqual(invoice_line2.stock_moves, [stock_move2])
 
 Check second invoices::
 
     >>> purchase.reload()
     >>> len(purchase.invoices)
     2
     >>> sum(l.quantity for i in purchase.invoices for l in i.lines)
@@ -352,15 +341,15 @@
     'waiting'
     >>> move_return, = ship_return.moves
     >>> move_return.product.rec_name
     'product'
     >>> move_return.quantity
     4.0
     >>> ship_return.click('assign_try')
-    >>> ship_return.click('done')
+    >>> ship_return.click('do')
     >>> ship_return.state
     'done'
     >>> return_.reload()
     >>> return_.state
     'processing'
     >>> return_.shipment_state
     'received'
@@ -415,22 +404,22 @@
     >>> mix_shipment.supplier = supplier
     >>> for move in mix.moves:
     ...     if move.id in [m.id for m in mix_return.moves]:
     ...         continue
     ...     incoming_move = Move(id=move.id)
     ...     mix_shipment.incoming_moves.append(incoming_move)
     >>> mix_shipment.click('receive')
-    >>> mix_shipment.click('done')
+    >>> mix_shipment.click('do')
     >>> mix.reload()
     >>> len(mix.shipments)
     1
 
     >>> mix_return.click('wait')
     >>> mix_return.click('assign_try')
-    >>> mix_return.click('done')
+    >>> mix_return.click('do')
     >>> move_return, = mix_return.moves
     >>> move_return.product.rec_name
     'product'
     >>> move_return.quantity
     2.0
 
 Checking the invoice::
@@ -482,22 +471,22 @@
     >>> mix_shipment.supplier = supplier
     >>> for move in mix.moves:
     ...     if move.id in [m.id for m in mix_return.moves]:
     ...         continue
     ...     incoming_move = Move(id=move.id)
     ...     mix_shipment.incoming_moves.append(incoming_move)
     >>> mix_shipment.click('receive')
-    >>> mix_shipment.click('done')
+    >>> mix_shipment.click('do')
     >>> mix.reload()
     >>> len(mix.shipments)
     1
 
     >>> mix_return.click('wait')
     >>> mix_return.click('assign_try')
-    >>> mix_return.click('done')
+    >>> mix_return.click('do')
     >>> move_return, = mix_return.moves
     >>> move_return.product.rec_name
     'product'
     >>> move_return.quantity
     3.0
 
 Purchase services::
@@ -560,15 +549,15 @@
     ...     incoming_move = Move(id=move.id)
     ...     incoming_move.quantity = 5.0
     ...     shipment.incoming_moves.append(incoming_move)
     >>> shipment.save()
     >>> for move in shipment.inventory_moves:
     ...     move.quantity = 5.0
     >>> shipment.click('receive')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> purchase.reload()
     >>> invoice, = purchase.invoices
     >>> invoice_line, = invoice.lines
     >>> invoice_line.quantity
     5.0
     >>> stock_move, = invoice_line.stock_moves
     >>> stock_move.quantity
@@ -594,15 +583,15 @@
     ...     incoming_move = Move(id=move.id)
     ...     incoming_move.quantity = 8.0
     ...     shipment.incoming_moves.append(incoming_move)
     >>> shipment.save()
     >>> for move in shipment.inventory_moves:
     ...     move.quantity = 8.0
     >>> shipment.click('receive')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> purchase.reload()
     >>> invoice, = purchase.invoices
     >>> invoice_line, = invoice.lines
     >>> invoice_line.quantity
     10.0
     >>> draft_stock_move, stock_move = sorted(
     ...     invoice_line.stock_moves, key=lambda m: m.quantity)
```

### Comparing `trytond_purchase-7.0.3/tests/scenario_purchase_copy_product_suppliers.rst` & `trytond_purchase-7.2.0/tests/scenario_purchase_copy_product_suppliers.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ========================================
 Purchase Copy Product Suppliers Scenario
 ========================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('purchase')
 
 Create company::
 
@@ -40,16 +40,15 @@
     >>> template.cost_price_method = 'fixed'
     >>> product_supplier = template.product_suppliers.new()
     >>> product_supplier.party = supplier
     >>> template.save()
     >>> product, = template.products
     >>> product_supplier = product.product_suppliers.new()
     >>> product_supplier.party = supplier
-    >>> product_supplier.template == template
-    True
+    >>> assertEqual(product_supplier.template, template)
     >>> product.save()
 
 Supplier is copied when copying the template::
 
     >>> template_copy, = template.duplicate()
     >>> product_copy, = template_copy.products
     >>> len(template_copy.product_suppliers)
```

### Comparing `trytond_purchase-7.0.3/tests/scenario_purchase_default_taxes.rst` & `trytond_purchase-7.2.0/tests/scenario_purchase_default_taxes.rst`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 ===========================
 
 Imports::
 
     >>> from decimal import Decimal
 
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts, create_tax)
+    ...     create_chart, create_tax, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('purchase')
 
     >>> Party = Model.get('party.party')
     >>> Purchase = Model.get('purchase.purchase')
@@ -41,16 +41,15 @@
     >>> supplier = Party(name="Supplier")
     >>> supplier.save()
 
 Create a purchase without product::
 
     >>> purchase = Purchase(party=supplier)
     >>> line = purchase.lines.new()
-    >>> line.taxes == [tax]
-    True
+    >>> assertEqual(line.taxes, [tax])
     >>> line.quantity = 1
     >>> line.unit_price = Decimal('100.0000')
     >>> purchase.click('quote')
     >>> purchase.total_amount
     Decimal('110.00')
     >>> purchase.click('confirm')
     >>> purchase.state
@@ -58,9 +57,8 @@
 
 Check invoice::
 
     >>> invoice, = purchase.invoices
     >>> invoice.total_amount
     Decimal('110.00')
     >>> line, = invoice.lines
-    >>> line.account == accounts['expense']
-    True
+    >>> assertEqual(line.account, accounts['expense'])
```

### Comparing `trytond_purchase-7.0.3/tests/scenario_purchase_empty.rst` & `trytond_purchase-7.2.0/tests/scenario_purchase_empty.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 =======================
 Purchase Empty Scenario
 =======================
 
 Imports::
 
     >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart
 
 Activate modules::
 
     >>> config = activate_modules('purchase')
 
 Create company::
```

### Comparing `trytond_purchase-7.0.3/tests/scenario_purchase_manual_invoice.rst` & `trytond_purchase-7.2.0/tests/scenario_purchase_manual_invoice.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 ================================
 
 Imports::
 
     >>> from decimal import Decimal
 
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
     >>> from trytond.modules.company.tests.tools import create_company
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('purchase')
 
     >>> Party = Model.get('party.party')
     >>> ProductCategory = Model.get('product.category')
```

### Comparing `trytond_purchase-7.0.3/tests/scenario_purchase_modify_header.rst` & `trytond_purchase-7.2.0/tests/scenario_purchase_modify_header.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ===============================
 Purchase Modify Header Scenario
 ===============================
 
 Imports::
 
-    >>> from proteus import Model, Wizard
     >>> from decimal import Decimal
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, create_tax, get_accounts
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_tax, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('purchase')
 
 Create company::
 
@@ -84,16 +84,15 @@
     >>> purchase.save()
     >>> purchase.untaxed_amount, purchase.tax_amount, purchase.total_amount
     (Decimal('15.00'), Decimal('1.50'), Decimal('16.50'))
 
 Change the party::
 
     >>> modify_header = purchase.click('modify_header')
-    >>> modify_header.form.party == supplier
-    True
+    >>> assertEqual(modify_header.form.party, supplier)
     >>> modify_header.form.party = another
     >>> modify_header.execute('modify')
 
     >>> purchase.party.name
     'Another Supplier'
     >>> purchase.untaxed_amount, purchase.tax_amount, purchase.total_amount
     (Decimal('15.00'), Decimal('0'), Decimal('15.00'))
```

### Comparing `trytond_purchase-7.0.3/tests/scenario_purchase_reporting.rst` & `trytond_purchase-7.2.0/tests/scenario_purchase_reporting.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 ===========================
 Purchase Reporting Scenario
 ===========================
 
 Imports::
 
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
+
+    >>> from dateutil.relativedelta import relativedelta
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
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('purchase')
     >>> Party = Model.get('party.party')
     >>> ProductUom = Model.get('product.uom')
     >>> ProductTemplate = Model.get('product.template')
@@ -103,28 +104,26 @@
     ...         period='month')
     >>> with config.set_context(context=context):
     ...     reports = Supplier.find([])
     ...     time_series = SupplierTimeseries.find([])
     >>> len(reports)
     2
     >>> with config.set_context(context=context):
-    ...     sorted((r.supplier.id, r.number, r.expense) for r in reports) == \
-    ...     sorted([(supplier1.id, 1, Decimal('30')),
-    ...             (supplier2.id, 1, Decimal('10'))])
-    True
+    ...     assertEqual({(r.supplier.id, r.number, r.expense) for r in reports},
+    ...         {(supplier1.id, 1, Decimal('30')),
+    ...             (supplier2.id, 1, Decimal('10'))})
     >>> len(time_series)
     2
     >>> purchase1_ts_date = purchase1.purchase_date.replace(day=1)
     >>> purchase2_ts_date = purchase2.purchase_date.replace(day=1)
     >>> with config.set_context(context=context):
-    ...     sorted((r.supplier.id, r.date, r.number, r.expense)
-    ...         for r in time_series) == sorted(
-    ...     [(supplier1.id, purchase1_ts_date, 1, Decimal('30')),
-    ...     (supplier2.id, purchase2_ts_date, 1, Decimal('10'))])
-    True
+    ...     assertEqual({(r.supplier.id, r.date, r.number, r.expense)
+    ...         for r in time_series},
+    ...         {(supplier1.id, purchase1_ts_date, 1, Decimal('30')),
+    ...         (supplier2.id, purchase2_ts_date, 1, Decimal('10'))})
 
 Check purchase reporting per product without supplier::
 
     >>> with config.set_context(context=context):
     ...     reports = Product.find([])
     ...     time_series = ProductTimeseries.find([])
     >>> len(reports)
@@ -135,19 +134,17 @@
     >>> context['supplier'] = supplier1.id
     >>> with config.set_context(context=context):
     ...     reports = Product.find([])
     ...     time_series = ProductTimeseries.find([])
     >>> len(reports)
     2
     >>> with config.set_context(context=context):
-    ...     sorted((r.product.id, r.number, r.expense) for r in reports) == \
-    ...     sorted([(product1.id, 1, Decimal('20')),
-    ...         (product2.id, 1, Decimal('10'))])
-    True
+    ...     assertEqual({(r.product.id, r.number, r.expense) for r in reports},
+    ...         {(product1.id, 1, Decimal('20')),
+    ...             (product2.id, 1, Decimal('10'))})
     >>> len(time_series)
     2
     >>> with config.set_context(context=context):
-    ...     sorted((r.product.id, r.date, r.number, r.expense)
-    ...         for r in time_series) == sorted(
-    ...     [(product1.id, purchase1_ts_date, 1, Decimal('20')),
-    ...     (product2.id, purchase1_ts_date, 1, Decimal('10'))])
-    True
+    ...     assertEqual({(r.product.id, r.date, r.number, r.expense)
+    ...         for r in time_series},
+    ...         {(product1.id, purchase1_ts_date, 1, Decimal('20')),
+    ...             (product2.id, purchase1_ts_date, 1, Decimal('10'))})
```

### Comparing `trytond_purchase-7.0.3/tests/scenario_purchase_return_wizard.rst` & `trytond_purchase-7.2.0/tests/scenario_purchase_return_wizard.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ===============================
 Purchase Return Wizard Scenario
 ===============================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('purchase')
 
 Create company::
 
@@ -84,11 +84,10 @@
     'processing'
     >>> return_purchase = Wizard('purchase.return_purchase', [
     ...     purchase_to_return])
     >>> return_purchase.execute('return_')
     >>> returned_purchase, = Purchase.find([
     ...     ('state', '=', 'draft'),
     ...     ])
-    >>> returned_purchase.origin == purchase_to_return
-    True
+    >>> assertEqual(returned_purchase.origin, purchase_to_return)
     >>> sorted([x.quantity or 0 for x in returned_purchase.lines])
     [-1.0, 0]
```

### Comparing `trytond_purchase-7.0.3/tests/test_module.py` & `trytond_purchase-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/tox.ini` & `trytond_purchase-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/trytond_purchase.egg-info/PKG-INFO` & `trytond_purchase-7.2.0/trytond_purchase.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_purchase
-Version: 7.0.3
+Version: 7.2.0
 Summary: Tryton module for purchase
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-purchase/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -49,28 +49,28 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: sparklines
 Requires-Dist: pygal; extra == "sparklines"
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ###############
 Purchase Module
 ###############
 
 The *Purchase Module* provides everything that is required to create and
 manage purchases made by the company.
```

### Comparing `trytond_purchase-7.0.3/trytond_purchase.egg-info/SOURCES.txt` & `trytond_purchase-7.2.0/trytond_purchase.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_purchase.rst
 ./tests/scenario_purchase_copy_product_suppliers.rst
 ./tests/scenario_purchase_default_taxes.rst
 ./tests/scenario_purchase_empty.rst
+./tests/scenario_purchase_line_cancelled.rst
+./tests/scenario_purchase_line_cancelled_on_shipment.rst
 ./tests/scenario_purchase_manual_invoice.rst
 ./tests/scenario_purchase_modify_header.rst
 ./tests/scenario_purchase_reporting.rst
 ./tests/scenario_purchase_return_wizard.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/configuration_form.xml
@@ -113,17 +115,17 @@
 ./view/template_tree.xml
 doc/conf.py
 doc/design.rst
 doc/index.rst
 doc/releases.rst
 doc/requirements-doc.txt
 doc/usage/index.rst
-doc/usage/prepurchase.rst
-doc/usage/process.rst
-doc/usage/returns.rst
+doc/usage/prepurchase.inc.rst
+doc/usage/process.inc.rst
+doc/usage/returns.inc.rst
 icons/LICENSE
 icons/tryton-purchase.svg
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
@@ -147,14 +149,16 @@
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_purchase.rst
 tests/scenario_purchase_copy_product_suppliers.rst
 tests/scenario_purchase_default_taxes.rst
 tests/scenario_purchase_empty.rst
+tests/scenario_purchase_line_cancelled.rst
+tests/scenario_purchase_line_cancelled_on_shipment.rst
 tests/scenario_purchase_manual_invoice.rst
 tests/scenario_purchase_modify_header.rst
 tests/scenario_purchase_reporting.rst
 tests/scenario_purchase_return_wizard.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_purchase.egg-info/PKG-INFO
```

### Comparing `trytond_purchase-7.0.3/view/party_form.xml` & `trytond_purchase-7.2.0/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/view/product_supplier_form.xml` & `trytond_purchase-7.2.0/view/product_supplier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/view/purchase_form.xml` & `trytond_purchase-7.2.0/view/purchase_form.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_purchase-7.0.3/view/purchase_form.xml` & `trytond_purchase-7.2.0/view/purchase_form.xml`

```diff
@@ -56,14 +56,17 @@
       <label name="quoted_by"/>
       <field name="quoted_by"/>
       <label name="confirmed_by"/>
       <field name="confirmed_by"/>
       <separator name="comment" colspan="4"/>
       <field name="comment" colspan="4"/>
     </page>
+    <page name="invoices_ignored" col="1">
+      <field name="invoices_ignored"/>
+    </page>
   </notebook>
   <group id="links" col="-1" colspan="3">
     <link icon="tryton-shipment-in" name="purchase.act_shipment_form"/>
     <link icon="tryton-account" name="purchase.act_invoice_form"/>
     <link icon="tryton-shipment-out" name="purchase.act_return_form"/>
   </group>
   <group col="-1" colspan="3" id="buttons">
```

### Comparing `trytond_purchase-7.0.3/view/purchase_line_form.xml` & `trytond_purchase-7.2.0/view/purchase_line_form.xml`

 * *Files 7% similar despite different names*

#### Comparing `trytond_purchase-7.0.3/view/purchase_line_form.xml` & `trytond_purchase-7.2.0/view/purchase_line_form.xml`

```diff
@@ -31,14 +31,15 @@
       <field name="description" colspan="4"/>
     </page>
     <page string="Taxes" id="taxes">
       <field name="taxes" colspan="4"/>
     </page>
     <page name="moves" col="1">
       <field name="moves"/>
+      <field name="moves_ignored"/>
     </page>
     <page name="invoice_lines" col="1">
       <field name="invoice_lines"/>
     </page>
     <page string="Notes" id="notes">
       <separator name="note" colspan="4"/>
       <field name="note" colspan="4"/>
```

### Comparing `trytond_purchase-7.0.3/view/purchase_line_tree.xml` & `trytond_purchase-7.2.0/view/purchase_line_tree_sequence.xml`

 * *Files 20% similar despite different names*

#### Comparing `trytond_purchase-7.0.3/view/purchase_line_tree.xml` & `trytond_purchase-7.2.0/view/purchase_line_tree_sequence.xml`

```diff
@@ -1,17 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
-<tree>
+<tree sequence="sequence">
   <field name="purchase" expand="1"/>
-  <field name="supplier" expand="1" optional="0"/>
-  <field name="purchase_date" optional="1"/>
   <field name="type" optional="1"/>
   <field name="product" expand="1" optional="0"/>
   <field name="product_supplier" expand="1" optional="1"/>
   <field name="summary" expand="1" optional="1"/>
-  <field name="actual_quantity" symbol="unit" optional="0"/>
-  <field name="quantity" symbol="unit" optional="0"/>
+  <field name="quantity" symbol="unit"/>
   <field name="unit_price"/>
+  <field name="taxes" optional="0"/>
   <field name="amount"/>
-  <field name="purchase_state"/>
 </tree>
```

### Comparing `trytond_purchase-7.0.3/view/purchase_line_tree_sequence.xml` & `trytond_purchase-7.2.0/view/purchase_tree.xml`

 * *Files 14% similar despite different names*

#### Comparing `trytond_purchase-7.0.3/view/purchase_line_tree_sequence.xml` & `trytond_purchase-7.2.0/view/purchase_tree.xml`

```diff
@@ -1,14 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
-<tree sequence="sequence">
-  <field name="purchase" expand="1"/>
-  <field name="type" optional="1"/>
-  <field name="product" expand="1" optional="0"/>
-  <field name="product_supplier" expand="1" optional="1"/>
-  <field name="summary" expand="1" optional="1"/>
-  <field name="quantity" symbol="unit"/>
-  <field name="unit_price"/>
-  <field name="taxes" optional="0"/>
-  <field name="amount"/>
+<tree>
+  <field name="company" expand="1" optional="1"/>
+  <field name="number" expand="1"/>
+  <field name="reference" expand="1" optional="0"/>
+  <field name="purchase_date" optional="0"/>
+  <field name="party" expand="2"/>
+  <field name="warehouse" optional="1"/>
+  <field name="untaxed_amount" optional="0"/>
+  <field name="description" expand="1" optional="1"/>
+  <field name="state"/>
+  <field name="invoice_state"/>
+  <field name="shipment_state"/>
 </tree>
```

### Comparing `trytond_purchase-7.0.3/view/purchase_reporting_context_form.xml` & `trytond_purchase-7.2.0/view/purchase_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.0.3/view/template_form.xml` & `trytond_purchase-7.2.0/view/template_form.xml`

 * *Files identical despite different names*

