# Comparing `tmp/trytond_stock_secondary_unit-7.0.0.tar.gz` & `tmp/trytond_stock_secondary_unit-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_secondary_unit-7.0.0.tar", last modified: Mon Oct 30 17:43:41 2023, max compression
+gzip compressed data, was "trytond_stock_secondary_unit-7.2.0.tar", last modified: Mon Apr 29 15:52:47 2024, max compression
```

## Comparing `trytond_stock_secondary_unit-7.0.0.tar` & `trytond_stock_secondary_unit-7.2.0.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:41.459397 trytond_stock_secondary_unit-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-10-22 17:23:27.000000 trytond_stock_secondary_unit-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      897 2023-10-30 17:15:21.000000 trytond_stock_secondary_unit-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:15:20.000000 trytond_stock_secondary_unit-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2507 2023-10-30 17:43:41.459397 trytond_stock_secondary_unit-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-10-07 15:40:36.000000 trytond_stock_secondary_unit-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:41.456064 trytond_stock_secondary_unit-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2821 2023-10-22 17:23:27.000000 trytond_stock_secondary_unit-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:27.000000 trytond_stock_secondary_unit-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:41.456064 trytond_stock_secondary_unit-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)      916 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)      880 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)      922 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)      920 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)      862 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      921 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      747 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-10-30 16:47:45.000000 trytond_stock_secondary_unit-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:43:41.459397 trytond_stock_secondary_unit-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4396 2023-10-27 17:38:49.000000 trytond_stock_secondary_unit-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6752 2023-10-24 07:56:52.000000 trytond_stock_secondary_unit-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1488 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:41.456064 trytond_stock_secondary_unit-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_stock_secondary_unit-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-10-30 17:15:17.000000 trytond_stock_secondary_unit-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:41.456064 trytond_stock_secondary_unit-7.0.0/trytond_stock_secondary_unit.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2507 2023-10-30 17:43:41.000000 trytond_stock_secondary_unit-7.0.0/trytond_stock_secondary_unit.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1465 2023-10-30 17:43:41.000000 trytond_stock_secondary_unit-7.0.0/trytond_stock_secondary_unit.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:43:41.000000 trytond_stock_secondary_unit-7.0.0/trytond_stock_secondary_unit.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2023-10-30 17:43:41.000000 trytond_stock_secondary_unit-7.0.0/trytond_stock_secondary_unit.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_stock_secondary_unit-7.0.0/trytond_stock_secondary_unit.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-10-30 17:43:41.000000 trytond_stock_secondary_unit-7.0.0/trytond_stock_secondary_unit.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:43:41.000000 trytond_stock_secondary_unit-7.0.0/trytond_stock_secondary_unit.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:41.456064 trytond_stock_secondary_unit-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.0.0/view/stock_move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.0.0/view/stock_move_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:47.993362 trytond_stock_secondary_unit-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      998 2024-04-29 15:28:55.000000 trytond_stock_secondary_unit-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:28:55.000000 trytond_stock_secondary_unit-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2507 2024-04-29 15:52:47.993362 trytond_stock_secondary_unit-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-02-04 18:51:26.000000 trytond_stock_secondary_unit-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:47.990028 trytond_stock_secondary_unit-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3083 2024-04-27 16:30:39.000000 trytond_stock_secondary_unit-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      141 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:36.000000 trytond_stock_secondary_unit-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:47.993362 trytond_stock_secondary_unit-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      916 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      880 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      922 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      920 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      862 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      921 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      908 2024-04-29 13:17:17.000000 trytond_stock_secondary_unit-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-27 16:43:28.000000 trytond_stock_secondary_unit-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:52:47.996695 trytond_stock_secondary_unit-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4396 2024-03-17 11:01:36.000000 trytond_stock_secondary_unit-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6752 2024-02-04 18:51:26.000000 trytond_stock_secondary_unit-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1488 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:47.993362 trytond_stock_secondary_unit-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:36.000000 trytond_stock_secondary_unit-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:28:51.000000 trytond_stock_secondary_unit-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:47.993362 trytond_stock_secondary_unit-7.2.0/trytond_stock_secondary_unit.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2507 2024-04-29 15:52:47.000000 trytond_stock_secondary_unit-7.2.0/trytond_stock_secondary_unit.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1447 2024-04-29 15:52:47.000000 trytond_stock_secondary_unit-7.2.0/trytond_stock_secondary_unit.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:52:47.000000 trytond_stock_secondary_unit-7.2.0/trytond_stock_secondary_unit.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:52:47.000000 trytond_stock_secondary_unit-7.2.0/trytond_stock_secondary_unit.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:05.000000 trytond_stock_secondary_unit-7.2.0/trytond_stock_secondary_unit.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2024-04-29 15:52:47.000000 trytond_stock_secondary_unit-7.2.0/trytond_stock_secondary_unit.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:52:47.000000 trytond_stock_secondary_unit-7.2.0/trytond_stock_secondary_unit.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:47.993362 trytond_stock_secondary_unit-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.2.0/view/stock_move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_stock_secondary_unit-7.2.0/view/stock_move_tree.xml
```

### Comparing `trytond_stock_secondary_unit-7.0.0/CHANGELOG` & `trytond_stock_secondary_unit-7.2.0/CHANGELOG`

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

### Comparing `trytond_stock_secondary_unit-7.0.0/LICENSE` & `trytond_stock_secondary_unit-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/PKG-INFO` & `trytond_stock_secondary_unit-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_secondary_unit
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add a secondary unit on stock move
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
@@ -46,17 +46,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Stock Secondary Unit Module
 ###########################
 
 The stock secondary unit module adds a secondary unit of measure on the stock
 move.
```

### Comparing `trytond_stock_secondary_unit-7.0.0/doc/conf.py` & `trytond_stock_secondary_unit-7.2.0/doc/conf.py`

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

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/bg.po` & `trytond_stock_secondary_unit-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/ca.po` & `trytond_stock_secondary_unit-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/cs.po` & `trytond_stock_secondary_unit-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/de.po` & `trytond_stock_secondary_unit-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/es.po` & `trytond_stock_secondary_unit-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/es_419.po` & `trytond_stock_secondary_unit-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/et.po` & `trytond_stock_secondary_unit-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/fa.po` & `trytond_stock_secondary_unit-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/fi.po` & `trytond_stock_secondary_unit-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/fr.po` & `trytond_stock_secondary_unit-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/hu.po` & `trytond_stock_secondary_unit-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/id.po` & `trytond_stock_secondary_unit-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/it.po` & `trytond_stock_secondary_unit-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/lo.po` & `trytond_stock_secondary_unit-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/lt.po` & `trytond_stock_secondary_unit-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/nl.po` & `trytond_stock_secondary_unit-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/pl.po` & `trytond_stock_secondary_unit-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/pt.po` & `trytond_stock_secondary_unit-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/ro.po` & `trytond_stock_secondary_unit-7.2.0/locale/ru.po`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 msgctxt "field:stock.move,secondary_unit:"
 msgid "Secondary Unit"
 msgstr ""
 
 msgctxt "field:stock.move,secondary_unit_price:"
 msgid "Secondary Unit Price"
-msgstr "Preţ Unitate Secundara"
+msgstr ""
 
 msgctxt "help:stock.move,product_secondary_uom_category:"
 msgid "The category of secondary Unit of Measure for the product."
 msgstr ""
 
 msgctxt "view:stock.move:"
 msgid "Quantity:"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/ru.po` & `trytond_stock_secondary_unit-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/sl.po` & `trytond_stock_secondary_unit-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/tr.po` & `trytond_stock_secondary_unit-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/locale/uk.po` & `trytond_stock_secondary_unit-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/setup.py` & `trytond_stock_secondary_unit-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/stock.py` & `trytond_stock_secondary_unit-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/stock.xml` & `trytond_stock_secondary_unit-7.2.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/tox.ini` & `trytond_stock_secondary_unit-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_secondary_unit-7.0.0/trytond_stock_secondary_unit.egg-info/PKG-INFO` & `trytond_stock_secondary_unit-7.2.0/trytond_stock_secondary_unit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-stock-secondary-unit
-Version: 7.0.0
+Name: trytond_stock_secondary_unit
+Version: 7.2.0
 Summary: Tryton module to add a secondary unit on stock move
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
@@ -46,17 +46,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
 
 Stock Secondary Unit Module
 ###########################
 
 The stock secondary unit module adds a secondary unit of measure on the stock
 move.
```

### Comparing `trytond_stock_secondary_unit-7.0.0/trytond_stock_secondary_unit.egg-info/SOURCES.txt` & `trytond_stock_secondary_unit-7.2.0/trytond_stock_secondary_unit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

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

### Comparing `trytond_stock_secondary_unit-7.0.0/view/stock_move_form.xml` & `trytond_stock_secondary_unit-7.2.0/view/stock_move_form.xml`

 * *Files identical despite different names*

