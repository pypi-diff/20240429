# Comparing `tmp/trytond_product_cost_history-7.0.0.tar.gz` & `tmp/trytond_product_cost_history-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_cost_history-7.0.0.tar", last modified: Mon Oct 30 17:32:33 2023, max compression
+gzip compressed data, was "trytond_product_cost_history-7.2.0.tar", last modified: Mon Apr 29 15:42:55 2024, max compression
```

## Comparing `trytond_product_cost_history-7.0.0.tar` & `trytond_product_cost_history-7.2.0.tar`

### file list

```diff
@@ -1,60 +1,59 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:33.866213 trytond_product_cost_history-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-10-22 17:23:09.000000 trytond_product_cost_history-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2662 2023-10-30 17:08:48.000000 trytond_product_cost_history-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2023-10-30 17:08:47.000000 trytond_product_cost_history-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_cost_history-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2939 2023-10-30 17:32:33.866213 trytond_product_cost_history-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:33.866213 trytond_product_cost_history-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2821 2023-10-22 17:23:09.000000 trytond_product_cost_history-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:09.000000 trytond_product_cost_history-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:33.862880 trytond_product_cost_history-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      633 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      587 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      591 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      546 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      599 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      586 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      592 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      513 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      593 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      623 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      576 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      574 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      588 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      572 2023-10-30 16:47:45.000000 trytond_product_cost_history-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      500 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      541 2023-10-28 12:11:23.000000 trytond_product_cost_history-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6804 2023-10-07 15:40:36.000000 trytond_product_cost_history-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2100 2023-01-16 14:00:20.000000 trytond_product_cost_history-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:32:33.866213 trytond_product_cost_history-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4470 2023-10-27 17:38:49.000000 trytond_product_cost_history-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:33.862880 trytond_product_cost_history-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5152 2023-08-13 15:26:13.000000 trytond_product_cost_history-7.0.0/tests/scenario_product_cost_history.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_product_cost_history-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-10-30 17:08:44.000000 trytond_product_cost_history-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:33.866213 trytond_product_cost_history-7.0.0/trytond_product_cost_history.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2939 2023-10-30 17:32:33.000000 trytond_product_cost_history-7.0.0/trytond_product_cost_history.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1645 2023-10-30 17:32:33.000000 trytond_product_cost_history-7.0.0/trytond_product_cost_history.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:32:33.000000 trytond_product_cost_history-7.0.0/trytond_product_cost_history.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-10-30 17:32:33.000000 trytond_product_cost_history-7.0.0/trytond_product_cost_history.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_product_cost_history-7.0.0/trytond_product_cost_history.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      105 2023-10-30 17:32:33.000000 trytond_product_cost_history-7.0.0/trytond_product_cost_history.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:32:33.000000 trytond_product_cost_history-7.0.0/trytond_product_cost_history.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:33.866213 trytond_product_cost_history-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-01-16 14:00:20.000000 trytond_product_cost_history-7.0.0/view/product_cost_history_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      270 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.0.0/view/product_cost_history_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:55.235531 trytond_product_cost_history-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2763 2024-04-29 15:21:39.000000 trytond_product_cost_history-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:21:38.000000 trytond_product_cost_history-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_cost_history-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2939 2024-04-29 15:42:55.235531 trytond_product_cost_history-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:55.232198 trytond_product_cost_history-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-27 16:30:39.000000 trytond_product_cost_history-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:15.000000 trytond_product_cost_history-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:55.235531 trytond_product_cost_history-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      633 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      587 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      591 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      546 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      599 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      586 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      592 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      513 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      593 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      623 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      576 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      575 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      585 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      574 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      588 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      572 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      500 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      541 2024-04-27 16:43:24.000000 trytond_product_cost_history-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6804 2024-02-04 18:51:26.000000 trytond_product_cost_history-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2100 2023-01-16 14:00:20.000000 trytond_product_cost_history-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:42:55.235531 trytond_product_cost_history-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4470 2024-03-17 11:01:36.000000 trytond_product_cost_history-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:55.235531 trytond_product_cost_history-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5105 2024-04-22 12:14:36.000000 trytond_product_cost_history-7.2.0/tests/scenario_product_cost_history.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:15.000000 trytond_product_cost_history-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:21:34.000000 trytond_product_cost_history-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:55.235531 trytond_product_cost_history-7.2.0/trytond_product_cost_history.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2939 2024-04-29 15:42:54.000000 trytond_product_cost_history-7.2.0/trytond_product_cost_history.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1627 2024-04-29 15:42:55.000000 trytond_product_cost_history-7.2.0/trytond_product_cost_history.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:42:54.000000 trytond_product_cost_history-7.2.0/trytond_product_cost_history.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:42:54.000000 trytond_product_cost_history-7.2.0/trytond_product_cost_history.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_product_cost_history-7.2.0/trytond_product_cost_history.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      105 2024-04-29 15:42:54.000000 trytond_product_cost_history-7.2.0/trytond_product_cost_history.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:42:54.000000 trytond_product_cost_history-7.2.0/trytond_product_cost_history.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:55.235531 trytond_product_cost_history-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-01-16 14:00:20.000000 trytond_product_cost_history-7.2.0/view/product_cost_history_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      270 2023-04-15 07:12:15.000000 trytond_product_cost_history-7.2.0/view/product_cost_history_tree.xml
```

### Comparing `trytond_product_cost_history-7.0.0/CHANGELOG` & `trytond_product_cost_history-7.2.0/CHANGELOG`

 * *Files 5% similar despite different names*

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
 * Use product cost price from stock move for cost history
 
 Version 6.8.0 - 2023-05-01
```

### Comparing `trytond_product_cost_history-7.0.0/COPYRIGHT` & `trytond_product_cost_history-7.2.0/COPYRIGHT`

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

### Comparing `trytond_product_cost_history-7.0.0/LICENSE` & `trytond_product_cost_history-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/PKG-INFO` & `trytond_product_cost_history-7.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_product_cost_history
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to historize product cost
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
 
 Product Cost History Module
 ###########################
 
 The Product Cost History Module adds a *Cost History* relate on the product
 form showing the cost price evolution of the product. The history is based on
 the cost price stored on the incoming stock moves for goods and assets and
```

### Comparing `trytond_product_cost_history-7.0.0/doc/conf.py` & `trytond_product_cost_history-7.2.0/doc/conf.py`

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

### Comparing `trytond_product_cost_history-7.0.0/locale/bg.po` & `trytond_product_cost_history-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/ca.po` & `trytond_product_cost_history-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/cs.po` & `trytond_product_cost_history-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/de.po` & `trytond_product_cost_history-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/es.po` & `trytond_product_cost_history-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/es_419.po` & `trytond_product_cost_history-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/et.po` & `trytond_product_cost_history-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/fa.po` & `trytond_product_cost_history-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/fi.po` & `trytond_product_cost_history-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/fr.po` & `trytond_product_cost_history-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/hu.po` & `trytond_product_cost_history-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/id.po` & `trytond_product_cost_history-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/it.po` & `trytond_product_cost_history-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/lo.po` & `trytond_product_cost_history-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/lt.po` & `trytond_product_cost_history-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/nl.po` & `trytond_product_cost_history-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/pl.po` & `trytond_product_cost_history-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/pt.po` & `trytond_product_cost_history-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/ro.po` & `trytond_product_cost_history-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/ru.po` & `trytond_product_cost_history-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/sl.po` & `trytond_product_cost_history-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/tr.po` & `trytond_product_cost_history-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/locale/zh_CN.po` & `trytond_product_cost_history-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/product.py` & `trytond_product_cost_history-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/product.xml` & `trytond_product_cost_history-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/setup.py` & `trytond_product_cost_history-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/tests/scenario_product_cost_history.rst` & `trytond_product_cost_history-7.2.0/tests/scenario_product_cost_history.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 ====================
 Product Cost History
 ====================
 
 Imports::
 
     >>> import datetime as dt
-    >>> import time
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('product_cost_history')
 
     >>> Date = Model.get('ir.date')
 
@@ -105,22 +104,20 @@
     ...     currency=company.currency,
     ...     effective_date=today).click('do')
 
 
 Check cost history::
 
     >>> order = [('date', 'ASC')]
-    >>> [c.cost_price for c in ProductCostHistory.find([], order=order)] == [
-    ...     Decimal('100.0000'), Decimal('120.0000'), Decimal('110.0000')]
-    True
-    >>> [c.date for c in ProductCostHistory.find([], order=order)] == [
+    >>> [c.cost_price for c in ProductCostHistory.find([], order=order)]
+    [Decimal('100.0000'), Decimal('120.0000'), Decimal('110.0000')]
+    >>> assertEqual([c.date for c in ProductCostHistory.find([], order=order)], [
     ...     today - dt.timedelta(days=2),
     ...     today - dt.timedelta(days=1),
-    ...     today]
-    True
+    ...     today])
 
 Check cost price history on product::
 
     >>> product.reload()
     >>> product.cost_price
     Decimal('110.0000')
 
@@ -156,9 +153,9 @@
 
     >>> service.cost_price += 5
     >>> service.save()
 
 Check cost history::
 
     >>> history, = ProductCostHistory.find([('product', '=', service.id)])
-    >>> history.cost_price == Decimal('35.0000')
-    True
+    >>> history.cost_price
+    Decimal('35.0000')
```

### Comparing `trytond_product_cost_history-7.0.0/tox.ini` & `trytond_product_cost_history-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_history-7.0.0/trytond_product_cost_history.egg-info/PKG-INFO` & `trytond_product_cost_history-7.2.0/trytond_product_cost_history.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-product-cost-history
-Version: 7.0.0
+Name: trytond_product_cost_history
+Version: 7.2.0
 Summary: Tryton module to historize product cost
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
 
 Product Cost History Module
 ###########################
 
 The Product Cost History Module adds a *Cost History* relate on the product
 form showing the cost price evolution of the product. The history is based on
 the cost price stored on the incoming stock moves for goods and assets and
```

### Comparing `trytond_product_cost_history-7.0.0/trytond_product_cost_history.egg-info/SOURCES.txt` & `trytond_product_cost_history-7.2.0/trytond_product_cost_history.egg-info/SOURCES.txt`

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
 product.py
```

