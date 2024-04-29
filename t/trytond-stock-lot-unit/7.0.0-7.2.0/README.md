# Comparing `tmp/trytond_stock_lot_unit-7.0.0.tar.gz` & `tmp/trytond_stock_lot_unit-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_lot_unit-7.0.0.tar", last modified: Mon Oct 30 17:42:14 2023, max compression
+gzip compressed data, was "trytond_stock_lot_unit-7.2.0.tar", last modified: Mon Apr 29 15:51:36 2024, max compression
```

## Comparing `trytond_stock_lot_unit-7.0.0.tar` & `trytond_stock_lot_unit-7.2.0.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:14.852317 trytond_stock_lot_unit-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-10-22 17:23:25.000000 trytond_stock_lot_unit-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1084 2023-10-30 17:14:34.000000 trytond_stock_lot_unit-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-10-30 17:14:34.000000 trytond_stock_lot_unit-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_lot_unit-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2952 2023-10-30 17:42:14.852317 trytond_stock_lot_unit-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      853 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:14.848984 trytond_stock_lot_unit-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-10-22 17:23:25.000000 trytond_stock_lot_unit-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:25.000000 trytond_stock_lot_unit-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      254 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:14.845651 trytond_stock_lot_unit-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2331 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2404 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2332 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2272 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2674 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2379 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2437 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2404 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2023-10-30 16:47:45.000000 trytond_stock_lot_unit-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      802 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-10-24 07:56:52.000000 trytond_stock_lot_unit-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:21.000000 trytond_stock_lot_unit-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:42:14.852317 trytond_stock_lot_unit-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4383 2023-10-27 17:38:49.000000 trytond_stock_lot_unit-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7318 2023-10-24 07:56:52.000000 trytond_stock_lot_unit-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      986 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:14.845651 trytond_stock_lot_unit-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5680 2023-10-24 07:56:52.000000 trytond_stock_lot_unit-7.0.0/tests/scenario_stock_lot_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1930 2023-08-13 15:26:13.000000 trytond_stock_lot_unit-7.0.0/tests/scenario_stock_lot_unit_move_add.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_stock_lot_unit-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-10-30 17:14:30.000000 trytond_stock_lot_unit-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:14.852317 trytond_stock_lot_unit-7.0.0/trytond_stock_lot_unit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2952 2023-10-30 17:42:14.000000 trytond_stock_lot_unit-7.0.0/trytond_stock_lot_unit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1755 2023-10-30 17:42:14.000000 trytond_stock_lot_unit-7.0.0/trytond_stock_lot_unit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:42:14.000000 trytond_stock_lot_unit-7.0.0/trytond_stock_lot_unit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-10-30 17:42:14.000000 trytond_stock_lot_unit-7.0.0/trytond_stock_lot_unit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_stock_lot_unit-7.0.0/trytond_stock_lot_unit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      151 2023-10-30 17:42:14.000000 trytond_stock_lot_unit-7.0.0/trytond_stock_lot_unit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:42:14.000000 trytond_stock_lot_unit-7.0.0/trytond_stock_lot_unit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:14.848984 trytond_stock_lot_unit-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.0.0/view/lot_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-01-16 14:00:21.000000 trytond_stock_lot_unit-7.0.0/view/lot_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2023-10-24 07:56:52.000000 trytond_stock_lot_unit-7.0.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:36.055243 trytond_stock_lot_unit-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1185 2024-04-29 15:28:05.000000 trytond_stock_lot_unit-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2024-04-29 15:28:04.000000 trytond_stock_lot_unit-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_lot_unit-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2952 2024-04-29 15:51:36.055243 trytond_stock_lot_unit-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      853 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:36.048577 trytond_stock_lot_unit-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_stock_lot_unit-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:33.000000 trytond_stock_lot_unit-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      254 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:36.051910 trytond_stock_lot_unit-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2347 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2420 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2348 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2270 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2672 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2395 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2435 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2420 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2024-04-29 13:17:17.000000 trytond_stock_lot_unit-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      802 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1048 2024-04-27 16:30:39.000000 trytond_stock_lot_unit-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:21.000000 trytond_stock_lot_unit-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:51:36.055243 trytond_stock_lot_unit-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4383 2024-03-17 11:01:36.000000 trytond_stock_lot_unit-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7318 2024-04-22 12:01:28.000000 trytond_stock_lot_unit-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      986 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:36.051910 trytond_stock_lot_unit-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5551 2024-04-27 16:30:39.000000 trytond_stock_lot_unit-7.2.0/tests/scenario_stock_lot_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1924 2024-04-22 12:14:36.000000 trytond_stock_lot_unit-7.2.0/tests/scenario_stock_lot_unit_move_add.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:33.000000 trytond_stock_lot_unit-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-29 15:28:00.000000 trytond_stock_lot_unit-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:36.051910 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2952 2024-04-29 15:51:35.000000 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1737 2024-04-29 15:51:36.000000 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:51:35.000000 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:51:35.000000 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      151 2024-04-29 15:51:35.000000 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:51:35.000000 trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:36.051910 trytond_stock_lot_unit-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      413 2023-04-15 07:12:15.000000 trytond_stock_lot_unit-7.2.0/view/lot_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-01-16 14:00:21.000000 trytond_stock_lot_unit-7.2.0/view/lot_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-02-04 18:51:26.000000 trytond_stock_lot_unit-7.2.0/view/template_form.xml
```

### Comparing `trytond_stock_lot_unit-7.0.0/CHANGELOG` & `trytond_stock_lot_unit-7.2.0/CHANGELOG`

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
 * Rename Lot Unit to Lot UoM for product
 
 Version 6.8.0 - 2023-05-01
```

### Comparing `trytond_stock_lot_unit-7.0.0/COPYRIGHT` & `trytond_stock_lot_unit-7.2.0/COPYRIGHT`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (C) 2018-2023 Cédric Krier
+Copyright (C) 2018-2024 Cédric Krier
 Copyright (C) 2017-2023 Nicolas Évrard
-Copyright (C) 2017-2023 B2CK
+Copyright (C) 2017-2024 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_lot_unit-7.0.0/LICENSE` & `trytond_stock_lot_unit-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.0.0/PKG-INFO` & `trytond_stock_lot_unit-7.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_lot_unit
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to define unit on stock lot
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
@@ -46,21 +46,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_lot<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_lot<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_production<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_production<7.3,>=7.2; extra == "test"
 
 Stock Lot Unit Module
 #####################
 
 The ``stock_lot_unit`` module allows to define a unit and quantity on stock
 lot.
```

### Comparing `trytond_stock_lot_unit-7.0.0/__init__.py` & `trytond_stock_lot_unit-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.0.0/doc/conf.py` & `trytond_stock_lot_unit-7.2.0/doc/conf.py`

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

### Comparing `trytond_stock_lot_unit-7.0.0/locale/bg.po` & `trytond_stock_lot_unit-7.2.0/locale/bg.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/ca.po` & `trytond_stock_lot_unit-7.2.0/locale/ca.po`

 * *Files 6% similar despite different names*

```diff
@@ -30,20 +30,22 @@
 msgid "Unit"
 msgstr "Unitat"
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr "Quantitat unitària"
 
+#, fuzzy
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "La unitat de mesuera per defecte del lot."
 
+#, fuzzy
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "La unitat de mesuera per defecte del lot."
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr "La major unitat del lot."
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/cs.po` & `trytond_stock_lot_unit-7.2.0/locale/cs.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/de.po` & `trytond_stock_lot_unit-7.2.0/locale/de.po`

 * *Files 9% similar despite different names*

```diff
@@ -30,20 +30,22 @@
 msgid "Unit"
 msgstr "Einheit"
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr "Maßeinheit Menge"
 
+#, fuzzy
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "Die Standardmaßeinheit für Chargen."
 
+#, fuzzy
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "Die Standardmaßeinheit für Chargen."
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr "Die größte Maßeinheit für die Charge."
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/es.po` & `trytond_stock_lot_unit-7.2.0/locale/es.po`

 * *Files 5% similar despite different names*

```diff
@@ -30,20 +30,22 @@
 msgid "Unit"
 msgstr "Unidad"
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr "Cantidad unitaria"
 
+#, fuzzy
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "La unidad de medida por defecto del lote."
 
+#, fuzzy
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "La unidad de medida por defecto del lote."
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr "La mayor unidad del lote."
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/es_419.po` & `trytond_stock_lot_unit-7.2.0/locale/es_419.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/et.po` & `trytond_stock_lot_unit-7.2.0/locale/et.po`

 * *Files 5% similar despite different names*

```diff
@@ -38,20 +38,20 @@
 #, fuzzy
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr "Kogus"
 
 #, fuzzy
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "Partii vaikeühik."
 
 #, fuzzy
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "Partii vaikeühik."
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr "Partii suurim ühik."
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/fa.po` & `trytond_stock_lot_unit-7.2.0/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -38,20 +38,20 @@
 #, fuzzy
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr "مقدار"
 
 #, fuzzy
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "واحد پیشفرض قطعه."
 
 #, fuzzy
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "واحد پیشفرض قطعه."
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr "بزرگترین واحد برای قطعه"
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/fi.po` & `trytond_stock_lot_unit-7.2.0/locale/fi.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/fr.po` & `trytond_stock_lot_unit-7.2.0/locale/fr.po`

 * *Files 9% similar despite different names*

```diff
@@ -30,20 +30,22 @@
 msgid "Unit"
 msgstr "Unité"
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr "Quantité Unitaire"
 
+#, fuzzy
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "L'unité par défaut pour les lots."
 
+#, fuzzy
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "L'unité par défaut pour les lots."
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr "La plus grande unité pour le lot."
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/hu.po` & `trytond_stock_lot_unit-7.2.0/locale/hu.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/id.po` & `trytond_stock_lot_unit-7.2.0/locale/id.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/it.po` & `trytond_stock_lot_unit-7.2.0/locale/it.po`

 * *Files 4% similar despite different names*

```diff
@@ -35,20 +35,20 @@
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr "Quantità unitaria"
 
 #, fuzzy
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "L'unità predefinita per il lotto."
 
 #, fuzzy
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "L'unità predefinita per il lotto."
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr "L'unità più grande per il lotto."
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/lo.po` & `trytond_stock_lot_unit-7.2.0/locale/lo.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/lt.po` & `trytond_stock_lot_unit-7.2.0/locale/lt.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/nl.po` & `trytond_stock_lot_unit-7.2.0/locale/nl.po`

 * *Files 10% similar despite different names*

```diff
@@ -30,20 +30,22 @@
 msgid "Unit"
 msgstr "Eenheid"
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr "Eenheid Hoeveelheid"
 
+#, fuzzy
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "De standaard maateenheid voor een batch."
 
+#, fuzzy
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr "De standaard maateenheid voor een batch."
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr "De grootste eenheid voor een batch."
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/pl.po` & `trytond_stock_lot_unit-7.2.0/locale/pl.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/pt.po` & `trytond_stock_lot_unit-7.2.0/locale/pt.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/ro.po` & `trytond_stock_lot_unit-7.2.0/locale/ro.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/ru.po` & `trytond_stock_lot_unit-7.2.0/locale/ru.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/sl.po` & `trytond_stock_lot_unit-7.2.0/locale/sl.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/tr.po` & `trytond_stock_lot_unit-7.2.0/locale/tr.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/uk.po` & `trytond_stock_lot_unit-7.2.0/locale/uk.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/locale/zh_CN.po` & `trytond_stock_lot_unit-7.2.0/locale/zh_CN.po`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 msgstr ""
 
 msgctxt "field:stock.move.add.lots.start.lot,unit_quantity:"
 msgid "Unit Quantity"
 msgstr ""
 
 msgctxt "help:product.product,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:product.template,lot_uom:"
-msgid "The default unit of measurer for lot."
+msgid "The default unit of measure for lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit:"
 msgid "The biggest unit for the lot."
 msgstr ""
 
 msgctxt "help:stock.lot,unit_quantity:"
```

### Comparing `trytond_stock_lot_unit-7.0.0/message.xml` & `trytond_stock_lot_unit-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.0.0/product.py` & `trytond_stock_lot_unit-7.2.0/product.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     lot_uom = fields.Many2One('product.uom', "Lot UoM",
         domain=[
             ('category', '=', Eval('default_uom_category', -1)),
             ],
         states={
             'invisible': Eval('type') == 'service',
             },
-        help="The default unit of measurer for lot.")
+        help="The default unit of measure for lot.")
 
     @classmethod
     def __register__(cls, module_name):
         table_h = cls.__table_handler__(module_name)
 
         # Migration from 6.8: rename lot_unit to lot_uom
         if (table_h.column_exist('lot_unit')
```

### Comparing `trytond_stock_lot_unit-7.0.0/setup.py` & `trytond_stock_lot_unit-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.0.0/stock.py` & `trytond_stock_lot_unit-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.0.0/stock.xml` & `trytond_stock_lot_unit-7.2.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.0.0/tests/scenario_stock_lot_unit.rst` & `trytond_stock_lot_unit-7.2.0/tests/scenario_stock_lot_unit.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 =======================
 Stock Lot Unit Scenario
 =======================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import config, Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('stock_lot_unit')
 
 Create company::
 
@@ -72,22 +72,21 @@
     >>> move2.product = product
     >>> move2.quantity = 40
     >>> move2.unit_price = Decimal('8')
     >>> move2.currency = company.currency
     >>> move2.from_location = supplier_loc
     >>> move2.to_location = input_loc
     >>> shipment.click('receive')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
 
 Let's ship a product with a lot::
 
     >>> Lot = Model.get('stock.lot')
     >>> lot = Lot(number='00001', product=product)
-    >>> lot.unit == unit
-    True
+    >>> assertEqual(lot.unit, unit)
     >>> lot.unit_quantity
     1.0
     >>> lot.save()
 
     >>> ShipmentOut = Model.get('stock.shipment.out')
     >>> shipment = ShipmentOut()
     >>> shipment.customer = customer
@@ -99,15 +98,15 @@
     >>> move.from_location = output_loc
     >>> move.to_location = customer_loc
     >>> shipment.click('wait')
     >>> shipment.click('assign_try')
     >>> move.lot = lot
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
 
 Let's ship now two times the same lot::
 
     >>> lot = Lot(number='00002', product=product)
     >>> lot.save()
 
     >>> shipment = ShipmentOut()
@@ -128,15 +127,15 @@
     >>> move2.to_location = customer_loc
     >>> shipment.click('wait')
     >>> shipment.click('assign_try')
     >>> move1, move2 = shipment.inventory_moves
     >>> move1.lot = lot
     >>> move2.lot = lot
     >>> shipment.save()
-    >>> shipment.click('pick')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> shipment.click('pick')
     Traceback (most recent call last):
         ...
     LotUnitQuantityError: ...
 
 Now let's ship one move with a quantity bigger than lot unit quantity::
 
     >>> lot = Lot(number='00003', product=product)
@@ -152,15 +151,15 @@
     >>> move.currency = company.currency
     >>> move.from_location = output_loc
     >>> move.to_location = customer_loc
     >>> shipment.click('wait')
     >>> shipment.click('assign_try')
     >>> move, = shipment.inventory_moves
     >>> move.lot = lot
-    >>> shipment.click('pick')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> shipment.click('pick')
     Traceback (most recent call last):
         ...
     LotUnitQuantityError: ...
 
 Make an inventory::
 
     >>> lot = Lot(number='00004', product=product)
@@ -171,15 +170,15 @@
     >>> inventory = Inventory()
     >>> inventory.location = storage_loc
     >>> line = inventory.lines.new()
     >>> line.product = product
     >>> line.lot = lot
     >>> line.quantity = 3
     >>> inventory.save()
-    >>> inventory.click('confirm')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> inventory.click('confirm')
     Traceback (most recent call last):
         ...
     LotUnitQuantityError: ...
 
     >>> line, = inventory.lines
     >>> line.quantity = 2
     >>> inventory.click('confirm')
```

### Comparing `trytond_stock_lot_unit-7.0.0/tests/scenario_stock_lot_unit_move_add.rst` & `trytond_stock_lot_unit-7.2.0/tests/scenario_stock_lot_unit_move_add.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ================================
 Stock Lot Unit Move Add Scenario
 ================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('stock_lot_unit')
 
 Create company::
 
@@ -63,13 +63,12 @@
 
     >>> add_lots = move.click('add_lots_wizard')
     >>> lot = add_lots.form.lots.new()
     >>> lot.quantity
     5.0
     >>> lot.product = product  # proteus does not set reverse domain
     >>> lot.number = '01'
-    >>> lot.unit == unit
-    True
+    >>> assertEqual(lot.unit, unit)
     >>> lot.unit_quantity
     1.0
     >>> lot.quantity
     1.0
```

### Comparing `trytond_stock_lot_unit-7.0.0/tox.ini` & `trytond_stock_lot_unit-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_unit-7.0.0/trytond_stock_lot_unit.egg-info/PKG-INFO` & `trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-stock-lot-unit
-Version: 7.0.0
+Name: trytond_stock_lot_unit
+Version: 7.2.0
 Summary: Tryton module to define unit on stock lot
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
@@ -46,21 +46,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_lot<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_lot<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_production<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_production<7.3,>=7.2; extra == "test"
 
 Stock Lot Unit Module
 #####################
 
 The ``stock_lot_unit`` module allows to define a unit and quantity on stock
 lot.
```

### Comparing `trytond_stock_lot_unit-7.0.0/trytond_stock_lot_unit.egg-info/SOURCES.txt` & `trytond_stock_lot_unit-7.2.0/trytond_stock_lot_unit.egg-info/SOURCES.txt`

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
 exceptions.py
```

