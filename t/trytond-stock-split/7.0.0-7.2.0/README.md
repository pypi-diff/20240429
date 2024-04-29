# Comparing `tmp/trytond_stock_split-7.0.0.tar.gz` & `tmp/trytond_stock_split-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_split-7.0.0.tar", last modified: Mon Oct 30 17:44:08 2023, max compression
+gzip compressed data, was "trytond_stock_split-7.2.0.tar", last modified: Mon Apr 29 15:53:11 2024, max compression
```

## Comparing `trytond_stock_split-7.0.0.tar` & `trytond_stock_split-7.2.0.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:08.586193 trytond_stock_split-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      203 2023-10-22 17:23:28.000000 trytond_stock_split-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2090 2023-10-30 17:15:39.000000 trytond_stock_split-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:15:38.000000 trytond_stock_split-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_split-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_split-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2902 2023-10-30 17:44:08.586193 trytond_stock_split-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      476 2023-01-16 14:00:21.000000 trytond_stock_split-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      572 2023-04-15 07:12:15.000000 trytond_stock_split-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:08.582860 trytond_stock_split-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2812 2023-10-22 17:23:28.000000 trytond_stock_split-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      476 2023-01-16 14:00:21.000000 trytond_stock_split-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:28.000000 trytond_stock_split-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:08.582860 trytond_stock_split-7.0.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_stock_split-7.0.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_stock_split-7.0.0/icons/tryton-stock-split.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:08.582860 trytond_stock_split-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     2285 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2420 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2161 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2519 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2430 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2059 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2187 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2599 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2161 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2457 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2284 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2054 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2244 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2397 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2161 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2431 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2215 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2418 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2033 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2283 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2255 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2161 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2033 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2191 2023-10-30 16:47:45.000000 trytond_stock_split-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:44:08.586193 trytond_stock_split-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4399 2023-10-27 17:38:49.000000 trytond_stock_split-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6569 2023-10-24 07:56:52.000000 trytond_stock_split-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4342 2023-04-15 07:12:15.000000 trytond_stock_split-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:08.582860 trytond_stock_split-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_split-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2592 2023-10-07 17:14:58.000000 trytond_stock_split-7.0.0/tests/scenario_stock_split_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3283 2023-10-07 17:14:58.000000 trytond_stock_split-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_split-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_stock_split-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-10-30 17:15:35.000000 trytond_stock_split-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:08.582860 trytond_stock_split-7.0.0/trytond_stock_split.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2902 2023-10-30 17:44:08.000000 trytond_stock_split-7.0.0/trytond_stock_split.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1768 2023-10-30 17:44:08.000000 trytond_stock_split-7.0.0/trytond_stock_split.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:44:08.000000 trytond_stock_split-7.0.0/trytond_stock_split.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       60 2023-10-30 17:44:08.000000 trytond_stock_split-7.0.0/trytond_stock_split.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_stock_split-7.0.0/trytond_stock_split.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-10-30 17:44:08.000000 trytond_stock_split-7.0.0/trytond_stock_split.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:44:08.000000 trytond_stock_split-7.0.0/trytond_stock_split.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:08.582860 trytond_stock_split-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_stock_split-7.0.0/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-01-16 14:00:21.000000 trytond_stock_split-7.0.0/view/move_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      297 2023-01-16 14:00:21.000000 trytond_stock_split-7.0.0/view/shipment_split_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 trytond_stock_split-7.0.0/view/shipment_split_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-10-07 17:14:58.000000 trytond_stock_split-7.0.0/view/split_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:11.772740 trytond_stock_split-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2191 2024-04-29 15:29:15.000000 trytond_stock_split-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:29:15.000000 trytond_stock_split-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_split-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_split-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2902 2024-04-29 15:53:11.772740 trytond_stock_split-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      476 2023-01-16 14:00:21.000000 trytond_stock_split-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      572 2023-04-15 07:12:15.000000 trytond_stock_split-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:11.766073 trytond_stock_split-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3074 2024-04-27 16:30:39.000000 trytond_stock_split-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      476 2023-01-16 14:00:21.000000 trytond_stock_split-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:37.000000 trytond_stock_split-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:11.766073 trytond_stock_split-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_stock_split-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_stock_split-7.2.0/icons/tryton-stock-split.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:11.769407 trytond_stock_split-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2285 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2420 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2161 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2519 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2430 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2059 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2187 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2599 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2161 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2457 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2284 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2054 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2244 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2397 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2161 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2431 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2215 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2418 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2033 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2283 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2255 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2161 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2033 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2191 2024-04-27 16:43:28.000000 trytond_stock_split-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:53:11.772740 trytond_stock_split-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4399 2024-03-17 11:01:36.000000 trytond_stock_split-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6569 2024-02-04 18:51:27.000000 trytond_stock_split-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4250 2024-04-27 16:30:39.000000 trytond_stock_split-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:11.769407 trytond_stock_split-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_split-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2575 2024-04-22 12:14:36.000000 trytond_stock_split-7.2.0/tests/scenario_stock_split_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3283 2024-02-04 18:51:27.000000 trytond_stock_split-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_split-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:37.000000 trytond_stock_split-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:29:11.000000 trytond_stock_split-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:11.769407 trytond_stock_split-7.2.0/trytond_stock_split.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2902 2024-04-29 15:53:11.000000 trytond_stock_split-7.2.0/trytond_stock_split.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1750 2024-04-29 15:53:11.000000 trytond_stock_split-7.2.0/trytond_stock_split.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:53:11.000000 trytond_stock_split-7.2.0/trytond_stock_split.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       60 2024-04-29 15:53:11.000000 trytond_stock_split-7.2.0/trytond_stock_split.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_stock_split-7.2.0/trytond_stock_split.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:53:11.000000 trytond_stock_split-7.2.0/trytond_stock_split.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:53:11.000000 trytond_stock_split-7.2.0/trytond_stock_split.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:11.769407 trytond_stock_split-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-04-15 07:12:15.000000 trytond_stock_split-7.2.0/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-01-16 14:00:21.000000 trytond_stock_split-7.2.0/view/move_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      297 2023-01-16 14:00:21.000000 trytond_stock_split-7.2.0/view/shipment_split_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 trytond_stock_split-7.2.0/view/shipment_split_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-02-04 18:51:27.000000 trytond_stock_split-7.2.0/view/split_start_form.xml
```

### Comparing `trytond_stock_split-7.0.0/CHANGELOG` & `trytond_stock_split-7.2.0/CHANGELOG`

 * *Files 1% similar despite different names*

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

### Comparing `trytond_stock_split-7.0.0/LICENSE` & `trytond_stock_split-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/PKG-INFO` & `trytond_stock_split-7.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_split
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to split stock move
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
@@ -48,18 +48,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Stock Split Module
 ##################
 
 The Stock Split module adds on the stock move a wizard that allows to split them.
 The move is split into moves of *Quantity*. If *Counts* is set, it will be
 split only this number of times. On occasion there can be a move with the
```

### Comparing `trytond_stock_split-7.0.0/__init__.py` & `trytond_stock_split-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/doc/conf.py` & `trytond_stock_split-7.2.0/doc/conf.py`

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

### Comparing `trytond_stock_split-7.0.0/icons/LICENSE` & `trytond_stock_split-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/bg.po` & `trytond_stock_split-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/ca.po` & `trytond_stock_split-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/cs.po` & `trytond_stock_split-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/de.po` & `trytond_stock_split-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/es.po` & `trytond_stock_split-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/es_419.po` & `trytond_stock_split-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/et.po` & `trytond_stock_split-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/fa.po` & `trytond_stock_split-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/fi.po` & `trytond_stock_split-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/fr.po` & `trytond_stock_split-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/hu.po` & `trytond_stock_split-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/id.po` & `trytond_stock_split-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/it.po` & `trytond_stock_split-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/lo.po` & `trytond_stock_split-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/lt.po` & `trytond_stock_split-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/nl.po` & `trytond_stock_split-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/pl.po` & `trytond_stock_split-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/pt.po` & `trytond_stock_split-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/ro.po` & `trytond_stock_split-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/ru.po` & `trytond_stock_split-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/sl.po` & `trytond_stock_split-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/tr.po` & `trytond_stock_split-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/uk.po` & `trytond_stock_split-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/locale/zh_CN.po` & `trytond_stock_split-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/setup.py` & `trytond_stock_split-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/stock.py` & `trytond_stock_split-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/stock.xml` & `trytond_stock_split-7.2.0/stock.xml`

 * *Files 8% similar despite different names*

#### Comparing `trytond_stock_split-7.0.0/stock.xml` & `trytond_stock_split-7.2.0/stock.xml`

```diff
@@ -34,47 +34,47 @@
     </record>
     <record model="ir.ui.view" id="split_start_view_form">
       <field name="model">stock.move.split.start</field>
       <field name="type">form</field>
       <field name="name">split_start_form</field>
     </record>
     <record model="ir.model.button" id="move_split_wizard_button">
+      <field name="model">stock.move</field>
       <field name="name">split_wizard</field>
       <field name="string">Split</field>
-      <field name="model" search="[('model', '=', 'stock.move')]"/>
     </record>
     <record model="ir.ui.view" id="shipment_in_return_view_form">
       <field name="model">stock.shipment.in.return</field>
       <field name="inherit" ref="stock.shipment_in_return_view_form"/>
       <field name="name">shipment_split_form</field>
     </record>
     <record model="ir.model.button" id="shipment_in_return_split_wizard_button">
+      <field name="model">stock.shipment.in.return</field>
       <field name="name">split_wizard</field>
       <field name="string">Split</field>
-      <field name="model" search="[('model', '=', 'stock.shipment.in.return')]"/>
     </record>
     <record model="ir.ui.view" id="shipment_out_view_form">
       <field name="model">stock.shipment.out</field>
       <field name="inherit" ref="stock.shipment_out_view_form"/>
       <field name="name">shipment_split_form</field>
     </record>
     <record model="ir.model.button" id="shipment_out_split_wizard_button">
+      <field name="model">stock.shipment.out</field>
       <field name="name">split_wizard</field>
       <field name="string">Split</field>
-      <field name="model" search="[('model', '=', 'stock.shipment.out')]"/>
     </record>
     <record model="ir.ui.view" id="shipment_internal_view_form">
       <field name="model">stock.shipment.internal</field>
       <field name="inherit" ref="stock.shipment_internal_view_form"/>
       <field name="name">shipment_split_form</field>
     </record>
     <record model="ir.model.button" id="shipment_internal_split_wizard_button">
+      <field name="model">stock.shipment.internal</field>
       <field name="name">split_wizard</field>
       <field name="string">Split</field>
-      <field name="model" search="[('model', '=', 'stock.shipment.internal')]"/>
     </record>
     <record model="ir.action.wizard" id="wizard_split_shipment">
       <field name="name">Split Shipment</field>
       <field name="wiz_name">stock.shipment.split</field>
     </record>
     <record model="ir.ui.view" id="shipment_split_start_view_form">
       <field name="model">stock.shipment.split.start</field>
```

### Comparing `trytond_stock_split-7.0.0/tests/scenario_stock_split_shipment.rst` & `trytond_stock_split-7.2.0/tests/scenario_stock_split_shipment.rst`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 Stock Split Shipment
 ====================
 
 Imports::
 
     >>> from decimal import Decimal
 
-    >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+    >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate modules::
 
     >>> config = activate_modules('stock_split')
 
 Create company::
 
@@ -67,30 +66,28 @@
 
     >>> shipment1.save()
     >>> move1, move2 = shipment1.outgoing_moves
 
 Set to waiting and go back to draft to get inventory moves::
 
     >>> shipment1.click('wait')
-    >>> shipment1.click('draft')
     >>> len(shipment1.inventory_moves)
     2
+    >>> shipment1.click('draft')
 
 Split shipment::
 
     >>> split_shipment = shipment1.click('split_wizard')
     >>> len(split_shipment.form.domain_moves)
     2
     >>> split_shipment.form.moves.append(Move(move2.id))
     >>> split_shipment.execute('split')
 
     >>> shipment2, = Shipment.find([('id', '!=', shipment1.id)])
 
     >>> move, = shipment1.outgoing_moves
-    >>> move.id == move1.id
-    True
+    >>> assertEqual(move, move1)
     >>> len(shipment1.inventory_moves)
     0
 
     >>> move, = shipment2.outgoing_moves
-    >>> move.id == move2.id
-    True
+    >>> assertEqual(move, move2)
```

### Comparing `trytond_stock_split-7.0.0/tests/test_module.py` & `trytond_stock_split-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/tox.ini` & `trytond_stock_split-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_split-7.0.0/trytond_stock_split.egg-info/PKG-INFO` & `trytond_stock_split-7.2.0/trytond_stock_split.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-stock-split
-Version: 7.0.0
+Name: trytond_stock_split
+Version: 7.2.0
 Summary: Tryton module to split stock move
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
@@ -48,18 +48,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Stock Split Module
 ##################
 
 The Stock Split module adds on the stock move a wizard that allows to split them.
 The move is split into moves of *Quantity*. If *Counts* is set, it will be
 split only this number of times. On occasion there can be a move with the
```

### Comparing `trytond_stock_split-7.0.0/trytond_stock_split.egg-info/SOURCES.txt` & `trytond_stock_split-7.2.0/trytond_stock_split.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 setup.py
```

