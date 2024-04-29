# Comparing `tmp/trytond_web_shop_shopify-7.0.2.tar.gz` & `tmp/trytond_web_shop_shopify-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_shop_shopify-7.0.2.tar", last modified: Sat Feb  3 11:05:06 2024, max compression
+gzip compressed data, was "trytond_web_shop_shopify-7.2.0.tar", last modified: Mon Apr 29 15:54:10 2024, max compression
```

## Comparing `trytond_web_shop_shopify-7.0.2.tar` & `trytond_web_shop_shopify-7.2.0.tar`

### file list

```diff
@@ -1,88 +1,87 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:05:06.647541 trytond_web_shop_shopify-7.0.2/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1015 2024-02-03 11:04:58.000000 trytond_web_shop_shopify-7.0.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-02-03 11:04:57.000000 trytond_web_shop_shopify-7.0.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3701 2024-02-03 11:05:06.647541 trytond_web_shop_shopify-7.0.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2282 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5112 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5698 2023-11-27 22:51:19.000000 trytond_web_shop_shopify-7.0.2/common.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:05:06.630875 trytond_web_shop_shopify-7.0.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2817 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1206 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:05:06.637541 trytond_web_shop_shopify-7.0.2/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10401 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10720 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10444 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10685 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7596 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7584 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10331 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7575 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4150 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4339 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21497 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      790 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1995 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17230 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-02-03 11:05:06.647541 trytond_web_shop_shopify-7.0.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5043 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1075 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/shopify_retry.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6221 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2852 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:05:06.637541 trytond_web_shop_shopify-7.0.2/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19789 2024-01-26 17:50:56.000000 trytond_web_shop_shopify-7.0.2/tests/scenario_web_shop_shopify.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7417 2024-01-26 17:50:56.000000 trytond_web_shop_shopify-7.0.2/tests/scenario_web_shop_shopify_secondary_unit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-12-01 23:16:23.000000 trytond_web_shop_shopify-7.0.2/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:05:06.644208 trytond_web_shop_shopify-7.0.2/trytond_web_shop_shopify.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3701 2024-02-03 11:05:05.000000 trytond_web_shop_shopify-7.0.2/trytond_web_shop_shopify.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2785 2024-02-03 11:05:06.000000 trytond_web_shop_shopify-7.0.2/trytond_web_shop_shopify.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-02-03 11:05:05.000000 trytond_web_shop_shopify-7.0.2/trytond_web_shop_shopify.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-02-03 11:05:05.000000 trytond_web_shop_shopify-7.0.2/trytond_web_shop_shopify.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:21.000000 trytond_web_shop_shopify-7.0.2/trytond_web_shop_shopify.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      631 2024-02-03 11:05:05.000000 trytond_web_shop_shopify-7.0.2/trytond_web_shop_shopify.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-02-03 11:05:05.000000 trytond_web_shop_shopify-7.0.2/trytond_web_shop_shopify.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:05:06.644208 trytond_web_shop_shopify-7.0.2/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/view/product_attribute_set_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1201 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/view/shop_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/view/shop_shopify_identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/view/shop_shopify_identifier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      439 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/view/shop_shopify_payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      309 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/view/shop_shopify_payment_journal_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/view/shop_stock_location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-10-30 17:06:39.000000 trytond_web_shop_shopify-7.0.2/view/shop_stock_location_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/view/stock_shipment_shopify_identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/view/stock_shipment_shopify_identifier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    28233 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/web.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-10-30 17:06:38.000000 trytond_web_shop_shopify-7.0.2/web.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:10.951192 trytond_web_shop_shopify-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      914 2024-04-29 15:30:01.000000 trytond_web_shop_shopify-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:30:01.000000 trytond_web_shop_shopify-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3692 2024-04-29 15:54:10.951192 trytond_web_shop_shopify-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2282 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5112 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5698 2024-03-17 11:01:36.000000 trytond_web_shop_shopify-7.2.0/common.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:10.944526 trytond_web_shop_shopify-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_web_shop_shopify-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1745 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:39.000000 trytond_web_shop_shopify-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1194 2024-04-22 12:14:37.000000 trytond_web_shop_shopify-7.2.0/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2024-03-25 13:26:54.000000 trytond_web_shop_shopify-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:10.947859 trytond_web_shop_shopify-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10401 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10720 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10444 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10685 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7596 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7584 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10331 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7575 2024-04-27 16:43:28.000000 trytond_web_shop_shopify-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4150 2024-03-25 13:26:54.000000 trytond_web_shop_shopify-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4339 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21497 2024-02-04 18:51:27.000000 trytond_web_shop_shopify-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      790 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1995 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17230 2024-02-04 18:51:27.000000 trytond_web_shop_shopify-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:54:10.951192 trytond_web_shop_shopify-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     5034 2024-04-27 16:30:39.000000 trytond_web_shop_shopify-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1075 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/shopify_retry.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6221 2024-02-04 18:51:27.000000 trytond_web_shop_shopify-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2806 2024-04-27 16:30:39.000000 trytond_web_shop_shopify-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:10.947859 trytond_web_shop_shopify-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19751 2024-04-27 16:30:39.000000 trytond_web_shop_shopify-7.2.0/tests/scenario_web_shop_shopify.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7351 2024-04-22 12:14:37.000000 trytond_web_shop_shopify-7.2.0/tests/scenario_web_shop_shopify_secondary_unit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:39.000000 trytond_web_shop_shopify-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-04-29 15:29:57.000000 trytond_web_shop_shopify-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:10.947859 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3692 2024-04-29 15:54:10.000000 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2767 2024-04-29 15:54:10.000000 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:54:10.000000 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:54:10.000000 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      631 2024-04-29 15:54:10.000000 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:54:10.000000 trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:10.947859 trytond_web_shop_shopify-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/product_attribute_set_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1201 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/shop_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/shop_shopify_identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/shop_shopify_identifier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      439 2024-02-04 18:51:27.000000 trytond_web_shop_shopify-7.2.0/view/shop_shopify_payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      309 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/shop_shopify_payment_journal_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/shop_stock_location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/shop_stock_location_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/stock_shipment_shopify_identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_web_shop_shopify-7.2.0/view/stock_shipment_shopify_identifier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    28233 2024-03-25 13:26:54.000000 trytond_web_shop_shopify-7.2.0/web.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4327 2024-04-27 16:30:39.000000 trytond_web_shop_shopify-7.2.0/web.xml
```

### Comparing `trytond_web_shop_shopify-7.0.2/CHANGELOG` & `trytond_web_shop_shopify-7.2.0/CHANGELOG`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 
-Version 7.0.2 - 2024-02-03
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-
-Version 7.0.1 - 2023-12-01
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_web_shop_shopify-7.0.2/COPYRIGHT` & `trytond_web_shop_shopify-7.2.0/COPYRIGHT`

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

### Comparing `trytond_web_shop_shopify-7.0.2/LICENSE` & `trytond_web_shop_shopify-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/PKG-INFO` & `trytond_web_shop_shopify-7.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop_shopify
-Version: 7.0.2
+Version: 7.2.0
 Summary: Module to integrate Tryton with Shopify
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-web-shop-shopify
+Project-URL: Documentation, https://docs.tryton.org/modules-web-shop-shopify
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: web shopify ecommerce
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -51,34 +51,34 @@
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: ShopifyAPI
 Requires-Dist: pyactiveresource
 Requires-Dist: python-sql
 Requires-Dist: python-dateutil
-Requires-Dist: trytond_account_payment<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_product_attribute<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_sale_amendment<7.1,>=7.0
-Requires-Dist: trytond_sale_payment<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_web_shop<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_payment<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_product_attribute<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_sale_amendment<7.3,>=7.2
+Requires-Dist: trytond_sale_payment<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_web_shop<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_payment_clearing<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_customs<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product_measurements<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product_image<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_discount<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_secondary_unit<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_payment_clearing<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_customs<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product_measurements<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product_image<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_discount<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_secondary_unit<7.3,>=7.2; extra == "test"
 
 #######################
 Web Shop Shopify Module
 #######################
 
 The *Web Shop Shopify Module* provides a way to manage `Shopify
 <https://www.shopify.com/>`_ stores.
```

### Comparing `trytond_web_shop_shopify-7.0.2/__init__.py` & `trytond_web_shop_shopify-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/account.py` & `trytond_web_shop_shopify-7.2.0/account.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/common.py` & `trytond_web_shop_shopify-7.2.0/common.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/doc/conf.py` & `trytond_web_shop_shopify-7.2.0/doc/conf.py`

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

### Comparing `trytond_web_shop_shopify-7.0.2/doc/design.rst` & `trytond_web_shop_shopify-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/doc/usage.rst` & `trytond_web_shop_shopify-7.2.0/doc/usage.rst`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 .. _Configure Shopify Web Shop:
 
 Configure Shopify Web Shop
 ==========================
 
 First you must create a new `custom app
-<https://help.shopify.com/en/manual/apps/app-types#custom-apps>`_ for your
-Shopify store with, as a minimum, the following permissions:
+<https://help.shopify.com/en/manual/apps/app-types>`_ for your Shopify store
+with, as a minimum, the following permissions:
 
    * Fulfillment services: Read and write
 
    * Inventory: Read and write
 
    * Orders: Read and write
```

### Comparing `trytond_web_shop_shopify-7.0.2/ir.py` & `trytond_web_shop_shopify-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/ir.xml` & `trytond_web_shop_shopify-7.2.0/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/bg.po` & `trytond_web_shop_shopify-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/ca.po` & `trytond_web_shop_shopify-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/cs.po` & `trytond_web_shop_shopify-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/de.po` & `trytond_web_shop_shopify-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/es.po` & `trytond_web_shop_shopify-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/es_419.po` & `trytond_web_shop_shopify-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/et.po` & `trytond_web_shop_shopify-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/fa.po` & `trytond_web_shop_shopify-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/fi.po` & `trytond_web_shop_shopify-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/fr.po` & `trytond_web_shop_shopify-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/hu.po` & `trytond_web_shop_shopify-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/id.po` & `trytond_web_shop_shopify-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/it.po` & `trytond_web_shop_shopify-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/lo.po` & `trytond_web_shop_shopify-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/lt.po` & `trytond_web_shop_shopify-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/nl.po` & `trytond_web_shop_shopify-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/pl.po` & `trytond_web_shop_shopify-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/pt.po` & `trytond_web_shop_shopify-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/ro.po` & `trytond_web_shop_shopify-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/ru.po` & `trytond_web_shop_shopify-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/sl.po` & `trytond_web_shop_shopify-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/tr.po` & `trytond_web_shop_shopify-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/uk.po` & `trytond_web_shop_shopify-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/locale/zh_CN.po` & `trytond_web_shop_shopify-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/message.xml` & `trytond_web_shop_shopify-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/party.py` & `trytond_web_shop_shopify-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/product.py` & `trytond_web_shop_shopify-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/product.xml` & `trytond_web_shop_shopify-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/routes.py` & `trytond_web_shop_shopify-7.2.0/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/sale.py` & `trytond_web_shop_shopify-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/setup.py` & `trytond_web_shop_shopify-7.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": (
-            'https://docs.tryton.org/projects/modules-web-shop-shopify'),
+            'https://docs.tryton.org/modules-web-shop-shopify'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='web shopify ecommerce',
     package_dir={'trytond.modules.web_shop_shopify': '.'},
     packages=(
         ['trytond.modules.web_shop_shopify']
```

### Comparing `trytond_web_shop_shopify-7.0.2/shopify_retry.py` & `trytond_web_shop_shopify-7.2.0/shopify_retry.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/stock.py` & `trytond_web_shop_shopify-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/stock.xml` & `trytond_web_shop_shopify-7.2.0/stock.xml`

 * *Files 6% similar despite different names*

#### Comparing `trytond_web_shop_shopify-7.0.2/stock.xml` & `trytond_web_shop_shopify-7.2.0/stock.xml`

```diff
@@ -25,22 +25,22 @@
     <record model="ir.action.act_window.view" id="act_stock_shipment_shopify_identifier_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="stock_shipment_shopify_identifier_view_form"/>
       <field name="act_window" ref="act_stock_shipment_shopify_identifier_form"/>
     </record>
     <menuitem parent="menu_shop_shopify_identifier_form" action="act_stock_shipment_shopify_identifier_form" sequence="50" id="menu_stock_shipment_shopify_identifier_form"/>
     <record model="ir.model.access" id="access_stock_shipment_shopify_identifier">
-      <field name="model" search="[('model', '=', 'stock.shipment.shopify_identifier')]"/>
+      <field name="model">stock.shipment.shopify_identifier</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_stock_shipment_shopify_identifier_admin">
-      <field name="model" search="[('model', '=', 'stock.shipment.shopify_identifier')]"/>
+      <field name="model">stock.shipment.shopify_identifier</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_web_shop_shopify-7.0.2/tests/scenario_web_shop_shopify.rst` & `trytond_web_shop_shopify-7.2.0/tests/scenario_web_shop_shopify.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 =========================
 Web Shop Shopify Scenario
 =========================
 
 Imports::
 
-    >>> import datetime as dt
     >>> import os
     >>> import random
     >>> import string
     >>> import time
     >>> import urllib.request
     >>> from decimal import Decimal
 
     >>> import shopify
     >>> from shopify.api_version import ApiVersion
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from proteus import Model
     >>> from trytond.modules.account.tests.tools import (
-    ...     create_fiscalyear, create_chart, get_accounts, create_tax)
+    ...     create_chart, create_fiscalyear, create_tax, get_accounts)
     >>> from trytond.modules.account_invoice.tests.tools import (
     ...     set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.modules.web_shop_shopify.product import Template
+    >>> from trytond.modules.web_shop_shopify.web import Shop
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> FETCH_SLEEP, MAX_SLEEP = 1, 10
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'web_shop_shopify',
@@ -58,25 +58,23 @@
     >>> ShopifyIdentifier = Model.get('web.shop.shopify_identifier')
     >>> Tariff = Model.get('customs.tariff.code')
     >>> Uom = Model.get('product.uom')
     >>> WebShop = Model.get('web.shop')
 
 Set metafields to product::
 
-    >>> from trytond.modules.web_shop_shopify.product import Template
     >>> def get_shopify_metafields(self, shop):
     ...     return {
     ...         'global.test': {
     ...             'value': self.name,
     ...             },
     ...         }
 
     >>> Template.get_shopify_metafields = get_shopify_metafields
 
-    >>> from trytond.modules.web_shop_shopify.web import Shop
     >>> def managed_metafields(self):
     ...     return {'global.test'}
 
     >>> Shop.managed_metafields = managed_metafields
 
 Create country::
 
@@ -507,16 +505,15 @@
     >>> len(sale.payments)
     1
     >>> payment, = sale.payments
     >>> payment.state
     'processing'
     >>> payment.amount
     Decimal('258.98')
-    >>> sale.carrier == carrier
-    True
+    >>> assertEqual(sale.carrier, carrier)
     >>> sale.state
     'quotation'
 
 Capture full amount::
 
     >>> transaction = order.capture('258.98')
     >>> test_transaction_id = transaction.parent_id
@@ -541,15 +538,15 @@
 Make a partial shipment::
 
     >>> shipment, = sale.shipments
     >>> move, = [m for m in shipment.inventory_moves if m.product == variant1]
     >>> move.quantity = 3
     >>> shipment.click('pick')
     >>> shipment.click('pack')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
 
     >>> sale.reload()
     >>> len(sale.invoices)
     0
 
@@ -605,16 +602,15 @@
     'succeeded'
 
 Correct taxes as partial invoice can get rounding gap::
 
     >>> tax_line, = invoice.taxes
     >>> tax_line.amount += payment.amount - invoice.total_amount
     >>> invoice.save()
-    >>> invoice.total_amount == payment.amount
-    True
+    >>> assertEqual(invoice.total_amount, payment.amount)
 
 Post invoice::
 
     >>> invoice.click('post')
     >>> invoice.state
     'paid'
     >>> sale.reload()
```

### Comparing `trytond_web_shop_shopify-7.0.2/tests/scenario_web_shop_shopify_secondary_unit.rst` & `trytond_web_shop_shopify-7.2.0/tests/scenario_web_shop_shopify_secondary_unit.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 ========================================
 Web Shop Shopify Secondary Unit Scenario
 ========================================
 
 Imports::
 
-    >>> import datetime as dt
     >>> import os
     >>> import random
     >>> import string
     >>> import time
-    >>> import urllib.request
     >>> from decimal import Decimal
 
     >>> import shopify
     >>> from shopify.api_version import ApiVersion
 
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
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> FETCH_SLEEP, MAX_SLEEP = 1, 10
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'web_shop_shopify',
@@ -202,22 +199,20 @@
     >>> len(sale.lines)
     2
     >>> sale.total_amount
     Decimal('202.00')
     >>> line, = [l for l in sale.lines if l.product]
     >>> line.quantity
     2.0
-    >>> line.unit == unit
-    True
+    >>> assertEqual(line.unit, unit)
     >>> line.unit_price
     Decimal('100.0000')
     >>> line.secondary_quantity
     50.0
-    >>> line.secondary_unit == cm
-    True
+    >>> assertEqual(line.secondary_unit, cm)
     >>> line.secondary_unit_price
     Decimal('4.0000')
 
 Clean up::
 
     >>> order.destroy()
     >>> for product in ShopifyIdentifier.find(
```

### Comparing `trytond_web_shop_shopify-7.0.2/tox.ini` & `trytond_web_shop_shopify-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/trytond_web_shop_shopify.egg-info/PKG-INFO` & `trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop_shopify
-Version: 7.0.2
+Version: 7.2.0
 Summary: Module to integrate Tryton with Shopify
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-web-shop-shopify
+Project-URL: Documentation, https://docs.tryton.org/modules-web-shop-shopify
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: web shopify ecommerce
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -51,34 +51,34 @@
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: ShopifyAPI
 Requires-Dist: pyactiveresource
 Requires-Dist: python-sql
 Requires-Dist: python-dateutil
-Requires-Dist: trytond_account_payment<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_product_attribute<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_sale_amendment<7.1,>=7.0
-Requires-Dist: trytond_sale_payment<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_web_shop<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account_payment<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_product_attribute<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_sale_amendment<7.3,>=7.2
+Requires-Dist: trytond_sale_payment<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_web_shop<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_account_payment_clearing<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_customs<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product_measurements<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product_image<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_discount<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_secondary_unit<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_account_payment_clearing<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_customs<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product_measurements<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product_image<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_discount<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_secondary_unit<7.3,>=7.2; extra == "test"
 
 #######################
 Web Shop Shopify Module
 #######################
 
 The *Web Shop Shopify Module* provides a way to manage `Shopify
 <https://www.shopify.com/>`_ stores.
```

### Comparing `trytond_web_shop_shopify-7.0.2/trytond_web_shop_shopify.egg-info/SOURCES.txt` & `trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/SOURCES.txt`

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
 account.py
```

### Comparing `trytond_web_shop_shopify-7.0.2/trytond_web_shop_shopify.egg-info/requires.txt` & `trytond_web_shop_shopify-7.2.0/trytond_web_shop_shopify.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ShopifyAPI
 pyactiveresource
 python-sql
 python-dateutil
-trytond_account_payment<7.1,>=7.0
-trytond_currency<7.1,>=7.0
-trytond_party<7.1,>=7.0
-trytond_product<7.1,>=7.0
-trytond_product_attribute<7.1,>=7.0
-trytond_sale<7.1,>=7.0
-trytond_sale_amendment<7.1,>=7.0
-trytond_sale_payment<7.1,>=7.0
-trytond_stock<7.1,>=7.0
-trytond_web_shop<7.1,>=7.0
-trytond<7.1,>=7.0
+trytond_account_payment<7.3,>=7.2
+trytond_currency<7.3,>=7.2
+trytond_party<7.3,>=7.2
+trytond_product<7.3,>=7.2
+trytond_product_attribute<7.3,>=7.2
+trytond_sale<7.3,>=7.2
+trytond_sale_amendment<7.3,>=7.2
+trytond_sale_payment<7.3,>=7.2
+trytond_stock<7.3,>=7.2
+trytond_web_shop<7.3,>=7.2
+trytond<7.3,>=7.2
 
 [test]
-proteus<7.1,>=7.0
-trytond_account_payment_clearing<7.1,>=7.0
-trytond_customs<7.1,>=7.0
-trytond_product_measurements<7.1,>=7.0
-trytond_product_image<7.1,>=7.0
-trytond_sale_discount<7.1,>=7.0
-trytond_sale_shipment_cost<7.1,>=7.0
-trytond_sale_secondary_unit<7.1,>=7.0
+proteus<7.3,>=7.2
+trytond_account_payment_clearing<7.3,>=7.2
+trytond_customs<7.3,>=7.2
+trytond_product_measurements<7.3,>=7.2
+trytond_product_image<7.3,>=7.2
+trytond_sale_discount<7.3,>=7.2
+trytond_sale_shipment_cost<7.3,>=7.2
+trytond_sale_secondary_unit<7.3,>=7.2
```

### Comparing `trytond_web_shop_shopify-7.0.2/view/shop_form.xml` & `trytond_web_shop_shopify-7.2.0/view/shop_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/web.py` & `trytond_web_shop_shopify-7.2.0/web.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_shopify-7.0.2/web.xml` & `trytond_web_shop_shopify-7.2.0/web.xml`

 * *Files 3% similar despite different names*

#### Comparing `trytond_web_shop_shopify-7.0.2/web.xml` & `trytond_web_shop_shopify-7.2.0/web.xml`

```diff
@@ -42,32 +42,32 @@
     <record model="ir.action.act_window.view" id="act_shop_shopify_identifier_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="shop_shopify_identifier_view_form"/>
       <field name="act_window" ref="act_shop_shopify_identifier_form"/>
     </record>
     <menuitem parent="ir.menu_models" action="act_shop_shopify_identifier_form" sequence="50" id="menu_shop_shopify_identifier_form"/>
     <record model="ir.model.access" id="access_shop_shopify_identifier">
-      <field name="model" search="[('model', '=', 'web.shop.shopify_identifier')]"/>
+      <field name="model">web.shop.shopify_identifier</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_shop_shopify_identifier_admin">
-      <field name="model" search="[('model', '=', 'web.shop.shopify_identifier')]"/>
+      <field name="model">web.shop.shopify_identifier</field>
       <field name="group" ref="res.group_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="shop_shopify_identifier_set_to_update_button">
+      <field name="model">web.shop.shopify_identifier</field>
       <field name="name">set_to_update</field>
       <field name="string">Set to Update</field>
-      <field name="model" search="[('model', '=', 'web.shop.shopify_identifier')]"/>
     </record>
     <record model="ir.ui.view" id="shop_shopify_payment_journal_view_form">
       <field name="model">web.shop.shopify_payment_journal</field>
       <field name="type">form</field>
       <field name="name">shop_shopify_payment_journal_form</field>
     </record>
     <record model="ir.ui.view" id="shop_shopify_payment_journal_view_list">
```

