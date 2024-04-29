# Comparing `tmp/trytond_sale_product_customer-7.0.1.tar.gz` & `tmp/trytond_sale_product_customer-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_product_customer-7.0.1.tar", last modified: Sat Feb  3 11:18:20 2024, max compression
+gzip compressed data, was "trytond_sale_product_customer-7.2.0.tar", last modified: Mon Apr 29 15:48:47 2024, max compression
```

## Comparing `trytond_sale_product_customer-7.0.1.tar` & `trytond_sale_product_customer-7.2.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:18:20.254046 trytond_sale_product_customer-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      223 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1114 2024-02-03 11:18:12.000000 trytond_sale_product_customer-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      719 2024-02-03 11:18:11.000000 trytond_sale_product_customer-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2948 2024-02-03 11:18:20.254046 trytond_sale_product_customer-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      899 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:18:20.244042 trytond_sale_product_customer-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2822 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:18:20.247376 trytond_sale_product_customer-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1236 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1208 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1252 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1249 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1216 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1254 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1218 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1237 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6053 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8023 2024-01-26 18:05:24.000000 trytond_sale_product_customer-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4759 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-02-03 11:18:20.254046 trytond_sale_product_customer-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4591 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:18:20.247376 trytond_sale_product_customer-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1670 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/tests/scenario_sale_copy_product_customer.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1923 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/tests/scenario_sale_product_customer.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      155 2023-10-30 17:55:12.000000 trytond_sale_product_customer-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:18:20.254046 trytond_sale_product_customer-7.0.1/trytond_sale_product_customer.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2948 2024-02-03 11:18:19.000000 trytond_sale_product_customer-7.0.1/trytond_sale_product_customer.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2308 2024-02-03 11:18:20.000000 trytond_sale_product_customer-7.0.1/trytond_sale_product_customer.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-02-03 11:18:19.000000 trytond_sale_product_customer-7.0.1/trytond_sale_product_customer.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-02-03 11:18:19.000000 trytond_sale_product_customer-7.0.1/trytond_sale_product_customer.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:08.000000 trytond_sale_product_customer-7.0.1/trytond_sale_product_customer.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      167 2024-02-03 11:18:19.000000 trytond_sale_product_customer-7.0.1/trytond_sale_product_customer.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-02-03 11:18:19.000000 trytond_sale_product_customer-7.0.1/trytond_sale_product_customer.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:18:20.254046 trytond_sale_product_customer-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      671 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/view/product_customer_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/view/product_customer_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/view/product_customer_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/view/sale_amendment_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/view/sale_blanket_agreement_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/view/sale_blanket_agreement_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/view/sale_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/view/sale_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2023-10-30 17:06:38.000000 trytond_sale_product_customer-7.0.1/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:47.722979 trytond_sale_product_customer-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1114 2024-04-29 15:25:52.000000 trytond_sale_product_customer-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      719 2024-04-29 15:25:52.000000 trytond_sale_product_customer-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-04-29 15:48:47.722979 trytond_sale_product_customer-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      964 2024-04-27 16:30:39.000000 trytond_sale_product_customer-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      629 2024-04-27 16:30:39.000000 trytond_sale_product_customer-7.2.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:47.719646 trytond_sale_product_customer-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3084 2024-04-27 16:30:39.000000 trytond_sale_product_customer-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:27.000000 trytond_sale_product_customer-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:47.719646 trytond_sale_product_customer-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1236 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1208 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1252 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1249 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1216 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1254 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1218 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1237 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:26.000000 trytond_sale_product_customer-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6066 2024-04-27 16:30:39.000000 trytond_sale_product_customer-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8255 2024-04-27 16:30:39.000000 trytond_sale_product_customer-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4713 2024-04-27 16:30:39.000000 trytond_sale_product_customer-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:48:47.722979 trytond_sale_product_customer-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4591 2024-03-17 11:01:36.000000 trytond_sale_product_customer-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      612 2024-04-27 16:30:39.000000 trytond_sale_product_customer-7.2.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:47.719646 trytond_sale_product_customer-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1672 2024-04-22 12:14:36.000000 trytond_sale_product_customer-7.2.0/tests/scenario_sale_copy_product_customer.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1894 2024-04-22 12:14:36.000000 trytond_sale_product_customer-7.2.0/tests/scenario_sale_product_customer.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:27.000000 trytond_sale_product_customer-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2024-04-29 15:25:48.000000 trytond_sale_product_customer-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:47.722979 trytond_sale_product_customer-7.2.0/trytond_sale_product_customer.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-04-29 15:48:47.000000 trytond_sale_product_customer-7.2.0/trytond_sale_product_customer.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2334 2024-04-29 15:48:47.000000 trytond_sale_product_customer-7.2.0/trytond_sale_product_customer.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:48:47.000000 trytond_sale_product_customer-7.2.0/trytond_sale_product_customer.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:48:47.000000 trytond_sale_product_customer-7.2.0/trytond_sale_product_customer.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:03.000000 trytond_sale_product_customer-7.2.0/trytond_sale_product_customer.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-04-29 15:48:47.000000 trytond_sale_product_customer-7.2.0/trytond_sale_product_customer.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:48:47.000000 trytond_sale_product_customer-7.2.0/trytond_sale_product_customer.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:48:47.722979 trytond_sale_product_customer-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      671 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/view/product_customer_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/view/product_customer_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/view/product_customer_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/view/sale_amendment_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/view/sale_blanket_agreement_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/view/sale_blanket_agreement_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/view/sale_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-04-15 07:12:15.000000 trytond_sale_product_customer-7.2.0/view/sale_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-02-04 18:51:26.000000 trytond_sale_product_customer-7.2.0/view/template_form.xml
```

### Comparing `trytond_sale_product_customer-7.0.1/CHANGELOG` & `trytond_sale_product_customer-7.2.0/CHANGELOG`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-02-03
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_sale_product_customer-7.0.1/COPYRIGHT` & `trytond_sale_product_customer-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/LICENSE` & `trytond_sale_product_customer-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/PKG-INFO` & `trytond_sale_product_customer-7.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_product_customer
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to manage customer product on sale
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
@@ -47,21 +47,23 @@
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
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_amendment<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_blanket_agreement<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_amendment<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_blanket_agreement<7.3,>=7.2; extra == "test"
 
 Sale Product Customer Module
 ############################
 
 The sale_product_customer module defines customer's names and
 codes for products and/or variants.
```

### Comparing `trytond_sale_product_customer-7.0.1/__init__.py` & `trytond_sale_product_customer-7.2.0/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 from trytond.pool import Pool
 
-from . import product, sale
+from . import account, product, sale, stock
 
 __all__ = ['register']
 
 
 def register():
     Pool.register(
         product.Template,
         product.Product,
         product.ProductCustomer,
         sale.Line,
+        account.InvoiceLine,
+        stock.Move,
         module='sale_product_customer', type_='model')
     Pool.register(
         sale.AmendmentLine,
         module='sale_product_customer', type_='model',
         depends=['sale_amendment'])
     Pool.register(
         sale.LineBlanketAgreement,
```

### Comparing `trytond_sale_product_customer-7.0.1/doc/conf.py` & `trytond_sale_product_customer-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_product_customer-7.0.1/locale/bg.po` & `trytond_sale_product_customer-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/ca.po` & `trytond_sale_product_customer-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/cs.po` & `trytond_sale_product_customer-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/de.po` & `trytond_sale_product_customer-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/es.po` & `trytond_sale_product_customer-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/es_419.po` & `trytond_sale_product_customer-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/et.po` & `trytond_sale_product_customer-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/fa.po` & `trytond_sale_product_customer-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/fi.po` & `trytond_sale_product_customer-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/fr.po` & `trytond_sale_product_customer-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/hu.po` & `trytond_sale_product_customer-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/id.po` & `trytond_sale_product_customer-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/it.po` & `trytond_sale_product_customer-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/lo.po` & `trytond_sale_product_customer-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/lt.po` & `trytond_sale_product_customer-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/nl.po` & `trytond_sale_product_customer-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/pl.po` & `trytond_sale_product_customer-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/pt.po` & `trytond_sale_product_customer-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/ro.po` & `trytond_sale_product_customer-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/ru.po` & `trytond_sale_product_customer-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/sl.po` & `trytond_sale_product_customer-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/tr.po` & `trytond_sale_product_customer-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/uk.po` & `trytond_sale_product_customer-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/locale/zh_CN.po` & `trytond_sale_product_customer-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/product.py` & `trytond_sale_product_customer-7.2.0/product.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 from trytond.model import (
-    DeactivableMixin, MatchMixin, ModelSQL, ModelView, fields,
-    sequence_ordered)
+    MatchMixin, ModelSQL, ModelView, fields, sequence_ordered)
+from trytond.modules.product import ProductDeactivatableMixin
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Bool, Eval, If
 from trytond.tools import is_full_text, lstrip_wildcard
 
 
 class ProductCustomer(
-        sequence_ordered(), DeactivableMixin, ModelSQL, ModelView, MatchMixin):
+        sequence_ordered(), ProductDeactivatableMixin, MatchMixin,
+        ModelSQL, ModelView):
     'Product Customer'
     __name__ = 'sale.product_customer'
 
     template = fields.Many2One(
         'product.template', "Product",
         required=True, ondelete='CASCADE',
         domain=[
             If(Bool(Eval('product')),
                 ('products', '=', Eval('product')),
                 ()),
-            If(Eval('active'), ('active', '=', True), ()),
             ],
         states={
             'readonly': Eval('id', -1) >= 0,
             })
     product = fields.Many2One(
         'product.product', "Variant",
         domain=[
             If(Bool(Eval('template')),
                 ('template', '=', Eval('template')),
                 ()),
-            If(Eval('active'), ('active', '=', True), ()),
             ],
         states={
             'readonly': Eval('id', -1) >= 0,
             })
     party = fields.Many2One(
         'party.party', "Customer", required=True, ondelete='CASCADE',
         states={
@@ -48,22 +47,28 @@
     @fields.depends(
         'product', '_parent_product.template')
     def on_change_product(self):
         if self.product:
             self.template = self.product.template
 
     def get_rec_name(self, name):
-        if self.name:
-            name = self.name
-        elif self.product:
-            name = self.product.name
+        if not self.name and not self.code:
+            if self.product:
+                name = self.product.rec_name
+            else:
+                name = self.template.rec_name
         else:
-            name = self.template.name
-        if self.code:
-            name = '[' + self.code + '] ' + name
+            if self.name:
+                name = self.name
+            elif self.product:
+                name = self.product.name
+            else:
+                name = self.template.name
+            if self.code:
+                name = '[' + self.code + '] ' + name
         return name
 
     @classmethod
     def search_rec_name(cls, name, clause):
         _, operator, operand, *extra = clause
         if operator.startswith('!') or operator.startswith('not '):
             bool_op = 'AND'
@@ -83,18 +88,15 @@
 
 class Template(metaclass=PoolMeta):
     __name__ = 'product.template'
     product_customers = fields.One2Many(
         'sale.product_customer', 'template', "Customers",
         states={
             'invisible': ~Eval('salable', False),
-            },
-        domain=[
-            If(~Eval('active'), ('active', '=', False), ()),
-            ])
+            })
 
     def product_customer_used(self, **pattern):
         for product_customer in self.product_customers:
             if product_customer.match(pattern):
                 yield product_customer
 
     @classmethod
@@ -125,15 +127,14 @@
 
 class Product(metaclass=PoolMeta):
     __name__ = 'product.product'
     product_customers = fields.One2Many(
         'sale.product_customer', 'product', "Customers",
         domain=[
             ('template', '=', Eval('template')),
-            If(~Eval('active'), ('active', '=', False), ()),
             ],
         states={
             'invisible': ~Eval('salable', False),
             })
 
     def product_customer_used(self, **pattern):
         for product_customer in self.product_customers:
```

### Comparing `trytond_sale_product_customer-7.0.1/sale.py` & `trytond_sale_product_customer-7.2.0/sale.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 
 from trytond.model import fields
 from trytond.pool import PoolMeta
 from trytond.pyson import Bool, Eval, If
+from trytond.tools import cached_property
 
 
 class Line(metaclass=PoolMeta):
     __name__ = 'sale.line'
 
     product_customer = fields.Many2One(
         'sale.product_customer', "Customer's Product",
@@ -58,14 +59,21 @@
             if self.product_customer.product:
                 self.product = self.product_customer.product
             elif not self.product:
                 if len(self.product_customer.template.products) == 1:
                     self.product, = self.product_customer.template.products
         self.on_change_product()
 
+    @cached_property
+    def product_name(self):
+        name = super().product_name
+        if self.product_customer:
+            name = self.product_customer.rec_name
+        return name
+
 
 class AmendmentLine(metaclass=PoolMeta):
     __name__ = 'sale.amendment.line'
 
     product_customer = fields.Many2One(
         'sale.product_customer', "Customer's Product",
         domain=[
```

### Comparing `trytond_sale_product_customer-7.0.1/sale.xml` & `trytond_sale_product_customer-7.2.0/sale.xml`

 * *Files 1% similar despite different names*

#### Comparing `trytond_sale_product_customer-7.0.1/sale.xml` & `trytond_sale_product_customer-7.2.0/sale.xml`

```diff
@@ -47,22 +47,22 @@
     <record model="ir.action.act_window.view" id="act_product_customer_form_view">
       <field name="sequence" eval="20"/>
       <field name="view" ref="product_customer_view_form"/>
       <field name="act_window" ref="act_product_customer_form"/>
     </record>
     <menuitem parent="product.menu_template" action="act_product_customer_form" sequence="20" id="menu_product_customer"/>
     <record model="ir.model.access" id="access_product_customer">
-      <field name="model" search="[('model', '=', 'sale.product_customer')]"/>
+      <field name="model">sale.product_customer</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_product_customer_sale">
-      <field name="model" search="[('model', '=', 'sale.product_customer')]"/>
+      <field name="model">sale.product_customer</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_sale_product_customer-7.0.1/setup.py` & `trytond_sale_product_customer-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/tests/scenario_sale_copy_product_customer.rst` & `trytond_sale_product_customer-7.2.0/tests/scenario_sale_copy_product_customer.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ===================================
 Sale Copy Product Customer Scenario
 ===================================
 
 Imports::
 
     >>> from decimal import Decimal
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('sale_product_customer')
 
 Create company::
 
@@ -40,16 +40,15 @@
     >>> template.cost_price_method = 'fixed'
     >>> product_customer = template.product_customers.new()
     >>> product_customer.party = customer
     >>> template.save()
     >>> product, = template.products
     >>> product_customer = product.product_customers.new()
     >>> product_customer.party = customer
-    >>> product_customer.template == template
-    True
+    >>> assertEqual(product_customer.template, template)
     >>> product.save()
 
 Customer is copied when copying the template::
 
     >>> template_copy, = template.duplicate()
     >>> product_copy, = template_copy.products
     >>> len(template_copy.product_customers)
```

### Comparing `trytond_sale_product_customer-7.0.1/tests/scenario_sale_product_customer.rst` & `trytond_sale_product_customer-7.2.0/tests/scenario_sale_product_customer.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ==============================
 Sale Product Customer Scenario
 ==============================
 
 Imports::
 
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
 
 Activate modules::
 
     >>> config = activate_modules('sale_product_customer')
 
 Create company::
 
@@ -65,9 +65,9 @@
     >>> template.save()
 
 Count product linked to customer::
 
     >>> ProductCustomer = Model.get('sale.product_customer')
     >>> products = ProductCustomer.find(
     ...     [('party', '=', customer.id)])
-    >>> len(products) == 2
-    True
+    >>> len(products)
+    2
```

### Comparing `trytond_sale_product_customer-7.0.1/tox.ini` & `trytond_sale_product_customer-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_product_customer-7.0.1/trytond_sale_product_customer.egg-info/PKG-INFO` & `trytond_sale_product_customer-7.2.0/trytond_sale_product_customer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_product_customer
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to manage customer product on sale
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
@@ -47,21 +47,23 @@
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
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_amendment<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_blanket_agreement<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_amendment<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_blanket_agreement<7.3,>=7.2; extra == "test"
 
 Sale Product Customer Module
 ############################
 
 The sale_product_customer module defines customer's names and
 codes for products and/or variants.
```

### Comparing `trytond_sale_product_customer-7.0.1/trytond_sale_product_customer.egg-info/SOURCES.txt` & `trytond_sale_product_customer-7.2.0/trytond_sale_product_customer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
+account.py
 product.py
 product.xml
 sale.py
 sale.xml
 setup.py
+stock.py
 tox.ini
 tryton.cfg
 ./__init__.py
+./account.py
 ./product.py
 ./product.xml
 ./sale.py
 ./sale.xml
+./stock.py
 ./tryton.cfg
 ./locale/bg.po
 ./locale/ca.po
 ./locale/cs.po
 ./locale/de.po
 ./locale/es.po
 ./locale/es_419.po
```

### Comparing `trytond_sale_product_customer-7.0.1/view/product_customer_form.xml` & `trytond_sale_product_customer-7.2.0/view/product_customer_form.xml`

 * *Files identical despite different names*

