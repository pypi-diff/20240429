# Comparing `tmp/trytond_sale_supply-7.0.5.tar.gz` & `tmp/trytond_sale_supply-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_supply-7.0.5.tar", last modified: Sun Mar  3 12:15:58 2024, max compression
+gzip compressed data, was "trytond_sale_supply-7.2.0.tar", last modified: Mon Apr 29 15:50:13 2024, max compression
```

## Comparing `trytond_sale_supply-7.0.5.tar` & `trytond_sale_supply-7.2.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:15:58.065324 trytond_sale_supply-7.0.5/
--rw-r--r--   0 ced       (1000) ced       (1000)      203 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2738 2024-03-03 12:15:55.000000 trytond_sale_supply-7.0.5/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-03-03 12:15:55.000000 trytond_sale_supply-7.0.5/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3191 2024-03-03 12:15:58.065324 trytond_sale_supply-7.0.5/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2024-02-05 16:24:27.000000 trytond_sale_supply-7.0.5/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:15:58.061989 trytond_sale_supply-7.0.5/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2812 2024-02-05 16:24:27.000000 trytond_sale_supply-7.0.5/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:15:58.061989 trytond_sale_supply-7.0.5/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1652 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1899 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1885 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1898 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1562 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1657 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1743 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1906 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1601 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1553 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1684 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1809 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1852 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1628 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1711 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1652 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1699 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1728 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1543 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1596 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3446 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4435 2024-02-29 11:50:49.000000 trytond_sale_supply-7.0.5/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13061 2024-02-05 16:24:27.000000 trytond_sale_supply-7.0.5/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1729 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-03-03 12:15:58.065324 trytond_sale_supply-7.0.5/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4441 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2873 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:15:58.061989 trytond_sale_supply-7.0.5/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7845 2024-02-05 16:24:27.000000 trytond_sale_supply-7.0.5/tests/scenario_sale_supply.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1550 2024-02-05 16:24:27.000000 trytond_sale_supply-7.0.5/tests/scenario_sale_supply_notifications.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3849 2024-02-05 16:24:27.000000 trytond_sale_supply-7.0.5/tests/scenario_sale_supply_shipment_on_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3356 2024-02-05 16:24:27.000000 trytond_sale_supply-7.0.5/tests/scenario_sale_supply_stock_first.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      174 2024-02-15 18:32:11.000000 trytond_sale_supply-7.0.5/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:15:58.065324 trytond_sale_supply-7.0.5/trytond_sale_supply.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3191 2024-03-03 12:15:57.000000 trytond_sale_supply-7.0.5/trytond_sale_supply.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1910 2024-03-03 12:15:58.000000 trytond_sale_supply-7.0.5/trytond_sale_supply.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-03-03 12:15:57.000000 trytond_sale_supply-7.0.5/trytond_sale_supply.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       60 2024-03-03 12:15:57.000000 trytond_sale_supply-7.0.5/trytond_sale_supply.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:12.000000 trytond_sale_supply-7.0.5/trytond_sale_supply.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-03-03 12:15:57.000000 trytond_sale_supply-7.0.5/trytond_sale_supply.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-03-03 12:15:57.000000 trytond_sale_supply-7.0.5/trytond_sale_supply.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:15:58.065324 trytond_sale_supply-7.0.5/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-10-30 17:06:38.000000 trytond_sale_supply-7.0.5/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:13.614066 trytond_sale_supply-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2334 2024-04-29 15:27:03.000000 trytond_sale_supply-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:27:03.000000 trytond_sale_supply-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_supply-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_supply-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3191 2024-04-29 15:50:13.614066 trytond_sale_supply-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-01-27 09:58:52.000000 trytond_sale_supply-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      560 2024-04-22 12:14:36.000000 trytond_sale_supply-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:13.610733 trytond_sale_supply-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3074 2024-04-27 16:30:39.000000 trytond_sale_supply-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-01-27 09:58:52.000000 trytond_sale_supply-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:30.000000 trytond_sale_supply-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:13.610733 trytond_sale_supply-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1652 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1899 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1885 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1898 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1562 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1657 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1743 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1906 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1601 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1553 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1684 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1809 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1852 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1628 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1711 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1543 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1652 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1699 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1728 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1543 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1596 2024-04-27 16:43:27.000000 trytond_sale_supply-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2024-01-27 09:58:52.000000 trytond_sale_supply-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3446 2024-02-04 18:51:26.000000 trytond_sale_supply-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:21.000000 trytond_sale_supply-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2069 2024-04-27 16:30:39.000000 trytond_sale_supply-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10362 2024-04-22 12:14:36.000000 trytond_sale_supply-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1729 2023-01-16 14:00:21.000000 trytond_sale_supply-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:50:13.614066 trytond_sale_supply-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4441 2024-03-17 11:01:36.000000 trytond_sale_supply-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2854 2024-04-27 16:30:39.000000 trytond_sale_supply-7.2.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:13.610733 trytond_sale_supply-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_supply-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7830 2024-04-27 16:30:39.000000 trytond_sale_supply-7.2.0/tests/scenario_sale_supply.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1549 2024-04-22 12:14:36.000000 trytond_sale_supply-7.2.0/tests/scenario_sale_supply_notifications.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4144 2024-04-22 12:14:36.000000 trytond_sale_supply-7.2.0/tests/scenario_sale_supply_request_cancelled.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3809 2024-04-22 12:14:36.000000 trytond_sale_supply-7.2.0/tests/scenario_sale_supply_shipment_on_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3333 2024-04-22 12:14:36.000000 trytond_sale_supply-7.2.0/tests/scenario_sale_supply_stock_first.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-01-27 09:58:52.000000 trytond_sale_supply-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_supply-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:30.000000 trytond_sale_supply-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      174 2024-04-29 15:26:59.000000 trytond_sale_supply-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:13.614066 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3191 2024-04-29 15:50:13.000000 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1992 2024-04-29 15:50:13.000000 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:50:13.000000 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       60 2024-04-29 15:50:13.000000 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-04-29 15:50:13.000000 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:50:13.000000 trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:13.614066 trytond_sale_supply-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_sale_supply-7.2.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-01-16 14:00:21.000000 trytond_sale_supply-7.2.0/view/template_form.xml
```

### Comparing `trytond_sale_supply-7.0.5/CHANGELOG` & `trytond_sale_supply-7.2.0/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,9 @@
 
-Version 7.0.5 - 2024-03-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.4 - 2024-02-15
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.3 - 2024-02-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.2 - 2024-01-15
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2024-01-01
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_sale_supply-7.0.5/COPYRIGHT` & `trytond_sale_supply-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/LICENSE` & `trytond_sale_supply-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/PKG-INFO` & `trytond_sale_supply-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_supply
-Version: 7.0.5
+Version: 7.2.0
 Summary: Tryton module for sale supply
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
@@ -48,22 +48,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond_purchase_request<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond_purchase_request<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_supply<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_supply<7.3,>=7.2; extra == "test"
 
 Sale Supply Module
 ##################
 
 The Sale Supply module adds a "supply on sale option" to purchasable products.
 If selected, it will generate a purchase request for each sale line of this
 product depending of the option and the stock levels.
```

### Comparing `trytond_sale_supply-7.0.5/README.rst` & `trytond_sale_supply-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/__init__.py` & `trytond_sale_supply-7.2.0/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,18 +7,14 @@
 
 
 def register():
     Pool.register(
         sale.Sale,
         sale.Line,
         purchase.Request,
-        purchase.Purchase,
         stock.ShipmentIn,
         product.Template,
         product.Product,
         module='sale_supply', type_='model')
     Pool.register(
-        purchase.HandlePurchaseCancellationException,
-        module='sale_supply', type_='wizard')
-    Pool.register(
         stock.OrderPoint,
         module='sale_supply', type_='model', depends=['stock_supply'])
```

### Comparing `trytond_sale_supply-7.0.5/doc/conf.py` & `trytond_sale_supply-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_supply-7.0.5/doc/index.rst` & `trytond_sale_supply-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/bg.po` & `trytond_sale_supply-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/ca.po` & `trytond_sale_supply-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/cs.po` & `trytond_sale_supply-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/de.po` & `trytond_sale_supply-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/es.po` & `trytond_sale_supply-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/es_419.po` & `trytond_sale_supply-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/et.po` & `trytond_sale_supply-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/fa.po` & `trytond_sale_supply-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/fi.po` & `trytond_sale_supply-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/fr.po` & `trytond_sale_supply-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/hu.po` & `trytond_sale_supply-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/id.po` & `trytond_sale_supply-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/it.po` & `trytond_sale_supply-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/lo.po` & `trytond_sale_supply-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/lt.po` & `trytond_sale_supply-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/nl.po` & `trytond_sale_supply-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/pl.po` & `trytond_sale_supply-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/pt.po` & `trytond_sale_supply-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/ro.po` & `trytond_sale_supply-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/ru.po` & `trytond_sale_supply-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/sl.po` & `trytond_sale_supply-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/tr.po` & `trytond_sale_supply-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/uk.po` & `trytond_sale_supply-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/locale/zh_CN.po` & `trytond_sale_supply-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/message.xml` & `trytond_sale_supply-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/product.py` & `trytond_sale_supply-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/sale.py` & `trytond_sale_supply-7.2.0/sale.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 from collections import defaultdict
 from itertools import groupby
 from operator import attrgetter
 
-from trytond.model import Model, fields
+from trytond.model import fields
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval
 from trytond.transaction import Transaction
 
 
 class Sale(metaclass=PoolMeta):
     __name__ = 'sale.sale'
@@ -50,61 +50,79 @@
             product_quantities.clear()
         super()._process_shipment(sales)
 
     @classmethod
     def _process_supply(cls, sales, product_quantities):
         pool = Pool()
         Line = pool.get('sale.line')
-        Move = pool.get('stock.move')
         PurchaseRequest = pool.get('purchase.request')
-        ShipmentOut = pool.get('stock.shipment.out')
 
         requests, lines = [], []
-        moves_to_draft, shipments_to_wait = [], set()
         for sale in sales:
             reqs, lns = sale.create_purchase_requests(product_quantities)
             requests.extend(reqs)
             lines.extend(lns)
         PurchaseRequest.save(requests)
         Line.save(lines)
 
-        for sale in sales:
-            moves, shipments = sale.create_move_from_supply()
-            moves_to_draft.extend(moves)
-            shipments_to_wait.update(shipments)
-        shipments_to_wait = ShipmentOut.browse(list(shipments_to_wait))
-        Move.draft(moves_to_draft)
-        ShipmentOut.wait(shipments_to_wait)
+        cls._update_moves_from_supply(sales)
 
     def create_purchase_requests(self, product_quantities):
         requests, lines = [], []
         for line in self.lines:
             request = line.get_purchase_request(product_quantities)
             if not request:
                 continue
             requests.append(request)
             assert not line.purchase_request
             line.purchase_request = request
             lines.append(line)
         return requests, lines
 
-    def create_move_from_supply(self):
-        'Set to draft move linked to supply'
+    @classmethod
+    def _update_moves_from_supply(cls, sales):
         pool = Pool()
-        ShipmentOut = pool.get('stock.shipment.out')
-        moves = []
-        for line in self.lines:
-            if (not line.has_supply
-                    or line.supply_state in {'supplied', 'cancelled'}):
+        Shipment = pool.get('stock.shipment.out')
+        Move = pool.get('stock.move')
+
+        shipments = set()
+
+        def add_shipment(shipment):
+            if (isinstance(shipment, Shipment)
+                    and shipment.state in {'draft', 'waiting'}):
+                shipments.add(shipment)
+
+        moves_to_draft, moves_to_cancel = [], []
+        for sale in sales:
+            for line in sale.lines:
                 for move in line.moves:
                     if move.state == 'staging':
-                        moves.append(move)
-        shipments = {m.shipment for m in moves
-            if isinstance(m.shipment, ShipmentOut)}
-        return moves, shipments
+                        if (not line.has_supply
+                                or line.supply_state == 'supplied'):
+                            moves_to_draft.append(move)
+                        elif line.supply_state == 'cancelled':
+                            moves_to_cancel.append(move)
+                        else:
+                            continue
+                        add_shipment(move.shipment)
+        if moves_to_draft:
+            Move.draft(moves_to_draft)
+        shipments = Shipment.browse(shipments)
+        shipments_waiting = [s for s in shipments if s.state == 'waiting']
+        if shipments:
+            Shipment.draft(shipments)  # clear inventory moves
+        if moves_to_cancel:
+            Move.cancel(moves_to_cancel)
+        if shipments:
+            Shipment.wait([
+                    s for s in shipments_waiting
+                    if any(m.state != 'cancelled' for m in s.moves)])
+            Shipment.cancel([
+                    s for s in shipments
+                    if all(m.state == 'cancelled' for m in s.moves)])
 
 
 class Line(metaclass=PoolMeta):
     __name__ = 'sale.line'
 
     purchase_request = fields.Many2One('purchase.request', 'Purchase Request',
         ondelete='SET NULL', readonly=True)
@@ -236,122 +254,31 @@
             warehouse=self.warehouse,
             origin=self.sale,
             )
 
     def assign_supplied(self, quantities, grouping=('product',)):
         '''
         Assign supplied move
-
-        location_quantities will be updated according to assigned
-        quantities.
+        The quantities will be updated according to assigned quantities.
         '''
         pool = Pool()
-        Uom = pool.get('product.uom')
         Move = pool.get('stock.move')
         ShipmentOut = pool.get('stock.shipment.out')
-        Location = pool.get('stock.location')
 
         if self.supply_state != 'supplied':
             return
 
-        def get_key(move, location_id):
-            key = (location_id,)
-            for field in grouping:
-                value = getattr(move, field)
-                if isinstance(value, Model):
-                    value = value.id
-                key += (value,)
-            return key
-
-        def get_values(key, location_name):
-            yield location_name, key[0]
-            for field, value in zip(grouping, key[1:]):
-                if value is not None and '.' not in field:
-                    yield field, value
-
-        def match(key, pattern):
-            for k, p in zip(key, pattern):
-                if p is None or k == p:
-                    continue
-                else:
-                    return False
-            else:
-                return True
-
         moves = set()
         for move in self.moves:
             shipment = move.shipment
             if isinstance(shipment, ShipmentOut):
                 if shipment.warehouse_storage == shipment.warehouse_output:
                     inventory_moves = shipment.outgoing_moves
                 else:
                     inventory_moves = shipment.inventory_moves
                 for inv_move in inventory_moves:
                     if inv_move.product == self.product:
                         moves.add(inv_move)
 
-        child_locations = {}
-        to_write = []
-        to_assign = []
-        for move in moves:
-            if move.state != 'draft':
-                continue
-
-            childs = child_locations.get(move.from_location)
-            if childs is None:
-                childs = Location.search([
-                        ('parent', 'child_of', [move.from_location.id]),
-                        ('type', '!=', 'view'),
-                        ])
-                child_locations[move.from_location] = childs
-            # Prevent picking from the destination location
-            try:
-                childs.remove(move.to_location)
-            except ValueError:
-                pass
-            # Try first to pick from source location
-            try:
-                childs.remove(move.from_location)
-                childs.insert(0, move.from_location)
-            except ValueError:
-                # from_location may be a view
-                pass
-            qties_converted = []
-            for key, quantity in quantities.items():
-                move_key = get_key(move, key[0])
-                if match(key, move_key):
-                    qty = Uom.compute_qty(
-                        move.product.default_uom, quantity, move.unit,
-                        round=False)
-                    qties_converted.append((key, qty))
-
-            location_qties = move.sort_quantities(
-                qties_converted, childs, grouping)
-            to_pick = move.pick_product(location_qties)
-
-            picked_qties = sum(qty for _, qty in to_pick)
-            if picked_qties < move.quantity:
-                first = False
-                Move.write([move], {
-                        'quantity': move.quantity - picked_qties,
-                        })
-            else:
-                first = True
-            for key, qty in to_pick:
-                values = dict(get_values(key, 'from_location'))
-                values['quantity'] = move.unit.round(qty)
-                if first:
-                    to_write.extend([[move], values])
-                    to_assign.append(move)
-                    first = False
-                else:
-                    with Transaction().set_context(_stock_move_split=True):
-                        to_assign.extend(Move.copy([move], default=values))
-
-                qty_default_uom = Uom.compute_qty(
-                    move.unit, qty, move.product.default_uom, round=False)
-
-                quantities[key] -= qty_default_uom
-        if to_write:
-            Move.write(*to_write)
-        if to_assign:
-            Move.assign(to_assign)
+        Move.assign_try(list(moves), grouping=grouping, pblc={
+                self.company.id: quantities,
+                })
```

### Comparing `trytond_sale_supply-7.0.5/sale.xml` & `trytond_sale_supply-7.2.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/setup.py` & `trytond_sale_supply-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/stock.py` & `trytond_sale_supply-7.2.0/stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 class ShipmentIn(metaclass=PoolMeta):
     __name__ = 'stock.shipment.in'
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
-    def done(cls, shipments):
-        super(ShipmentIn, cls).done(shipments)
+    def do(cls, shipments):
+        super().do(shipments)
 
         # Assigned sale move lines
         for shipment in shipments:
             shipment.assign_supplied()
 
     def assign_supplied(self, grouping=('product',), filter_=None):
         pool = Pool()
```

### Comparing `trytond_sale_supply-7.0.5/tests/scenario_sale_supply.rst` & `trytond_sale_supply-7.2.0/tests/scenario_sale_supply.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ====================
 Sale Supply Scenario
 ====================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
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
 
     >>> config = activate_modules(['sale_supply', 'sale', 'purchase'])
 
 Create company::
 
@@ -176,15 +176,15 @@
     >>> ShipmentIn = Model.get('stock.shipment.in')
     >>> Move = Model.get('stock.move')
     >>> shipment = ShipmentIn(supplier=supplier)
     >>> move, = shipment.incoming_moves.find()
     >>> shipment.incoming_moves.append(move)
     >>> move.quantity = 100
     >>> shipment.click('receive')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
     >>> set_user(sale_user)
     >>> sale.reload()
     >>> shipment, = sale.shipments
     >>> move, = [x for x in shipment.inventory_moves
     ...     if x.state == 'assigned']
@@ -247,11 +247,11 @@
     >>> shipment.click('pack')
 
     >>> set_user(admin_user)
     >>> changing_template.supply_on_sale = 'always'
     >>> changing_template.save()
 
     >>> set_user(stock_user)
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> set_user(purchase_user)
     >>> len(PurchaseRequest.find([('product', '=', changing_product.id)]))
     0
```

### Comparing `trytond_sale_supply-7.0.5/tests/scenario_sale_supply_notifications.rst` & `trytond_sale_supply-7.2.0/tests/scenario_sale_supply_notifications.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 =========================
 Sale Supply Notifications
 =========================
 
 Imports::
 
     >>> from proteus import Model
-
-    >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules(['sale_supply', 'stock_supply'])
 
     >>> Location = Model.get('stock.location')
     >>> OrderPoint = Model.get('stock.order_point')
```

### Comparing `trytond_sale_supply-7.0.5/tests/scenario_sale_supply_shipment_on_invoice.rst` & `trytond_sale_supply-7.2.0/tests/scenario_sale_supply_shipment_on_invoice.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =============================================
 Sale Supply with Shipment on Invoice Scenario
 =============================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
 
 Activate modules::
 
     >>> config = activate_modules('sale_supply')
 
 Create company::
```

### Comparing `trytond_sale_supply-7.0.5/tests/scenario_sale_supply_stock_first.rst` & `trytond_sale_supply-7.2.0/tests/scenario_sale_supply_stock_first.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 Sale Supply Stock First Scenario
 ================================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
     >>> from trytond.modules.company.tests.tools import create_company
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
+    >>> from trytond.tests.tools import activate_modules
 
 Activate modules::
 
     >>> config = activate_modules('sale_supply')
 
     >>> Inventory = Model.get('stock.inventory')
     >>> Location = Model.get('stock.location')
```

### Comparing `trytond_sale_supply-7.0.5/tox.ini` & `trytond_sale_supply-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply-7.0.5/trytond_sale_supply.egg-info/PKG-INFO` & `trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_supply
-Version: 7.0.5
+Version: 7.2.0
 Summary: Tryton module for sale supply
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
@@ -48,22 +48,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond_purchase_request<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond_purchase_request<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_supply<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_supply<7.3,>=7.2; extra == "test"
 
 Sale Supply Module
 ##################
 
 The Sale Supply module adds a "supply on sale option" to purchasable products.
 If selected, it will generate a purchase request for each sale line of this
 product depending of the option and the stock levels.
```

### Comparing `trytond_sale_supply-7.0.5/trytond_sale_supply.egg-info/SOURCES.txt` & `trytond_sale_supply-7.2.0/trytond_sale_supply.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 message.xml
@@ -47,14 +46,15 @@
 ./locale/sl.po
 ./locale/tr.po
 ./locale/uk.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/scenario_sale_supply.rst
 ./tests/scenario_sale_supply_notifications.rst
+./tests/scenario_sale_supply_request_cancelled.rst
 ./tests/scenario_sale_supply_shipment_on_invoice.rst
 ./tests/scenario_sale_supply_stock_first.rst
 ./tests/test_module.py
 ./tests/test_scenario.py
 ./view/sale_line_form.xml
 ./view/template_form.xml
 doc/conf.py
@@ -83,14 +83,15 @@
 locale/sl.po
 locale/tr.po
 locale/uk.po
 locale/zh_CN.po
 tests/__init__.py
 tests/scenario_sale_supply.rst
 tests/scenario_sale_supply_notifications.rst
+tests/scenario_sale_supply_request_cancelled.rst
 tests/scenario_sale_supply_shipment_on_invoice.rst
 tests/scenario_sale_supply_stock_first.rst
 tests/test_module.py
 tests/test_scenario.py
 trytond_sale_supply.egg-info/PKG-INFO
 trytond_sale_supply.egg-info/SOURCES.txt
 trytond_sale_supply.egg-info/dependency_links.txt
```

