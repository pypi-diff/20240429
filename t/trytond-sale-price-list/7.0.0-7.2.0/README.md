# Comparing `tmp/trytond_sale_price_list-7.0.0.tar.gz` & `tmp/trytond_sale_price_list-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_price_list-7.0.0.tar", last modified: Mon Oct 30 17:38:51 2023, max compression
+gzip compressed data, was "trytond_sale_price_list-7.2.0.tar", last modified: Mon Apr 29 15:48:41 2024, max compression
```

## Comparing `trytond_sale_price_list-7.0.0.tar` & `trytond_sale_price_list-7.2.0.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:51.681348 trytond_sale_price_list-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-22 17:23:19.000000 trytond_sale_price_list-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2537 2023-10-30 17:12:32.000000 trytond_sale_price_list-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:12:31.000000 trytond_sale_price_list-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_price_list-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2748 2023-10-30 17:38:51.681348 trytond_sale_price_list-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      160 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      573 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1165 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.0.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:21.000000 trytond_sale_price_list-7.0.0/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:51.678015 trytond_sale_price_list-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2816 2023-10-22 17:23:19.000000 trytond_sale_price_list-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      160 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:19.000000 trytond_sale_price_list-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:51.678015 trytond_sale_price_list-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1811 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1811 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1485 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1857 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1820 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1673 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1806 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2029 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1485 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1893 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1902 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1776 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1594 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1833 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1891 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1542 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1485 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1651 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1485 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1485 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1485 2023-10-28 12:11:25.000000 trytond_sale_price_list-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2212 2023-08-13 15:26:13.000000 trytond_sale_price_list-7.0.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1858 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.0.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3055 2023-10-07 15:40:36.000000 trytond_sale_price_list-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2484 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-01-16 14:00:21.000000 trytond_sale_price_list-7.0.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:38:51.681348 trytond_sale_price_list-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4422 2023-10-27 17:38:49.000000 trytond_sale_price_list-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:51.678015 trytond_sale_price_list-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5314 2023-10-07 15:40:36.000000 trytond_sale_price_list-7.0.0/tests/scenario_sale_price_list.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_price_list-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      163 2023-10-30 17:12:28.000000 trytond_sale_price_list-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:51.678015 trytond_sale_price_list-7.0.0/trytond_sale_price_list.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2748 2023-10-30 17:38:51.000000 trytond_sale_price_list-7.0.0/trytond_sale_price_list.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1820 2023-10-30 17:38:51.000000 trytond_sale_price_list-7.0.0/trytond_sale_price_list.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:38:51.000000 trytond_sale_price_list-7.0.0/trytond_sale_price_list.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-10-30 17:38:51.000000 trytond_sale_price_list-7.0.0/trytond_sale_price_list.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 trytond_sale_price_list-7.0.0/trytond_sale_price_list.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      154 2023-10-30 17:38:51.000000 trytond_sale_price_list-7.0.0/trytond_sale_price_list.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:38:51.000000 trytond_sale_price_list-7.0.0/trytond_sale_price_list.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:38:51.678015 trytond_sale_price_list-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-01-16 14:00:21.000000 trytond_sale_price_list-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-01-16 14:00:21.000000 trytond_sale_price_list-7.0.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.0.0/view/product_sale_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-01-16 14:00:21.000000 trytond_sale_price_list-7.0.0/view/sale_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:41.243149 trytond_sale_price_list-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2638 2024-04-29 15:25:47.000000 trytond_sale_price_list-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:25:47.000000 trytond_sale_price_list-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_price_list-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2748 2024-04-29 15:48:41.243149 trytond_sale_price_list-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      160 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      573 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1165 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.2.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:21.000000 trytond_sale_price_list-7.2.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:41.239815 trytond_sale_price_list-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_sale_price_list-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      160 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:27.000000 trytond_sale_price_list-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:41.239815 trytond_sale_price_list-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1811 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1811 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1485 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1857 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1820 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1673 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1806 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2029 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1485 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1893 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1810 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1902 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1776 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1594 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1833 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1754 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1891 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2024-04-29 13:17:17.000000 trytond_sale_price_list-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1485 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1651 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1485 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1485 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1485 2024-04-27 16:43:26.000000 trytond_sale_price_list-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2233 2024-04-22 12:14:36.000000 trytond_sale_price_list-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1830 2024-04-27 16:30:39.000000 trytond_sale_price_list-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3055 2024-02-04 18:51:26.000000 trytond_sale_price_list-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2484 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-01-16 14:00:21.000000 trytond_sale_price_list-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:48:41.243149 trytond_sale_price_list-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4422 2024-03-17 11:01:36.000000 trytond_sale_price_list-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:41.239815 trytond_sale_price_list-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5288 2024-04-22 12:14:36.000000 trytond_sale_price_list-7.2.0/tests/scenario_sale_price_list.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:27.000000 trytond_sale_price_list-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      163 2024-04-29 15:25:43.000000 trytond_sale_price_list-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:41.243149 trytond_sale_price_list-7.2.0/trytond_sale_price_list.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2748 2024-04-29 15:48:40.000000 trytond_sale_price_list-7.2.0/trytond_sale_price_list.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1802 2024-04-29 15:48:41.000000 trytond_sale_price_list-7.2.0/trytond_sale_price_list.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:48:40.000000 trytond_sale_price_list-7.2.0/trytond_sale_price_list.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:48:40.000000 trytond_sale_price_list-7.2.0/trytond_sale_price_list.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 trytond_sale_price_list-7.2.0/trytond_sale_price_list.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      154 2024-04-29 15:48:40.000000 trytond_sale_price_list-7.2.0/trytond_sale_price_list.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:48:40.000000 trytond_sale_price_list-7.2.0/trytond_sale_price_list.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:41.243149 trytond_sale_price_list-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-01-16 14:00:21.000000 trytond_sale_price_list-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-01-16 14:00:21.000000 trytond_sale_price_list-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_sale_price_list-7.2.0/view/product_sale_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-01-16 14:00:21.000000 trytond_sale_price_list-7.2.0/view/sale_form.xml
```

### Comparing `trytond_sale_price_list-7.0.0/CHANGELOG` & `trytond_sale_price_list-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_sale_price_list-7.0.0/COPYRIGHT` & `trytond_sale_price_list-7.2.0/COPYRIGHT`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2009-2023 Cédric Krier.
+Copyright (C) 2009-2024 Cédric Krier.
 Copyright (C) 2009-2012 Bertrand Chenal.
-Copyright (C) 2009-2023 B2CK SPRL.
+Copyright (C) 2009-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_price_list-7.0.0/LICENSE` & `trytond_sale_price_list-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/PKG-INFO` & `trytond_sale_price_list-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_price_list
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add price list on sale
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
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product_price_list<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product_price_list<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Price List Module
 ######################
 
 The sale price list module adds support for price list on sale.
 A price list can be set per party or as default.
```

### Comparing `trytond_sale_price_list-7.0.0/__init__.py` & `trytond_sale_price_list-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/configuration.py` & `trytond_sale_price_list-7.2.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/doc/conf.py` & `trytond_sale_price_list-7.2.0/doc/conf.py`

 * *Files 3% similar despite different names*

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

### Comparing `trytond_sale_price_list-7.0.0/locale/bg.po` & `trytond_sale_price_list-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/ca.po` & `trytond_sale_price_list-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/cs.po` & `trytond_sale_price_list-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/de.po` & `trytond_sale_price_list-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/es.po` & `trytond_sale_price_list-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/es_419.po` & `trytond_sale_price_list-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/et.po` & `trytond_sale_price_list-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/fa.po` & `trytond_sale_price_list-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/fi.po` & `trytond_sale_price_list-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/fr.po` & `trytond_sale_price_list-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/hu.po` & `trytond_sale_price_list-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/id.po` & `trytond_sale_price_list-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/it.po` & `trytond_sale_price_list-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/lo.po` & `trytond_sale_price_list-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/lt.po` & `trytond_sale_price_list-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/nl.po` & `trytond_sale_price_list-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/pl.po` & `trytond_sale_price_list-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/pt.po` & `trytond_sale_price_list-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/ro.po` & `trytond_sale_price_list-7.2.0/locale/ru.po`

 * *Files 2% similar despite different names*

```diff
@@ -8,43 +8,43 @@
 
 msgctxt "field:party.party,sale_price_lists:"
 msgid "Sale Price Lists"
 msgstr ""
 
 msgctxt "field:party.party.sale_price_list,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:party.party.sale_price_list,party:"
 msgid "Party"
-msgstr "Parte"
+msgstr ""
 
 msgctxt "field:party.party.sale_price_list,sale_price_list:"
 msgid "Sale Price List"
 msgstr ""
 
 msgctxt "field:product.sale.context,price_list:"
 msgid "Price List"
-msgstr "Listă de prețuri"
+msgstr ""
 
 msgctxt "field:sale.configuration,sale_price_list:"
 msgid "Sale Price List"
 msgstr ""
 
 msgctxt "field:sale.configuration.sale_price_list,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr ""
 
 msgctxt "field:sale.configuration.sale_price_list,sale_price_list:"
 msgid "Sale Price List"
 msgstr ""
 
 msgctxt "field:sale.sale,price_list:"
 msgid "Price List"
-msgstr "Listă de prețuri"
+msgstr ""
 
 msgctxt "help:party.party,sale_price_list:"
 msgid "The default price list for new sales."
 msgstr ""
 
 msgctxt "help:sale.configuration,sale_price_list:"
 msgid "The default price list for new parties."
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_sale_price_list-7.0.0/locale/ru.po` & `trytond_sale_price_list-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/sl.po` & `trytond_sale_price_list-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/tr.po` & `trytond_sale_price_list-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/locale/uk.po` & `trytond_sale_price_list-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/party.py` & `trytond_sale_price_list-7.2.0/party.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,11 +47,11 @@
     party = fields.Many2One(
         'party.party', "Party", ondelete='CASCADE',
         context={
             'company': Eval('company', -1),
             },
         depends={'company'})
     sale_price_list = fields.Many2One(
-        'product.price_list', "Sale Price List",
+        'product.price_list', "Sale Price List", ondelete='RESTRICT',
         domain=[
             ('company', '=', Eval('company', -1)),
             ])
```

### Comparing `trytond_sale_price_list-7.0.0/party.xml` & `trytond_sale_price_list-7.2.0/party.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_sale_price_list-7.0.0/party.xml` & `trytond_sale_price_list-7.2.0/party.xml`

```diff
@@ -5,30 +5,34 @@
   <data>
     <record model="ir.ui.view" id="party_view_form">
       <field name="model">party.party</field>
       <field name="inherit" ref="party.party_view_form"/>
       <field name="name">party_form</field>
     </record>
     <record model="ir.model.field.access" id="access_party_sale_price_lists">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'sale_price_lists')]"/>
+      <field name="model">party.party</field>
+      <field name="field">sale_price_lists</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_sale_price_lists_group_sale">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'sale_price_lists')]"/>
+      <field name="model">party.party</field>
+      <field name="field">sale_price_lists</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="access_party_sale_price_list">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'sale_price_list')]"/>
+      <field name="model">party.party</field>
+      <field name="field">sale_price_list</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="access_party_sale_price_list_group_sale">
-      <field name="field" search="[('model.model', '=', 'party.party'), ('name', '=', 'sale_price_list')]"/>
+      <field name="model">party.party</field>
+      <field name="field">sale_price_list</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_sale_price_list-7.0.0/product.py` & `trytond_sale_price_list-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/sale.py` & `trytond_sale_price_list-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/setup.py` & `trytond_sale_price_list-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/tests/scenario_sale_price_list.rst` & `trytond_sale_price_list-7.2.0/tests/scenario_sale_price_list.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 ========================
 Sale Price List Scenario
 ========================
 
 Imports::
 
-    >>> import datetime
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, set_user
 
 Activate modules::
 
     >>> config = activate_modules('sale_price_list')
 
 Create company::
 
@@ -125,16 +124,15 @@
 
 Use the price list on sale::
 
     >>> set_user(sale_user)
     >>> Sale = Model.get('sale.sale')
     >>> sale = Sale()
     >>> sale.party = customer
-    >>> sale.price_list == price_list
-    True
+    >>> assertEqual(sale.price_list, price_list)
     >>> sale.payment_term = payment_term
     >>> sale_line = sale.lines.new()
     >>> sale_line.product = product
     >>> sale_line.unit_price
     Decimal('8.0000')
     >>> sale_line.quantity = 12.0
     >>> sale_line.unit_price
@@ -159,9 +157,8 @@
     >>> config.sale_price_list = sale_price_list
     >>> config.save()
 
 Use the sale price list on sale::
 
     >>> set_user(sale_user)
     >>> sale.party = customer_without_price_list
-    >>> sale.price_list == sale_price_list
-    True
+    >>> assertEqual(sale.price_list, sale_price_list)
```

### Comparing `trytond_sale_price_list-7.0.0/tox.ini` & `trytond_sale_price_list-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_price_list-7.0.0/trytond_sale_price_list.egg-info/PKG-INFO` & `trytond_sale_price_list-7.2.0/trytond_sale_price_list.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-sale-price-list
-Version: 7.0.0
+Name: trytond_sale_price_list
+Version: 7.2.0
 Summary: Tryton module to add price list on sale
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
@@ -48,20 +48,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product_price_list<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product_price_list<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Price List Module
 ######################
 
 The sale price list module adds support for price list on sale.
 A price list can be set per party or as default.
```

### Comparing `trytond_sale_price_list-7.0.0/trytond_sale_price_list.egg-info/SOURCES.txt` & `trytond_sale_price_list-7.2.0/trytond_sale_price_list.egg-info/SOURCES.txt`

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
 configuration.py
```

