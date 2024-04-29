# Comparing `tmp/trytond_stock_consignment-7.0.0.tar.gz` & `tmp/trytond_stock_consignment-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_consignment-7.0.0.tar", last modified: Mon Oct 30 17:41:23 2023, max compression
+gzip compressed data, was "trytond_stock_consignment-7.2.0.tar", last modified: Mon Apr 29 15:50:50 2024, max compression
```

## Comparing `trytond_stock_consignment-7.0.0.tar` & `trytond_stock_consignment-7.2.0.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:23.188737 trytond_stock_consignment-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2023-10-22 17:23:23.000000 trytond_stock_consignment-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1317 2023-10-30 17:14:03.000000 trytond_stock_consignment-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:14:03.000000 trytond_stock_consignment-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_consignment-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4008 2023-10-30 17:41:23.188737 trytond_stock_consignment-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1209 2023-01-16 14:00:21.000000 trytond_stock_consignment-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      609 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      685 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.0.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:23.185404 trytond_stock_consignment-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2818 2023-10-22 17:23:23.000000 trytond_stock_consignment-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1209 2023-01-16 14:00:21.000000 trytond_stock_consignment-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:23.000000 trytond_stock_consignment-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:23.185404 trytond_stock_consignment-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      490 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      487 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      504 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-10-28 12:11:26.000000 trytond_stock_consignment-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:41:23.188737 trytond_stock_consignment-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4513 2023-10-27 17:38:49.000000 trytond_stock_consignment-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10711 2023-10-07 17:14:58.000000 trytond_stock_consignment-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:23.185404 trytond_stock_consignment-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8480 2023-10-07 17:14:58.000000 trytond_stock_consignment-7.0.0/tests/scenario_stock_consignment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5393 2023-08-13 15:26:13.000000 trytond_stock_consignment-7.0.0/tests/scenario_stock_consignment_supplier_customer.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_stock_consignment-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      216 2023-10-30 17:13:59.000000 trytond_stock_consignment-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:23.185404 trytond_stock_consignment-7.0.0/trytond_stock_consignment.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4008 2023-10-30 17:41:22.000000 trytond_stock_consignment-7.0.0/trytond_stock_consignment.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1700 2023-10-30 17:41:23.000000 trytond_stock_consignment-7.0.0/trytond_stock_consignment.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:41:22.000000 trytond_stock_consignment-7.0.0/trytond_stock_consignment.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-10-30 17:41:22.000000 trytond_stock_consignment-7.0.0/trytond_stock_consignment.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_stock_consignment-7.0.0/trytond_stock_consignment.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-10-30 17:41:22.000000 trytond_stock_consignment-7.0.0/trytond_stock_consignment.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:41:22.000000 trytond_stock_consignment-7.0.0/trytond_stock_consignment.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:23.185404 trytond_stock_consignment-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.0.0/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.0.0/view/stock_move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:50.526434 trytond_stock_consignment-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1418 2024-04-29 15:27:29.000000 trytond_stock_consignment-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:27:28.000000 trytond_stock_consignment-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_consignment-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4008 2024-04-29 15:50:50.523101 trytond_stock_consignment-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1209 2023-01-16 14:00:21.000000 trytond_stock_consignment-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      609 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      685 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.2.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:50.519767 trytond_stock_consignment-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-27 16:30:39.000000 trytond_stock_consignment-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1209 2023-01-16 14:00:21.000000 trytond_stock_consignment-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:31.000000 trytond_stock_consignment-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:50.523101 trytond_stock_consignment-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      490 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      487 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      504 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2024-04-29 13:17:17.000000 trytond_stock_consignment-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      458 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-27 16:43:27.000000 trytond_stock_consignment-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:50:50.526434 trytond_stock_consignment-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4513 2024-03-17 11:01:36.000000 trytond_stock_consignment-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10711 2024-02-04 18:51:26.000000 trytond_stock_consignment-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:50.523101 trytond_stock_consignment-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8480 2024-04-27 16:30:39.000000 trytond_stock_consignment-7.2.0/tests/scenario_stock_consignment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5366 2024-04-27 16:30:39.000000 trytond_stock_consignment-7.2.0/tests/scenario_stock_consignment_supplier_customer.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:31.000000 trytond_stock_consignment-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      216 2024-04-29 15:27:24.000000 trytond_stock_consignment-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:50.523101 trytond_stock_consignment-7.2.0/trytond_stock_consignment.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4008 2024-04-29 15:50:50.000000 trytond_stock_consignment-7.2.0/trytond_stock_consignment.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1682 2024-04-29 15:50:50.000000 trytond_stock_consignment-7.2.0/trytond_stock_consignment.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:50:50.000000 trytond_stock_consignment-7.2.0/trytond_stock_consignment.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-29 15:50:50.000000 trytond_stock_consignment-7.2.0/trytond_stock_consignment.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_stock_consignment-7.2.0/trytond_stock_consignment.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2024-04-29 15:50:50.000000 trytond_stock_consignment-7.2.0/trytond_stock_consignment.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:50:50.000000 trytond_stock_consignment-7.2.0/trytond_stock_consignment.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:50.523101 trytond_stock_consignment-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.2.0/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_stock_consignment-7.2.0/view/stock_move_form.xml
```

### Comparing `trytond_stock_consignment-7.0.0/CHANGELOG` & `trytond_stock_consignment-7.2.0/CHANGELOG`

 * *Files 11% similar despite different names*

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

### Comparing `trytond_stock_consignment-7.0.0/COPYRIGHT` & `trytond_stock_consignment-7.2.0/COPYRIGHT`

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

### Comparing `trytond_stock_consignment-7.0.0/LICENSE` & `trytond_stock_consignment-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-7.0.0/PKG-INFO` & `trytond_stock_consignment-7.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_consignment
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to manage consignment stock
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
@@ -48,25 +48,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_account_invoice_line_standalone<7.1,>=7.0
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_account_invoice_line_standalone<7.3,>=7.2
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_supply<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_supply<7.3,>=7.2; extra == "test"
 
 Stock Consignment Module
 ########################
 
 The stock consignment modules allow to manage consignment stock from supplier
 or at customer warehouse.
```

### Comparing `trytond_stock_consignment-7.0.0/README.rst` & `trytond_stock_consignment-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-7.0.0/__init__.py` & `trytond_stock_consignment-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-7.0.0/account.py` & `trytond_stock_consignment-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-7.0.0/doc/conf.py` & `trytond_stock_consignment-7.2.0/doc/conf.py`

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

### Comparing `trytond_stock_consignment-7.0.0/doc/index.rst` & `trytond_stock_consignment-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-7.0.0/locale/fa.po` & `trytond_stock_consignment-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-7.0.0/setup.py` & `trytond_stock_consignment-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-7.0.0/stock.py` & `trytond_stock_consignment-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-7.0.0/stock.xml` & `trytond_stock_consignment-7.2.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-7.0.0/tests/scenario_stock_consignment.rst` & `trytond_stock_consignment-7.2.0/tests/scenario_stock_consignment.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 Stock Consignment Scenario
 ==========================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts, create_tax
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_tax, get_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('stock_consignment')
 
 Create company::
 
@@ -122,15 +121,15 @@
     >>> move.to_location = supplier_consignment_loc
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_try')
     >>> shipment.state
     'assigned'
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
 Use supplier consignment stock::
 
     >>> shipment = Shipment()
     >>> shipment.from_location = supplier_consignment_loc
@@ -142,35 +141,31 @@
     >>> move.to_location = storage_loc
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_try')
     >>> shipment.state
     'assigned'
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
 Check supplier invoice line::
 
     >>> InvoiceLine = Model.get('account.invoice.line')
     >>> invoice_line, = InvoiceLine.find([('invoice_type', '=', 'in')])
-    >>> invoice_line.product == product
-    True
+    >>> assertEqual(invoice_line.product, product)
     >>> invoice_line.quantity
     4.0
-    >>> invoice_line.unit == unit
-    True
+    >>> assertEqual(invoice_line.unit, unit)
     >>> invoice_line.unit_price
     Decimal('4.0000')
-    >>> invoice_line.taxes == [supplier_tax]
-    True
+    >>> assertEqual(invoice_line.taxes, [supplier_tax])
     >>> move, = shipment.moves
-    >>> move.origin == invoice_line
-    True
+    >>> assertEqual(move.origin, invoice_line)
 
 Use supplier consignment stock for shipment out::
 
     >>> ShipmentOut = Model.get('stock.shipment.out')
     >>> shipment_out = ShipmentOut()
     >>> shipment_out.customer = customer
     >>> shipment_out.warehouse = warehouse_loc
@@ -203,15 +198,15 @@
     >>> move.to_location = customer_consignment_loc
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_try')
     >>> shipment.state
     'assigned'
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
 Use customer consignment stock::
 
     >>> shipment = Shipment()
     >>> shipment.from_location = customer_consignment_loc
@@ -223,34 +218,30 @@
     >>> move.to_location = customer_loc
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_try')
     >>> shipment.state
     'assigned'
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
 Check customer invoice line::
 
     >>> invoice_line, = InvoiceLine.find([('invoice_type', '=', 'out')])
-    >>> invoice_line.product == product
-    True
+    >>> assertEqual(invoice_line.product, product)
     >>> invoice_line.quantity
     1.0
-    >>> invoice_line.unit == unit
-    True
+    >>> assertEqual(invoice_line.unit, unit)
     >>> invoice_line.unit_price
     Decimal('10.0000')
-    >>> invoice_line.taxes == [customer_tax]
-    True
+    >>> assertEqual(invoice_line.taxes, [customer_tax])
     >>> move, = shipment.moves
-    >>> move.origin == invoice_line
-    True
+    >>> assertEqual(move.origin, invoice_line)
 
 Duplicate shipment clear origin::
 
     >>> duplicate, = shipment.duplicate()
     >>> move, = duplicate.moves
     >>> move.origin
```

### Comparing `trytond_stock_consignment-7.0.0/tests/scenario_stock_consignment_supplier_customer.rst` & `trytond_stock_consignment-7.2.0/tests/scenario_stock_consignment_supplier_customer.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 Stock Consignment Supplier to Customer Scenario
 ===============================================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts, create_tax
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('stock_consignment')
 
 Create company::
 
@@ -110,15 +108,15 @@
     >>> move.to_location = supplier_consignment_loc
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_try')
     >>> shipment.state
     'assigned'
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
 Use supplier consignment stock by customer::
 
     >>> shipment = Shipment()
     >>> shipment.from_location = supplier_consignment_loc
@@ -130,44 +128,38 @@
     >>> move.to_location = customer_loc
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_try')
     >>> shipment.state
     'assigned'
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
     >>> move, = shipment.moves
     >>> len(move.invoice_lines)
     2
     >>> move.origin in move.invoice_lines
     True
 
 Check supplier invoice line::
 
     >>> InvoiceLine = Model.get('account.invoice.line')
     >>> invoice_line, = InvoiceLine.find([('invoice_type', '=', 'in')])
-    >>> invoice_line.product == product
-    True
+    >>> assertEqual(invoice_line.product, product)
     >>> invoice_line.quantity
     4.0
-    >>> invoice_line.unit == unit
-    True
+    >>> assertEqual(invoice_line.unit, unit)
     >>> invoice_line.unit_price
     Decimal('4.0000')
-    >>> invoice_line.origin == move
-    True
+    >>> assertEqual(invoice_line.origin, move)
 
 Check customer invoice line::
 
     >>> invoice_line, = InvoiceLine.find([('invoice_type', '=', 'out')])
-    >>> invoice_line.product == product
-    True
+    >>> assertEqual(invoice_line.product, product)
     >>> invoice_line.quantity
     4.0
-    >>> invoice_line.unit == unit
-    True
+    >>> assertEqual(invoice_line.unit, unit)
     >>> invoice_line.unit_price
     Decimal('10.0000')
-    >>> invoice_line.origin == move
-    True
+    >>> assertEqual(invoice_line.origin, move)
```

### Comparing `trytond_stock_consignment-7.0.0/tox.ini` & `trytond_stock_consignment-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_consignment-7.0.0/trytond_stock_consignment.egg-info/PKG-INFO` & `trytond_stock_consignment-7.2.0/trytond_stock_consignment.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-stock-consignment
-Version: 7.0.0
+Name: trytond_stock_consignment
+Version: 7.2.0
 Summary: Tryton module to manage consignment stock
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
@@ -48,25 +48,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_account_invoice_line_standalone<7.1,>=7.0
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_account_invoice_line_standalone<7.3,>=7.2
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_supply<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_supply<7.3,>=7.2; extra == "test"
 
 Stock Consignment Module
 ########################
 
 The stock consignment modules allow to manage consignment stock from supplier
 or at customer warehouse.
```

### Comparing `trytond_stock_consignment-7.0.0/trytond_stock_consignment.egg-info/SOURCES.txt` & `trytond_stock_consignment-7.2.0/trytond_stock_consignment.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

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

