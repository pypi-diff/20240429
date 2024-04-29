# Comparing `tmp/trytond_sale_subscription_asset-7.0.0.tar.gz` & `tmp/trytond_sale_subscription_asset-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_subscription_asset-7.0.0.tar", last modified: Mon Oct 30 17:40:30 2023, max compression
+gzip compressed data, was "trytond_sale_subscription_asset-7.2.0.tar", last modified: Mon Apr 29 15:50:07 2024, max compression
```

## Comparing `trytond_sale_subscription_asset-7.0.0.tar` & `trytond_sale_subscription_asset-7.2.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:30.068484 trytond_sale_subscription_asset-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-10-22 17:23:22.000000 trytond_sale_subscription_asset-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1043 2023-10-30 17:13:36.000000 trytond_sale_subscription_asset-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-10-30 17:13:35.000000 trytond_sale_subscription_asset-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_subscription_asset-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3066 2023-10-30 17:40:30.068484 trytond_sale_subscription_asset-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      632 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-04-15 07:12:15.000000 trytond_sale_subscription_asset-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:30.065151 trytond_sale_subscription_asset-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2824 2023-10-22 17:23:22.000000 trytond_sale_subscription_asset-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      632 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:22.000000 trytond_sale_subscription_asset-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:30.061818 trytond_sale_subscription_asset-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1383 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1453 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1389 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1374 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1122 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1392 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1370 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1118 2023-10-28 12:11:25.000000 trytond_sale_subscription_asset-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-04-15 07:12:15.000000 trytond_sale_subscription_asset-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5858 2023-09-18 07:38:16.000000 trytond_sale_subscription_asset-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1113 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.0.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:40:30.068484 trytond_sale_subscription_asset-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4458 2023-10-27 17:38:49.000000 trytond_sale_subscription_asset-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:30.065151 trytond_sale_subscription_asset-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_subscription_asset-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4985 2023-04-15 07:12:15.000000 trytond_sale_subscription_asset-7.0.0/tests/scenario_sale_subscription_asset.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_sale_subscription_asset-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_subscription_asset-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_sale_subscription_asset-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      123 2023-10-30 17:13:32.000000 trytond_sale_subscription_asset-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:30.065151 trytond_sale_subscription_asset-7.0.0/trytond_sale_subscription_asset.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3066 2023-10-30 17:40:29.000000 trytond_sale_subscription_asset-7.0.0/trytond_sale_subscription_asset.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1836 2023-10-30 17:40:30.000000 trytond_sale_subscription_asset-7.0.0/trytond_sale_subscription_asset.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:40:29.000000 trytond_sale_subscription_asset-7.0.0/trytond_sale_subscription_asset.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       84 2023-10-30 17:40:29.000000 trytond_sale_subscription_asset-7.0.0/trytond_sale_subscription_asset.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_sale_subscription_asset-7.0.0/trytond_sale_subscription_asset.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      108 2023-10-30 17:40:29.000000 trytond_sale_subscription_asset-7.0.0/trytond_sale_subscription_asset.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:40:29.000000 trytond_sale_subscription_asset-7.0.0/trytond_sale_subscription_asset.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:40:30.065151 trytond_sale_subscription_asset-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.0.0/view/stock_lot_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:15.000000 trytond_sale_subscription_asset-7.0.0/view/subscription_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.0.0/view/subscription_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.0.0/view/subscription_service_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:07.127569 trytond_sale_subscription_asset-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1144 2024-04-29 15:26:58.000000 trytond_sale_subscription_asset-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2024-04-29 15:26:58.000000 trytond_sale_subscription_asset-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_subscription_asset-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3066 2024-04-29 15:50:07.124236 trytond_sale_subscription_asset-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      632 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-04-15 07:12:15.000000 trytond_sale_subscription_asset-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:07.120903 trytond_sale_subscription_asset-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3086 2024-04-27 16:30:39.000000 trytond_sale_subscription_asset-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      632 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:30.000000 trytond_sale_subscription_asset-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:07.124236 trytond_sale_subscription_asset-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1383 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1453 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1389 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1374 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1122 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1392 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1370 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1118 2024-04-27 16:43:27.000000 trytond_sale_subscription_asset-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-04-15 07:12:15.000000 trytond_sale_subscription_asset-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5858 2023-09-18 07:38:16.000000 trytond_sale_subscription_asset-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1113 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:50:07.127569 trytond_sale_subscription_asset-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4458 2024-03-17 11:01:36.000000 trytond_sale_subscription_asset-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      462 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:07.124236 trytond_sale_subscription_asset-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_subscription_asset-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4891 2024-04-22 12:14:36.000000 trytond_sale_subscription_asset-7.2.0/tests/scenario_sale_subscription_asset.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-04-15 07:12:15.000000 trytond_sale_subscription_asset-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_subscription_asset-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:30.000000 trytond_sale_subscription_asset-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      123 2024-04-29 15:26:54.000000 trytond_sale_subscription_asset-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:07.124236 trytond_sale_subscription_asset-7.2.0/trytond_sale_subscription_asset.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3066 2024-04-29 15:50:06.000000 trytond_sale_subscription_asset-7.2.0/trytond_sale_subscription_asset.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1818 2024-04-29 15:50:07.000000 trytond_sale_subscription_asset-7.2.0/trytond_sale_subscription_asset.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:50:06.000000 trytond_sale_subscription_asset-7.2.0/trytond_sale_subscription_asset.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       84 2024-04-29 15:50:06.000000 trytond_sale_subscription_asset-7.2.0/trytond_sale_subscription_asset.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_sale_subscription_asset-7.2.0/trytond_sale_subscription_asset.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      108 2024-04-29 15:50:06.000000 trytond_sale_subscription_asset-7.2.0/trytond_sale_subscription_asset.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:50:06.000000 trytond_sale_subscription_asset-7.2.0/trytond_sale_subscription_asset.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:07.124236 trytond_sale_subscription_asset-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.2.0/view/stock_lot_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-04-15 07:12:15.000000 trytond_sale_subscription_asset-7.2.0/view/subscription_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.2.0/view/subscription_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      378 2023-01-16 14:00:21.000000 trytond_sale_subscription_asset-7.2.0/view/subscription_service_form.xml
```

### Comparing `trytond_sale_subscription_asset-7.0.0/CHANGELOG` & `trytond_sale_subscription_asset-7.2.0/CHANGELOG`

 * *Files 3% similar despite different names*

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

### Comparing `trytond_sale_subscription_asset-7.0.0/COPYRIGHT` & `trytond_sale_subscription_asset-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2018-2023 B2CK
-Copyright (C) 2018-2023 Cédric Krier
+Copyright (C) 2018-2024 B2CK
+Copyright (C) 2018-2024 Cédric Krier
 Copyright (C) 2018-2023 Nicolas Évrard
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_sale_subscription_asset-7.0.0/LICENSE` & `trytond_sale_subscription_asset-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/PKG-INFO` & `trytond_sale_subscription_asset-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_subscription_asset
-Version: 7.0.0
+Version: 7.2.0
 Summary: A module to handle asset in the sale subscriptions
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
@@ -46,19 +46,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_sale_subscription<7.1,>=7.0
-Requires-Dist: trytond_stock_lot<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_sale_subscription<7.3,>=7.2
+Requires-Dist: trytond_stock_lot<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Subscription Asset Module
 ##############################
 
 The sale subscription asset module adds the notion of asset to the sale
 subscription module.
```

### Comparing `trytond_sale_subscription_asset-7.0.0/README.rst` & `trytond_sale_subscription_asset-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/doc/conf.py` & `trytond_sale_subscription_asset-7.2.0/doc/conf.py`

 * *Files 8% similar despite different names*

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

### Comparing `trytond_sale_subscription_asset-7.0.0/doc/index.rst` & `trytond_sale_subscription_asset-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/bg.po` & `trytond_sale_subscription_asset-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/ca.po` & `trytond_sale_subscription_asset-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/cs.po` & `trytond_sale_subscription_asset-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/de.po` & `trytond_sale_subscription_asset-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/es.po` & `trytond_sale_subscription_asset-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/es_419.po` & `trytond_sale_subscription_asset-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/et.po` & `trytond_sale_subscription_asset-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/fa.po` & `trytond_sale_subscription_asset-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/fi.po` & `trytond_sale_subscription_asset-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/fr.po` & `trytond_sale_subscription_asset-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/hu.po` & `trytond_sale_subscription_asset-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/id.po` & `trytond_sale_subscription_asset-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/it.po` & `trytond_sale_subscription_asset-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/lo.po` & `trytond_sale_subscription_asset-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/lt.po` & `trytond_sale_subscription_asset-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/nl.po` & `trytond_sale_subscription_asset-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/pl.po` & `trytond_sale_subscription_asset-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/pt.po` & `trytond_sale_subscription_asset-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/ro.po` & `trytond_sale_subscription_asset-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/ru.po` & `trytond_sale_subscription_asset-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/sl.po` & `trytond_sale_subscription_asset-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/tr.po` & `trytond_sale_subscription_asset-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/uk.po` & `trytond_sale_subscription_asset-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/locale/zh_CN.po` & `trytond_sale_subscription_asset-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/sale.py` & `trytond_sale_subscription_asset-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/sale.xml` & `trytond_sale_subscription_asset-7.2.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/setup.py` & `trytond_sale_subscription_asset-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/stock.py` & `trytond_sale_subscription_asset-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/tests/scenario_sale_subscription_asset.rst` & `trytond_sale_subscription_asset-7.2.0/tests/scenario_sale_subscription_asset.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 Sale Subscription Asset Scenario
 ================================
 
 Imports::
 
     >>> import datetime
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
 
     >>> config = activate_modules('sale_subscription_asset')
 
 Create company::
 
@@ -96,15 +95,15 @@
     >>> subscription.invoice_start_date = datetime.date(2016, 2, 1)
     >>> subscription.invoice_recurrence = monthly
     >>> line = subscription.lines.new()
     >>> line.service = service
     >>> line.quantity = 1
 
     >>> subscription.click('quote')
-    >>> subscription.click('run')  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> subscription.click('run')
     Traceback (most recent call last):
         ...
     RequiredValidationError: ...
 
     >>> subscription.click('draft')
     >>> line, = subscription.lines
     >>> line.asset_lot = lot1
@@ -113,16 +112,15 @@
 
     >>> with config.set_context(date=datetime.date(2017, 1, 1)):
     ...     lot1.reload()
     ...     subscribed_line = lot1.subscribed
     ...     service.reload()
     ...     lots_available = sorted(
     ...         l.number for l in service.asset_lots_available)
-    >>> subscribed_line == line
-    True
+    >>> assertEqual(subscribed_line, line)
     >>> lots_available
     ['002']
 
 Creating an overlapping line won't work::
 
     >>> overlapping = Subscription()
     >>> overlapping.party = customer
@@ -130,15 +128,15 @@
     >>> overlapping.invoice_start_date = datetime.date(2017, 2, 1)
     >>> overlapping.invoice_recurrence = monthly
     >>> line = overlapping.lines.new()
     >>> line.service = service
     >>> line.start_date = datetime.date(2017, 1, 1)
     >>> line.quantity = 1
     >>> line.asset_lot = lot1
-    >>> overlapping.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> overlapping.save()
     Traceback (most recent call last):
         ...
     ValidationError: ....
 
 Cancelling the subscription will remove lot from the lines thus making it
 available again::
```

### Comparing `trytond_sale_subscription_asset-7.0.0/tox.ini` & `trytond_sale_subscription_asset-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_subscription_asset-7.0.0/trytond_sale_subscription_asset.egg-info/PKG-INFO` & `trytond_sale_subscription_asset-7.2.0/trytond_sale_subscription_asset.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-sale-subscription-asset
-Version: 7.0.0
+Name: trytond_sale_subscription_asset
+Version: 7.2.0
 Summary: A module to handle asset in the sale subscriptions
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
@@ -46,19 +46,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_sale_subscription<7.1,>=7.0
-Requires-Dist: trytond_stock_lot<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_sale_subscription<7.3,>=7.2
+Requires-Dist: trytond_stock_lot<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Sale Subscription Asset Module
 ##############################
 
 The sale subscription asset module adds the notion of asset to the sale
 subscription module.
```

### Comparing `trytond_sale_subscription_asset-7.0.0/trytond_sale_subscription_asset.egg-info/SOURCES.txt` & `trytond_sale_subscription_asset-7.2.0/trytond_sale_subscription_asset.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

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

