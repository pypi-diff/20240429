# Comparing `tmp/trytond_timesheet_cost-7.0.0.tar.gz` & `tmp/trytond_timesheet_cost-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_timesheet_cost-7.0.0.tar", last modified: Mon Oct 30 17:44:52 2023, max compression
+gzip compressed data, was "trytond_timesheet_cost-7.2.0.tar", last modified: Mon Apr 29 15:53:52 2024, max compression
```

## Comparing `trytond_timesheet_cost-7.0.0.tar` & `trytond_timesheet_cost-7.2.0.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:52.093067 trytond_timesheet_cost-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-10-22 17:23:29.000000 trytond_timesheet_cost-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     1886 2023-10-30 17:16:05.000000 trytond_timesheet_cost-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:16:05.000000 trytond_timesheet_cost-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_timesheet_cost-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2582 2023-10-30 17:44:52.093067 trytond_timesheet_cost-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      101 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.0.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.0.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2653 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.0.0/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:52.089734 trytond_timesheet_cost-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-10-22 17:23:29.000000 trytond_timesheet_cost-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      101 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:29.000000 trytond_timesheet_cost-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:52.089734 trytond_timesheet_cost-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1491 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1366 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1420 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1398 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1307 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1389 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1366 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1121 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1341 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1338 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1293 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1430 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1293 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1639 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1344 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1432 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1127 2023-10-28 12:11:27.000000 trytond_timesheet_cost-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:44:52.093067 trytond_timesheet_cost-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4288 2023-10-27 17:38:49.000000 trytond_timesheet_cost-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:52.089734 trytond_timesheet_cost-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1899 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1438 2023-08-13 15:26:13.000000 trytond_timesheet_cost-7.0.0/timesheet.py
--rw-r--r--   0 ced       (1000) ced       (1000)      989 2023-01-16 14:00:21.000000 trytond_timesheet_cost-7.0.0/timesheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_timesheet_cost-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      130 2023-10-30 17:16:01.000000 trytond_timesheet_cost-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:52.093067 trytond_timesheet_cost-7.0.0/trytond_timesheet_cost.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2582 2023-10-30 17:44:51.000000 trytond_timesheet_cost-7.0.0/trytond_timesheet_cost.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1599 2023-10-30 17:44:52.000000 trytond_timesheet_cost-7.0.0/trytond_timesheet_cost.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:44:51.000000 trytond_timesheet_cost-7.0.0/trytond_timesheet_cost.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       66 2023-10-30 17:44:51.000000 trytond_timesheet_cost-7.0.0/trytond_timesheet_cost.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_timesheet_cost-7.0.0/trytond_timesheet_cost.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      112 2023-10-30 17:44:51.000000 trytond_timesheet_cost-7.0.0/trytond_timesheet_cost.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:44:51.000000 trytond_timesheet_cost-7.0.0/trytond_timesheet_cost.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:44:52.089734 trytond_timesheet_cost-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-01-16 14:00:21.000000 trytond_timesheet_cost-7.0.0/view/employee_cost_price_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-01-16 14:00:21.000000 trytond_timesheet_cost-7.0.0/view/employee_cost_price_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.0.0/view/employee_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:52.358345 trytond_timesheet_cost-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1987 2024-04-29 15:29:46.000000 trytond_timesheet_cost-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:29:45.000000 trytond_timesheet_cost-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_timesheet_cost-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2582 2024-04-29 15:53:52.358345 trytond_timesheet_cost-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      101 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.2.0/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2529 2024-04-27 16:30:39.000000 trytond_timesheet_cost-7.2.0/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:52.351678 trytond_timesheet_cost-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3077 2024-04-27 16:30:39.000000 trytond_timesheet_cost-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      101 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:38.000000 trytond_timesheet_cost-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:52.355012 trytond_timesheet_cost-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1491 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1366 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1420 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1398 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1343 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1307 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1389 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1366 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1121 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1341 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1338 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1293 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1430 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1293 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1639 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1344 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1432 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1127 2024-04-27 16:43:28.000000 trytond_timesheet_cost-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      409 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:53:52.358345 trytond_timesheet_cost-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4288 2024-03-17 11:01:36.000000 trytond_timesheet_cost-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:52.355012 trytond_timesheet_cost-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1899 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1438 2024-01-27 09:58:52.000000 trytond_timesheet_cost-7.2.0/timesheet.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      943 2024-04-27 16:30:39.000000 trytond_timesheet_cost-7.2.0/timesheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:38.000000 trytond_timesheet_cost-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      130 2024-04-29 15:29:41.000000 trytond_timesheet_cost-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:52.355012 trytond_timesheet_cost-7.2.0/trytond_timesheet_cost.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2582 2024-04-29 15:53:51.000000 trytond_timesheet_cost-7.2.0/trytond_timesheet_cost.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1581 2024-04-29 15:53:52.000000 trytond_timesheet_cost-7.2.0/trytond_timesheet_cost.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:53:51.000000 trytond_timesheet_cost-7.2.0/trytond_timesheet_cost.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       66 2024-04-29 15:53:51.000000 trytond_timesheet_cost-7.2.0/trytond_timesheet_cost.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_timesheet_cost-7.2.0/trytond_timesheet_cost.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      112 2024-04-29 15:53:51.000000 trytond_timesheet_cost-7.2.0/trytond_timesheet_cost.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:53:51.000000 trytond_timesheet_cost-7.2.0/trytond_timesheet_cost.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:52.355012 trytond_timesheet_cost-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-01-16 14:00:21.000000 trytond_timesheet_cost-7.2.0/view/employee_cost_price_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-01-16 14:00:21.000000 trytond_timesheet_cost-7.2.0/view/employee_cost_price_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_timesheet_cost-7.2.0/view/employee_form.xml
```

### Comparing `trytond_timesheet_cost-7.0.0/CHANGELOG` & `trytond_timesheet_cost-7.2.0/CHANGELOG`

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

### Comparing `trytond_timesheet_cost-7.0.0/COPYRIGHT` & `trytond_timesheet_cost-7.2.0/COPYRIGHT`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2008-2023 Cédric Krier.
-Copyright (C) 2008-2023 B2CK SPRL.
+Copyright (C) 2008-2024 Cédric Krier.
+Copyright (C) 2008-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_timesheet_cost-7.0.0/LICENSE` & `trytond_timesheet_cost-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/PKG-INFO` & `trytond_timesheet_cost-7.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_timesheet_cost
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to add cost on timesheet
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
@@ -49,16 +49,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_timesheet<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_timesheet<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Timesheet Cost Module
 #####################
 
 The timesheet cost module adds cost price per employee.
```

### Comparing `trytond_timesheet_cost-7.0.0/company.py` & `trytond_timesheet_cost-7.2.0/company.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/company.xml` & `trytond_timesheet_cost-7.2.0/company.xml`

 * *Files 9% similar despite different names*

#### Comparing `trytond_timesheet_cost-7.0.0/company.xml` & `trytond_timesheet_cost-7.2.0/company.xml`

```diff
@@ -15,34 +15,36 @@
     </record>
     <record model="ir.ui.view" id="employee_view_form">
       <field name="model">company.employee</field>
       <field name="inherit" ref="company.employee_view_form"/>
       <field name="name">employee_form</field>
     </record>
     <record model="ir.model.access" id="access_employee_cost_price">
-      <field name="model" search="[('model', '=', 'company.employee_cost_price')]"/>
+      <field name="model">company.employee_cost_price</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_employee_cost_price_admin">
-      <field name="model" search="[('model', '=', 'company.employee_cost_price')]"/>
+      <field name="model">company.employee_cost_price</field>
       <field name="group" ref="company.group_employee_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.field.access" id="model_field_access_employee_cost_price">
-      <field name="field" search="[('model.model', '=', 'company.employee'), ('name', '=', 'cost_price')]"/>
+      <field name="model">company.employee</field>
+      <field name="field">cost_price</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
     </record>
     <record model="ir.model.field.access" id="model_field_access_employee_cost_price_admin">
-      <field name="field" search="[('model.model', '=', 'company.employee'), ('name', '=', 'cost_price')]"/>
+      <field name="model">company.employee</field>
+      <field name="field">cost_price</field>
       <field name="group" ref="company.group_employee_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
     </record>
   </data>
 </tryton>
```

### Comparing `trytond_timesheet_cost-7.0.0/doc/conf.py` & `trytond_timesheet_cost-7.2.0/doc/conf.py`

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

### Comparing `trytond_timesheet_cost-7.0.0/locale/bg.po` & `trytond_timesheet_cost-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/ca.po` & `trytond_timesheet_cost-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/cs.po` & `trytond_timesheet_cost-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/de.po` & `trytond_timesheet_cost-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/es.po` & `trytond_timesheet_cost-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/es_419.po` & `trytond_timesheet_cost-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/et.po` & `trytond_timesheet_cost-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/fa.po` & `trytond_timesheet_cost-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/fi.po` & `trytond_timesheet_cost-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/fr.po` & `trytond_timesheet_cost-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/hu.po` & `trytond_timesheet_cost-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/id.po` & `trytond_timesheet_cost-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/it.po` & `trytond_timesheet_cost-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/lo.po` & `trytond_timesheet_cost-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/lt.po` & `trytond_timesheet_cost-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/nl.po` & `trytond_timesheet_cost-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/pl.po` & `trytond_timesheet_cost-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/pt.po` & `trytond_timesheet_cost-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/ro.po` & `trytond_timesheet_cost-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/ru.po` & `trytond_timesheet_cost-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/sl.po` & `trytond_timesheet_cost-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/tr.po` & `trytond_timesheet_cost-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/uk.po` & `trytond_timesheet_cost-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/locale/zh_CN.po` & `trytond_timesheet_cost-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/setup.py` & `trytond_timesheet_cost-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/tests/test_module.py` & `trytond_timesheet_cost-7.2.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/timesheet.py` & `trytond_timesheet_cost-7.2.0/timesheet.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/tox.ini` & `trytond_timesheet_cost-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_timesheet_cost-7.0.0/trytond_timesheet_cost.egg-info/PKG-INFO` & `trytond_timesheet_cost-7.2.0/trytond_timesheet_cost.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-timesheet-cost
-Version: 7.0.0
+Name: trytond_timesheet_cost
+Version: 7.2.0
 Summary: Tryton module to add cost on timesheet
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
@@ -49,16 +49,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_party<7.1,>=7.0
-Requires-Dist: trytond_timesheet<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_party<7.3,>=7.2
+Requires-Dist: trytond_timesheet<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Timesheet Cost Module
 #####################
 
 The timesheet cost module adds cost price per employee.
```

### Comparing `trytond_timesheet_cost-7.0.0/trytond_timesheet_cost.egg-info/SOURCES.txt` & `trytond_timesheet_cost-7.2.0/trytond_timesheet_cost.egg-info/SOURCES.txt`

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
 company.py
```

