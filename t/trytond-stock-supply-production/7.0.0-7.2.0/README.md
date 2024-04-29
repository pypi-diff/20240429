# Comparing `tmp/trytond_stock_supply_production-7.0.0.tar.gz` & `tmp/trytond_stock_supply_production-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_supply_production-7.0.0.tar", last modified: Mon Oct 30 17:44:37 2023, max compression
+gzip compressed data, was "trytond_stock_supply_production-7.2.0.tar", last modified: Mon Apr 29 15:53:38 2024, max compression
```

## Comparing `trytond_stock_supply_production-7.0.0.tar` & `trytond_stock_supply_production-7.2.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:37.072996 trytond_stock_supply_production-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-10-22 17:23:28.000000 trytond_stock_supply_production-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2294 2023-10-30 17:15:56.000000 trytond_stock_supply_production-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:15:56.000000 trytond_stock_supply_production-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_supply_production-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3337 2023-10-30 17:44:37.072996 trytond_stock_supply_production-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      745 2023-01-16 14:00:21.000000 trytond_stock_supply_production-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      609 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:37.072996 trytond_stock_supply_production-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2824 2023-10-22 17:23:28.000000 trytond_stock_supply_production-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      745 2023-01-16 14:00:21.000000 trytond_stock_supply_production-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:28.000000 trytond_stock_supply_production-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:37.069662 trytond_stock_supply_production-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      912 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      965 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      823 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      954 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      960 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      775 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      873 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      957 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      823 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      968 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      880 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      864 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      900 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      981 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      823 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      922 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      822 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      937 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      775 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      860 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      906 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      823 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      775 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      823 2023-10-28 12:11:27.000000 trytond_stock_supply_production-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9286 2023-10-07 17:14:58.000000 trytond_stock_supply_production-7.0.0/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1458 2023-01-16 14:00:21.000000 trytond_stock_supply_production-7.0.0/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:44:37.072996 trytond_stock_supply_production-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4487 2023-10-27 17:38:49.000000 trytond_stock_supply_production-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3619 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      618 2023-01-16 14:00:21.000000 trytond_stock_supply_production-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:37.072996 trytond_stock_supply_production-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4286 2023-06-10 11:39:56.000000 trytond_stock_supply_production-7.0.0/tests/scenario_stock_supply_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_stock_supply_production-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      147 2023-10-30 17:15:52.000000 trytond_stock_supply_production-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:37.072996 trytond_stock_supply_production-7.0.0/trytond_stock_supply_production.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3337 2023-10-30 17:44:36.000000 trytond_stock_supply_production-7.0.0/trytond_stock_supply_production.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1710 2023-10-30 17:44:37.000000 trytond_stock_supply_production-7.0.0/trytond_stock_supply_production.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:44:36.000000 trytond_stock_supply_production-7.0.0/trytond_stock_supply_production.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-10-30 17:44:36.000000 trytond_stock_supply_production-7.0.0/trytond_stock_supply_production.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_stock_supply_production-7.0.0/trytond_stock_supply_production.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      154 2023-10-30 17:44:36.000000 trytond_stock_supply_production-7.0.0/trytond_stock_supply_production.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:44:36.000000 trytond_stock_supply_production-7.0.0/trytond_stock_supply_production.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:37.072996 trytond_stock_supply_production-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-01-16 14:00:21.000000 trytond_stock_supply_production-7.0.0/view/production_configuration_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:38.158716 trytond_stock_supply_production-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2395 2024-04-29 15:29:36.000000 trytond_stock_supply_production-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:29:35.000000 trytond_stock_supply_production-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_supply_production-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3337 2024-04-29 15:53:38.158716 trytond_stock_supply_production-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      745 2023-01-16 14:00:21.000000 trytond_stock_supply_production-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      609 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:38.155383 trytond_stock_supply_production-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-27 16:30:39.000000 trytond_stock_supply_production-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      745 2023-01-16 14:00:21.000000 trytond_stock_supply_production-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:37.000000 trytond_stock_supply_production-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:38.158716 trytond_stock_supply_production-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      912 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      965 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      823 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      954 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      960 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      775 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      873 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      957 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      823 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      968 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      880 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      864 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      900 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      981 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      823 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      922 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      822 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      937 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      775 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      860 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      906 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      823 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      775 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      823 2024-04-27 16:43:28.000000 trytond_stock_supply_production-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      516 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9286 2024-02-04 18:51:26.000000 trytond_stock_supply_production-7.2.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1458 2023-01-16 14:00:21.000000 trytond_stock_supply_production-7.2.0/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:53:38.158716 trytond_stock_supply_production-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4487 2024-03-17 11:01:36.000000 trytond_stock_supply_production-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3619 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      618 2023-01-16 14:00:21.000000 trytond_stock_supply_production-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:38.158716 trytond_stock_supply_production-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4323 2024-04-22 12:14:37.000000 trytond_stock_supply_production-7.2.0/tests/scenario_stock_supply_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_supply_production-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:37.000000 trytond_stock_supply_production-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      147 2024-04-29 15:29:31.000000 trytond_stock_supply_production-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:38.158716 trytond_stock_supply_production-7.2.0/trytond_stock_supply_production.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3337 2024-04-29 15:53:37.000000 trytond_stock_supply_production-7.2.0/trytond_stock_supply_production.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1692 2024-04-29 15:53:38.000000 trytond_stock_supply_production-7.2.0/trytond_stock_supply_production.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:53:37.000000 trytond_stock_supply_production-7.2.0/trytond_stock_supply_production.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-04-29 15:53:37.000000 trytond_stock_supply_production-7.2.0/trytond_stock_supply_production.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_stock_supply_production-7.2.0/trytond_stock_supply_production.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      154 2024-04-29 15:53:37.000000 trytond_stock_supply_production-7.2.0/trytond_stock_supply_production.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:53:37.000000 trytond_stock_supply_production-7.2.0/trytond_stock_supply_production.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:38.158716 trytond_stock_supply_production-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-01-16 14:00:21.000000 trytond_stock_supply_production-7.2.0/view/production_configuration_form.xml
```

### Comparing `trytond_stock_supply_production-7.0.0/CHANGELOG` & `trytond_stock_supply_production-7.2.0/CHANGELOG`

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

### Comparing `trytond_stock_supply_production-7.0.0/LICENSE` & `trytond_stock_supply_production-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/PKG-INFO` & `trytond_stock_supply_production-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_supply_production
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for stock supply of production
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
@@ -48,21 +48,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_production<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_supply<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_production<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_supply<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Stock Supply Production Module
 ##############################
 
 The Stock Supply Production module adds automatic supply mechanisms via
 production request.
```

### Comparing `trytond_stock_supply_production-7.0.0/README.rst` & `trytond_stock_supply_production-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/__init__.py` & `trytond_stock_supply_production-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/doc/conf.py` & `trytond_stock_supply_production-7.2.0/doc/conf.py`

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

### Comparing `trytond_stock_supply_production-7.0.0/doc/index.rst` & `trytond_stock_supply_production-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/bg.po` & `trytond_stock_supply_production-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/ca.po` & `trytond_stock_supply_production-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/cs.po` & `trytond_stock_supply_production-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/de.po` & `trytond_stock_supply_production-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/es.po` & `trytond_stock_supply_production-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/es_419.po` & `trytond_stock_supply_production-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/et.po` & `trytond_stock_supply_production-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/fa.po` & `trytond_stock_supply_production-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/fi.po` & `trytond_stock_supply_production-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/fr.po` & `trytond_stock_supply_production-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/hu.po` & `trytond_stock_supply_production-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/id.po` & `trytond_stock_supply_production-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/it.po` & `trytond_stock_supply_production-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/lo.po` & `trytond_stock_supply_production-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/lt.po` & `trytond_stock_supply_production-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/nl.po` & `trytond_stock_supply_production-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/pl.po` & `trytond_stock_supply_production-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/pt.po` & `trytond_stock_supply_production-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/ro.po` & `trytond_stock_supply_production-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/ru.po` & `trytond_stock_supply_production-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/sl.po` & `trytond_stock_supply_production-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/tr.po` & `trytond_stock_supply_production-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/uk.po` & `trytond_stock_supply_production-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/locale/zh_CN.po` & `trytond_stock_supply_production-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/product.py` & `trytond_stock_supply_production-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/production.py` & `trytond_stock_supply_production-7.2.0/production.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/production.xml` & `trytond_stock_supply_production-7.2.0/production.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/setup.py` & `trytond_stock_supply_production-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/stock.py` & `trytond_stock_supply_production-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/stock.xml` & `trytond_stock_supply_production-7.2.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/tests/scenario_stock_supply_production.rst` & `trytond_stock_supply_production-7.2.0/tests/scenario_stock_supply_production.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 Production Request Scenario
 ===========================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.modules.stock.exceptions import MoveFutureWarning
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock_supply_production')
 
@@ -71,15 +71,15 @@
     ... except MoveFutureWarning as warning:
     ...     _, (key, *_) = warning.args
 
     >>> Warning = Model.get('res.user.warning')
     >>> Warning(user=config.user, name=key).save()
     >>> move.click('do')
 
-The is no production request::
+There is no production request::
 
     >>> Production = Model.get('production')
     >>> Production.find([])
     []
 
 Create production request::
 
@@ -89,21 +89,20 @@
 There is now a production request::
 
     >>> productions = Production.find([])
     >>> len(productions)
     2
     >>> {p.state for p in productions}
     {'request'}
-    >>> all(p.product == product for p in productions)
-    True
+    >>> for production in productions:
+    ...     assertEqual(production.product, product)
     >>> sum(p.quantity for p in productions)
     2.0
-    >>> sorted(p.planned_date for p in productions) == [
-    ...     today, today + dt.timedelta(days=9)]
-    True
+    >>> assertEqual(sorted(p.planned_date for p in productions),
+    ...     [today, today + dt.timedelta(days=9)])
 
 Create an order point negative minimal quantity::
 
     >>> OrderPoint = Model.get('stock.order_point')
     >>> order_point = OrderPoint()
     >>> order_point.type = 'production'
     >>> order_point.product = product
@@ -113,15 +112,15 @@
     >>> order_point.save()
 
 Create production request::
 
     >>> create_pr = Wizard('stock.supply')
     >>> create_pr.execute('create_')
 
-The is no more production request::
+There is no more production request::
 
     >>> Production = Model.get('production')
     >>> Production.find([])
     []
 
 Set a minimal quantity on order point::
 
@@ -134,25 +133,23 @@
     >>> create_pr.execute('create_')
 
 There is now a production request::
 
     >>> production, = Production.find([])
     >>> production.state
     'request'
-    >>> production.product == product
-    True
+    >>> assertEqual(production.product, product)
     >>> production.quantity
     11.0
 
 Using zero as minimal quantity also creates a production request::
 
     >>> order_point.min_quantity = 0
     >>> order_point.save()
     >>> create_pr = Wizard('stock.supply')
     >>> create_pr.execute('create_')
     >>> production, = Production.find([])
     >>> production.state
     'request'
-    >>> production.product == product
-    True
+    >>> assertEqual(production.product, product)
     >>> production.quantity
     11.0
```

### Comparing `trytond_stock_supply_production-7.0.0/tox.ini` & `trytond_stock_supply_production-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_supply_production-7.0.0/trytond_stock_supply_production.egg-info/PKG-INFO` & `trytond_stock_supply_production-7.2.0/trytond_stock_supply_production.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-stock-supply-production
-Version: 7.0.0
+Name: trytond_stock_supply_production
+Version: 7.2.0
 Summary: Tryton module for stock supply of production
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
@@ -48,21 +48,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_production<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_supply<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_production<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_supply<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Stock Supply Production Module
 ##############################
 
 The Stock Supply Production module adds automatic supply mechanisms via
 production request.
```

### Comparing `trytond_stock_supply_production-7.0.0/trytond_stock_supply_production.egg-info/SOURCES.txt` & `trytond_stock_supply_production-7.2.0/trytond_stock_supply_production.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

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

