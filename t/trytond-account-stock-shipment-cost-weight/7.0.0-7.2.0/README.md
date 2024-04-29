# Comparing `tmp/trytond_account_stock_shipment_cost_weight-7.0.0.tar.gz` & `tmp/trytond_account_stock_shipment_cost_weight-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_stock_shipment_cost_weight-7.0.0.tar", last modified: Mon Oct 30 17:25:52 2023, max compression
+gzip compressed data, was "trytond_account_stock_shipment_cost_weight-7.2.0.tar", last modified: Mon Apr 29 15:37:04 2024, max compression
```

## Comparing `trytond_account_stock_shipment_cost_weight-7.0.0.tar` & `trytond_account_stock_shipment_cost_weight-7.2.0.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:52.400965 trytond_account_stock_shipment_cost_weight-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      249 2023-10-22 17:22:57.000000 trytond_account_stock_shipment_cost_weight-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-10-30 17:04:07.000000 trytond_account_stock_shipment_cost_weight-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:04:07.000000 trytond_account_stock_shipment_cost_weight-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2820 2023-10-30 17:25:52.400965 trytond_account_stock_shipment_cost_weight-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1246 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.0.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:52.397632 trytond_account_stock_shipment_cost_weight-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2835 2023-10-22 17:22:57.000000 trytond_account_stock_shipment_cost_weight-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:57.000000 trytond_account_stock_shipment_cost_weight-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:52.397632 trytond_account_stock_shipment_cost_weight-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      159 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      160 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      161 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      160 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      163 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      175 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      152 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost_weight-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:25:52.400965 trytond_account_stock_shipment_cost_weight-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4805 2023-10-27 17:38:49.000000 trytond_account_stock_shipment_cost_weight-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:52.397632 trytond_account_stock_shipment_cost_weight-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5378 2023-08-13 15:26:13.000000 trytond_account_stock_shipment_cost_weight-7.0.0/tests/scenario_account_stock_shipment_cost_weight.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_stock_shipment_cost_weight-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      108 2023-10-30 17:04:03.000000 trytond_account_stock_shipment_cost_weight-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:52.400965 trytond_account_stock_shipment_cost_weight-7.0.0/trytond_account_stock_shipment_cost_weight.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2820 2023-10-30 17:25:51.000000 trytond_account_stock_shipment_cost_weight-7.0.0/trytond_account_stock_shipment_cost_weight.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1616 2023-10-30 17:25:52.000000 trytond_account_stock_shipment_cost_weight-7.0.0/trytond_account_stock_shipment_cost_weight.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:25:51.000000 trytond_account_stock_shipment_cost_weight-7.0.0/trytond_account_stock_shipment_cost_weight.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      106 2023-10-30 17:25:51.000000 trytond_account_stock_shipment_cost_weight-7.0.0/trytond_account_stock_shipment_cost_weight.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_account_stock_shipment_cost_weight-7.0.0/trytond_account_stock_shipment_cost_weight.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      136 2023-10-30 17:25:51.000000 trytond_account_stock_shipment_cost_weight-7.0.0/trytond_account_stock_shipment_cost_weight.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:25:51.000000 trytond_account_stock_shipment_cost_weight-7.0.0/trytond_account_stock_shipment_cost_weight.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:04.648034 trytond_account_stock_shipment_cost_weight-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2024-04-29 15:17:06.000000 trytond_account_stock_shipment_cost_weight-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:17:06.000000 trytond_account_stock_shipment_cost_weight-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2811 2024-04-29 15:37:04.648034 trytond_account_stock_shipment_cost_weight-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1246 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.2.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:04.644701 trytond_account_stock_shipment_cost_weight-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3097 2024-04-27 16:30:39.000000 trytond_account_stock_shipment_cost_weight-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      278 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:02.000000 trytond_account_stock_shipment_cost_weight-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:04.648034 trytond_account_stock_shipment_cost_weight-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      159 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      160 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      161 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      160 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      163 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      175 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      152 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost_weight-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:37:04.648034 trytond_account_stock_shipment_cost_weight-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4796 2024-04-27 16:30:39.000000 trytond_account_stock_shipment_cost_weight-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:04.648034 trytond_account_stock_shipment_cost_weight-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5351 2024-04-27 16:30:39.000000 trytond_account_stock_shipment_cost_weight-7.2.0/tests/scenario_account_stock_shipment_cost_weight.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost_weight-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:02.000000 trytond_account_stock_shipment_cost_weight-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      108 2024-04-29 15:17:00.000000 trytond_account_stock_shipment_cost_weight-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:37:04.648034 trytond_account_stock_shipment_cost_weight-7.2.0/trytond_account_stock_shipment_cost_weight.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2811 2024-04-29 15:37:04.000000 trytond_account_stock_shipment_cost_weight-7.2.0/trytond_account_stock_shipment_cost_weight.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1598 2024-04-29 15:37:04.000000 trytond_account_stock_shipment_cost_weight-7.2.0/trytond_account_stock_shipment_cost_weight.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:37:04.000000 trytond_account_stock_shipment_cost_weight-7.2.0/trytond_account_stock_shipment_cost_weight.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      106 2024-04-29 15:37:04.000000 trytond_account_stock_shipment_cost_weight-7.2.0/trytond_account_stock_shipment_cost_weight.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_account_stock_shipment_cost_weight-7.2.0/trytond_account_stock_shipment_cost_weight.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      136 2024-04-29 15:37:04.000000 trytond_account_stock_shipment_cost_weight-7.2.0/trytond_account_stock_shipment_cost_weight.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:37:04.000000 trytond_account_stock_shipment_cost_weight-7.2.0/trytond_account_stock_shipment_cost_weight.egg-info/top_level.txt
```

### Comparing `trytond_account_stock_shipment_cost_weight-7.0.0/COPYRIGHT` & `trytond_account_stock_shipment_cost_weight-7.2.0/COPYRIGHT`

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

### Comparing `trytond_account_stock_shipment_cost_weight-7.0.0/LICENSE` & `trytond_account_stock_shipment_cost_weight-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost_weight-7.0.0/PKG-INFO` & `trytond_account_stock_shipment_cost_weight-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_shipment_cost_weight
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to allocate shipment cost per weight
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-stock-shipment-cost-weight
+Project-URL: Documentation, https://docs.tryton.org/modules-account-stock-shipment-cost-weight
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account stock shipment cost carrier weight
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,19 +47,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_stock_shipment_cost<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_measurements<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_stock_shipment_cost<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_measurements<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 #########################################
 Account Stock Shipment Cost Weight Module
 #########################################
 
 The *Account Stock Shipment Cost Weight Module* adds the "By Weight" as
 allocation method on shipment cost.
```

### Comparing `trytond_account_stock_shipment_cost_weight-7.0.0/account.py` & `trytond_account_stock_shipment_cost_weight-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost_weight-7.0.0/doc/conf.py` & `trytond_account_stock_shipment_cost_weight-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_stock_shipment_cost_weight-7.0.0/setup.py` & `trytond_account_stock_shipment_cost_weight-7.2.0/setup.py`

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
             'modules-account-stock-shipment-cost-weight'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account stock shipment cost carrier weight',
     package_dir={'trytond.modules.account_stock_shipment_cost_weight': '.'},
     packages=(
```

### Comparing `trytond_account_stock_shipment_cost_weight-7.0.0/tests/scenario_account_stock_shipment_cost_weight.rst` & `trytond_account_stock_shipment_cost_weight-7.2.0/tests/scenario_account_stock_shipment_cost_weight.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 ===========================================
 
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
 
     >>> config = activate_modules('account_stock_shipment_cost_weight')
 
@@ -109,26 +108,26 @@
     >>> move.to_location = customer_loc
     >>> move.unit_price = Decimal('100.00')
     >>> move.currency = company.currency
     >>> shipment1.click('wait')
     >>> shipment1.click('assign_force')
     >>> shipment1.click('pick')
     >>> shipment1.click('pack')
-    >>> shipment1.click('done')
+    >>> shipment1.click('do')
     >>> shipment1.state
     'done'
 
     >>> shipment2, = shipment1.duplicate()
     >>> move, = shipment2.outgoing_moves
     >>> move.quantity = 5
     >>> shipment2.click('wait')
     >>> shipment2.click('assign_force')
     >>> shipment2.click('pick')
     >>> shipment2.click('pack')
-    >>> shipment2.click('done')
+    >>> shipment2.click('do')
     >>> shipment2.state
     'done'
 
 Invoice shipment cost::
 
     >>> invoice = Invoice(type='in')
     >>> invoice.party = carrier
```

### Comparing `trytond_account_stock_shipment_cost_weight-7.0.0/tox.ini` & `trytond_account_stock_shipment_cost_weight-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost_weight-7.0.0/trytond_account_stock_shipment_cost_weight.egg-info/PKG-INFO` & `trytond_account_stock_shipment_cost_weight-7.2.0/trytond_account_stock_shipment_cost_weight.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-account-stock-shipment-cost-weight
-Version: 7.0.0
+Name: trytond_account_stock_shipment_cost_weight
+Version: 7.2.0
 Summary: Tryton module to allocate shipment cost per weight
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-stock-shipment-cost-weight
+Project-URL: Documentation, https://docs.tryton.org/modules-account-stock-shipment-cost-weight
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account stock shipment cost carrier weight
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,19 +47,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_stock_shipment_cost<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_measurements<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_stock_shipment_cost<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_measurements<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 #########################################
 Account Stock Shipment Cost Weight Module
 #########################################
 
 The *Account Stock Shipment Cost Weight Module* adds the "By Weight" as
 allocation method on shipment cost.
```

### Comparing `trytond_account_stock_shipment_cost_weight-7.0.0/trytond_account_stock_shipment_cost_weight.egg-info/SOURCES.txt` & `trytond_account_stock_shipment_cost_weight-7.2.0/trytond_account_stock_shipment_cost_weight.egg-info/SOURCES.txt`

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
