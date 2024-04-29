# Comparing `tmp/trytond_production-7.0.1.tar.gz` & `tmp/trytond_production-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_production-7.0.1.tar", last modified: Mon Jan 15 23:20:00 2024, max compression
+gzip compressed data, was "trytond_production-7.2.0.tar", last modified: Mon Apr 29 15:43:58 2024, max compression
```

## Comparing `trytond_production-7.0.1.tar` & `trytond_production-7.2.0.tar`

### file list

```diff
@@ -1,102 +1,104 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:20:00.816428 trytond_production-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-30 17:06:38.000000 trytond_production-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     3524 2024-01-15 23:19:58.000000 trytond_production-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-01-15 23:19:58.000000 trytond_production-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_production-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_production-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4373 2024-01-15 23:20:00.816428 trytond_production-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1781 2023-10-30 17:06:38.000000 trytond_production-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1045 2023-10-30 17:06:38.000000 trytond_production-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9453 2023-10-30 17:06:38.000000 trytond_production-7.0.1/bom.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6296 2023-10-30 17:06:38.000000 trytond_production-7.0.1/bom.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1826 2023-10-30 17:06:38.000000 trytond_production-7.0.1/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2122 2023-10-30 17:06:38.000000 trytond_production-7.0.1/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:20:00.809761 trytond_production-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2811 2023-10-30 17:06:38.000000 trytond_production-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1781 2023-10-30 17:06:38.000000 trytond_production-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_production-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      230 2023-10-30 17:06:38.000000 trytond_production-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:20:00.809761 trytond_production-7.0.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_production-7.0.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-10-30 17:06:38.000000 trytond_production-7.0.1/icons/tryton-production.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      574 2023-10-30 17:06:38.000000 trytond_production-7.0.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:20:00.809761 trytond_production-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14569 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14348 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12671 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14334 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14215 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11823 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13229 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14373 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12658 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14272 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13334 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12270 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13882 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14285 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12731 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14089 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13274 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13811 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12158 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14726 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13667 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13554 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11806 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12726 2023-10-30 17:06:38.000000 trytond_production-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      811 2023-10-30 17:06:38.000000 trytond_production-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4297 2023-10-30 17:06:38.000000 trytond_production-7.0.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4276 2023-10-30 17:06:38.000000 trytond_production-7.0.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    32449 2024-01-08 11:30:23.000000 trytond_production-7.0.1/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12924 2023-10-30 17:06:38.000000 trytond_production-7.0.1/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-01-15 23:20:00.816428 trytond_production-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4462 2023-10-30 17:06:38.000000 trytond_production-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5952 2023-10-30 17:06:38.000000 trytond_production-7.0.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1940 2023-10-30 17:06:38.000000 trytond_production-7.0.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:20:00.813094 trytond_production-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_production-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7219 2023-10-30 17:06:38.000000 trytond_production-7.0.1/tests/scenario_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2745 2023-10-30 17:06:38.000000 trytond_production-7.0.1/tests/scenario_production_by_product.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2030 2023-10-30 17:06:38.000000 trytond_production-7.0.1/tests/scenario_production_lot_number.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2179 2023-10-30 17:06:38.000000 trytond_production-7.0.1/tests/scenario_production_no_list_price.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2475 2023-10-30 17:06:38.000000 trytond_production-7.0.1/tests/scenario_production_rounding.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3160 2023-10-30 17:06:38.000000 trytond_production-7.0.1/tests/scenario_production_set_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2947 2023-10-30 17:06:38.000000 trytond_production-7.0.1/tests/scenario_production_waste.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1517 2023-10-30 17:06:38.000000 trytond_production-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_production-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_production-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2023-10-30 17:55:12.000000 trytond_production-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:20:00.816428 trytond_production-7.0.1/trytond_production.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4373 2024-01-15 23:20:00.000000 trytond_production-7.0.1/trytond_production.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3599 2024-01-15 23:20:00.000000 trytond_production-7.0.1/trytond_production.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-01-15 23:20:00.000000 trytond_production-7.0.1/trytond_production.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-01-15 23:20:00.000000 trytond_production-7.0.1/trytond_production.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:57.000000 trytond_production-7.0.1/trytond_production.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-01-15 23:20:00.000000 trytond_production-7.0.1/trytond_production.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-01-15 23:20:00.000000 trytond_production-7.0.1/trytond_production.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-01-15 23:20:00.816428 trytond_production-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      457 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/bom_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/bom_input_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/bom_input_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/bom_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/bom_output_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/bom_output_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/bom_tree_open_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/bom_tree_open_tree_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/bom_tree_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      266 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      605 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/product_bom_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/product_bom_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/product_bom_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/production_calendar.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2236 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/production_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/production_lead_time_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      268 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/production_lead_time_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/production_lead_time_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      536 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/production_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/stock_move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      309 2023-10-30 17:06:38.000000 trytond_production-7.0.1/view/template_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:58.843868 trytond_production-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4169 2024-04-29 15:22:30.000000 trytond_production-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:22:30.000000 trytond_production-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_production-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_production-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2836 2024-04-29 15:43:58.843868 trytond_production-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-27 16:30:39.000000 trytond_production-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1045 2024-01-27 09:58:52.000000 trytond_production-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9434 2024-04-27 16:30:39.000000 trytond_production-7.2.0/bom.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6250 2024-04-27 16:30:39.000000 trytond_production-7.2.0/bom.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1826 2024-01-27 09:58:52.000000 trytond_production-7.2.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2076 2024-04-27 16:30:39.000000 trytond_production-7.2.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:58.837201 trytond_production-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-27 16:30:39.000000 trytond_production-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3141 2024-04-27 16:30:39.000000 trytond_production-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-27 16:30:39.000000 trytond_production-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-27 16:30:39.000000 trytond_production-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:17.000000 trytond_production-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      230 2023-04-15 07:12:15.000000 trytond_production-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:58.837201 trytond_production-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_production-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      338 2023-01-16 14:00:20.000000 trytond_production-7.2.0/icons/tryton-production.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      951 2024-04-27 16:30:39.000000 trytond_production-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:58.840535 trytond_production-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14569 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14348 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12671 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14334 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14215 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11823 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13229 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14373 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12658 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14272 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13334 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12270 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13882 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14285 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12731 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14089 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13274 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13811 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14032 2024-04-29 13:17:17.000000 trytond_production-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14726 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13667 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13554 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11806 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12726 2024-04-27 16:43:25.000000 trytond_production-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      811 2023-04-15 07:12:15.000000 trytond_production-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4297 2024-01-27 09:58:52.000000 trytond_production-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4152 2024-04-27 16:30:39.000000 trytond_production-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    32160 2024-04-27 16:30:39.000000 trytond_production-7.2.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12522 2024-04-27 16:30:39.000000 trytond_production-7.2.0/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:43:58.843868 trytond_production-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4602 2024-04-27 16:30:39.000000 trytond_production-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6212 2024-04-27 16:30:39.000000 trytond_production-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1917 2024-04-27 16:30:39.000000 trytond_production-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:58.840535 trytond_production-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_production-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7298 2024-04-27 16:30:39.000000 trytond_production-7.2.0/tests/scenario_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2722 2024-04-27 16:30:39.000000 trytond_production-7.2.0/tests/scenario_production_by_product.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2013 2024-04-27 16:30:39.000000 trytond_production-7.2.0/tests/scenario_production_lot_number.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2908 2024-04-27 16:30:39.000000 trytond_production-7.2.0/tests/scenario_production_lot_trace.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2156 2024-04-27 16:30:39.000000 trytond_production-7.2.0/tests/scenario_production_no_list_price.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2454 2024-04-22 12:14:36.000000 trytond_production-7.2.0/tests/scenario_production_rounding.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3137 2024-04-27 16:30:39.000000 trytond_production-7.2.0/tests/scenario_production_set_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2923 2024-04-27 16:30:39.000000 trytond_production-7.2.0/tests/scenario_production_waste.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1517 2024-02-04 18:51:26.000000 trytond_production-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_production-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:17.000000 trytond_production-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-29 15:22:25.000000 trytond_production-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:58.843868 trytond_production-7.2.0/trytond_production.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2836 2024-04-29 15:43:58.000000 trytond_production-7.2.0/trytond_production.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3695 2024-04-29 15:43:58.000000 trytond_production-7.2.0/trytond_production.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:43:58.000000 trytond_production-7.2.0/trytond_production.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-29 15:43:58.000000 trytond_production-7.2.0/trytond_production.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_production-7.2.0/trytond_production.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-29 15:43:58.000000 trytond_production-7.2.0/trytond_production.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:43:58.000000 trytond_production-7.2.0/trytond_production.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:58.843868 trytond_production-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      457 2023-01-16 14:00:21.000000 trytond_production-7.2.0/view/bom_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-02-04 18:51:26.000000 trytond_production-7.2.0/view/bom_input_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-02-04 18:51:26.000000 trytond_production-7.2.0/view/bom_input_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 trytond_production-7.2.0/view/bom_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-02-04 18:51:26.000000 trytond_production-7.2.0/view/bom_output_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-02-04 18:51:26.000000 trytond_production-7.2.0/view/bom_output_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-02-04 18:51:26.000000 trytond_production-7.2.0/view/bom_tree_open_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      215 2023-01-16 14:00:21.000000 trytond_production-7.2.0/view/bom_tree_open_tree_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-02-04 18:51:26.000000 trytond_production-7.2.0/view/bom_tree_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      266 2023-01-16 14:00:21.000000 trytond_production-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      605 2023-04-15 07:12:15.000000 trytond_production-7.2.0/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2023-01-16 14:00:21.000000 trytond_production-7.2.0/view/product_bom_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-01-16 14:00:20.000000 trytond_production-7.2.0/view/product_bom_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-01-16 14:00:20.000000 trytond_production-7.2.0/view/product_bom_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2024-01-27 09:58:52.000000 trytond_production-7.2.0/view/product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2023-01-16 14:00:21.000000 trytond_production-7.2.0/view/production_calendar.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2234 2024-04-27 16:30:39.000000 trytond_production-7.2.0/view/production_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-01-16 14:00:21.000000 trytond_production-7.2.0/view/production_lead_time_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      268 2023-01-16 14:00:21.000000 trytond_production-7.2.0/view/production_lead_time_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_production-7.2.0/view/production_lead_time_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      536 2024-02-04 18:51:26.000000 trytond_production-7.2.0/view/production_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-04-15 07:12:15.000000 trytond_production-7.2.0/view/stock_move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-04-15 07:12:15.000000 trytond_production-7.2.0/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      309 2023-04-15 07:12:15.000000 trytond_production-7.2.0/view/template_list.xml
```

### Comparing `trytond_production-7.0.1/CHANGELOG` & `trytond_production-7.2.0/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
-Version 7.0.1 - 2024-01-15
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
-
+* Rename 'done' button to 'do'
+* Fill production number only in waiting state
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 * Rename Uom to Unit for bill of material
 * Rename Uom to Unit for production
@@ -22,99 +23,121 @@
 * Assign all possible productions when trying
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 6.4.0 - 2022-05-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Show production on stock move form
 * Add support for Python 3.10
 * Remove support for Python 3.6
 
 Version 6.2.0 - 2021-11-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Show warning when output product's list price is empty
 * Remove unique product constraint on BOM
 
 Version 6.0.0 - 2021-05-03
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Allow productions to be automatically assigned
 * Default to ordering productions by date
 
 Version 5.8.0 - 2020-11-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove support for Python 3.5
 * Add production picking and output locations
 * Add cron task to reschedule past productions
 * Allow lost_found as output of production
 * Keep cost of unused input products
 * Use the shipment assign wizard for production
 * Rename production state from cancel to cancelled
 
 Version 5.6.0 - 2020-05-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add origin to production
 * Delete cancelled moves when a production is reset to draft
 * Add employee on productions for some states
 * Convert set_moves into dualmethod
 * Add reference to production record name
 * Add cron task to update production cost
 * Allocate cost based on list price of each product
 
 Version 5.4.0 - 2019-11-04
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.2.0 - 2019-05-06
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 5.0.0 - 2018-10-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove support for Python 2.7
 * Set output cost in done transition
 
 Version 4.8.0 - 2018-04-23
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 4.6.0 - 2017-10-30
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 4.4.0 - 2017-05-01
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Ceil input and floor output quantities
 * Add producible to product template
 
 Version 4.2.0 - 2016-11-28
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add Lead Time of Production
 * Add Start Dates on Production
 
 Version 4.0.0 - 2016-05-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Rename Production code into number
 * Add Python3 support
 
 Version 3.8.0 - 2015-11-02
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 3.6.0 - 2015-04-20
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for PyPy
+
 Version 3.4.0 - 2014-10-20
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 3.2.0 - 2014-04-21
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Allow to define effective date of productions
 
 Version 3.0.0 - 2013-10-21
+--------------------------
 * Bug fixes (see mercurial logs for details)
 * Add calendar view
 
 Version 2.8.0 - 2013-04-22
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.6.0 - 2012-10-22
+--------------------------
 * Bug fixes (see mercurial logs for details)
 
 Version 2.4.0 - 2012-08-15
+--------------------------
 * Initial release
```

### Comparing `trytond_production-7.0.1/LICENSE` & `trytond_production-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/__init__.py` & `trytond_production-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/bom.py` & `trytond_production-7.2.0/bom.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     def compute_quantity(self, factor):
         return self.unit.ceil(self.quantity * factor)
 
 
 class BOMOutput(BOMInput):
     "Bill of Material Output"
     __name__ = 'production.bom.output'
-    _table = 'production_bom_output'  # Needed to override BOMInput._table
+    _table = None  # Needed to override BOMInput._table
 
     def compute_quantity(self, factor):
         return self.unit.floor(self.quantity * factor)
 
     @classmethod
     def delete(cls, outputs):
         pool = Pool()
```

### Comparing `trytond_production-7.0.1/bom.xml` & `trytond_production-7.2.0/bom.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_production-7.0.1/bom.xml` & `trytond_production-7.2.0/bom.xml`

```diff
@@ -29,22 +29,22 @@
     </record>
     <menuitem parent="menu_configuration" action="act_bom_list" sequence="20" id="menu_bom_list"/>
     <record model="ir.action.act_window" id="act_bom_form">
       <field name="name">BOM</field>
       <field name="res_model">production.bom</field>
     </record>
     <record model="ir.model.access" id="access_bom">
-      <field name="model" search="[('model', '=', 'production.bom')]"/>
+      <field name="model">production.bom</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_bom_admin">
-      <field name="model" search="[('model', '=', 'production.bom')]"/>
+      <field name="model">production.bom</field>
       <field name="group" ref="group_production_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="bom_input_view_list">
```

### Comparing `trytond_production-7.0.1/configuration.py` & `trytond_production-7.2.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/configuration.xml` & `trytond_production-7.2.0/configuration.xml`

 * *Files 10% similar despite different names*

#### Comparing `trytond_production-7.0.1/configuration.xml` & `trytond_production-7.2.0/configuration.xml`

```diff
@@ -15,22 +15,22 @@
     <record model="ir.action.act_window.view" id="act_production_configuration_form_view1">
       <field name="sequence" eval="10"/>
       <field name="view" ref="production_configuration_view_form"/>
       <field name="act_window" ref="act_production_configuration_form"/>
     </record>
     <menuitem parent="menu_configuration" action="act_production_configuration_form" sequence="10" id="menu_production_configuration" icon="tryton-list"/>
     <record model="ir.model.access" id="access_production_configuration">
-      <field name="model" search="[('model', '=', 'production.configuration')]"/>
+      <field name="model">production.configuration</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_production_configuration_production_admin">
-      <field name="model" search="[('model', '=', 'production.configuration')]"/>
+      <field name="model">production.configuration</field>
       <field name="group" ref="group_production_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_production-7.0.1/doc/conf.py` & `trytond_production-7.2.0/doc/conf.py`

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

### Comparing `trytond_production-7.0.1/icons/LICENSE` & `trytond_production-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/bg.po` & `trytond_production-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/ca.po` & `trytond_production-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/cs.po` & `trytond_production-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/de.po` & `trytond_production-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/es.po` & `trytond_production-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/es_419.po` & `trytond_production-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/et.po` & `trytond_production-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/fa.po` & `trytond_production-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/fi.po` & `trytond_production-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/fr.po` & `trytond_production-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/hu.po` & `trytond_production-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/id.po` & `trytond_production-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/it.po` & `trytond_production-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/lo.po` & `trytond_production-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/lt.po` & `trytond_production-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/nl.po` & `trytond_production-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/pl.po` & `trytond_production-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/pt.po` & `trytond_production-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/ro.po` & `trytond_production-7.2.0/locale/tr.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,281 +1,290 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
-msgstr ""
+msgstr "BOMlar"
 
 msgctxt "field:product.product,producible:"
 msgid "Producible"
-msgstr ""
+msgstr "Üretilebilir"
 
+#, fuzzy
 msgctxt "field:product.product,production_lead_times:"
 msgid "Lead Times"
-msgstr ""
+msgstr "Tedarik Süreleri"
 
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
-msgstr ""
+msgstr "BOM"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr "Ürün"
 
 msgctxt "field:product.template,producible:"
 msgid "Producible"
-msgstr ""
+msgstr "Üretilebilir"
 
+#, fuzzy
 msgctxt "field:production,assigned_by:"
 msgid "Assigned By"
-msgstr ""
+msgstr "Assigned"
 
 msgctxt "field:production,bom:"
 msgid "BOM"
-msgstr ""
+msgstr "BOM"
 
 msgctxt "field:production,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr "Şirket"
 
 msgctxt "field:production,cost:"
 msgid "Cost"
-msgstr "Cost"
+msgstr "Maliyet"
 
+#, fuzzy
 msgctxt "field:production,done_by:"
 msgid "Done By"
-msgstr ""
+msgstr "Done"
 
 msgctxt "field:production,effective_start_date:"
 msgid "Effective Start Date"
-msgstr ""
+msgstr "Yürürlük Başlangıç Tarihi"
 
 msgctxt "field:production,inputs:"
 msgid "Inputs"
-msgstr ""
+msgstr "Girdiler"
 
 msgctxt "field:production,location:"
 msgid "Location"
-msgstr ""
+msgstr "Lokasyon"
 
 msgctxt "field:production,number:"
 msgid "Number"
-msgstr ""
+msgstr "Sayı"
 
 msgctxt "field:production,origin:"
 msgid "Origin"
-msgstr "Origine"
+msgstr ""
 
 msgctxt "field:production,outputs:"
 msgid "Outputs"
-msgstr ""
+msgstr "Çıktılar"
 
+#, fuzzy
 msgctxt "field:production,partially_assigned:"
 msgid "Partially Assigned"
-msgstr ""
+msgstr "Assigned"
 
 msgctxt "field:production,planned_start_date:"
 msgid "Planned Start Date"
-msgstr ""
+msgstr "Planlanan Başlangıç Tarihi"
 
 msgctxt "field:production,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr "Ürün"
 
 msgctxt "field:production,quantity:"
 msgid "Quantity"
-msgstr "Cantitate"
+msgstr "Miktar"
 
 msgctxt "field:production,reference:"
 msgid "Reference"
-msgstr "Referinţă"
+msgstr "Referans"
 
 msgctxt "field:production,run_by:"
 msgid "Run By"
 msgstr ""
 
 msgctxt "field:production,state:"
 msgid "State"
-msgstr ""
+msgstr "Durum"
 
+#, fuzzy
 msgctxt "field:production,unit:"
 msgid "Unit"
-msgstr ""
+msgstr "Birim"
 
 #, fuzzy
 msgctxt "field:production,uom_category:"
 msgid "UoM Category"
-msgstr "Categorie"
+msgstr "Ölçü Birimi Kategorisi"
 
 msgctxt "field:production,warehouse:"
 msgid "Warehouse"
-msgstr ""
+msgstr "Depo"
 
 msgctxt "field:production.bom,inputs:"
 msgid "Inputs"
-msgstr ""
+msgstr "Girdiler"
 
 msgctxt "field:production.bom,name:"
 msgid "Name"
-msgstr ""
+msgstr "Ad"
 
 msgctxt "field:production.bom,output_products:"
 msgid "Output Products"
-msgstr ""
+msgstr "Çıktı Ürünler"
 
 msgctxt "field:production.bom,outputs:"
 msgid "Outputs"
-msgstr ""
+msgstr "Çıktılar"
 
 msgctxt "field:production.bom.input,bom:"
 msgid "BOM"
-msgstr ""
+msgstr "BOM"
 
 msgctxt "field:production.bom.input,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr "Ürün"
 
 msgctxt "field:production.bom.input,quantity:"
 msgid "Quantity"
-msgstr "Cantitate"
+msgstr "Miktar"
 
+#, fuzzy
 msgctxt "field:production.bom.input,unit:"
 msgid "Unit"
-msgstr ""
+msgstr "Birim"
 
 msgctxt "field:production.bom.input,uom_category:"
 msgid "Uom Category"
-msgstr ""
+msgstr "Ölçü Birimi Kategorisi"
 
 msgctxt "field:production.bom.output,bom:"
 msgid "BOM"
-msgstr ""
+msgstr "BOM"
 
 msgctxt "field:production.bom.output,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr "Ürün"
 
 msgctxt "field:production.bom.output,quantity:"
 msgid "Quantity"
-msgstr ""
+msgstr "Miktar"
 
+#, fuzzy
 msgctxt "field:production.bom.output,unit:"
 msgid "Unit"
-msgstr ""
+msgstr "Birim"
 
 msgctxt "field:production.bom.output,uom_category:"
 msgid "Uom Category"
-msgstr ""
+msgstr "Ölçü Birimi Kategorisi"
 
 msgctxt "field:production.bom.tree,childs:"
 msgid "Childs"
-msgstr ""
+msgstr "Alt Elemanlar"
 
 msgctxt "field:production.bom.tree,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr "Ürün"
 
 msgctxt "field:production.bom.tree,quantity:"
 msgid "Quantity"
-msgstr ""
+msgstr "Miktar"
 
+#, fuzzy
 msgctxt "field:production.bom.tree,unit:"
 msgid "Unit"
-msgstr ""
+msgstr "Birim"
 
 msgctxt "field:production.bom.tree.open.start,bom:"
 msgid "BOM"
-msgstr ""
+msgstr "BOM"
 
 msgctxt "field:production.bom.tree.open.start,category:"
 msgid "Category"
-msgstr "Categorie"
+msgstr "Kategori"
 
 msgctxt "field:production.bom.tree.open.start,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr "Ürün"
 
 msgctxt "field:production.bom.tree.open.start,quantity:"
 msgid "Quantity"
-msgstr "Cantitate"
+msgstr "Miktar"
 
+#, fuzzy
 msgctxt "field:production.bom.tree.open.start,unit:"
 msgid "Unit"
-msgstr ""
+msgstr "Birim"
 
 msgctxt "field:production.bom.tree.open.tree,bom_tree:"
 msgid "BOM Tree"
-msgstr ""
+msgstr "BOM Ağacı"
 
 msgctxt "field:production.configuration,production_sequence:"
 msgid "Production Sequence"
-msgstr ""
+msgstr "Ürün Sırası"
 
 msgctxt "field:production.configuration.production_sequence,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr "Şirket"
 
 msgctxt ""
 "field:production.configuration.production_sequence,production_sequence:"
 msgid "Production Sequence"
-msgstr ""
+msgstr "Ürün Sırası"
 
 msgctxt "field:production.lead_time,bom:"
 msgid "BOM"
-msgstr ""
+msgstr "BOM"
 
 msgctxt "field:production.lead_time,lead_time:"
 msgid "Lead Time"
-msgstr ""
+msgstr "Tedarik Süresi"
 
 msgctxt "field:production.lead_time,product:"
 msgid "Product"
-msgstr "Produs"
+msgstr "Ürün"
 
 msgctxt "field:stock.location,production_location:"
 msgid "Production"
-msgstr ""
+msgstr "Ürün"
 
 #, fuzzy
 msgctxt "field:stock.location,production_output_location:"
 msgid "Production Output"
-msgstr "Produs"
+msgstr "Ürün Çıktısı"
 
 #, fuzzy
 msgctxt "field:stock.location,production_picking_location:"
 msgid "Production Picking"
-msgstr "Produs"
+msgstr "Ürün"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,production_input:"
 msgid "Production Input"
-msgstr "Produs"
+msgstr "Ürün Girdisi"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,production_output:"
 msgid "Production Output"
-msgstr "Produs"
+msgstr "Ürün Çıktısı"
 
 #, fuzzy
 msgctxt "field:stock.move,production:"
 msgid "Production"
-msgstr "Produs"
+msgstr "Ürün"
 
 msgctxt "field:stock.move,production_cost_price_updated:"
 msgid "Cost Price Updated"
 msgstr ""
 
 msgctxt "field:stock.move,production_input:"
 msgid "Production Input"
-msgstr ""
+msgstr "Ürün Girdisi"
 
 msgctxt "field:stock.move,production_output:"
 msgid "Production Output"
-msgstr ""
+msgstr "Ürün Çıktısı"
 
 msgctxt "help:production,number:"
 msgid "The main identifier for the shipment."
 msgstr ""
 
 msgctxt "help:production,reference:"
 msgid "The external identifier for the shipment."
@@ -295,95 +304,113 @@
 msgid ""
 "Where the production components are picked from.\n"
 "Leave empty to use the warehouse storage location."
 msgstr ""
 
 msgctxt "model:ir.action,name:act_bom_form"
 msgid "BOM"
-msgstr ""
+msgstr "BOM"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_bom_list"
 msgid "BOMs"
-msgstr ""
+msgstr "BOMs"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_product_in_bom"
 msgid "BOMs"
-msgstr ""
+msgstr "BOMs"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_production_calendar"
 msgid "Productions"
-msgstr "Producţie"
+msgstr "Productions"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_production_configuration_form"
 msgid "Configuration"
-msgstr "Configurare"
+msgstr "Configuration"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_production_list"
 msgid "Productions"
-msgstr "Producţie"
+msgstr "Productions"
 
+#, fuzzy
 msgctxt "model:ir.action,name:wizard_bom_tree_open"
 msgid "BOM Tree"
-msgstr ""
+msgstr "BOM Tree"
 
 #, fuzzy
 msgctxt "model:ir.action,name:wizard_production_assign"
 msgid "Assign Production"
-msgstr "Produs"
+msgstr "Assign Production"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_product_in_bom_output_domain_input"
 msgid "As Inputs"
-msgstr ""
+msgstr "As Inputs"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_product_in_bom_output_domain_output"
 msgid "As Outputs"
-msgstr ""
+msgstr "As Outputs"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_all"
 msgid "All"
-msgstr ""
+msgstr "All"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_assigned"
 msgid "Assigned"
-msgstr ""
+msgstr "Assigned"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_available"
 msgid "Partially Assigned"
-msgstr ""
+msgstr "Assigned"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_draft"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_requests"
 msgid "Requests"
-msgstr ""
+msgstr "Requests"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_running"
 msgid "Running"
-msgstr ""
+msgstr "Running"
 
+#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_waiting"
 msgid "Waiting"
-msgstr ""
+msgstr "Waiting"
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_missing_product_list_price"
 msgid ""
 "The product \"%(product)s\" on production \"%(production)s\" does not have "
 "any list price defined."
 msgstr ""
+"Üretim \"%(production)s\" çıktılarının (%(outputs)s) maliyetleri üretim "
+"(%(costs)s) maliyetleri ile uyuşmamaktadır."
 
 msgctxt "model:ir.message,text:msg_recursive_bom"
 msgid "You cannot create a recursive BOM for product \"%(product)s\"."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_stock_move_production_single"
 msgid "Move can not be used for production input and output."
@@ -391,198 +418,211 @@
 
 msgctxt "model:ir.model.button,confirm:production_done_button"
 msgid "Are you sure you want to complete the production?"
 msgstr ""
 
 msgctxt "model:ir.model.button,string:production_assign_wizard_button"
 msgid "Assign"
-msgstr ""
+msgstr "Assign"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
-msgstr ""
+msgstr "Cancel"
 
 msgctxt "model:ir.model.button,string:production_done_button"
 msgid "Done"
-msgstr ""
+msgstr "Done"
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
-msgstr ""
+msgstr "Draft"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
-msgstr ""
+msgstr "Reset to BOM"
 
 msgctxt "model:ir.model.button,string:production_run_button"
 msgid "Run"
-msgstr ""
+msgstr "Run"
 
 msgctxt "model:ir.model.button,string:production_wait_button"
 msgid "Wait"
-msgstr ""
+msgstr "Wait"
 
 msgctxt "model:ir.rule.group,name:rule_group_production_companies"
 msgid "User in companies"
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.sequence,name:sequence_production"
 msgid "Production"
-msgstr ""
+msgstr "Production"
 
+#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_production"
 msgid "Production"
-msgstr ""
+msgstr "Production"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_bom_list"
 msgid "BOMs"
-msgstr ""
+msgstr "BOMs"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configurare"
+msgstr "Configuration"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_production"
 msgid "Productions"
-msgstr "Producţie"
+msgstr "Productions"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_production_calendar"
 msgid "Productions"
-msgstr "Producţie"
+msgstr "Productions"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_production_configuration"
 msgid "Configuration"
-msgstr "Configurație"
+msgstr "Configuration"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_production_list"
 msgid "Productions"
-msgstr "Producţie"
+msgstr "Productions"
 
 msgctxt "model:product.product-production.bom,name:"
 msgid "Product - BOM"
-msgstr ""
+msgstr "Ürün - BOM"
 
 msgctxt "model:production,name:"
 msgid "Production"
-msgstr ""
+msgstr "Üretim"
 
 msgctxt "model:production.bom,name:"
 msgid "Bill of Material"
-msgstr ""
+msgstr "BOM"
 
 msgctxt "model:production.bom.input,name:"
 msgid "Bill of Material Input"
-msgstr ""
+msgstr "bOM Girdi"
 
 msgctxt "model:production.bom.output,name:"
 msgid "Bill of Material Output"
-msgstr ""
+msgstr "BOM Çıktı"
 
 msgctxt "model:production.bom.tree,name:"
 msgid "BOM Tree"
-msgstr ""
+msgstr "BOM Ağacı"
 
 msgctxt "model:production.bom.tree.open.start,name:"
 msgid "Open BOM Tree"
-msgstr ""
+msgstr "BOM Ağacı Aç"
 
 msgctxt "model:production.bom.tree.open.tree,name:"
 msgid "Open BOM Tree"
-msgstr ""
+msgstr "BOM Ağacı"
 
 msgctxt "model:production.configuration,name:"
 msgid "Production Configuration"
-msgstr ""
+msgstr "Üretim Konfigurasyon"
 
 msgctxt "model:production.configuration.production_sequence,name:"
 msgid "Production Configuration Production Sequence"
-msgstr ""
+msgstr "Üretim Konfigurasyon Üretim Sırası"
 
 msgctxt "model:production.lead_time,name:"
 msgid "Production Lead Time"
-msgstr ""
+msgstr "Üretim Tedarik Sırası"
 
+#, fuzzy
 msgctxt "model:res.group,name:group_production"
 msgid "Production"
-msgstr ""
+msgstr "Production"
 
+#, fuzzy
 msgctxt "model:res.group,name:group_production_admin"
 msgid "Production Administration"
-msgstr ""
+msgstr "Production Administration"
 
+#, fuzzy
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
-msgstr ""
+msgstr "Production"
 
+#, fuzzy
 msgctxt "selection:ir.cron,method:"
 msgid "Assign Productions"
-msgstr "Atribuire Producţie"
+msgstr "Assign Production"
 
+#, fuzzy
 msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
-msgstr "Reprogramare Producţie"
+msgstr "Productions"
 
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
 msgstr ""
 
 msgctxt "selection:production,state:"
 msgid "Assigned"
-msgstr ""
+msgstr "Atanmış"
 
+#, fuzzy
 msgctxt "selection:production,state:"
 msgid "Cancelled"
-msgstr ""
+msgstr "Vazgeçilmiş"
 
 msgctxt "selection:production,state:"
 msgid "Done"
-msgstr ""
+msgstr "Yapılmış"
 
 msgctxt "selection:production,state:"
 msgid "Draft"
-msgstr ""
+msgstr "Taslak"
 
 msgctxt "selection:production,state:"
 msgid "Request"
-msgstr ""
+msgstr "Talep"
 
 msgctxt "selection:production,state:"
 msgid "Running"
-msgstr ""
+msgstr "Çalışan"
 
 msgctxt "selection:production,state:"
 msgid "Waiting"
-msgstr ""
+msgstr "Bekleyen"
 
 #, fuzzy
 msgctxt "view:product.template:"
 msgid "Production"
-msgstr "Produs"
+msgstr "Ürün"
 
 msgctxt "view:production.bom:"
 msgid "Lines"
-msgstr ""
+msgstr "Hatlar"
 
 msgctxt "view:production:"
 msgid "Lines"
-msgstr ""
+msgstr "Hatlar"
 
 msgctxt "view:production:"
 msgid "Other Info"
-msgstr ""
+msgstr "Diğer Bilgi"
 
 msgctxt "wizard_button:production.bom.tree.open,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "Vazgeç"
 
 msgctxt "wizard_button:production.bom.tree.open,start,tree:"
 msgid "OK"
-msgstr ""
+msgstr "Tamam"
 
 msgctxt "wizard_button:production.bom.tree.open,tree,end:"
 msgid "Close"
-msgstr ""
+msgstr "Kapat"
 
 msgctxt "wizard_button:production.bom.tree.open,tree,start:"
 msgid "Change"
-msgstr ""
+msgstr "Değiştir"
```

### Comparing `trytond_production-7.0.1/locale/ru.po` & `trytond_production-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/sl.po` & `trytond_production-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/tr.po` & `trytond_production-7.2.0/locale/ro.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,628 +1,605 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:product.product,boms:"
 msgid "BOMs"
-msgstr "BOMlar"
+msgstr "BOM-uri"
 
 msgctxt "field:product.product,producible:"
 msgid "Producible"
-msgstr "Üretilebilir"
+msgstr "Productibil"
 
-#, fuzzy
 msgctxt "field:product.product,production_lead_times:"
 msgid "Lead Times"
-msgstr "Tedarik Süreleri"
+msgstr "Timpi de livrare"
 
 msgctxt "field:product.product-production.bom,bom:"
 msgid "BOM"
 msgstr "BOM"
 
 msgctxt "field:product.product-production.bom,product:"
 msgid "Product"
-msgstr "Ürün"
+msgstr "Produs"
 
 msgctxt "field:product.template,producible:"
 msgid "Producible"
-msgstr "Üretilebilir"
+msgstr "Productibil"
 
-#, fuzzy
 msgctxt "field:production,assigned_by:"
 msgid "Assigned By"
-msgstr "Assigned"
+msgstr "Alocat de"
 
 msgctxt "field:production,bom:"
 msgid "BOM"
 msgstr "BOM"
 
 msgctxt "field:production,company:"
 msgid "Company"
-msgstr "Şirket"
+msgstr "Companie"
 
 msgctxt "field:production,cost:"
 msgid "Cost"
-msgstr "Maliyet"
+msgstr "Cost"
 
-#, fuzzy
 msgctxt "field:production,done_by:"
 msgid "Done By"
-msgstr "Done"
+msgstr "Făcut De"
 
 msgctxt "field:production,effective_start_date:"
 msgid "Effective Start Date"
-msgstr "Yürürlük Başlangıç Tarihi"
+msgstr "Data de începere efectivă"
 
 msgctxt "field:production,inputs:"
 msgid "Inputs"
-msgstr "Girdiler"
+msgstr "Intrări"
 
 msgctxt "field:production,location:"
 msgid "Location"
-msgstr "Lokasyon"
+msgstr "Locație"
 
 msgctxt "field:production,number:"
 msgid "Number"
-msgstr "Sayı"
+msgstr "Număr"
 
 msgctxt "field:production,origin:"
 msgid "Origin"
-msgstr ""
+msgstr "Origine"
 
 msgctxt "field:production,outputs:"
 msgid "Outputs"
-msgstr "Çıktılar"
+msgstr "Ieșiri"
 
-#, fuzzy
 msgctxt "field:production,partially_assigned:"
 msgid "Partially Assigned"
-msgstr "Assigned"
+msgstr "Parțial Alocat"
 
 msgctxt "field:production,planned_start_date:"
 msgid "Planned Start Date"
-msgstr "Planlanan Başlangıç Tarihi"
+msgstr "Data de începere planificată"
 
 msgctxt "field:production,product:"
 msgid "Product"
-msgstr "Ürün"
+msgstr "Produs"
 
 msgctxt "field:production,quantity:"
 msgid "Quantity"
-msgstr "Miktar"
+msgstr "Cantitate"
 
 msgctxt "field:production,reference:"
 msgid "Reference"
-msgstr "Referans"
+msgstr "Referinţă"
 
+#, fuzzy
 msgctxt "field:production,run_by:"
 msgid "Run By"
-msgstr ""
+msgstr "Condus de"
 
 msgctxt "field:production,state:"
 msgid "State"
-msgstr "Durum"
+msgstr "Stare"
 
-#, fuzzy
 msgctxt "field:production,unit:"
 msgid "Unit"
-msgstr "Birim"
+msgstr "Unitate"
 
-#, fuzzy
 msgctxt "field:production,uom_category:"
 msgid "UoM Category"
-msgstr "Ölçü Birimi Kategorisi"
+msgstr "Categorie UM"
 
 msgctxt "field:production,warehouse:"
 msgid "Warehouse"
-msgstr "Depo"
+msgstr "Depozit"
 
 msgctxt "field:production.bom,inputs:"
 msgid "Inputs"
-msgstr "Girdiler"
+msgstr "Intrări"
 
 msgctxt "field:production.bom,name:"
 msgid "Name"
-msgstr "Ad"
+msgstr "Nume"
 
 msgctxt "field:production.bom,output_products:"
 msgid "Output Products"
-msgstr "Çıktı Ürünler"
+msgstr "Produse de ieșire"
 
 msgctxt "field:production.bom,outputs:"
 msgid "Outputs"
-msgstr "Çıktılar"
+msgstr "Ieșiri"
 
 msgctxt "field:production.bom.input,bom:"
 msgid "BOM"
 msgstr "BOM"
 
 msgctxt "field:production.bom.input,product:"
 msgid "Product"
-msgstr "Ürün"
+msgstr "Produs"
 
 msgctxt "field:production.bom.input,quantity:"
 msgid "Quantity"
-msgstr "Miktar"
+msgstr "Cantitate"
 
-#, fuzzy
 msgctxt "field:production.bom.input,unit:"
 msgid "Unit"
-msgstr "Birim"
+msgstr "Unitate"
 
 msgctxt "field:production.bom.input,uom_category:"
 msgid "Uom Category"
-msgstr "Ölçü Birimi Kategorisi"
+msgstr "Categorie UM"
 
 msgctxt "field:production.bom.output,bom:"
 msgid "BOM"
 msgstr "BOM"
 
 msgctxt "field:production.bom.output,product:"
 msgid "Product"
-msgstr "Ürün"
+msgstr "Produs"
 
 msgctxt "field:production.bom.output,quantity:"
 msgid "Quantity"
-msgstr "Miktar"
+msgstr "Cantitate"
 
-#, fuzzy
 msgctxt "field:production.bom.output,unit:"
 msgid "Unit"
-msgstr "Birim"
+msgstr "Unitate"
 
 msgctxt "field:production.bom.output,uom_category:"
 msgid "Uom Category"
-msgstr "Ölçü Birimi Kategorisi"
+msgstr "Categorie UM"
 
 msgctxt "field:production.bom.tree,childs:"
 msgid "Childs"
-msgstr "Alt Elemanlar"
+msgstr ""
 
 msgctxt "field:production.bom.tree,product:"
 msgid "Product"
-msgstr "Ürün"
+msgstr "Produs"
 
 msgctxt "field:production.bom.tree,quantity:"
 msgid "Quantity"
-msgstr "Miktar"
+msgstr "Cantitate"
 
-#, fuzzy
 msgctxt "field:production.bom.tree,unit:"
 msgid "Unit"
-msgstr "Birim"
+msgstr "Unitate"
 
 msgctxt "field:production.bom.tree.open.start,bom:"
 msgid "BOM"
 msgstr "BOM"
 
 msgctxt "field:production.bom.tree.open.start,category:"
 msgid "Category"
-msgstr "Kategori"
+msgstr "Categorie"
 
 msgctxt "field:production.bom.tree.open.start,product:"
 msgid "Product"
-msgstr "Ürün"
+msgstr "Produs"
 
 msgctxt "field:production.bom.tree.open.start,quantity:"
 msgid "Quantity"
-msgstr "Miktar"
+msgstr "Cantitate"
 
-#, fuzzy
 msgctxt "field:production.bom.tree.open.start,unit:"
 msgid "Unit"
-msgstr "Birim"
+msgstr "Unitate"
 
 msgctxt "field:production.bom.tree.open.tree,bom_tree:"
 msgid "BOM Tree"
-msgstr "BOM Ağacı"
+msgstr "Arborele BOM"
 
 msgctxt "field:production.configuration,production_sequence:"
 msgid "Production Sequence"
-msgstr "Ürün Sırası"
+msgstr "Secvența de producție"
 
 msgctxt "field:production.configuration.production_sequence,company:"
 msgid "Company"
-msgstr "Şirket"
+msgstr "Companie"
 
 msgctxt ""
 "field:production.configuration.production_sequence,production_sequence:"
 msgid "Production Sequence"
-msgstr "Ürün Sırası"
+msgstr "Secvența de producție"
 
 msgctxt "field:production.lead_time,bom:"
 msgid "BOM"
 msgstr "BOM"
 
+#, fuzzy
 msgctxt "field:production.lead_time,lead_time:"
 msgid "Lead Time"
-msgstr "Tedarik Süresi"
+msgstr "Timp de livrare"
 
 msgctxt "field:production.lead_time,product:"
 msgid "Product"
-msgstr "Ürün"
+msgstr "Produs"
 
 msgctxt "field:stock.location,production_location:"
 msgid "Production"
-msgstr "Ürün"
+msgstr "Producţie"
 
 #, fuzzy
 msgctxt "field:stock.location,production_output_location:"
 msgid "Production Output"
-msgstr "Ürün Çıktısı"
+msgstr "Ieșire de producție"
 
 #, fuzzy
 msgctxt "field:stock.location,production_picking_location:"
 msgid "Production Picking"
-msgstr "Ürün"
+msgstr "Alegerea producției"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,production_input:"
 msgid "Production Input"
-msgstr "Ürün Girdisi"
+msgstr "Intrare de producție"
 
 #, fuzzy
 msgctxt "field:stock.lot.trace,production_output:"
 msgid "Production Output"
-msgstr "Ürün Çıktısı"
+msgstr "Ieșire de producție"
 
-#, fuzzy
 msgctxt "field:stock.move,production:"
 msgid "Production"
-msgstr "Ürün"
+msgstr "Producţie"
 
+#, fuzzy
 msgctxt "field:stock.move,production_cost_price_updated:"
 msgid "Cost Price Updated"
-msgstr ""
+msgstr "Preț actualizat"
 
+#, fuzzy
 msgctxt "field:stock.move,production_input:"
 msgid "Production Input"
-msgstr "Ürün Girdisi"
+msgstr "Intrare de producție"
 
+#, fuzzy
 msgctxt "field:stock.move,production_output:"
 msgid "Production Output"
-msgstr "Ürün Çıktısı"
+msgstr "Ieșire de producție"
 
 msgctxt "help:production,number:"
 msgid "The main identifier for the shipment."
-msgstr ""
+msgstr "Identificatorul principal pentru expediere."
 
 msgctxt "help:production,reference:"
 msgid "The external identifier for the shipment."
-msgstr ""
+msgstr "Identificatorul extern pentru expediere."
 
 msgctxt "help:production,uom_category:"
 msgid "The category of Unit of Measure."
-msgstr ""
+msgstr "Categoria de unitate de măsură."
 
 msgctxt "help:stock.location,production_output_location:"
 msgid ""
 "Where the produced goods are stored.\n"
 "Leave empty to use the warehouse storage location."
 msgstr ""
+"Unde sunt depozitate bunurile produse.\n"
+"Lăsați gol pentru a folosi locația de depozitare a depozitului."
 
 msgctxt "help:stock.location,production_picking_location:"
 msgid ""
 "Where the production components are picked from.\n"
 "Leave empty to use the warehouse storage location."
 msgstr ""
+"De unde se ridică componentele de producție.\n"
+"Lăsați gol pentru a folosi locația de depozitare a depozitului."
 
 msgctxt "model:ir.action,name:act_bom_form"
 msgid "BOM"
 msgstr "BOM"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_bom_list"
 msgid "BOMs"
-msgstr "BOMs"
+msgstr "BOM-uri"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_product_in_bom"
 msgid "BOMs"
-msgstr "BOMs"
+msgstr "BOM-uri"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_production_calendar"
 msgid "Productions"
-msgstr "Productions"
+msgstr "Producţie"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_production_configuration_form"
 msgid "Configuration"
-msgstr "Configuration"
+msgstr "Configurare"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_production_list"
 msgid "Productions"
-msgstr "Productions"
+msgstr "Producţie"
 
-#, fuzzy
 msgctxt "model:ir.action,name:wizard_bom_tree_open"
 msgid "BOM Tree"
-msgstr "BOM Tree"
+msgstr "Arborele BOM"
 
 #, fuzzy
 msgctxt "model:ir.action,name:wizard_production_assign"
 msgid "Assign Production"
-msgstr "Assign Production"
+msgstr "Alocare Producţie"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_product_in_bom_output_domain_input"
 msgid "As Inputs"
-msgstr "As Inputs"
+msgstr "Ca intrări"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_product_in_bom_output_domain_output"
 msgid "As Outputs"
-msgstr "As Outputs"
+msgstr "Ca Ieșiri"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_all"
 msgid "All"
-msgstr "All"
+msgstr "Tot"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_assigned"
 msgid "Assigned"
-msgstr "Assigned"
+msgstr "Alocat"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_available"
 msgid "Partially Assigned"
-msgstr "Assigned"
+msgstr "Parțial Alocat"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_draft"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciornă"
 
 #, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_requests"
 msgid "Requests"
-msgstr "Requests"
+msgstr "Cereri"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_running"
 msgid "Running"
-msgstr "Running"
+msgstr "În derulare"
 
-#, fuzzy
 msgctxt ""
 "model:ir.action.act_window.domain,name:act_production_list_domain_waiting"
 msgid "Waiting"
-msgstr "Waiting"
+msgstr "În Aşteptare"
 
-#, fuzzy
 msgctxt "model:ir.message,text:msg_missing_product_list_price"
 msgid ""
 "The product \"%(product)s\" on production \"%(production)s\" does not have "
 "any list price defined."
 msgstr ""
-"Üretim \"%(production)s\" çıktılarının (%(outputs)s) maliyetleri üretim "
-"(%(costs)s) maliyetleri ile uyuşmamaktadır."
+"Produsul \"%(product)s\" din producția \"%(production)s\" nu are niciun preț"
+" de listă definit."
 
 msgctxt "model:ir.message,text:msg_recursive_bom"
 msgid "You cannot create a recursive BOM for product \"%(product)s\"."
-msgstr ""
+msgstr "Nu puteți crea un BOM recursiv pentru produsul „%(product)s”."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_stock_move_production_single"
 msgid "Move can not be used for production input and output."
-msgstr ""
+msgstr "Mișcarea nu poate fi utilizată pentru intrarea și ieșirea producției."
 
+#, fuzzy
 msgctxt "model:ir.model.button,confirm:production_done_button"
 msgid "Are you sure you want to complete the production?"
-msgstr ""
+msgstr "Sunteți sigur că doriți să finalizați producția?"
 
 msgctxt "model:ir.model.button,string:production_assign_wizard_button"
 msgid "Assign"
-msgstr "Assign"
+msgstr "Alocare"
 
 msgctxt "model:ir.model.button,string:production_cancel_button"
 msgid "Cancel"
-msgstr "Cancel"
+msgstr "Anulare"
 
 msgctxt "model:ir.model.button,string:production_done_button"
 msgid "Done"
-msgstr "Done"
+msgstr "Terminat"
 
 msgctxt "model:ir.model.button,string:production_draft_button"
 msgid "Draft"
-msgstr "Draft"
+msgstr "Ciornă"
 
 msgctxt "model:ir.model.button,string:production_reset_bom_button"
 msgid "Reset to BOM"
-msgstr "Reset to BOM"
+msgstr "Resetați la BOM"
 
 msgctxt "model:ir.model.button,string:production_run_button"
 msgid "Run"
-msgstr "Run"
+msgstr "Rulează"
 
 msgctxt "model:ir.model.button,string:production_wait_button"
 msgid "Wait"
-msgstr "Wait"
+msgstr "Așteptare"
 
 msgctxt "model:ir.rule.group,name:rule_group_production_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "Utilizator în Companii"
 
-#, fuzzy
 msgctxt "model:ir.sequence,name:sequence_production"
 msgid "Production"
-msgstr "Production"
+msgstr "Producţie"
 
-#, fuzzy
 msgctxt "model:ir.sequence.type,name:sequence_type_production"
 msgid "Production"
-msgstr "Production"
+msgstr "Producţie"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_bom_list"
 msgid "BOMs"
-msgstr "BOMs"
+msgstr "BOM-uri"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configuration"
+msgstr "Configurare"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_production"
 msgid "Productions"
-msgstr "Productions"
+msgstr "Producţie"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_production_calendar"
 msgid "Productions"
-msgstr "Productions"
+msgstr "Producţie"
 
 #, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_production_configuration"
 msgid "Configuration"
-msgstr "Configuration"
+msgstr "Configurație"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_production_list"
 msgid "Productions"
-msgstr "Productions"
+msgstr "Producţie"
 
 msgctxt "model:product.product-production.bom,name:"
 msgid "Product - BOM"
-msgstr "Ürün - BOM"
+msgstr "Produs - BOM"
 
 msgctxt "model:production,name:"
 msgid "Production"
-msgstr "Üretim"
+msgstr "Producţie"
 
 msgctxt "model:production.bom,name:"
 msgid "Bill of Material"
-msgstr "BOM"
+msgstr "Lista materialelor"
 
 msgctxt "model:production.bom.input,name:"
 msgid "Bill of Material Input"
-msgstr "bOM Girdi"
+msgstr ""
 
 msgctxt "model:production.bom.output,name:"
 msgid "Bill of Material Output"
-msgstr "BOM Çıktı"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:production.bom.tree,name:"
 msgid "BOM Tree"
-msgstr "BOM Ağacı"
+msgstr "Arborele BOM"
 
 msgctxt "model:production.bom.tree.open.start,name:"
 msgid "Open BOM Tree"
-msgstr "BOM Ağacı Aç"
+msgstr "Deschideți arborele BOM"
 
 msgctxt "model:production.bom.tree.open.tree,name:"
 msgid "Open BOM Tree"
-msgstr "BOM Ağacı"
+msgstr "Deschideți arborele BOM"
 
 msgctxt "model:production.configuration,name:"
 msgid "Production Configuration"
-msgstr "Üretim Konfigurasyon"
+msgstr "Configurația producției"
 
+#, fuzzy
 msgctxt "model:production.configuration.production_sequence,name:"
 msgid "Production Configuration Production Sequence"
-msgstr "Üretim Konfigurasyon Üretim Sırası"
+msgstr "Configurația producției Secvența de producție"
 
 msgctxt "model:production.lead_time,name:"
 msgid "Production Lead Time"
-msgstr "Üretim Tedarik Sırası"
+msgstr ""
 
-#, fuzzy
 msgctxt "model:res.group,name:group_production"
 msgid "Production"
-msgstr "Production"
+msgstr "Producţie"
 
 #, fuzzy
 msgctxt "model:res.group,name:group_production_admin"
 msgid "Production Administration"
-msgstr "Production Administration"
+msgstr "Administrare producție"
 
-#, fuzzy
 msgctxt "model:stock.location,name:location_production"
 msgid "Production"
-msgstr "Production"
+msgstr "Producţie"
 
-#, fuzzy
 msgctxt "selection:ir.cron,method:"
 msgid "Assign Productions"
-msgstr "Assign Production"
+msgstr "Atribuire Producţie"
 
-#, fuzzy
 msgctxt "selection:ir.cron,method:"
 msgid "Reschedule Productions"
-msgstr "Productions"
+msgstr "Reprogramare Producţie"
 
+#, fuzzy
 msgctxt "selection:ir.cron,method:"
 msgid "Set Cost from Moves"
-msgstr ""
+msgstr "Setați costul din mișcări"
 
 msgctxt "selection:production,state:"
 msgid "Assigned"
-msgstr "Atanmış"
+msgstr "Alocat"
 
-#, fuzzy
 msgctxt "selection:production,state:"
 msgid "Cancelled"
-msgstr "Vazgeçilmiş"
+msgstr "Anulat"
 
 msgctxt "selection:production,state:"
 msgid "Done"
-msgstr "Yapılmış"
+msgstr "Terminat"
 
 msgctxt "selection:production,state:"
 msgid "Draft"
-msgstr "Taslak"
+msgstr "Ciornă"
 
+#, fuzzy
 msgctxt "selection:production,state:"
 msgid "Request"
-msgstr "Talep"
+msgstr "Cerere"
 
 msgctxt "selection:production,state:"
 msgid "Running"
-msgstr "Çalışan"
+msgstr "În derulare"
 
 msgctxt "selection:production,state:"
 msgid "Waiting"
-msgstr "Bekleyen"
+msgstr "În Aşteptare"
 
-#, fuzzy
 msgctxt "view:product.template:"
 msgid "Production"
-msgstr "Ürün"
+msgstr "Producţie"
 
 msgctxt "view:production.bom:"
 msgid "Lines"
-msgstr "Hatlar"
+msgstr "Rânduri"
 
 msgctxt "view:production:"
 msgid "Lines"
-msgstr "Hatlar"
+msgstr "Rânduri"
 
 msgctxt "view:production:"
 msgid "Other Info"
-msgstr "Diğer Bilgi"
+msgstr "Alte informații"
 
 msgctxt "wizard_button:production.bom.tree.open,start,end:"
 msgid "Cancel"
-msgstr "Vazgeç"
+msgstr "Anulare"
 
 msgctxt "wizard_button:production.bom.tree.open,start,tree:"
 msgid "OK"
-msgstr "Tamam"
+msgstr "OK"
 
 msgctxt "wizard_button:production.bom.tree.open,tree,end:"
 msgid "Close"
-msgstr "Kapat"
+msgstr "Închidere"
 
 msgctxt "wizard_button:production.bom.tree.open,tree,start:"
 msgid "Change"
-msgstr "Değiştir"
+msgstr "Schimbare"
```

### Comparing `trytond_production-7.0.1/locale/uk.po` & `trytond_production-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/locale/zh_CN.po` & `trytond_production-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/message.xml` & `trytond_production-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/product.py` & `trytond_production-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/product.xml` & `trytond_production-7.2.0/product.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_production-7.0.1/product.xml` & `trytond_production-7.2.0/product.xml`

```diff
@@ -15,22 +15,22 @@
     </record>
     <record model="ir.ui.view" id="product-bom_view_form">
       <field name="model">product.product-production.bom</field>
       <field name="type">form</field>
       <field name="name">product_bom_form</field>
     </record>
     <record model="ir.model.access" id="access_product-bom">
-      <field name="model" search="[('model', '=', 'product.product-production.bom')]"/>
+      <field name="model">product.product-production.bom</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_product-bom_admin">
-      <field name="model" search="[('model', '=', 'product.product-production.bom')]"/>
+      <field name="model">product.product-production.bom</field>
       <field name="group" ref="group_production_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="template_view_form">
@@ -60,22 +60,22 @@
     </record>
     <record model="ir.ui.view" id="production_lead_time_view_form">
       <field name="model">production.lead_time</field>
       <field name="type">form</field>
       <field name="name">production_lead_time_form</field>
     </record>
     <record model="ir.model.access" id="access_production_lead_time">
-      <field name="model" search="[('model', '=', 'production.lead_time')]"/>
+      <field name="model">production.lead_time</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_production_lead_time_admin">
-      <field name="model" search="[('model', '=', 'production.lead_time')]"/>
+      <field name="model">production.lead_time</field>
       <field name="group" ref="group_production_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_production-7.0.1/production.py` & `trytond_production-7.2.0/production.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 from collections import defaultdict
 from datetime import timedelta
 from decimal import Decimal
 from itertools import chain, groupby
 
+from sql import Null
 from sql.conditionals import Coalesce
 from sql.functions import CharLength
 
 from trytond.i18n import gettext
 from trytond.model import (
     Index, ModelSQL, ModelView, Workflow, dualmethod, fields)
 from trytond.modules.company.model import employee_field, set_employee
@@ -223,15 +224,15 @@
                             'tryton-forward')),
                     'depends': ['state'],
                     },
                 'run': {
                     'invisible': Eval('state') != 'assigned',
                     'depends': ['state'],
                     },
-                'done': {
+                'do': {
                     'invisible': Eval('state') != 'running',
                     'depends': ['state'],
                     },
                 'assign_wizard': {
                     'invisible': Eval('state') != 'waiting',
                     'depends': ['state'],
                     },
@@ -278,15 +279,17 @@
         cursor.execute(*table.update(
                 [table.state], ['cancelled'],
                 where=table.state == 'cancel'))
 
     @classmethod
     def order_number(cls, tables):
         table, _ = tables[None]
-        return [CharLength(table.number), table.number]
+        return [
+            ~((table.state == 'cancelled') & (table.number == Null)),
+            CharLength(table.number), table.number]
 
     @classmethod
     def order_effective_date(cls, tables):
         table, _ = tables[None]
         return [Coalesce(
                 table.effective_start_date, table.effective_date,
                 table.planned_start_date, table.planned_date)]
@@ -363,61 +366,56 @@
         pool = Pool()
         Move = pool.get('stock.move')
         assert type in {'input', 'output'}
         move = Move(
             product=product,
             unit=unit,
             quantity=quantity,
-            company=self.company,
-            currency=self.company.currency if self.company else None)
+            company=self.company)
         if type == 'input':
             move.from_location = self.picking_location
             move.to_location = self.location
             move.production_input = self
         else:
             move.from_location = self.location
             move.to_location = self.output_location
             move.production_output = self
-        return move
-
-    @fields.depends(methods=['_move'])
-    def _explode_move_values(self, type, bom_io, quantity):
-        move = self._move(type, bom_io.product, bom_io.unit, quantity)
-        move.unit_price_required = move.on_change_with_unit_price_required()
+        if move.on_change_with_unit_price_required():
+            move.unit_price = Decimal(0)
+            if self.company:
+                move.currency = self.company.currency
         return move
 
     @fields.depends(
-        'bom', 'product', 'unit', 'quantity', 'company', 'inputs', 'outputs',
-        methods=['_explode_move_values'])
+        'bom', 'product', 'unit', 'quantity', 'inputs', 'outputs',
+        methods=['_move'])
     def explode_bom(self):
         pool = Pool()
         Uom = pool.get('product.uom')
         if not (self.bom and self.product and self.unit):
             return
 
         factor = self.bom.compute_factor(
             self.product, self.quantity or 0, self.unit)
         inputs = []
         for input_ in self.bom.inputs:
             quantity = input_.compute_quantity(factor)
-            move = self._explode_move_values('input', input_, quantity)
+            move = self._move('input', input_.product, input_.unit, quantity)
             if move:
                 inputs.append(move)
                 quantity = Uom.compute_qty(
                     input_.unit, quantity, input_.product.default_uom,
                     round=False)
         self.inputs = inputs
 
         outputs = []
         for output in self.bom.outputs:
             quantity = output.compute_quantity(factor)
-            move = self._explode_move_values('output', output, quantity)
+            move = self._move('output', output.product, output.unit, quantity)
             if move:
-                move.unit_price = Decimal(0)
-                move.currency = self.company.currency
                 outputs.append(move)
         self.outputs = outputs
 
     @fields.depends('warehouse')
     def on_change_warehouse(self):
         self.location = None
         if self.warehouse:
@@ -495,16 +493,14 @@
         for production in productions:
             if not production.bom:
                 if production.product:
                     move = production._move(
                         'output', production.product, production.unit,
                         production.quantity)
                     if move:
-                        move.unit_price = Decimal(0)
-                        move.currency = production.company.currency
                         to_save.append(move)
                 continue
 
             factor = production.bom.compute_factor(
                 production.product, production.quantity, production.unit)
             for input_ in production.bom.inputs:
                 quantity = input_.compute_quantity(factor)
@@ -516,16 +512,14 @@
 
             for output in production.bom.outputs:
                 quantity = output.compute_quantity(factor)
                 product = output.product
                 move = production._move(
                     'output', product, output.unit, quantity)
                 if move:
-                    move.unit_price = Decimal(0)
-                    move.currency = production.company.currency
                     to_save.append(move)
         Move.save(to_save)
         cls._set_move_planned_date(productions)
 
     @classmethod
     def set_cost_from_moves(cls):
         pool = Pool()
@@ -630,25 +624,31 @@
                         or output.currency != production.company.currency):
                     output.unit_price = unit_price
                     output.currency = production.company.currency
                     moves.append(output)
         Move.save(moves)
 
     @classmethod
-    def create(cls, vlist):
-        Config = Pool().get('production.configuration')
+    def set_number(cls, productions):
+        '''
+        Fill the number field with the production sequence
+        '''
+        pool = Pool()
+        Config = pool.get('production.configuration')
 
-        vlist = [x.copy() for x in vlist]
         config = Config(1)
-        default_company = cls.default_company()
-        for values in vlist:
-            if values.get('number') is None:
-                values['number'] = config.get_multivalue(
+        for production in productions:
+            if not production.number:
+                production.number = config.get_multivalue(
                     'production_sequence',
-                    company=values.get('company', default_company)).get()
+                    company=production.company.id).get()
+        cls.save(productions)
+
+    @classmethod
+    def create(cls, vlist):
         productions = super(Production, cls).create(vlist)
         for production in productions:
             production._set_move_planned_date()
         return productions
 
     @classmethod
     def write(cls, *args):
@@ -725,14 +725,15 @@
         Move.delete(to_delete)
 
     @classmethod
     @ModelView.button
     @Workflow.transition('waiting')
     def wait(cls, productions):
         pool = Pool()
+        cls.set_number(productions)
         Move = pool.get('stock.move')
         Move.draft([m for p in productions
                 for m in p.inputs + p.outputs])
 
     @classmethod
     @Workflow.transition('assigned')
     @set_employee('assigned_by')
@@ -758,15 +759,15 @@
                     'effective_start_date': today,
                     })
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
     @set_employee('done_by')
-    def done(cls, productions):
+    def do(cls, productions):
         pool = Pool()
         Move = pool.get('stock.move')
         Date = pool.get('ir.date')
         cls.set_cost(productions)
         Move.do([m for p in productions for m in p.outputs])
         for company, productions in groupby(
                 productions, key=lambda p: p.company):
@@ -859,23 +860,23 @@
 
 class Production_Lot(metaclass=PoolMeta):
     __name__ = 'production'
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
-    def done(cls, productions):
+    def do(cls, productions):
         pool = Pool()
         Lot = pool.get('stock.lot')
         Move = pool.get('stock.move')
         lots, moves = [], []
         for production in productions:
             for move in production.outputs:
                 if not move.lot and move.product.lot_is_required(
                         move.from_location, move.to_location):
                     move.add_lot()
                     if move.lot:
                         lots.append(move.lot)
                         moves.append(move)
         Lot.save(lots)
         Move.save(moves)
-        super().done(productions)
+        super().do(productions)
```

### Comparing `trytond_production-7.0.1/production.xml` & `trytond_production-7.2.0/production.xml`

 * *Files 7% similar despite different names*

#### Comparing `trytond_production-7.0.1/production.xml` & `trytond_production-7.2.0/production.xml`

```diff
@@ -138,84 +138,84 @@
       <field name="group" ref="group_production_admin"/>
     </record>
     <record model="ir.sequence" id="sequence_production">
       <field name="name">Production</field>
       <field name="sequence_type" ref="sequence_type_production"/>
     </record>
     <record model="ir.model.access" id="access_production">
-      <field name="model" search="[('model', '=', 'production')]"/>
+      <field name="model">production</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_production_group_production">
-      <field name="model" search="[('model', '=', 'production')]"/>
+      <field name="model">production</field>
       <field name="group" ref="group_production"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_production_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'production')]"/>
+      <field name="model">production</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_production_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_production_companies"/>
     </record>
     <record model="ir.model.button" id="production_cancel_button">
+      <field name="model">production</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'production')]"/>
     </record>
     <record model="ir.model.button" id="production_draft_button">
+      <field name="model">production</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'production')]"/>
     </record>
     <record model="ir.model.button" id="production_wait_button">
+      <field name="model">production</field>
       <field name="name">wait</field>
       <field name="string">Wait</field>
-      <field name="model" search="[('model', '=', 'production')]"/>
     </record>
     <record model="ir.model.button" id="production_run_button">
+      <field name="model">production</field>
       <field name="name">run</field>
       <field name="string">Run</field>
-      <field name="model" search="[('model', '=', 'production')]"/>
     </record>
     <record model="ir.model.button" id="production_done_button">
-      <field name="name">done</field>
-      <field name="string">Done</field>
+      <field name="model">production</field>
+      <field name="name">do</field>
+      <field name="string">Complete</field>
       <field name="confirm">Are you sure you want to complete the production?</field>
-      <field name="model" search="[('model', '=', 'production')]"/>
     </record>
     <record model="ir.model.button" id="production_assign_try_button">
+      <field name="model">production</field>
       <field name="name">assign_try</field>
-      <field name="model" search="[('model', '=', 'production')]"/>
     </record>
     <record model="ir.model.button" id="production_assign_force_button">
+      <field name="model">production</field>
       <field name="name">assign_force</field>
-      <field name="model" search="[('model', '=', 'production')]"/>
     </record>
     <record model="ir.model.button-res.group" id="production_assign_force_button_group_production">
       <field name="button" ref="production_assign_force_button"/>
       <field name="group" ref="stock.group_stock_force_assignment"/>
     </record>
     <record model="ir.model.button" id="production_assign_wizard_button">
+      <field name="model">production</field>
       <field name="name">assign_wizard</field>
       <field name="string">Assign</field>
-      <field name="model" search="[('model', '=', 'production')]"/>
     </record>
     <record model="ir.model.button" id="production_reset_bom_button">
+      <field name="model">production</field>
       <field name="name">reset_bom</field>
       <field name="string">Reset to BOM</field>
-      <field name="model" search="[('model', '=', 'production')]"/>
     </record>
     <record model="ir.action.wizard" id="wizard_production_assign">
       <field name="name">Assign Production</field>
       <field name="wiz_name">stock.shipment.assign</field>
       <field name="model">production</field>
     </record>
     <record model="ir.cron" id="cron_set_cost_from_moves">
```

### Comparing `trytond_production-7.0.1/setup.py` & `trytond_production-7.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 import re
 from configparser import ConfigParser
 
 from setuptools import find_packages, setup
 
 
 def read(fname):
-    return io.open(
+    content = io.open(
         os.path.join(os.path.dirname(__file__), fname),
         'r', encoding='utf-8').read()
+    content = re.sub(
+        r'(?m)^\.\. toctree::\r?\n((^$|^\s.*$)\r?\n)*', '', content)
+    return content
 
 
 def get_require_version(name):
     require = '%s >= %s.%s, < %s.%s'
     require %= (name, major_version, minor_version,
         major_version, minor_version + 1)
     return require
@@ -58,15 +61,15 @@
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": 'https://docs.tryton.org/',
+        "Documentation": 'https://docs.tryton.org/products/modules-production',
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton production',
     package_dir={'trytond.modules.production': '.'},
     packages=(
         ['trytond.modules.production']
```

### Comparing `trytond_production-7.0.1/stock.py` & `trytond_production-7.2.0/stock.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,19 @@
         cls._sql_constraints += [
             ('production_single', Check(t, (
                         (t.production_input == Null)
                         | (t.production_output == Null))),
                 'production.msg_stock_move_production_single'),
             ]
 
+    @fields.depends('production_output', '_parent_production_output.company')
+    def on_change_production_output(self):
+        if self.production_output and self.production_output.company:
+            self.currency = self.production_output.company.currency
+
     @fields.depends(
         'production_input', '_parent_production_input.id',
         'production_output', '_parent_production_output.id')
     def on_change_with_production(self, name=None):
         if self.production_input:
             return self.production_input
         elif self.production_output:
```

### Comparing `trytond_production-7.0.1/stock.xml` & `trytond_production-7.2.0/stock.xml`

 * *Files 7% similar despite different names*

#### Comparing `trytond_production-7.0.1/stock.xml` & `trytond_production-7.2.0/stock.xml`

```diff
@@ -5,15 +5,15 @@
   <data>
     <record model="ir.ui.view" id="location_view_form">
       <field name="model">stock.location</field>
       <field name="inherit" ref="stock.location_view_form"/>
       <field name="name">location_form</field>
     </record>
     <record model="ir.model.access" id="access_move_group_production">
-      <field name="model" search="[('model', '=', 'stock.move')]"/>
+      <field name="model">stock.move</field>
       <field name="group" ref="group_production"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.action.keyword" id="wizard_open_product_quantities_by_warehouse_keyword_production">
```

### Comparing `trytond_production-7.0.1/tests/scenario_production.rst` & `trytond_production-7.2.0/tests/scenario_production.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Production Scenario
 ===================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, assertNotEqual
 
     >>> today = dt.date.today()
     >>> yesterday = today - dt.timedelta(days=1)
     >>> before_yesterday = yesterday - dt.timedelta(days=1)
 
 Activate modules::
 
@@ -125,88 +125,86 @@
 
     >>> Production = Model.get('production')
     >>> production = Production()
     >>> production.planned_date = today
     >>> production.product = product
     >>> production.bom = bom
     >>> production.quantity = 2
-    >>> production.planned_start_date == yesterday
-    True
-    >>> sorted([i.quantity for i in production.inputs]) == [10, 300]
-    True
+    >>> assertEqual(production.planned_start_date, yesterday)
+    >>> sorted([i.quantity for i in production.inputs])
+    [10.0, 300.0]
     >>> output, = production.outputs
-    >>> output.quantity == 2
-    True
+    >>> output.quantity
+    2.0
     >>> production.save()
     >>> production.cost
     Decimal('25.0000')
+    >>> production.number
     >>> production.click('wait')
     >>> production.state
     'waiting'
+    >>> assertNotEqual(production.number, None)
 
 Test reset bom button::
 
     >>> for input in production.inputs:
     ...     input.quantity += 1
     >>> production.click(
     ...     'reset_bom',
     ...     change=[
     ...         'bom', 'product', 'unit', 'quantity',
     ...         'inputs', 'outputs', 'company', 'warehouse', 'location'])
-    >>> sorted([i.quantity for i in production.inputs]) == [10, 300]
-    True
+    >>> sorted([i.quantity for i in production.inputs])
+    [10.0, 300.0]
     >>> output, = production.outputs
-    >>> output.quantity == 2
-    True
+    >>> output.quantity
+    2.0
 
 Do the production::
 
     >>> production.click('assign_try')
     >>> production.state
     'assigned'
-    >>> all(i.state == 'assigned' for i in production.inputs)
-    True
+    >>> {i.state for i in production.inputs}
+    {'assigned'}
     >>> production.click('run')
-    >>> all(i.state == 'done' for i in production.inputs)
-    True
-    >>> len(set(i.effective_date == today for i in production.inputs))
-    1
-    >>> production.click('done')
+    >>> {i.state for i in production.inputs}
+    {'done'}
+    >>> for input_ in production.inputs:
+    ...     assertEqual(input_.effective_date, today)
+    >>> production.click('do')
     >>> output, = production.outputs
     >>> output.state
     'done'
-    >>> output.effective_date == production.effective_date
-    True
+    >>> assertEqual(output.effective_date, production.effective_date)
     >>> output.unit_price
     Decimal('12.5000')
     >>> with config.set_context(locations=[storage.id]):
-    ...     Product(product.id).quantity == 2
-    True
+    ...     Product(product.id).quantity
+    2.0
 
 Make a production with effective date yesterday and running the day before::
 
     >>> Production = Model.get('production')
     >>> production = Production()
     >>> production.effective_date = yesterday
     >>> production.effective_start_date = before_yesterday
     >>> production.product = product
     >>> production.bom = bom
     >>> production.quantity = 2
     >>> production.click('wait')
     >>> production.click('assign_try')
     >>> production.click('run')
     >>> production.reload()
-    >>> all(i.effective_date == before_yesterday for i in production.inputs)
-    True
-    >>> production.click('done')
+    >>> for input_ in production.inputs:
+    ...     assertEqual(input_.effective_date, before_yesterday)
+    >>> production.click('do')
     >>> production.reload()
     >>> output, = production.outputs
-    >>> output.effective_date == yesterday
-    True
-
+    >>> assertEqual(output.effective_date, yesterday)
 
 Make a production with a bom of zero quantity::
 
     >>> zero_bom, = BOM.duplicate([bom])
     >>> for input_ in bom.inputs:
     ...     input_.quantity = 0.0
     >>> bom_output, = bom.outputs
@@ -228,9 +226,8 @@
     >>> production.click('wait')
     >>> Cron = Model.get('ir.cron')
     >>> cron = Cron(method='production|reschedule')
     >>> cron.interval_number = 1
     >>> cron.interval_type = 'months'
     >>> cron.click('run_once')
     >>> production.reload()
-    >>> production.planned_start_date == today
-    True
+    >>> assertEqual(production.planned_start_date, today)
```

### Comparing `trytond_production-7.0.1/tests/scenario_production_by_product.rst` & `trytond_production-7.2.0/tests/scenario_production_by_product.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ==========================
 Production with By-product
 ==========================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
 
 Activate modules::
 
     >>> config = activate_modules('production')
 
 Create company::
 
@@ -87,13 +87,13 @@
     >>> production = Production()
     >>> production.product = product
     >>> production.bom = bom
     >>> production.quantity = 4
     >>> production.click('wait')
     >>> production.click('assign_force')
     >>> production.click('run')
-    >>> production.click('done')
+    >>> production.click('do')
 
 Check output price::
 
     >>> sorted([o.unit_price for o in production.outputs])
     [Decimal('0'), Decimal('5.0000'), Decimal('15.0000')]
```

### Comparing `trytond_production-7.0.1/tests/scenario_production_lot_number.rst` & `trytond_production-7.2.0/tests/scenario_production_lot_number.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 ====================================
 
 Imports::
 
     >>> from decimal import Decimal
 
     >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
 
 Activate modules::
 
     >>> config = activate_modules(['stock_lot', 'production'])
 
     >>> ProductTemplate = Model.get('product.template')
     >>> Production = Model.get('production')
@@ -57,14 +56,14 @@
     >>> output.product = product
     >>> output.quantity = 1
     >>> output.unit_price = Decimal(0)
     >>> output.currency = production.company.currency
     >>> production.click('wait')
     >>> production.click('assign_force')
     >>> production.click('run')
-    >>> production.click('done')
+    >>> production.click('do')
     >>> production.state
     'done'
 
     >>> output, = production.outputs
     >>> bool(output.lot)
     True
```

### Comparing `trytond_production-7.0.1/tests/scenario_production_no_list_price.rst` & `trytond_production-7.2.0/tests/scenario_production_no_list_price.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 =============================
 Production without list price
 =============================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
 
 Activate modules::
 
     >>> config = activate_modules('production')
 
 Create company::
 
@@ -67,15 +67,15 @@
     >>> production.click('wait')
     >>> production.click('assign_force')
     >>> production.click('run')
     >>> output, = production.outputs
     >>> output.quantity = 2
     >>> output.save()
     >>> _ = output.duplicate()
-    >>> production.click('done')
+    >>> production.click('do')
 
 Check output price::
 
     >>> production.cost
     Decimal('40.0000')
     >>> sorted([o.unit_price for o in production.outputs])
     [Decimal('10.0000'), Decimal('10.0000')]
```

### Comparing `trytond_production-7.0.1/tests/scenario_production_rounding.rst` & `trytond_production-7.2.0/tests/scenario_production_rounding.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ============================
 Production Rounding Scenario
 ============================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
 
 Activate modules::
 
     >>> config = activate_modules('production')
 
 Create company::
```

### Comparing `trytond_production-7.0.1/tests/scenario_production_set_cost.rst` & `trytond_production-7.2.0/tests/scenario_production_set_cost.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ===================
 Production Set Cost
 ===================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
 
 Activate modules::
 
     >>> config = activate_modules('production')
 
 Create company::
 
@@ -70,15 +70,15 @@
     >>> output = production.outputs.new()
     >>> output.product = component
     >>> output.quantity = 2
     >>> output.unit_price = Decimal(0)
     >>> output.currency = company.currency
     >>> output.from_location = production.location
     >>> output.to_location = production.warehouse.storage_location
-    >>> production.click('done')
+    >>> production.click('do')
 
 Check output price::
 
     >>> production.cost
     Decimal('30.0000')
     >>> sorted([o.unit_price for o in production.outputs])
     [Decimal('5.0000'), Decimal('10.0000')]
```

### Comparing `trytond_production-7.0.1/tests/scenario_production_waste.rst` & `trytond_production-7.2.0/tests/scenario_production_waste.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 =========================
 Production Waste Scenario
 =========================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
 
 Activate modules::
 
     >>> config = activate_modules('production')
 
 Create company::
 
@@ -77,15 +77,15 @@
     >>> output.unit_price = Decimal('0')
     >>> output.currency = company.currency
     >>> waste_output = production.outputs.new()
     >>> waste_output.quantity = 1.0
     >>> waste_output.product = product
     >>> waste_output.from_location = production.location
     >>> waste_output.to_location = lost_found_loc
-    >>> production.click('done')
+    >>> production.click('do')
     >>> production.cost
     Decimal('20.0000')
     >>> output, = [o for o in production.outputs
     ...     if o.to_location.type != 'lost_found']
     >>> output.unit_price
     Decimal('20.0000')
     >>> waste_output, = [o for o in production.outputs
```

### Comparing `trytond_production-7.0.1/tests/test_module.py` & `trytond_production-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/tox.ini` & `trytond_production-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/trytond_production.egg-info/SOURCES.txt` & `trytond_production-7.2.0/trytond_production.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 bom.py
@@ -61,14 +60,15 @@
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_production.rst
 ./tests/scenario_production_by_product.rst
 ./tests/scenario_production_lot_number.rst
+./tests/scenario_production_lot_trace.rst
 ./tests/scenario_production_no_list_price.rst
 ./tests/scenario_production_rounding.rst
 ./tests/scenario_production_set_cost.rst
 ./tests/scenario_production_waste.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/bom_form.xml
@@ -92,15 +92,17 @@
 ./view/production_lead_time_list.xml
 ./view/production_lead_time_list_sequence.xml
 ./view/production_list.xml
 ./view/stock_move_form.xml
 ./view/template_form.xml
 ./view/template_list.xml
 doc/conf.py
+doc/design.rst
 doc/index.rst
+doc/releases.rst
 doc/requirements-doc.txt
 icons/LICENSE
 icons/tryton-production.svg
 locale/bg.po
 locale/ca.po
 locale/cs.po
 locale/de.po
@@ -124,14 +126,15 @@
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_production.rst
 tests/scenario_production_by_product.rst
 tests/scenario_production_lot_number.rst
+tests/scenario_production_lot_trace.rst
 tests/scenario_production_no_list_price.rst
 tests/scenario_production_rounding.rst
 tests/scenario_production_set_cost.rst
 tests/scenario_production_waste.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_production.egg-info/PKG-INFO
```

### Comparing `trytond_production-7.0.1/view/location_form.xml` & `trytond_production-7.2.0/view/location_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/view/production_form.xml` & `trytond_production-7.2.0/view/production_form.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_production-7.0.1/view/production_form.xml` & `trytond_production-7.2.0/view/production_form.xml`

```diff
@@ -52,10 +52,10 @@
   <group col="-1" colspan="2" id="buttons">
     <button name="cancel" icon="tryton-cancel"/>
     <button name="draft"/>
     <button name="reset_bom" icon="tryton-clear"/>
     <button name="wait"/>
     <button name="assign_wizard" icon="tryton-forward"/>
     <button name="run" icon="tryton-forward"/>
-    <button name="done" icon="tryton-forward"/>
+    <button name="do" icon="tryton-forward"/>
   </group>
 </form>
```

### Comparing `trytond_production-7.0.1/view/production_list.xml` & `trytond_production-7.2.0/view/production_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.0.1/view/template_form.xml` & `trytond_production-7.2.0/view/template_form.xml`

 * *Files identical despite different names*

