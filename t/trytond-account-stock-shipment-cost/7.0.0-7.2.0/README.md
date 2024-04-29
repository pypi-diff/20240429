# Comparing `tmp/trytond_account_stock_shipment_cost-7.0.0.tar.gz` & `tmp/trytond_account_stock_shipment_cost-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_stock_shipment_cost-7.0.0.tar", last modified: Mon Oct 30 17:25:43 2023, max compression
+gzip compressed data, was "trytond_account_stock_shipment_cost-7.2.0.tar", last modified: Mon Apr 29 15:36:57 2024, max compression
```

## Comparing `trytond_account_stock_shipment_cost-7.0.0.tar` & `trytond_account_stock_shipment_cost-7.2.0.tar`

### file list

```diff
@@ -1,72 +1,71 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:43.880924 trytond_account_stock_shipment_cost-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      235 2023-10-22 17:22:57.000000 trytond_account_stock_shipment_cost-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      726 2023-10-30 17:04:02.000000 trytond_account_stock_shipment_cost-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:04:02.000000 trytond_account_stock_shipment_cost-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2958 2023-10-30 17:25:43.880924 trytond_account_stock_shipment_cost-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      897 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15600 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9525 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:43.877591 trytond_account_stock_shipment_cost-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2828 2023-10-22 17:22:57.000000 trytond_account_stock_shipment_cost-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1207 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:57.000000 trytond_account_stock_shipment_cost-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:43.874257 trytond_account_stock_shipment_cost-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7039 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6981 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6998 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7192 2023-10-30 16:47:45.000000 trytond_account_stock_shipment_cost-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5888 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5878 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6857 2023-10-30 16:47:45.000000 trytond_account_stock_shipment_cost-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5888 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5879 2023-10-30 16:47:45.000000 trytond_account_stock_shipment_cost-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5852 2023-10-28 12:11:20.000000 trytond_account_stock_shipment_cost-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      671 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:25:43.880924 trytond_account_stock_shipment_cost-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4818 2023-10-27 17:38:49.000000 trytond_account_stock_shipment_cost-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      709 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:43.874257 trytond_account_stock_shipment_cost-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7257 2023-08-13 15:26:13.000000 trytond_account_stock_shipment_cost-7.0.0/tests/scenario_account_stock_shipment_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_stock_shipment_cost-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      170 2023-10-30 17:03:59.000000 trytond_account_stock_shipment_cost-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:43.877591 trytond_account_stock_shipment_cost-7.0.0/trytond_account_stock_shipment_cost.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2958 2023-10-30 17:25:43.000000 trytond_account_stock_shipment_cost-7.0.0/trytond_account_stock_shipment_cost.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2152 2023-10-30 17:25:43.000000 trytond_account_stock_shipment_cost-7.0.0/trytond_account_stock_shipment_cost.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:25:43.000000 trytond_account_stock_shipment_cost-7.0.0/trytond_account_stock_shipment_cost.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       92 2023-10-30 17:25:43.000000 trytond_account_stock_shipment_cost-7.0.0/trytond_account_stock_shipment_cost.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_stock_shipment_cost-7.0.0/trytond_account_stock_shipment_cost.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      203 2023-10-30 17:25:43.000000 trytond_account_stock_shipment_cost-7.0.0/trytond_account_stock_shipment_cost.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:25:43.000000 trytond_account_stock_shipment_cost-7.0.0/trytond_account_stock_shipment_cost.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:43.877591 trytond_account_stock_shipment_cost-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      387 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      897 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/view/shipment_cost_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/view/shipment_cost_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/view/shipment_cost_show_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/view/shipment_cost_show_shipment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.0.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:57.221562 trytond_account_stock_shipment_cost-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      827 2024-04-29 15:17:00.000000 trytond_account_stock_shipment_cost-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:16:59.000000 trytond_account_stock_shipment_cost-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2949 2024-04-29 15:36:57.221562 trytond_account_stock_shipment_cost-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      897 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15600 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9364 2024-04-27 16:30:39.000000 trytond_account_stock_shipment_cost-7.2.0/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:57.218228 trytond_account_stock_shipment_cost-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3090 2024-04-27 16:30:39.000000 trytond_account_stock_shipment_cost-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1207 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:02.000000 trytond_account_stock_shipment_cost-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:57.218228 trytond_account_stock_shipment_cost-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7039 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6981 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6998 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7192 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5888 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5878 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6857 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5887 2024-04-29 13:17:17.000000 trytond_account_stock_shipment_cost-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5879 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5852 2024-04-27 16:43:22.000000 trytond_account_stock_shipment_cost-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      671 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:36:57.221562 trytond_account_stock_shipment_cost-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4809 2024-04-27 16:30:39.000000 trytond_account_stock_shipment_cost-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      709 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:57.218228 trytond_account_stock_shipment_cost-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7193 2024-04-27 16:30:39.000000 trytond_account_stock_shipment_cost-7.2.0/tests/scenario_account_stock_shipment_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:02.000000 trytond_account_stock_shipment_cost-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      170 2024-04-29 15:16:54.000000 trytond_account_stock_shipment_cost-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:57.221562 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2949 2024-04-29 15:36:56.000000 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2134 2024-04-29 15:36:57.000000 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:36:56.000000 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       92 2024-04-29 15:36:56.000000 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      203 2024-04-29 15:36:56.000000 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:36:56.000000 trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:57.221562 trytond_account_stock_shipment_cost-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      387 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      897 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/view/shipment_cost_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/view/shipment_cost_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/view/shipment_cost_show_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/view/shipment_cost_show_shipment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_account_stock_shipment_cost-7.2.0/view/template_form.xml
```

### Comparing `trytond_account_stock_shipment_cost-7.0.0/CHANGELOG` & `trytond_account_stock_shipment_cost-7.2.0/CHANGELOG`

 * *Files 22% similar despite different names*

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

### Comparing `trytond_account_stock_shipment_cost-7.0.0/COPYRIGHT` & `trytond_account_stock_shipment_cost-7.2.0/COPYRIGHT`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2021-2023 B2CK
-Copyright (C) 2021-2023 Cédric Krier
+Copyright (C) 2021-2024 B2CK
+Copyright (C) 2021-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_stock_shipment_cost-7.0.0/LICENSE` & `trytond_account_stock_shipment_cost-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/PKG-INFO` & `trytond_account_stock_shipment_cost-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_shipment_cost
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to allocate shipment cost based on invoice
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-stock-shipment-cost
+Project-URL: Documentation, https://docs.tryton.org/modules-account-stock-shipment-cost
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account stock shipment cost carrier invoice
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,22 +49,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_cost<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_cost<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##################################
 Account Stock Shipment Cost Module
 ##################################
 
 The *Account Stock Shipment Cost Module* allocates shipment cost based on
 invoice.
```

### Comparing `trytond_account_stock_shipment_cost-7.0.0/__init__.py` & `trytond_account_stock_shipment_cost-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/account.py` & `trytond_account_stock_shipment_cost-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/account.xml` & `trytond_account_stock_shipment_cost-7.2.0/account.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_account_stock_shipment_cost-7.0.0/account.xml` & `trytond_account_stock_shipment_cost-7.2.0/account.xml`

```diff
@@ -89,51 +89,51 @@
     </record>
     <record model="ir.action.keyword" id="act_shipment_cost_form_shipment_keyword2">
       <field name="keyword">form_relate</field>
       <field name="model">stock.shipment.out.return,-1</field>
       <field name="action" ref="act_shipment_cost_form_shipment"/>
     </record>
     <record model="ir.model.access" id="access_shipment_cost">
-      <field name="model" search="[('model', '=', 'account.shipment_cost')]"/>
+      <field name="model">account.shipment_cost</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_shipment_cost_account">
-      <field name="model" search="[('model', '=', 'account.shipment_cost')]"/>
+      <field name="model">account.shipment_cost</field>
       <field name="group" ref="account.group_account"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="shipment_cost_cancel_button">
+      <field name="model">account.shipment_cost</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'account.shipment_cost')]"/>
     </record>
     <record model="ir.model.button" id="shipment_cost_post_button">
+      <field name="model">account.shipment_cost</field>
       <field name="name">post_wizard</field>
       <field name="string">Post</field>
-      <field name="model" search="[('model', '=', 'account.shipment_cost')]"/>
     </record>
     <record model="ir.model.button" id="shipment_cost_show_button">
+      <field name="model">account.shipment_cost</field>
       <field name="name">show</field>
       <field name="string">Show</field>
-      <field name="model" search="[('model', '=', 'account.shipment_cost')]"/>
     </record>
     <record model="ir.model.button" id="shipment_cost_draft_button">
+      <field name="model">account.shipment_cost</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'account.shipment_cost')]"/>
     </record>
     <record model="ir.rule.group" id="rule_group_shipment_cost_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'account.shipment_cost')]"/>
+      <field name="model">account.shipment_cost</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_shipment_cost_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_shipment_cost_companies"/>
     </record>
     <record model="ir.action.wizard" id="wizard_shipment_cost_post">
```

### Comparing `trytond_account_stock_shipment_cost-7.0.0/doc/conf.py` & `trytond_account_stock_shipment_cost-7.2.0/doc/conf.py`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_account_stock_shipment_cost-7.0.0/doc/design.rst` & `trytond_account_stock_shipment_cost-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/bg.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/ca.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/cs.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/de.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/es.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/es_419.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/et.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/fa.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/fi.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/fr.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/hu.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/id.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/it.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/lo.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/lt.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/nl.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/pl.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/pt.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/ro.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/ro.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #
-#, fuzzy
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:account.configuration,shipment_cost_sequence:"
 msgid "Shipment Cost Sequence"
 msgstr ""
 
@@ -231,15 +230,15 @@
 
 msgctxt "selection:account.shipment_cost.show.shipment,shipment:"
 msgid "Shipment Return"
 msgstr ""
 
 msgctxt "view:account.configuration:"
 msgid "Sequence"
-msgstr ""
+msgstr "Secventa"
 
 msgctxt "view:account.configuration:"
 msgid "Shipment Cost"
 msgstr ""
 
 msgctxt "wizard_button:account.shipment_cost.post,show,end:"
 msgid "Cancel"
```

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/ru.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/sl.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/tr.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/uk.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/locale/zh_CN.po` & `trytond_account_stock_shipment_cost-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/message.xml` & `trytond_account_stock_shipment_cost-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/product.py` & `trytond_account_stock_shipment_cost-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/setup.py` & `trytond_account_stock_shipment_cost-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/'
+            'https://docs.tryton.org/'
             'modules-account-stock-shipment-cost'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton account stock shipment cost carrier invoice',
     package_dir={'trytond.modules.account_stock_shipment_cost': '.'},
     packages=(
```

### Comparing `trytond_account_stock_shipment_cost-7.0.0/stock.py` & `trytond_account_stock_shipment_cost-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/tests/scenario_account_stock_shipment_cost.rst` & `trytond_account_stock_shipment_cost-7.2.0/tests/scenario_account_stock_shipment_cost.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 ====================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts)
+    ...     create_chart, create_fiscalyear, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
     >>> from trytond.modules.account_stock_shipment_cost.exceptions import (
     ...     SamePartiesWarning)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('account_stock_shipment_cost')
 
@@ -109,24 +108,24 @@
     >>> move.to_location = customer_loc
     >>> move.unit_price = Decimal('100.00')
     >>> move.currency = company.currency
     >>> shipment1.click('wait')
     >>> shipment1.click('assign_force')
     >>> shipment1.click('pick')
     >>> shipment1.click('pack')
-    >>> shipment1.click('done')
+    >>> shipment1.click('do')
     >>> shipment1.state
     'done'
 
     >>> shipment2, = shipment1.duplicate()
     >>> shipment2.click('wait')
     >>> shipment2.click('assign_force')
     >>> shipment2.click('pick')
     >>> shipment2.click('pack')
-    >>> shipment2.click('done')
+    >>> shipment2.click('do')
     >>> shipment2.state
     'done'
 
 Invoice shipment cost::
 
     >>> invoice = Invoice(type='in')
     >>> invoice.party = carrier
@@ -199,15 +198,15 @@
     Decimal('2.0000')
     >>> sorted([s.cost for s in post_shipment_cost.form.shipments])
     [Decimal('2.0000')]
     >>> try:
     ...     post_shipment_cost.execute('post')
     ... except SamePartiesWarning as warning:
     ...     _, (key, *_) = warning.args
-    ...     raise  # doctest: +IGNORE_EXCEPTION_DETAIL
+    ...     raise
     Traceback (most recent call last):
         ...
     SamePartiesWarning: ...
     >>> Warning(user=config.user, name=key).save()
     >>> post_shipment_cost.execute('post')
     >>> shipment_cost2.state
     'posted'
```

### Comparing `trytond_account_stock_shipment_cost-7.0.0/tox.ini` & `trytond_account_stock_shipment_cost-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_shipment_cost-7.0.0/trytond_account_stock_shipment_cost.egg-info/PKG-INFO` & `trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-account-stock-shipment-cost
-Version: 7.0.0
+Name: trytond_account_stock_shipment_cost
+Version: 7.2.0
 Summary: Tryton module to allocate shipment cost based on invoice
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-account-stock-shipment-cost
+Project-URL: Documentation, https://docs.tryton.org/modules-account-stock-shipment-cost
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton account stock shipment cost carrier invoice
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -49,22 +49,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_cost<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_cost<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 ##################################
 Account Stock Shipment Cost Module
 ##################################
 
 The *Account Stock Shipment Cost Module* allocates shipment cost based on
 invoice.
```

### Comparing `trytond_account_stock_shipment_cost-7.0.0/trytond_account_stock_shipment_cost.egg-info/SOURCES.txt` & `trytond_account_stock_shipment_cost-7.2.0/trytond_account_stock_shipment_cost.egg-info/SOURCES.txt`

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
 account.py
```

### Comparing `trytond_account_stock_shipment_cost-7.0.0/view/shipment_cost_form.xml` & `trytond_account_stock_shipment_cost-7.2.0/view/shipment_cost_form.xml`

 * *Files identical despite different names*

