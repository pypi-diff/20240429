# Comparing `tmp/trytond_sale_subscription-7.0.1.tar.gz` & `tmp/trytond_sale_subscription-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_subscription-7.0.1.tar", last modified: Sat Feb  3 11:17:29 2024, max compression
+gzip compressed data, was "trytond_sale_subscription-7.2.0.tar", last modified: Mon Apr 29 15:49:59 2024, max compression
```

## Comparing `trytond_sale_subscription-7.0.1.tar` & `trytond_sale_subscription-7.2.0.tar`

### file list

```diff
@@ -1,97 +1,96 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:17:29.630070 trytond_sale_subscription-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2039 2024-02-03 11:17:21.000000 trytond_sale_subscription-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      686 2024-02-03 11:17:21.000000 trytond_sale_subscription-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     6227 2024-02-03 11:17:29.630070 trytond_sale_subscription-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3531 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1238 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1841 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:17:29.613395 trytond_sale_subscription-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2818 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3531 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:17:29.613395 trytond_sale_subscription-7.0.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/icons/tryton-sale-subscription.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      737 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:17:29.620065 trytond_sale_subscription-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18247 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18369 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18386 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14786 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16241 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    19172 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18505 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15286 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16546 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16524 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    18167 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16783 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17696 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14978 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17598 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14786 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16263 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1771 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1205 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9249 2024-01-26 17:58:33.000000 trytond_sale_subscription-7.0.1/recurrence.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4545 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/recurrence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1014 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/service.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2462 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/service.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-02-03 11:17:29.630070 trytond_sale_subscription-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4488 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    37614 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/subscription.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14252 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/subscription.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:17:29.620065 trytond_sale_subscription-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5558 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/tests/scenario_sale_subscription.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5381 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/tests/scenario_sale_subscription_advanced_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4727 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/tests/scenario_sale_subscription_new_line.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      254 2023-10-30 17:55:12.000000 trytond_sale_subscription-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:17:29.626735 trytond_sale_subscription-7.0.1/trytond_sale_subscription.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     6227 2024-02-03 11:17:28.000000 trytond_sale_subscription-7.0.1/trytond_sale_subscription.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3500 2024-02-03 11:17:29.000000 trytond_sale_subscription-7.0.1/trytond_sale_subscription.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-02-03 11:17:28.000000 trytond_sale_subscription-7.0.1/trytond_sale_subscription.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-02-03 11:17:28.000000 trytond_sale_subscription-7.0.1/trytond_sale_subscription.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:11.000000 trytond_sale_subscription-7.0.1/trytond_sale_subscription.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-02-03 11:17:28.000000 trytond_sale_subscription-7.0.1/trytond_sale_subscription.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-02-03 11:17:28.000000 trytond_sale_subscription-7.0.1/trytond_sale_subscription.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-03 11:17:29.626735 trytond_sale_subscription-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/create_invoice_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/line_consumption_create_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      961 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/recurrence_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/recurrence_rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/recurrence_rule_set_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/recurrence_rule_set_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/recurrence_rule_set_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/recurrence_rule_set_test_result_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/service_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/service_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2120 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/subscription_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/subscription_line_consumption_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/subscription_line_consumption_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1246 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/subscription_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      527 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/subscription_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/subscription_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-10-30 17:06:38.000000 trytond_sale_subscription-7.0.1/view/subscription_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:59.174444 trytond_sale_subscription-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2039 2024-04-29 15:26:53.000000 trytond_sale_subscription-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      686 2024-04-29 15:26:53.000000 trytond_sale_subscription-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_subscription-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     6227 2024-04-29 15:49:59.174444 trytond_sale_subscription-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3531 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1238 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1841 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:59.171110 trytond_sale_subscription-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-27 16:30:39.000000 trytond_sale_subscription-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3531 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:30.000000 trytond_sale_subscription-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:59.171110 trytond_sale_subscription-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/icons/tryton-sale-subscription.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      737 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      602 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:59.171110 trytond_sale_subscription-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18247 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18369 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18386 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14786 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16241 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    19172 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18505 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15286 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16546 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16524 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    18167 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16783 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17696 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14978 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17598 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14786 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16263 2024-04-27 16:43:27.000000 trytond_sale_subscription-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1771 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1205 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9249 2024-04-22 12:14:36.000000 trytond_sale_subscription-7.2.0/recurrence.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4499 2024-04-27 16:30:39.000000 trytond_sale_subscription-7.2.0/recurrence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1014 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/service.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2384 2024-04-27 16:30:39.000000 trytond_sale_subscription-7.2.0/service.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:49:59.174444 trytond_sale_subscription-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4488 2024-03-17 11:01:36.000000 trytond_sale_subscription-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    37697 2024-04-22 12:14:36.000000 trytond_sale_subscription-7.2.0/subscription.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14027 2024-04-27 16:30:39.000000 trytond_sale_subscription-7.2.0/subscription.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:59.174444 trytond_sale_subscription-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5489 2024-04-22 12:14:36.000000 trytond_sale_subscription-7.2.0/tests/scenario_sale_subscription.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5298 2024-04-22 12:14:36.000000 trytond_sale_subscription-7.2.0/tests/scenario_sale_subscription_advanced_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4643 2024-04-22 12:14:36.000000 trytond_sale_subscription-7.2.0/tests/scenario_sale_subscription_new_line.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:30.000000 trytond_sale_subscription-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      254 2024-04-29 15:26:49.000000 trytond_sale_subscription-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:59.174444 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6227 2024-04-29 15:49:58.000000 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3482 2024-04-29 15:49:59.000000 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:49:58.000000 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-29 15:49:58.000000 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-29 15:49:58.000000 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:49:58.000000 trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:59.174444 trytond_sale_subscription-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-01-16 14:00:21.000000 trytond_sale_subscription-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      419 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/create_invoice_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/line_consumption_create_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      961 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/recurrence_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/recurrence_rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-01-16 14:00:21.000000 trytond_sale_subscription-7.2.0/view/recurrence_rule_set_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-01-16 14:00:21.000000 trytond_sale_subscription-7.2.0/view/recurrence_rule_set_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/recurrence_rule_set_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/recurrence_rule_set_test_result_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      458 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/service_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/service_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2120 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/subscription_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      410 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/subscription_line_consumption_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/subscription_line_consumption_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1246 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/subscription_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      527 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/subscription_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/subscription_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2023-04-15 07:12:15.000000 trytond_sale_subscription-7.2.0/view/subscription_list.xml
```

### Comparing `trytond_sale_subscription-7.0.1/CHANGELOG` & `trytond_sale_subscription-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_sale_subscription-7.0.1/COPYRIGHT` & `trytond_sale_subscription-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/LICENSE` & `trytond_sale_subscription-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/PKG-INFO` & `trytond_sale_subscription-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_subscription
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for subscription
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
@@ -49,23 +49,23 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-dateutil
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Subscription Module
 ########################
 
 The sale subscription module defines subscription, services and recurrence rule
 models.
```

### Comparing `trytond_sale_subscription-7.0.1/README.rst` & `trytond_sale_subscription-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/__init__.py` & `trytond_sale_subscription-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/configuration.py` & `trytond_sale_subscription-7.2.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/configuration.xml` & `trytond_sale_subscription-7.2.0/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/doc/conf.py` & `trytond_sale_subscription-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_subscription-7.0.1/doc/index.rst` & `trytond_sale_subscription-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/icons/LICENSE` & `trytond_sale_subscription-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/invoice.py` & `trytond_sale_subscription-7.2.0/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/ir.py` & `trytond_sale_subscription-7.2.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/bg.po` & `trytond_sale_subscription-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/ca.po` & `trytond_sale_subscription-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/cs.po` & `trytond_sale_subscription-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/de.po` & `trytond_sale_subscription-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/es.po` & `trytond_sale_subscription-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/es_419.po` & `trytond_sale_subscription-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/et.po` & `trytond_sale_subscription-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/fa.po` & `trytond_sale_subscription-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/fi.po` & `trytond_sale_subscription-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/fr.po` & `trytond_sale_subscription-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/hu.po` & `trytond_sale_subscription-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/id.po` & `trytond_sale_subscription-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/it.po` & `trytond_sale_subscription-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/lo.po` & `trytond_sale_subscription-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/lt.po` & `trytond_sale_subscription-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/nl.po` & `trytond_sale_subscription-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/pl.po` & `trytond_sale_subscription-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/pt.po` & `trytond_sale_subscription-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/ro.po` & `trytond_sale_subscription-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/ru.po` & `trytond_sale_subscription-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/sl.po` & `trytond_sale_subscription-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/tr.po` & `trytond_sale_subscription-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/uk.po` & `trytond_sale_subscription-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/locale/zh_CN.po` & `trytond_sale_subscription-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/message.xml` & `trytond_sale_subscription-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/party.py` & `trytond_sale_subscription-7.2.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/product.py` & `trytond_sale_subscription-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/recurrence.py` & `trytond_sale_subscription-7.2.0/recurrence.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/recurrence.xml` & `trytond_sale_subscription-7.2.0/recurrence.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_sale_subscription-7.0.1/recurrence.xml` & `trytond_sale_subscription-7.2.0/recurrence.xml`

```diff
@@ -25,22 +25,22 @@
     <record model="ir.action.act_window.view" id="act_recurrence_rule_set_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="recurrence_rule_set_view_form"/>
       <field name="act_window" ref="act_recurrence_rule_set_form"/>
     </record>
     <menuitem parent="menu_configuration" action="act_recurrence_rule_set_form" sequence="10" id="menu_recurrence_rule_set_form"/>
     <record model="ir.model.access" id="access_recurrence_rule_set">
-      <field name="model" search="[('model', '=', 'sale.subscription.recurrence.rule.set')]"/>
+      <field name="model">sale.subscription.recurrence.rule.set</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_recurrence_rule_set_product_admin">
-      <field name="model" search="[('model', '=', 'sale.subscription.recurrence.rule.set')]"/>
+      <field name="model">sale.subscription.recurrence.rule.set</field>
       <field name="group" ref="product.group_product_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.ui.view" id="recurrence_rule_view_form">
```

### Comparing `trytond_sale_subscription-7.0.1/service.py` & `trytond_sale_subscription-7.2.0/service.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/service.xml` & `trytond_sale_subscription-7.2.0/service.xml`

 * *Files 7% similar despite different names*

#### Comparing `trytond_sale_subscription-7.0.1/service.xml` & `trytond_sale_subscription-7.2.0/service.xml`

```diff
@@ -25,22 +25,22 @@
     <record model="ir.action.act_window.view" id="act_service_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="service_view_form"/>
       <field name="act_window" ref="act_service_form"/>
     </record>
     <menuitem parent="product.menu_template" action="act_service_form" sequence="20" id="menu_service_form"/>
     <record model="ir.model.access" id="access_service">
-      <field name="model" search="[('model', '=', 'sale.subscription.service')]"/>
+      <field name="model">sale.subscription.service</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_service_product_admin">
-      <field name="model" search="[('model', '=', 'sale.subscription.service')]"/>
+      <field name="model">sale.subscription.service</field>
       <field name="group" ref="product.group_product_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_sale_subscription-7.0.1/setup.py` & `trytond_sale_subscription-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/subscription.py` & `trytond_sale_subscription-7.2.0/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,17 @@
         cursor.execute(*table.update(
                 [table.state], ['cancelled'],
                 where=table.state == 'canceled'))
 
     @classmethod
     def order_number(cls, tables):
         table, _ = tables[None]
-        return [CharLength(table.number), table.number]
+        return [
+            ~((table.state == 'cancelled') & (table.number == Null)),
+            CharLength(table.number), table.number]
 
     @classmethod
     def default_company(cls):
         return Transaction().context.get('company')
 
     @classmethod
     def default_currency(cls, **pattern):
```

### Comparing `trytond_sale_subscription-7.0.1/subscription.xml` & `trytond_sale_subscription-7.2.0/subscription.xml`

 * *Files 2% similar despite different names*

#### Comparing `trytond_sale_subscription-7.0.1/subscription.xml` & `trytond_sale_subscription-7.2.0/subscription.xml`

```diff
@@ -71,55 +71,55 @@
     </record>
     <record model="ir.action-res.group" id="act_subscription_party_relate-group_sale">
       <field name="action" ref="act_subscription_party_relate"/>
       <field name="group" ref="sale.group_sale"/>
     </record>
     <record model="ir.rule.group" id="rule_group_subscription_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'sale.subscription')]"/>
+      <field name="model">sale.subscription</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_subscription_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_subscription_companies"/>
     </record>
     <record model="ir.model.access" id="access_subscription">
-      <field name="model" search="[('model', '=', 'sale.subscription')]"/>
+      <field name="model">sale.subscription</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_subscription_sale">
-      <field name="model" search="[('model', '=', 'sale.subscription')]"/>
+      <field name="model">sale.subscription</field>
       <field name="group" ref="sale.group_sale"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="subscription_draft_button">
+      <field name="model">sale.subscription</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'sale.subscription')]"/>
     </record>
     <record model="ir.model.button" id="subscription_run_button">
+      <field name="model">sale.subscription</field>
       <field name="name">run</field>
       <field name="string">Run</field>
-      <field name="model" search="[('model', '=', 'sale.subscription')]"/>
     </record>
     <record model="ir.model.button" id="subscription_cancel_button">
+      <field name="model">sale.subscription</field>
       <field name="name">cancel</field>
       <field name="string">Cancel</field>
-      <field name="model" search="[('model', '=', 'sale.subscription')]"/>
     </record>
     <record model="ir.model.button" id="subscription_quote_button">
+      <field name="model">sale.subscription</field>
       <field name="name">quote</field>
       <field name="string">Quote</field>
-      <field name="model" search="[('model', '=', 'sale.subscription')]"/>
     </record>
     <record model="ir.ui.view" id="subscription_line_view_form">
       <field name="model">sale.subscription.line</field>
       <field name="type">form</field>
       <field name="name">subscription_line_form</field>
     </record>
     <record model="ir.ui.view" id="subscription_line_view_list">
```

### Comparing `trytond_sale_subscription-7.0.1/tests/scenario_sale_subscription.rst` & `trytond_sale_subscription-7.2.0/tests/scenario_sale_subscription.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 Sale Subscription Scenario
 ==========================
 
 Imports::
 
     >>> import datetime
     >>> from decimal import Decimal
-    >>> from dateutil.relativedelta import relativedelta
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('sale_subscription')
 
 Create company::
 
@@ -111,16 +109,15 @@
     >>> subscription.party = customer
     >>> subscription.start_date = datetime.date(2016, 1, 1)
     >>> subscription.invoice_start_date = datetime.date(2016, 2, 1)
     >>> subscription.invoice_recurrence = monthly
     >>> line = subscription.lines.new()
     >>> line.service = service
     >>> line.quantity = 10
-    >>> line.start_date == subscription.start_date
-    True
+    >>> assertEqual(line.start_date, subscription.start_date)
 
     >>> subscription.click('quote')
     >>> subscription.state
     'quotation'
     >>> subscription.click('run')
     >>> subscription.state
     'running'
```

### Comparing `trytond_sale_subscription-7.0.1/tests/scenario_sale_subscription_advanced_invoice.rst` & `trytond_sale_subscription-7.2.0/tests/scenario_sale_subscription_advanced_invoice.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 Sale Subscription with Advanced Invoice Scenario
 ================================================
 
 Imports::
 
     >>> import datetime
     >>> from decimal import Decimal
-    >>> from dateutil.relativedelta import relativedelta
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
 
 Activate modules::
 
     >>> config = activate_modules('sale_subscription')
 
 Create company::
 
@@ -171,8 +169,8 @@
     >>> invoice2, = Invoice.find([('id', '!=', invoice.id)])
     >>> line, = invoice2.lines
     >>> line.quantity
     10.0
 
     >>> subscription.reload()
     >>> subscription.next_invoice_date
-    datetime.date(2016, 3, 31)
+    datetime.date(2016, 3, 31)
```

### Comparing `trytond_sale_subscription-7.0.1/tests/scenario_sale_subscription_new_line.rst` & `trytond_sale_subscription-7.2.0/tests/scenario_sale_subscription_new_line.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 Sale Subscription New Line Scenario
 ===================================
 
 Imports::
 
     >>> import datetime
     >>> from decimal import Decimal
-    >>> from dateutil.relativedelta import relativedelta
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
 
 Activate modules::
 
     >>> config = activate_modules('sale_subscription')
 
 Create company::
```

### Comparing `trytond_sale_subscription-7.0.1/tox.ini` & `trytond_sale_subscription-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/trytond_sale_subscription.egg-info/PKG-INFO` & `trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_subscription
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for subscription
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
@@ -49,23 +49,23 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-dateutil
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Subscription Module
 ########################
 
 The sale subscription module defines subscription, services and recurrence rule
 models.
```

### Comparing `trytond_sale_subscription-7.0.1/trytond_sale_subscription.egg-info/SOURCES.txt` & `trytond_sale_subscription-7.2.0/trytond_sale_subscription.egg-info/SOURCES.txt`

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
 configuration.py
```

### Comparing `trytond_sale_subscription-7.0.1/view/recurrence_rule_form.xml` & `trytond_sale_subscription-7.2.0/view/recurrence_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/view/recurrence_rule_list.xml` & `trytond_sale_subscription-7.2.0/view/recurrence_rule_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/view/subscription_form.xml` & `trytond_sale_subscription-7.2.0/view/subscription_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/view/subscription_line_form.xml` & `trytond_sale_subscription-7.2.0/view/subscription_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/view/subscription_line_list.xml` & `trytond_sale_subscription-7.2.0/view/subscription_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/view/subscription_line_list_sequence.xml` & `trytond_sale_subscription-7.2.0/view/subscription_line_list_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription-7.0.1/view/subscription_list.xml` & `trytond_sale_subscription-7.2.0/view/subscription_list.xml`

 * *Files identical despite different names*

