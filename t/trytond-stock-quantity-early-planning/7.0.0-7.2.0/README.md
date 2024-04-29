# Comparing `tmp/trytond_stock_quantity_early_planning-7.0.0.tar.gz` & `tmp/trytond_stock_quantity_early_planning-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_quantity_early_planning-7.0.0.tar", last modified: Mon Oct 30 17:43:22 2023, max compression
+gzip compressed data, was "trytond_stock_quantity_early_planning-7.2.0.tar", last modified: Mon Apr 29 15:52:32 2024, max compression
```

## Comparing `trytond_stock_quantity_early_planning-7.0.0.tar` & `trytond_stock_quantity_early_planning-7.2.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:22.535973 trytond_stock_quantity_early_planning-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-10-22 17:23:26.000000 trytond_stock_quantity_early_planning-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      891 2023-10-30 17:15:12.000000 trytond_stock_quantity_early_planning-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2023-10-30 17:15:12.000000 trytond_stock_quantity_early_planning-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2806 2023-10-30 17:43:22.535973 trytond_stock_quantity_early_planning-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      700 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:22.532640 trytond_stock_quantity_early_planning-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2830 2023-10-22 17:23:26.000000 trytond_stock_quantity_early_planning-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1692 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.0.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.0.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:26.000000 trytond_stock_quantity_early_planning-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.0.0/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:22.529307 trytond_stock_quantity_early_planning-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4526 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4531 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4557 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4575 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3865 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3823 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4490 2023-10-30 16:47:45.000000 trytond_stock_quantity_early_planning-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3810 2023-10-30 16:47:45.000000 trytond_stock_quantity_early_planning-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3798 2023-10-28 12:11:26.000000 trytond_stock_quantity_early_planning-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:43:22.535973 trytond_stock_quantity_early_planning-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4794 2023-10-27 17:38:49.000000 trytond_stock_quantity_early_planning-7.0.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21215 2023-08-13 15:26:13.000000 trytond_stock_quantity_early_planning-7.0.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6786 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.0.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:22.532640 trytond_stock_quantity_early_planning-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5182 2023-06-10 11:39:56.000000 trytond_stock_quantity_early_planning-7.0.0/tests/scenario_stock_quantity_early_planning.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4842 2023-06-10 11:39:56.000000 trytond_stock_quantity_early_planning-7.0.0/tests/scenario_stock_quantity_early_planning_incoming.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_stock_quantity_early_planning-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      110 2023-10-30 17:15:08.000000 trytond_stock_quantity_early_planning-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:22.532640 trytond_stock_quantity_early_planning-7.0.0/trytond_stock_quantity_early_planning.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2806 2023-10-30 17:43:22.000000 trytond_stock_quantity_early_planning-7.0.0/trytond_stock_quantity_early_planning.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1976 2023-10-30 17:43:22.000000 trytond_stock_quantity_early_planning-7.0.0/trytond_stock_quantity_early_planning.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:43:22.000000 trytond_stock_quantity_early_planning-7.0.0/trytond_stock_quantity_early_planning.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       96 2023-10-30 17:43:22.000000 trytond_stock_quantity_early_planning-7.0.0/trytond_stock_quantity_early_planning.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_stock_quantity_early_planning-7.0.0/trytond_stock_quantity_early_planning.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      123 2023-10-30 17:43:22.000000 trytond_stock_quantity_early_planning-7.0.0/trytond_stock_quantity_early_planning.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:43:22.000000 trytond_stock_quantity_early_planning-7.0.0/trytond_stock_quantity_early_planning.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:43:22.532640 trytond_stock_quantity_early_planning-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1483 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.0.0/view/quantity_early_plan_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.0.0/view/quantity_early_plan_generate_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.0.0/view/quantity_early_plan_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:32.617097 trytond_stock_quantity_early_planning-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      992 2024-04-29 15:28:45.000000 trytond_stock_quantity_early_planning-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-29 15:28:45.000000 trytond_stock_quantity_early_planning-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2797 2024-04-29 15:52:32.613764 trytond_stock_quantity_early_planning-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      700 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:32.610431 trytond_stock_quantity_early_planning-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3092 2024-04-27 16:30:39.000000 trytond_stock_quantity_early_planning-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1692 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.2.0/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      277 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.2.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:35.000000 trytond_stock_quantity_early_planning-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.2.0/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:32.613764 trytond_stock_quantity_early_planning-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4526 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4531 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4557 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4575 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3865 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3823 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4490 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3810 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3798 2024-04-27 16:43:28.000000 trytond_stock_quantity_early_planning-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:52:32.617097 trytond_stock_quantity_early_planning-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4785 2024-04-27 16:30:39.000000 trytond_stock_quantity_early_planning-7.2.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21215 2024-01-27 09:58:52.000000 trytond_stock_quantity_early_planning-7.2.0/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6625 2024-04-27 16:30:39.000000 trytond_stock_quantity_early_planning-7.2.0/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:32.613764 trytond_stock_quantity_early_planning-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5191 2024-04-22 12:14:37.000000 trytond_stock_quantity_early_planning-7.2.0/tests/scenario_stock_quantity_early_planning.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4845 2024-04-22 12:14:37.000000 trytond_stock_quantity_early_planning-7.2.0/tests/scenario_stock_quantity_early_planning_incoming.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      477 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:35.000000 trytond_stock_quantity_early_planning-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      110 2024-04-29 15:28:41.000000 trytond_stock_quantity_early_planning-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:32.613764 trytond_stock_quantity_early_planning-7.2.0/trytond_stock_quantity_early_planning.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2797 2024-04-29 15:52:32.000000 trytond_stock_quantity_early_planning-7.2.0/trytond_stock_quantity_early_planning.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1958 2024-04-29 15:52:32.000000 trytond_stock_quantity_early_planning-7.2.0/trytond_stock_quantity_early_planning.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:52:32.000000 trytond_stock_quantity_early_planning-7.2.0/trytond_stock_quantity_early_planning.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       96 2024-04-29 15:52:32.000000 trytond_stock_quantity_early_planning-7.2.0/trytond_stock_quantity_early_planning.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_stock_quantity_early_planning-7.2.0/trytond_stock_quantity_early_planning.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      123 2024-04-29 15:52:32.000000 trytond_stock_quantity_early_planning-7.2.0/trytond_stock_quantity_early_planning.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:52:32.000000 trytond_stock_quantity_early_planning-7.2.0/trytond_stock_quantity_early_planning.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:52:32.613764 trytond_stock_quantity_early_planning-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1483 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.2.0/view/quantity_early_plan_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.2.0/view/quantity_early_plan_generate_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2023-04-15 07:12:15.000000 trytond_stock_quantity_early_planning-7.2.0/view/quantity_early_plan_list.xml
```

### Comparing `trytond_stock_quantity_early_planning-7.0.0/CHANGELOG` & `trytond_stock_quantity_early_planning-7.2.0/CHANGELOG`

 * *Files 22% similar despite different names*

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

### Comparing `trytond_stock_quantity_early_planning-7.0.0/COPYRIGHT` & `trytond_stock_quantity_early_planning-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2021-2023 Cédric Krier
+Copyright (C) 2021-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_stock_quantity_early_planning-7.0.0/LICENSE` & `trytond_stock_quantity_early_planning-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/PKG-INFO` & `trytond_stock_quantity_early_planning-7.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trytond_stock_quantity_early_planning
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to plan earlier shipments and productions
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-quantity-early-planning
+Project-URL: Documentation, https://docs.tryton.org/modules-stock-quantity-early-planning
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock planning shipment production
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,20 +47,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_production<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_production<7.3,>=7.2; extra == "test"
 
 ####################################
 Stock Quantity Early Planning Module
 ####################################
 
 The *Stock Quantity Early Planning Module* helps reducing stock level by
 proposing to consume earlier.
```

### Comparing `trytond_stock_quantity_early_planning-7.0.0/__init__.py` & `trytond_stock_quantity_early_planning-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/doc/conf.py` & `trytond_stock_quantity_early_planning-7.2.0/doc/conf.py`

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

### Comparing `trytond_stock_quantity_early_planning-7.0.0/doc/design.rst` & `trytond_stock_quantity_early_planning-7.2.0/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/bg.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/ca.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/cs.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/de.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/es.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/es_419.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/et.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/fa.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/fi.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/fr.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/hu.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/id.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/it.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/lo.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/lt.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/nl.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/pl.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/pt.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/ro.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/ru.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/sl.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/tr.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/uk.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/locale/zh_CN.po` & `trytond_stock_quantity_early_planning-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/setup.py` & `trytond_stock_quantity_early_planning-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     long_description=read('README.rst'),
     author='Tryton',
     author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
-        "Documentation": ('https://docs.tryton.org/projects/'
+        "Documentation": ('https://docs.tryton.org/'
             'modules-stock-quantity-early-planning'),
         "Forum": 'https://www.tryton.org/forum',
         "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock planning shipment production',
     package_dir={'trytond.modules.stock_quantity_early_planning': '.'},
     packages=(
```

### Comparing `trytond_stock_quantity_early_planning-7.0.0/stock.py` & `trytond_stock_quantity_early_planning-7.2.0/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/stock.xml` & `trytond_stock_quantity_early_planning-7.2.0/stock.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_stock_quantity_early_planning-7.0.0/stock.xml` & `trytond_stock_quantity_early_planning-7.2.0/stock.xml`

```diff
@@ -45,56 +45,56 @@
       <field name="name">All</field>
       <field name="sequence" eval="9999"/>
       <field name="domain"/>
       <field name="act_window" ref="act_quantity_early_plan_form"/>
     </record>
     <menuitem parent="stock.menu_stock" action="act_quantity_early_plan_form" sequence="50" id="menu_quantity_early_plan_form"/>
     <record model="ir.model.access" id="access_quantity_early_plan">
-      <field name="model" search="[('model', '=', 'stock.quantity.early_plan')]"/>
+      <field name="model">stock.quantity.early_plan</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_quantity_early_plan_group_stock">
-      <field name="model" search="[('model', '=', 'stock.quantity.early_plan')]"/>
+      <field name="model">stock.quantity.early_plan</field>
       <field name="group" ref="stock.group_stock"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_quantity_early_plan_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'stock.quantity.early_plan')]"/>
+      <field name="model">stock.quantity.early_plan</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_quantity_early_plan_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_quantity_early_plan_companies"/>
     </record>
     <record model="ir.model.button" id="quantity_early_plan_open_button">
+      <field name="model">stock.quantity.early_plan</field>
       <field name="name">open</field>
       <field name="string">Reset to Open</field>
-      <field name="model" search="[('model', '=', 'stock.quantity.early_plan')]"/>
     </record>
     <record model="ir.model.button" id="quantity_early_plan_process_button">
+      <field name="model">stock.quantity.early_plan</field>
       <field name="name">process</field>
       <field name="string">Process</field>
-      <field name="model" search="[('model', '=', 'stock.quantity.early_plan')]"/>
     </record>
     <record model="ir.model.button" id="quantity_early_plan_close_button">
+      <field name="model">stock.quantity.early_plan</field>
       <field name="name">close</field>
       <field name="string">Close</field>
-      <field name="model" search="[('model', '=', 'stock.quantity.early_plan')]"/>
     </record>
     <record model="ir.model.button" id="quantity_early_plan_ignore_button">
+      <field name="model">stock.quantity.early_plan</field>
       <field name="name">ignore</field>
       <field name="string">Ignore</field>
-      <field name="model" search="[('model', '=', 'stock.quantity.early_plan')]"/>
     </record>
     <record model="ir.action.wizard" id="act_quantity_early_plan_generate">
       <field name="name">Generate Stock Quantity Early Planning</field>
       <field name="wiz_name">stock.quantity.early_plan.generate</field>
     </record>
     <record model="ir.action-res.group" id="act_quantity_early_plan_generate_group_stock_admin">
       <field name="action" ref="act_quantity_early_plan_generate"/>
```

### Comparing `trytond_stock_quantity_early_planning-7.0.0/tests/scenario_stock_quantity_early_planning.rst` & `trytond_stock_quantity_early_planning-7.2.0/tests/scenario_stock_quantity_early_planning.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 ======================================
 Stock Quantity Early Planning Scenario
 ======================================
 
 Imports::
 
-    >>> from decimal import Decimal
-
     >>> import datetime as dt
+    >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
     >>> week1 = today + dt.timedelta(weeks=1)
     >>> week2 = today + dt.timedelta(weeks=2)
     >>> week3 = today + dt.timedelta(weeks=3)
     >>> week4 = today + dt.timedelta(weeks=4)
 
@@ -135,31 +133,25 @@
     >>> generate_planning = Wizard('stock.quantity.early_plan.generate')
     >>> generate_planning.execute('generate')
 
 Check early planning::
 
     >>> plan1, = QuantityEarlyPlan.find(
     ...     [('origin', '=', str(shipment_out1))])
-    >>> plan1.earlier_date == week2
-    True
-    >>> plan1.earliest_date == today
-    True
+    >>> assertEqual(plan1.earlier_date, week2)
+    >>> assertEqual(plan1.earliest_date, today)
     >>> plan1.earliest_percentage
     0.4
 
     >>> plan2, = QuantityEarlyPlan.find(
     ...     [('origin', '=', str(shipment_out2))])
-    >>> plan2.earlier_date == week2
-    True
-    >>> plan2.earliest_date == week2
-    True
+    >>> assertEqual(plan2.earlier_date, week2)
+    >>> assertEqual(plan2.earliest_date, week2)
     >>> plan2.earliest_percentage
     1.0
 
     >>> plan3, = QuantityEarlyPlan.find(
     ...     [('origin', '=', str(shipment_out3))])
-    >>> plan3.earlier_date == week4
-    True
-    >>> plan3.earliest_date == today
-    True
+    >>> assertEqual(plan3.earlier_date, week4)
+    >>> assertEqual(plan3.earliest_date, today)
     >>> plan3.earliest_percentage
     0.75
```

### Comparing `trytond_stock_quantity_early_planning-7.0.0/tests/scenario_stock_quantity_early_planning_incoming.rst` & `trytond_stock_quantity_early_planning-7.2.0/tests/scenario_stock_quantity_early_planning_incoming.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 ===============================================
 Stock Quantity Early Planning Incoming Scenario
 ===============================================
 
 Imports::
 
-    >>> from decimal import Decimal
-
     >>> import datetime as dt
+    >>> from decimal import Decimal
 
     >>> from proteus import Model, Wizard
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import (
-    ...     create_company, get_company)
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
     >>> today = dt.date.today()
     >>> week1 = today + dt.timedelta(weeks=1)
     >>> week2 = today + dt.timedelta(weeks=2)
     >>> week3 = today + dt.timedelta(weeks=3)
 
 Activate modules::
@@ -130,19 +128,16 @@
     >>> generate_planning = Wizard('stock.quantity.early_plan.generate')
     >>> generate_planning.execute('generate')
 
 Check early planning::
 
     >>> plan, = QuantityEarlyPlan.find(
     ...     [('origin', '=', str(shipment_int1))])
-    >>> plan.earlier_date == week1
-    True
+    >>> assertEqual(plan.earlier_date, week1)
 
     >>> plan, = QuantityEarlyPlan.find(
     ...     [('origin', '=', str(shipment_int2))])
-    >>> plan.earlier_date == today
-    True
+    >>> assertEqual(plan.earlier_date, today)
 
     >>> plan, = QuantityEarlyPlan.find(
     ...     [('origin', '=', str(shipment_out))])
-    >>> plan.earlier_date == week1
-    True
+    >>> assertEqual(plan.earlier_date, week1)
```

### Comparing `trytond_stock_quantity_early_planning-7.0.0/tox.ini` & `trytond_stock_quantity_early_planning-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_quantity_early_planning-7.0.0/trytond_stock_quantity_early_planning.egg-info/PKG-INFO` & `trytond_stock_quantity_early_planning-7.2.0/trytond_stock_quantity_early_planning.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: trytond-stock-quantity-early-planning
-Version: 7.0.0
+Name: trytond_stock_quantity_early_planning
+Version: 7.2.0
 Summary: Tryton module to plan earlier shipments and productions
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
-Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock-quantity-early-planning
+Project-URL: Documentation, https://docs.tryton.org/modules-stock-quantity-early-planning
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock planning shipment production
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -47,20 +47,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_production<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_production<7.3,>=7.2; extra == "test"
 
 ####################################
 Stock Quantity Early Planning Module
 ####################################
 
 The *Stock Quantity Early Planning Module* helps reducing stock level by
 proposing to consume earlier.
```

### Comparing `trytond_stock_quantity_early_planning-7.0.0/trytond_stock_quantity_early_planning.egg-info/SOURCES.txt` & `trytond_stock_quantity_early_planning-7.2.0/trytond_stock_quantity_early_planning.egg-info/SOURCES.txt`

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
 setup.py
```

### Comparing `trytond_stock_quantity_early_planning-7.0.0/view/quantity_early_plan_form.xml` & `trytond_stock_quantity_early_planning-7.2.0/view/quantity_early_plan_form.xml`

 * *Files identical despite different names*

