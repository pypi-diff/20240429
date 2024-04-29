# Comparing `tmp/trytond_stock_assign_manual-7.0.0.tar.gz` & `tmp/trytond_stock_assign_manual-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_assign_manual-7.0.0.tar", last modified: Mon Oct 30 17:41:15 2023, max compression
+gzip compressed data, was "trytond_stock_assign_manual-7.2.0.tar", last modified: Mon Apr 29 15:50:44 2024, max compression
```

## Comparing `trytond_stock_assign_manual-7.0.0.tar` & `trytond_stock_assign_manual-7.2.0.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:15.562034 trytond_stock_assign_manual-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      219 2023-10-22 17:23:23.000000 trytond_stock_assign_manual-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      760 2023-10-30 17:13:59.000000 trytond_stock_assign_manual-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-10-30 17:13:58.000000 trytond_stock_assign_manual-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2762 2023-10-30 17:41:15.562034 trytond_stock_assign_manual-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      805 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:15.562034 trytond_stock_assign_manual-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2820 2023-10-22 17:23:23.000000 trytond_stock_assign_manual-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:23.000000 trytond_stock_assign_manual-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:15.558701 trytond_stock_assign_manual-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4822 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5004 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4846 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4869 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3876 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4886 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3867 2023-10-28 12:11:26.000000 trytond_stock_assign_manual-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      770 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.0.0/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1070 2023-10-27 17:38:49.000000 trytond_stock_assign_manual-7.0.0/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:41:15.562034 trytond_stock_assign_manual-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4619 2023-10-27 17:38:49.000000 trytond_stock_assign_manual-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15512 2023-10-07 17:14:58.000000 trytond_stock_assign_manual-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5170 2023-10-27 17:38:49.000000 trytond_stock_assign_manual-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:15.558701 trytond_stock_assign_manual-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6214 2023-10-07 17:14:58.000000 trytond_stock_assign_manual-7.0.0/tests/scenario_stock_assign_manual.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_stock_assign_manual-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      133 2023-10-30 17:13:55.000000 trytond_stock_assign_manual-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:15.562034 trytond_stock_assign_manual-7.0.0/trytond_stock_assign_manual.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2762 2023-10-30 17:41:15.000000 trytond_stock_assign_manual-7.0.0/trytond_stock_assign_manual.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1946 2023-10-30 17:41:15.000000 trytond_stock_assign_manual-7.0.0/trytond_stock_assign_manual.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:41:15.000000 trytond_stock_assign_manual-7.0.0/trytond_stock_assign_manual.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       76 2023-10-30 17:41:15.000000 trytond_stock_assign_manual-7.0.0/trytond_stock_assign_manual.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_stock_assign_manual-7.0.0/trytond_stock_assign_manual.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       97 2023-10-30 17:41:15.000000 trytond_stock_assign_manual-7.0.0/trytond_stock_assign_manual.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:41:15.000000 trytond_stock_assign_manual-7.0.0/trytond_stock_assign_manual.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:41:15.562034 trytond_stock_assign_manual-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.0.0/view/shipment_assign_manual_show_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      432 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.0.0/view/shipment_assigned_move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.0.0/view/shipment_assigned_move_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.0.0/view/shipment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.0.0/view/shipment_unassign_manual_show_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:44.019937 trytond_stock_assign_manual-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      861 2024-04-29 15:27:23.000000 trytond_stock_assign_manual-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:27:23.000000 trytond_stock_assign_manual-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2762 2024-04-29 15:50:44.019937 trytond_stock_assign_manual-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      805 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:44.013271 trytond_stock_assign_manual-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3082 2024-04-27 16:30:39.000000 trytond_stock_assign_manual-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:31.000000 trytond_stock_assign_manual-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:44.016604 trytond_stock_assign_manual-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4822 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5004 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4846 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4869 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3876 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4886 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3867 2024-04-27 16:43:27.000000 trytond_stock_assign_manual-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      770 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.2.0/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1047 2024-04-27 16:30:39.000000 trytond_stock_assign_manual-7.2.0/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:50:44.019937 trytond_stock_assign_manual-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4619 2024-03-17 11:01:36.000000 trytond_stock_assign_manual-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15512 2024-02-04 18:51:26.000000 trytond_stock_assign_manual-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5101 2024-04-27 16:30:39.000000 trytond_stock_assign_manual-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:44.016604 trytond_stock_assign_manual-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6217 2024-04-22 12:14:36.000000 trytond_stock_assign_manual-7.2.0/tests/scenario_stock_assign_manual.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:31.000000 trytond_stock_assign_manual-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      133 2024-04-29 15:27:19.000000 trytond_stock_assign_manual-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:44.016604 trytond_stock_assign_manual-7.2.0/trytond_stock_assign_manual.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2762 2024-04-29 15:50:43.000000 trytond_stock_assign_manual-7.2.0/trytond_stock_assign_manual.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1928 2024-04-29 15:50:43.000000 trytond_stock_assign_manual-7.2.0/trytond_stock_assign_manual.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:50:43.000000 trytond_stock_assign_manual-7.2.0/trytond_stock_assign_manual.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       76 2024-04-29 15:50:43.000000 trytond_stock_assign_manual-7.2.0/trytond_stock_assign_manual.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_stock_assign_manual-7.2.0/trytond_stock_assign_manual.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       97 2024-04-29 15:50:43.000000 trytond_stock_assign_manual-7.2.0/trytond_stock_assign_manual.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:50:43.000000 trytond_stock_assign_manual-7.2.0/trytond_stock_assign_manual.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:50:44.016604 trytond_stock_assign_manual-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      368 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.2.0/view/shipment_assign_manual_show_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      432 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.2.0/view/shipment_assigned_move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.2.0/view/shipment_assigned_move_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.2.0/view/shipment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_stock_assign_manual-7.2.0/view/shipment_unassign_manual_show_form.xml
```

### Comparing `trytond_stock_assign_manual-7.0.0/CHANGELOG` & `trytond_stock_assign_manual-7.2.0/CHANGELOG`

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

### Comparing `trytond_stock_assign_manual-7.0.0/COPYRIGHT` & `trytond_stock_assign_manual-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2020-2023 Cédric Krier
+Copyright (C) 2020-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_assign_manual-7.0.0/LICENSE` & `trytond_stock_assign_manual-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/PKG-INFO` & `trytond_stock_assign_manual-7.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_stock_assign_manual
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to assign manually stock move
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
@@ -47,19 +47,19 @@
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
-Requires-Dist: trytond_production<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_production<7.3,>=7.2; extra == "test"
 
 Stock Assign Manual Module
 ##########################
 
 The Stock Assign Manual module adds a wizard on shipments and production that
 allows you to decide from which precise location to pick products.
```

### Comparing `trytond_stock_assign_manual-7.0.0/__init__.py` & `trytond_stock_assign_manual-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/doc/conf.py` & `trytond_stock_assign_manual-7.2.0/doc/conf.py`

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

### Comparing `trytond_stock_assign_manual-7.0.0/locale/bg.po` & `trytond_stock_assign_manual-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/ca.po` & `trytond_stock_assign_manual-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/cs.po` & `trytond_stock_assign_manual-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/de.po` & `trytond_stock_assign_manual-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/es.po` & `trytond_stock_assign_manual-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/es_419.po` & `trytond_stock_assign_manual-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/et.po` & `trytond_stock_assign_manual-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/fa.po` & `trytond_stock_assign_manual-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/fi.po` & `trytond_stock_assign_manual-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/fr.po` & `trytond_stock_assign_manual-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/hu.po` & `trytond_stock_assign_manual-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/id.po` & `trytond_stock_assign_manual-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/it.po` & `trytond_stock_assign_manual-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/lo.po` & `trytond_stock_assign_manual-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/lt.po` & `trytond_stock_assign_manual-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/nl.po` & `trytond_stock_assign_manual-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/pl.po` & `trytond_stock_assign_manual-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/pt.po` & `trytond_stock_assign_manual-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/ro.po` & `trytond_stock_assign_manual-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/ru.po` & `trytond_stock_assign_manual-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/sl.po` & `trytond_stock_assign_manual-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/tr.po` & `trytond_stock_assign_manual-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/uk.po` & `trytond_stock_assign_manual-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/locale/zh_CN.po` & `trytond_stock_assign_manual-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/message.xml` & `trytond_stock_assign_manual-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/production.py` & `trytond_stock_assign_manual-7.2.0/production.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/production.xml` & `trytond_stock_assign_manual-7.2.0/production.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_stock_assign_manual-7.0.0/production.xml` & `trytond_stock_assign_manual-7.2.0/production.xml`

```diff
@@ -5,17 +5,17 @@
   <data depends="production">
     <record model="ir.ui.view" id="production_view_form">
       <field name="model">production</field>
       <field name="inherit" ref="production.production_view_form"/>
       <field name="name">shipment_form</field>
     </record>
     <record model="ir.model.button" id="production_assign_manual_wizard_button">
+      <field name="model">production</field>
       <field name="name">assign_manual_wizard</field>
       <field name="string">Manual Assign</field>
-      <field name="model" search="[('model', '=', 'production')]"/>
     </record>
     <record model="ir.action.wizard" id="wizard_production_assign_manual">
       <field name="name">Manual Assign Production</field>
       <field name="wiz_name">stock.shipment.assign.manual</field>
       <field name="model">production</field>
     </record>
   </data>
```

### Comparing `trytond_stock_assign_manual-7.0.0/setup.py` & `trytond_stock_assign_manual-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/stock.py` & `trytond_stock_assign_manual-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/stock.xml` & `trytond_stock_assign_manual-7.2.0/stock.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_stock_assign_manual-7.0.0/stock.xml` & `trytond_stock_assign_manual-7.2.0/stock.xml`

```diff
@@ -5,37 +5,37 @@
   <data>
     <record model="ir.ui.view" id="shipment_in_return_view_form">
       <field name="model">stock.shipment.in.return</field>
       <field name="inherit" ref="stock.shipment_in_return_view_form"/>
       <field name="name">shipment_form</field>
     </record>
     <record model="ir.model.button" id="shipment_in_return_assign_manual_wizard_button">
+      <field name="model">stock.shipment.in.return</field>
       <field name="name">assign_manual_wizard</field>
       <field name="string">Manual Assign</field>
-      <field name="model" search="[('model', '=', 'stock.shipment.in.return')]"/>
     </record>
     <record model="ir.ui.view" id="shipment_out_view_form">
       <field name="model">stock.shipment.out</field>
       <field name="inherit" ref="stock.shipment_out_view_form"/>
       <field name="name">shipment_form</field>
     </record>
     <record model="ir.model.button" id="shipment_out_assign_manual_wizard_button">
+      <field name="model">stock.shipment.out</field>
       <field name="name">assign_manual_wizard</field>
       <field name="string">Manual Assign</field>
-      <field name="model" search="[('model', '=', 'stock.shipment.out')]"/>
     </record>
     <record model="ir.ui.view" id="shipment_internal_view_form">
       <field name="model">stock.shipment.internal</field>
       <field name="inherit" ref="stock.shipment_internal_view_form"/>
       <field name="name">shipment_form</field>
     </record>
     <record model="ir.model.button" id="shipment_internal_assign_manual_wizard_button">
+      <field name="model">stock.shipment.internal</field>
       <field name="name">assign_manual_wizard</field>
       <field name="string">Manual Assign</field>
-      <field name="model" search="[('model', '=', 'stock.shipment.internal')]"/>
     </record>
     <record model="ir.action.wizard" id="wizard_shipment_in_return_assign_manual">
       <field name="name">Manual Assign Supplier Return Shipment</field>
       <field name="wiz_name">stock.shipment.assign.manual</field>
       <field name="model">stock.shipment.in.return</field>
     </record>
     <record model="ir.action.wizard" id="wizard_shipment_out_assign_manual">
```

### Comparing `trytond_stock_assign_manual-7.0.0/tests/scenario_stock_assign_manual.rst` & `trytond_stock_assign_manual-7.2.0/tests/scenario_stock_assign_manual.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Stock Assign Manual Scenario
 ============================
 
 Imports::
 
     >>> import json
     >>> from decimal import Decimal
+
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate stock_assign_manual::
 
     >>> config = activate_modules('stock_assign_manual')
 
 Create company::
 
@@ -95,16 +95,15 @@
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
 
 Assign manually the first move::
 
     >>> assign_manual = shipment.click('assign_manual_wizard')
-    >>> assign_manual.form.move == shipment.inventory_moves[0]
-    True
+    >>> assertEqual(assign_manual.form.move, shipment.inventory_moves[0])
     >>> assign_manual.form.move_quantity
     2.0
     >>> assign_manual.form.place = json.dumps([storage_loc.id, product.id])
     >>> assign_manual.execute('assign')
     >>> assign_manual.form.move_quantity
     1.0
     >>> assign_manual.form.place = json.dumps([storage_loc2.id, product.id])
@@ -119,17 +118,16 @@
 
     >>> shipment.state
     'waiting'
     >>> sorted([m.state for m in shipment.inventory_moves])
     ['assigned', 'assigned', 'draft']
     >>> [m.quantity for m in shipment.inventory_moves if m.state == 'assigned']
     [1.0, 1.0]
-    >>> {m.from_location for m in shipment.inventory_moves
-    ...     if m.state == 'assigned'} == {storage_loc, storage_loc2}
-    True
+    >>> assertEqual({m.from_location for m in shipment.inventory_moves
+    ...     if m.state == 'assigned'}, {storage_loc, storage_loc2})
 
 Assign manually remaining move::
 
     >>> assign_manual = shipment.click('assign_manual_wizard')
     >>> assign_manual.form.place = json.dumps([storage_loc2.id, product.id])
     >>> assign_manual.execute('assign')
```

### Comparing `trytond_stock_assign_manual-7.0.0/tox.ini` & `trytond_stock_assign_manual-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_assign_manual-7.0.0/trytond_stock_assign_manual.egg-info/PKG-INFO` & `trytond_stock_assign_manual-7.2.0/trytond_stock_assign_manual.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-stock-assign-manual
-Version: 7.0.0
+Name: trytond_stock_assign_manual
+Version: 7.2.0
 Summary: Tryton module to assign manually stock move
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
@@ -47,19 +47,19 @@
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
-Requires-Dist: trytond_production<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_production<7.3,>=7.2; extra == "test"
 
 Stock Assign Manual Module
 ##########################
 
 The Stock Assign Manual module adds a wizard on shipments and production that
 allows you to decide from which precise location to pick products.
```

### Comparing `trytond_stock_assign_manual-7.0.0/trytond_stock_assign_manual.egg-info/SOURCES.txt` & `trytond_stock_assign_manual-7.2.0/trytond_stock_assign_manual.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

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

