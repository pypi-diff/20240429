# Comparing `tmp/trytond_stock_lot_sled-7.0.0.tar.gz` & `tmp/trytond_stock_lot_sled-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_lot_sled-7.0.0.tar", last modified: Mon Oct 30 17:42:06 2023, max compression
+gzip compressed data, was "trytond_stock_lot_sled-7.2.0.tar", last modified: Mon Apr 29 15:51:28 2024, max compression
```

## Comparing `trytond_stock_lot_sled-7.0.0.tar` & `trytond_stock_lot_sled-7.2.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:06.702278 trytond_stock_lot_sled-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-10-22 17:23:24.000000 trytond_stock_lot_sled-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1672 2023-10-30 17:14:30.000000 trytond_stock_lot_sled-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2023-10-30 17:14:29.000000 trytond_stock_lot_sled-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_lot_sled-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2980 2023-10-30 17:42:06.702278 trytond_stock_lot_sled-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-01-16 14:00:21.000000 trytond_stock_lot_sled-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:06.698945 trytond_stock_lot_sled-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-10-22 17:23:24.000000 trytond_stock_lot_sled-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-01-16 14:00:21.000000 trytond_stock_lot_sled-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:24.000000 trytond_stock_lot_sled-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.0.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:06.698945 trytond_stock_lot_sled-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6070 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6264 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5262 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6523 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6340 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5726 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5733 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7054 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5262 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6650 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6292 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5462 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5563 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5670 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5262 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6435 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5743 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6376 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5240 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6414 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6021 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5262 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5240 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5472 2023-10-28 12:11:26.000000 trytond_stock_lot_sled-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      865 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1145 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:21.000000 trytond_stock_lot_sled-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:42:06.702278 trytond_stock_lot_sled-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4403 2023-10-27 17:38:49.000000 trytond_stock_lot_sled-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15229 2023-10-07 15:40:36.000000 trytond_stock_lot_sled-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1663 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:06.698945 trytond_stock_lot_sled-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6774 2023-10-07 17:14:58.000000 trytond_stock_lot_sled-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_stock_lot_sled-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      126 2023-10-30 17:14:26.000000 trytond_stock_lot_sled-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:06.702278 trytond_stock_lot_sled-7.0.0/trytond_stock_lot_sled.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2980 2023-10-30 17:42:06.000000 trytond_stock_lot_sled-7.0.0/trytond_stock_lot_sled.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1607 2023-10-30 17:42:06.000000 trytond_stock_lot_sled-7.0.0/trytond_stock_lot_sled.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:42:06.000000 trytond_stock_lot_sled-7.0.0/trytond_stock_lot_sled.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-10-30 17:42:06.000000 trytond_stock_lot_sled-7.0.0/trytond_stock_lot_sled.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_stock_lot_sled-7.0.0/trytond_stock_lot_sled.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      120 2023-10-30 17:42:06.000000 trytond_stock_lot_sled-7.0.0/trytond_stock_lot_sled.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:42:06.000000 trytond_stock_lot_sled-7.0.0/trytond_stock_lot_sled.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:42:06.698945 trytond_stock_lot_sled-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.0.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.0.0/view/lot_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.0.0/view/lot_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      673 2023-01-16 14:00:21.000000 trytond_stock_lot_sled-7.0.0/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:28.855431 trytond_stock_lot_sled-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1773 2024-04-29 15:27:59.000000 trytond_stock_lot_sled-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2024-04-29 15:27:59.000000 trytond_stock_lot_sled-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock_lot_sled-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2980 2024-04-29 15:51:28.855431 trytond_stock_lot_sled-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-01-16 14:00:21.000000 trytond_stock_lot_sled-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:28.852098 trytond_stock_lot_sled-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_stock_lot_sled-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-01-16 14:00:21.000000 trytond_stock_lot_sled-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:33.000000 trytond_stock_lot_sled-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:28.852098 trytond_stock_lot_sled-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6070 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6264 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5262 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6523 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6340 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5726 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5733 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7054 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5262 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6650 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6292 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5462 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5563 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5670 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5262 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6435 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5743 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6376 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5240 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6414 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6021 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5262 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5240 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5472 2024-04-27 16:43:27.000000 trytond_stock_lot_sled-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      865 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1145 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-01-16 14:00:21.000000 trytond_stock_lot_sled-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:51:28.855431 trytond_stock_lot_sled-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4403 2024-03-17 11:01:36.000000 trytond_stock_lot_sled-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15229 2024-04-22 12:01:28.000000 trytond_stock_lot_sled-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1663 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:28.852098 trytond_stock_lot_sled-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6774 2024-02-04 18:51:26.000000 trytond_stock_lot_sled-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:33.000000 trytond_stock_lot_sled-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      126 2024-04-29 15:27:54.000000 trytond_stock_lot_sled-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:28.855431 trytond_stock_lot_sled-7.2.0/trytond_stock_lot_sled.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2980 2024-04-29 15:51:28.000000 trytond_stock_lot_sled-7.2.0/trytond_stock_lot_sled.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1589 2024-04-29 15:51:28.000000 trytond_stock_lot_sled-7.2.0/trytond_stock_lot_sled.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:51:28.000000 trytond_stock_lot_sled-7.2.0/trytond_stock_lot_sled.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:51:28.000000 trytond_stock_lot_sled-7.2.0/trytond_stock_lot_sled.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_stock_lot_sled-7.2.0/trytond_stock_lot_sled.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      120 2024-04-29 15:51:28.000000 trytond_stock_lot_sled-7.2.0/trytond_stock_lot_sled.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:51:28.000000 trytond_stock_lot_sled-7.2.0/trytond_stock_lot_sled.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:51:28.855431 trytond_stock_lot_sled-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.2.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      465 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.2.0/view/lot_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-04-15 07:12:15.000000 trytond_stock_lot_sled-7.2.0/view/lot_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      673 2023-01-16 14:00:21.000000 trytond_stock_lot_sled-7.2.0/view/template_form.xml
```

### Comparing `trytond_stock_lot_sled-7.0.0/CHANGELOG` & `trytond_stock_lot_sled-7.2.0/CHANGELOG`

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

### Comparing `trytond_stock_lot_sled-7.0.0/COPYRIGHT` & `trytond_stock_lot_sled-7.2.0/COPYRIGHT`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2014-2023 Cédric Krier.
-Copyright (C) 2014-2023 B2CK SPRL.
+Copyright (C) 2014-2024 Cédric Krier.
+Copyright (C) 2014-2024 B2CK SPRL.
 Copyright (C) 2013-2015 NaN·tic
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `trytond_stock_lot_sled-7.0.0/LICENSE` & `trytond_stock_lot_sled-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/PKG-INFO` & `trytond_stock_lot_sled-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_lot_sled
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module for shelf life expiration date of product lots
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
@@ -49,18 +49,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.5
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_lot<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_lot<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Stock Lot Shelf Life Expiration Date
 ####################################
 
 The stock_lot_sled module adds two fields on lot of products:
```

### Comparing `trytond_stock_lot_sled-7.0.0/__init__.py` & `trytond_stock_lot_sled-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/doc/conf.py` & `trytond_stock_lot_sled-7.2.0/doc/conf.py`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_stock_lot_sled-7.0.0/locale/bg.po` & `trytond_stock_lot_sled-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/ca.po` & `trytond_stock_lot_sled-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/cs.po` & `trytond_stock_lot_sled-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/de.po` & `trytond_stock_lot_sled-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/es.po` & `trytond_stock_lot_sled-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/es_419.po` & `trytond_stock_lot_sled-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/et.po` & `trytond_stock_lot_sled-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/fa.po` & `trytond_stock_lot_sled-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/fi.po` & `trytond_stock_lot_sled-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/fr.po` & `trytond_stock_lot_sled-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/hu.po` & `trytond_stock_lot_sled-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/id.po` & `trytond_stock_lot_sled-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/it.po` & `trytond_stock_lot_sled-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/lo.po` & `trytond_stock_lot_sled-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/lt.po` & `trytond_stock_lot_sled-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/nl.po` & `trytond_stock_lot_sled-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/pl.po` & `trytond_stock_lot_sled-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/pt.po` & `trytond_stock_lot_sled-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/ro.po` & `trytond_stock_lot_sled-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/ru.po` & `trytond_stock_lot_sled-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/sl.po` & `trytond_stock_lot_sled-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/tr.po` & `trytond_stock_lot_sled-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/uk.po` & `trytond_stock_lot_sled-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/locale/zh_CN.po` & `trytond_stock_lot_sled-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/message.xml` & `trytond_stock_lot_sled-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/product.py` & `trytond_stock_lot_sled-7.2.0/product.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/setup.py` & `trytond_stock_lot_sled-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/stock.py` & `trytond_stock_lot_sled-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/stock.xml` & `trytond_stock_lot_sled-7.2.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/tests/test_module.py` & `trytond_stock_lot_sled-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/tox.ini` & `trytond_stock_lot_sled-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot_sled-7.0.0/trytond_stock_lot_sled.egg-info/PKG-INFO` & `trytond_stock_lot_sled-7.2.0/trytond_stock_lot_sled.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-stock-lot-sled
-Version: 7.0.0
+Name: trytond_stock_lot_sled
+Version: 7.2.0
 Summary: Tryton module for shelf life expiration date of product lots
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
@@ -49,18 +49,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.5
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_stock_lot<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_stock_lot<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Stock Lot Shelf Life Expiration Date
 ####################################
 
 The stock_lot_sled module adds two fields on lot of products:
```

### Comparing `trytond_stock_lot_sled-7.0.0/trytond_stock_lot_sled.egg-info/SOURCES.txt` & `trytond_stock_lot_sled-7.2.0/trytond_stock_lot_sled.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

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

### Comparing `trytond_stock_lot_sled-7.0.0/view/template_form.xml` & `trytond_stock_lot_sled-7.2.0/view/template_form.xml`

 * *Files identical despite different names*
