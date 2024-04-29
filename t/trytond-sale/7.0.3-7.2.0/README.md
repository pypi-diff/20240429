# Comparing `tmp/trytond_sale-7.0.3.tar.gz` & `tmp/trytond_sale-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale-7.0.3.tar", last modified: Wed Apr 17 10:40:26 2024, max compression
+gzip compressed data, was "trytond_sale-7.2.0.tar", last modified: Mon Apr 29 15:46:55 2024, max compression
```

## Comparing `trytond_sale-7.0.3.tar` & `trytond_sale-7.2.0.tar`

### file list

```diff
@@ -1,126 +1,129 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:26.825860 trytond_sale-7.0.3/
--rw-r--r--   0 ced       (1000) ced       (1000)     6835 2024-04-17 10:40:23.000000 trytond_sale-7.0.3/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-17 10:40:23.000000 trytond_sale-7.0.3/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-17 10:40:26.825860 trytond_sale-7.0.3/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2345 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3898 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2425 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:26.819193 trytond_sale-7.0.3/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2783 2024-03-03 16:24:20.000000 trytond_sale-7.0.3/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9118 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:26.819193 trytond_sale-7.0.3/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1985 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/doc/usage/presales.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4006 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/doc/usage/process.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      726 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/doc/usage/reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1618 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/doc/usage/returns.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:26.819193 trytond_sale-7.0.3/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/icons/tryton-sale.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     5255 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1800 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:26.822526 trytond_sale-7.0.3/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    41487 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42300 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36585 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    43026 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42500 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34894 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39826 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    44547 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36546 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42901 2024-01-26 17:57:52.000000 trytond_sale-7.0.3/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40842 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37767 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39110 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40549 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40909 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42387 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38023 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39321 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42391 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41566 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39026 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36537 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34330 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36845 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4617 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4574 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3022 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8949 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2740 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    76266 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/sale.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    84658 2024-04-12 17:44:57.000000 trytond_sale-7.0.3/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24435 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    36553 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/sale_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    56250 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/sale_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-17 10:40:26.825860 trytond_sale-7.0.3/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4556 2024-03-03 16:24:03.000000 trytond_sale-7.0.3/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7657 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3013 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:26.822526 trytond_sale-7.0.3/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20146 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/tests/scenario_sale.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      938 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/tests/scenario_sale_default_methods.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1500 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/tests/scenario_sale_default_taxes.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1244 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/tests/scenario_sale_empty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2359 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/tests/scenario_sale_manual_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2033 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/tests/scenario_sale_manual_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3028 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/tests/scenario_sale_modify_header.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    12999 2024-02-05 16:24:27.000000 trytond_sale-7.0.3/tests/scenario_sale_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2524 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-04 07:49:46.000000 trytond_sale-7.0.3/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:26.825860 trytond_sale-7.0.3/trytond_sale.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-17 10:40:26.000000 trytond_sale-7.0.3/trytond_sale.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     5186 2024-04-17 10:40:26.000000 trytond_sale-7.0.3/trytond_sale.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-17 10:40:26.000000 trytond_sale-7.0.3/trytond_sale.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2024-04-17 10:40:26.000000 trytond_sale-7.0.3/trytond_sale.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:04.000000 trytond_sale-7.0.3/trytond_sale.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-04-17 10:40:26.000000 trytond_sale-7.0.3/trytond_sale.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-17 10:40:26.000000 trytond_sale-7.0.3/trytond_sale.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-17 10:40:26.825860 trytond_sale-7.0.3/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/handle_invoice_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/handle_shipment_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/modify_header_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      844 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/product_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/product_list_sale_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/product_sale_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/return_sale_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3846 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1554 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      668 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_country_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_customer_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_customer_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_customer_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_customer_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_customer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_main_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_main_time_series_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_product_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_product_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_product_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_product_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_reporting_region_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/sale_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      935 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_sale-7.0.3/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.542580 trytond_sale-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6684 2024-04-29 15:24:31.000000 trytond_sale-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-04-29 15:24:31.000000 trytond_sale-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-29 15:46:55.542580 trytond_sale-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2345 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3898 2024-01-27 09:58:52.000000 trytond_sale-7.2.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2379 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.532580 trytond_sale-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3067 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9121 2024-03-17 11:01:36.000000 trytond_sale-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:23.000000 trytond_sale-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.532580 trytond_sale-7.2.0/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      268 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1985 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/doc/usage/presales.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4187 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/doc/usage/process.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      726 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/doc/usage/reporting.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1618 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/doc/usage/returns.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2024-02-04 18:51:26.000000 trytond_sale-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.532580 trytond_sale-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-01-16 14:00:21.000000 trytond_sale-7.2.0/icons/tryton-sale.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5255 2024-01-27 09:58:52.000000 trytond_sale-7.2.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1754 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.535913 trytond_sale-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    41606 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42411 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36682 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    43131 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42615 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34974 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39927 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    44661 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36643 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    43010 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40949 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37869 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39224 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40656 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41015 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42496 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38125 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39436 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42533 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41687 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39131 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36634 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34410 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36942 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4617 2024-02-04 18:51:26.000000 trytond_sale-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4595 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2980 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9027 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2740 2024-02-04 18:51:26.000000 trytond_sale-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    76278 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/sale.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    89113 2024-04-29 13:17:17.000000 trytond_sale-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25512 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    36794 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/sale_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    55353 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/sale_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:46:55.542580 trytond_sale-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4556 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7637 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2944 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.535913 trytond_sale-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20145 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/tests/scenario_sale.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      898 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_default_methods.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1517 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_default_taxes.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1197 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_empty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2700 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_line_cancelled.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2414 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_line_cancelled_on_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2423 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_line_cancelled_on_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2344 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_manual_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1935 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_manual_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3004 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_modify_header.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    12959 2024-04-22 12:14:36.000000 trytond_sale-7.2.0/tests/scenario_sale_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2524 2024-02-04 18:51:26.000000 trytond_sale-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:23.000000 trytond_sale-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-29 15:24:27.000000 trytond_sale-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.542580 trytond_sale-7.2.0/trytond_sale.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-04-29 15:46:55.000000 trytond_sale-7.2.0/trytond_sale.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     5488 2024-04-29 15:46:55.000000 trytond_sale-7.2.0/trytond_sale.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:46:55.000000 trytond_sale-7.2.0/trytond_sale.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       46 2024-04-29 15:46:55.000000 trytond_sale-7.2.0/trytond_sale.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_sale-7.2.0/trytond_sale.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-04-29 15:46:55.000000 trytond_sale-7.2.0/trytond_sale.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:46:55.000000 trytond_sale-7.2.0/trytond_sale.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:55.542580 trytond_sale-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-01-16 14:00:21.000000 trytond_sale-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/handle_invoice_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/handle_shipment_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-01-16 14:00:21.000000 trytond_sale-7.2.0/view/modify_header_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2024-02-04 18:51:26.000000 trytond_sale-7.2.0/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      844 2024-01-27 09:58:52.000000 trytond_sale-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/product_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/product_list_sale_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/product_sale_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/return_sale_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3954 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1596 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      845 2024-04-27 16:30:39.000000 trytond_sale-7.2.0/view/sale_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_country_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_customer_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_customer_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_customer_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_customer_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_customer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_main_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-01-27 09:58:52.000000 trytond_sale-7.2.0/view/sale_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_main_time_series_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-01-27 09:58:52.000000 trytond_sale-7.2.0/view/sale_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_product_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_product_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_product_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_product_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/sale_reporting_region_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      652 2023-09-26 14:46:01.000000 trytond_sale-7.2.0/view/sale_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      935 2024-01-27 09:58:52.000000 trytond_sale-7.2.0/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_sale-7.2.0/view/template_tree.xml
```

### Comparing `trytond_sale-7.0.3/CHANGELOG` & `trytond_sale-7.2.0/CHANGELOG`

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
 * Add warning when receiving too much goods from sale return
 * Do not invoice non sale line
```

### Comparing `trytond_sale-7.0.3/COPYRIGHT` & `trytond_sale-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/LICENSE` & `trytond_sale-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/PKG-INFO` & `trytond_sale-7.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale
-Version: 7.0.3
+Version: 7.2.0
 Summary: Tryton module for sale
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-sale/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -50,29 +50,29 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
 Requires-Dist: python-dateutil
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_country<7.1,>=7.0
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
+Requires-Dist: trytond_country<7.3,>=7.2
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
 
 ###########
 Sale Module
 ###########
 
 The *Sale Module* helps organise and manage sales made by the company.
 It adds the concept of a sale to Tryton and allows it to be tracked through
```

### Comparing `trytond_sale-7.0.3/__init__.py` & `trytond_sale-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/configuration.py` & `trytond_sale-7.2.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/configuration.xml` & `trytond_sale-7.2.0/configuration.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_sale-7.0.3/configuration.xml` & `trytond_sale-7.2.0/configuration.xml`

```diff
@@ -20,22 +20,22 @@
     <record model="ir.action.act_window.view" id="act_sale_configuration_view1">
       <field name="sequence" eval="1"/>
       <field name="view" ref="sale_configuration_view_form"/>
       <field name="act_window" ref="act_sale_configuration_form"/>
     </record>
     <menuitem parent="menu_configuration" action="act_sale_configuration_form" sequence="10" id="menu_sale_configuration" icon="tryton-list"/>
     <record model="ir.model.access" id="access_sale_configuration">
-      <field name="model" search="[('model', '=', 'sale.configuration')]"/>
+      <field name="model">sale.configuration</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_sale_configuration_sale_admin">
-      <field name="model" search="[('model', '=', 'sale.configuration')]"/>
+      <field name="model">sale.configuration</field>
       <field name="group" ref="group_sale_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_sale-7.0.3/doc/conf.py` & `trytond_sale-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale-7.0.3/doc/design.rst` & `trytond_sale-7.2.0/doc/design.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 .. _model-sale.sale:
 
 Sale
 ====
 
 The *Sale* concept is used to manage the selling process.
 Each sale, at any time, can be in one of several different states.
-A sale progress though these states until it is either done or gets cancelled.
+A sale progresses through these states until it is either done or gets
+cancelled.
 When some of these state changes happen the
 `Employee <company:model-company.employee>` that triggered the state change
 is also recorded.
 
 Each sale contains details of the `Party <party:model-party.party>` that the
 sale is made to, including details such as the party's preferred
 `Contact Method <party:model-party.contact_mechanism>`, and what
```

### Comparing `trytond_sale-7.0.3/doc/usage/presales.rst` & `trytond_sale-7.2.0/doc/usage/presales.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/doc/usage/process.rst` & `trytond_sale-7.2.0/doc/usage/process.inc.rst`

 * *Files 6% similar despite different names*

```diff
@@ -97,14 +97,20 @@
 
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
 .. _Finishing a sale:
 
 Finishing a sale
 ================
 
 In Tryton once a `Sale <model-sale.sale>` is being processed there is no
 button that moves the sale into a done state.
```

### Comparing `trytond_sale-7.0.3/doc/usage/reporting.rst` & `trytond_sale-7.2.0/doc/usage/reporting.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/doc/usage/returns.rst` & `trytond_sale-7.2.0/doc/usage/returns.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/icons/LICENSE` & `trytond_sale-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/invoice.py` & `trytond_sale-7.2.0/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/invoice.xml` & `trytond_sale-7.2.0/invoice.xml`

 * *Files 16% similar despite different names*

#### Comparing `trytond_sale-7.0.3/invoice.xml` & `trytond_sale-7.2.0/invoice.xml`

```diff
@@ -10,23 +10,23 @@
     </record>
     <record model="ir.action.keyword" id="act_open_invoice_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">sale.sale,-1</field>
       <field name="action" ref="act_invoice_form"/>
     </record>
     <record model="ir.model.access" id="access_invoice_sale">
-      <field name="model" search="[('model', '=', 'account.invoice')]"/>
+      <field name="model">account.invoice</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_invoice_line_sale">
-      <field name="model" search="[('model', '=', 'account.invoice.line')]"/>
+      <field name="model">account.invoice.line</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_sale-7.0.3/locale/bg.po` & `trytond_sale-7.2.0/locale/bg.po`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,19 @@
 msgid "From Location"
 msgstr "От местонахождение"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Редове от фактура"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Адрес за фактура"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Движения"
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
```

### Comparing `trytond_sale-7.0.3/locale/ca.po` & `trytond_sale-7.2.0/locale/ca.po`

 * *Files 0% similar despite different names*

```diff
@@ -210,14 +210,19 @@
 msgid "From Location"
 msgstr "Des de la ubicació"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Línies de factura"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Adreça de facturació"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Moviments"
 
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
 msgstr "Moviments en excepció"
```

### Comparing `trytond_sale-7.0.3/locale/cs.po` & `trytond_sale-7.2.0/locale/tr.po`

 * *Files 0% similar despite different names*

```diff
@@ -222,14 +222,19 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Invoices"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
@@ -409,18 +414,17 @@
 msgid "Children"
 msgstr ""
 
 msgctxt "field:sale.reporting.customer.category.tree,currency:"
 msgid "Currency"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:sale.reporting.customer.category.tree,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:sale.reporting.customer.category.tree,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:sale.reporting.customer.category.tree,revenue:"
 msgid "Revenue"
@@ -448,18 +452,17 @@
 msgid "Children"
 msgstr ""
 
 msgctxt "field:sale.reporting.product.category.tree,currency:"
 msgid "Currency"
 msgstr ""
 
-#, fuzzy
 msgctxt "field:sale.reporting.product.category.tree,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:sale.reporting.product.category.tree,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:sale.reporting.product.category.tree,revenue:"
 msgid "Revenue"
@@ -470,18 +473,17 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.reporting.region.tree,currency:"
 msgid "Currency"
 msgstr "Sales per Customer"
 
-#, fuzzy
 msgctxt "field:sale.reporting.region.tree,name:"
 msgid "Name"
-msgstr "Namu"
+msgstr ""
 
 msgctxt "field:sale.reporting.region.tree,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:sale.reporting.region.tree,revenue:"
 msgid "Revenue"
@@ -1394,15 +1396,14 @@
 msgid "Sale - Ignored Invoice"
 msgstr ""
 
 msgctxt "model:sale.sale-recreated-account.invoice,name:"
 msgid "Sale - Recreated Invoice"
 msgstr ""
 
-#, fuzzy
 msgctxt "report:sale.sale:"
 msgid ":"
 msgstr ":"
 
 msgctxt "report:sale.sale:"
 msgid "Amount"
 msgstr ""
```

### Comparing `trytond_sale-7.0.3/locale/de.po` & `trytond_sale-7.2.0/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -210,14 +210,19 @@
 msgid "From Location"
 msgstr "Von Lagerort"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Rechnungspositionen"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Rechnungsadresse"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Warenbewegungen"
 
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
 msgstr "Warenbewegungen mit Vorbehalt"
```

### Comparing `trytond_sale-7.0.3/locale/es.po` & `trytond_sale-7.2.0/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,19 @@
 msgid "From Location"
 msgstr "Desde ubicación"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Líneas de factura"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Dirección de facturación"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Movimientos"
 
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
 msgstr "Movimientos en excepción"
```

### Comparing `trytond_sale-7.0.3/locale/es_419.po` & `trytond_sale-7.2.0/locale/es_419.po`

 * *Files 0% similar despite different names*

```diff
@@ -213,14 +213,18 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr ""
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
```

### Comparing `trytond_sale-7.0.3/locale/et.po` & `trytond_sale-7.2.0/locale/et.po`

 * *Files 0% similar despite different names*

```diff
@@ -238,14 +238,19 @@
 msgid "From Location"
 msgstr "Asukohast"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Arve read"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Arve aadress"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Kanded"
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
```

### Comparing `trytond_sale-7.0.3/locale/fa.po` & `trytond_sale-7.2.0/locale/fa.po`

 * *Files 0% similar despite different names*

```diff
@@ -238,14 +238,19 @@
 msgid "From Location"
 msgstr "از مکان"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "خطوط صورتحساب"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "آدرس صورتحساب"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "جابجایی ها"
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
```

### Comparing `trytond_sale-7.0.3/locale/fi.po` & `trytond_sale-7.2.0/locale/cs.po`

 * *Files 1% similar despite different names*

```diff
@@ -222,14 +222,19 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Invoices"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
@@ -409,17 +414,18 @@
 msgid "Children"
 msgstr ""
 
 msgctxt "field:sale.reporting.customer.category.tree,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.reporting.customer.category.tree,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:sale.reporting.customer.category.tree,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:sale.reporting.customer.category.tree,revenue:"
 msgid "Revenue"
@@ -447,17 +453,18 @@
 msgid "Children"
 msgstr ""
 
 msgctxt "field:sale.reporting.product.category.tree,currency:"
 msgid "Currency"
 msgstr ""
 
+#, fuzzy
 msgctxt "field:sale.reporting.product.category.tree,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:sale.reporting.product.category.tree,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:sale.reporting.product.category.tree,revenue:"
 msgid "Revenue"
@@ -468,17 +475,18 @@
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.reporting.region.tree,currency:"
 msgid "Currency"
 msgstr "Sales per Customer"
 
+#, fuzzy
 msgctxt "field:sale.reporting.region.tree,name:"
 msgid "Name"
-msgstr ""
+msgstr "Namu"
 
 msgctxt "field:sale.reporting.region.tree,parent:"
 msgid "Parent"
 msgstr ""
 
 msgctxt "field:sale.reporting.region.tree,revenue:"
 msgid "Revenue"
```

### Comparing `trytond_sale-7.0.3/locale/fr.po` & `trytond_sale-7.2.0/locale/fr.po`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,18 @@
 msgid "From Location"
 msgstr "Emplacement d'origine"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Lignes de facture"
 
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Progression de la facturation"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Mouvements"
 
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
 msgstr "Mouvements en exception"
```

### Comparing `trytond_sale-7.0.3/locale/hu.po` & `trytond_sale-7.2.0/locale/hu.po`

 * *Files 0% similar despite different names*

```diff
@@ -228,14 +228,19 @@
 msgid "From Location"
 msgstr "Induló tárhely"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Számlasorok"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Számlázási cím"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Mozgások"
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
```

### Comparing `trytond_sale-7.0.3/locale/id.po` & `trytond_sale-7.2.0/locale/id.po`

 * *Files 0% similar despite different names*

```diff
@@ -227,14 +227,19 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Baris Faktur"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Alamat Faktur"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Perpindahan"
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
```

### Comparing `trytond_sale-7.0.3/locale/it.po` & `trytond_sale-7.2.0/locale/it.po`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,19 @@
 msgid "From Location"
 msgstr "da locazione"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Righe fattura"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Indirizzo di fatturazione"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Movimenti"
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
```

### Comparing `trytond_sale-7.0.3/locale/lo.po` & `trytond_sale-7.2.0/locale/lo.po`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,19 @@
 
 #, fuzzy
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "ລາຍການເກັບເງິນ"
 
 #, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "ທີ່ຢູ່"
+
+#, fuzzy
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "ຕັດບັນຊີສາງ"
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
```

### Comparing `trytond_sale-7.0.3/locale/lt.po` & `trytond_sale-7.2.0/locale/lt.po`

 * *Files 0% similar despite different names*

```diff
@@ -238,14 +238,19 @@
 msgid "From Location"
 msgstr "Išsiuntimo vieta"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Sąskaitos faktūros eilutės"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Juridinis adresas"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Operacijos"
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
```

### Comparing `trytond_sale-7.0.3/locale/nl.po` & `trytond_sale-7.2.0/locale/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,19 @@
 msgid "From Location"
 msgstr "Van locatie"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Factuur regels"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Factuur adres"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Mutaties"
 
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
 msgstr "Mutaties Uitzondering"
@@ -1039,15 +1044,15 @@
 
 msgctxt "model:ir.message,text:msg_sale_reporting_revenue"
 msgid "Revenue"
 msgstr "Omzet"
 
 msgctxt "model:ir.message,text:msg_sale_reporting_revenue_trend"
 msgid "Revenue Trend"
-msgstr "Omzet trent"
+msgstr "Omzet ontwikkeling"
 
 msgctxt "model:ir.message,text:msg_sale_reporting_time_series"
 msgid "Time Series"
 msgstr "Tijdreeksen"
 
 msgctxt ""
 "model:ir.message,text:msg_sale_shipment_address_required_for_quotation"
```

### Comparing `trytond_sale-7.0.3/locale/pl.po` & `trytond_sale-7.2.0/locale/pl.po`

 * *Files 0% similar despite different names*

```diff
@@ -233,14 +233,19 @@
 msgid "From Location"
 msgstr "Z lokalizacji"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Wiersze faktury"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Adres faktury"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Ruchy"
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
```

### Comparing `trytond_sale-7.0.3/locale/pt.po` & `trytond_sale-7.2.0/locale/pt.po`

 * *Files 0% similar despite different names*

```diff
@@ -238,14 +238,19 @@
 msgid "From Location"
 msgstr "Origem"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Linhas da fatura"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Endereço para faturamento"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Movimentações"
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
```

### Comparing `trytond_sale-7.0.3/locale/ro.po` & `trytond_sale-7.2.0/locale/ro.po`

 * *Files 3% similar despite different names*

```diff
@@ -10,37 +10,34 @@
 msgid "Sales"
 msgstr "Vânzări"
 
 msgctxt "field:party.party,customer_currencies:"
 msgid "Customer Currencies"
 msgstr "Valute Clienți"
 
-#, fuzzy
 msgctxt "field:party.party,customer_currency:"
 msgid "Customer Currency"
-msgstr "Moneda"
+msgstr "Moneda Client"
 
 msgctxt "field:party.party,sale_invoice_method:"
 msgid "Invoice Method"
 msgstr "Metoda de facturare"
 
 msgctxt "field:party.party,sale_methods:"
 msgid "Sale Methods"
 msgstr "Metode de Vânzare"
 
 msgctxt "field:party.party,sale_shipment_method:"
 msgid "Shipment Method"
 msgstr "Metoda de Expediere"
 
-#, fuzzy
 msgctxt "field:party.party.customer_currency,customer_currency:"
 msgid "Customer Currency"
-msgstr "Moneda"
+msgstr "Moneda Client"
 
-#, fuzzy
 msgctxt "field:party.party.customer_currency,party:"
 msgid "Party"
 msgstr "Parte"
 
 msgctxt "field:party.party.sale_method,company:"
 msgid "Company"
 msgstr "Companie"
@@ -61,44 +58,41 @@
 msgid "Default Lead Time"
 msgstr "Timp Implicit de execuţie"
 
 msgctxt "field:product.configuration.default_lead_time,default_lead_time:"
 msgid "Default Lead Time"
 msgstr "Timp Implicit de execuţie"
 
-#, fuzzy
 msgctxt "field:product.lead_time,lead_time:"
 msgid "Lead Time"
 msgstr "Timp de livrare"
 
 msgctxt "field:product.lead_time,template:"
 msgid "Template"
 msgstr "Șablon"
 
 msgctxt "field:product.product,lead_time:"
 msgid "Lead Time"
 msgstr "Timp de livrare"
 
-#, fuzzy
 msgctxt "field:product.product,lead_times:"
 msgid "Lead Times"
-msgstr "Timp de livrare"
+msgstr "Timpi de livrare"
 
 msgctxt "field:product.product,salable:"
 msgid "Salable"
 msgstr "Marfă"
 
 msgctxt "field:product.product,sale_price_uom:"
 msgid "Sale Price"
 msgstr "Preț de vânzare"
 
-#, fuzzy
 msgctxt "field:product.product,sale_uom:"
 msgid "Sale UoM"
-msgstr "Vânzare UM"
+msgstr "UM Vânzare"
 
 msgctxt "field:product.sale.context,company:"
 msgid "Company"
 msgstr "Companie"
 
 msgctxt "field:product.sale.context,currency:"
 msgid "Currency"
@@ -124,27 +118,25 @@
 msgid "Stock End Date"
 msgstr "Data încheiere Stoc"
 
 msgctxt "field:product.template,lead_time:"
 msgid "Lead Time"
 msgstr "Timp de livrare"
 
-#, fuzzy
 msgctxt "field:product.template,lead_times:"
 msgid "Lead Times"
-msgstr "Timp de livrare"
+msgstr "Timpi de livrare"
 
 msgctxt "field:product.template,salable:"
 msgid "Salable"
 msgstr "Marfă"
 
-#, fuzzy
 msgctxt "field:product.template,sale_uom:"
 msgid "Sale UoM"
-msgstr "Vânzare UM"
+msgstr "UM Vânzare"
 
 msgctxt "field:sale.configuration,sale_invoice_method:"
 msgid "Sale Invoice Method"
 msgstr "Metoda facturii de vânzare"
 
 msgctxt "field:sale.configuration,sale_process_after:"
 msgid "Process Sale after"
@@ -218,58 +210,59 @@
 msgid "From Location"
 msgstr "Din locație"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Rând factură"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Adresa de facturare"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Mișcări"
 
-#, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
-msgstr "Excepție de Miscare"
+msgstr "Excepție de Mișcare"
 
 msgctxt "field:sale.line,moves_ignored:"
 msgid "Ignored Moves"
 msgstr "Mișcări ignorate"
 
-#, fuzzy
 msgctxt "field:sale.line,moves_progress:"
 msgid "Moves Progress"
-msgstr "Mișcari Finalizate"
+msgstr "Progres Mișcări"
 
 msgctxt "field:sale.line,moves_recreated:"
 msgid "Recreated Moves"
 msgstr "Mișcări recreate"
 
 msgctxt "field:sale.line,note:"
 msgid "Note"
 msgstr "Nota"
 
 msgctxt "field:sale.line,product:"
 msgid "Product"
 msgstr "Produs"
 
-#, fuzzy
 msgctxt "field:sale.line,product_uom_category:"
 msgid "Product UoM Category"
 msgstr "Categorie UM Produs"
 
 msgctxt "field:sale.line,quantity:"
 msgid "Quantity"
 msgstr "Cantitate"
 
 msgctxt "field:sale.line,sale:"
 msgid "Sale"
 msgstr "Vânzare"
 
-#, fuzzy
 msgctxt "field:sale.line,sale_date:"
 msgid "Sale Date"
 msgstr "Data vânzării"
 
 msgctxt "field:sale.line,sale_state:"
 msgid "Sale State"
 msgstr "Starea vanzarii"
@@ -370,25 +363,22 @@
 msgid "Subdivision"
 msgstr "Subdiviziune"
 
 msgctxt "field:sale.reporting.country.time_series,country:"
 msgid "Country"
 msgstr "Țară"
 
-#, fuzzy
 msgctxt "field:sale.reporting.country.tree,children:"
 msgid "Children"
 msgstr "Copii"
 
-#, fuzzy
 msgctxt "field:sale.reporting.country.tree,parent:"
 msgid "Parent"
 msgstr "Părinte"
 
-#, fuzzy
 msgctxt "field:sale.reporting.country.tree,region:"
 msgid "Region"
 msgstr "Regiune"
 
 msgctxt "field:sale.reporting.customer,customer:"
 msgid "Customer"
 msgstr "Client"
@@ -413,15 +403,14 @@
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:sale.reporting.customer.category.tree,parent:"
 msgid "Parent"
 msgstr "Părinte"
 
-#, fuzzy
 msgctxt "field:sale.reporting.customer.category.tree,revenue:"
 msgid "Revenue"
 msgstr "Venituri"
 
 msgctxt "field:sale.reporting.customer.time_series,customer:"
 msgid "Customer"
 msgstr "Client"
@@ -450,47 +439,41 @@
 msgid "Name"
 msgstr "Denumire"
 
 msgctxt "field:sale.reporting.product.category.tree,parent:"
 msgid "Parent"
 msgstr "Părinte"
 
-#, fuzzy
 msgctxt "field:sale.reporting.product.category.tree,revenue:"
 msgid "Revenue"
 msgstr "Venituri"
 
 msgctxt "field:sale.reporting.product.time_series,product:"
 msgid "Product"
 msgstr "Produs"
 
-#, fuzzy
 msgctxt "field:sale.reporting.region.tree,currency:"
 msgid "Currency"
 msgstr "Moneda"
 
-#, fuzzy
 msgctxt "field:sale.reporting.region.tree,name:"
 msgid "Name"
-msgstr "Denumire"
+msgstr "Nume"
 
-#, fuzzy
 msgctxt "field:sale.reporting.region.tree,parent:"
 msgid "Parent"
 msgstr "Părinte"
 
-#, fuzzy
 msgctxt "field:sale.reporting.region.tree,revenue:"
 msgid "Revenue"
 msgstr "Venituri"
 
-#, fuzzy
 msgctxt "field:sale.reporting.region.tree,subregions:"
 msgid "Subregions"
-msgstr "Regiune"
+msgstr "Sub-regiuni"
 
 msgctxt "field:sale.sale,comment:"
 msgid "Comment"
 msgstr "Cometariu"
 
 msgctxt "field:sale.sale,company:"
 msgid "Company"
@@ -612,36 +595,33 @@
 msgid "State"
 msgstr "Stare"
 
 msgctxt "field:sale.sale,tax_amount:"
 msgid "Tax"
 msgstr "Impozit"
 
-#, fuzzy
 msgctxt "field:sale.sale,tax_amount_cache:"
 msgid "Tax Cache"
-msgstr "Impozit precalculat"
+msgstr "Cache Impozit"
 
 msgctxt "field:sale.sale,total_amount:"
 msgid "Total"
 msgstr "Total"
 
-#, fuzzy
 msgctxt "field:sale.sale,total_amount_cache:"
 msgid "Total Cache"
-msgstr "Impozit precalculat"
+msgstr "Cache Total"
 
 msgctxt "field:sale.sale,untaxed_amount:"
 msgid "Untaxed"
 msgstr "Neimpozitat"
 
-#, fuzzy
 msgctxt "field:sale.sale,untaxed_amount_cache:"
 msgid "Untaxed Cache"
-msgstr "Baza de impozitare"
+msgstr "Neimpozitat Cache"
 
 msgctxt "field:sale.sale,warehouse:"
 msgid "Warehouse"
 msgstr "Depozit"
 
 msgctxt "field:sale.sale-ignored-account.invoice,invoice:"
 msgid "Invoice"
@@ -665,15 +645,15 @@
 
 msgctxt "field:stock.move,sale_exception_state:"
 msgid "Exception State"
 msgstr "Stare de excepție"
 
 msgctxt "help:party.party,customer_currency:"
 msgid "Default currency for sales to this party."
-msgstr ""
+msgstr "Moneda implicită pentru vânzări către această parte."
 
 msgctxt "help:party.party,sale_invoice_method:"
 msgid ""
 "The default sale invoice method for the customer.\n"
 "Leave empty to use the default value from the configuration."
 msgstr ""
 "Metoda implicită de facturare pentru client.\n"
@@ -685,15 +665,15 @@
 "Leave empty to use the default value from the configuration."
 msgstr ""
 "Metoda implicită de facturare pentru client.\n"
 "Lăsaţi gol pentru a utiliza valoarea implicită din configurare."
 
 msgctxt "help:party.party.customer_currency,customer_currency:"
 msgid "Default currency for sales to this party."
-msgstr ""
+msgstr "Moneda implicită pentru vânzări către această parte."
 
 msgctxt "help:product.configuration,default_lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "Used for products without a lead time."
 msgstr ""
 "Timpul între confirmarea vânzării pana la trimiterea al produselor.\n"
@@ -713,27 +693,27 @@
 "If empty the default lead time from the configuration is used."
 msgstr ""
 "Timpul de la confirmarea vânzării pana la trimiterea al produselor.\n"
 "Daca este gol se va folosi timpul implicit de execuţie."
 
 msgctxt "help:product.product,sale_uom:"
 msgid "The default Unit of Measure for sales."
-msgstr ""
+msgstr "Unitatea de Masura implicita pentru vanzari."
 
 msgctxt "help:product.template,lead_time:"
 msgid ""
 "The time from confirming the sales order to sending the products.\n"
 "If empty the default lead time from the configuration is used."
 msgstr ""
 "Timpul de la confirmarea vânzării pana la trimiterea al produselor.\n"
 "Daca este gol se va folosi timpul implicit de execuţie."
 
 msgctxt "help:product.template,sale_uom:"
 msgid "The default Unit of Measure for sales."
-msgstr ""
+msgstr "Unitatea de Masura Implicita pentru vanzari."
 
 msgctxt "help:sale.configuration,sale_process_after:"
 msgid ""
 "The grace period during which confirmed sale can still be reset to draft.\n"
 "Applied if a worker queue is activated."
 msgstr ""
 "Perioada de grație în timpul căreia vânzarea confirmată poate fi încă resetată la draft.\n"
@@ -742,15 +722,15 @@
 msgctxt "help:sale.handle.invoice.exception.ask,recreate_invoices:"
 msgid ""
 "The selected invoices will be recreated. The other ones will be ignored."
 msgstr "Facturile selectate vor fi recreate. Celelalte vor fi ignorate."
 
 msgctxt "help:sale.line,product_uom_category:"
 msgid "The category of Unit of Measure for the product."
-msgstr ""
+msgstr "Categoria de Unitate de Masura pentru produs."
 
 msgctxt "help:sale.sale,shipping_date:"
 msgid "When the shipping of goods should start."
 msgstr "Când ar trebui sa se expediază marfa."
 
 msgctxt "model:ir.action,name:act_invoice_form"
 msgid "Invoices"
@@ -768,18 +748,17 @@
 msgid "Sales per Subdivision"
 msgstr "Vânzări pe subdiviziune"
 
 msgctxt "model:ir.action,name:act_reporting_country_time_series"
 msgid "Sales per Country"
 msgstr "Vânzări pe țară"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_country_tree"
 msgid "Sales per Country"
-msgstr "Vânzări pe țară"
+msgstr "Vânzări per țară"
 
 msgctxt "model:ir.action,name:act_reporting_customer"
 msgid "Sales per Customer"
 msgstr "Vânzări pe client"
 
 msgctxt "model:ir.action,name:act_reporting_customer_category"
 msgid "Sales per Customer Category"
@@ -821,46 +800,42 @@
 msgid "Sales per Product Category"
 msgstr "Vânzări pe Categorie de Produs"
 
 msgctxt "model:ir.action,name:act_reporting_product_time_series"
 msgid "Sales per Product"
 msgstr "Vânzări pe produs"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_reporting_region_tree"
 msgid "Sales per Region"
-msgstr "Vânzări pe regiune"
+msgstr "Vânzări per regiune"
 
 msgctxt "model:ir.action,name:act_return_form"
 msgid "Returns"
 msgstr "Retururi"
 
 msgctxt "model:ir.action,name:act_sale_configuration_form"
 msgid "Configuration"
 msgstr "Configurare"
 
 msgctxt "model:ir.action,name:act_sale_form"
 msgid "Sales"
 msgstr "Vânzări"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_sale_line_relate"
 msgid "Sale Lines"
-msgstr "Rând de vânzare"
+msgstr "Rânduri de vânzare"
 
 msgctxt "model:ir.action,name:act_sale_move_relate"
 msgid "Moves"
 msgstr "Mișcări"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_sale_relate"
 msgid "Sales"
 msgstr "Vânzări"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_sale_relate_simple"
 msgid "Sales"
 msgstr "Vânzări"
 
 msgctxt "model:ir.action,name:act_shipment_form"
 msgid "Shipments"
 msgstr "Expedieri"
@@ -873,20 +848,18 @@
 msgid "Handle Invoice Exception"
 msgstr "Gestionare Excepție Factura"
 
 msgctxt "model:ir.action,name:wizard_modify_header"
 msgid "Modify Header"
 msgstr "Modificați antetul"
 
-#, fuzzy
 msgctxt "model:ir.action,name:wizard_reporting_country_tree_open"
 msgid "Open Region"
 msgstr "Regiune deschisă"
 
-#, fuzzy
 msgctxt "model:ir.action,name:wizard_reporting_region_tree_open"
 msgid "Open Region"
 msgstr "Regiune deschisă"
 
 msgctxt "model:ir.action,name:wizard_return_sale"
 msgid "Return Sale"
 msgstr "Retur Vânzarii"
@@ -919,41 +892,37 @@
 msgstr "Se prelucreaza"
 
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_sale_form_domain_quotation"
 msgid "Quotation"
 msgstr "Ofertă"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_all"
 msgid "All"
 msgstr "Tot"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_done"
 msgid "Done"
 msgstr "Terminat"
 
 msgctxt "model:ir.action.act_window.domain,name:act_sale_line_relate_pending"
 msgid "Pending"
-msgstr ""
+msgstr "In derulare"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_all"
 msgid "All"
 msgstr "Tot"
 
-#, fuzzy
 msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_done"
 msgid "Done"
 msgstr "Terminat"
 
 msgctxt "model:ir.action.act_window.domain,name:act_sale_relate_pending"
 msgid "Pending"
-msgstr ""
+msgstr "In derulare"
 
 msgctxt "model:ir.message,text:msg_erase_party_pending_sale"
 msgid ""
 "You cannot erase party \"%(party)s\" while they have pending sales with "
 "company \"%(company)s\"."
 msgstr ""
 "Nu se poate șterge parte \"%(party)s\" când au vănzări nefinalizate cu "
@@ -990,40 +959,41 @@
 msgid ""
 "You cannot reset invoice \"%(invoice)s\" to draft because it was generated "
 "by a sale."
 msgstr ""
 "Nu puteți devalida factura \"%(invoice)s\", deoarece a fost generată de o "
 "vânzare."
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_line_create_draft"
 msgid ""
 "You cannot add lines to sale \"%(sale)s\" because it is no longer in a draft"
 " state."
 msgstr ""
-"Pentru a modifica antetul vânzării \"%(sale)s\", acesta trebuie să fie în "
-"stare devalidata."
+"Nu puteți adăuga rânduri la vânzarea \"%(sale)s\" deoarece nu mai este în "
+"stare de ciornă."
 
 msgctxt "model:ir.message,text:msg_sale_line_delete_cancel_draft"
 msgid ""
 "To delete line \"%(line)s\" you must cancel or reset to draft sale "
 "\"%(sale)s\"."
 msgstr ""
 "Pentru a șterge rândul \"%(line)s\" trebuie anulat sau resetat \"%(sale)s\" "
 "la proiectul de vânzare."
 
 msgctxt "model:ir.message,text:msg_sale_line_move_quantity"
 msgid ""
 "The sale line \"%(line)s\" is moving %(extra)s in addition to the "
 "%(quantity)s ordered."
 msgstr ""
+"Linia de vânzare \"%(line)s\" mută %(extra)s în plus față de %(quantity)s "
+"comandată."
 
 msgctxt "model:ir.message,text:msg_sale_line_tax_unique"
 msgid "A tax can be added only once to a sale line."
-msgstr "O taxă poate fi adăugată o singură dată la o linie de vânzare."
+msgstr "O taxă poate fi adăugată o singură dată la un rând de vânzare."
 
 msgctxt "model:ir.message,text:msg_sale_missing_account_revenue"
 msgid "To invoice sale \"%(sale)s\" you must configure a default account revenue."
 msgstr ""
 "Pentru facturarea vânzării \"%(sale)s\" trebuie să configurati un cont "
 "implicit pentru venit."
 
@@ -1073,15 +1043,14 @@
 msgid "Revenue"
 msgstr "Venit"
 
 msgctxt "model:ir.message,text:msg_sale_reporting_revenue_trend"
 msgid "Revenue Trend"
 msgstr "Tendința veniturilor"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_sale_reporting_time_series"
 msgid "Time Series"
 msgstr "Seria de timp"
 
 msgctxt ""
 "model:ir.message,text:msg_sale_shipment_address_required_for_quotation"
 msgid "To get a quote for sale \"%(sale)s\" you must enter a shipment address."
@@ -1111,23 +1080,21 @@
 msgid "Handle Invoice Exception"
 msgstr "Gestionare Excepție Factura"
 
 msgctxt "model:ir.model.button,string:sale_handle_shipment_exception_button"
 msgid "Handle Shipment Exception"
 msgstr "Gestioneaza Excepție de expediere"
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:sale_manual_invoice_button"
 msgid "Create Invoice"
-msgstr "Recreați facturi"
+msgstr "Creare Factura"
 
-#, fuzzy
 msgctxt "model:ir.model.button,string:sale_manual_shipment_button"
 msgid "Create Shipment"
-msgstr "Expedieri"
+msgstr "Creare Expediere"
 
 msgctxt "model:ir.model.button,string:sale_modify_header_button"
 msgid "Modify Header"
 msgstr "Modificare Antet"
 
 msgctxt "model:ir.model.button,string:sale_process_button"
 msgid "Process"
@@ -1143,15 +1110,14 @@
 msgstr "Utilizator în companii"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_country_time_series_companies"
 msgid "User in companies"
 msgstr "Utilizator în companii"
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_reporting_country_tree_companies"
 msgid "User in companies"
 msgstr "Utilizator în companii"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_customer_category_companies"
 msgid "User in companies"
@@ -1169,39 +1135,39 @@
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_customer_time_series_companies"
 msgid "User in companies"
 msgstr "Utilizator în companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_main_companies"
 msgid "User in companies"
-msgstr "Utilizator în companii"
+msgstr "Utilizator în Companii"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_main_time_series_companies"
 msgid "User in companies"
-msgstr "Utilizator în companii"
+msgstr "Utilizator în Companii"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_product_category_companies"
 msgid "User in companies"
 msgstr "Utilizator în companii"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_product_category_time_series_companies"
 msgid "User in companies"
 msgstr "Utilizator în companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_reporting_product_companies"
 msgid "User in companies"
-msgstr "Utilizator în companii"
+msgstr "Utilizator în Companii"
 
 msgctxt ""
 "model:ir.rule.group,name:rule_group_reporting_product_time_series_companies"
 msgid "User in companies"
-msgstr "Utilizator în companii"
+msgstr "Utilizator în Companii"
 
 msgctxt "model:ir.rule.group,name:rule_group_sale_companies"
 msgid "User in companies"
 msgstr "Utilizator în companii"
 
 msgctxt "model:ir.sequence,name:sequence_sale"
 msgid "Sale"
@@ -1241,28 +1207,27 @@
 
 msgctxt "model:ir.ui.menu,name:menu_sale_form"
 msgid "Sales"
 msgstr "Vânzări"
 
 msgctxt "model:party.party.customer_currency,name:"
 msgid "Party Customer Currency"
-msgstr ""
+msgstr "Valută Clientului"
 
 msgctxt "model:party.party.sale_method,name:"
 msgid "Party Sale Method"
 msgstr "Metodă de Vânzare al Părţi"
 
 msgctxt "model:product.configuration.default_lead_time,name:"
 msgid "Product Default Lead Time"
 msgstr "Timpul Implicit de Execuţie al Produsului"
 
-#, fuzzy
 msgctxt "model:product.lead_time,name:"
 msgid "Product Lead Time"
-msgstr "Timpul Implicit de Execuţie al Produsului"
+msgstr "Timp de Execuţie al Produsului"
 
 msgctxt "model:product.sale.context,name:"
 msgid "Product Sale Context"
 msgstr "Contextul vânzării produselor"
 
 msgctxt "model:res.group,name:group_sale"
 msgid "Sales"
@@ -1294,19 +1259,19 @@
 
 msgctxt "model:sale.line,name:"
 msgid "Sale Line"
 msgstr "Rând de vânzare"
 
 msgctxt "model:sale.line-account.tax,name:"
 msgid "Sale Line - Tax"
-msgstr "Linie de vânzare - impozit"
+msgstr "Rând Vânzare - Impozit"
 
 msgctxt "model:sale.line-ignored-stock.move,name:"
 msgid "Sale Line - Ignored Move"
-msgstr "Linie de vânzare - Mișcare Ignorată"
+msgstr "Rând de vânzare - Mișcare Ignorată"
 
 msgctxt "model:sale.line-recreated-stock.move,name:"
 msgid "Sale Line - Recreated Move"
 msgstr "Rând de vânzare - Mișcare recreată"
 
 msgctxt "model:sale.reporting.context,name:"
 msgid "Sale Reporting Context"
@@ -1324,18 +1289,17 @@
 msgid "Sale Reporting per Subdivision"
 msgstr "Raportarea vânzărilor pe subdiviziune"
 
 msgctxt "model:sale.reporting.country.time_series,name:"
 msgid "Sale Reporting per Country"
 msgstr "Raportarea vânzărilor pe țară"
 
-#, fuzzy
 msgctxt "model:sale.reporting.country.tree,name:"
 msgid "Sale Reporting per Country"
-msgstr "Raportarea vânzărilor pe țară"
+msgstr "Raportare vânzări per țară"
 
 msgctxt "model:sale.reporting.customer,name:"
 msgid "Sale Reporting per Customer"
 msgstr "Raportarea vânzărilor pe client"
 
 msgctxt "model:sale.reporting.customer.category,name:"
 msgid "Sale Reporting per Customer Category"
@@ -1377,18 +1341,17 @@
 msgid "Sale Reporting per Product Category"
 msgstr "Raportarea Vânzărilor pe Categorie de Produse"
 
 msgctxt "model:sale.reporting.product.time_series,name:"
 msgid "Sale Reporting per Product"
 msgstr "Raportarea vânzărilor pe produs"
 
-#, fuzzy
 msgctxt "model:sale.reporting.region.tree,name:"
 msgid "Sale Reporting per Region"
-msgstr "Raportarea vânzărilor pe regiune"
+msgstr "Raportare vânzări per regiune"
 
 msgctxt "model:sale.return_sale.start,name:"
 msgid "Return Sale"
 msgstr "Retur Vânzare"
 
 msgctxt "model:sale.sale,name:"
 msgid "Sale"
@@ -1410,18 +1373,17 @@
 msgid "Amount"
 msgstr "Suma"
 
 msgctxt "report:sale.sale:"
 msgid "Date:"
 msgstr "Data:"
 
-#, fuzzy
 msgctxt "report:sale.sale:"
 msgid "Delivery Address:"
-msgstr "Adresa de facturare"
+msgstr "Adresa de livrare:"
 
 msgctxt "report:sale.sale:"
 msgid "Description"
 msgstr "Descriere"
 
 msgctxt "report:sale.sale:"
 msgid "Description:"
@@ -1513,15 +1475,15 @@
 
 msgctxt "selection:sale.sale,invoice_method:"
 msgid "On Shipment Sent"
 msgstr "La expediere trimis"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Awaiting Payment"
-msgstr ""
+msgstr "În așteptarea plății"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Exception"
 msgstr "Excepție"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "None"
@@ -1529,19 +1491,19 @@
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Paid"
 msgstr "Plătit"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Partially Paid"
-msgstr ""
+msgstr "Plătit Parțial"
 
 msgctxt "selection:sale.sale,invoice_state:"
 msgid "Pending"
-msgstr ""
+msgstr "In derulare"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "Manual"
 msgstr "Manual"
 
 msgctxt "selection:sale.sale,shipment_method:"
 msgid "On Invoice Paid"
@@ -1557,15 +1519,15 @@
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "None"
 msgstr "Nici unul"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Partially Shipped"
-msgstr ""
+msgstr "Livrat parțial"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Sent"
 msgstr "Trimis"
 
 msgctxt "selection:sale.sale,shipment_state:"
 msgid "Waiting"
```

### Comparing `trytond_sale-7.0.3/locale/ru.po` & `trytond_sale-7.2.0/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,19 @@
 msgid "From Location"
 msgstr "Из местоположения"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Строки инвойса"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Адрес для инвойса"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Перемещения"
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
```

### Comparing `trytond_sale-7.0.3/locale/sl.po` & `trytond_sale-7.2.0/locale/sl.po`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,19 @@
 msgid "From Location"
 msgstr "Iz lokacije"
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr "Postavke računa"
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Naslov plačnika"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr "Promet"
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
```

### Comparing `trytond_sale-7.0.3/locale/tr.po` & `trytond_sale-7.2.0/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -222,14 +222,19 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Invoices"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
@@ -1391,14 +1396,15 @@
 msgid "Sale - Ignored Invoice"
 msgstr ""
 
 msgctxt "model:sale.sale-recreated-account.invoice,name:"
 msgid "Sale - Recreated Invoice"
 msgstr ""
 
+#, fuzzy
 msgctxt "report:sale.sale:"
 msgid ":"
 msgstr ":"
 
 msgctxt "report:sale.sale:"
 msgid "Amount"
 msgstr ""
```

### Comparing `trytond_sale-7.0.3/locale/uk.po` & `trytond_sale-7.2.0/locale/uk.po`

 * *Files 0% similar despite different names*

```diff
@@ -210,14 +210,18 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr ""
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr ""
 
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
 msgstr ""
```

### Comparing `trytond_sale-7.0.3/locale/zh_CN.po` & `trytond_sale-7.2.0/locale/zh_CN.po`

 * *Files 0% similar despite different names*

```diff
@@ -223,14 +223,19 @@
 msgid "From Location"
 msgstr ""
 
 msgctxt "field:sale.line,invoice_lines:"
 msgid "Invoice Lines"
 msgstr ""
 
+#, fuzzy
+msgctxt "field:sale.line,invoice_progress:"
+msgid "Invoice Progress"
+msgstr "Invoices"
+
 msgctxt "field:sale.line,moves:"
 msgid "Moves"
 msgstr ""
 
 #, fuzzy
 msgctxt "field:sale.line,moves_exception:"
 msgid "Moves Exception"
```

### Comparing `trytond_sale-7.0.3/message.xml` & `trytond_sale-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/party.py` & `trytond_sale-7.2.0/party.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     CompanyMultiValueMixin, CompanyValueMixin)
 from trytond.modules.party.exceptions import EraseError
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval
 from trytond.transaction import Transaction
 
 customer_currency = fields.Many2One(
-    'currency.currency', "Customer Currency",
+    'currency.currency', "Customer Currency", ondelete='RESTRICT',
     help="Default currency for sales to this party.")
 
 
 def get_sale_methods(field_name):
     @classmethod
     def func(cls):
         pool = Pool()
```

### Comparing `trytond_sale-7.0.3/party.xml` & `trytond_sale-7.2.0/party.xml`

 * *Files 17% similar despite different names*

#### Comparing `trytond_sale-7.0.3/party.xml` & `trytond_sale-7.2.0/party.xml`

```diff
@@ -10,41 +10,47 @@
     </record>
     <record model="ir.action.wizard" id="act_open_customer">
       <field name="name">Parties associated to Sales</field>
       <field name="wiz_name">sale.open_customer</field>
     </record>
     <menuitem name="Associated to Sales" parent="party.menu_party_form" action="act_open_customer" sequence="50" id="menu_customer" icon="tryton-list"/>
     <record model="ir.model.field.access" id="access_party_sale_invoice_method">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'sale_invoice_method')]"/>
+      <field name="model">party.party</field>
+      <field name="field">sale_invoice_method</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_sale_invoice_method_group_sale">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'sale_invoice_method')]"/>
+      <field name="model">party.party</field>
+      <field name="field">sale_invoice_method</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_party_sale_shipment_method">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'sale_shipment_method')]"/>
+      <field name="model">party.party</field>
+      <field name="field">sale_shipment_method</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_sale_shipment_method_group_sale">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'sale_shipment_method')]"/>
+      <field name="model">party.party</field>
+      <field name="field">sale_shipment_method</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_party_customer_currency">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'customer_currency')]"/>
+      <field name="model">party.party</field>
+      <field name="field">customer_currency</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_customer_currency_group_sale">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'customer_currency')]"/>
+      <field name="model">party.party</field>
+      <field name="field">customer_currency</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_sale-7.0.3/product.py` & `trytond_sale-7.2.0/product.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 
 
 class DefaultLeadTime(ModelSQL, ValueMixin):
     "Product Default Lead Time"
     __name__ = 'product.configuration.default_lead_time'
     default_lead_time = default_lead_time
 
+    @classmethod
+    def default_default_lead_time(cls, **pattern):
+        return datetime.timedelta(0)
+
 
 class Template(metaclass=PoolMeta):
     __name__ = 'product.template'
     salable = fields.Boolean("Salable")
     sale_uom = fields.Many2One(
         'product.uom', "Sale UoM",
         states={
@@ -157,16 +161,16 @@
         assert len(products) == len(set(products)), "Duplicate products"
 
         uom = None
         if context.get('uom'):
             uom = Uom(context['uom'])
 
         currency = None
-        if Transaction().context.get('currency'):
-            currency = Currency(Transaction().context.get('currency'))
+        if context.get('currency'):
+            currency = Currency(context.get('currency'))
         company = None
         if context.get('company'):
             company = Company(context['company'])
         date = context.get('sale_date') or Date.today()
 
         for product in products:
             unit_price = product._get_sale_unit_price(quantity=quantity)
```

### Comparing `trytond_sale-7.0.3/product.xml` & `trytond_sale-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/sale.fodt` & `trytond_sale-7.2.0/sale.fodt`

 * *Files 0% similar despite different names*

#### Comparing `trytond_sale-7.0.3/sale.fodt` & `trytond_sale-7.2.0/sale.fodt`

```diff
@@ -601,15 +601,15 @@
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
@@ -621,15 +621,15 @@
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
@@ -793,18 +793,18 @@
           <table:covered-table-cell/>
           <table:covered-table-cell/>
           <table:covered-table-cell/>
         </table:table-row>
         <table:table-row>
           <table:table-cell table:style-name="Table1.A5" office:value-type="string">
             <text:p text:style-name="P20">
-              <text:placeholder text:placeholder-type="text">&lt;if test=&quot;line.product&quot;&gt;</text:placeholder>
+              <text:placeholder text:placeholder-type="text">&lt;if test=&quot;line.product_name&quot;&gt;</text:placeholder>
             </text:p>
             <text:p text:style-name="P20">
-              <text:placeholder text:placeholder-type="text">&lt;line.product.rec_name&gt;</text:placeholder>
+              <text:placeholder text:placeholder-type="text">&lt;line.product_name&gt;</text:placeholder>
             </text:p>
             <text:p text:style-name="P20">
               <text:placeholder text:placeholder-type="text">&lt;/if&gt;</text:placeholder>
             </text:p>
             <text:p text:style-name="P20">
               <text:placeholder text:placeholder-type="text">&lt;if test=&quot;line.description&quot;&gt;</text:placeholder>
             </text:p>
```

### Comparing `trytond_sale-7.0.3/sale.py` & `trytond_sale-7.2.0/sale.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
+import math
 from collections import defaultdict
 from decimal import Decimal
 from functools import partial
 from itertools import chain, groupby
 
+from sql import Null
 from sql.functions import CharLength
 
+from trytond import backend
 from trytond.i18n import gettext
 from trytond.ir.attachment import AttachmentCopyMixin
 from trytond.ir.note import NoteCopyMixin
 from trytond.model import (
     Index, Model, ModelSQL, ModelView, Unique, Workflow, fields,
     sequence_ordered)
 from trytond.model.exceptions import AccessError
@@ -20,15 +23,15 @@
 from trytond.modules.company import CompanyReport
 from trytond.modules.company.model import (
     employee_field, reset_employee, set_employee)
 from trytond.modules.currency.fields import Monetary
 from trytond.modules.product import price_digits
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, If, PYSONEncoder
-from trytond.tools import firstline, sortable_values
+from trytond.tools import cached_property, firstline, sortable_values
 from trytond.transaction import Transaction
 from trytond.wizard import (
     Button, StateAction, StateTransition, StateView, Wizard)
 
 from .exceptions import (
     PartyLocationError, SaleMoveQuantity, SaleQuotationError,
     SaleValidationError)
@@ -119,14 +122,15 @@
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
@@ -140,14 +144,15 @@
             })
     shipment_party = fields.Many2One('party.party', 'Shipment Party',
         states={
             'readonly': (Eval('state') != 'draft'),
             },
         context={
             'company': Eval('company', -1),
+            'party_contact_mechanism_usage': 'delivery',
             },
         search_context={
             'related_party': Eval('party'),
             },
         depends={'company'})
     shipment_address = fields.Many2One('party.address', 'Shipment Address',
         domain=['OR',
@@ -205,16 +210,24 @@
             ('partially paid', "Partially Paid"),
             ('paid', 'Paid'),
             ('exception', 'Exception'),
             ], 'Invoice State', readonly=True, required=True, sort=False)
     invoices = fields.Function(fields.Many2Many(
             'account.invoice', None, None, "Invoices"),
         'get_invoices', searcher='search_invoices')
-    invoices_ignored = fields.Many2Many('sale.sale-ignored-account.invoice',
-            'sale', 'invoice', 'Ignored Invoices', readonly=True)
+    invoices_ignored = fields.Many2Many(
+        'sale.sale-ignored-account.invoice', 'sale', 'invoice',
+        "Ignored Invoices",
+        domain=[
+            ('id', 'in', Eval('invoices', [])),
+            ('state', '=', 'cancelled'),
+            ],
+        states={
+            'invisible': ~Eval('invoices_ignored', []),
+            })
     invoices_recreated = fields.Many2Many(
         'sale.sale-recreated-account.invoice', 'sale', 'invoice',
         'Recreated Invoices', readonly=True)
     shipment_method = fields.Selection([
             ('manual', 'Manual'),
             ('order', 'On Order Processed'),
             ('invoice', 'On Invoice Paid'),
@@ -331,15 +344,15 @@
                     },
                 'confirm': {
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
@@ -387,15 +400,17 @@
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
     def default_payment_term(cls, **pattern):
         pool = Pool()
         Configuration = pool.get('account.configuration')
         config = Configuration(1)
         payment_term = config.get_multivalue(
@@ -649,18 +664,18 @@
     search_shipment_returns = search_shipments_returns(
         'stock.shipment.out.return')
 
     def get_shipment_state(self):
         '''
         Return the shipment state for the sale.
         '''
-        if self.moves:
-            if any(l.moves_exception for l in self.lines):
-                return 'exception'
-            elif all(l.moves_progress >= 1.0 for l in self.lines
+        if any(l.moves_exception for l in self.lines):
+            return 'exception'
+        elif any(m.state != 'cancelled' for m in self.moves):
+            if all(l.moves_progress >= 1.0 for l in self.lines
                     if l.moves_progress is not None):
                 return 'sent'
             elif any(l.moves_progress for l in self.lines):
                 return 'partially shipped'
             else:
                 return 'waiting'
         return 'none'
@@ -965,20 +980,24 @@
                 + [x[1] for x in grouped_moves])
             shipments.append(shipment)
         return shipments
 
     def is_done(self):
         return ((self.invoice_state == 'paid'
                 or (self.invoice_state == 'none'
-                    and self.invoice_method != 'manual'))
+                    and all(
+                        l.invoice_progress >= 1
+                        for l in self.lines
+                        if l.invoice_progress is not None)))
             and (self.shipment_state == 'sent'
                 or (self.shipment_state == 'none'
-                    and self.shipment_method != 'manual')
-                or all(l.product.type == 'service'
-                    for l in self.lines if l.product)))
+                    and all(
+                        l.moves_progress >= 1
+                        for l in self.lines
+                        if l.moves_progress is not None))))
 
     @classmethod
     def delete(cls, sales):
         # Cancel before delete
         cls.cancel(sales)
         for sale in sales:
             if sale.state != 'cancelled':
@@ -1167,29 +1186,49 @@
     def modify_header(cls, sales):
         pass
 
 
 class SaleIgnoredInvoice(ModelSQL):
     'Sale - Ignored Invoice'
     __name__ = 'sale.sale-ignored-account.invoice'
-    _table = 'sale_invoice_ignored_rel'
     sale = fields.Many2One(
         'sale.sale', "Sale", ondelete='CASCADE', required=True)
     invoice = fields.Many2One(
-        'account.invoice', "Invoice", ondelete='RESTRICT', required=True)
+        'account.invoice', "Invoice", ondelete='RESTRICT', required=True,
+        domain=[
+            ('sales', '=', Eval('sale', -1)),
+            ('state', '=', 'cancelled'),
+            ])
+
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'sale_invoice_ignored_rel', cls._table)
+        super().__register__(module)
 
 
 class SaleRecreatedInvoice(ModelSQL):
     'Sale - Recreated Invoice'
     __name__ = 'sale.sale-recreated-account.invoice'
-    _table = 'sale_invoice_recreated_rel'
     sale = fields.Many2One(
         'sale.sale', "Sale", ondelete='CASCADE', required=True)
     invoice = fields.Many2One(
-        'account.invoice', "Invoice", ondelete='RESTRICT', required=True)
+        'account.invoice', "Invoice", ondelete='RESTRICT', required=True,
+        domain=[
+            ('sales', '=', Eval('sale', -1)),
+            ('state', '=', 'cancelled'),
+            ])
+
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'sale_invoice_recreated_rel', cls._table)
+        super().__register__(module)
 
 
 class SaleLine(TaxableMixin, sequence_ordered(), ModelSQL, ModelView):
     'Sale Line'
     __name__ = 'sale.line'
     sale = fields.Many2One(
         'sale.sale', "Sale", ondelete='CASCADE', required=True,
@@ -1326,21 +1365,32 @@
             },
         depends={'sale'})
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
-    moves_ignored = fields.Many2Many('sale.line-ignored-stock.move',
-            'sale_line', 'move', 'Ignored Moves', readonly=True)
+    moves_ignored = fields.Many2Many(
+        'sale.line-ignored-stock.move', 'sale_line', 'move',
+        "Ignored Moves",
+        domain=[
+            ('id', 'in', Eval('moves', [])),
+            ('state', '=', 'cancelled'),
+            ],
+        states={
+            'invisible': ~Eval('moves_ignored', []),
+            })
     moves_recreated = fields.Many2Many('sale.line-recreated-stock.move',
             'sale_line', 'move', 'Recreated Moves', readonly=True)
     moves_exception = fields.Function(
         fields.Boolean("Moves Exception"), 'get_moves_exception')
     moves_progress = fields.Function(
         fields.Float("Moves Progress", digits=(1, 4)),
         'get_moves_progress')
@@ -1386,32 +1436,75 @@
         cls._order.insert(0, ('sale.sale_date', 'DESC NULLS FIRST'))
         cls._order.insert(1, ('sale.id', 'DESC'))
 
     @staticmethod
     def default_type():
         return 'line'
 
-    @fields.depends('type')
+    @fields.depends('type', 'taxes')
     def on_change_type(self):
         if self.type != 'line':
             self.product = None
             self.unit = None
             self.taxes = None
 
     @property
+    def _invoice_remaining_quantity(self):
+        "Compute the remaining quantity to be paid"
+        pool = Pool()
+        UoM = pool.get('product.uom')
+        if self.type != 'line':
+            return
+        skips = set(self.sale.invoices_ignored)
+        quantity = self.quantity
+        if self.sale.invoice_method == 'shipment':
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
         "Compute the remaining quantity to ship"
         pool = Pool()
         Uom = pool.get('product.uom')
         if self.type != 'line' or not self.product:
             return
         if self.product.type == 'service':
             return
         skips = set(self.moves_ignored)
         quantity = abs(self.quantity)
+        if self.sale.shipment_method == 'invoice':
+            invoices_ignored = set(self.sale.invoices_ignored)
+            for invoice_line in self.invoice_lines:
+                if invoice_line.type != 'line':
+                    continue
+                if invoice_line.invoice in invoices_ignored:
+                    quantity -= Uom.compute_qty(
+                        invoice_line.unit or self.unit, invoice_line.quantity,
+                        self.unit)
         for move in self.moves:
             if move.state == 'done' or move in skips:
                 quantity -= Uom.compute_qty(
                     move.unit, move.quantity, self.unit)
         return quantity
 
     def get_moves_exception(self, name):
@@ -1422,15 +1515,15 @@
 
     def get_moves_progress(self, name):
         progress = None
         quantity = self._move_remaining_quantity
         if quantity is not None and self.quantity:
             progress = round(
                 (abs(self.quantity) - quantity) / abs(self.quantity), 4)
-            progress = max(0, min(1, progress))
+            progress = max(0., min(1., progress))
         return progress
 
     @property
     def taxable_lines(self):
         # In case we're called from an on_change
         # we have to use some sensible defaults
         if getattr(self, 'type', None) == 'line':
@@ -1470,24 +1563,25 @@
             context['uom'] = self.unit.id
         elif self.product:
             context['uom'] = self.product.sale_uom.id
         context['taxes'] = [t.id for t in self.taxes or []]
         return context
 
     @fields.depends(
-        'sale', '_parent_sale.party', '_parent_sale.invoice_party',
+        'sale', 'taxes', '_parent_sale.party', '_parent_sale.invoice_party',
         methods=['compute_taxes', 'on_change_with_amount'])
     def on_change_sale(self):
         party = None
         if self.sale:
             party = self.sale.invoice_party or self.sale.party
         self.taxes = self.compute_taxes(party)
         self.amount = self.on_change_with_amount()
 
-    @fields.depends('product', 'unit', 'sale',
+    @fields.depends(
+        'product', 'unit', 'sale', 'taxes',
         '_parent_sale.party', '_parent_sale.invoice_party',
         methods=['compute_taxes', 'compute_unit_price',
             'on_change_with_amount'])
     def on_change_product(self):
         party = None
         if self.sale:
             party = self.sale.invoice_party or self.sale.party
@@ -1500,14 +1594,18 @@
             if not self.unit or self.unit.category != category:
                 self.unit = self.product.sale_uom
 
             self.unit_price = self.compute_unit_price()
 
         self.amount = self.on_change_with_amount()
 
+    @cached_property
+    def product_name(self):
+        return self.product.rec_name if self.product else ''
+
     @fields.depends(
         'type', 'product',
         methods=['on_change_with_company', '_get_tax_rule_pattern'])
     def compute_taxes(self, party):
         pool = Pool()
         AccountConfiguration = pool.get('account.configuration')
 
@@ -2010,48 +2108,73 @@
         default.setdefault('actual_quantity')
         return super(SaleLine, cls).copy(lines, default=default)
 
 
 class SaleLineTax(ModelSQL):
     'Sale Line - Tax'
     __name__ = 'sale.line-account.tax'
-    _table = 'sale_line_account_tax'
     line = fields.Many2One(
         'sale.line', "Sale Line", ondelete='CASCADE', required=True)
     tax = fields.Many2One(
         'account.tax', "Tax", ondelete='RESTRICT', required=True)
 
     @classmethod
     def __setup__(cls):
         super().__setup__()
         t = cls.__table__()
         cls._sql_constraints += [
             ('line_tax_unique', Unique(t, t.line, t.tax),
                 'sale.msg_sale_line_tax_unique'),
             ]
 
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename('sale_line_account_tax', cls._table)
+        super().__register__(module)
+
 
 class SaleLineIgnoredMove(ModelSQL):
     'Sale Line - Ignored Move'
     __name__ = 'sale.line-ignored-stock.move'
-    _table = 'sale_line_moves_ignored_rel'
     sale_line = fields.Many2One(
         'sale.line', "Sale Line", ondelete='CASCADE', required=True)
     move = fields.Many2One(
-        'stock.move', "Move", ondelete='RESTRICT', required=True)
+        'stock.move', "Move", ondelete='RESTRICT', required=True,
+        domain=[
+            ('origin.id', '=', Eval('sale_line', -1), 'sale.line'),
+            ('state', '=', 'cancelled'),
+            ])
+
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'sale_line_moves_ignored_rel', cls._table)
+        super().__register__(module)
 
 
 class SaleLineRecreatedMove(ModelSQL):
     'Sale Line - Recreated Move'
     __name__ = 'sale.line-recreated-stock.move'
-    _table = 'sale_line_moves_recreated_rel'
     sale_line = fields.Many2One(
         'sale.line', "Sale Line", ondelete='CASCADE', required=True)
     move = fields.Many2One(
-        'stock.move', "Move", ondelete='RESTRICT', required=True)
+        'stock.move', "Move", ondelete='RESTRICT', required=True,
+        domain=[
+            ('origin.id', '=', Eval('sale_line', -1), 'sale.line'),
+            ('state', '=', 'cancelled'),
+            ])
+
+    @classmethod
+    def __register__(cls, module):
+        # Migration from 7.0: rename to standard name
+        backend.TableHandler.table_rename(
+            'sale_line_moves_recreated_rel', cls._table)
+        super().__register__(module)
 
 
 class SaleReport(CompanyReport):
     __name__ = 'sale.sale'
 
     @classmethod
     def execute(cls, ids, data):
```

### Comparing `trytond_sale-7.0.3/sale.xml` & `trytond_sale-7.2.0/sale.xml`

 * *Files 10% similar despite different names*

#### Comparing `trytond_sale-7.0.3/sale.xml` & `trytond_sale-7.2.0/sale.xml`

```diff
@@ -201,106 +201,119 @@
     </record>
     <record model="ir.action.keyword" id="act_sale_relate_simple_keyword_shipment_out_return">
       <field name="keyword">form_relate</field>
       <field name="model">stock.shipment.out.return,-1</field>
       <field name="action" ref="act_sale_relate_simple"/>
     </record>
     <record model="ir.model.access" id="access_sale">
-      <field name="model" search="[('model', '=', 'sale.sale')]"/>
+      <field name="model">sale.sale</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_sale_sale">
-      <field name="model" search="[('model', '=', 'sale.sale')]"/>
+      <field name="model">sale.sale</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
+    <record model="ir.model.field.access" id="access_sale_sale_invoices_ignored">
+      <field name="model">sale.sale</field>
+      <field name="field">invoices_ignored</field>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="False"/>
+    </record>
+    <record model="ir.model.field.access" id="access_sale_sale_invoices_ignored_sale_admin">
+      <field name="model">sale.sale</field>
+      <field name="field">invoices_ignored</field>
+      <field name="group" ref="group_sale_admin"/>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="True"/>
+    </record>
     <record model="ir.rule.group" id="rule_group_sale_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.sale')]"/>
+      <field name="model">sale.sale</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_sale_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_sale_companies"/>
     </record>
     <record model="ir.model.button" id="sale_cancel_button">
+      <field name="model">sale.sale</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'sale.sale')]"/>
     </record>
     <record model="ir.model.button" id="sale_draft_button">
+      <field name="model">sale.sale</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'sale.sale')]"/>
     </record>
     <record model="ir.model.button" id="sale_quote_button">
+      <field name="model">sale.sale</field>
       <field name="name">quote</field>
       <field name="string">Quote</field>
-      <field name="model" search="[('model', '=', 'sale.sale')]"/>
     </record>
     <record model="ir.model.button" id="sale_confirm_button">
+      <field name="model">sale.sale</field>
       <field name="name">confirm</field>
       <field name="string">Confirm</field>
-      <field name="model" search="[('model', '=', 'sale.sale')]"/>
     </record>
     <record model="ir.model.button" id="sale_process_button">
+      <field name="model">sale.sale</field>
       <field name="name">process</field>
       <field name="string">Process</field>
-      <field name="model" search="[('model', '=', 'sale.sale')]"/>
     </record>
     <record model="ir.model.button-res.group" id="sale_process_button_group_sale_admin">
       <field name="button" ref="sale_process_button"/>
       <field name="group" ref="group_sale_admin"/>
     </record>
     <record model="ir.model.button" id="sale_manual_invoice_button">
+      <field name="model">sale.sale</field>
       <field name="name">manual_invoice</field>
       <field name="string">Create Invoice</field>
-      <field name="model" search="[('model', '=', 'sale.sale')]"/>
     </record>
     <record model="ir.model.button-res.group" id="sale_manual_invoice_button_group_sale">
       <field name="button" ref="sale_manual_invoice_button"/>
       <field name="group" ref="group_sale"/>
     </record>
     <record model="ir.model.button-res.group" id="sale_manual_invoice_button_group_account">
       <field name="button" ref="sale_manual_invoice_button"/>
       <field name="group" ref="account.group_account"/>
     </record>
     <record model="ir.model.button" id="sale_manual_shipment_button">
+      <field name="model">sale.sale</field>
       <field name="name">manual_shipment</field>
       <field name="string">Create Shipment</field>
-      <field name="model" search="[('model', '=', 'sale.sale')]"/>
     </record>
     <record model="ir.model.button-res.group" id="sale_manual_shipment_button_group_sale">
       <field name="button" ref="sale_manual_shipment_button"/>
       <field name="group" ref="group_sale"/>
     </record>
     <record model="ir.model.button-res.group" id="sale_manual_shipment_button_group_stock">
       <field name="button" ref="sale_manual_shipment_button"/>
       <field name="group" ref="stock.group_stock"/>
     </record>
     <record model="ir.model.button" id="sale_modify_header_button">
+      <field name="model">sale.sale</field>
       <field name="name">modify_header</field>
       <field name="string">Modify Header</field>
-      <field name="model" search="[('model', '=', 'sale.sale')]"/>
     </record>
     <record model="ir.model.button" id="sale_handle_shipment_exception_button">
+      <field name="model">sale.sale</field>
       <field name="name">handle_shipment_exception</field>
       <field name="string">Handle Shipment Exception</field>
-      <field name="model" search="[('model', '=', 'sale.sale')]"/>
     </record>
     <record model="ir.model.button" id="sale_handle_invoice_exception_button">
+      <field name="model">sale.sale</field>
       <field name="name">handle_invoice_exception</field>
       <field name="string">Handle Invoice Exception</field>
-      <field name="model" search="[('model', '=', 'sale.sale')]"/>
     </record>
     <record model="ir.sequence.type" id="sequence_type_sale">
       <field name="name">Sale</field>
     </record>
     <record model="ir.sequence.type-res.group" id="sequence_type_sale_group_admin">
       <field name="sequence_type" ref="sequence_type_sale"/>
       <field name="group" ref="res.group_admin"/>
@@ -337,14 +350,27 @@
     </record>
     <record model="ir.ui.view" id="sale_line_view_tree_sequence">
       <field name="model">sale.line</field>
       <field name="type">tree</field>
       <field name="priority" eval="20"/>
       <field name="name">sale_line_tree_sequence</field>
     </record>
+    <record model="ir.model.field.access" id="access_sale_line_moves_ignored">
+      <field name="model">sale.line</field>
+      <field name="field">moves_ignored</field>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="False"/>
+    </record>
+    <record model="ir.model.field.access" id="access_sale_line_moves_ignored_sale_admin">
+      <field name="model">sale.line</field>
+      <field name="field">moves_ignored</field>
+      <field name="group" ref="group_sale_admin"/>
+      <field name="perm_read" eval="True"/>
+      <field name="perm_write" eval="True"/>
+    </record>
     <record model="ir.action.act_window" id="act_sale_line_relate">
       <field name="name">Sale Lines</field>
       <field name="res_model">sale.line</field>
       <field name="domain" eval="[('type', '=', 'line'),                 If(Eval('active_model') == 'sale.sale',                 ('sale', 'in', Eval('active_ids', [])), ()),                 If(Eval('active_model') == 'product.product',                 ('product', 'in', Eval('active_ids', [])), ()),                 If(Eval('active_model') == 'product.template',                 ('product.template.id', 'in', Eval('active_ids', [])), ()),                 If(Eval('active_model') == 'party.party',                 ('customer', 'in', Eval('active_ids', [])), ()),                 ]" pyson="1"/>
     </record>
     <record model="ir.action.act_window.view" id="act_sale_line_relate_view1">
       <field name="sequence" eval="10"/>
```

### Comparing `trytond_sale-7.0.3/sale_reporting.py` & `trytond_sale-7.2.0/sale_reporting.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     import pygal
 except ImportError:
     pygal = None
 from dateutil.relativedelta import relativedelta
 from sql import Column, Literal, Null, Union, With
 from sql.aggregate import Count, Max, Min, Sum
 from sql.conditionals import Coalesce
-from sql.functions import Ceil, CurrentTimestamp, DateTrunc, Log, Power
+from sql.functions import Ceil, CurrentTimestamp, DateTrunc, Log, Power, Round
 from sql.operators import Concat
 
 from trytond.i18n import lazy_gettext
 from trytond.model import ModelSQL, ModelView, UnionMixin, fields, sum_tree
 from trytond.modules.currency.fields import Monetary
 from trytond.pool import Pool
 from trytond.pyson import Eval, If
@@ -34,18 +34,16 @@
         lazy_gettext("sale.msg_sale_reporting_revenue"),
         digits='currency', currency='currency')
     revenue_trend = fields.Function(
         fields.Char(lazy_gettext("sale.msg_sale_reporting_revenue_trend")),
         'get_trend')
     time_series = None
 
-    currency = fields.Function(fields.Many2One(
-            'currency.currency',
-            lazy_gettext("sale.msg_sale_reporting_currency")),
-        'get_currency')
+    currency = fields.Many2One(
+        'currency.currency', lazy_gettext("sale.msg_sale_reporting_currency"))
 
     @classmethod
     def table_query(cls):
         from_item, tables, withs = cls._joins()
         return from_item.select(*cls._columns(tables, withs),
             where=cls._where(tables, withs),
             group_by=cls._group_by(tables, withs),
@@ -97,65 +95,71 @@
 
         tables = {}
         company = context.get('company')
         lines = cls._lines()
         tables['line'] = line = Union(*(
                 l(len(lines), i, company) for i, l in enumerate(lines)))
         tables['line.company'] = company = Company.__table__()
+        tables['line.company.currency'] = currency = Currency.__table__()
         withs = {}
         currency_sale = With(query=Currency.currency_rate_sql())
         withs['currency_sale'] = currency_sale
         currency_company = With(query=Currency.currency_rate_sql())
         withs['currency_company'] = currency_company
 
         from_item = (line
             .join(currency_sale,
                 condition=(line.currency == currency_sale.currency)
                 & (currency_sale.start_date <= line.date)
                 & ((currency_sale.end_date == Null)
                     | (currency_sale.end_date > line.date))
                 )
             .join(company, condition=line.company == company.id)
+            .join(currency, condition=company.currency == currency.id)
             .join(currency_company,
                 condition=(company.currency == currency_company.currency)
                 & (currency_company.start_date <= line.date)
                 & ((currency_company.end_date == Null)
                     | (currency_company.end_date > line.date))
                 ))
         return from_item, tables, withs
 
     @classmethod
     def _columns(cls, tables, withs):
         line = tables['line']
+        currency = tables['line.company.currency']
         currency_company = withs['currency_company']
         currency_sale = withs['currency_sale']
 
-        revenue = cls.revenue.sql_cast(
-            Sum(line.quantity * line.unit_price
-                * currency_company.rate / currency_sale.rate))
+        revenue = Round(cls.revenue.sql_cast(
+                Sum(line.quantity * line.unit_price
+                    * currency_company.rate / currency_sale.rate)),
+            currency.digits)
         return [
             cls._column_id(tables, withs).as_('id'),
             Literal(0).as_('create_uid'),
             CurrentTimestamp().as_('create_date'),
             cls.write_uid.sql_cast(Literal(Null)).as_('write_uid'),
             cls.write_date.sql_cast(Literal(Null)).as_('write_date'),
             line.company.as_('company'),
             revenue.as_('revenue'),
             Count(line.order, distinct=True).as_('number'),
+            line.currency.as_('currency'),
             ]
 
     @classmethod
     def _column_id(cls, tables, withs):
         line = tables['line']
         return Min(line.id)
 
     @classmethod
     def _group_by(cls, tables, withs):
         line = tables['line']
-        return [line.company]
+        currency = tables['line.company.currency']
+        return [line.company, line.currency, currency.digits]
 
     @classmethod
     def _where(cls, tables, withs):
         pool = Pool()
         Location = pool.get('stock.location')
         context = Transaction().context
         line = tables['line']
@@ -204,17 +208,14 @@
         name = name[:-len('_trend')]
         if pygal:
             chart = pygal.Line()
             chart.add('', [getattr(ts, name) if ts else 0
                     for ts in self.time_series_all])
             return chart.render_sparktext()
 
-    def get_currency(self, name):
-        return self.company.currency.id
-
 
 class AbstractTimeseries(Abstract):
 
     date = fields.Date(lazy_gettext('sale.msg_sale_reporting_date'))
 
     @classmethod
     def __setup__(cls):
```

### Comparing `trytond_sale-7.0.3/sale_reporting.xml` & `trytond_sale-7.2.0/sale_reporting.xml`

 * *Files 11% similar despite different names*

#### Comparing `trytond_sale-7.0.3/sale_reporting.xml` & `trytond_sale-7.2.0/sale_reporting.xml`

```diff
@@ -39,30 +39,30 @@
     <record model="ir.action.keyword" id="act_reporting_main_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model" ref="menu_reporting_sale"/>
       <field name="action" ref="act_reporting_main"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_main_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.reporting.main')]"/>
+      <field name="model">sale.reporting.main</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_main_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_main_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_main">
-      <field name="model" search="[('model', '=', 'sale.reporting.main')]"/>
+      <field name="model">sale.reporting.main</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_main_sale">
-      <field name="model" search="[('model', '=', 'sale.reporting.main')]"/>
+      <field name="model">sale.reporting.main</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="reporting_main_time_series_view_list">
@@ -104,30 +104,30 @@
     <record model="ir.action.keyword" id="act_reporting_main_time_series_list_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">sale.reporting.main,-1</field>
       <field name="action" ref="act_reporting_main_time_series"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_main_time_series_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.reporting.main.time_series')]"/>
+      <field name="model">sale.reporting.main.time_series</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_main_time_series_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_main_time_series_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_main_time_series">
-      <field name="model" search="[('model', '=', 'sale.reporting.main.time_series')]"/>
+      <field name="model">sale.reporting.main.time_series</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_main_time_series_sale">
-      <field name="model" search="[('model', '=', 'sale.reporting.main.time_series')]"/>
+      <field name="model">sale.reporting.main.time_series</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <!-- Customer -->
@@ -178,30 +178,30 @@
     <record model="ir.action.keyword" id="act_reporting_customer_keyword2">
       <field name="keyword">tree_open</field>
       <field name="model">sale.reporting.customer.category.tree,-1</field>
       <field name="action" ref="act_reporting_customer"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_customer_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.reporting.customer')]"/>
+      <field name="model">sale.reporting.customer</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_customer_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_customer_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_customer">
-      <field name="model" search="[('model', '=', 'sale.reporting.customer')]"/>
+      <field name="model">sale.reporting.customer</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_customer_sale">
-      <field name="model" search="[('model', '=', 'sale.reporting.customer')]"/>
+      <field name="model">sale.reporting.customer</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="reporting_customer_time_series_view_list">
@@ -244,30 +244,30 @@
     <record model="ir.action.keyword" id="act_reporting_customer_time_series_list_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">sale.reporting.customer,-1</field>
       <field name="action" ref="act_reporting_customer_time_series"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_customer_time_series_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.reporting.customer.time_series')]"/>
+      <field name="model">sale.reporting.customer.time_series</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_customer_time_series_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_customer_time_series_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_customer_time_series">
-      <field name="model" search="[('model', '=', 'sale.reporting.customer.time_series')]"/>
+      <field name="model">sale.reporting.customer.time_series</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_customer_time_series_sale">
-      <field name="model" search="[('model', '=', 'sale.reporting.customer.time_series')]"/>
+      <field name="model">sale.reporting.customer.time_series</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <!-- Customer Category -->
@@ -313,30 +313,30 @@
     <record model="ir.action.keyword" id="act_reporting_customer_category_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">sale.reporting.customer.category.tree,-1</field>
       <field name="action" ref="act_reporting_customer_category"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_customer_category_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.reporting.customer.category')]"/>
+      <field name="model">sale.reporting.customer.category</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_customer_category_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_customer_category_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_customer_category">
-      <field name="model" search="[('model', '=', 'sale.reporting.customer.category')]"/>
+      <field name="model">sale.reporting.customer.category</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_customer_category_sale">
-      <field name="model" search="[('model', '=', 'sale.reporting.customer.category')]"/>
+      <field name="model">sale.reporting.customer.category</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="reporting_customer_category_time_series_view_list">
@@ -379,30 +379,30 @@
     <record model="ir.action.keyword" id="act_reporting_customer_category_time_series_list_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">sale.reporting.customer.category,-1</field>
       <field name="action" ref="act_reporting_customer_category_time_series"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_customer_category_time_series_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.reporting.customer.category.time_series')]"/>
+      <field name="model">sale.reporting.customer.category.time_series</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_customer_category_time_series_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_customer_category_time_series_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_customer_category_time_series">
-      <field name="model" search="[('model', '=', 'sale.reporting.customer.category.time_series')]"/>
+      <field name="model">sale.reporting.customer.category.time_series</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_customer_category_time_series_sale">
-      <field name="model" search="[('model', '=', 'sale.reporting.customer.category.time_series')]"/>
+      <field name="model">sale.reporting.customer.category.time_series</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <!-- Product -->
@@ -453,30 +453,30 @@
     <record model="ir.action.keyword" id="act_reporting_product_keyword2">
       <field name="keyword">tree_open</field>
       <field name="model">sale.reporting.product.category.tree,-1</field>
       <field name="action" ref="act_reporting_product"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_product_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.reporting.product')]"/>
+      <field name="model">sale.reporting.product</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_product_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_product_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_product">
-      <field name="model" search="[('model', '=', 'sale.reporting.product')]"/>
+      <field name="model">sale.reporting.product</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_product_sale">
-      <field name="model" search="[('model', '=', 'sale.reporting.product')]"/>
+      <field name="model">sale.reporting.product</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="reporting_product_time_series_view_list">
@@ -519,30 +519,30 @@
     <record model="ir.action.keyword" id="act_reporting_product_time_series_list_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">sale.reporting.product,-1</field>
       <field name="action" ref="act_reporting_product_time_series"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_product_time_series_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.reporting.product.time_series')]"/>
+      <field name="model">sale.reporting.product.time_series</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_product_time_series_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_product_time_series_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_product_time_series">
-      <field name="model" search="[('model', '=', 'sale.reporting.product.time_series')]"/>
+      <field name="model">sale.reporting.product.time_series</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_product_time_series_sale">
-      <field name="model" search="[('model', '=', 'sale.reporting.product.time_series')]"/>
+      <field name="model">sale.reporting.product.time_series</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <!-- Product Category -->
@@ -588,30 +588,30 @@
     <record model="ir.action.keyword" id="act_reporting_product_category_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">sale.reporting.product.category.tree,-1</field>
       <field name="action" ref="act_reporting_product_category"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_product_category_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.reporting.product.category')]"/>
+      <field name="model">sale.reporting.product.category</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_product_category_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_product_category_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_product_category">
-      <field name="model" search="[('model', '=', 'sale.reporting.product.category')]"/>
+      <field name="model">sale.reporting.product.category</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_product_category_sale">
-      <field name="model" search="[('model', '=', 'sale.reporting.product.category')]"/>
+      <field name="model">sale.reporting.product.category</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="reporting_product_category_time_series_view_list">
@@ -654,30 +654,30 @@
     <record model="ir.action.keyword" id="act_reporting_product_category_time_series_list_keyword1">
       <field name="keyword">tree_open</field>
       <field name="model">sale.reporting.product.category,-1</field>
       <field name="action" ref="act_reporting_product_category_time_series"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_product_category_time_series_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.reporting.product.category.time_series')]"/>
+      <field name="model">sale.reporting.product.category.time_series</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_product_category_time_series_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_product_category_time_series_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_product_category_time_series">
-      <field name="model" search="[('model', '=', 'sale.reporting.product.category.time_series')]"/>
+      <field name="model">sale.reporting.product.category.time_series</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_product_category_time_series_sale">
-      <field name="model" search="[('model', '=', 'sale.reporting.product.category.time_series')]"/>
+      <field name="model">sale.reporting.product.category.time_series</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <!-- Region -->
@@ -728,30 +728,30 @@
     <record model="ir.action.act_window.view" id="act_reporting_country_tree_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="reporting_country_tree_view_tree"/>
       <field name="act_window" ref="act_reporting_country_tree"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_country_tree_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.reporting.country.tree')]"/>
+      <field name="model">sale.reporting.country.tree</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_country_tree_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_country_tree_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_country_tree">
-      <field name="model" search="[('model', '=', 'sale.reporting.country.tree')]"/>
+      <field name="model">sale.reporting.country.tree</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_country_tree_sale">
-      <field name="model" search="[('model', '=', 'sale.reporting.country.tree')]"/>
+      <field name="model">sale.reporting.country.tree</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="reporting_country_time_series_view_list">
@@ -789,30 +789,30 @@
     <record model="ir.action.act_window.view" id="act_reporting_country_time_series_view3">
       <field name="sequence" eval="30"/>
       <field name="view" ref="reporting_country_time_series_view_graph_number"/>
       <field name="act_window" ref="act_reporting_country_time_series"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_country_time_series_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.reporting.country.time_series')]"/>
+      <field name="model">sale.reporting.country.time_series</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_country_time_series_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_country_time_series_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_country_time_series">
-      <field name="model" search="[('model', '=', 'sale.reporting.country.time_series')]"/>
+      <field name="model">sale.reporting.country.time_series</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_country_time_series_sale">
-      <field name="model" search="[('model', '=', 'sale.reporting.country.time_series')]"/>
+      <field name="model">sale.reporting.country.time_series</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="reporting_country_subdivision_time_series_view_list">
@@ -850,30 +850,30 @@
     <record model="ir.action.act_window.view" id="act_reporting_country_subdivision_time_series_view3">
       <field name="sequence" eval="30"/>
       <field name="view" ref="reporting_country_subdivision_time_series_view_graph_number"/>
       <field name="act_window" ref="act_reporting_country_subdivision_time_series"/>
     </record>
     <record model="ir.rule.group" id="rule_group_reporting_country_subdivision_time_series_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.reporting.country.subdivision.time_series')]"/>
+      <field name="model">sale.reporting.country.subdivision.time_series</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_reporting_country_subdivision_time_series_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_reporting_country_subdivision_time_series_companies"/>
     </record>
     <record model="ir.model.access" id="access_reporting_country_subdivision_time_series">
-      <field name="model" search="[('model', '=', 'sale.reporting.country.subdivision.time_series')]"/>
+      <field name="model">sale.reporting.country.subdivision.time_series</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_reporting_country_subdivision_time_series_sale">
-      <field name="model" search="[('model', '=', 'sale.reporting.country.subdivision.time_series')]"/>
+      <field name="model">sale.reporting.country.subdivision.time_series</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.action.wizard" id="wizard_reporting_country_tree_open">
```

### Comparing `trytond_sale-7.0.3/setup.py` & `trytond_sale-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/stock.py` & `trytond_sale-7.2.0/stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 
         return super(ShipmentOut, cls).draft(shipments)
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
     @process_sale('outgoing_moves')
-    def done(cls, shipments):
-        super(ShipmentOut, cls).done(shipments)
+    def do(cls, shipments):
+        super().do(shipments)
 
     @classmethod
     @ModelView.button
     @Workflow.transition('cancelled')
     @process_sale('outgoing_moves')
     def cancel(cls, shipments):
         super(ShipmentOut, cls).cancel(shipments)
```

### Comparing `trytond_sale-7.0.3/stock.xml` & `trytond_sale-7.2.0/stock.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_sale-7.0.3/stock.xml` & `trytond_sale-7.2.0/stock.xml`

```diff
@@ -6,15 +6,15 @@
     <record model="ir.ui.view" id="move_view_list_shipment">
       <field name="model">stock.move</field>
       <field name="type">tree</field>
       <field name="priority" eval="20"/>
       <field name="name">move_list_shipment</field>
     </record>
     <record model="ir.model.access" id="access_move_group_sale">
-      <field name="model" search="[('model', '=', 'stock.move')]"/>
+      <field name="model">stock.move</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.action.act_window" id="act_sale_move_relate">
@@ -34,23 +34,23 @@
     </record>
     <record model="ir.action.keyword" id="act_move_form_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">sale.sale,-1</field>
       <field name="action" ref="act_sale_move_relate"/>
     </record>
     <record model="ir.model.access" id="access_shipment_out_group_sale">
-      <field name="model" search="[('model', '=', 'stock.shipment.out')]"/>
+      <field name="model">stock.shipment.out</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_shipment_out_return_group_sale">
-      <field name="model" search="[('model', '=', 'stock.shipment.out.return')]"/>
+      <field name="model">stock.shipment.out.return</field>
       <field name="group" ref="group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_sale-7.0.3/tests/scenario_sale.rst` & `trytond_sale-7.2.0/tests/scenario_sale.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 =============
 Sale Scenario
 =============
 
 Imports::
 
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
+    >>> from proteus import Model, Report, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, create_tax, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, set_user
 
 Activate modules::
 
     >>> config = activate_modules('sale')
 
 Create company::
 
@@ -156,55 +155,47 @@
     >>> sale_line = SaleLine()
     >>> sale.lines.append(sale_line)
     >>> sale_line.product = product
     >>> sale_line.quantity = 3.0
     >>> sale.click('quote')
     >>> sale.untaxed_amount, sale.tax_amount, sale.total_amount
     (Decimal('50.00'), Decimal('5.00'), Decimal('55.00'))
-    >>> sale.quoted_by == employee
-    True
+    >>> assertEqual(sale.quoted_by, employee)
     >>> sale.click('confirm')
     >>> sale.untaxed_amount, sale.tax_amount, sale.total_amount
     (Decimal('50.00'), Decimal('5.00'), Decimal('55.00'))
-    >>> sale.confirmed_by == employee
-    True
+    >>> assertEqual(sale.confirmed_by, employee)
     >>> sale.state
     'processing'
     >>> sale.shipment_state
     'waiting'
     >>> sale.invoice_state
     'pending'
     >>> len(sale.shipments), len(sale.shipment_returns), len(sale.invoices)
     (1, 0, 1)
     >>> invoice, = sale.invoices
-    >>> invoice.origins == sale.rec_name
-    True
+    >>> assertEqual(invoice.origins, sale.rec_name)
     >>> shipment, = sale.shipments
-    >>> shipment.origins == sale.rec_name
-    True
+    >>> assertEqual(shipment.origins, sale.rec_name)
 
 Invoice line must be linked to stock move::
 
     >>> invoice_line1, invoice_line2 = sorted(
     ...     invoice.lines, key=lambda l: l.quantity or 0)
     >>> stock_move1, stock_move2 = sorted(shipment.outgoing_moves,
     ...     key=lambda m: m.quantity or 0)
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
 
-    >>> all(l.quantity == l.actual_quantity for l in sale.lines)
-    True
+    >>> for line in sale.lines:
+    ...     assertEqual(line.quantity, line.actual_quantity)
 
 Post invoice and check no new invoices::
 
 
     >>> for invoice in sale.invoices:
     ...     invoice.click('post')
     >>> sale.reload()
@@ -265,15 +256,15 @@
     0
 
 Validate Shipments::
 
     >>> shipment.click('assign_try')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
 
 Open customer invoice::
 
     >>> sale.reload()
     >>> sale.invoice_state
     'pending'
     >>> invoice, = sale.invoices
@@ -284,18 +275,16 @@
     >>> for line in invoice.lines:
     ...     line.quantity = 1
     ...     line.save()
     >>> invoice.click('post')
 
 Invoice lines must be linked to each stock moves::
 
-    >>> invoice_line1.stock_moves == [stock_move1]
-    True
-    >>> invoice_line2.stock_moves == [stock_move2]
-    True
+    >>> assertEqual(invoice_line1.stock_moves, [stock_move1])
+    >>> assertEqual(invoice_line2.stock_moves, [stock_move2])
 
 Check second invoices::
 
     >>> sale.reload()
     >>> len(sale.invoices)
     2
     >>> sum(l.quantity for i in sale.invoices for l in i.lines)
@@ -352,27 +341,26 @@
 
     >>> sale.reload()
     >>> shipment, = sale.shipments
     >>> shipment.reload()
     >>> stock_move, = shipment.outgoing_moves
     >>> stock_move.quantity
     4.0
-    >>> stock_move.invoice_lines == [invoice_line]
-    True
+    >>> assertEqual(stock_move.invoice_lines, [invoice_line])
 
 Ship 3 products::
 
     >>> stock_inventory_move, = shipment.inventory_moves
     >>> stock_inventory_move.quantity
     4.0
     >>> stock_inventory_move.quantity = 3.0
     >>> shipment.click('assign_try')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
 New shipments created::
 
     >>> sale.reload()
     >>> len(sale.shipments)
@@ -504,15 +492,15 @@
     >>> move_return.product.rec_name
     'product'
     >>> move_return.quantity
     2.0
     >>> mix_shipment.click('assign_try')
     >>> mix_shipment.click('pick')
     >>> mix_shipment.click('pack')
-    >>> mix_shipment.click('done')
+    >>> mix_shipment.click('do')
     >>> move_shipment, = mix_shipment.outgoing_moves
     >>> move_shipment.product.rec_name
     'product'
     >>> move_shipment.quantity
     7.0
 
 Checking the invoice::
@@ -630,16 +618,15 @@
     >>> sale_to_return.state
     'processing'
     >>> return_sale = Wizard('sale.return_sale', [sale_to_return])
     >>> return_sale.execute('return_')
     >>> returned_sale, = Sale.find([
     ...     ('state', '=', 'draft'),
     ...     ])
-    >>> returned_sale.origin == sale_to_return
-    True
+    >>> assertEqual(returned_sale.origin, sale_to_return)
     >>> sorted([x.quantity or 0 for x in returned_sale.lines])
     [-1.0, 0]
 
 Create a sale to be invoiced on shipment partialy and check correctly linked
 to invoices::
 
     >>> sale = Sale()
@@ -653,15 +640,15 @@
     >>> sale.click('confirm')
     >>> shipment, = sale.shipments
     >>> for move in shipment.inventory_moves:
     ...     move.quantity = 5.0
     >>> shipment.click('assign_try')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> sale.reload()
     >>> invoice, = sale.invoices
     >>> invoice_line, = invoice.lines
     >>> invoice_line.quantity
     5.0
     >>> stock_move, = invoice_line.stock_moves
     >>> stock_move.quantity
@@ -679,16 +666,15 @@
     >>> line = sale.lines.new()
     >>> line.product = product
     >>> line.quantity = 10.0
     >>> sale.click('quote')
     >>> sale.click('confirm')
     >>> invoice, = sale.invoices
     >>> invoice_line, = invoice.lines
-    >>> invoice_line.stock_moves == []
-    True
+    >>> assertEqual(invoice_line.stock_moves, [])
     >>> invoice_line.quantity = 5.0
     >>> invoice.click('post')
     >>> pay = invoice.click('pay')
     >>> pay.form.payment_method = payment_method
     >>> pay.execute('choice')
     >>> invoice.reload()
     >>> invoice.state
```

### Comparing `trytond_sale-7.0.3/tests/scenario_sale_default_methods.rst` & `trytond_sale-7.2.0/tests/scenario_sale_default_methods.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 =============================
 Sale Default Methods Scenario
 =============================
 
 Imports::
 
-    >>> from proteus import Model, Wizard, Report
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('sale')
 
 Create company::
```

### Comparing `trytond_sale-7.0.3/tests/scenario_sale_default_taxes.rst` & `trytond_sale-7.2.0/tests/scenario_sale_default_taxes.rst`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 =======================
 
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
 
     >>> config = activate_modules('sale')
 
     >>> Party = Model.get('party.party')
     >>> Sale = Model.get('sale.sale')
@@ -41,16 +41,15 @@
     >>> customer = Party(name="Customer")
     >>> customer.save()
 
 Create a sale without product::
 
     >>> sale = Sale(party=customer)
     >>> line = sale.lines.new()
-    >>> line.taxes == [tax]
-    True
+    >>> assertEqual(line.taxes, [tax])
     >>> line.quantity = 1
     >>> line.unit_price = Decimal('100.0000')
     >>> sale.click('quote')
     >>> sale.total_amount
     Decimal('110.00')
     >>> sale.click('confirm')
     >>> sale.state
@@ -58,9 +57,8 @@
 
 Check invoice::
 
     >>> invoice, = sale.invoices
     >>> invoice.total_amount
     Decimal('110.00')
     >>> line, = invoice.lines
-    >>> line.account == accounts['revenue']
-    True
+    >>> assertEqual(line.account, accounts['revenue'])
```

### Comparing `trytond_sale-7.0.3/tests/scenario_sale_empty.rst` & `trytond_sale-7.2.0/tests/scenario_sale_empty.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 ===================
 Sale Empty Scenario
 ===================
 
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
 
     >>> config = activate_modules('sale')
 
 Create company::
```

### Comparing `trytond_sale-7.0.3/tests/scenario_sale_manual_invoice.rst` & `trytond_sale-7.2.0/tests/scenario_sale_manual_invoice.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 ============================
 
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
 
     >>> config = activate_modules('sale')
 
     >>> Party = Model.get('party.party')
     >>> ProductCategory = Model.get('product.category')
```

### Comparing `trytond_sale-7.0.3/tests/scenario_sale_manual_shipment.rst` & `trytond_sale-7.2.0/tests/scenario_sale_manual_shipment.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 =============================
 
 Imports::
 
     >>> from decimal import Decimal
 
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('sale')
 
     >>> Party = Model.get('party.party')
     >>> ProductCategory = Model.get('product.category')
```

### Comparing `trytond_sale-7.0.3/tests/scenario_sale_modify_header.rst` & `trytond_sale-7.2.0/tests/scenario_sale_modify_header.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ===========================
 Sale Modify Header Scenario
 ===========================
 
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
 
     >>> config = activate_modules('sale')
 
 Create company::
 
@@ -86,16 +86,15 @@
     >>> sale.save()
     >>> sale.untaxed_amount, sale.tax_amount, sale.total_amount
     (Decimal('30.00'), Decimal('3.00'), Decimal('33.00'))
 
 Change the party::
 
     >>> modify_header = sale.click('modify_header')
-    >>> modify_header.form.party == customer
-    True
+    >>> assertEqual(modify_header.form.party, customer)
     >>> modify_header.form.party = another
     >>> modify_header.execute('modify')
 
     >>> sale.party.name
     'Another Customer'
     >>> sale.untaxed_amount, sale.tax_amount, sale.total_amount
     (Decimal('30.00'), Decimal('1.50'), Decimal('31.50'))
```

### Comparing `trytond_sale-7.0.3/tests/scenario_sale_reporting.rst` & `trytond_sale-7.2.0/tests/scenario_sale_reporting.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 =======================
 Sale Reporting Scenario
 =======================
 
 Imports::
 
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
+
+    >>> from dateutil.relativedelta import relativedelta
+
     >>> from proteus import Model
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
 
     >>> config = activate_modules('sale')
 
 Create company::
 
@@ -53,17 +54,19 @@
     >>> new_york.save()
 
 Create party categories::
 
     >>> PartyCategory = Model.get('party.category')
     >>> party_category_root1 = PartyCategory(name="Root1")
     >>> party_category_root1.save()
-    >>> party_category_child1 = PartyCategory(name="Child1", parent=party_category_root1)
+    >>> party_category_child1 = PartyCategory(
+    ...     name="Child1", parent=party_category_root1)
     >>> party_category_child1.save()
-    >>> party_category_child2 = PartyCategory(name="Child2", parent=party_category_root1)
+    >>> party_category_child2 = PartyCategory(
+    ...     name="Child2", parent=party_category_root1)
     >>> party_category_child2.save()
     >>> party_category_root2 = PartyCategory(name="Root2")
     >>> party_category_root2.save()
 
 Create parties::
 
     >>> Party = Model.get('party.party')
@@ -160,133 +163,128 @@
     ...         period='month')
     >>> with config.set_context(context=context):
     ...     reports = Customer.find([])
     ...     time_series = CustomerTimeseries.find([])
     >>> len(reports)
     2
     >>> with config.set_context(context=context):
-    ...     sorted((r.customer.id, r.number, r.revenue) for r in reports) == \
-    ...     sorted([(customer1.id, 1, Decimal('30')),
-    ...             (customer2.id, 1, Decimal('10'))])
-    True
+    ...     assertEqual({(r.customer.id, r.number, r.revenue) for r in reports},
+    ...         {(customer1.id, 1, Decimal('30')),
+    ...             (customer2.id, 1, Decimal('10'))})
     >>> len(time_series)
     2
     >>> with config.set_context(context=context):
-    ...     sorted((r.customer.id, r.date, r.number, r.revenue)
-    ...         for r in time_series) == sorted(
-    ...     [(customer1.id, sale1.sale_date.replace(day=1), 1, Decimal('30')),
-    ...     (customer2.id, sale2.sale_date.replace(day=1), 1, Decimal('10'))])
-    True
+    ...     assertEqual({(r.customer.id, r.date, r.number, r.revenue)
+    ...             for r in time_series},
+    ...         {(customer1.id, sale1.sale_date.replace(day=1), 1, Decimal('30')),
+    ...         (customer2.id, sale2.sale_date.replace(day=1), 1, Decimal('10'))})
 
 Check sale reporting per customer categories::
 
     >>> CustomerCategory = Model.get('sale.reporting.customer.category')
     >>> CustomerCategoryTimeseries = Model.get(
     ...     'sale.reporting.customer.category.time_series')
     >>> CustomerCategoryTree = Model.get('sale.reporting.customer.category.tree')
     >>> with config.set_context(context=context):
     ...     reports = CustomerCategory.find([])
     ...     time_series = CustomerCategoryTimeseries.find([])
     ...     tree = CustomerCategoryTree.find([])
     >>> len(reports)
     3
     >>> with config.set_context(context=context):
-    ...     sorted((r.category.id, r.number, r.revenue) for r in reports) == \
-    ...     sorted([(party_category_child1.id, 1, Decimal('30')),
+    ...     assertEqual({(r.category.id, r.number, r.revenue) for r in reports},
+    ...     {(party_category_child1.id, 1, Decimal('30')),
     ...         (party_category_root2.id, 1, Decimal('30')),
-    ...         (party_category_child2.id, 1, Decimal('10'))])
-    True
+    ...         (party_category_child2.id, 1, Decimal('10'))})
     >>> len(time_series)
     3
     >>> with config.set_context(context=context):
-    ...     sorted((r.category.id, r.date, r.number, r.revenue)
-    ...         for r in time_series) == sorted(
-    ...     [(party_category_child1.id, sale1.sale_date.replace(day=1), 1, Decimal('30')),
-    ...     (party_category_root2.id, sale1.sale_date.replace(day=1), 1, Decimal('30')),
-    ...     (party_category_child2.id, sale2.sale_date.replace(day=1), 1, Decimal('10'))])
-    True
+    ...     assertEqual({
+    ...             (r.category.id, r.date, r.number, r.revenue)
+    ...             for r in time_series},
+    ...         {
+    ...             (party_category_child1.id, sale1.sale_date.replace(day=1),
+    ...                 1, Decimal('30')),
+    ...             (party_category_root2.id, sale1.sale_date.replace(day=1),
+    ...                 1, Decimal('30')),
+    ...             (party_category_child2.id, sale2.sale_date.replace(day=1),
+    ...                 1, Decimal('10'))})
     >>> len(tree)
     4
     >>> with config.set_context(context=context):
-    ...     sorted((r.name, r.revenue) for r in tree) == sorted([
-    ...         ('Root1', Decimal('40')),
+    ...     assertEqual({(r.name, r.revenue) for r in tree},
+    ...         {('Root1', Decimal('40')),
     ...         ('Child1', Decimal('30')),
     ...         ('Child2', Decimal('10')),
-    ...         ('Root2', Decimal('30'))])
-    True
+    ...         ('Root2', Decimal('30'))})
     >>> child1, = CustomerCategoryTree.find([('rec_name', '=', 'Child1')])
     >>> child1.rec_name
     'Child1'
 
 Check sale reporting per product::
 
     >>> Product = Model.get('sale.reporting.product')
     >>> ProductTimeseries = Model.get('sale.reporting.product.time_series')
     >>> with config.set_context(context=context):
     ...     reports = Product.find([])
     ...     time_series = ProductTimeseries.find([])
     >>> len(reports)
     2
     >>> with config.set_context(context=context):
-    ...     sorted((r.product.id, r.number, r.revenue) for r in reports) == \
-    ...     sorted([(product1.id, 2, Decimal('30')),
-    ...         (product2.id, 1, Decimal('10'))])
-    True
+    ...     assertEqual({(r.product.id, r.number, r.revenue) for r in reports},
+    ...     {(product1.id, 2, Decimal('30')),
+    ...         (product2.id, 1, Decimal('10'))})
     >>> len(time_series)
     3
     >>> with config.set_context(context=context):
-    ...     sorted((r.product.id, r.date, r.number, r.revenue)
-    ...         for r in time_series) == sorted(
-    ...     [(product1.id, sale1.sale_date.replace(day=1), 1, Decimal('20')),
+    ...     assertEqual({(r.product.id, r.date, r.number, r.revenue)
+    ...         for r in time_series},
+    ...     {(product1.id, sale1.sale_date.replace(day=1), 1, Decimal('20')),
     ...     (product2.id, sale1.sale_date.replace(day=1), 1, Decimal('10')),
-    ...     (product1.id, sale2.sale_date.replace(day=1), 1, Decimal('10'))])
-    True
+    ...     (product1.id, sale2.sale_date.replace(day=1), 1, Decimal('10'))})
 
 Check sale reporting per product categories::
 
     >>> ProductCategory = Model.get('sale.reporting.product.category')
     >>> ProductCategoryTimeseries = Model.get(
     ...     'sale.reporting.product.category.time_series')
     >>> ProductCategoryTree = Model.get('sale.reporting.product.category.tree')
     >>> with config.set_context(context=context):
     ...     reports = ProductCategory.find([])
     ...     time_series = ProductCategoryTimeseries.find([])
     ...     tree = ProductCategoryTree.find([])
     >>> len(reports)
     4
     >>> with config.set_context(context=context):
-    ...     sorted((r.category.id, r.number, r.revenue) for r in reports) == \
-    ...     sorted([(category_child1.id, 2, Decimal('30')),
+    ...     assertEqual({(r.category.id, r.number, r.revenue) for r in reports},
+    ...     {(category_child1.id, 2, Decimal('30')),
     ...         (category_root2.id, 2, Decimal('30')),
     ...         (category_child2.id, 1, Decimal('10')),
-    ...         (account_category.id, 2, Decimal('40'))])
-    True
+    ...         (account_category.id, 2, Decimal('40'))})
     >>> len(time_series)
     7
     >>> with config.set_context(context=context):
-    ...     sorted((r.category.id, r.date, r.number, r.revenue)
-    ...         for r in time_series) == sorted(
-    ...     [(category_child1.id, sale1.sale_date.replace(day=1), 1, Decimal('20')),
+    ...     assertEqual({(r.category.id, r.date, r.number, r.revenue)
+    ...         for r in time_series},
+    ...     {(category_child1.id, sale1.sale_date.replace(day=1), 1, Decimal('20')),
     ...     (category_root2.id, sale1.sale_date.replace(day=1), 1, Decimal('20')),
     ...     (category_child2.id, sale1.sale_date.replace(day=1), 1, Decimal('10')),
     ...     (category_child1.id, sale2.sale_date.replace(day=1), 1, Decimal('10')),
     ...     (category_root2.id, sale2.sale_date.replace(day=1), 1, Decimal('10')),
     ...     (account_category.id, sale1.sale_date.replace(day=1), 1, Decimal('30')),
-    ...     (account_category.id, sale2.sale_date.replace(day=1), 1, Decimal('10'))])
-    True
+    ...     (account_category.id, sale2.sale_date.replace(day=1), 1, Decimal('10'))})
     >>> len(tree)
     5
     >>> with config.set_context(context=context):
-    ...     sorted((r.name, r.revenue) for r in tree) == sorted([
-    ...         ('Root1', Decimal('40')),
+    ...     assertEqual({(r.name, r.revenue) for r in tree},
+    ...         {('Root1', Decimal('40')),
     ...         ('Child1', Decimal('30')),
     ...         ('Child2', Decimal('10')),
     ...         ('Root2', Decimal('30')),
-    ...         ('Account Category', Decimal('40'))])
-    True
+    ...         ('Account Category', Decimal('40'))})
     >>> child1, = ProductCategoryTree.find([('rec_name', '=', 'Child1')])
     >>> child1.rec_name
     'Child1'
 
 Check sale reporting per countries::
 
     >>> RegionTree = Model.get('sale.reporting.region.tree')
@@ -295,35 +293,30 @@
     >>> SubdivisionTimeseries = Model.get(
     ...     'sale.reporting.country.subdivision.time_series')
     >>> with config.set_context(context=context):
     ...     region = RegionTree(north_america.id)
     ...     countries = CountryTree.find([])
     ...     country_time_series = CountryTimeseries.find([])
     ...     subdivision_time_series = SubdivisionTimeseries.find([])
-    >>> region.revenue == Decimal('40')
-    True
-    >>> region.parent.revenue == Decimal('40')
-    True
+    >>> region.revenue
+    Decimal('40.00')
+    >>> region.parent.revenue
+    Decimal('40.00')
     >>> len(countries)
     3
     >>> with config.set_context(context=context):
-    ...     sorted((c.region, c.number, c.revenue) for c in countries) == \
-    ...     sorted([('United States', 2, Decimal('40')),
-    ...         ('California', 1, Decimal('30')),
-    ...         ('New York', 1, Decimal('10'))])
-    True
+    ...     sorted((c.region, c.number, c.revenue) for c in countries)
+    [('California', 1, Decimal('30.00')), ('New York', 1, Decimal('10.00')), ('United States', 2, Decimal('40.00'))]
     >>> len(country_time_series)
     2
     >>> with config.set_context(context=context):
-    ...     sorted((r.country.id, r.date, r.number, r.revenue)
-    ...         for r in country_time_series) == sorted(
-    ...     [(country_us.id, sale1.sale_date.replace(day=1), 1, Decimal('30')),
-    ...     (country_us.id, sale2.sale_date.replace(day=1), 1, Decimal('10'))])
-    True
+    ...     assertEqual({(r.country.id, r.date, r.number, r.revenue)
+    ...         for r in country_time_series},
+    ...     {(country_us.id, sale1.sale_date.replace(day=1), 1, Decimal('30')),
+    ...     (country_us.id, sale2.sale_date.replace(day=1), 1, Decimal('10'))})
     >>> len(subdivision_time_series)
     2
     >>> with config.set_context(context=context):
-    ...     sorted((r.subdivision.id, r.date, r.number, r.revenue)
-    ...         for r in subdivision_time_series) == sorted(
-    ...     [(california.id, sale1.sale_date.replace(day=1), 1, Decimal('30')),
-    ...     (new_york.id, sale2.sale_date.replace(day=1), 1, Decimal('10'))])
-    True
+    ...     assertEqual({(r.subdivision.id, r.date, r.number, r.revenue)
+    ...         for r in subdivision_time_series},
+    ...     {(california.id, sale1.sale_date.replace(day=1), 1, Decimal('30')),
+    ...     (new_york.id, sale2.sale_date.replace(day=1), 1, Decimal('10'))})
```

### Comparing `trytond_sale-7.0.3/tests/test_module.py` & `trytond_sale-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/tox.ini` & `trytond_sale-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/trytond_sale.egg-info/PKG-INFO` & `trytond_sale-7.2.0/trytond_sale.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale
-Version: 7.0.3
+Version: 7.2.0
 Summary: Tryton module for sale
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/modules-sale/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -50,29 +50,29 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
 Requires-Dist: python-dateutil
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_country<7.1,>=7.0
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
+Requires-Dist: trytond_country<7.3,>=7.2
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
 
 ###########
 Sale Module
 ###########
 
 The *Sale Module* helps organise and manage sales made by the company.
 It adds the concept of a sale to Tryton and allows it to be tracked through
```

### Comparing `trytond_sale-7.0.3/trytond_sale.egg-info/SOURCES.txt` & `trytond_sale-7.2.0/trytond_sale.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -69,14 +69,17 @@
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_sale.rst
 ./tests/scenario_sale_default_methods.rst
 ./tests/scenario_sale_default_taxes.rst
 ./tests/scenario_sale_empty.rst
+./tests/scenario_sale_line_cancelled.rst
+./tests/scenario_sale_line_cancelled_on_invoice.rst
+./tests/scenario_sale_line_cancelled_on_shipment.rst
 ./tests/scenario_sale_manual_invoice.rst
 ./tests/scenario_sale_manual_shipment.rst
 ./tests/scenario_sale_modify_header.rst
 ./tests/scenario_sale_reporting.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/configuration_form.xml
@@ -117,18 +120,18 @@
 ./view/template_tree.xml
 doc/conf.py
 doc/design.rst
 doc/index.rst
 doc/releases.rst
 doc/requirements-doc.txt
 doc/usage/index.rst
-doc/usage/presales.rst
-doc/usage/process.rst
-doc/usage/reporting.rst
-doc/usage/returns.rst
+doc/usage/presales.inc.rst
+doc/usage/process.inc.rst
+doc/usage/reporting.inc.rst
+doc/usage/returns.inc.rst
 icons/LICENSE
 icons/tryton-sale.svg
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
 locale/es.po
@@ -152,14 +155,17 @@
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_sale.rst
 tests/scenario_sale_default_methods.rst
 tests/scenario_sale_default_taxes.rst
 tests/scenario_sale_empty.rst
+tests/scenario_sale_line_cancelled.rst
+tests/scenario_sale_line_cancelled_on_invoice.rst
+tests/scenario_sale_line_cancelled_on_shipment.rst
 tests/scenario_sale_manual_invoice.rst
 tests/scenario_sale_manual_shipment.rst
 tests/scenario_sale_modify_header.rst
 tests/scenario_sale_reporting.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_sale.egg-info/PKG-INFO
```

### Comparing `trytond_sale-7.0.3/view/configuration_form.xml` & `trytond_sale-7.2.0/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/view/party_form.xml` & `trytond_sale-7.2.0/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/view/product_list_sale_line.xml` & `trytond_sale-7.2.0/view/product_list_sale_line.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/view/product_sale_context_form.xml` & `trytond_sale-7.2.0/view/product_sale_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/view/sale_form.xml` & `trytond_sale-7.2.0/view/sale_form.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_sale-7.0.3/view/sale_form.xml` & `trytond_sale-7.2.0/view/sale_form.xml`

```diff
@@ -63,14 +63,17 @@
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
     <link icon="tryton-shipment-out" name="sale.act_shipment_form"/>
     <link icon="tryton-account" name="sale.act_invoice_form"/>
     <link icon="tryton-shipment-in" name="sale.act_return_form"/>
   </group>
   <group col="-1" colspan="3" id="buttons">
```

### Comparing `trytond_sale-7.0.3/view/sale_line_form.xml` & `trytond_sale-7.2.0/view/sale_line_form.xml`

 * *Files 5% similar despite different names*

#### Comparing `trytond_sale-7.0.3/view/sale_line_form.xml` & `trytond_sale-7.2.0/view/sale_line_form.xml`

```diff
@@ -27,14 +27,15 @@
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

### Comparing `trytond_sale-7.0.3/view/sale_line_tree.xml` & `trytond_sale-7.2.0/view/sale_line_tree.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_sale-7.0.3/view/sale_line_tree.xml` & `trytond_sale-7.2.0/view/sale_line_tree.xml`

```diff
@@ -8,9 +8,11 @@
   <field name="type" optional="1"/>
   <field name="product" expand="1" optional="0"/>
   <field name="summary" expand="1" optional="1"/>
   <field name="actual_quantity" symbol="unit" optional="0"/>
   <field name="quantity" symbol="unit" optional="0"/>
   <field name="unit_price"/>
   <field name="amount"/>
+  <field name="moves_progress" string="Shipping" widget="progressbar" optional="1"/>
+  <field name="invoice_progress" string="Invoicing" widget="progressbar" optional="1"/>
   <field name="sale_state"/>
 </tree>
```

### Comparing `trytond_sale-7.0.3/view/sale_line_tree_sequence.xml` & `trytond_sale-7.2.0/view/sale_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/view/sale_reporting_context_form.xml` & `trytond_sale-7.2.0/view/sale_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/view/sale_reporting_customer_category_list.xml` & `trytond_sale-7.2.0/view/sale_reporting_customer_category_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/view/sale_reporting_product_category_list.xml` & `trytond_sale-7.2.0/view/sale_reporting_product_category_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/view/sale_tree.xml` & `trytond_sale-7.2.0/view/sale_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.0.3/view/template_form.xml` & `trytond_sale-7.2.0/view/template_form.xml`

 * *Files identical despite different names*

