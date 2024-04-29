# Comparing `tmp/trytond_sale_shipment_tolerance-7.0.0.tar.gz` & `tmp/trytond_sale_shipment_tolerance-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_shipment_tolerance-7.0.0.tar", last modified: Mon Oct 30 17:40:08 2023, max compression
+gzip compressed data, was "trytond_sale_shipment_tolerance-7.2.0.tar", last modified: Mon Apr 29 15:49:47 2024, max compression
```

## Comparing `trytond_sale_shipment_tolerance-7.0.0.tar` & `trytond_sale_shipment_tolerance-7.2.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:08.691716 trytond_sale_shipment_tolerance-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-10-22 17:23:21.000000 trytond_sale_shipment_tolerance-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1221 2023-10-30 17:13:22.000000 trytond_sale_shipment_tolerance-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:13:21.000000 trytond_sale_shipment_tolerance-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_shipment_tolerance-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2808 2023-10-30 17:40:08.691716 trytond_sale_shipment_tolerance-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-01-16 14:00:21.000000 trytond_sale_shipment_tolerance-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2585 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.0.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:21.000000 trytond_sale_shipment_tolerance-7.0.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:08.691716 trytond_sale_shipment_tolerance-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2824 2023-10-22 17:23:21.000000 trytond_sale_shipment_tolerance-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-01-16 14:00:21.000000 trytond_sale_shipment_tolerance-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:21.000000 trytond_sale_shipment_tolerance-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:08.688382 trytond_sale_shipment_tolerance-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2124 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2050 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2089 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1539 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1540 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2220 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2099 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1540 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2128 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2051 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1540 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2089 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1539 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1540 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1539 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1549 2023-10-28 12:11:25.000000 trytond_sale_shipment_tolerance-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2925 2023-10-07 17:14:58.000000 trytond_sale_shipment_tolerance-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:40:08.691716 trytond_sale_shipment_tolerance-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4409 2023-10-27 17:38:49.000000 trytond_sale_shipment_tolerance-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      895 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.0.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:08.688382 trytond_sale_shipment_tolerance-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3281 2023-10-27 17:38:49.000000 trytond_sale_shipment_tolerance-7.0.0/tests/scenario_sale_over_shipment_tolerance.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2846 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.0.0/tests/scenario_sale_under_shipment_tolerance.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_shipment_tolerance-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      101 2023-10-30 17:13:18.000000 trytond_sale_shipment_tolerance-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:08.691716 trytond_sale_shipment_tolerance-7.0.0/trytond_sale_shipment_tolerance.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2808 2023-10-30 17:40:08.000000 trytond_sale_shipment_tolerance-7.0.0/trytond_sale_shipment_tolerance.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1812 2023-10-30 17:40:08.000000 trytond_sale_shipment_tolerance-7.0.0/trytond_sale_shipment_tolerance.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:40:08.000000 trytond_sale_shipment_tolerance-7.0.0/trytond_sale_shipment_tolerance.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-10-30 17:40:08.000000 trytond_sale_shipment_tolerance-7.0.0/trytond_sale_shipment_tolerance.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_sale_shipment_tolerance-7.0.0/trytond_sale_shipment_tolerance.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       91 2023-10-30 17:40:08.000000 trytond_sale_shipment_tolerance-7.0.0/trytond_sale_shipment_tolerance.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:40:08.000000 trytond_sale_shipment_tolerance-7.0.0/trytond_sale_shipment_tolerance.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:08.691716 trytond_sale_shipment_tolerance-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1023 2023-01-16 14:00:21.000000 trytond_sale_shipment_tolerance-7.0.0/view/configuration_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:47.481416 trytond_sale_shipment_tolerance-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1322 2024-04-29 15:26:43.000000 trytond_sale_shipment_tolerance-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:26:43.000000 trytond_sale_shipment_tolerance-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_shipment_tolerance-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2808 2024-04-29 15:49:47.481416 trytond_sale_shipment_tolerance-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-01-16 14:00:21.000000 trytond_sale_shipment_tolerance-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2585 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:21.000000 trytond_sale_shipment_tolerance-7.2.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:47.478083 trytond_sale_shipment_tolerance-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-27 16:30:39.000000 trytond_sale_shipment_tolerance-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-01-16 14:00:21.000000 trytond_sale_shipment_tolerance-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:29.000000 trytond_sale_shipment_tolerance-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:47.478083 trytond_sale_shipment_tolerance-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:26.000000 trytond_sale_shipment_tolerance-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2124 2024-04-27 16:43:26.000000 trytond_sale_shipment_tolerance-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2050 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2089 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1539 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1540 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2220 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2099 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1540 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2128 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2051 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1540 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2089 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1539 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1540 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1539 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-27 16:43:27.000000 trytond_sale_shipment_tolerance-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2925 2024-02-04 18:51:26.000000 trytond_sale_shipment_tolerance-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:49:47.481416 trytond_sale_shipment_tolerance-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4409 2024-03-17 11:01:36.000000 trytond_sale_shipment_tolerance-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      895 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:47.478083 trytond_sale_shipment_tolerance-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3215 2024-04-27 16:30:39.000000 trytond_sale_shipment_tolerance-7.2.0/tests/scenario_sale_over_shipment_tolerance.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2807 2024-04-27 16:30:39.000000 trytond_sale_shipment_tolerance-7.2.0/tests/scenario_sale_under_shipment_tolerance.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_shipment_tolerance-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:29.000000 trytond_sale_shipment_tolerance-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      101 2024-04-29 15:26:39.000000 trytond_sale_shipment_tolerance-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:47.481416 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2808 2024-04-29 15:49:47.000000 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1794 2024-04-29 15:49:47.000000 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:49:47.000000 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-04-29 15:49:47.000000 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       91 2024-04-29 15:49:47.000000 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:49:47.000000 trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:47.481416 trytond_sale_shipment_tolerance-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1023 2023-01-16 14:00:21.000000 trytond_sale_shipment_tolerance-7.2.0/view/configuration_form.xml
```

### Comparing `trytond_sale_shipment_tolerance-7.0.0/CHANGELOG` & `trytond_sale_shipment_tolerance-7.2.0/CHANGELOG`

 * *Files 6% similar despite different names*

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

### Comparing `trytond_sale_shipment_tolerance-7.0.0/COPYRIGHT` & `trytond_sale_shipment_tolerance-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2017-2023 Cédric Krier
-Copyright (C) 2017-2023 B2CK
+Copyright (C) 2017-2024 Cédric Krier
+Copyright (C) 2017-2024 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_shipment_tolerance-7.0.0/LICENSE` & `trytond_sale_shipment_tolerance-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/PKG-INFO` & `trytond_sale_shipment_tolerance-7.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_shipment_tolerance
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to define tolerance for sale shipment
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
@@ -45,19 +45,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Shipment Tolerance Module
 ##############################
 
 The sale_shipment_tolerance modules adds under and over shipment tolerance on
 the sale.
 If the quantity of a sale line is under shipped but inside the tolerance
```

### Comparing `trytond_sale_shipment_tolerance-7.0.0/configuration.py` & `trytond_sale_shipment_tolerance-7.2.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/doc/conf.py` & `trytond_sale_shipment_tolerance-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/bg.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/ca.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/cs.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/de.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/es.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/es_419.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/et.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/fa.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/fi.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/fr.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/hu.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/id.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/it.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/lo.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/lt.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/nl.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/pl.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/pt.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/ro.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/ru.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/sl.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/tr.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/uk.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/locale/zh_CN.po` & `trytond_sale_shipment_tolerance-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/sale.py` & `trytond_sale_shipment_tolerance-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/setup.py` & `trytond_sale_shipment_tolerance-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/stock.py` & `trytond_sale_shipment_tolerance-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/tests/scenario_sale_over_shipment_tolerance.rst` & `trytond_sale_shipment_tolerance-7.2.0/tests/scenario_sale_over_shipment_tolerance.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 =====================================
 Sale Over Shipment Tolerance Scenario
 =====================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
 
 Activate modules::
 
     >>> config = activate_modules('sale_shipment_tolerance')
 
 Create company::
 
@@ -80,15 +79,15 @@
     >>> shipment, = sale.shipments
     >>> shipment.click('draft')
     >>> move, = shipment.outgoing_moves
     >>> move.quantity = 13
     >>> shipment.click('wait')
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
-    >>> shipment.click('pack')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> shipment.click('pack')
     Traceback (most recent call last):
         ...
     OverShipmentWarning: ...
 
 Cancel shipment and recreate::
 
     >>> shipment.click('cancel')
@@ -104,14 +103,14 @@
     >>> shipment.click('draft')
     >>> move, = shipment.outgoing_moves
     >>> move.quantity = 12
     >>> shipment.click('wait')
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
 
 No new shipment as shipped inside tolerance::
 
     >>> sale.reload()
     >>> len(sale.shipments)
     2
```

### Comparing `trytond_sale_shipment_tolerance-7.0.0/tests/scenario_sale_under_shipment_tolerance.rst` & `trytond_sale_shipment_tolerance-7.2.0/tests/scenario_sale_under_shipment_tolerance.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 ======================================
 Sale Under Shipment Tolerance Scenario
 ======================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
 
 Activate modules::
 
     >>> config = activate_modules('sale_shipment_tolerance')
 
 Create company::
 
@@ -79,26 +78,26 @@
 
     >>> shipment, = sale.shipments
     >>> move, = shipment.inventory_moves
     >>> move.quantity = 5
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
 
 Under ship 4 products::
 
     >>> sale.reload()
     >>> _, shipment = sale.shipments
     >>> move, = shipment.inventory_moves
     >>> move.quantity = 4
     >>> shipment.click('assign_force')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
 
 No new shipment as shipped inside tolerance::
 
     >>> sale.reload()
     >>> len(sale.shipments)
     2
     >>> sale.shipment_state
```

### Comparing `trytond_sale_shipment_tolerance-7.0.0/tox.ini` & `trytond_sale_shipment_tolerance-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_tolerance-7.0.0/trytond_sale_shipment_tolerance.egg-info/PKG-INFO` & `trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-sale-shipment-tolerance
-Version: 7.0.0
+Name: trytond_sale_shipment_tolerance
+Version: 7.2.0
 Summary: Tryton module to define tolerance for sale shipment
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
@@ -45,19 +45,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Shipment Tolerance Module
 ##############################
 
 The sale_shipment_tolerance modules adds under and over shipment tolerance on
 the sale.
 If the quantity of a sale line is under shipped but inside the tolerance
```

### Comparing `trytond_sale_shipment_tolerance-7.0.0/trytond_sale_shipment_tolerance.egg-info/SOURCES.txt` & `trytond_sale_shipment_tolerance-7.2.0/trytond_sale_shipment_tolerance.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 configuration.py
```

### Comparing `trytond_sale_shipment_tolerance-7.0.0/view/configuration_form.xml` & `trytond_sale_shipment_tolerance-7.2.0/view/configuration_form.xml`

 * *Files identical despite different names*

