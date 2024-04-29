# Comparing `tmp/trytond_product_cost_fifo-7.0.0.tar.gz` & `tmp/trytond_product_cost_fifo-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_cost_fifo-7.0.0.tar", last modified: Mon Oct 30 17:32:26 2023, max compression
+gzip compressed data, was "trytond_product_cost_fifo-7.2.0.tar", last modified: Mon Apr 29 15:42:48 2024, max compression
```

## Comparing `trytond_product_cost_fifo-7.0.0.tar` & `trytond_product_cost_fifo-7.2.0.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:26.859513 trytond_product_cost_fifo-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2023-10-22 17:23:08.000000 trytond_product_cost_fifo-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2658 2023-10-30 17:08:43.000000 trytond_product_cost_fifo-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:08:43.000000 trytond_product_cost_fifo-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_cost_fifo-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3004 2023-10-30 17:32:26.859513 trytond_product_cost_fifo-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-01-16 14:00:20.000000 trytond_product_cost_fifo-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:26.856180 trytond_product_cost_fifo-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2818 2023-10-22 17:23:08.000000 trytond_product_cost_fifo-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-01-16 14:00:20.000000 trytond_product_cost_fifo-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:08.000000 trytond_product_cost_fifo-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:26.856180 trytond_product_cost_fifo-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1125 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1427 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1480 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1434 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1306 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1538 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1492 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1214 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1513 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1478 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1465 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1208 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1417 2023-10-30 16:47:45.000000 trytond_product_cost_fifo-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1175 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2023-10-28 12:11:23.000000 trytond_product_cost_fifo-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      827 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6559 2023-10-07 17:14:58.000000 trytond_product_cost_fifo-7.0.0/move.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9974 2023-10-07 17:14:58.000000 trytond_product_cost_fifo-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:32:26.859513 trytond_product_cost_fifo-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4473 2023-10-27 17:38:49.000000 trytond_product_cost_fifo-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:26.856180 trytond_product_cost_fifo-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4856 2023-10-07 17:14:58.000000 trytond_product_cost_fifo-7.0.0/tests/scenario_product_cost_fifo.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3245 2023-10-07 17:14:58.000000 trytond_product_cost_fifo-7.0.0/tests/scenario_product_cost_fifo_no_in.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4849 2023-10-07 15:40:36.000000 trytond_product_cost_fifo-7.0.0/tests/scenario_product_cost_fifo_recompute_cost_price.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3421 2023-10-07 15:40:36.000000 trytond_product_cost_fifo-7.0.0/tests/scenario_product_cost_fifo_recompute_cost_price_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4687 2023-10-07 17:14:58.000000 trytond_product_cost_fifo-7.0.0/tests/scenario_product_cost_fifo_uom.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_product_cost_fifo-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-10-30 17:08:39.000000 trytond_product_cost_fifo-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:26.856180 trytond_product_cost_fifo-7.0.0/trytond_product_cost_fifo.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3004 2023-10-30 17:32:26.000000 trytond_product_cost_fifo-7.0.0/trytond_product_cost_fifo.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1920 2023-10-30 17:32:26.000000 trytond_product_cost_fifo-7.0.0/trytond_product_cost_fifo.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:32:26.000000 trytond_product_cost_fifo-7.0.0/trytond_product_cost_fifo.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2023-10-30 17:32:26.000000 trytond_product_cost_fifo-7.0.0/trytond_product_cost_fifo.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_product_cost_fifo-7.0.0/trytond_product_cost_fifo.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      105 2023-10-30 17:32:26.000000 trytond_product_cost_fifo-7.0.0/trytond_product_cost_fifo.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:32:26.000000 trytond_product_cost_fifo-7.0.0/trytond_product_cost_fifo.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:48.752368 trytond_product_cost_fifo-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2759 2024-04-29 15:21:34.000000 trytond_product_cost_fifo-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:21:33.000000 trytond_product_cost_fifo-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_cost_fifo-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3004 2024-04-29 15:42:48.752368 trytond_product_cost_fifo-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-01-16 14:00:20.000000 trytond_product_cost_fifo-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:48.749035 trytond_product_cost_fifo-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-27 16:30:39.000000 trytond_product_cost_fifo-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-01-16 14:00:20.000000 trytond_product_cost_fifo-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:15.000000 trytond_product_cost_fifo-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:48.749035 trytond_product_cost_fifo-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1125 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1427 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1480 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1434 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1306 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1538 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1492 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1214 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1513 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1478 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1465 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1208 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1417 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1175 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      827 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6559 2024-02-04 18:51:26.000000 trytond_product_cost_fifo-7.2.0/move.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9974 2024-02-04 18:51:26.000000 trytond_product_cost_fifo-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:42:48.752368 trytond_product_cost_fifo-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4473 2024-03-17 11:01:36.000000 trytond_product_cost_fifo-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:48.752368 trytond_product_cost_fifo-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4836 2024-04-22 12:14:36.000000 trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3233 2024-04-22 12:14:36.000000 trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_no_in.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4837 2024-04-22 12:14:36.000000 trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_recompute_cost_price.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3406 2024-04-22 12:14:36.000000 trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_recompute_cost_price_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4610 2024-04-22 12:14:36.000000 trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_uom.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:15.000000 trytond_product_cost_fifo-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:21:29.000000 trytond_product_cost_fifo-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:48.752368 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3004 2024-04-29 15:42:48.000000 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1902 2024-04-29 15:42:48.000000 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:42:48.000000 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-29 15:42:48.000000 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      105 2024-04-29 15:42:48.000000 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:42:48.000000 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/top_level.txt
```

### Comparing `trytond_product_cost_fifo-7.0.0/CHANGELOG` & `trytond_product_cost_fifo-7.2.0/CHANGELOG`

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
 * Fill product cost price on outgoing stock move
 
 Version 6.8.0 - 2023-05-01
```

### Comparing `trytond_product_cost_fifo-7.0.0/LICENSE` & `trytond_product_cost_fifo-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/PKG-INFO` & `trytond_product_cost_fifo-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_product_cost_fifo
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add FIFO cost method
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
@@ -49,19 +49,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Product Cost FIFO Module
 ########################
 
 The Product Cost FIFO Module add a *FIFO* option in the Cost Method
 field of the product form.
```

### Comparing `trytond_product_cost_fifo-7.0.0/doc/conf.py` & `trytond_product_cost_fifo-7.2.0/doc/conf.py`

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

### Comparing `trytond_product_cost_fifo-7.0.0/locale/bg.po` & `trytond_product_cost_fifo-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/ca.po` & `trytond_product_cost_fifo-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/cs.po` & `trytond_product_cost_fifo-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/de.po` & `trytond_product_cost_fifo-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/es.po` & `trytond_product_cost_fifo-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/es_419.po` & `trytond_product_cost_fifo-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/et.po` & `trytond_product_cost_fifo-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/fa.po` & `trytond_product_cost_fifo-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/fi.po` & `trytond_product_cost_fifo-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/fr.po` & `trytond_product_cost_fifo-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/hu.po` & `trytond_product_cost_fifo-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/id.po` & `trytond_product_cost_fifo-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/it.po` & `trytond_product_cost_fifo-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/lo.po` & `trytond_product_cost_fifo-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/lt.po` & `trytond_product_cost_fifo-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/nl.po` & `trytond_product_cost_fifo-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/pl.po` & `trytond_product_cost_fifo-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/pt.po` & `trytond_product_cost_fifo-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/ro.po` & `trytond_product_cost_fifo-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/ru.po` & `trytond_product_cost_fifo-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/sl.po` & `trytond_product_cost_fifo-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/tr.po` & `trytond_product_cost_fifo-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/uk.po` & `trytond_product_cost_fifo-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/locale/zh_CN.po` & `trytond_product_cost_fifo-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/message.xml` & `trytond_product_cost_fifo-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/move.py` & `trytond_product_cost_fifo-7.2.0/move.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/product.py` & `trytond_product_cost_fifo-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/setup.py` & `trytond_product_cost_fifo-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/tests/scenario_product_cost_fifo.rst` & `trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 Stock FIFO Cost Price
 =====================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('product_cost_fifo')
 
 Create company::
```

### Comparing `trytond_product_cost_fifo-7.0.0/tests/scenario_product_cost_fifo_no_in.rst` & `trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_no_in.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 Stock FIFO Cost Price with no Input
 ===================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('product_cost_fifo')
 
 Create company::
```

### Comparing `trytond_product_cost_fifo-7.0.0/tests/scenario_product_cost_fifo_recompute_cost_price.rst` & `trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_recompute_cost_price.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 Product Cost FIFO Recompute Cost Price
 ======================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('product_cost_fifo')
 
 Create company::
```

### Comparing `trytond_product_cost_fifo-7.0.0/tests/scenario_product_cost_fifo_recompute_cost_price_production.rst` & `trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_recompute_cost_price_production.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
 
     >>> today = dt.date.today()
     >>> yesterday = today - dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('product_cost_fifo')
```

### Comparing `trytond_product_cost_fifo-7.0.0/tests/scenario_product_cost_fifo_uom.rst` & `trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_uom.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 =========================
 Stock FIFO Cost Price UoM
 =========================
 
 Imports::
 
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('product_cost_fifo')
 
 Create company::
```

### Comparing `trytond_product_cost_fifo-7.0.0/tox.ini` & `trytond_product_cost_fifo-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.0.0/trytond_product_cost_fifo.egg-info/PKG-INFO` & `trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-product-cost-fifo
-Version: 7.0.0
+Name: trytond_product_cost_fifo
+Version: 7.2.0
 Summary: Tryton module to add FIFO cost method
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
@@ -49,19 +49,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Product Cost FIFO Module
 ########################
 
 The Product Cost FIFO Module add a *FIFO* option in the Cost Method
 field of the product form.
```

### Comparing `trytond_product_cost_fifo-7.0.0/trytond_product_cost_fifo.egg-info/SOURCES.txt` & `trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

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

