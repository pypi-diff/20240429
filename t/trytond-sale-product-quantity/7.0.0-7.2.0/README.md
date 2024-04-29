# Comparing `tmp/trytond_sale_product_quantity-7.0.0.tar.gz` & `tmp/trytond_sale_product_quantity-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_product_quantity-7.0.0.tar", last modified: Mon Oct 30 17:39:06 2023, max compression
+gzip compressed data, was "trytond_sale_product_quantity-7.2.0.tar", last modified: Mon Apr 29 15:48:53 2024, max compression
```

## Comparing `trytond_sale_product_quantity-7.0.0.tar` & `trytond_sale_product_quantity-7.2.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:06.578086 trytond_sale_product_quantity-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      223 2023-10-22 17:23:19.000000 trytond_sale_product_quantity-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-10-30 17:12:41.000000 trytond_sale_product_quantity-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:12:40.000000 trytond_sale_product_quantity-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2761 2023-10-30 17:39:06.578086 trytond_sale_product_quantity-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      254 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      510 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:06.574753 trytond_sale_product_quantity-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2822 2023-10-22 17:23:19.000000 trytond_sale_product_quantity-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      254 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:19.000000 trytond_sale_product_quantity-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:06.574753 trytond_sale_product_quantity-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1408 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1406 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1375 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1408 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1419 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2023-10-28 12:11:25.000000 trytond_sale_product_quantity-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      672 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1715 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      486 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3641 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:39:06.578086 trytond_sale_product_quantity-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4714 2023-10-27 17:38:49.000000 trytond_sale_product_quantity-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:06.574753 trytond_sale_product_quantity-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2545 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/tests/scenario_sale_product_quantity.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2768 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/tests/scenario_sale_product_quantity_pos.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_product_quantity-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       97 2023-10-30 17:12:37.000000 trytond_sale_product_quantity-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:06.578086 trytond_sale_product_quantity-7.0.0/trytond_sale_product_quantity.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2761 2023-10-30 17:39:06.000000 trytond_sale_product_quantity-7.0.0/trytond_sale_product_quantity.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1740 2023-10-30 17:39:06.000000 trytond_sale_product_quantity-7.0.0/trytond_sale_product_quantity.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:39:06.000000 trytond_sale_product_quantity-7.0.0/trytond_sale_product_quantity.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-10-30 17:39:06.000000 trytond_sale_product_quantity-7.0.0/trytond_sale_product_quantity.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_sale_product_quantity-7.0.0/trytond_sale_product_quantity.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      122 2023-10-30 17:39:06.000000 trytond_sale_product_quantity-7.0.0/trytond_sale_product_quantity.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:39:06.000000 trytond_sale_product_quantity-7.0.0/trytond_sale_product_quantity.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:06.574753 trytond_sale_product_quantity-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.0.0/view/product_template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:53.499495 trytond_sale_product_quantity-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2024-04-29 15:25:57.000000 trytond_sale_product_quantity-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:25:57.000000 trytond_sale_product_quantity-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2752 2024-04-29 15:48:53.499495 trytond_sale_product_quantity-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      254 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      510 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:53.496162 trytond_sale_product_quantity-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3084 2024-04-27 16:30:39.000000 trytond_sale_product_quantity-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      254 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:27.000000 trytond_sale_product_quantity-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:53.496162 trytond_sale_product_quantity-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1408 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1406 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1375 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1408 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1419 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2024-04-27 16:43:26.000000 trytond_sale_product_quantity-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      672 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1715 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      486 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3641 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:48:53.499495 trytond_sale_product_quantity-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4705 2024-04-27 16:30:39.000000 trytond_sale_product_quantity-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:53.496162 trytond_sale_product_quantity-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2374 2024-04-22 12:14:36.000000 trytond_sale_product_quantity-7.2.0/tests/scenario_sale_product_quantity.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2671 2024-04-22 12:14:36.000000 trytond_sale_product_quantity-7.2.0/tests/scenario_sale_product_quantity_pos.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:27.000000 trytond_sale_product_quantity-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       97 2024-04-29 15:25:53.000000 trytond_sale_product_quantity-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:53.499495 trytond_sale_product_quantity-7.2.0/trytond_sale_product_quantity.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2752 2024-04-29 15:48:53.000000 trytond_sale_product_quantity-7.2.0/trytond_sale_product_quantity.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1722 2024-04-29 15:48:53.000000 trytond_sale_product_quantity-7.2.0/trytond_sale_product_quantity.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:48:53.000000 trytond_sale_product_quantity-7.2.0/trytond_sale_product_quantity.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:48:53.000000 trytond_sale_product_quantity-7.2.0/trytond_sale_product_quantity.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_sale_product_quantity-7.2.0/trytond_sale_product_quantity.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      122 2024-04-29 15:48:53.000000 trytond_sale_product_quantity-7.2.0/trytond_sale_product_quantity.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:48:53.000000 trytond_sale_product_quantity-7.2.0/trytond_sale_product_quantity.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:53.499495 trytond_sale_product_quantity-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2023-04-15 07:12:15.000000 trytond_sale_product_quantity-7.2.0/view/product_template_form.xml
```

### Comparing `trytond_sale_product_quantity-7.0.0/COPYRIGHT` & `trytond_sale_product_quantity-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2022-2023 B2CK
-Copyright (C) 2022-2023 Cédric Krier
+Copyright (C) 2022-2024 B2CK
+Copyright (C) 2022-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_sale_product_quantity-7.0.0/LICENSE` & `trytond_sale_product_quantity-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/PKG-INFO` & `trytond_sale_product_quantity-7.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_sale_product_quantity
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add quantity constraints on sale line
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale-product-quantity
+Project-URL: Documentation, https://docs.tryton.org/modules-sale-product-quantity
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale product quantity
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,20 +47,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_point<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_point<7.3,>=7.2; extra == "test"
 
 ############################
 Sale Product Quantity Module
 ############################
 
 The *Sale Product Quantity Module* permits to enforce the minimal and the
 rounding of quantity sold per product.
```

### Comparing `trytond_sale_product_quantity-7.0.0/doc/conf.py` & `trytond_sale_product_quantity-7.2.0/doc/conf.py`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_sale_product_quantity-7.0.0/locale/bg.po` & `trytond_sale_product_quantity-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/ca.po` & `trytond_sale_product_quantity-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/cs.po` & `trytond_sale_product_quantity-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/de.po` & `trytond_sale_product_quantity-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/es.po` & `trytond_sale_product_quantity-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/es_419.po` & `trytond_sale_product_quantity-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/et.po` & `trytond_sale_product_quantity-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/fa.po` & `trytond_sale_product_quantity-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/fi.po` & `trytond_sale_product_quantity-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/fr.po` & `trytond_sale_product_quantity-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/hu.po` & `trytond_sale_product_quantity-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/id.po` & `trytond_sale_product_quantity-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/it.po` & `trytond_sale_product_quantity-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/lo.po` & `trytond_sale_product_quantity-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/lt.po` & `trytond_sale_product_quantity-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/nl.po` & `trytond_sale_product_quantity-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/pl.po` & `trytond_sale_product_quantity-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/pt.po` & `trytond_sale_product_quantity-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/ro.po` & `trytond_sale_product_quantity-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/ru.po` & `trytond_sale_product_quantity-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/sl.po` & `trytond_sale_product_quantity-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/tr.po` & `trytond_sale_product_quantity-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/uk.po` & `trytond_sale_product_quantity-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/locale/zh_CN.po` & `trytond_sale_product_quantity-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/message.xml` & `trytond_sale_product_quantity-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/product.py` & `trytond_sale_product_quantity-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/sale.py` & `trytond_sale_product_quantity-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/setup.py` & `trytond_sale_product_quantity-7.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-sale-product-quantity'),
+            'https://docs.tryton.org/modules-sale-product-quantity'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton sale product quantity',
     package_dir={'trytond.modules.sale_product_quantity': '.'},
     packages=(
         ['trytond.modules.sale_product_quantity']
```

### Comparing `trytond_sale_product_quantity-7.0.0/tests/scenario_sale_product_quantity.rst` & `trytond_sale_product_quantity-7.2.0/tests/scenario_sale_product_quantity_pos.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,59 @@
-==============================
-Sale Product Quantity Scenario
-==============================
+==================================
+Sale Product Quantity POS Scenario
+==================================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
 
 Activate modules::
 
-    >>> config = activate_modules('sale_product_quantity')
+    >>> config = activate_modules(
+    ...     ['sale_product_quantity', 'sale_point'])
 
+    >>> Journal = Model.get('account.journal')
+    >>> Location = Model.get('stock.location')
+    >>> POS = Model.get('sale.point')
     >>> Party = Model.get('party.party')
     >>> ProductTemplate = Model.get('product.template')
     >>> ProductUom = Model.get('product.uom')
-    >>> Sale = Model.get('sale.sale')
+    >>> Sale = Model.get('sale.point.sale')
+    >>> SequenceStrict = Model.get('ir.sequence.strict')
+    >>> SequenceType = Model.get('ir.sequence.type')
 
 Create company::
 
     >>> _ = create_company()
     >>> company = get_company()
 
-Create parties::
+Get journal::
 
-    >>> customer = Party(name="Customer")
-    >>> customer.save()
+    >>> journal_revenue, = Journal.find([('type', '=', 'revenue')], limit=1)
+
+Get stock locations::
+
+    >>> storage_loc, = Location.find([('code', '=', 'STO')])
+    >>> customer_loc, = Location.find([('code', '=', 'CUS')])
+
+Create POS::
+
+    >>> pos = POS(name="POS")
+    >>> pos.journal = journal_revenue
+    >>> pos.sequence = SequenceStrict(name="POS", company=pos.company)
+    >>> pos.sequence.sequence_type, = SequenceType.find(
+    ...     [('name', '=', "POS")], limit=1)
+    >>> pos.sequence.save()
+    >>> pos.storage_location = storage_loc
+    >>> pos.customer_location = customer_loc
+    >>> pos.save()
 
 Create product::
 
     >>> gr, = ProductUom.find([('name', '=', "Gram")])
     >>> kg, = ProductUom.find([('name', '=', "Kilogram")])
 
     >>> template = ProductTemplate()
@@ -45,57 +66,32 @@
     >>> template.sale_quantity_minimal = 0.1
     >>> template.sale_quantity_rounding = 0.05
     >>> template.save()
     >>> product, = template.products
 
 Make a sale::
 
-    >>> sale = Sale()
-    >>> sale.party = customer
+    >>> sale = Sale(point=pos)
+
     >>> line = sale.lines.new()
     >>> line.product = product
     >>> line.quantity
     0.1
     >>> sale.save()
 
 Can not set quantity below minimal::
 
     >>> line, = sale.lines
     >>> line.quantity = 0.05
-    >>> sale.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> sale.save()
     Traceback (most recent call last):
         ...
     SaleValidationError: ...
 
 Can not set quantity different than rounding::
 
     >>> line, = sale.lines
     >>> line.quantity = 1.01
-    >>> sale.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
-    Traceback (most recent call last):
-        ...
-    SaleValidationError: ...
-
-Use different unit::
-
-    >>> line, = sale.lines
-    >>> line.unit = gr
-    >>> line.quantity = 500
     >>> sale.save()
-
-Can not set quantity below minimal::
-
-    >>> line, = sale.lines
-    >>> line.quantity = 50
-    >>> sale.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
-    Traceback (most recent call last):
-        ...
-    SaleValidationError: ...
-
-Can not set quantity different than rounding::
-
-    >>> line, = sale.lines
-    >>> line.quantity = 505
-    >>> sale.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
     Traceback (most recent call last):
         ...
     SaleValidationError: ...
```

### Comparing `trytond_sale_product_quantity-7.0.0/tox.ini` & `trytond_sale_product_quantity-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_quantity-7.0.0/trytond_sale_product_quantity.egg-info/PKG-INFO` & `trytond_sale_product_quantity-7.2.0/trytond_sale_product_quantity.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-sale-product-quantity
-Version: 7.0.0
+Name: trytond_sale_product_quantity
+Version: 7.2.0
 Summary: Tryton module to add quantity constraints on sale line
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-sale-product-quantity
+Project-URL: Documentation, https://docs.tryton.org/modules-sale-product-quantity
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton sale product quantity
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,20 +47,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_point<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_point<7.3,>=7.2; extra == "test"
 
 ############################
 Sale Product Quantity Module
 ############################
 
 The *Sale Product Quantity Module* permits to enforce the minimal and the
 rounding of quantity sold per product.
```

### Comparing `trytond_sale_product_quantity-7.0.0/trytond_sale_product_quantity.egg-info/SOURCES.txt` & `trytond_sale_product_quantity-7.2.0/trytond_sale_product_quantity.egg-info/SOURCES.txt`

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

