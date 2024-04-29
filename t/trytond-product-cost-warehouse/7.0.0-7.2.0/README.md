# Comparing `tmp/trytond_product_cost_warehouse-7.0.0.tar.gz` & `tmp/trytond_product_cost_warehouse-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_cost_warehouse-7.0.0.tar", last modified: Mon Oct 30 17:32:40 2023, max compression
+gzip compressed data, was "trytond_product_cost_warehouse-7.2.0.tar", last modified: Mon Apr 29 15:43:01 2024, max compression
```

## Comparing `trytond_product_cost_warehouse-7.0.0.tar` & `trytond_product_cost_warehouse-7.2.0.tar`

### file list

```diff
@@ -1,73 +1,72 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:40.689579 trytond_product_cost_warehouse-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-10-22 17:23:09.000000 trytond_product_cost_warehouse-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      844 2023-10-30 17:08:52.000000 trytond_product_cost_warehouse-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:08:52.000000 trytond_product_cost_warehouse-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3037 2023-10-30 17:32:40.689579 trytond_product_cost_warehouse-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      468 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      742 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/company.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:40.686246 trytond_product_cost_warehouse-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2823 2023-10-22 17:23:09.000000 trytond_product_cost_warehouse-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:09.000000 trytond_product_cost_warehouse-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1530 2023-08-13 15:26:13.000000 trytond_product_cost_warehouse-7.0.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1326 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:40.682912 trytond_product_cost_warehouse-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2625 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2769 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2683 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2720 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2366 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2069 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2700 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2632 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2701 2023-10-30 16:47:45.000000 trytond_product_cost_warehouse-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-10-28 12:11:23.000000 trytond_product_cost_warehouse-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      468 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    10188 2023-08-13 15:26:13.000000 trytond_product_cost_warehouse-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:32:40.689579 trytond_product_cost_warehouse-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4904 2023-10-27 17:38:49.000000 trytond_product_cost_warehouse-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8889 2023-10-07 17:14:58.000000 trytond_product_cost_warehouse-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:40.686246 trytond_product_cost_warehouse-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4445 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/tests/scenario_account_stock_continental.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4447 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/tests/scenario_product_cost_fifo_warehouse.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6371 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/tests/scenario_product_cost_warehouse.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      492 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_product_cost_warehouse-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-10-30 17:08:48.000000 trytond_product_cost_warehouse-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:40.689579 trytond_product_cost_warehouse-7.0.0/trytond_product_cost_warehouse.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3037 2023-10-30 17:32:40.000000 trytond_product_cost_warehouse-7.0.0/trytond_product_cost_warehouse.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2062 2023-10-30 17:32:40.000000 trytond_product_cost_warehouse-7.0.0/trytond_product_cost_warehouse.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:32:40.000000 trytond_product_cost_warehouse-7.0.0/trytond_product_cost_warehouse.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2023-10-30 17:32:40.000000 trytond_product_cost_warehouse-7.0.0/trytond_product_cost_warehouse.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_product_cost_warehouse-7.0.0/trytond_product_cost_warehouse.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      279 2023-10-30 17:32:40.000000 trytond_product_cost_warehouse-7.0.0/trytond_product_cost_warehouse.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:32:40.000000 trytond_product_cost_warehouse-7.0.0/trytond_product_cost_warehouse.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:32:40.686246 trytond_product_cost_warehouse-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/view/ir_cron_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.0.0/view/stock_location_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:01.068712 trytond_product_cost_warehouse-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      945 2024-04-29 15:21:44.000000 trytond_product_cost_warehouse-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:21:44.000000 trytond_product_cost_warehouse-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3028 2024-04-29 15:43:01.068712 trytond_product_cost_warehouse-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      468 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      742 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/company.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:01.065379 trytond_product_cost_warehouse-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-27 16:30:39.000000 trytond_product_cost_warehouse-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:15.000000 trytond_product_cost_warehouse-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1530 2024-01-27 09:58:52.000000 trytond_product_cost_warehouse-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1326 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:01.065379 trytond_product_cost_warehouse-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2625 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2769 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2683 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2720 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2366 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2069 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2700 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2632 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2701 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2024-04-27 16:43:24.000000 trytond_product_cost_warehouse-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      468 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    10188 2024-01-27 09:58:52.000000 trytond_product_cost_warehouse-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:43:01.068712 trytond_product_cost_warehouse-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4895 2024-04-27 16:30:39.000000 trytond_product_cost_warehouse-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9319 2024-04-27 16:30:39.000000 trytond_product_cost_warehouse-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:01.065379 trytond_product_cost_warehouse-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4421 2024-04-27 16:30:39.000000 trytond_product_cost_warehouse-7.2.0/tests/scenario_account_stock_continental.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4403 2024-04-22 12:14:36.000000 trytond_product_cost_warehouse-7.2.0/tests/scenario_product_cost_fifo_warehouse.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6288 2024-04-27 16:30:39.000000 trytond_product_cost_warehouse-7.2.0/tests/scenario_product_cost_warehouse.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      492 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:15.000000 trytond_product_cost_warehouse-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      261 2024-04-29 15:21:39.000000 trytond_product_cost_warehouse-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:01.068712 trytond_product_cost_warehouse-7.2.0/trytond_product_cost_warehouse.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3028 2024-04-29 15:43:00.000000 trytond_product_cost_warehouse-7.2.0/trytond_product_cost_warehouse.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2044 2024-04-29 15:43:01.000000 trytond_product_cost_warehouse-7.2.0/trytond_product_cost_warehouse.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:43:00.000000 trytond_product_cost_warehouse-7.2.0/trytond_product_cost_warehouse.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:43:00.000000 trytond_product_cost_warehouse-7.2.0/trytond_product_cost_warehouse.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_product_cost_warehouse-7.2.0/trytond_product_cost_warehouse.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      279 2024-04-29 15:43:00.000000 trytond_product_cost_warehouse-7.2.0/trytond_product_cost_warehouse.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:43:00.000000 trytond_product_cost_warehouse-7.2.0/trytond_product_cost_warehouse.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:43:01.068712 trytond_product_cost_warehouse-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/view/ir_cron_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_product_cost_warehouse-7.2.0/view/stock_location_form.xml
```

### Comparing `trytond_product_cost_warehouse-7.0.0/CHANGELOG` & `trytond_product_cost_warehouse-7.2.0/CHANGELOG`

 * *Files 19% similar despite different names*

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

### Comparing `trytond_product_cost_warehouse-7.0.0/COPYRIGHT` & `trytond_product_cost_warehouse-7.2.0/COPYRIGHT`

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

### Comparing `trytond_product_cost_warehouse-7.0.0/LICENSE` & `trytond_product_cost_warehouse-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/PKG-INFO` & `trytond_product_cost_warehouse-7.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_product_cost_warehouse
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to compute product cost per warehouse
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-product-cost-warehouse
+Project-URL: Documentation, https://docs.tryton.org/modules-product-cost-warehouse
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product cost warehouse
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,24 +47,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product_cost_fifo<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product_cost_history<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_stock_continental<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product_cost_fifo<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product_cost_history<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_stock_continental<7.3,>=7.2; extra == "test"
 
 #############################
 Product Cost Warehouse Module
 #############################
 
 The *Product Cost Warehouse Module* allows the cost price of products to
 be calculated separately for each warehouse.
```

### Comparing `trytond_product_cost_warehouse-7.0.0/__init__.py` & `trytond_product_cost_warehouse-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/company.py` & `trytond_product_cost_warehouse-7.2.0/company.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/doc/conf.py` & `trytond_product_cost_warehouse-7.2.0/doc/conf.py`

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

### Comparing `trytond_product_cost_warehouse-7.0.0/doc/usage.rst` & `trytond_product_cost_warehouse-7.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/ir.py` & `trytond_product_cost_warehouse-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/bg.po` & `trytond_product_cost_warehouse-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/ca.po` & `trytond_product_cost_warehouse-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/cs.po` & `trytond_product_cost_warehouse-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/de.po` & `trytond_product_cost_warehouse-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/es.po` & `trytond_product_cost_warehouse-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/es_419.po` & `trytond_product_cost_warehouse-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/et.po` & `trytond_product_cost_warehouse-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/fa.po` & `trytond_product_cost_warehouse-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/fi.po` & `trytond_product_cost_warehouse-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/fr.po` & `trytond_product_cost_warehouse-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/hu.po` & `trytond_product_cost_warehouse-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/id.po` & `trytond_product_cost_warehouse-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/it.po` & `trytond_product_cost_warehouse-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/lo.po` & `trytond_product_cost_warehouse-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/lt.po` & `trytond_product_cost_warehouse-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/nl.po` & `trytond_product_cost_warehouse-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/pl.po` & `trytond_product_cost_warehouse-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/pt.po` & `trytond_product_cost_warehouse-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/ro.po` & `trytond_product_cost_warehouse-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/ru.po` & `trytond_product_cost_warehouse-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/sl.po` & `trytond_product_cost_warehouse-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/tr.po` & `trytond_product_cost_warehouse-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/uk.po` & `trytond_product_cost_warehouse-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/locale/zh_CN.po` & `trytond_product_cost_warehouse-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/product.py` & `trytond_product_cost_warehouse-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/res.py` & `trytond_product_cost_warehouse-7.2.0/res.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/setup.py` & `trytond_product_cost_warehouse-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-product-cost-warehouse'),
+            'https://docs.tryton.org/modules-product-cost-warehouse'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton product cost warehouse',
     package_dir={'trytond.modules.product_cost_warehouse': '.'},
     packages=(
         ['trytond.modules.product_cost_warehouse']
```

### Comparing `trytond_product_cost_warehouse-7.0.0/stock.py` & `trytond_product_cost_warehouse-7.2.0/stock.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,49 +51,61 @@
             })
 
 
 class Move(metaclass=PoolMeta):
     __name__ = 'stock.move'
 
     @property
-    def from_warehouse(self):
-        return super().from_warehouse or self.from_location.cost_warehouse
+    @fields.depends('from_location')
+    def from_cost_warehouse(self):
+        if self.from_location:
+            return (
+                self.from_location.warehouse
+                or self.from_location.cost_warehouse)
 
     @property
-    def to_warehouse(self):
-        return super().to_warehouse or self.to_location.cost_warehouse
+    @fields.depends('to_location')
+    def to_cost_warehouse(self):
+        if self.to_location:
+            return (
+                self.to_location.warehouse
+                or self.to_location.cost_warehouse)
 
-    @fields.depends('company', 'from_location', 'to_location')
+    @property
+    def cost_warehouse(self):
+        return self.from_cost_warehouse or self.to_cost_warehouse
+
+    @fields.depends(
+        'company', methods=['from_cost_warehouse', 'to_cost_warehouse'])
     def on_change_with_unit_price_required(self, name=None):
         required = super().on_change_with_unit_price_required(name=name)
         if (self.company and self.company.cost_price_warehouse
-                and self.from_location and self.to_location
-                and self.from_warehouse != self.to_warehouse):
+                and self.from_cost_warehouse != self.to_cost_warehouse):
             required = True
         return required
 
-    @fields.depends('company', 'from_location', 'to_location')
+    @fields.depends(
+        'company', methods=['from_cost_warehouse', 'to_cost_warehouse'])
     def on_change_with_cost_price_required(self, name=None):
         required = super().on_change_with_cost_price_required(name=name)
         if (self.company and self.company.cost_price_warehouse
-                and self.from_location and self.to_location
-                and self.from_warehouse != self.to_warehouse):
+                and self.from_cost_warehouse != self.to_cost_warehouse):
             required = True
         return required
 
     @classmethod
     def get_unit_price_company(cls, moves, name):
         pool = Pool()
         ShipmentInternal = pool.get('stock.shipment.internal')
         Uom = pool.get('product.uom')
         prices = super().get_unit_price_company(moves, name)
         for move in moves:
             if (move.company.cost_price_warehouse
-                    and move.from_warehouse != move.to_warehouse
-                    and move.to_warehouse
+                    and move.from_cost_warehouse != move.to_cost_warehouse
+                    and move.to_cost_warehouse
                     and isinstance(move.shipment, ShipmentInternal)):
                 cost = total_qty = 0
                 for outgoing_move in move.shipment.outgoing_moves:
                     if outgoing_move.product == move.product:
                         qty = Uom.compute_qty(
                             outgoing_move.unit, outgoing_move.quantity,
                             move.product.default_uom)
@@ -107,16 +119,16 @@
 
     def get_cost_price(self, product_cost_price=None):
         pool = Pool()
         ShipmentInternal = pool.get('stock.shipment.internal')
         cost_price = super().get_cost_price(
             product_cost_price=product_cost_price)
         if (self.company.cost_price_warehouse
-                and self.from_warehouse != self.to_warehouse
-                and self.to_warehouse
+                and self.from_cost_warehouse != self.to_cost_warehouse
+                and self.to_cost_warehouse
                 and isinstance(self.shipment, ShipmentInternal)):
             cost_price = self.unit_price_company
         return cost_price
 
     @classmethod
     def validate(cls, moves):
         pool = Pool()
@@ -135,83 +147,83 @@
             else:
                 transit_location = transit_locations[company]
             if (company.cost_price_warehouse
                     and move.from_location.type == 'storage'
                     and move.from_location != transit_location
                     and move.to_location.type == 'storage'
                     and move.to_location != transit_location):
-                if move.from_warehouse != move.to_warehouse:
+                if move.from_cost_warehouse != move.to_cost_warehouse:
                     raise MoveValidationError(gettext(
                             'product_cost_warehouse'
                             '.msg_move_storage_location_same_warehouse',
                             from_=move.from_location.rec_name,
                             to=move.to_location.rec_name))
 
     def _do(self):
         cost_price, to_save = super()._do()
         if (self.company.cost_price_warehouse
                 and self.from_location.type == 'storage'
                 and self.to_location.type == 'storage'
-                and self.from_warehouse != self.to_warehouse):
-            if self.from_warehouse:
+                and self.from_cost_warehouse != self.to_cost_warehouse):
+            if self.from_cost_warehouse:
                 cost_price = self._compute_product_cost_price('out')
-            elif self.to_warehouse:
+            elif self.to_cost_warehouse:
                 cost_price = self._compute_product_cost_price(
                     'in', self.unit_price_company)
         return cost_price, to_save
 
     @property
     def _cost_price_pattern(self):
         pattern = super()._cost_price_pattern
         if self.company.cost_price_warehouse:
             pattern['warehouse'] = (
-                self.warehouse.id if self.warehouse else None)
+                self.cost_warehouse.id if self.cost_warehouse else None)
         return pattern
 
     def _cost_price_key(self):
         key = super()._cost_price_key()
         if self.company.cost_price_warehouse:
             key += (('warehouse',
-                    (self.warehouse.id if self.warehouse else None)),
+                    (self.cost_warehouse.id if self.cost_warehouse else None)),
                 )
         return key
 
     @classmethod
     def _cost_price_context(cls, moves):
         pool = Pool()
         Location = pool.get('stock.location')
         context = super()._cost_price_context(moves)
         if moves[0].company.cost_price_warehouse:
-            warehouse = moves[0].warehouse
+            warehouse = moves[0].cost_warehouse
             locations = Location.search([
                     ('type', '=', 'storage'),
                     ['OR',
                         ('parent', 'child_of',
                             warehouse.id if warehouse else []),
                         ('cost_warehouse', '=',
                             warehouse.id if warehouse else None),
                         ],
                     ])
             context['locations'] = [l.id for l in locations]
         return context
 
     def get_fifo_move(self, quantity=0.0, date=None):
-        warehouse = self.warehouse.id if self.warehouse else None
+        warehouse = self.cost_warehouse.id if self.cost_warehouse else None
         with Transaction().set_context(warehouse=warehouse):
             return super().get_fifo_move(quantity=quantity, date=date)
 
     def _get_account_stock_move_type(self):
         type_ = super()._get_account_stock_move_type()
         if (self.company.cost_price_warehouse
                 and self.from_location.type == 'storage'
                 and self.to_location.type == 'storage'
-                and self.from_warehouse != self.to_warehouse):
-            if self.from_warehouse and not self.to_warehouse:
+                and self.from_cost_warehouse != self.to_cost_warehouse):
+            if self.from_cost_warehouse and not self.to_cost_warehouse:
                 type_ = 'out_warehouse'
-            elif not self.from_warehouse and self.to_warehouse:
+            elif not self.from_cost_warehouse and self.to_cost_warehouse:
                 type_ = 'in_warehouse'
         return type_
 
 
 class ShipmentInternal(metaclass=PoolMeta):
     __name__ = 'stock.shipment.internal'
```

### Comparing `trytond_product_cost_warehouse-7.0.0/tests/scenario_account_stock_continental.rst` & `trytond_product_cost_warehouse-7.2.0/tests/scenario_account_stock_continental.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ==================================
 Account Stock Continental Scenario
 ==================================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_stock_continental.tests.tools import (
     ...     add_stock_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
 Activate product_cost_warehouse::
 
     >>> config = activate_modules([
     ...         'product_cost_warehouse', 'account_stock_continental'])
 
     >>> Location = Model.get('stock.location')
@@ -121,13 +121,13 @@
     >>> shipment.click('ship')
     >>> shipment.state
     'shipped'
     >>> accounts['stock'].reload()
     >>> accounts['stock'].balance
     Decimal('0.00')
 
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
     >>> accounts['stock'].reload()
     >>> accounts['stock'].balance
     Decimal('100.00')
```

### Comparing `trytond_product_cost_warehouse-7.0.0/tests/scenario_product_cost_fifo_warehouse.rst` & `trytond_product_cost_warehouse-7.2.0/tests/scenario_product_cost_fifo_warehouse.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 ====================================
 Product Cost FIFO Warehouse Scenario
 ====================================
 
 Imports::
 
-    >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
 
 Activate product_cost_warehouse::
 
     >>> config = activate_modules(
     ...     ['product_cost_warehouse', 'product_cost_fifo'])
 
 Create company::
```

### Comparing `trytond_product_cost_warehouse-7.0.0/tests/scenario_product_cost_warehouse.rst` & `trytond_product_cost_warehouse-7.2.0/tests/scenario_product_cost_warehouse.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 ===============================
 Product Cost Warehouse Scenario
 ===============================
 
 Imports::
 
-    >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
 
 Activate modules::
 
     >>> config = activate_modules('product_cost_warehouse')
 
 Create company::
 
@@ -139,15 +138,15 @@
     >>> move.product = product
     >>> move.quantity = 1
     >>> move.from_location = warehouse1.storage_location
     >>> move.to_location = warehouse2.storage_location
     >>> move.unit_price = product.cost_price
     >>> move.currency = company.currency
     >>> move.save()
-    >>> move.click('do')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> move.click('do')
     Traceback (most recent call last):
         ...
     MoveValidationError: ...
 
     >>> move.to_location = transit
     >>> move.click('do')
     >>> move.state
@@ -178,15 +177,15 @@
     'shipped'
     >>> move, = shipment.outgoing_moves
     >>> move.state
     'done'
     >>> move.cost_price
     Decimal('90.0000')
 
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
     >>> move, = shipment.incoming_moves
     >>> move.state
     'done'
     >>> move.cost_price
     Decimal('85.0000')
```

### Comparing `trytond_product_cost_warehouse-7.0.0/tox.ini` & `trytond_product_cost_warehouse-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_warehouse-7.0.0/trytond_product_cost_warehouse.egg-info/PKG-INFO` & `trytond_product_cost_warehouse-7.2.0/trytond_product_cost_warehouse.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-product-cost-warehouse
-Version: 7.0.0
+Name: trytond_product_cost_warehouse
+Version: 7.2.0
 Summary: Tryton module to compute product cost per warehouse
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-product-cost-warehouse
+Project-URL: Documentation, https://docs.tryton.org/modules-product-cost-warehouse
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton product cost warehouse
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,24 +47,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product_cost_fifo<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product_cost_history<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_stock_continental<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product_cost_fifo<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product_cost_history<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_stock_continental<7.3,>=7.2; extra == "test"
 
 #############################
 Product Cost Warehouse Module
 #############################
 
 The *Product Cost Warehouse Module* allows the cost price of products to
 be calculated separately for each warehouse.
```

### Comparing `trytond_product_cost_warehouse-7.0.0/trytond_product_cost_warehouse.egg-info/SOURCES.txt` & `trytond_product_cost_warehouse-7.2.0/trytond_product_cost_warehouse.egg-info/SOURCES.txt`

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
 account.py
```

