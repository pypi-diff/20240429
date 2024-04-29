# Comparing `tmp/trytond_sale_secondary_unit-7.0.0.tar.gz` & `tmp/trytond_sale_secondary_unit-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_secondary_unit-7.0.0.tar", last modified: Mon Oct 30 17:39:45 2023, max compression
+gzip compressed data, was "trytond_sale_secondary_unit-7.2.0.tar", last modified: Mon Apr 29 15:49:29 2024, max compression
```

## Comparing `trytond_sale_secondary_unit-7.0.0.tar` & `trytond_sale_secondary_unit-7.2.0.tar`

### file list

```diff
@@ -1,70 +1,69 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:45.508272 trytond_sale_secondary_unit-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      219 2023-10-22 17:23:21.000000 trytond_sale_secondary_unit-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      897 2023-10-30 17:13:08.000000 trytond_sale_secondary_unit-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:13:08.000000 trytond_sale_secondary_unit-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3274 2023-10-30 17:39:45.508272 trytond_sale_secondary_unit-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      962 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1189 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:45.504938 trytond_sale_secondary_unit-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2820 2023-10-22 17:23:21.000000 trytond_sale_secondary_unit-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:21.000000 trytond_sale_secondary_unit-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:45.501605 trytond_sale_secondary_unit-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6200 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6216 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6243 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6266 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6359 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4583 2023-10-30 16:47:45.000000 trytond_sale_secondary_unit-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6328 2023-10-24 07:56:52.000000 trytond_sale_secondary_unit-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      834 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    13210 2023-10-24 07:56:52.000000 trytond_sale_secondary_unit-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      983 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:39:45.508272 trytond_sale_secondary_unit-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4658 2023-10-27 17:38:49.000000 trytond_sale_secondary_unit-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1172 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      504 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:45.504938 trytond_sale_secondary_unit-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3727 2023-08-13 15:26:13.000000 trytond_sale_secondary_unit-7.0.0/tests/scenario_sale_blanket_agreement_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3532 2023-10-24 07:56:52.000000 trytond_sale_secondary_unit-7.0.0/tests/scenario_sale_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_secondary_unit-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-10-30 17:13:04.000000 trytond_sale_secondary_unit-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:45.504938 trytond_sale_secondary_unit-7.0.0/trytond_sale_secondary_unit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3274 2023-10-30 17:39:45.000000 trytond_sale_secondary_unit-7.0.0/trytond_sale_secondary_unit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2016 2023-10-30 17:39:45.000000 trytond_sale_secondary_unit-7.0.0/trytond_sale_secondary_unit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:39:45.000000 trytond_sale_secondary_unit-7.0.0/trytond_sale_secondary_unit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-10-30 17:39:45.000000 trytond_sale_secondary_unit-7.0.0/trytond_sale_secondary_unit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_sale_secondary_unit-7.0.0/trytond_sale_secondary_unit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-10-30 17:39:45.000000 trytond_sale_secondary_unit-7.0.0/trytond_sale_secondary_unit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:39:45.000000 trytond_sale_secondary_unit-7.0.0/trytond_sale_secondary_unit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:39:45.504938 trytond_sale_secondary_unit-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      665 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/view/product_customer_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      711 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      642 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/view/sale_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.0.0/view/stock_move_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:29.208561 trytond_sale_secondary_unit-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      998 2024-04-29 15:26:28.000000 trytond_sale_secondary_unit-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:26:28.000000 trytond_sale_secondary_unit-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3274 2024-04-29 15:49:29.208561 trytond_sale_secondary_unit-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      962 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1189 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:29.205227 trytond_sale_secondary_unit-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3082 2024-04-27 16:30:39.000000 trytond_sale_secondary_unit-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:28.000000 trytond_sale_secondary_unit-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:29.205227 trytond_sale_secondary_unit-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6216 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6243 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6266 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6359 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4583 2024-04-27 16:43:26.000000 trytond_sale_secondary_unit-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6328 2024-02-04 18:51:26.000000 trytond_sale_secondary_unit-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      834 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    13210 2024-02-04 18:51:26.000000 trytond_sale_secondary_unit-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      983 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:49:29.208561 trytond_sale_secondary_unit-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4658 2024-03-17 11:01:36.000000 trytond_sale_secondary_unit-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1172 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      504 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:29.205227 trytond_sale_secondary_unit-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3710 2024-04-22 12:14:36.000000 trytond_sale_secondary_unit-7.2.0/tests/scenario_sale_blanket_agreement_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3516 2024-04-22 12:14:36.000000 trytond_sale_secondary_unit-7.2.0/tests/scenario_sale_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:28.000000 trytond_sale_secondary_unit-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-04-29 15:26:24.000000 trytond_sale_secondary_unit-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:29.208561 trytond_sale_secondary_unit-7.2.0/trytond_sale_secondary_unit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3274 2024-04-29 15:49:28.000000 trytond_sale_secondary_unit-7.2.0/trytond_sale_secondary_unit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1998 2024-04-29 15:49:29.000000 trytond_sale_secondary_unit-7.2.0/trytond_sale_secondary_unit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:49:28.000000 trytond_sale_secondary_unit-7.2.0/trytond_sale_secondary_unit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2024-04-29 15:49:28.000000 trytond_sale_secondary_unit-7.2.0/trytond_sale_secondary_unit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_sale_secondary_unit-7.2.0/trytond_sale_secondary_unit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2024-04-29 15:49:28.000000 trytond_sale_secondary_unit-7.2.0/trytond_sale_secondary_unit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:49:28.000000 trytond_sale_secondary_unit-7.2.0/trytond_sale_secondary_unit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:29.208561 trytond_sale_secondary_unit-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      665 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/view/product_customer_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      711 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      642 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/view/sale_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_sale_secondary_unit-7.2.0/view/stock_move_list.xml
```

### Comparing `trytond_sale_secondary_unit-7.0.0/CHANGELOG` & `trytond_sale_secondary_unit-7.2.0/CHANGELOG`

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

### Comparing `trytond_sale_secondary_unit-7.0.0/LICENSE` & `trytond_sale_secondary_unit-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/PKG-INFO` & `trytond_sale_secondary_unit-7.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_secondary_unit
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add a secondary unit on sale line
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
@@ -46,25 +46,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_secondary_unit<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_blanket_agreement<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_secondary_unit<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_product_customer<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_secondary_unit<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_blanket_agreement<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_secondary_unit<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_product_customer<7.3,>=7.2; extra == "test"
 
 Sale Secondary Unit Module
 ##########################
 
 The sale secondary unit module adds a secondary unit of measure on sale lines.
 The secondary quantity and unit price are kept synchronized with the quantity
 and unit price.
```

### Comparing `trytond_sale_secondary_unit-7.0.0/__init__.py` & `trytond_sale_secondary_unit-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/account.py` & `trytond_sale_secondary_unit-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/doc/conf.py` & `trytond_sale_secondary_unit-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/bg.po` & `trytond_sale_secondary_unit-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/ca.po` & `trytond_sale_secondary_unit-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/cs.po` & `trytond_sale_secondary_unit-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/de.po` & `trytond_sale_secondary_unit-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/es.po` & `trytond_sale_secondary_unit-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/es_419.po` & `trytond_sale_secondary_unit-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/et.po` & `trytond_sale_secondary_unit-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/fa.po` & `trytond_sale_secondary_unit-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/fi.po` & `trytond_sale_secondary_unit-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/fr.po` & `trytond_sale_secondary_unit-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/hu.po` & `trytond_sale_secondary_unit-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/id.po` & `trytond_sale_secondary_unit-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/it.po` & `trytond_sale_secondary_unit-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/lo.po` & `trytond_sale_secondary_unit-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/lt.po` & `trytond_sale_secondary_unit-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/nl.po` & `trytond_sale_secondary_unit-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/pl.po` & `trytond_sale_secondary_unit-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/pt.po` & `trytond_sale_secondary_unit-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/ro.po` & `trytond_sale_secondary_unit-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/ru.po` & `trytond_sale_secondary_unit-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/sl.po` & `trytond_sale_secondary_unit-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/tr.po` & `trytond_sale_secondary_unit-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/uk.po` & `trytond_sale_secondary_unit-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/locale/zh_CN.po` & `trytond_sale_secondary_unit-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/product.py` & `trytond_sale_secondary_unit-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/product.xml` & `trytond_sale_secondary_unit-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/sale.py` & `trytond_sale_secondary_unit-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/sale.xml` & `trytond_sale_secondary_unit-7.2.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/setup.py` & `trytond_sale_secondary_unit-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/stock.py` & `trytond_sale_secondary_unit-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/tests/scenario_sale_blanket_agreement_secondary_unit.rst` & `trytond_sale_secondary_unit-7.2.0/tests/scenario_sale_blanket_agreement_secondary_unit.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 ==============================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
     >>> later = today + dt.timedelta(days=30)
 
 Activate modules::
 
     >>> config = activate_modules([
@@ -83,32 +81,28 @@
     >>> blanket_agreement.click('run')
     >>> blanket_agreement.state
     'running'
 
 Create sale from blanket agreement::
 
     >>> create_sale = blanket_agreement.click('create_sale')
-    >>> create_sale.form.lines[0].unit == gr
-    True
+    >>> assertEqual(create_sale.form.lines[0].unit, gr)
     >>> create_sale.execute('create_sale')
 
     >>> sale, = create_sale.actions[0]
     >>> line, = sale.lines
-    >>> line.product == product
-    True
+    >>> assertEqual(line.product, product)
 
-    >>> line.secondary_unit == gr
-    True
+    >>> assertEqual(line.secondary_unit, gr)
     >>> line.secondary_quantity
     800.0
     >>> line.secondary_unit_price
     Decimal('9.0000')
 
-    >>> line.unit == unit
-    True
+    >>> assertEqual(line.unit, unit)
     >>> line.quantity
     8.0
     >>> line.unit_price
     Decimal('900.0000')
 
     >>> line.secondary_quantity = 300.0
     >>> sale.save()
```

### Comparing `trytond_sale_secondary_unit-7.0.0/tests/scenario_sale_secondary_unit.rst` & `trytond_sale_secondary_unit-7.2.0/tests/scenario_sale_secondary_unit.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 ============================
 Sale Secondary Unit Scenario
 ============================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules(
     ...     ['sale_secondary_unit',
     ...     'account_invoice_secondary_unit',
     ...     'stock_secondary_unit'])
@@ -106,30 +105,27 @@
     >>> sale.shipment_state
     'waiting'
 
 Check secondary unit on invoice::
 
     >>> invoice, = sale.invoices
     >>> line, = invoice.lines
-    >>> line.secondary_unit == kg
-    True
+    >>> assertEqual(line.secondary_unit, kg)
     >>> line.secondary_quantity
     2.0
     >>> line.secondary_unit_price
     Decimal('50.0000')
 
 Check secondary unit on move::
 
     >>> move, = sale.moves
-    >>> move.secondary_unit == kg
-    True
+    >>> assertEqual(move.secondary_unit, kg)
     >>> move.secondary_quantity
     2.0
     >>> move.secondary_unit_price
     Decimal('50.0000')
 
     >>> shipment, = sale.shipments
     >>> move, = shipment.inventory_moves
-    >>> move.secondary_unit == kg
-    True
+    >>> assertEqual(move.secondary_unit, kg)
     >>> move.secondary_quantity
     2.0
```

### Comparing `trytond_sale_secondary_unit-7.0.0/tox.ini` & `trytond_sale_secondary_unit-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/trytond_sale_secondary_unit.egg-info/PKG-INFO` & `trytond_sale_secondary_unit-7.2.0/trytond_sale_secondary_unit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-sale-secondary-unit
-Version: 7.0.0
+Name: trytond_sale_secondary_unit
+Version: 7.2.0
 Summary: Tryton module to add a secondary unit on sale line
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
@@ -46,25 +46,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_secondary_unit<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_blanket_agreement<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_secondary_unit<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_product_customer<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_secondary_unit<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_blanket_agreement<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_secondary_unit<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_product_customer<7.3,>=7.2; extra == "test"
 
 Sale Secondary Unit Module
 ##########################
 
 The sale secondary unit module adds a secondary unit of measure on sale lines.
 The secondary quantity and unit price are kept synchronized with the quantity
 and unit price.
```

### Comparing `trytond_sale_secondary_unit-7.0.0/trytond_sale_secondary_unit.egg-info/SOURCES.txt` & `trytond_sale_secondary_unit-7.2.0/trytond_sale_secondary_unit.egg-info/SOURCES.txt`

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

### Comparing `trytond_sale_secondary_unit-7.0.0/view/product_customer_form.xml` & `trytond_sale_secondary_unit-7.2.0/view/product_customer_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/view/product_template_form.xml` & `trytond_sale_secondary_unit-7.2.0/view/product_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_secondary_unit-7.0.0/view/sale_line_form.xml` & `trytond_sale_secondary_unit-7.2.0/view/sale_line_form.xml`

 * *Files identical despite different names*

