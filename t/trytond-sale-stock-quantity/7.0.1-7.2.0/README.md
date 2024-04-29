# Comparing `tmp/trytond_sale_stock_quantity-7.0.1.tar.gz` & `tmp/trytond_sale_stock_quantity-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale_stock_quantity-7.0.1.tar", last modified: Thu Feb 15 18:33:03 2024, max compression
+gzip compressed data, was "trytond_sale_stock_quantity-7.2.0.tar", last modified: Mon Apr 29 15:49:53 2024, max compression
```

## Comparing `trytond_sale_stock_quantity-7.0.1.tar` & `trytond_sale_stock_quantity-7.2.0.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:33:03.846268 trytond_sale_stock_quantity-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      219 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1743 2024-02-15 18:33:01.000000 trytond_sale_stock_quantity-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-02-15 18:33:00.000000 trytond_sale_stock_quantity-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2911 2024-02-15 18:33:03.846268 trytond_sale_stock_quantity-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:33:03.842934 trytond_sale_stock_quantity-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2820 2024-02-05 16:24:27.000000 trytond_sale_stock_quantity-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:33:03.846268 trytond_sale_stock_quantity-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      848 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      840 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      832 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      844 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      990 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      859 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      844 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      826 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      920 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      847 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      840 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      842 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      848 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      577 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      703 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    10880 2024-02-10 10:13:14.000000 trytond_sale_stock_quantity-7.0.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      586 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-02-15 18:33:03.846268 trytond_sale_stock_quantity-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4530 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:33:03.846268 trytond_sale_stock_quantity-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6077 2024-02-05 16:24:27.000000 trytond_sale_stock_quantity-7.0.1/tests/scenario_sale_stock_quantity.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_sale_stock_quantity-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      145 2024-02-05 16:24:27.000000 trytond_sale_stock_quantity-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-02-15 18:33:03.846268 trytond_sale_stock_quantity-7.0.1/trytond_sale_stock_quantity.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2911 2024-02-15 18:33:03.000000 trytond_sale_stock_quantity-7.0.1/trytond_sale_stock_quantity.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1534 2024-02-15 18:33:03.000000 trytond_sale_stock_quantity-7.0.1/trytond_sale_stock_quantity.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-02-15 18:33:03.000000 trytond_sale_stock_quantity-7.0.1/trytond_sale_stock_quantity.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2024-02-15 18:33:03.000000 trytond_sale_stock_quantity-7.0.1/trytond_sale_stock_quantity.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:11.000000 trytond_sale_stock_quantity-7.0.1/trytond_sale_stock_quantity.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      148 2024-02-15 18:33:03.000000 trytond_sale_stock_quantity-7.0.1/trytond_sale_stock_quantity.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-02-15 18:33:03.000000 trytond_sale_stock_quantity-7.0.1/trytond_sale_stock_quantity.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:53.371262 trytond_sale_stock_quantity-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1743 2024-04-29 15:26:48.000000 trytond_sale_stock_quantity-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:26:48.000000 trytond_sale_stock_quantity-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_sale_stock_quantity-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2911 2024-04-29 15:49:53.371262 trytond_sale_stock_quantity-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-01-16 14:00:21.000000 trytond_sale_stock_quantity-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:53.367929 trytond_sale_stock_quantity-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3082 2024-04-27 16:30:39.000000 trytond_sale_stock_quantity-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      327 2023-01-16 14:00:21.000000 trytond_sale_stock_quantity-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:29.000000 trytond_sale_stock_quantity-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:53.367929 trytond_sale_stock_quantity-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      848 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      840 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      832 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      844 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      990 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      859 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      844 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      826 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      920 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      847 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      840 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      842 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      848 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      577 2024-04-27 16:43:27.000000 trytond_sale_stock_quantity-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      703 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    10652 2024-04-22 12:14:36.000000 trytond_sale_stock_quantity-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      586 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:49:53.371262 trytond_sale_stock_quantity-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4530 2024-03-17 11:01:36.000000 trytond_sale_stock_quantity-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:53.371262 trytond_sale_stock_quantity-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5942 2024-04-22 12:14:36.000000 trytond_sale_stock_quantity-7.2.0/tests/scenario_sale_stock_quantity.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_sale_stock_quantity-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:29.000000 trytond_sale_stock_quantity-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      145 2024-04-29 15:26:44.000000 trytond_sale_stock_quantity-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:49:53.371262 trytond_sale_stock_quantity-7.2.0/trytond_sale_stock_quantity.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2911 2024-04-29 15:49:52.000000 trytond_sale_stock_quantity-7.2.0/trytond_sale_stock_quantity.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1516 2024-04-29 15:49:53.000000 trytond_sale_stock_quantity-7.2.0/trytond_sale_stock_quantity.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:49:52.000000 trytond_sale_stock_quantity-7.2.0/trytond_sale_stock_quantity.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2024-04-29 15:49:52.000000 trytond_sale_stock_quantity-7.2.0/trytond_sale_stock_quantity.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:06.000000 trytond_sale_stock_quantity-7.2.0/trytond_sale_stock_quantity.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      148 2024-04-29 15:49:52.000000 trytond_sale_stock_quantity-7.2.0/trytond_sale_stock_quantity.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:49:52.000000 trytond_sale_stock_quantity-7.2.0/trytond_sale_stock_quantity.egg-info/top_level.txt
```

### Comparing `trytond_sale_stock_quantity-7.0.1/CHANGELOG` & `trytond_sale_stock_quantity-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-02-15
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_sale_stock_quantity-7.0.1/COPYRIGHT` & `trytond_sale_stock_quantity-7.2.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/LICENSE` & `trytond_sale_stock_quantity-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/PKG-INFO` & `trytond_sale_stock_quantity-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_stock_quantity
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to add stock warning on sale
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
@@ -48,21 +48,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_supply<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_supply<7.3,>=7.2; extra == "test"
 
 Sale Stock Quantity
 ###################
 
 The sale_stock_quantity module check the stock quantity of the products when
 quoting a sale. The check will warn the user if the forecast quantity at the
 sale date (and further dates until next supply) is lower than the quantity sold
```

### Comparing `trytond_sale_stock_quantity-7.0.1/doc/conf.py` & `trytond_sale_stock_quantity-7.2.0/doc/conf.py`

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

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/bg.po` & `trytond_sale_stock_quantity-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/ca.po` & `trytond_sale_stock_quantity-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/cs.po` & `trytond_sale_stock_quantity-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/de.po` & `trytond_sale_stock_quantity-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/es.po` & `trytond_sale_stock_quantity-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/es_419.po` & `trytond_sale_stock_quantity-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/et.po` & `trytond_sale_stock_quantity-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/fa.po` & `trytond_sale_stock_quantity-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/fi.po` & `trytond_sale_stock_quantity-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/fr.po` & `trytond_sale_stock_quantity-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/hu.po` & `trytond_sale_stock_quantity-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/id.po` & `trytond_sale_stock_quantity-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/it.po` & `trytond_sale_stock_quantity-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/lo.po` & `trytond_sale_stock_quantity-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/lt.po` & `trytond_sale_stock_quantity-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/nl.po` & `trytond_sale_stock_quantity-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/pl.po` & `trytond_sale_stock_quantity-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/pt.po` & `trytond_sale_stock_quantity-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/ro.po` & `trytond_sale_stock_quantity-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/ru.po` & `trytond_sale_stock_quantity-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/sl.po` & `trytond_sale_stock_quantity-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/tr.po` & `trytond_sale_stock_quantity-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/uk.po` & `trytond_sale_stock_quantity-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/locale/zh_CN.po` & `trytond_sale_stock_quantity-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/message.xml` & `trytond_sale_stock_quantity-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/sale.py` & `trytond_sale_stock_quantity-7.2.0/sale.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,20 @@
 from collections import defaultdict
 from itertools import groupby
 from operator import attrgetter
 
 from trytond.i18n import gettext
 from trytond.model import ModelView, Workflow, fields
 from trytond.pool import Pool, PoolMeta
-from trytond.tools import grouped_slice
+from trytond.tools import grouped_slice, sortable_values
 from trytond.transaction import Transaction
 
 from .exceptions import StockQuantityError, StockQuantityWarning
 
 
-def sortable_values(func):
-    def wrapper(*args, **kwargs):
-        result = list(func(*args, **kwargs))
-        for i, value in enumerate(list(result)):
-            result[i] = (value is None, value)
-        return result
-    return wrapper
-
-
 class Sale(metaclass=PoolMeta):
     __name__ = 'sale.sale'
 
     @classmethod
     @ModelView.button
     @Workflow.transition('quotation')
     def quote(cls, sales):
```

### Comparing `trytond_sale_stock_quantity-7.0.1/sale.xml` & `trytond_sale_stock_quantity-7.2.0/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/setup.py` & `trytond_sale_stock_quantity-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/tests/scenario_sale_stock_quantity.rst` & `trytond_sale_stock_quantity-7.2.0/tests/scenario_sale_stock_quantity.rst`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 Sale Stock Quantity
 ===================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard, Report
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_fiscalyear, \
-    ...     create_chart, get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     set_fiscalyear_invoice_sequences, create_payment_term
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import (
+    ...     create_chart, create_fiscalyear, get_accounts)
+    >>> from trytond.modules.account_invoice.tests.tools import (
+    ...     create_payment_term, set_fiscalyear_invoice_sequences)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.modules.stock.exceptions import InventoryFutureWarning
+    >>> from trytond.tests.tools import activate_modules
 
     >>> today = dt.date.today()
     >>> later = today + dt.timedelta(days=2)
 
 Activate modules::
 
     >>> config = activate_modules(['sale_stock_quantity', 'stock_supply'])
@@ -134,15 +134,15 @@
     >>> sale.party = customer
     >>> sale.payment_term = payment_term
     >>> sale_line = sale.lines.new()
     >>> sale_line.product = product
     >>> sale_line.quantity = 2.0
     >>> len(sale_line.notifications())
     0
-    >>> sale.click('quote') # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> sale.click('quote')
     Traceback (most recent call last):
         ...
     StockQuantityWarning: ...
 
 Clean sales::
 
     >>> Sale.delete(Sale.find([]))
@@ -153,15 +153,15 @@
     >>> sale.party = customer
     >>> sale.payment_term = payment_term
     >>> sale_line = sale.lines.new()
     >>> sale_line.product = product
     >>> sale_line.quantity = 6.0
     >>> len(sale_line.notifications())
     1
-    >>> sale.click('quote') # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> sale.click('quote')
     Traceback (most recent call last):
         ...
     StockQuantityWarning: ...
     >>> sale.delete()
 
 Make an inventory of 3 products in 2 days::
 
@@ -183,15 +183,15 @@
 
     >>> sale = Sale()
     >>> sale.party = customer
     >>> sale.payment_term = payment_term
     >>> sale_line = sale.lines.new()
     >>> sale_line.product = product
     >>> sale_line.quantity = 4.0
-    >>> sale.click('quote') # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> sale.click('quote')
     Traceback (most recent call last):
         ...
     StockQuantityWarning: ...
     >>> sale.delete()
 
 Sale 2 products with enough forecast::
```

### Comparing `trytond_sale_stock_quantity-7.0.1/tox.ini` & `trytond_sale_stock_quantity-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale_stock_quantity-7.0.1/trytond_sale_stock_quantity.egg-info/PKG-INFO` & `trytond_sale_stock_quantity-7.2.0/trytond_sale_stock_quantity.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_sale_stock_quantity
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module to add stock warning on sale
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
@@ -48,21 +48,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_stock_supply<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_stock_supply<7.3,>=7.2; extra == "test"
 
 Sale Stock Quantity
 ###################
 
 The sale_stock_quantity module check the stock quantity of the products when
 quoting a sale. The check will warn the user if the forecast quantity at the
 sale date (and further dates until next supply) is lower than the quantity sold
```

### Comparing `trytond_sale_stock_quantity-7.0.1/trytond_sale_stock_quantity.egg-info/SOURCES.txt` & `trytond_sale_stock_quantity-7.2.0/trytond_sale_stock_quantity.egg-info/SOURCES.txt`

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
 exceptions.py
```

