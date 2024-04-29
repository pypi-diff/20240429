# Comparing `tmp/trytond_account_stock_eu-7.0.0.tar.gz` & `tmp/trytond_account_stock_eu-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_stock_eu-7.0.0.tar", last modified: Mon Oct 30 17:25:18 2023, max compression
+gzip compressed data, was "trytond_account_stock_eu-7.2.0.tar", last modified: Mon Apr 29 15:36:38 2024, max compression
```

## Comparing `trytond_account_stock_eu-7.0.0.tar` & `trytond_account_stock_eu-7.2.0.tar`

### file list

```diff
@@ -1,93 +1,92 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:18.324136 trytond_account_stock_eu-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-10-22 17:22:57.000000 trytond_account_stock_eu-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-30 17:03:49.000000 trytond_account_stock_eu-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:03:49.000000 trytond_account_stock_eu-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3325 2023-10-30 17:25:18.320802 trytond_account_stock_eu-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      270 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2119 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      416 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    19525 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/account_stock_eu.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21023 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/account_stock_eu.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)      485 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/carrier.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      968 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1838 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/country.py
--rw-r--r--   0 ced       (1000) ced       (1000)      784 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/country.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/customs.py
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/customs.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:18.317469 trytond_account_stock_eu-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2817 2023-10-22 17:22:57.000000 trytond_account_stock_eu-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2951 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      270 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:57.000000 trytond_account_stock_eu-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      704 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:18.314136 trytond_account_stock_eu-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20067 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20753 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20327 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    20322 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19903 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18290 2023-10-30 16:47:45.000000 trytond_account_stock_eu-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15780 2023-10-28 12:11:20.000000 trytond_account_stock_eu-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:25:18.324136 trytond_account_stock_eu-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4779 2023-10-27 17:38:49.000000 trytond_account_stock_eu-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26402 2023-10-07 17:14:58.000000 trytond_account_stock_eu-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10052 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:18.314136 trytond_account_stock_eu-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9932 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/tests/scenario_account_stock_eu_arrival.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    10227 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/tests/scenario_account_stock_eu_dispatch.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      391 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_stock_eu-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-10-30 17:03:46.000000 trytond_account_stock_eu-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:18.320802 trytond_account_stock_eu-7.0.0/trytond_account_stock_eu.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3325 2023-10-30 17:25:17.000000 trytond_account_stock_eu-7.0.0/trytond_account_stock_eu.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3295 2023-10-30 17:25:18.000000 trytond_account_stock_eu-7.0.0/trytond_account_stock_eu.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:25:17.000000 trytond_account_stock_eu-7.0.0/trytond_account_stock_eu.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2023-10-30 17:25:17.000000 trytond_account_stock_eu-7.0.0/trytond_account_stock_eu.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:01:16.000000 trytond_account_stock_eu-7.0.0/trytond_account_stock_eu.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-10-30 17:25:17.000000 trytond_account_stock_eu-7.0.0/trytond_account_stock_eu.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:25:17.000000 trytond_account_stock_eu-7.0.0/trytond_account_stock_eu.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:18.317469 trytond_account_stock_eu-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/account_fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/country_subdivision_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/country_subdivision_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/customs_tariff_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/intrastat_declaration_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/intrastat_declaration_export_result_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      510 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/intrastat_declaration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      541 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/intrastat_declaration_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/intrastat_declaration_line_list_incoterm.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      387 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/intrastat_declaration_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/intrastat_transaction_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/intrastat_transaction_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/intrastat_transport_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/intrastat_transport_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1581 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/stock_move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      490 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/stock_move_form_incoterm.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-08-13 15:26:13.000000 trytond_account_stock_eu-7.0.0/view/stock_shipment_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:38.855375 trytond_account_stock_eu-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2024-04-29 15:16:40.000000 trytond_account_stock_eu-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:16:40.000000 trytond_account_stock_eu-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3316 2024-04-29 15:36:38.855375 trytond_account_stock_eu-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      270 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2119 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      416 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    19525 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/account_stock_eu.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20839 2024-04-27 16:30:39.000000 trytond_account_stock_eu-7.2.0/account_stock_eu.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      485 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/carrier.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      970 2024-04-27 16:30:39.000000 trytond_account_stock_eu-7.2.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1838 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/country.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      784 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/country.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/customs.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/customs.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:38.848709 trytond_account_stock_eu-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_account_stock_eu-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2951 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      270 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:01.000000 trytond_account_stock_eu-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      704 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:38.852042 trytond_account_stock_eu-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20067 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20753 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20327 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    20322 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19903 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:21.000000 trytond_account_stock_eu-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:22.000000 trytond_account_stock_eu-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:22.000000 trytond_account_stock_eu-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18290 2024-04-27 16:43:22.000000 trytond_account_stock_eu-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:22.000000 trytond_account_stock_eu-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:22.000000 trytond_account_stock_eu-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15780 2024-04-27 16:43:22.000000 trytond_account_stock_eu-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:36:38.855375 trytond_account_stock_eu-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4770 2024-04-27 16:30:39.000000 trytond_account_stock_eu-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26402 2024-02-04 18:51:26.000000 trytond_account_stock_eu-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9898 2024-04-27 16:30:39.000000 trytond_account_stock_eu-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:38.852042 trytond_account_stock_eu-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9933 2024-04-27 16:30:39.000000 trytond_account_stock_eu-7.2.0/tests/scenario_account_stock_eu_arrival.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    10228 2024-04-27 16:30:39.000000 trytond_account_stock_eu-7.2.0/tests/scenario_account_stock_eu_dispatch.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      391 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:01.000000 trytond_account_stock_eu-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2024-04-29 15:16:34.000000 trytond_account_stock_eu-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:38.855375 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3316 2024-04-29 15:36:38.000000 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3277 2024-04-29 15:36:38.000000 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:36:38.000000 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:36:38.000000 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 12:01:16.000000 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2024-04-29 15:36:38.000000 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:36:38.000000 trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:38.855375 trytond_account_stock_eu-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      410 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/account_fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/country_subdivision_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/country_subdivision_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/customs_tariff_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_declaration_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_declaration_export_result_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      510 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_declaration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      541 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_declaration_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_declaration_line_list_incoterm.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      387 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_declaration_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_transaction_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_transaction_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_transport_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/intrastat_transport_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1581 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/stock_move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      490 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/stock_move_form_incoterm.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      512 2024-01-27 09:58:52.000000 trytond_account_stock_eu-7.2.0/view/stock_shipment_form.xml
```

### Comparing `trytond_account_stock_eu-7.0.0/COPYRIGHT` & `trytond_account_stock_eu-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2022-2023 B2CK
-Copyright (C) 2022-2023 Cédric Krier
+Copyright (C) 2022-2024 B2CK
+Copyright (C) 2022-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_stock_eu-7.0.0/LICENSE` & `trytond_account_stock_eu-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/PKG-INFO` & `trytond_account_stock_eu-7.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_eu
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for european stock accounting
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: bugs@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-stock-eu
+Project-URL: Documentation, https://docs.tryton.org/modules-account-stock-eu
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account stock europe intrastat
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,30 +49,30 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_country<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_customs<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_product_measurements<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_measurements<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_country<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_customs<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_product_measurements<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_measurements<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_carrier<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_incoterm<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_consignment<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_carrier<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_incoterm<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_consignment<7.3,>=7.2; extra == "test"
 
 #######################
 Account Stock EU Module
 #######################
 
 The *Account Stock EU Module* is used to generate the `Intrastat
 <https://en.wikipedia.org/wiki/Intrastat>`_ declarations every month.
```

### Comparing `trytond_account_stock_eu-7.0.0/__init__.py` & `trytond_account_stock_eu-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/account_stock_eu.py` & `trytond_account_stock_eu-7.2.0/account_stock_eu.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/account_stock_eu.xml` & `trytond_account_stock_eu-7.2.0/account_stock_eu.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_account_stock_eu-7.0.0/account_stock_eu.xml` & `trytond_account_stock_eu-7.2.0/account_stock_eu.xml`

```diff
@@ -10,15 +10,15 @@
     </record>
     <record model="ir.ui.view" id="intrastat_transaction_view_list">
       <field name="model">account.stock.eu.intrastat.transaction</field>
       <field name="type">tree</field>
       <field name="name">intrastat_transaction_list</field>
     </record>
     <record model="ir.model.access" id="access_intrastat_transaction">
-      <field name="model" search="[('model', '=', 'account.stock.eu.intrastat.transaction')]"/>
+      <field name="model">account.stock.eu.intrastat.transaction</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="intrastat_transport_view_form">
       <field name="model">account.stock.eu.intrastat.transport</field>
@@ -27,15 +27,15 @@
     </record>
     <record model="ir.ui.view" id="intrastat_transport_view_list">
       <field name="model">account.stock.eu.intrastat.transport</field>
       <field name="type">tree</field>
       <field name="name">intrastat_transport_list</field>
     </record>
     <record model="ir.model.access" id="access_intrastat_transport">
-      <field name="model" search="[('model', '=', 'account.stock.eu.intrastat.transport')]"/>
+      <field name="model">account.stock.eu.intrastat.transport</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.ui.view" id="intrastat_declaration_view_form">
       <field name="model">account.stock.eu.intrastat.declaration</field>
@@ -72,36 +72,36 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_intrastat_declaration_form"/>
     </record>
     <menuitem parent="account.menu_processing" action="act_intrastat_declaration_form" sequence="50" id="menu_intrastat_declaration"/>
     <record model="ir.model.button" id="intrastat_declaration_export_button">
+      <field name="model">account.stock.eu.intrastat.declaration</field>
       <field name="name">export</field>
       <field name="string">Export</field>
-      <field name="model" search="[('model', '=', 'account.stock.eu.intrastat.declaration')]"/>
     </record>
     <record model="ir.model.access" id="access_intrastat_declaration">
-      <field name="model" search="[('model', '=', 'account.stock.eu.intrastat.declaration')]"/>
+      <field name="model">account.stock.eu.intrastat.declaration</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_intrastat_declaration_account">
-      <field name="model" search="[('model', '=', 'account.stock.eu.intrastat.declaration')]"/>
+      <field name="model">account.stock.eu.intrastat.declaration</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.rule.group" id="rule_group_intrastat_declaration_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.stock.eu.intrastat.declaration')]"/>
+      <field name="model">account.stock.eu.intrastat.declaration</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_intrastat_declaration_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_intrastat_declaration_companies"/>
     </record>
     <record model="ir.ui.view" id="intrastat_declaration_context_view_form">
@@ -111,22 +111,22 @@
     </record>
     <record model="ir.ui.view" id="intrastat_declaration_line_view_list">
       <field name="model">account.stock.eu.intrastat.declaration.line</field>
       <field name="type">tree</field>
       <field name="name">intrastat_declaration_line_list</field>
     </record>
     <record model="ir.model.access" id="access_intrastat_declaration_line">
-      <field name="model" search="[('model', '=', 'account.stock.eu.intrastat.declaration.line')]"/>
+      <field name="model">account.stock.eu.intrastat.declaration.line</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_intrastat_declaration_line_account">
-      <field name="model" search="[('model', '=', 'account.stock.eu.intrastat.declaration.line')]"/>
+      <field name="model">account.stock.eu.intrastat.declaration.line</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.action.act_window" id="act_intrastat_declaration_line_form">
```

### Comparing `trytond_account_stock_eu-7.0.0/company.py` & `trytond_account_stock_eu-7.2.0/company.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,11 +20,11 @@
         currencies = {}
         eur = None
         for company in companies:
             if company.currency.code == 'EUR':
                 currency = company.currency
             else:
                 if not eur:
-                    eur, = Currency.find([('code', '=', 'EUR')], limit=1)
+                    eur, = Currency.search([('code', '=', 'EUR')], limit=1)
                 currency = eur
             currencies[company.id] = currency
         return currencies
```

### Comparing `trytond_account_stock_eu-7.0.0/country.py` & `trytond_account_stock_eu-7.2.0/country.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/country.xml` & `trytond_account_stock_eu-7.2.0/country.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/doc/conf.py` & `trytond_account_stock_eu-7.2.0/doc/conf.py`

 * *Files 5% similar despite different names*

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

### Comparing `trytond_account_stock_eu-7.0.0/doc/design.rst` & `trytond_account_stock_eu-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/doc/usage.rst` & `trytond_account_stock_eu-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/bg.po` & `trytond_account_stock_eu-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/ca.po` & `trytond_account_stock_eu-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/cs.po` & `trytond_account_stock_eu-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/de.po` & `trytond_account_stock_eu-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/es.po` & `trytond_account_stock_eu-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/es_419.po` & `trytond_account_stock_eu-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/et.po` & `trytond_account_stock_eu-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/fa.po` & `trytond_account_stock_eu-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/fi.po` & `trytond_account_stock_eu-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/fr.po` & `trytond_account_stock_eu-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/hu.po` & `trytond_account_stock_eu-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/id.po` & `trytond_account_stock_eu-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/it.po` & `trytond_account_stock_eu-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/lo.po` & `trytond_account_stock_eu-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/lt.po` & `trytond_account_stock_eu-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/nl.po` & `trytond_account_stock_eu-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/pl.po` & `trytond_account_stock_eu-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/pt.po` & `trytond_account_stock_eu-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/ro.po` & `trytond_account_stock_eu-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/ru.po` & `trytond_account_stock_eu-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/sl.po` & `trytond_account_stock_eu-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/tr.po` & `trytond_account_stock_eu-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/uk.po` & `trytond_account_stock_eu-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/locale/zh_CN.po` & `trytond_account_stock_eu-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/message.xml` & `trytond_account_stock_eu-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/setup.py` & `trytond_account_stock_eu-7.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     author='Tryton',
     author_email='bugs@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-account-stock-eu'),
+            'https://docs.tryton.org/modules-account-stock-eu'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account stock europe intrastat',
     package_dir={'trytond.modules.account_stock_eu': '.'},
     packages=(
         ['trytond.modules.account_stock_eu']
```

### Comparing `trytond_account_stock_eu-7.0.0/stock.py` & `trytond_account_stock_eu-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/stock.xml` & `trytond_account_stock_eu-7.2.0/stock.xml`

 * *Files 23% similar despite different names*

#### Comparing `trytond_account_stock_eu-7.0.0/stock.xml` & `trytond_account_stock_eu-7.2.0/stock.xml`

```diff
@@ -5,138 +5,160 @@
   <data>
     <record model="ir.ui.view" id="stock_move_view_form">
       <field name="model">stock.move</field>
       <field name="inherit" ref="stock.move_view_form"/>
       <field name="name">stock_move_form</field>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_type">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_type')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_type</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_type_account">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_type')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_type</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_warehouse_country">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_warehouse_country')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_warehouse_country</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_warehouse_country_account">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_warehouse_country')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_warehouse_country</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_country">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_country')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_country</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_country_account">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_country')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_country</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_subdivision">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_subdivision')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_subdivision</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_subdivision_account">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_subdivision')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_subdivision</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_tariff_code">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_tariff_code')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_tariff_code</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_tariff_code_account">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_tariff_code')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_tariff_code</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_transaction">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_transaction')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_transaction</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_transaction_account">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_transaction')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_transaction</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_additional_unit">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_additional_unit')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_additional_unit</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_additional_unit_account">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_additional_unit')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_additional_unit</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_country_of_origin">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_country_of_origin')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_country_of_origin</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_country_of_origin_account">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_country_of_origin')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_country_of_origin</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_vat">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_vat')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_vat</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_vat_account">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_vat')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_vat</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
   </data>
   <data depends="incoterm">
     <record model="ir.ui.view" id="stock_move_view_form_incoterm">
       <field name="model">stock.move</field>
       <field name="inherit" ref="stock.move_view_form"/>
       <field name="priority" eval="20"/>
       <field name="name">stock_move_form_incoterm</field>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_transport">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_transport')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_transport</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_transport_account">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_transport')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_transport</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_incoterm">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_incoterm')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_incoterm</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="account_stock_move_intrastat_incoterm_account">
-      <field name="field" search="[('model.model', '=', 'stock.move'), ('name', '=', 'intrastat_incoterm')]"/>
+      <field name="model">stock.move</field>
+      <field name="field">intrastat_incoterm</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
   </data>
   <data>
     <record model="ir.ui.view" id="stock_shipment_in_view_form">
```

### Comparing `trytond_account_stock_eu-7.0.0/tests/scenario_account_stock_eu_arrival.rst` & `trytond_account_stock_eu-7.2.0/tests/scenario_account_stock_eu_arrival.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
     >>> import datetime as dt
     >>> import io
     >>> import zipfile
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_stock_eu')
 
     >>> Country = Model.get('country.country')
     >>> IntrastatDeclaration = Model.get('account.stock.eu.intrastat.declaration')
-    >>> IntrastatDeclarationLine = Model.get('account.stock.eu.intrastat.declaration.line')
+    >>> IntrastatDeclarationLine = Model.get(
+    ...     'account.stock.eu.intrastat.declaration.line')
     >>> Organization = Model.get('country.organization')
     >>> Party = Model.get('party.party')
     >>> ProductTemplate = Model.get('product.template')
     >>> ProductUom = Model.get('product.uom')
     >>> ShipmentIn = Model.get('stock.shipment.in')
     >>> ShipmentOutReturn = Model.get('stock.shipment.out.return')
     >>> StockLocation = Model.get('stock.location')
@@ -130,15 +130,15 @@
     >>> move.from_location = shipment.supplier_location
     >>> move.to_location = shipment.warehouse_input
     >>> move.product = product
     >>> move.quantity = 10
     >>> move.unit_price = Decimal('100.0000')
     >>> move.currency = eur
     >>> shipment.click('receive')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
     >>> move, = shipment.incoming_moves
     >>> move.intrastat_type
 
     >>> move, = shipment.inventory_moves
@@ -152,15 +152,15 @@
     >>> move.from_location = shipment.supplier_location
     >>> move.to_location = shipment.warehouse_input
     >>> move.product = product
     >>> move.quantity = 20
     >>> move.unit_price = Decimal('90.0000')
     >>> move.currency = eur
     >>> shipment.click('receive')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
     >>> move, = shipment.incoming_moves
     >>> move.intrastat_type
     'arrival'
     >>> move.intrastat_warehouse_country.code
@@ -175,16 +175,15 @@
     Decimal('1800.00')
     >>> move.intrastat_transaction.code
     '11'
     >>> move.intrastat_additional_unit
     20.0
     >>> move.intrastat_country_of_origin
     >>> move.intrastat_vat
-    >>> move.intrastat_declaration.month == today.replace(day=1)
-    True
+    >>> assertEqual(move.intrastat_declaration.month, today.replace(day=1))
 
     >>> move, = shipment.inventory_moves
     >>> move.intrastat_type
 
 Receive products from US::
 
     >>> shipment = ShipmentIn()
@@ -193,15 +192,15 @@
     >>> move.from_location = shipment.supplier_location
     >>> move.to_location = shipment.warehouse_input
     >>> move.product = product
     >>> move.quantity = 30
     >>> move.unit_price = Decimal('120.0000')
     >>> move.currency = usd
     >>> shipment.click('receive')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
     >>> move, = shipment.incoming_moves
     >>> move.intrastat_type
 
     >>> move, = shipment.inventory_moves
@@ -215,15 +214,15 @@
     >>> move.from_location = shipment.customer_location
     >>> move.to_location = shipment.warehouse_input
     >>> move.product = product
     >>> move.quantity = 5
     >>> move.unit_price = Decimal('150.0000')
     >>> move.currency = eur
     >>> shipment.click('receive')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
     >>> move, = shipment.incoming_moves
     >>> move.intrastat_type
     'arrival'
     >>> move.intrastat_warehouse_country.code
@@ -238,27 +237,25 @@
     Decimal('750.00')
     >>> move.intrastat_transaction.code
     '21'
     >>> move.intrastat_additional_unit
     5.0
     >>> move.intrastat_country_of_origin
     >>> move.intrastat_vat
-    >>> move.intrastat_declaration.month == today.replace(day=1)
-    True
+    >>> assertEqual(move.intrastat_declaration.month, today.replace(day=1))
 
     >>> move, = shipment.inventory_moves
     >>> move.intrastat_type
 
 Check declaration::
 
     >>> declaration, = IntrastatDeclaration.find([])
     >>> declaration.country.code
     'BE'
-    >>> declaration.month == today.replace(day=1)
-    True
+    >>> assertEqual(declaration.month, today.replace(day=1))
     >>> declaration.state
     'opened'
     >>> bool(declaration.extended)
     False
 
     >>> with config.set_context(declaration=declaration.id):
     ...     declaration_line, _ = IntrastatDeclarationLine.find([])
@@ -268,16 +265,16 @@
     'FR'
     >>> declaration_line.subdivision.intrastat_code
     '2'
     >>> declaration_line.tariff_code.code
     '9403 10 51'
     >>> declaration_line.weight
     60.0
-    >>> declaration_line.value == Decimal('1800.00')
-    True
+    >>> declaration_line.value
+    Decimal('1800.00')
     >>> declaration_line.transaction.code
     '11'
     >>> declaration_line.additional_unit
     20.0
     >>> declaration_line.country_of_origin
     >>> declaration_line.vat
```

### Comparing `trytond_account_stock_eu-7.0.0/tests/scenario_account_stock_eu_dispatch.rst` & `trytond_account_stock_eu-7.2.0/tests/scenario_account_stock_eu_dispatch.rst`

 * *Files 5% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
     >>> import datetime as dt
     >>> import io
     >>> import zipfile
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.modules.currency.tests.tools import get_currency
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_stock_eu')
 
     >>> Country = Model.get('country.country')
     >>> IntrastatDeclaration = Model.get('account.stock.eu.intrastat.declaration')
-    >>> IntrastatDeclarationLine = Model.get('account.stock.eu.intrastat.declaration.line')
+    >>> IntrastatDeclarationLine = Model.get(
+    ...     'account.stock.eu.intrastat.declaration.line')
     >>> Organization = Model.get('country.organization')
     >>> Party = Model.get('party.party')
     >>> ProductTemplate = Model.get('product.template')
     >>> ProductUom = Model.get('product.uom')
     >>> ShipmentOut = Model.get('stock.shipment.out')
     >>> ShipmentInReturn = Model.get('stock.shipment.in.return')
     >>> StockLocation = Model.get('stock.location')
@@ -133,15 +133,15 @@
     >>> move.product = product
     >>> move.quantity = 10
     >>> move.unit_price = Decimal('100.0000')
     >>> move.currency = eur
     >>> shipment.click('wait')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
     >>> move, = shipment.inventory_moves
     >>> move.intrastat_type
 
     >>> move, = shipment.outgoing_moves
@@ -157,15 +157,15 @@
     >>> move.product = product
     >>> move.quantity = 20
     >>> move.unit_price = Decimal('90.0000')
     >>> move.currency = eur
     >>> shipment.click('wait')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
     >>> move, = shipment.inventory_moves
     >>> move.intrastat_type
 
     >>> move, = shipment.outgoing_moves
@@ -184,16 +184,15 @@
     >>> move.intrastat_transaction.code
     '12'
     >>> move.intrastat_additional_unit
     20.0
     >>> move.intrastat_country_of_origin.code
     'CN'
     >>> move.intrastat_vat
-    >>> move.intrastat_declaration.month == today.replace(day=1)
-    True
+    >>> assertEqual(move.intrastat_declaration.month, today.replace(day=1))
 
 
 Send products to US::
 
     >>> shipment = ShipmentOut()
     >>> shipment.customer = customer_us
     >>> move = shipment.outgoing_moves.new()
@@ -202,15 +201,15 @@
     >>> move.product = product
     >>> move.quantity = 30
     >>> move.unit_price = Decimal('120.0000')
     >>> move.currency = usd
     >>> shipment.click('wait')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
     >>> move, = shipment.inventory_moves
     >>> move.intrastat_type
 
     >>> move, = shipment.outgoing_moves
@@ -226,15 +225,15 @@
     >>> move.to_location = shipment.to_location
     >>> move.product = product
     >>> move.quantity = 5
     >>> move.unit_price = Decimal('150.0000')
     >>> move.currency = eur
     >>> shipment.click('wait')
     >>> shipment.click('assign_force')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
     >>> move, = shipment.moves
     >>> move.intrastat_type
     'dispatch'
     >>> move.intrastat_warehouse_country.code
@@ -251,24 +250,22 @@
     '21'
     >>> move.intrastat_additional_unit
     5.0
     >>> move.intrastat_country_of_origin.code
     'CN'
     >>> move.intrastat_vat.code
     'FR40303265045'
-    >>> move.intrastat_declaration.month == today.replace(day=1)
-    True
+    >>> assertEqual(move.intrastat_declaration.month, today.replace(day=1))
 
 Check declaration::
 
     >>> declaration, = IntrastatDeclaration.find([])
     >>> declaration.country.code
     'BE'
-    >>> declaration.month == today.replace(day=1)
-    True
+    >>> assertEqual(declaration.month, today.replace(day=1))
     >>> declaration.state
     'opened'
 
     >>> with config.set_context(declaration=declaration.id):
     ...     _, declaration_line = IntrastatDeclarationLine.find([])
     >>> declaration_line.type
     'dispatch'
@@ -276,16 +273,16 @@
     'FR'
     >>> declaration_line.subdivision.intrastat_code
     '2'
     >>> declaration_line.tariff_code.code
     '9403 10 51'
     >>> declaration_line.weight
     15.0
-    >>> declaration_line.value == Decimal('750.00')
-    True
+    >>> declaration_line.value
+    Decimal('750.00')
     >>> declaration_line.transaction.code
     '21'
     >>> declaration_line.additional_unit
     5.0
     >>> declaration_line.country_of_origin.code
     'CN'
     >>> declaration_line.vat.code
```

### Comparing `trytond_account_stock_eu-7.0.0/tox.ini` & `trytond_account_stock_eu-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/trytond_account_stock_eu.egg-info/PKG-INFO` & `trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-account-stock-eu
-Version: 7.0.0
+Name: trytond_account_stock_eu
+Version: 7.2.0
 Summary: Tryton module for european stock accounting
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: bugs@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-stock-eu
+Project-URL: Documentation, https://docs.tryton.org/modules-account-stock-eu
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account stock europe intrastat
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,30 +49,30 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_country<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_customs<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_product_measurements<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_measurements<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_country<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_customs<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_product_measurements<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_measurements<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_carrier<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_incoterm<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_consignment<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_carrier<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_incoterm<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_consignment<7.3,>=7.2; extra == "test"
 
 #######################
 Account Stock EU Module
 #######################
 
 The *Account Stock EU Module* is used to generate the `Intrastat
 <https://en.wikipedia.org/wiki/Intrastat>`_ declarations every month.
```

### Comparing `trytond_account_stock_eu-7.0.0/trytond_account_stock_eu.egg-info/SOURCES.txt` & `trytond_account_stock_eu-7.2.0/trytond_account_stock_eu.egg-info/SOURCES.txt`

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

### Comparing `trytond_account_stock_eu-7.0.0/view/intrastat_declaration_line_list.xml` & `trytond_account_stock_eu-7.2.0/view/intrastat_declaration_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/view/stock_move_form.xml` & `trytond_account_stock_eu-7.2.0/view/stock_move_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_eu-7.0.0/view/stock_shipment_form.xml` & `trytond_account_stock_eu-7.2.0/view/stock_shipment_form.xml`

 * *Files identical despite different names*

