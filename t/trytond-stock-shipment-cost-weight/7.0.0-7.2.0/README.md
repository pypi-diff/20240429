# Comparing `tmp/trytond_stock_shipment_cost_weight-7.0.0.tar.gz` & `tmp/trytond_stock_shipment_cost_weight-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_shipment_cost_weight-7.0.0.tar", last modified: Mon Oct 30 17:43:54 2023, max compression
+gzip compressed data, was "trytond_stock_shipment_cost_weight-7.2.0.tar", last modified: Mon Apr 29 15:53:00 2024, max compression
```

## Comparing `trytond_stock_shipment_cost_weight-7.0.0.tar` & `trytond_stock_shipment_cost_weight-7.2.0.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:54.949461 trytond_stock_shipment_cost_weight-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-10-22 17:23:27.000000 trytond_stock_shipment_cost_weight-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-10-30 17:15:30.000000 trytond_stock_shipment_cost_weight-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:15:29.000000 trytond_stock_shipment_cost_weight-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2801 2023-10-30 17:43:54.949461 trytond_stock_shipment_cost_weight-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.0.0/carrier.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:54.949461 trytond_stock_shipment_cost_weight-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2827 2023-10-22 17:23:27.000000 trytond_stock_shipment_cost_weight-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:27.000000 trytond_stock_shipment_cost_weight-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:54.949461 trytond_stock_shipment_cost_weight-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      159 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      160 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      161 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      160 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      162 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      175 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:26.000000 trytond_stock_shipment_cost_weight-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:43:54.949461 trytond_stock_shipment_cost_weight-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4713 2023-10-27 17:38:49.000000 trytond_stock_shipment_cost_weight-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1201 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.0.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:54.949461 trytond_stock_shipment_cost_weight-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3739 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.0.0/tests/scenario_stock_shipment_cost_weight.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_stock_shipment_cost_weight-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      107 2023-10-30 17:15:26.000000 trytond_stock_shipment_cost_weight-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:54.949461 trytond_stock_shipment_cost_weight-7.0.0/trytond_stock_shipment_cost_weight.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2801 2023-10-30 17:43:54.000000 trytond_stock_shipment_cost_weight-7.0.0/trytond_stock_shipment_cost_weight.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1564 2023-10-30 17:43:54.000000 trytond_stock_shipment_cost_weight-7.0.0/trytond_stock_shipment_cost_weight.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:43:54.000000 trytond_stock_shipment_cost_weight-7.0.0/trytond_stock_shipment_cost_weight.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:43:54.000000 trytond_stock_shipment_cost_weight-7.0.0/trytond_stock_shipment_cost_weight.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_stock_shipment_cost_weight-7.0.0/trytond_stock_shipment_cost_weight.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      154 2023-10-30 17:43:54.000000 trytond_stock_shipment_cost_weight-7.0.0/trytond_stock_shipment_cost_weight.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:43:54.000000 trytond_stock_shipment_cost_weight-7.0.0/trytond_stock_shipment_cost_weight.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:00.079712 trytond_stock_shipment_cost_weight-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2024-04-29 15:29:05.000000 trytond_stock_shipment_cost_weight-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:29:05.000000 trytond_stock_shipment_cost_weight-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2792 2024-04-29 15:53:00.079712 trytond_stock_shipment_cost_weight-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.2.0/carrier.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:00.076379 trytond_stock_shipment_cost_weight-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-27 16:30:39.000000 trytond_stock_shipment_cost_weight-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:36.000000 trytond_stock_shipment_cost_weight-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:00.076379 trytond_stock_shipment_cost_weight-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      159 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      160 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      161 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      160 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      162 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      175 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:28.000000 trytond_stock_shipment_cost_weight-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:53:00.079712 trytond_stock_shipment_cost_weight-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4704 2024-04-27 16:30:39.000000 trytond_stock_shipment_cost_weight-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1201 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.2.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:00.076379 trytond_stock_shipment_cost_weight-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3715 2024-04-27 16:30:39.000000 trytond_stock_shipment_cost_weight-7.2.0/tests/scenario_stock_shipment_cost_weight.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_shipment_cost_weight-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:36.000000 trytond_stock_shipment_cost_weight-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      107 2024-04-29 15:29:01.000000 trytond_stock_shipment_cost_weight-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:00.079712 trytond_stock_shipment_cost_weight-7.2.0/trytond_stock_shipment_cost_weight.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2792 2024-04-29 15:52:59.000000 trytond_stock_shipment_cost_weight-7.2.0/trytond_stock_shipment_cost_weight.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1546 2024-04-29 15:53:00.000000 trytond_stock_shipment_cost_weight-7.2.0/trytond_stock_shipment_cost_weight.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:52:59.000000 trytond_stock_shipment_cost_weight-7.2.0/trytond_stock_shipment_cost_weight.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-29 15:52:59.000000 trytond_stock_shipment_cost_weight-7.2.0/trytond_stock_shipment_cost_weight.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_stock_shipment_cost_weight-7.2.0/trytond_stock_shipment_cost_weight.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      154 2024-04-29 15:52:59.000000 trytond_stock_shipment_cost_weight-7.2.0/trytond_stock_shipment_cost_weight.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:52:59.000000 trytond_stock_shipment_cost_weight-7.2.0/trytond_stock_shipment_cost_weight.egg-info/top_level.txt
```

### Comparing `trytond_stock_shipment_cost_weight-7.0.0/COPYRIGHT` & `trytond_stock_shipment_cost_weight-7.2.0/COPYRIGHT`

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

### Comparing `trytond_stock_shipment_cost_weight-7.0.0/LICENSE` & `trytond_stock_shipment_cost_weight-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost_weight-7.0.0/PKG-INFO` & `trytond_stock_shipment_cost_weight-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_stock_shipment_cost_weight
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to allocate shipment cost "by weight"
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-shipment-cost-weight
+Project-URL: Documentation, https://docs.tryton.org/modules-stock-shipment-cost-weight
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock shipment cost weight
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,20 +47,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_cost<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_measurements<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_cost<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_measurements<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 #################################
 Stock Shipment Cost Weight Module
 #################################
 
 The *Stock Shipment Cost Weight Module* adds "By Weight" as allocation method of
 shipment cost on the carrier.
```

### Comparing `trytond_stock_shipment_cost_weight-7.0.0/doc/conf.py` & `trytond_stock_shipment_cost_weight-7.2.0/doc/conf.py`

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

### Comparing `trytond_stock_shipment_cost_weight-7.0.0/setup.py` & `trytond_stock_shipment_cost_weight-7.2.0/setup.py`

 * *Files 1% similar despite different names*

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
             'modules-stock-shipment-cost-weight'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock shipment cost weight',
     package_dir={'trytond.modules.stock_shipment_cost_weight': '.'},
     packages=(
```

### Comparing `trytond_stock_shipment_cost_weight-7.0.0/stock.py` & `trytond_stock_shipment_cost_weight-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost_weight-7.0.0/tests/scenario_stock_shipment_cost_weight.rst` & `trytond_stock_shipment_cost_weight-7.2.0/tests/scenario_stock_shipment_cost_weight.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ===================================
 Stock Shipment Cost Weight Scenario
 ===================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+    >>> from unittest.mock import patch
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.modules.stock_shipment_cost.stock import ShipmentCostMixin
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
 
 Patch _get_shipment_cost::
 
-    >>> from unittest.mock import patch
-    >>> from trytond.modules.stock_shipment_cost.stock import ShipmentCostMixin
     >>> mock = patch.object(
     ...     ShipmentCostMixin, '_get_shipment_cost',
     ...     return_value=Decimal('8')).start()
 
 Activate modules::
 
     >>> config = activate_modules('stock_shipment_cost_weight')
@@ -106,15 +106,15 @@
     >>> move.to_location = customer_loc
     >>> move.unit_price = Decimal('40')
     >>> move.currency = company.currency
     >>> shipment.click('wait')
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
 Check move costs::
 
     >>> sorted([
     ...         (m.cost_price, m.shipment_out_cost_price)
```

### Comparing `trytond_stock_shipment_cost_weight-7.0.0/tox.ini` & `trytond_stock_shipment_cost_weight-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_shipment_cost_weight-7.0.0/trytond_stock_shipment_cost_weight.egg-info/PKG-INFO` & `trytond_stock_shipment_cost_weight-7.2.0/trytond_stock_shipment_cost_weight.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-stock-shipment-cost-weight
-Version: 7.0.0
+Name: trytond_stock_shipment_cost_weight
+Version: 7.2.0
 Summary: Tryton module to allocate shipment cost "by weight"
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-shipment-cost-weight
+Project-URL: Documentation, https://docs.tryton.org/modules-stock-shipment-cost-weight
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock shipment cost weight
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,20 +47,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_carrier<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_cost<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_measurements<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_carrier<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_cost<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_measurements<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 #################################
 Stock Shipment Cost Weight Module
 #################################
 
 The *Stock Shipment Cost Weight Module* adds "By Weight" as allocation method of
 shipment cost on the carrier.
```

### Comparing `trytond_stock_shipment_cost_weight-7.0.0/trytond_stock_shipment_cost_weight.egg-info/SOURCES.txt` & `trytond_stock_shipment_cost_weight-7.2.0/trytond_stock_shipment_cost_weight.egg-info/SOURCES.txt`

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
 carrier.py
```
