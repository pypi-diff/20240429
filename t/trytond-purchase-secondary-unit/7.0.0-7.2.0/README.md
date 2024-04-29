# Comparing `tmp/trytond_purchase_secondary_unit-7.0.0.tar.gz` & `tmp/trytond_purchase_secondary_unit-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_secondary_unit-7.0.0.tar", last modified: Mon Oct 30 17:36:17 2023, max compression
+gzip compressed data, was "trytond_purchase_secondary_unit-7.2.0.tar", last modified: Mon Apr 29 15:46:33 2024, max compression
```

## Comparing `trytond_purchase_secondary_unit-7.0.0.tar` & `trytond_purchase_secondary_unit-7.2.0.tar`

### file list

```diff
@@ -1,71 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:17.160611 trytond_purchase_secondary_unit-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-10-22 17:23:15.000000 trytond_purchase_secondary_unit-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      897 2023-10-30 17:11:04.000000 trytond_purchase_secondary_unit-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:11:04.000000 trytond_purchase_secondary_unit-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3242 2023-10-30 17:36:17.160611 trytond_purchase_secondary_unit-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      852 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1225 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:17.157278 trytond_purchase_secondary_unit-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2824 2023-10-22 17:23:15.000000 trytond_purchase_secondary_unit-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:15.000000 trytond_purchase_secondary_unit-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:17.153945 trytond_purchase_secondary_unit-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6815 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6848 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6819 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6908 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6952 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5107 2023-10-30 16:47:45.000000 trytond_purchase_secondary_unit-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6691 2023-10-24 07:56:52.000000 trytond_purchase_secondary_unit-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      770 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    15288 2023-10-24 07:56:52.000000 trytond_purchase_secondary_unit-7.0.0/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1044 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:36:17.160611 trytond_purchase_secondary_unit-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4750 2023-10-27 17:38:49.000000 trytond_purchase_secondary_unit-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1208 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:17.153945 trytond_purchase_secondary_unit-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3876 2023-06-10 11:39:56.000000 trytond_purchase_secondary_unit-7.0.0/tests/scenario_purchase_blanket_agreement_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3229 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/tests/scenario_purchase_requisition_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4005 2023-10-24 07:56:52.000000 trytond_purchase_secondary_unit-7.0.0/tests/scenario_purchase_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_purchase_secondary_unit-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-10-30 17:10:59.000000 trytond_purchase_secondary_unit-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:17.157278 trytond_purchase_secondary_unit-7.0.0/trytond_purchase_secondary_unit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3242 2023-10-30 17:36:16.000000 trytond_purchase_secondary_unit-7.0.0/trytond_purchase_secondary_unit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2204 2023-10-30 17:36:17.000000 trytond_purchase_secondary_unit-7.0.0/trytond_purchase_secondary_unit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:36:16.000000 trytond_purchase_secondary_unit-7.0.0/trytond_purchase_secondary_unit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-10-30 17:36:16.000000 trytond_purchase_secondary_unit-7.0.0/trytond_purchase_secondary_unit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:07.000000 trytond_purchase_secondary_unit-7.0.0/trytond_purchase_secondary_unit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-10-30 17:36:16.000000 trytond_purchase_secondary_unit-7.0.0/trytond_purchase_secondary_unit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:36:16.000000 trytond_purchase_secondary_unit-7.0.0/trytond_purchase_secondary_unit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:36:17.157278 trytond_purchase_secondary_unit-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      693 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/view/product_supplier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      723 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      642 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/view/purchase_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.0.0/view/stock_move_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:33.079834 trytond_purchase_secondary_unit-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      998 2024-04-29 15:24:16.000000 trytond_purchase_secondary_unit-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:24:15.000000 trytond_purchase_secondary_unit-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3242 2024-04-29 15:46:33.079834 trytond_purchase_secondary_unit-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      852 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1225 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:33.073167 trytond_purchase_secondary_unit-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-27 16:30:39.000000 trytond_purchase_secondary_unit-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:22.000000 trytond_purchase_secondary_unit-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:33.076501 trytond_purchase_secondary_unit-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6851 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6884 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6855 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6917 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6988 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5116 2024-04-29 13:17:17.000000 trytond_purchase_secondary_unit-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6694 2024-03-17 11:01:36.000000 trytond_purchase_secondary_unit-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      770 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    15288 2024-02-04 18:51:26.000000 trytond_purchase_secondary_unit-7.2.0/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1044 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:46:33.079834 trytond_purchase_secondary_unit-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4750 2024-03-17 11:01:36.000000 trytond_purchase_secondary_unit-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1208 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:33.076501 trytond_purchase_secondary_unit-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-22 12:14:36.000000 trytond_purchase_secondary_unit-7.2.0/tests/scenario_purchase_blanket_agreement_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3214 2024-04-22 12:14:36.000000 trytond_purchase_secondary_unit-7.2.0/tests/scenario_purchase_requisition_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3987 2024-04-22 12:14:36.000000 trytond_purchase_secondary_unit-7.2.0/tests/scenario_purchase_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:22.000000 trytond_purchase_secondary_unit-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2024-04-29 15:24:11.000000 trytond_purchase_secondary_unit-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:33.076501 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3242 2024-04-29 15:46:32.000000 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2186 2024-04-29 15:46:33.000000 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:46:32.000000 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-04-29 15:46:32.000000 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:07.000000 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2024-04-29 15:46:32.000000 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:46:32.000000 trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:46:33.076501 trytond_purchase_secondary_unit-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      693 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/view/product_supplier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      723 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      642 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/view/purchase_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_purchase_secondary_unit-7.2.0/view/stock_move_list.xml
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/CHANGELOG` & `trytond_purchase_secondary_unit-7.2.0/CHANGELOG`

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

### Comparing `trytond_purchase_secondary_unit-7.0.0/LICENSE` & `trytond_purchase_secondary_unit-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.0.0/PKG-INFO` & `trytond_purchase_secondary_unit-7.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_secondary_unit
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add a secondary unit on purchase line
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
@@ -46,26 +46,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_secondary_unit<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_blanket_agreement<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_request<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_requisition<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_secondary_unit<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_secondary_unit<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_blanket_agreement<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_request<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_requisition<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_secondary_unit<7.3,>=7.2; extra == "test"
 
 Purchase Secondary Unit Module
 ##############################
 
 The purchase secondary unit module adds a secondary unit of measure on purchase
 lines.
 The secondary quantity and unit price are kept synchronized with the quantity
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/__init__.py` & `trytond_purchase_secondary_unit-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.0.0/account.py` & `trytond_purchase_secondary_unit-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.0.0/doc/conf.py` & `trytond_purchase_secondary_unit-7.2.0/doc/conf.py`

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

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/bg.po` & `trytond_purchase_secondary_unit-7.2.0/locale/bg.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/ca.po` & `trytond_purchase_secondary_unit-7.2.0/locale/ca.po`

 * *Files 1% similar despite different names*

```diff
@@ -83,16 +83,17 @@
 msgid "Purchase Secondary UoM Rate"
 msgstr "Rati UdM de compra secundaria"
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr "Categoria de la UdM secundaria del producte"
 
+#, fuzzy
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr "La unitat de mesura secundaria de les compres."
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -103,16 +104,17 @@
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 "El coeficient de la formula:\n"
 "coeficent (unitat_compra) = 1 (unitat_secundaria)"
 
+#, fuzzy
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr "La unitat de mesura secundaria de les compres."
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -143,16 +145,17 @@
 msgid "The rate for the secondary Unit of Measure."
 msgstr "El rati de la unitat de mesura secundaria."
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr "La categoria de la unitat de mesura per defecte."
 
+#, fuzzy
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr "La unitat de mesura secundaria de les compres."
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/cs.po` & `trytond_purchase_secondary_unit-7.2.0/locale/cs.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/de.po` & `trytond_purchase_secondary_unit-7.2.0/locale/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,17 @@
 msgid "Purchase Secondary UoM Rate"
 msgstr "Einkauf Zweitmaßeinheit Kehrwert Faktor"
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr "Artikel Zweitmaßeinheitenkategorie"
 
+#, fuzzy
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr "Die zweite Maßeinheit für Einkäufe."
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -103,16 +104,17 @@
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 "Der Koeffizient für die Formel:\n"
 "Koeffizient(Einkaufseinheit) = 1 (Zweitmaßeinheit)"
 
+#, fuzzy
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr "Die zweite Maßeinheit für Einkäufe."
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -143,16 +145,17 @@
 msgid "The rate for the secondary Unit of Measure."
 msgstr "Der Kehrwert Faktor für die zweite Maßeinheit."
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr "Die Kategorie für die Standardmaßeinheit."
 
+#, fuzzy
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr "Die zweite Maßeinheit für Einkäufe."
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/es.po` & `trytond_purchase_secondary_unit-7.2.0/locale/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,17 @@
 msgid "Purchase Secondary UoM Rate"
 msgstr "Ratio UdM compra secundaria"
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr "Categoría de la UdM secundaria del producto"
 
+#, fuzzy
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr "La unidad de medida secundaria de las compras."
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -103,16 +104,17 @@
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 "El coeficiente de la fórmula:\n"
 "coeficiente (unidad_compra) = 1 (unidad secundaria)"
 
+#, fuzzy
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr "La unidad de medida secundaria de las compras."
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -143,16 +145,17 @@
 msgid "The rate for the secondary Unit of Measure."
 msgstr "El ratio de la unidad de medida secundaria."
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr "La categoría de la unidad de medida por defecto."
 
+#, fuzzy
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr "La unidad de medida secundaria de las compras."
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/es_419.po` & `trytond_purchase_secondary_unit-7.2.0/locale/es_419.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/et.po` & `trytond_purchase_secondary_unit-7.2.0/locale/et.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/fa.po` & `trytond_purchase_secondary_unit-7.2.0/locale/fa.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/fi.po` & `trytond_purchase_secondary_unit-7.2.0/locale/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/fr.po` & `trytond_purchase_secondary_unit-7.2.0/locale/fr.po`

 * *Files 6% similar despite different names*

```diff
@@ -84,16 +84,16 @@
 msgstr "Taux d'UDM secondaire d'achat"
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr "Catégorie d'UDM secondaire du produit"
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
-msgstr "L'Unité De Mesure secondaire pour les achats."
+msgid "The secondary Unit of Measure for purchases."
+msgstr "L'unité de mesure secondaire pour les achats."
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
 "Le coefficient pour la formule :\n"
@@ -104,16 +104,16 @@
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 "Le coefficient pour la formule :\n"
 "coefficient (unité d'achat) = 1 (unité secondaire)"
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
-msgstr "L'Unité De Mesure secondaire pour les achats."
+msgid "The secondary Unit of Measure for purchases."
+msgstr "L'unité de mesure secondaire pour les achats."
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
 "Le coefficient pour la formule :\n"
@@ -144,16 +144,16 @@
 msgstr "Le taux pour l’Unité De Mesure secondaire."
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr "La catégorie de l'Unité De Mesure par défaut."
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
-msgstr "L'Unité De Mesure secondaire pour les achats."
+msgid "The secondary Unit of Measure for purchases."
+msgstr "L'unité de mesure secondaire pour les achats."
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
 "Le coefficient pour la formule :\n"
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/hu.po` & `trytond_purchase_secondary_unit-7.2.0/locale/hu.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/id.po` & `trytond_purchase_secondary_unit-7.2.0/locale/id.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/it.po` & `trytond_purchase_secondary_unit-7.2.0/locale/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/lo.po` & `trytond_purchase_secondary_unit-7.2.0/locale/lo.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/lt.po` & `trytond_purchase_secondary_unit-7.2.0/locale/lt.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/nl.po` & `trytond_purchase_secondary_unit-7.2.0/locale/nl.po`

 * *Files 4% similar despite different names*

```diff
@@ -83,16 +83,17 @@
 msgid "Purchase Secondary UoM Rate"
 msgstr "Inkoop secundaire maateenheid verhouding"
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr "Product secundaire maateenheid categorie"
 
+#, fuzzy
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr "De tweede maateenheid voor inkopen."
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -103,16 +104,17 @@
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 "De coëfficiënt voor de formule:\n"
 "coëfficiënt (inkoopeenheid) = 1 (secundaire eenheid)"
 
+#, fuzzy
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr "De tweede maateenheid voor inkopen."
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -143,16 +145,17 @@
 msgid "The rate for the secondary Unit of Measure."
 msgstr "De verhouding voor de secundaire maateenheid."
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr "De categorie van de standaard maateenheid."
 
+#, fuzzy
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr "De tweede maateenheid voor inkopen."
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/pl.po` & `trytond_purchase_secondary_unit-7.2.0/locale/pl.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/pt.po` & `trytond_purchase_secondary_unit-7.2.0/locale/pt.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/ro.po` & `trytond_purchase_secondary_unit-7.2.0/locale/ro.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/ru.po` & `trytond_purchase_secondary_unit-7.2.0/locale/ru.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/sl.po` & `trytond_purchase_secondary_unit-7.2.0/locale/sl.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/tr.po` & `trytond_purchase_secondary_unit-7.2.0/locale/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/uk.po` & `trytond_purchase_secondary_unit-7.2.0/locale/uk.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/locale/zh_CN.po` & `trytond_purchase_secondary_unit-7.2.0/locale/zh_CN.po`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 msgstr ""
 
 msgctxt "field:purchase.requisition.line,product_secondary_uom_category:"
 msgid "Product Secondary UoM Category"
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.product,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -100,15 +100,15 @@
 msgctxt "help:product.product,purchase_secondary_uom_rate:"
 msgid ""
 "The coefficient for the formula:\n"
 "coefficient (purchase unit) = 1 (secondary unit)"
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:product.template,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
@@ -136,15 +136,15 @@
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,default_uom_category:"
 msgid "The category of the default Unit of Measure."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom:"
-msgid "The second Unit of Measure for purchases."
+msgid "The secondary Unit of Measure for purchases."
 msgstr ""
 
 msgctxt "help:purchase.product_supplier,purchase_secondary_uom_factor:"
 msgid ""
 "The coefficient for the formula:\n"
 "1 (purchase unit) = coefficient (secondary unit)"
 msgstr ""
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/product.py` & `trytond_purchase_secondary_unit-7.2.0/product.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class PurchaseSecondaryMixin:
     __slots__ = ()
     purchase_secondary_uom = fields.Many2One(
         'product.uom', "Purchase Secondary UoM",
         domain=[
             ('category', '!=', Eval('default_uom_category')),
             ],
-        help="The second Unit of Measure for purchases.")
+        help="The secondary Unit of Measure for purchases.")
     purchase_secondary_uom_factor = fields.Float(
         "Purchase Secondary UoM Factor", digits=uom_conversion_digits,
         states={
             'required': Bool(Eval('purchase_secondary_uom')),
             'invisible': ~Eval('purchase_secondary_uom'),
             },
         help="The coefficient for the formula:\n"
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/product.xml` & `trytond_purchase_secondary_unit-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.0.0/purchase.py` & `trytond_purchase_secondary_unit-7.2.0/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.0.0/purchase.xml` & `trytond_purchase_secondary_unit-7.2.0/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.0.0/setup.py` & `trytond_purchase_secondary_unit-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.0.0/stock.py` & `trytond_purchase_secondary_unit-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.0.0/tests/scenario_purchase_blanket_agreement_secondary_unit.rst` & `trytond_purchase_secondary_unit-7.2.0/tests/scenario_purchase_blanket_agreement_secondary_unit.rst`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
     >>> later = today + dt.timedelta(days=30)
 
 
 Activate modules::
 
@@ -85,32 +83,28 @@
     >>> blanket_agreement.state
     'running'
 
 Create purchase from blanket agreement::
 
     >>> create_purchase = Wizard(
     ...     'purchase.blanket_agreement.create_purchase', [blanket_agreement])
-    >>> create_purchase.form.lines[0].unit == gr
-    True
+    >>> assertEqual(create_purchase.form.lines[0].unit, gr)
     >>> create_purchase.execute('create_purchase')
 
     >>> purchase, = create_purchase.actions[0]
     >>> line, = purchase.lines
-    >>> line.product == product
-    True
+    >>> assertEqual(line.product, product)
 
-    >>> line.secondary_unit == gr
-    True
+    >>> assertEqual(line.secondary_unit, gr)
     >>> line.secondary_quantity
     800.0
     >>> line.secondary_unit_price
     Decimal('7.0000')
 
-    >>> line.unit == unit
-    True
+    >>> assertEqual(line.unit, unit)
     >>> line.quantity
     8.0
     >>> line.unit_price
     Decimal('700.0000')
 
     >>> line.secondary_quantity = 300.0
     >>> purchase.save()
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/tests/scenario_purchase_requisition_secondary_unit.rst` & `trytond_purchase_secondary_unit-7.2.0/tests/scenario_purchase_requisition_secondary_unit.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
-    >>> from trytond.modules.account.tests.tools import (
-    ...     create_chart, get_accounts)
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'purchase_secondary_unit',
@@ -96,13 +94,12 @@
 
     >>> request, = PurchaseRequest.find([('state', '=', 'draft')])
     >>> create_purchase = Wizard('purchase.request.create_purchase', [request])
     >>> create_purchase.form.party = supplier
     >>> create_purchase.execute('start')
     >>> request.state
     'purchased'
-    >>> request.purchase_line.unit == unit
-    True
+    >>> assertEqual(request.purchase_line.unit, unit)
     >>> request.purchase_line.quantity
     3.0
     >>> request.purchase_line.unit_price
     Decimal('200.0000')
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/tests/scenario_purchase_secondary_unit.rst` & `trytond_purchase_secondary_unit-7.2.0/tests/scenario_purchase_secondary_unit.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 ================================
 Purchase Secondary Unit Scenario
 ================================
 
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
 
     >>> config = activate_modules([
     ...         'purchase_secondary_unit',
     ...         'account_invoice_secondary_unit',
     ...         'stock_secondary_unit'])
@@ -119,23 +118,21 @@
     >>> purchase.shipment_state
     'waiting'
 
 Check secondary unit on invoice::
 
     >>> invoice, = purchase.invoices
     >>> line, = invoice.lines
-    >>> line.secondary_unit == kg
-    True
+    >>> assertEqual(line.secondary_unit, kg)
     >>> line.secondary_quantity
     2.0
     >>> line.secondary_unit_price
     Decimal('15.0000')
 
 Check secondary unit on move::
 
     >>> move, = purchase.moves
-    >>> move.secondary_unit == kg
-    True
+    >>> assertEqual(move.secondary_unit, kg)
     >>> move.secondary_quantity
     2.0
     >>> move.secondary_unit_price
     Decimal('15.0000')
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/tox.ini` & `trytond_purchase_secondary_unit-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.0.0/trytond_purchase_secondary_unit.egg-info/PKG-INFO` & `trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-purchase-secondary-unit
-Version: 7.0.0
+Name: trytond_purchase_secondary_unit
+Version: 7.2.0
 Summary: Tryton module to add a secondary unit on purchase line
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
@@ -46,26 +46,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_purchase<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_purchase<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_invoice_secondary_unit<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_blanket_agreement<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_request<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase_requisition<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_secondary_unit<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_invoice_secondary_unit<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_blanket_agreement<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_request<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase_requisition<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_secondary_unit<7.3,>=7.2; extra == "test"
 
 Purchase Secondary Unit Module
 ##############################
 
 The purchase secondary unit module adds a secondary unit of measure on purchase
 lines.
 The secondary quantity and unit price are kept synchronized with the quantity
```

### Comparing `trytond_purchase_secondary_unit-7.0.0/trytond_purchase_secondary_unit.egg-info/SOURCES.txt` & `trytond_purchase_secondary_unit-7.2.0/trytond_purchase_secondary_unit.egg-info/SOURCES.txt`

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

### Comparing `trytond_purchase_secondary_unit-7.0.0/view/product_supplier_form.xml` & `trytond_purchase_secondary_unit-7.2.0/view/product_supplier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.0.0/view/product_template_form.xml` & `trytond_purchase_secondary_unit-7.2.0/view/product_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_secondary_unit-7.0.0/view/purchase_line_form.xml` & `trytond_purchase_secondary_unit-7.2.0/view/purchase_line_form.xml`

 * *Files identical despite different names*

