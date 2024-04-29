# Comparing `tmp/trytond_account_stock_anglo_saxon-7.0.0.tar.gz` & `tmp/trytond_account_stock_anglo_saxon-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_stock_anglo_saxon-7.0.0.tar", last modified: Mon Oct 30 17:25:00 2023, max compression
+gzip compressed data, was "trytond_account_stock_anglo_saxon-7.2.0.tar", last modified: Mon Apr 29 15:36:25 2024, max compression
```

## Comparing `trytond_account_stock_anglo_saxon-7.0.0.tar` & `trytond_account_stock_anglo_saxon-7.2.0.tar`

### file list

```diff
@@ -1,77 +1,76 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:00.894052 trytond_account_stock_anglo_saxon-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      231 2023-10-22 17:22:56.000000 trytond_account_stock_anglo_saxon-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2552 2023-10-30 17:03:40.000000 trytond_account_stock_anglo_saxon-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:03:40.000000 trytond_account_stock_anglo_saxon-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_stock_anglo_saxon-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3812 2023-10-30 17:25:00.894052 trytond_account_stock_anglo_saxon-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:00.894052 trytond_account_stock_anglo_saxon-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2826 2023-10-22 17:22:56.000000 trytond_account_stock_anglo_saxon-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:22:56.000000 trytond_account_stock_anglo_saxon-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      231 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4253 2023-08-13 15:26:13.000000 trytond_account_stock_anglo_saxon-7.0.0/invoice.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:00.890719 trytond_account_stock_anglo_saxon-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1337 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1275 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      985 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1176 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1398 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1338 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1319 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1301 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-10-28 12:11:20.000000 trytond_account_stock_anglo_saxon-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      669 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1124 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      691 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2236 2023-08-13 15:26:13.000000 trytond_account_stock_anglo_saxon-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-01-16 14:00:20.000000 trytond_account_stock_anglo_saxon-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:25:00.894052 trytond_account_stock_anglo_saxon-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4685 2023-10-27 17:38:49.000000 trytond_account_stock_anglo_saxon-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6725 2023-10-07 17:14:58.000000 trytond_account_stock_anglo_saxon-7.0.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:00.890719 trytond_account_stock_anglo_saxon-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12328 2023-10-07 17:14:58.000000 trytond_account_stock_anglo_saxon-7.0.0/tests/scenario_account_stock_anglo_saxon.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8008 2023-08-13 15:26:13.000000 trytond_account_stock_anglo_saxon-7.0.0/tests/scenario_account_stock_anglo_saxon_with_drop_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1829 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-06-10 11:39:56.000000 trytond_account_stock_anglo_saxon-7.0.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_account_stock_anglo_saxon-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2023-10-30 17:03:37.000000 trytond_account_stock_anglo_saxon-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:00.894052 trytond_account_stock_anglo_saxon-7.0.0/trytond_account_stock_anglo_saxon.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3812 2023-10-30 17:25:00.000000 trytond_account_stock_anglo_saxon-7.0.0/trytond_account_stock_anglo_saxon.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2336 2023-10-30 17:25:00.000000 trytond_account_stock_anglo_saxon-7.0.0/trytond_account_stock_anglo_saxon.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:25:00.000000 trytond_account_stock_anglo_saxon-7.0.0/trytond_account_stock_anglo_saxon.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2023-10-30 17:25:00.000000 trytond_account_stock_anglo_saxon-7.0.0/trytond_account_stock_anglo_saxon.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_account_stock_anglo_saxon-7.0.0/trytond_account_stock_anglo_saxon.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-10-30 17:25:00.000000 trytond_account_stock_anglo_saxon-7.0.0/trytond_account_stock_anglo_saxon.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:25:00.000000 trytond_account_stock_anglo_saxon-7.0.0/trytond_account_stock_anglo_saxon.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:25:00.894052 trytond_account_stock_anglo_saxon-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-01-16 14:00:20.000000 trytond_account_stock_anglo_saxon-7.0.0/view/category_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:25.175733 trytond_account_stock_anglo_saxon-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2653 2024-04-29 15:16:26.000000 trytond_account_stock_anglo_saxon-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:16:26.000000 trytond_account_stock_anglo_saxon-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_stock_anglo_saxon-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3812 2024-04-29 15:36:25.175733 trytond_account_stock_anglo_saxon-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:25.172400 trytond_account_stock_anglo_saxon-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3088 2024-04-27 16:30:39.000000 trytond_account_stock_anglo_saxon-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:00.000000 trytond_account_stock_anglo_saxon-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      231 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4253 2024-01-27 09:58:52.000000 trytond_account_stock_anglo_saxon-7.2.0/invoice.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:25.172400 trytond_account_stock_anglo_saxon-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1337 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1275 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      985 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1176 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1398 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1338 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1319 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1301 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      669 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1124 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      691 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2236 2024-01-27 09:58:52.000000 trytond_account_stock_anglo_saxon-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-01-16 14:00:20.000000 trytond_account_stock_anglo_saxon-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:36:25.175733 trytond_account_stock_anglo_saxon-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4685 2024-03-17 11:01:36.000000 trytond_account_stock_anglo_saxon-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6725 2024-02-04 18:51:26.000000 trytond_account_stock_anglo_saxon-7.2.0/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:25.175733 trytond_account_stock_anglo_saxon-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12305 2024-04-27 16:30:39.000000 trytond_account_stock_anglo_saxon-7.2.0/tests/scenario_account_stock_anglo_saxon.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7997 2024-04-27 16:30:39.000000 trytond_account_stock_anglo_saxon-7.2.0/tests/scenario_account_stock_anglo_saxon_with_drop_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1829 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-01-27 09:58:52.000000 trytond_account_stock_anglo_saxon-7.2.0/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:00.000000 trytond_account_stock_anglo_saxon-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2024-04-29 15:16:21.000000 trytond_account_stock_anglo_saxon-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:25.175733 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3812 2024-04-29 15:36:24.000000 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2318 2024-04-29 15:36:25.000000 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:36:24.000000 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:36:24.000000 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2024-04-29 15:36:24.000000 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:36:24.000000 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:25.175733 trytond_account_stock_anglo_saxon-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-01-16 14:00:20.000000 trytond_account_stock_anglo_saxon-7.2.0/view/category_form.xml
```

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/CHANGELOG` & `trytond_account_stock_anglo_saxon-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

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

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/COPYRIGHT` & `trytond_account_stock_anglo_saxon-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2010-2023 Cédric Krier.
-Copyright (C) 2010-2023 B2CK SPRL.
+Copyright (C) 2010-2024 Cédric Krier.
+Copyright (C) 2010-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/LICENSE` & `trytond_account_stock_anglo_saxon-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/PKG-INFO` & `trytond_account_stock_anglo_saxon-7.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_anglo_saxon
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for anglo-saxon real-time stock valuation
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
@@ -48,25 +48,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_account_stock_continental<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond_account_stock_continental<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_supply_drop_shipment<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_supply_drop_shipment<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
 
 Account Stock Anglo-Saxon Module
 ################################
 
 The account_stock_anglo_saxon module adds anglo-saxon accounting model for
 stock valuation.
```

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/README.rst` & `trytond_account_stock_anglo_saxon-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/doc/conf.py` & `trytond_account_stock_anglo_saxon-7.2.0/doc/conf.py`

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

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/doc/index.rst` & `trytond_account_stock_anglo_saxon-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/invoice.py` & `trytond_account_stock_anglo_saxon-7.2.0/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/bg.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/ca.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/cs.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/de.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/es.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/es_419.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/et.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/fa.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/fi.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/fr.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/hu.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/id.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/it.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/lo.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/lt.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/nl.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/pl.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/pt.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/ro.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/ru.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/sl.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/tr.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/uk.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/locale/zh_CN.po` & `trytond_account_stock_anglo_saxon-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/message.xml` & `trytond_account_stock_anglo_saxon-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/minimal_chart.xml` & `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_bg.xml` & `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_ca.xml` & `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_de.xml` & `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_en.xml` & `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_es.xml` & `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_fr.xml` & `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_nl.xml` & `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_pt.xml` & `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_ru.xml` & `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/minimal_chart_sl.xml` & `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/product.py` & `trytond_account_stock_anglo_saxon-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/setup.py` & `trytond_account_stock_anglo_saxon-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/stock.py` & `trytond_account_stock_anglo_saxon-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/tests/scenario_account_stock_anglo_saxon.rst` & `trytond_account_stock_anglo_saxon-7.2.0/tests/scenario_account_stock_anglo_saxon.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 Account Stock Anglo-Saxon Scenario
 ==================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.account_stock_anglo_saxon.tests.tools import (
+    ...     add_cogs_accounts)
+    >>> from trytond.modules.account_stock_continental.tests.tools import (
+    ...     add_stock_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> from trytond.modules.account_stock_continental.tests.tools import \
-    ...     add_stock_accounts
-    >>> from trytond.modules.account_stock_anglo_saxon.tests.tools import \
-    ...     add_cogs_accounts
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'account_stock_anglo_saxon',
@@ -167,15 +167,15 @@
     >>> shipment.incoming_moves.append(move)
     >>> move.quantity = 4.0
     >>> move, = [m for m in purchase.moves if m.product == product_average]
     >>> move = Move(move.id)
     >>> shipment.incoming_moves.append(move)
     >>> move.quantity = 5.0
     >>> shipment.click('receive')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
     >>> stock_in.reload()
     >>> stock.reload()
     >>> stock_in.debit
     Decimal('0.00')
     >>> stock_in.credit
@@ -248,15 +248,15 @@
     'assigned'
     >>> shipment.click('pick')
     >>> shipment.state
     'picked'
     >>> shipment.click('pack')
     >>> shipment.state
     'packed'
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
     >>> stock_out.reload()
     >>> stock_out.debit
     Decimal('28.00')
     >>> stock_out.credit
     Decimal('0.00')
@@ -376,15 +376,15 @@
     >>> set_user(stock_user)
     >>> shipment = ShipmentIn(supplier=supplier)
     >>> move = Move(purchase.moves[0].id)
     >>> move.in_anglo_saxon_quantity
     0.0
     >>> shipment.incoming_moves.append(move)
     >>> shipment.click('receive')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
 
     >>> set_user(accountant)
     >>> purchase.reload()
     >>> invoice, = purchase.invoices
     >>> invoice.invoice_date = today
     >>> invoice.click('post')
     >>> invoice.state
```

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/tests/scenario_account_stock_anglo_saxon_with_drop_shipment.rst` & `trytond_account_stock_anglo_saxon-7.2.0/tests/scenario_account_stock_anglo_saxon_with_drop_shipment.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 Account Stock Anglo-Saxon with Drop Shipment Scenario
 =====================================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.account_stock_anglo_saxon.tests.tools import (
+    ...     add_cogs_accounts)
+    >>> from trytond.modules.account_stock_continental.tests.tools import (
+    ...     add_stock_accounts)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
-    >>> from trytond.modules.account_stock_continental.tests.tools import \
-    ...     add_stock_accounts
-    >>> from trytond.modules.account_stock_anglo_saxon.tests.tools import \
-    ...     add_cogs_accounts
 
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules([
     ...         'account_stock_anglo_saxon',
@@ -188,15 +188,15 @@
     []
     >>> shipment, = sale.drop_shipments
 
 Receive 50 products::
 
     >>> set_user(stock_user)
     >>> shipment.click('ship')
-    >>> shipment.click('done')
+    >>> shipment.click('do')
     >>> shipment.state
     'done'
     >>> set_user(account_user)
     >>> stock_in.reload()
     >>> stock_in.debit
     Decimal('0.00')
     >>> stock_in.credit
```

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/tests/test_module.py` & `trytond_account_stock_anglo_saxon-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/tests/tools.py` & `trytond_account_stock_anglo_saxon-7.2.0/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/tox.ini` & `trytond_account_stock_anglo_saxon-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/trytond_account_stock_anglo_saxon.egg-info/PKG-INFO` & `trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-account-stock-anglo-saxon
-Version: 7.0.0
+Name: trytond_account_stock_anglo_saxon
+Version: 7.2.0
 Summary: Tryton module for anglo-saxon real-time stock valuation
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
@@ -48,25 +48,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_account_invoice_stock<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_account_stock_continental<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_account_invoice_stock<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond_account_stock_continental<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale_supply_drop_shipment<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_sale<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_purchase<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_supply_drop_shipment<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_purchase<7.3,>=7.2; extra == "test"
 
 Account Stock Anglo-Saxon Module
 ################################
 
 The account_stock_anglo_saxon module adds anglo-saxon accounting model for
 stock valuation.
```

### Comparing `trytond_account_stock_anglo_saxon-7.0.0/trytond_account_stock_anglo_saxon.egg-info/SOURCES.txt` & `trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/SOURCES.txt`

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

