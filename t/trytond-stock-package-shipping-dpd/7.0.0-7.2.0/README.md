# Comparing `tmp/trytond_stock_package_shipping_dpd-7.0.0.tar.gz` & `tmp/trytond_stock_package_shipping_dpd-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_package_shipping_dpd-7.0.0.tar", last modified: Mon Oct 30 17:42:39 2023, max compression
+gzip compressed data, was "trytond_stock_package_shipping_dpd-7.2.0.tar", last modified: Mon Apr 29 15:51:59 2024, max compression
```

## Comparing `trytond_stock_package_shipping_dpd-7.0.0.tar` & `trytond_stock_package_shipping_dpd-7.2.0.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:39.949104 trytond_stock_package_shipping_dpd-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      233 2023-10-22 17:23:25.000000 trytond_stock_package_shipping_dpd-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1509 2023-10-30 17:14:49.000000 trytond_stock_package_shipping_dpd-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      684 2023-10-30 17:14:48.000000 trytond_stock_package_shipping_dpd-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_package_shipping_dpd-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3904 2023-10-30 17:42:39.949104 trytond_stock_package_shipping_dpd-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1094 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      583 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4192 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.0.0/carrier.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2827 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.0.0/carrier.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1107 2023-08-13 15:26:13.000000 trytond_stock_package_shipping_dpd-7.0.0/configuration.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:39.945770 trytond_stock_package_shipping_dpd-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2827 2023-10-22 17:23:25.000000 trytond_stock_package_shipping_dpd-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1094 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:25.000000 trytond_stock_package_shipping_dpd-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:39.942437 trytond_stock_package_shipping_dpd-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2746 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3220 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2567 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3223 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3249 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2490 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2623 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3229 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2567 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3281 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2638 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2543 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2591 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2700 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2591 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3138 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2664 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2814 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2489 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2700 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2799 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2567 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2481 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2582 2023-10-30 16:47:45.000000 trytond_stock_package_shipping_dpd-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1061 2023-10-27 17:38:49.000000 trytond_stock_package_shipping_dpd-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:42:39.949104 trytond_stock_package_shipping_dpd-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4602 2023-10-27 17:38:49.000000 trytond_stock_package_shipping_dpd-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11605 2023-10-27 17:38:49.000000 trytond_stock_package_shipping_dpd-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      459 2023-01-16 14:00:21.000000 trytond_stock_package_shipping_dpd-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:39.942437 trytond_stock_package_shipping_dpd-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7393 2023-10-27 17:38:49.000000 trytond_stock_package_shipping_dpd-7.0.0/tests/scenario_shipping_dpd.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_stock_package_shipping_dpd-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      207 2023-10-30 17:14:44.000000 trytond_stock_package_shipping_dpd-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:39.945770 trytond_stock_package_shipping_dpd-7.0.0/trytond_stock_package_shipping_dpd.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3904 2023-10-30 17:42:39.000000 trytond_stock_package_shipping_dpd-7.0.0/trytond_stock_package_shipping_dpd.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1825 2023-10-30 17:42:39.000000 trytond_stock_package_shipping_dpd-7.0.0/trytond_stock_package_shipping_dpd.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:42:39.000000 trytond_stock_package_shipping_dpd-7.0.0/trytond_stock_package_shipping_dpd.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-10-30 17:42:39.000000 trytond_stock_package_shipping_dpd-7.0.0/trytond_stock_package_shipping_dpd.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_stock_package_shipping_dpd-7.0.0/trytond_stock_package_shipping_dpd.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-10-30 17:42:39.000000 trytond_stock_package_shipping_dpd-7.0.0/trytond_stock_package_shipping_dpd.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:42:39.000000 trytond_stock_package_shipping_dpd-7.0.0/trytond_stock_package_shipping_dpd.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:39.942437 trytond_stock_package_shipping_dpd-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      655 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.0.0/view/carrier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.0.0/view/dpd_credential_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.0.0/view/dpd_credential_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:59.894620 trytond_stock_package_shipping_dpd-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1610 2024-04-29 15:28:20.000000 trytond_stock_package_shipping_dpd-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      684 2024-04-29 15:28:20.000000 trytond_stock_package_shipping_dpd-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_package_shipping_dpd-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3904 2024-04-29 15:51:59.894620 trytond_stock_package_shipping_dpd-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1094 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      583 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4192 2024-03-25 13:26:54.000000 trytond_stock_package_shipping_dpd-7.2.0/carrier.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2749 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_dpd-7.2.0/carrier.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1107 2024-01-27 09:58:52.000000 trytond_stock_package_shipping_dpd-7.2.0/configuration.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:59.887953 trytond_stock_package_shipping_dpd-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-27 16:30:39.000000 trytond_stock_package_shipping_dpd-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1094 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:34.000000 trytond_stock_package_shipping_dpd-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-03-25 13:26:54.000000 trytond_stock_package_shipping_dpd-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:59.891286 trytond_stock_package_shipping_dpd-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2746 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3220 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2567 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3223 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3249 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2490 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2623 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3229 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2567 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3281 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2638 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2543 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2591 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2700 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2591 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3138 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2664 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2814 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2489 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2700 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2799 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2567 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2481 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2582 2024-04-27 16:43:27.000000 trytond_stock_package_shipping_dpd-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1061 2024-03-25 13:26:54.000000 trytond_stock_package_shipping_dpd-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:51:59.894620 trytond_stock_package_shipping_dpd-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4602 2024-03-17 11:01:36.000000 trytond_stock_package_shipping_dpd-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11605 2024-02-04 18:51:26.000000 trytond_stock_package_shipping_dpd-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      459 2023-01-16 14:00:21.000000 trytond_stock_package_shipping_dpd-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:59.891286 trytond_stock_package_shipping_dpd-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7300 2024-04-22 12:14:37.000000 trytond_stock_package_shipping_dpd-7.2.0/tests/scenario_shipping_dpd.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:34.000000 trytond_stock_package_shipping_dpd-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      207 2024-04-29 15:28:15.000000 trytond_stock_package_shipping_dpd-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:59.891286 trytond_stock_package_shipping_dpd-7.2.0/trytond_stock_package_shipping_dpd.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3904 2024-04-29 15:51:59.000000 trytond_stock_package_shipping_dpd-7.2.0/trytond_stock_package_shipping_dpd.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1807 2024-04-29 15:51:59.000000 trytond_stock_package_shipping_dpd-7.2.0/trytond_stock_package_shipping_dpd.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:51:59.000000 trytond_stock_package_shipping_dpd-7.2.0/trytond_stock_package_shipping_dpd.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-29 15:51:59.000000 trytond_stock_package_shipping_dpd-7.2.0/trytond_stock_package_shipping_dpd.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_stock_package_shipping_dpd-7.2.0/trytond_stock_package_shipping_dpd.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      322 2024-04-29 15:51:59.000000 trytond_stock_package_shipping_dpd-7.2.0/trytond_stock_package_shipping_dpd.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:51:59.000000 trytond_stock_package_shipping_dpd-7.2.0/trytond_stock_package_shipping_dpd.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:59.891286 trytond_stock_package_shipping_dpd-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      655 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.2.0/view/carrier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.2.0/view/dpd_credential_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      311 2023-04-15 07:12:15.000000 trytond_stock_package_shipping_dpd-7.2.0/view/dpd_credential_list.xml
```

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/CHANGELOG` & `trytond_stock_package_shipping_dpd-7.2.0/CHANGELOG`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/COPYRIGHT` & `trytond_stock_package_shipping_dpd-7.2.0/COPYRIGHT`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2016-2023 B2CK.
+Copyright (C) 2016-2024 B2CK.
 Copyright (C) 2016-2023 Nicolas Évrard.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/LICENSE` & `trytond_stock_package_shipping_dpd-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/PKG-INFO` & `trytond_stock_package_shipping_dpd-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_package_shipping_dpd
-Version: 7.0.0
+Version: 7.2.0
 Summary: DPD connector for the Tryton application platform
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
@@ -49,25 +49,25 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: zeep>=0.12
 Requires-Dist: pypdf>=3
 Requires-Dist: lxml
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_measurements<7.1,>=7.0
-Requires-Dist: trytond_stock_package<7.1,>=7.0
-Requires-Dist: trytond_stock_package_shipping<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_measurements<7.3,>=7.2
+Requires-Dist: trytond_stock_package<7.3,>=7.2
+Requires-Dist: trytond_stock_package_shipping<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
 
 Stock Package Shipping DPD Module
 #################################
 
 The Stock Package Shipping DPD module allows you to generate the DPD label
 using the DPD webservices.
 DPD has many different web services, the module supports:
```

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/README.rst` & `trytond_stock_package_shipping_dpd-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/__init__.py` & `trytond_stock_package_shipping_dpd-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/carrier.py` & `trytond_stock_package_shipping_dpd-7.2.0/carrier.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/carrier.xml` & `trytond_stock_package_shipping_dpd-7.2.0/carrier.xml`

 * *Files 9% similar despite different names*

#### Comparing `trytond_stock_package_shipping_dpd-7.0.0/carrier.xml` & `trytond_stock_package_shipping_dpd-7.2.0/carrier.xml`

```diff
@@ -30,22 +30,22 @@
     <record model="ir.action.act_window.view" id="act_dpd_credential_form_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="credential_view_form"/>
       <field name="act_window" ref="act_dpd_credential_form"/>
     </record>
     <menuitem parent="carrier.menu_configuration" action="act_dpd_credential_form" sequence="50" id="menu_dpd_credential_form"/>
     <record model="ir.model.access" id="access_carrier_credential">
-      <field name="model" search="[('model', '=', 'carrier.credential.dpd')]"/>
+      <field name="model">carrier.credential.dpd</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_carrier_credential_carrier_admin">
-      <field name="model" search="[('model', '=', 'carrier.credential.dpd')]"/>
+      <field name="model">carrier.credential.dpd</field>
       <field name="group" ref="carrier.group_carrier_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
```

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/configuration.py` & `trytond_stock_package_shipping_dpd-7.2.0/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/doc/conf.py` & `trytond_stock_package_shipping_dpd-7.2.0/doc/conf.py`

 * *Files 9% similar despite different names*

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

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/doc/index.rst` & `trytond_stock_package_shipping_dpd-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/bg.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/ca.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/cs.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/de.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/es.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/es_419.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/et.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/fa.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/fi.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/fr.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/hu.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/id.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/it.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/lo.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/lt.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/nl.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/pl.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/pt.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/ro.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/ru.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/sl.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/tr.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/uk.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/locale/zh_CN.po` & `trytond_stock_package_shipping_dpd-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/message.xml` & `trytond_stock_package_shipping_dpd-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/setup.py` & `trytond_stock_package_shipping_dpd-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/stock.py` & `trytond_stock_package_shipping_dpd-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/tests/scenario_shipping_dpd.rst` & `trytond_stock_package_shipping_dpd-7.2.0/tests/scenario_shipping_dpd.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 Stock Package Shipping with DPD scenario
 ========================================
 
 Imports::
 
     >>> import os
     >>> from decimal import Decimal
-    >>> from operator import attrgetter
-    >>> from proteus import Model, Wizard, Report
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts, create_tax
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
 
 Activate modules::
 
     >>> config = activate_modules(
     ...     ['stock_package_shipping_dpd', 'sale', 'sale_shipment_cost'])
 
 Create company::
@@ -217,11 +216,11 @@
     >>> pack, = shipment.root_packages
     >>> pack.shipping_label is not None
     True
     >>> pack.shipping_label_mimetype
     'application/pdf'
     >>> pack.shipping_reference is not None
     True
-    >>> pack.shipping_tracking_url.startswith('https://tracking.dpd.de/status/')
-    True
+    >>> pack.shipping_tracking_url
+    'https://tracking.dpd.de/status/...'
     >>> pack.shipping_tracking_url.endswith(pack.shipping_reference)
     True
```

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/tox.ini` & `trytond_stock_package_shipping_dpd-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/trytond_stock_package_shipping_dpd.egg-info/PKG-INFO` & `trytond_stock_package_shipping_dpd-7.2.0/trytond_stock_package_shipping_dpd.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-stock-package-shipping-dpd
-Version: 7.0.0
+Name: trytond_stock_package_shipping_dpd
+Version: 7.2.0
 Summary: DPD connector for the Tryton application platform
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
@@ -49,25 +49,25 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: zeep>=0.12
 Requires-Dist: pypdf>=3
 Requires-Dist: lxml
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_shipment_measurements<7.1,>=7.0
-Requires-Dist: trytond_stock_package<7.1,>=7.0
-Requires-Dist: trytond_stock_package_shipping<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_shipment_measurements<7.3,>=7.2
+Requires-Dist: trytond_stock_package<7.3,>=7.2
+Requires-Dist: trytond_stock_package_shipping<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_shipment_cost<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
 
 Stock Package Shipping DPD Module
 #################################
 
 The Stock Package Shipping DPD module allows you to generate the DPD label
 using the DPD webservices.
 DPD has many different web services, the module supports:
```

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/trytond_stock_package_shipping_dpd.egg-info/SOURCES.txt` & `trytond_stock_package_shipping_dpd-7.2.0/trytond_stock_package_shipping_dpd.egg-info/SOURCES.txt`

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
 carrier.py
```

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/view/carrier_form.xml` & `trytond_stock_package_shipping_dpd-7.2.0/view/carrier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_package_shipping_dpd-7.0.0/view/dpd_credential_form.xml` & `trytond_stock_package_shipping_dpd-7.2.0/view/dpd_credential_form.xml`

 * *Files identical despite different names*

