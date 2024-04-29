# Comparing `tmp/trytond_stock_supply-7.0.2.tar.gz` & `tmp/trytond_stock_supply-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_supply-7.0.2.tar", last modified: Thu Apr  4 07:46:25 2024, max compression
+gzip compressed data, was "trytond_stock_supply-7.2.0.tar", last modified: Mon Apr 29 15:53:17 2024, max compression
```

## Comparing `trytond_stock_supply-7.0.2.tar` & `trytond_stock_supply-7.2.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:46:25.184930 trytond_stock_supply-7.0.2/
--rw-r--r--   0 ced       (1000) ced       (1000)     4072 2024-04-04 07:46:22.000000 trytond_stock_supply-7.0.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      761 2024-04-04 07:46:22.000000 trytond_stock_supply-7.0.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4553 2024-04-04 07:46:25.181596 trytond_stock_supply-7.0.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1936 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      819 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:46:25.178263 trytond_stock_supply-7.0.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2791 2024-03-03 16:24:20.000000 trytond_stock_supply-7.0.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1936 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:46:25.181596 trytond_stock_supply-7.0.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5635 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6000 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5981 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6050 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4704 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4985 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6098 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6102 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5766 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4701 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4980 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5109 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4839 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5820 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5039 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5924 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4611 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5634 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5684 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4827 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4597 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5505 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2091 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/location.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/location.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1357 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8358 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/order_point.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4016 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/order_point.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      848 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1637 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14550 2024-03-25 21:49:01.000000 trytond_stock_supply-7.0.2/purchase_request.py
--rw-r--r--   0 ced       (1000) ced       (1000)      966 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/purchase_request.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-04 07:46:25.184930 trytond_stock_supply-7.0.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4354 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7697 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/shipment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5026 2024-01-08 10:57:27.000000 trytond_stock_supply-7.0.2/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1279 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:46:25.181596 trytond_stock_supply-7.0.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5764 2024-02-05 16:24:27.000000 trytond_stock_supply-7.0.2/tests/scenario_stock_internal_supply.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4286 2024-02-05 16:24:27.000000 trytond_stock_supply-7.0.2/tests/scenario_stock_internal_supply_lead_time.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4459 2024-02-05 16:24:27.000000 trytond_stock_supply-7.0.2/tests/scenario_stock_internal_supply_overflow.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7517 2024-02-05 16:24:27.000000 trytond_stock_supply-7.0.2/tests/scenario_stock_supply_purchase_request.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6265 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-02-05 16:24:27.000000 trytond_stock_supply-7.0.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:46:25.181596 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4553 2024-04-04 07:46:24.000000 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2365 2024-04-04 07:46:25.000000 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-04 07:46:24.000000 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-04 07:46:24.000000 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:19.000000 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2024-04-04 07:46:24.000000 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-04 07:46:24.000000 trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-04 07:46:25.181596 trytond_stock_supply-7.0.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      451 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1076 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/view/order_point_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      486 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/view/order_point_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/view/purchase_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-10-30 17:06:38.000000 trytond_stock_supply-7.0.2/view/supply_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:17.792582 trytond_stock_supply-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3971 2024-04-29 15:29:20.000000 trytond_stock_supply-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      761 2024-04-29 15:29:20.000000 trytond_stock_supply-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_supply-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4553 2024-04-29 15:53:17.792582 trytond_stock_supply-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1936 2024-01-27 09:58:52.000000 trytond_stock_supply-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      819 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:17.785916 trytond_stock_supply-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3075 2024-04-27 16:30:39.000000 trytond_stock_supply-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1936 2024-01-27 09:58:52.000000 trytond_stock_supply-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:37.000000 trytond_stock_supply-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:17.789249 trytond_stock_supply-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5635 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6000 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5981 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6050 2024-04-29 13:17:17.000000 trytond_stock_supply-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4704 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4985 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6098 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6102 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5766 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4701 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4980 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5109 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4839 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5820 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5039 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5924 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4611 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5634 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5684 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4827 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4597 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5505 2024-04-27 16:43:28.000000 trytond_stock_supply-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2091 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/location.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-01-16 14:00:21.000000 trytond_stock_supply-7.2.0/location.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1357 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8358 2024-02-04 18:51:27.000000 trytond_stock_supply-7.2.0/order_point.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3947 2024-04-27 16:30:39.000000 trytond_stock_supply-7.2.0/order_point.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      848 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1637 2023-01-16 14:00:21.000000 trytond_stock_supply-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14550 2024-04-27 16:30:39.000000 trytond_stock_supply-7.2.0/purchase_request.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      943 2024-04-27 16:30:39.000000 trytond_stock_supply-7.2.0/purchase_request.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:53:17.792582 trytond_stock_supply-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4354 2024-03-17 11:01:36.000000 trytond_stock_supply-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7697 2024-02-04 18:51:27.000000 trytond_stock_supply-7.2.0/shipment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5026 2024-04-22 12:14:37.000000 trytond_stock_supply-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1279 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:17.789249 trytond_stock_supply-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5751 2024-04-22 12:14:37.000000 trytond_stock_supply-7.2.0/tests/scenario_stock_internal_supply.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4298 2024-04-22 12:14:37.000000 trytond_stock_supply-7.2.0/tests/scenario_stock_internal_supply_lead_time.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4435 2024-04-22 12:14:36.000000 trytond_stock_supply-7.2.0/tests/scenario_stock_internal_supply_overflow.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7452 2024-04-22 12:14:36.000000 trytond_stock_supply-7.2.0/tests/scenario_stock_supply_purchase_request.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6265 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:37.000000 trytond_stock_supply-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-29 15:29:16.000000 trytond_stock_supply-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:17.789249 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4553 2024-04-29 15:53:17.000000 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2365 2024-04-29 15:53:17.000000 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:53:17.000000 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       62 2024-04-29 15:53:17.000000 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      217 2024-04-29 15:53:17.000000 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:53:17.000000 trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:17.789249 trytond_stock_supply-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      451 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1076 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/view/order_point_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      486 2024-02-04 18:51:27.000000 trytond_stock_supply-7.2.0/view/order_point_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/view/purchase_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-04-15 07:12:15.000000 trytond_stock_supply-7.2.0/view/supply_start_form.xml
```

### Comparing `trytond_stock_supply-7.0.2/CHANGELOG` & `trytond_stock_supply-7.2.0/CHANGELOG`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 
-Version 7.0.2 - 2024-04-04
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2024-01-15
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_stock_supply-7.0.2/COPYRIGHT` & `trytond_stock_supply-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/LICENSE` & `trytond_stock_supply-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/PKG-INFO` & `trytond_stock_supply-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_supply
-Version: 7.0.2
+Version: 7.2.0
 Summary: Tryton module for stock supply
 Home-page: http://www.tryton.org/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
@@ -48,23 +48,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond_purchase_request<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond_purchase_request<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Stock Supply Module
 ###################
 
 The Stock Supply module add automatic supply mechanisms and introduce
 the concepts of order point.
```

### Comparing `trytond_stock_supply-7.0.2/README.rst` & `trytond_stock_supply-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/__init__.py` & `trytond_stock_supply-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/doc/conf.py` & `trytond_stock_supply-7.2.0/doc/conf.py`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_stock_supply-7.0.2/doc/index.rst` & `trytond_stock_supply-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/bg.po` & `trytond_stock_supply-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/ca.po` & `trytond_stock_supply-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/cs.po` & `trytond_stock_supply-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/de.po` & `trytond_stock_supply-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/es.po` & `trytond_stock_supply-7.2.0/locale/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 msgctxt "field:stock.order_point,storage_location:"
 msgid "Storage Location"
 msgstr "Ubicación interna"
 
 msgctxt "field:stock.order_point,target_quantity:"
 msgid "Target Quantity"
-msgstr "Cantidad destino"
+msgstr "Cantidad deseada"
 
 msgctxt "field:stock.order_point,type:"
 msgid "Type"
 msgstr "Tipo"
 
 msgctxt "field:stock.order_point,unit:"
 msgid "Unit"
```

### Comparing `trytond_stock_supply-7.0.2/locale/es_419.po` & `trytond_stock_supply-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/et.po` & `trytond_stock_supply-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/fa.po` & `trytond_stock_supply-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/fi.po` & `trytond_stock_supply-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/fr.po` & `trytond_stock_supply-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/hu.po` & `trytond_stock_supply-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/id.po` & `trytond_stock_supply-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/it.po` & `trytond_stock_supply-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/lo.po` & `trytond_stock_supply-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/lt.po` & `trytond_stock_supply-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/nl.po` & `trytond_stock_supply-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/pl.po` & `trytond_stock_supply-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/pt.po` & `trytond_stock_supply-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/ro.po` & `trytond_stock_supply-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/ru.po` & `trytond_stock_supply-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/sl.po` & `trytond_stock_supply-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/tr.po` & `trytond_stock_supply-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/uk.po` & `trytond_stock_supply-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/locale/zh_CN.po` & `trytond_stock_supply-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/location.py` & `trytond_stock_supply-7.2.0/location.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/message.xml` & `trytond_stock_supply-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/order_point.py` & `trytond_stock_supply-7.2.0/order_point.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/order_point.xml` & `trytond_stock_supply-7.2.0/order_point.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_stock_supply-7.0.2/order_point.xml` & `trytond_stock_supply-7.2.0/order_point.xml`

```diff
@@ -42,31 +42,31 @@
     <record model="ir.action.act_window.domain" id="act_order_point_form_domain_all">
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="act_window" ref="act_order_point_form"/>
     </record>
     <menuitem parent="stock.menu_stock" sequence="50" action="act_order_point_form" id="menu_order_point_form"/>
     <record model="ir.model.access" id="access_order_point">
-      <field name="model" search="[('model', '=', 'stock.order_point')]"/>
+      <field name="model">stock.order_point</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_order_point_admin">
-      <field name="model" search="[('model', '=', 'stock.order_point')]"/>
+      <field name="model">stock.order_point</field>
       <field name="group" ref="stock.group_stock_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_order_point_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'stock.order_point')]"/>
+      <field name="model">stock.order_point</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_order_point_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_order_point_companies"/>
     </record>
   </data>
```

### Comparing `trytond_stock_supply-7.0.2/product.py` & `trytond_stock_supply-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/product.xml` & `trytond_stock_supply-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/purchase_request.py` & `trytond_stock_supply-7.2.0/purchase_request.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/purchase_request.xml` & `trytond_stock_supply-7.2.0/purchase_request.xml`

 * *Files 10% similar despite different names*

#### Comparing `trytond_stock_supply-7.0.2/purchase_request.xml` & `trytond_stock_supply-7.2.0/purchase_request.xml`

```diff
@@ -5,15 +5,15 @@
   <data>
     <record model="ir.ui.view" id="purchase_configuration_view_form">
       <field name="model">purchase.configuration</field>
       <field name="inherit" ref="purchase.purchase_configuration_view_form"/>
       <field name="name">purchase_configuration_form</field>
     </record>
     <record model="ir.model.access" id="access_purchase_request_stock">
-      <field name="model" search="[('model', '=', 'purchase.request')]"/>
+      <field name="model">purchase.request</field>
       <field name="group" ref="stock.group_stock_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
   </data>
```

### Comparing `trytond_stock_supply-7.0.2/setup.py` & `trytond_stock_supply-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/shipment.py` & `trytond_stock_supply-7.2.0/shipment.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/stock.py` & `trytond_stock_supply-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/stock.xml` & `trytond_stock_supply-7.2.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/tests/scenario_stock_internal_supply.rst` & `trytond_stock_supply-7.2.0/tests/scenario_stock_internal_supply.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ===========================
 Stock Shipment Out Scenario
 ===========================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
 
 Activate modules::
 
     >>> config = activate_modules('stock_supply')
 
 Create company::
```

### Comparing `trytond_stock_supply-7.0.2/tests/scenario_stock_internal_supply_lead_time.rst` & `trytond_stock_supply-7.2.0/tests/scenario_stock_internal_supply_lead_time.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Stock Internal Supply Lead Time Scenario
 ========================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
     >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('stock_supply')
@@ -111,34 +111,28 @@
     >>> ShipmentInternal = Model.get('stock.shipment.internal')
     >>> Wizard('stock.supply').execute('create_')
     >>> shipments = ShipmentInternal.find([], order=[('planned_date', 'ASC')])
     >>> len(shipments)
     2
     >>> first, second = shipments
 
-    >>> first.planned_date == today
-    True
+    >>> assertEqual(first.planned_date, today)
     >>> first.state
     'request'
     >>> len(first.moves)
     1
     >>> move, = first.moves
-    >>> move.from_location == warehouse_loc.storage_location
-    True
-    >>> move.to_location == sec_warehouse_loc.storage_location
-    True
+    >>> assertEqual(move.from_location, warehouse_loc.storage_location)
+    >>> assertEqual(move.to_location, sec_warehouse_loc.storage_location)
     >>> move.quantity
     15.0
 
-    >>> second.planned_date == tomorrow
-    True
+    >>> assertEqual(second.planned_date, tomorrow)
     >>> second.state
     'request'
     >>> len(second.moves)
     1
     >>> move, = second.moves
-    >>> move.from_location == warehouse_loc.storage_location
-    True
-    >>> move.to_location == sec_warehouse_loc.storage_location
-    True
+    >>> assertEqual(move.from_location, warehouse_loc.storage_location)
+    >>> assertEqual(move.to_location, sec_warehouse_loc.storage_location)
     >>> move.quantity
     10.0
```

### Comparing `trytond_stock_supply-7.0.2/tests/scenario_stock_internal_supply_overflow.rst` & `trytond_stock_supply-7.2.0/tests/scenario_stock_internal_supply_overflow.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ====================================================
 Stock supply scenario: Internal supply with overflow
 ====================================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('stock_supply')
 
 Create company::
 
@@ -90,22 +90,19 @@
     >>> Wizard('stock.supply').execute('create_')
     >>> shipment, = ShipmentInternal.find([
     ...         ('to_location', '=', overflow_loc.id),
     ...         ])
     >>> shipment.state
     'request'
     >>> move, = shipment.moves
-    >>> move.product.id == product.id
-    True
+    >>> assertEqual(move.product, product)
     >>> move.quantity
     40.0
-    >>> move.from_location.id == overflowed_storage_loc.id
-    True
-    >>> move.to_location.id == overflow_loc.id
-    True
+    >>> assertEqual(move.from_location, overflowed_storage_loc)
+    >>> assertEqual(move.to_location, overflow_loc)
 
 Using an overflow location
 --------------------------
 
 Create the overflowed location::
 
     >>> sec_overflowed_storage_loc = Location()
@@ -128,15 +125,12 @@
 
     >>> Wizard('stock.supply').execute('create_')
     >>> shipment, = ShipmentInternal.find(
     ...     [('from_location', '=', sec_overflowed_storage_loc.id)])
     >>> shipment.state
     'request'
     >>> move, = shipment.moves
-    >>> move.product.id == product.id
-    True
+    >>> assertEqual(move.product, product)
     >>> move.quantity
     10.0
-    >>> move.from_location.id == sec_overflowed_storage_loc.id
-    True
-    >>> move.to_location.id == overflow_loc.id
-    True
+    >>> assertEqual(move.from_location, sec_overflowed_storage_loc)
+    >>> assertEqual(move.to_location, overflow_loc)
```

### Comparing `trytond_stock_supply-7.0.2/tests/scenario_stock_supply_purchase_request.rst` & `trytond_stock_supply-7.2.0/tests/scenario_stock_supply_purchase_request.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 =========================
 Purchase Request Scenario
 =========================
 
 Imports::
 
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import (create_chart,
-    ...     get_accounts)
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, set_user
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_supply')
 
@@ -172,16 +170,15 @@
     >>> create_pr = Wizard('stock.supply')
     >>> create_pr.execute('create_')
 
 There is now a draft purchase request::
 
     >>> set_user(purchase_user)
     >>> pr, = PurchaseRequest.find([('state', '=', 'draft')])
-    >>> pr.product == product
-    True
+    >>> assertEqual(pr.product, product)
     >>> pr.quantity
     2.0
 
 Create an order point with negative minimal quantity::
 
     >>> set_user(stock_admin_user)
     >>> OrderPoint = Model.get('stock.order_point')
@@ -212,16 +209,15 @@
     >>> create_pr = Wizard('stock.supply')
     >>> create_pr.execute('create_')
 
 There is now a draft purchase request::
 
     >>> set_user(purchase_user)
     >>> pr, = PurchaseRequest.find([('state', '=', 'draft')])
-    >>> pr.product == product
-    True
+    >>> assertEqual(pr.product, product)
     >>> pr.quantity
     12.0
 
 Using zero as minimal quantity on order point also creates purchase request::
 
     >>> set_user(stock_admin_user)
     >>> order_point.min_quantity = 0
@@ -229,16 +225,15 @@
     >>> create_pr = Wizard('stock.supply')
     >>> create_pr.execute('create_')
 
 There is now a draft purchase request::
 
     >>> set_user(purchase_user)
     >>> pr, = PurchaseRequest.find([('state', '=', 'draft')])
-    >>> pr.product == product
-    True
+    >>> assertEqual(pr.product, product)
     >>> pr.quantity
     12.0
 
 Re-run with purchased request::
 
     >>> create_purchase = Wizard('purchase.request.create_purchase', [pr])
     >>> pr.state
```

### Comparing `trytond_stock_supply-7.0.2/tests/test_module.py` & `trytond_stock_supply-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/tox.ini` & `trytond_stock_supply-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/PKG-INFO` & `trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_supply
-Version: 7.0.2
+Version: 7.2.0
 Summary: Tryton module for stock supply
 Home-page: http://www.tryton.org/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
@@ -48,23 +48,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond_purchase_request<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond_purchase_request<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Stock Supply Module
 ###################
 
 The Stock Supply module add automatic supply mechanisms and introduce
 the concepts of order point.
```

### Comparing `trytond_stock_supply-7.0.2/trytond_stock_supply.egg-info/SOURCES.txt` & `trytond_stock_supply-7.2.0/trytond_stock_supply.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply-7.0.2/view/order_point_form.xml` & `trytond_stock_supply-7.2.0/view/order_point_form.xml`

 * *Files identical despite different names*

