# Comparing `tmp/trytond_stock_location_move-7.0.0.tar.gz` & `tmp/trytond_stock_location_move-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_location_move-7.0.0.tar", last modified: Mon Oct 30 17:41:43 2023, max compression
+gzip compressed data, was "trytond_stock_location_move-7.2.0.tar", last modified: Mon Apr 29 15:51:10 2024, max compression
```

## Comparing `trytond_stock_location_move-7.0.0.tar` & `trytond_stock_location_move-7.2.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:43.932170 trytond_stock_location_move-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      219 2023-10-22 17:23:24.000000 trytond_stock_location_move-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1221 2023-10-30 17:14:17.000000 trytond_stock_location_move-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-10-30 17:14:16.000000 trytond_stock_location_move-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_location_move-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2953 2023-10-30 17:41:43.932170 trytond_stock_location_move-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      586 2023-10-07 15:40:36.000000 trytond_stock_location_move-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:43.932170 trytond_stock_location_move-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2820 2023-10-22 17:23:24.000000 trytond_stock_location_move-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      586 2023-10-07 15:40:36.000000 trytond_stock_location_move-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:24.000000 trytond_stock_location_move-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:43.928836 trytond_stock_location_move-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1240 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1223 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1252 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1030 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1073 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1295 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1291 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1036 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1230 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1100 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1030 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1030 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-10-28 12:11:26.000000 trytond_stock_location_move-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      898 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:41:43.932170 trytond_stock_location_move-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4458 2023-10-27 17:38:49.000000 trytond_stock_location_move-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9001 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3438 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:43.932170 trytond_stock_location_move-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3735 2023-08-13 15:26:13.000000 trytond_stock_location_move-7.0.0/tests/scenario_stock_location_move.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5101 2023-08-13 15:26:13.000000 trytond_stock_location_move-7.0.0/tests/scenario_stock_location_move_empty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3253 2023-06-10 11:39:56.000000 trytond_stock_location_move-7.0.0/tests/scenario_stock_location_move_supply.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_stock_location_move-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      116 2023-10-30 17:14:13.000000 trytond_stock_location_move-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:43.932170 trytond_stock_location_move-7.0.0/trytond_stock_location_move.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2953 2023-10-30 17:41:43.000000 trytond_stock_location_move-7.0.0/trytond_stock_location_move.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1832 2023-10-30 17:41:43.000000 trytond_stock_location_move-7.0.0/trytond_stock_location_move.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:41:43.000000 trytond_stock_location_move-7.0.0/trytond_stock_location_move.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-10-30 17:41:43.000000 trytond_stock_location_move-7.0.0/trytond_stock_location_move.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_stock_location_move-7.0.0/trytond_stock_location_move.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       99 2023-10-30 17:41:43.000000 trytond_stock_location_move-7.0.0/trytond_stock_location_move.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:41:43.000000 trytond_stock_location_move-7.0.0/trytond_stock_location_move.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:43.932170 trytond_stock_location_move-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-01-16 14:00:21.000000 trytond_stock_location_move-7.0.0/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-01-16 14:00:21.000000 trytond_stock_location_move-7.0.0/view/shipment_internal_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:10.432580 trytond_stock_location_move-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1322 2024-04-29 15:27:44.000000 trytond_stock_location_move-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:27:43.000000 trytond_stock_location_move-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_location_move-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2953 2024-04-29 15:51:10.432580 trytond_stock_location_move-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      586 2024-02-04 18:51:26.000000 trytond_stock_location_move-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      702 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:10.429247 trytond_stock_location_move-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3082 2024-04-27 16:30:39.000000 trytond_stock_location_move-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      586 2024-02-04 18:51:26.000000 trytond_stock_location_move-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:32.000000 trytond_stock_location_move-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:10.432580 trytond_stock_location_move-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1240 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1223 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1252 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1030 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1073 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1295 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1291 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1036 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1230 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1100 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1030 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1030 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-27 16:43:27.000000 trytond_stock_location_move-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      898 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:51:10.432580 trytond_stock_location_move-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4458 2024-03-17 11:01:36.000000 trytond_stock_location_move-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8931 2024-04-27 16:30:39.000000 trytond_stock_location_move-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3369 2024-04-27 16:30:39.000000 trytond_stock_location_move-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:10.432580 trytond_stock_location_move-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3657 2024-04-27 16:30:39.000000 trytond_stock_location_move-7.2.0/tests/scenario_stock_location_move.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5077 2024-04-27 16:30:39.000000 trytond_stock_location_move-7.2.0/tests/scenario_stock_location_move_empty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3239 2024-04-22 12:14:37.000000 trytond_stock_location_move-7.2.0/tests/scenario_stock_location_move_supply.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_location_move-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:32.000000 trytond_stock_location_move-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      116 2024-04-29 15:27:39.000000 trytond_stock_location_move-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:10.432580 trytond_stock_location_move-7.2.0/trytond_stock_location_move.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2953 2024-04-29 15:51:09.000000 trytond_stock_location_move-7.2.0/trytond_stock_location_move.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1814 2024-04-29 15:51:10.000000 trytond_stock_location_move-7.2.0/trytond_stock_location_move.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:51:09.000000 trytond_stock_location_move-7.2.0/trytond_stock_location_move.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2024-04-29 15:51:09.000000 trytond_stock_location_move-7.2.0/trytond_stock_location_move.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_stock_location_move-7.2.0/trytond_stock_location_move.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       99 2024-04-29 15:51:09.000000 trytond_stock_location_move-7.2.0/trytond_stock_location_move.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:51:09.000000 trytond_stock_location_move-7.2.0/trytond_stock_location_move.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:10.432580 trytond_stock_location_move-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-01-16 14:00:21.000000 trytond_stock_location_move-7.2.0/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-01-16 14:00:21.000000 trytond_stock_location_move-7.2.0/view/shipment_internal_form.xml
```

### Comparing `trytond_stock_location_move-7.0.0/CHANGELOG` & `trytond_stock_location_move-7.2.0/CHANGELOG`

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

### Comparing `trytond_stock_location_move-7.0.0/COPYRIGHT` & `trytond_stock_location_move-7.2.0/COPYRIGHT`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2017-2023 Cédric Krier
+Copyright (C) 2017-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_location_move-7.0.0/LICENSE` & `trytond_stock_location_move-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/PKG-INFO` & `trytond_stock_location_move-7.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_location_move
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to move storage locations
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
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_supply<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_supply<7.3,>=7.2; extra == "test"
 
 Stock Location Move Module
 ##########################
 
 The stock location move module allows to define some *Locations* as movable
 (like pallet).
```

### Comparing `trytond_stock_location_move-7.0.0/README.rst` & `trytond_stock_location_move-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/__init__.py` & `trytond_stock_location_move-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/doc/conf.py` & `trytond_stock_location_move-7.2.0/doc/conf.py`

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

### Comparing `trytond_stock_location_move-7.0.0/doc/index.rst` & `trytond_stock_location_move-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/bg.po` & `trytond_stock_location_move-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/ca.po` & `trytond_stock_location_move-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/cs.po` & `trytond_stock_location_move-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/de.po` & `trytond_stock_location_move-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/es.po` & `trytond_stock_location_move-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/es_419.po` & `trytond_stock_location_move-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/et.po` & `trytond_stock_location_move-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/fa.po` & `trytond_stock_location_move-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/fi.po` & `trytond_stock_location_move-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/fr.po` & `trytond_stock_location_move-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/hu.po` & `trytond_stock_location_move-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/id.po` & `trytond_stock_location_move-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/it.po` & `trytond_stock_location_move-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/lo.po` & `trytond_stock_location_move-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/lt.po` & `trytond_stock_location_move-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/nl.po` & `trytond_stock_location_move-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/pl.po` & `trytond_stock_location_move-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/pt.po` & `trytond_stock_location_move-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/ro.po` & `trytond_stock_location_move-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/ru.po` & `trytond_stock_location_move-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/sl.po` & `trytond_stock_location_move-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/tr.po` & `trytond_stock_location_move-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/uk.po` & `trytond_stock_location_move-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/locale/zh_CN.po` & `trytond_stock_location_move-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/product.py` & `trytond_stock_location_move-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/setup.py` & `trytond_stock_location_move-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/stock.py` & `trytond_stock_location_move-7.2.0/stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,28 +181,28 @@
             Location.write(*to_write)
         super(ShipmentInternal, cls).ship(shipments)
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
     @clear_location_assignation
-    def done(cls, shipments):
+    def do(cls, shipments):
         pool = Pool()
         Location = pool.get('stock.location')
         to_write = []
         for shipment in shipments:
             if not shipment.locations:
                 continue
             to_write.append(list(shipment.locations))
             to_write.append({
                     'parent': shipment.to_location.id,
                     })
         if to_write:
             Location.write(*to_write)
-        super(ShipmentInternal, cls).done(shipments)
+        super().do(shipments)
 
     @classmethod
     @ModelView.button
     @Workflow.transition('cancelled')
     @clear_location_assignation
     def cancel(cls, shipments):
         super(ShipmentInternal, cls).cancel(shipments)
@@ -240,27 +240,27 @@
 class ShipmentOut(metaclass=PoolMeta):
     __name__ = 'stock.shipment.out'
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
     @deactivate_empty_location
-    def done(cls, shipments):
-        super(ShipmentOut, cls).done(shipments)
+    def do(cls, shipments):
+        super().do(shipments)
 
 
 class ShipmentInReturn(metaclass=PoolMeta):
     __name__ = 'stock.shipment.in.return'
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
     @deactivate_empty_location
-    def done(cls, shipments):
-        super(ShipmentInReturn, cls).done(shipments)
+    def do(cls, shipments):
+        super().do(shipments)
 
 
 class Supply(metaclass=PoolMeta):
     __name__ = 'stock.supply'
 
     def transition_create_(self):
         with Transaction().set_context(forecast_location_move=True):
```

### Comparing `trytond_stock_location_move-7.0.0/stock.xml` & `trytond_stock_location_move-7.2.0/stock.xml`

 * *Files 16% similar despite different names*

#### Comparing `trytond_stock_location_move-7.0.0/stock.xml` & `trytond_stock_location_move-7.2.0/stock.xml`

```diff
@@ -7,24 +7,24 @@
       <field name="name">Stock Location Movable</field>
     </record>
     <record model="res.user-res.group" id="user_admin_group_stock_location_movable">
       <field name="user" ref="res.user_admin"/>
       <field name="group" ref="group_stock_location_movable"/>
     </record>
     <record model="ir.model.access" id="access_location">
-      <field name="model" search="[('model', '=', 'stock.location')]"/>
+      <field name="model">stock.location</field>
       <field name="group" ref="group_stock_location_movable"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.rule.group" id="rule_group_location_movable">
       <field name="name">Movable location</field>
-      <field name="model" search="[('model', '=', 'stock.location')]"/>
+      <field name="model">stock.location</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="False"/>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="False"/>
     </record>
@@ -34,15 +34,15 @@
     </record>
     <record model="ir.rule.group-res.group" id="rule_group_location_movable_group_stock_location_movable">
       <field name="rule_group" ref="rule_group_location_movable"/>
       <field name="group" ref="group_stock_location_movable"/>
     </record>
     <record model="ir.rule.group" id="rule_group_location_movable_admin">
       <field name="name">Any location</field>
-      <field name="model" search="[('model', '=', 'stock.location')]"/>
+      <field name="model">stock.location</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="False"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
```

### Comparing `trytond_stock_location_move-7.0.0/tests/scenario_stock_location_move.rst` & `trytond_stock_location_move-7.2.0/tests/scenario_stock_location_move.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Stock Location Move Scenario
 ============================
 
 Imports::
 
     >>> import datetime as dt
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
+
     >>> today = dt.date.today()
     >>> tomorrow = today + dt.timedelta(1)
 
 Activate modules::
 
     >>> config = activate_modules('stock_location_move')
 
@@ -42,35 +42,32 @@
     >>> shipment.locations.append(Location(pallet.id))
     >>> shipment.click('wait')
 
     >>> shipment.click('assign_try')
     >>> shipment.state
     'assigned'
     >>> pallet.reload()
-    >>> pallet.assigned_by == shipment
-    True
-    >>> pallet.parent == storage1
-    True
+    >>> assertEqual(pallet.assigned_by, shipment)
+    >>> assertEqual(pallet.parent, storage1)
 
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
     >>> pallet.reload()
     >>> pallet.assigned_by
-    >>> pallet.parent == storage2
-    True
+    >>> assertEqual(pallet.parent, storage2)
 
 Assign pallet from wrong location::
 
     >>> shipment = Shipment()
     >>> shipment.from_location = storage1
     >>> shipment.to_location = storage2
     >>> shipment.locations.append(Location(pallet.id))
     >>> shipment.click('wait')
-    >>> shipment.click('assign_try')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> shipment.click('assign_try')
     Traceback (most recent call last):
         ...
     DomainValidationError: ...
 
 Concurrently move pallet::
 
     >>> shipment1 = Shipment()
@@ -84,20 +81,20 @@
     >>> shipment2.to_location = storage1
     >>> shipment2.locations.append(Location(pallet.id))
     >>> shipment2.click('wait')
 
     >>> shipment1.click('assign_try')
     >>> shipment1.state
     'assigned'
-    >>> shipment2.click('assign_try')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> shipment2.click('assign_try')
     Traceback (most recent call last):
         ...
     AssignError: ...
 
-    >>> shipment1.click('done')
+    >>> shipment1.click('do')
 
 Add lead time between warehouses::
 
     >>> warehouse1 = storage_loc.warehouse
     >>> warehouse2, = warehouse1.duplicate()
 
     >>> LeadTime = Model.get('stock.location.lead_time')
@@ -116,14 +113,12 @@
     >>> shipment.to_location = warehouse2.storage_location
     >>> shipment.locations.append(Location(pallet.id))
     >>> shipment.click('wait')
     >>> shipment.click('assign_try')
 
     >>> shipment.click('ship')
     >>> pallet.reload()
-    >>> pallet.parent == shipment.transit_location
-    True
+    >>> assertEqual(pallet.parent, shipment.transit_location)
 
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> pallet.reload()
-    >>> pallet.parent == warehouse2.storage_location
-    True
+    >>> assertEqual(pallet.parent, warehouse2.storage_location)
```

### Comparing `trytond_stock_location_move-7.0.0/tests/scenario_stock_location_move_empty.rst` & `trytond_stock_location_move-7.2.0/tests/scenario_stock_location_move_empty.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 ==================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
 
     >>> today = dt.date.today()
     >>> yesterday = today - dt.timedelta(1)
     >>> tomorrow = today + dt.timedelta(1)
 
 Activate modules::
 
@@ -131,15 +130,15 @@
     >>> move.currency = company.currency
     >>> move.from_location = output_loc
     >>> move.to_location = customer_loc
     >>> shipment.click('wait')
     >>> shipment.click('assign_try')
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
 
 Check empty non movable location are still active::
 
     >>> storage1.reload()
     >>> bool(storage1.active)
     True
```

### Comparing `trytond_stock_location_move-7.0.0/tests/scenario_stock_location_move_supply.rst` & `trytond_stock_location_move-7.2.0/tests/scenario_stock_location_move_supply.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules(['stock_location_move', 'stock_supply'])
```

### Comparing `trytond_stock_location_move-7.0.0/tox.ini` & `trytond_stock_location_move-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_location_move-7.0.0/trytond_stock_location_move.egg-info/PKG-INFO` & `trytond_stock_location_move-7.2.0/trytond_stock_location_move.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-stock-location-move
-Version: 7.0.0
+Name: trytond_stock_location_move
+Version: 7.2.0
 Summary: Tryton module to move storage locations
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
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_supply<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_supply<7.3,>=7.2; extra == "test"
 
 Stock Location Move Module
 ##########################
 
 The stock location move module allows to define some *Locations* as movable
 (like pallet).
```

### Comparing `trytond_stock_location_move-7.0.0/trytond_stock_location_move.egg-info/SOURCES.txt` & `trytond_stock_location_move-7.2.0/trytond_stock_location_move.egg-info/SOURCES.txt`

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
 message.xml
```

