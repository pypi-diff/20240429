# Comparing `tmp/trytond_sale_shipment_grouping-7.0.0.tar.gz` & `tmp/trytond_sale_shipment_grouping-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_shipment_grouping-7.0.0.tar", last modified: Mon Oct 30 17:40:00 2023, max compression
+gzip compressed data, was "trytond_sale_shipment_grouping-7.2.0.tar", last modified: Mon Apr 29 15:49:41 2024, max compression
```

## Comparing `trytond_sale_shipment_grouping-7.0.0.tar` & `trytond_sale_shipment_grouping-7.2.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:00.305009 trytond_sale_shipment_grouping-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-22 17:23:21.000000 trytond_sale_shipment_grouping-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1815 2023-10-30 17:13:17.000000 trytond_sale_shipment_grouping-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      689 2023-10-30 17:13:17.000000 trytond_sale_shipment_grouping-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3016 2023-10-30 17:40:00.305009 trytond_sale_shipment_grouping-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1393 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-7.0.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-7.0.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:00.305009 trytond_sale_shipment_grouping-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2823 2023-10-22 17:23:21.000000 trytond_sale_shipment_grouping-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:21.000000 trytond_sale_shipment_grouping-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:00.301675 trytond_sale_shipment_grouping-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1474 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1769 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1399 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1795 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1817 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1742 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1733 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1959 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1399 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1912 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1802 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1420 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1863 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1873 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1411 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1772 2023-10-30 16:47:45.000000 trytond_sale_shipment_grouping-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1428 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1818 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1413 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1486 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1625 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1399 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1399 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1399 2023-10-28 12:11:25.000000 trytond_sale_shipment_grouping-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1567 2023-08-13 15:26:13.000000 trytond_sale_shipment_grouping-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3279 2023-10-24 07:57:53.000000 trytond_sale_shipment_grouping-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:40:00.305009 trytond_sale_shipment_grouping-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4432 2023-10-27 17:38:49.000000 trytond_sale_shipment_grouping-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:00.301675 trytond_sale_shipment_grouping-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5666 2023-08-13 15:26:13.000000 trytond_sale_shipment_grouping-7.0.0/tests/scenario_sale_shipment_grouping.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2888 2023-08-13 15:26:13.000000 trytond_sale_shipment_grouping-7.0.0/tests/scenario_sale_shipment_grouping_multiple.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2170 2023-08-13 15:26:13.000000 trytond_sale_shipment_grouping-7.0.0/tests/scenario_sale_shipment_grouping_return.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_shipment_grouping-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      117 2023-10-30 17:13:13.000000 trytond_sale_shipment_grouping-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:00.305009 trytond_sale_shipment_grouping-7.0.0/trytond_sale_shipment_grouping.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3016 2023-10-30 17:39:59.000000 trytond_sale_shipment_grouping-7.0.0/trytond_sale_shipment_grouping.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1905 2023-10-30 17:40:00.000000 trytond_sale_shipment_grouping-7.0.0/trytond_sale_shipment_grouping.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:39:59.000000 trytond_sale_shipment_grouping-7.0.0/trytond_sale_shipment_grouping.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-10-30 17:39:59.000000 trytond_sale_shipment_grouping-7.0.0/trytond_sale_shipment_grouping.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_sale_shipment_grouping-7.0.0/trytond_sale_shipment_grouping.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      115 2023-10-30 17:39:59.000000 trytond_sale_shipment_grouping-7.0.0/trytond_sale_shipment_grouping.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:39:59.000000 trytond_sale_shipment_grouping-7.0.0/trytond_sale_shipment_grouping.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:00.301675 trytond_sale_shipment_grouping-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      443 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-7.0.0/view/party_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:41.561571 trytond_sale_shipment_grouping-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1916 2024-04-29 15:26:38.000000 trytond_sale_shipment_grouping-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      689 2024-04-29 15:26:38.000000 trytond_sale_shipment_grouping-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3016 2024-04-29 15:49:41.561571 trytond_sale_shipment_grouping-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1393 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-7.2.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-7.2.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:41.558238 trytond_sale_shipment_grouping-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_sale_shipment_grouping-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:29.000000 trytond_sale_shipment_grouping-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:41.558238 trytond_sale_shipment_grouping-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1474 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1769 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1399 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1795 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1817 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1742 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1733 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1959 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1399 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1912 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1802 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1420 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1863 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1873 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1411 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1772 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1428 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1818 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1820 2024-04-29 13:17:17.000000 trytond_sale_shipment_grouping-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1486 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1625 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1399 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1399 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1399 2024-04-27 16:43:26.000000 trytond_sale_shipment_grouping-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1567 2024-01-27 09:58:52.000000 trytond_sale_shipment_grouping-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3282 2024-04-27 16:30:39.000000 trytond_sale_shipment_grouping-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:49:41.561571 trytond_sale_shipment_grouping-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4432 2024-03-17 11:01:36.000000 trytond_sale_shipment_grouping-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:41.558238 trytond_sale_shipment_grouping-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5605 2024-04-27 16:30:39.000000 trytond_sale_shipment_grouping-7.2.0/tests/scenario_sale_shipment_grouping.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2865 2024-04-22 12:14:36.000000 trytond_sale_shipment_grouping-7.2.0/tests/scenario_sale_shipment_grouping_multiple.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2140 2024-04-22 12:14:36.000000 trytond_sale_shipment_grouping-7.2.0/tests/scenario_sale_shipment_grouping_return.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_shipment_grouping-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:29.000000 trytond_sale_shipment_grouping-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      117 2024-04-29 15:26:34.000000 trytond_sale_shipment_grouping-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:41.561571 trytond_sale_shipment_grouping-7.2.0/trytond_sale_shipment_grouping.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3016 2024-04-29 15:49:41.000000 trytond_sale_shipment_grouping-7.2.0/trytond_sale_shipment_grouping.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1887 2024-04-29 15:49:41.000000 trytond_sale_shipment_grouping-7.2.0/trytond_sale_shipment_grouping.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:49:41.000000 trytond_sale_shipment_grouping-7.2.0/trytond_sale_shipment_grouping.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:49:41.000000 trytond_sale_shipment_grouping-7.2.0/trytond_sale_shipment_grouping.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_sale_shipment_grouping-7.2.0/trytond_sale_shipment_grouping.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      115 2024-04-29 15:49:41.000000 trytond_sale_shipment_grouping-7.2.0/trytond_sale_shipment_grouping.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:49:41.000000 trytond_sale_shipment_grouping-7.2.0/trytond_sale_shipment_grouping.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:41.561571 trytond_sale_shipment_grouping-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      443 2023-01-16 14:00:21.000000 trytond_sale_shipment_grouping-7.2.0/view/party_form.xml
```

### Comparing `trytond_sale_shipment_grouping-7.0.0/CHANGELOG` & `trytond_sale_shipment_grouping-7.2.0/CHANGELOG`

 * *Files 1% similar despite different names*

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

### Comparing `trytond_sale_shipment_grouping-7.0.0/COPYRIGHT` & `trytond_sale_shipment_grouping-7.2.0/COPYRIGHT`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Copyright (C) 2014-2023 Nicolas Évrard.
-Copyright (C) 2014-2023 B2CK SPRL.
+Copyright (C) 2014-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_shipment_grouping-7.0.0/LICENSE` & `trytond_sale_shipment_grouping-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/PKG-INFO` & `trytond_sale_shipment_grouping-7.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_shipment_grouping
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to group sale stock moves
 Home-page: http://www.tryton.org/
-Download-URL: http://dowloads.tryton.org/7.0/
+Download-URL: http://dowloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Shipment Grouping Module
 #############################
 
 The ``sale_shipment_grouping`` module adds an option to define how stock moves
 generated from sales will be grouped.
```

### Comparing `trytond_sale_shipment_grouping-7.0.0/configuration.py` & `trytond_sale_shipment_grouping-7.2.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/doc/conf.py` & `trytond_sale_shipment_grouping-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/bg.po` & `trytond_sale_shipment_grouping-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/ca.po` & `trytond_sale_shipment_grouping-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/cs.po` & `trytond_sale_shipment_grouping-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/de.po` & `trytond_sale_shipment_grouping-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/es.po` & `trytond_sale_shipment_grouping-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/es_419.po` & `trytond_sale_shipment_grouping-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/et.po` & `trytond_sale_shipment_grouping-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/fa.po` & `trytond_sale_shipment_grouping-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/fi.po` & `trytond_sale_shipment_grouping-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/fr.po` & `trytond_sale_shipment_grouping-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/hu.po` & `trytond_sale_shipment_grouping-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/id.po` & `trytond_sale_shipment_grouping-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/it.po` & `trytond_sale_shipment_grouping-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/lo.po` & `trytond_sale_shipment_grouping-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/lt.po` & `trytond_sale_shipment_grouping-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/nl.po` & `trytond_sale_shipment_grouping-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/pl.po` & `trytond_sale_shipment_grouping-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/pt.po` & `trytond_sale_shipment_grouping-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/ro.po` & `trytond_sale_shipment_grouping-7.2.0/locale/tr.po`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 msgctxt "field:party.party,sale_shipment_grouping_methods:"
 msgid "Sale Shipment Grouping Methods"
 msgstr ""
 
 msgctxt "field:party.party.sale_shipment_grouping_method,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt ""
 "field:party.party.sale_shipment_grouping_method,sale_shipment_grouping_method:"
 msgid "Sale Shipment Grouping Method"
 msgstr ""
 
 msgctxt "field:sale.configuration,sale_shipment_grouping_method:"
@@ -45,8 +45,8 @@
 
 msgctxt "selection:party.party,sale_shipment_grouping_method:"
 msgid "Standard"
 msgstr ""
 
 msgctxt "view:party.party:"
 msgid "Shipments"
-msgstr "Expedieri"
+msgstr ""
```

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/ru.po` & `trytond_sale_shipment_grouping-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/sl.po` & `trytond_sale_shipment_grouping-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/tr.po` & `trytond_sale_shipment_grouping-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/uk.po` & `trytond_sale_shipment_grouping-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/locale/zh_CN.po` & `trytond_sale_shipment_grouping-7.2.0/locale/ro.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
+#, fuzzy
 msgctxt "field:party.party,sale_shipment_grouping_method:"
 msgid "Sale Shipment Grouping Method"
-msgstr ""
+msgstr "Metoda de grupare a livrărilor de vânzare"
 
+#, fuzzy
 msgctxt "field:party.party,sale_shipment_grouping_methods:"
 msgid "Sale Shipment Grouping Methods"
-msgstr ""
+msgstr "Metode de grupare a livrărilor de vânzare"
 
 msgctxt "field:party.party.sale_shipment_grouping_method,party:"
 msgid "Party"
-msgstr ""
+msgstr "Parte"
 
+#, fuzzy
 msgctxt ""
 "field:party.party.sale_shipment_grouping_method,sale_shipment_grouping_method:"
 msgid "Sale Shipment Grouping Method"
-msgstr ""
+msgstr "Metoda de grupare a livrărilor de vânzare"
 
+#, fuzzy
 msgctxt "field:sale.configuration,sale_shipment_grouping_method:"
 msgid "Sale Shipment Grouping Method"
-msgstr ""
+msgstr "Metoda de grupare a livrărilor de vânzare"
 
+#, fuzzy
 msgctxt "field:sale.configuration.sale_method,sale_shipment_grouping_method:"
 msgid "Sale Shipment Grouping Method"
-msgstr ""
+msgstr "Metoda de grupare a livrărilor de vânzare"
 
 msgctxt "help:sale.configuration,sale_shipment_grouping_method:"
 msgid "The default shipment grouping method for new customers."
-msgstr ""
+msgstr "Metoda implicită de grupare a expedierilor pentru clienții noi."
 
 msgctxt "help:sale.configuration.sale_method,sale_shipment_grouping_method:"
 msgid "The default shipment grouping method for new customers."
-msgstr ""
+msgstr "Metoda implicită de grupare a expedierilor pentru clienții noi."
 
 msgctxt "model:party.party.sale_shipment_grouping_method,name:"
 msgid "Party Sale Shipment Grouping Method"
 msgstr ""
 
 msgctxt "selection:party.party,sale_shipment_grouping_method:"
 msgid "None"
-msgstr ""
+msgstr "Nici unul"
 
 msgctxt "selection:party.party,sale_shipment_grouping_method:"
 msgid "Standard"
-msgstr ""
+msgstr "Standard"
 
 msgctxt "view:party.party:"
 msgid "Shipments"
-msgstr ""
+msgstr "Expedieri"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `trytond_sale_shipment_grouping-7.0.0/party.py` & `trytond_sale_shipment_grouping-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/sale.py` & `trytond_sale_shipment_grouping-7.2.0/sale.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,37 +12,37 @@
 
     @property
     def shipment_grouping_method(self):
         return self.party.sale_shipment_grouping_method
 
     @property
     def _shipment_grouping_state(self):
-        return ['draft', 'waiting']
+        return {'draft', 'waiting'}
 
     def _get_shipment_grouping_fields(self, shipment):
         pool = Pool()
         ShipmentOut = pool.get('stock.shipment.out')
-        fields = ['customer', 'company', 'warehouse']
+        fields = {'customer', 'company', 'warehouse'}
         if isinstance(shipment, ShipmentOut):
-            fields.append('delivery_address')
+            fields.add('delivery_address')
         return fields
 
     def _get_grouped_shipment_planned_date(self, shipment):
         return [('planned_date', '=', shipment.planned_date)]
 
     def _get_grouped_shipment_order(self, Shipment):
         "Returns the order used to find shipments that should be grouped"
         return None
 
     def _get_grouped_shipment_domain(self, shipment):
         "Returns a domain that will find shipments that should be grouped"
         Shipment = shipment.__class__
         shipment_domain = [
             ('moves.origin', 'like', 'sale.line,%'),
-            ('state', 'in', self._shipment_grouping_state),
+            ('state', 'in', list(self._shipment_grouping_state)),
             ]
         shipment_domain += self._get_grouped_shipment_planned_date(shipment)
         fields = self._get_shipment_grouping_fields(shipment)
         defaults = Shipment.default_get(fields, with_rec_name=False)
         for field in fields:
             shipment_domain.append((field, '=',
                     getattr(shipment, field, defaults.get(field))))
```

### Comparing `trytond_sale_shipment_grouping-7.0.0/setup.py` & `trytond_sale_shipment_grouping-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/tests/scenario_sale_shipment_grouping.rst` & `trytond_sale_shipment_grouping-7.2.0/tests/scenario_sale_shipment_grouping.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 ===============================
 Sale Shipment Grouping Scenario
 ===============================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from operator import attrgetter
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
 
 Activate modules::
 
     >>> config = activate_modules('sale_shipment_grouping')
 
 Create company::
 
@@ -146,15 +145,15 @@
     >>> shipments = ShipmentOut.find([('customer', '=', customer.id)])
     >>> len(shipments)
     2
     >>> for shipment in shipments:
     ...     shipment.click('assign_try')
     ...     shipment.click('pick')
     ...     shipment.click('pack')
-    ...     shipment.click('done')
+    ...     shipment.click('do')
 
 Now we'll use the same scenario with the grouped customer::
 
     >>> set_user(sale_user)
     >>> sale = Sale()
     >>> sale.party = customer_grouped
     >>> sale.payment_term = payment_term
```

### Comparing `trytond_sale_shipment_grouping-7.0.0/tests/scenario_sale_shipment_grouping_multiple.rst` & `trytond_sale_shipment_grouping-7.2.0/tests/scenario_sale_shipment_grouping_multiple.rst`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 Sale Shipment Grouping Multiple Scenario
 ========================================
 
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
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('sale_shipment_grouping')
 
     >>> Party = Model.get('party.party')
     >>> ProductCategory = Model.get('product.category')
```

### Comparing `trytond_sale_shipment_grouping-7.0.0/tests/scenario_sale_shipment_grouping_return.rst` & `trytond_sale_shipment_grouping-7.2.0/tests/scenario_sale_shipment_grouping_return.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 ======================================
 Sale Shipment Grouping Return Scenario
 ======================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model
 
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
 
 Activate modules::
 
     >>> config = activate_modules('sale_shipment_grouping')
 
     >>> Party = Model.get('party.party')
     >>> ProductCategory = Model.get('product.category')
```

### Comparing `trytond_sale_shipment_grouping-7.0.0/tox.ini` & `trytond_sale_shipment_grouping-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_shipment_grouping-7.0.0/trytond_sale_shipment_grouping.egg-info/PKG-INFO` & `trytond_sale_shipment_grouping-7.2.0/trytond_sale_shipment_grouping.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-sale-shipment-grouping
-Version: 7.0.0
+Name: trytond_sale_shipment_grouping
+Version: 7.2.0
 Summary: Tryton module to group sale stock moves
 Home-page: http://www.tryton.org/
-Download-URL: http://dowloads.tryton.org/7.0/
+Download-URL: http://dowloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Shipment Grouping Module
 #############################
 
 The ``sale_shipment_grouping`` module adds an option to define how stock moves
 generated from sales will be grouped.
```

### Comparing `trytond_sale_shipment_grouping-7.0.0/trytond_sale_shipment_grouping.egg-info/SOURCES.txt` & `trytond_sale_shipment_grouping-7.2.0/trytond_sale_shipment_grouping.egg-info/SOURCES.txt`

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
 configuration.py
```

