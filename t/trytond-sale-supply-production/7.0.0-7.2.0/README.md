# Comparing `tmp/trytond_sale_supply_production-7.0.0.tar.gz` & `tmp/trytond_sale_supply_production-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_supply_production-7.0.0.tar", last modified: Mon Oct 30 17:40:53 2023, max compression
+gzip compressed data, was "trytond_sale_supply_production-7.2.0.tar", last modified: Mon Apr 29 15:50:27 2024, max compression
```

## Comparing `trytond_sale_supply_production-7.0.0.tar` & `trytond_sale_supply_production-7.2.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:53.961932 trytond_sale_supply_production-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-22 17:23:22.000000 trytond_sale_supply_production-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      824 2023-10-30 17:13:49.000000 trytond_sale_supply_production-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:13:49.000000 trytond_sale_supply_production-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3060 2023-10-30 17:40:53.961932 trytond_sale_supply_production-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      597 2023-08-13 15:26:13.000000 trytond_sale_supply_production-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      605 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:53.958598 trytond_sale_supply_production-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2823 2023-10-22 17:23:22.000000 trytond_sale_supply_production-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      597 2023-08-13 15:26:13.000000 trytond_sale_supply_production-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:22.000000 trytond_sale_supply_production-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:53.958598 trytond_sale_supply_production-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      565 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      552 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      527 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      528 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      504 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-28 12:11:25.000000 trytond_sale_supply_production-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      525 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3820 2023-08-13 15:26:13.000000 trytond_sale_supply_production-7.0.0/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3729 2023-10-07 17:14:58.000000 trytond_sale_supply_production-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      939 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.0.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:40:53.961932 trytond_sale_supply_production-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4594 2023-10-27 17:38:49.000000 trytond_sale_supply_production-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:53.958598 trytond_sale_supply_production-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4144 2023-08-13 15:26:13.000000 trytond_sale_supply_production-7.0.0/tests/scenario_sale_supply_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2987 2023-08-13 15:26:13.000000 trytond_sale_supply_production-7.0.0/tests/scenario_sale_supply_production_stock_first.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_supply_production-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      120 2023-10-30 17:13:45.000000 trytond_sale_supply_production-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:53.961932 trytond_sale_supply_production-7.0.0/trytond_sale_supply_production.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3060 2023-10-30 17:40:53.000000 trytond_sale_supply_production-7.0.0/trytond_sale_supply_production.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1769 2023-10-30 17:40:53.000000 trytond_sale_supply_production-7.0.0/trytond_sale_supply_production.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:40:53.000000 trytond_sale_supply_production-7.0.0/trytond_sale_supply_production.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-10-30 17:40:53.000000 trytond_sale_supply_production-7.0.0/trytond_sale_supply_production.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_sale_supply_production-7.0.0/trytond_sale_supply_production.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:40:53.000000 trytond_sale_supply_production-7.0.0/trytond_sale_supply_production.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:40:53.000000 trytond_sale_supply_production-7.0.0/trytond_sale_supply_production.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:53.958598 trytond_sale_supply_production-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.0.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:27.317041 trytond_sale_supply_production-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      925 2024-04-29 15:27:13.000000 trytond_sale_supply_production-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:27:13.000000 trytond_sale_supply_production-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3060 2024-04-29 15:50:27.317041 trytond_sale_supply_production-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      597 2024-01-27 09:58:52.000000 trytond_sale_supply_production-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      605 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:27.313708 trytond_sale_supply_production-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_sale_supply_production-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      597 2024-01-27 09:58:52.000000 trytond_sale_supply_production-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:31.000000 trytond_sale_supply_production-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:27.313708 trytond_sale_supply_production-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      565 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      552 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      527 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      528 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      504 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-27 16:43:27.000000 trytond_sale_supply_production-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      525 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3816 2024-04-27 16:30:39.000000 trytond_sale_supply_production-7.2.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3729 2024-02-04 18:51:26.000000 trytond_sale_supply_production-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      939 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:50:27.317041 trytond_sale_supply_production-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4594 2024-03-17 11:01:36.000000 trytond_sale_supply_production-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:27.313708 trytond_sale_supply_production-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4124 2024-04-27 16:30:39.000000 trytond_sale_supply_production-7.2.0/tests/scenario_sale_supply_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2937 2024-04-22 12:14:36.000000 trytond_sale_supply_production-7.2.0/tests/scenario_sale_supply_production_stock_first.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:31.000000 trytond_sale_supply_production-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      120 2024-04-29 15:27:09.000000 trytond_sale_supply_production-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:27.317041 trytond_sale_supply_production-7.2.0/trytond_sale_supply_production.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3060 2024-04-29 15:50:26.000000 trytond_sale_supply_production-7.2.0/trytond_sale_supply_production.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1751 2024-04-29 15:50:27.000000 trytond_sale_supply_production-7.2.0/trytond_sale_supply_production.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:50:26.000000 trytond_sale_supply_production-7.2.0/trytond_sale_supply_production.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:50:26.000000 trytond_sale_supply_production-7.2.0/trytond_sale_supply_production.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_sale_supply_production-7.2.0/trytond_sale_supply_production.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-29 15:50:26.000000 trytond_sale_supply_production-7.2.0/trytond_sale_supply_production.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:50:26.000000 trytond_sale_supply_production-7.2.0/trytond_sale_supply_production.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:27.317041 trytond_sale_supply_production-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:15.000000 trytond_sale_supply_production-7.2.0/view/template_form.xml
```

### Comparing `trytond_sale_supply_production-7.0.0/CHANGELOG` & `trytond_sale_supply_production-7.2.0/CHANGELOG`

 * *Files 4% similar despite different names*

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

### Comparing `trytond_sale_supply_production-7.0.0/COPYRIGHT` & `trytond_sale_supply_production-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2020-2023 B2CK
-Copyright (C) 2020-2023 Cédric Krier
+Copyright (C) 2020-2024 B2CK
+Copyright (C) 2020-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_supply_production-7.0.0/LICENSE` & `trytond_sale_supply_production-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-7.0.0/PKG-INFO` & `trytond_sale_supply_production-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_supply_production
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to supply sales from production
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
@@ -47,19 +47,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_production<7.1,>=7.0
-Requires-Dist: trytond_sale_supply<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_production<7.3,>=7.2
+Requires-Dist: trytond_sale_supply<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Supply Production Module
 #############################
 
 The Sale Supply Production module adds a "supply on sale" option to producible
 products.
 If selected, it will generate a production request for each sale line of this
```

### Comparing `trytond_sale_supply_production-7.0.0/README.rst` & `trytond_sale_supply_production-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-7.0.0/__init__.py` & `trytond_sale_supply_production-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-7.0.0/doc/conf.py` & `trytond_sale_supply_production-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_supply_production-7.0.0/doc/index.rst` & `trytond_sale_supply_production-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-7.0.0/locale/ca.po` & `trytond_sale_supply_production-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-7.0.0/locale/de.po` & `trytond_sale_supply_production-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-7.0.0/locale/es.po` & `trytond_sale_supply_production-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-7.0.0/locale/fr.po` & `trytond_sale_supply_production-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-7.0.0/locale/it.po` & `trytond_sale_supply_production-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-7.0.0/locale/nl.po` & `trytond_sale_supply_production-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-7.0.0/product.py` & `trytond_sale_supply_production-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-7.0.0/production.py` & `trytond_sale_supply_production-7.2.0/production.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,16 +75,16 @@
     def run(cls, productions):
         super().run(productions)
 
     @classmethod
     @ModelView.button
     @Workflow.transition('done')
     @process_sale_supply
-    def done(cls, productions):
-        super().done(productions)
+    def do(cls, productions):
+        super().do(productions)
 
         for production in productions:
             production.assign_supplied()
 
     def assign_supplied(self, grouping=('product',), filter_=None):
         pool = Pool()
         SaleLine = pool.get('sale.line')
```

### Comparing `trytond_sale_supply_production-7.0.0/sale.py` & `trytond_sale_supply_production-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-7.0.0/sale.xml` & `trytond_sale_supply_production-7.2.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-7.0.0/setup.py` & `trytond_sale_supply_production-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-7.0.0/tests/scenario_sale_supply_production.rst` & `trytond_sale_supply_production-7.2.0/tests/scenario_sale_supply_production.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 ===============================
 Sale Supply Production Scenario
 ===============================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('sale_supply_production')
 
 Create company::
 
@@ -111,20 +110,17 @@
 
 Check the production::
 
     >>> Production = Model.get('production')
     >>> production, = Production.find([])
     >>> production.state
     'request'
-    >>> production.origin == sale.lines[0]
-    True
-    >>> production.product == product
-    True
-    >>> production.bom == bom
-    True
+    >>> assertEqual(production.origin, sale.lines[0])
+    >>> assertEqual(production.product, product)
+    >>> assertEqual(production.bom, bom)
     >>> production.quantity
     10.0
 
 Delete the production, recreate one::
 
     >>> production.delete()
     >>> production, = Production.find([])
@@ -146,15 +142,15 @@
     'draft'
     >>> move, = shipment.inventory_moves
     >>> move.state
     'draft'
 
 Finish the production::
 
-    >>> production.click('done')
+    >>> production.click('do')
 
     >>> shipment.reload()
     >>> move, = shipment.outgoing_moves
     >>> move.state
     'draft'
     >>> move, = shipment.inventory_moves
     >>> move.state
```

### Comparing `trytond_sale_supply_production-7.0.0/tests/scenario_sale_supply_production_stock_first.rst` & `trytond_sale_supply_production-7.2.0/tests/scenario_sale_supply_production_stock_first.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 ===========================================
 Sale Supply Production Stock First Scenario
 ===========================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
 
 Activate modules::
 
     >>> config = activate_modules('sale_supply_production')
 
     >>> Inventory = Model.get('stock.inventory')
     >>> Location = Model.get('stock.location')
```

### Comparing `trytond_sale_supply_production-7.0.0/tox.ini` & `trytond_sale_supply_production-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_supply_production-7.0.0/trytond_sale_supply_production.egg-info/PKG-INFO` & `trytond_sale_supply_production-7.2.0/trytond_sale_supply_production.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-sale-supply-production
-Version: 7.0.0
+Name: trytond_sale_supply_production
+Version: 7.2.0
 Summary: Tryton module to supply sales from production
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
@@ -47,19 +47,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_production<7.1,>=7.0
-Requires-Dist: trytond_sale_supply<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_production<7.3,>=7.2
+Requires-Dist: trytond_sale_supply<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Supply Production Module
 #############################
 
 The Sale Supply Production module adds a "supply on sale" option to producible
 products.
 If selected, it will generate a production request for each sale line of this
```

### Comparing `trytond_sale_supply_production-7.0.0/trytond_sale_supply_production.egg-info/SOURCES.txt` & `trytond_sale_supply_production-7.2.0/trytond_sale_supply_production.egg-info/SOURCES.txt`

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

