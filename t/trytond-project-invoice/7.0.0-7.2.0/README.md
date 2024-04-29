# Comparing `tmp/trytond_project_invoice-7.0.0.tar.gz` & `tmp/trytond_project_invoice-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_project_invoice-7.0.0.tar", last modified: Mon Oct 30 17:34:30 2023, max compression
+gzip compressed data, was "trytond_project_invoice-7.2.0.tar", last modified: Mon Apr 29 15:44:48 2024, max compression
```

## Comparing `trytond_project_invoice-7.0.0.tar` & `trytond_project_invoice-7.2.0.tar`

### file list

```diff
@@ -1,71 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:30.746770 trytond_project_invoice-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-10-22 17:23:12.000000 trytond_project_invoice-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     2234 2023-10-30 17:10:04.000000 trytond_project_invoice-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-10-30 17:10:04.000000 trytond_project_invoice-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_project_invoice-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_project_invoice-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3279 2023-10-30 17:34:30.746770 trytond_project_invoice-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_project_invoice-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      515 2023-04-15 07:12:15.000000 trytond_project_invoice-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:30.743437 trytond_project_invoice-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2816 2023-10-22 17:23:12.000000 trytond_project_invoice-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_project_invoice-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:12.000000 trytond_project_invoice-7.0.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-04-15 07:12:15.000000 trytond_project_invoice-7.0.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4842 2023-10-07 15:40:36.000000 trytond_project_invoice-7.0.0/invoice.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:30.740104 trytond_project_invoice-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4615 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5513 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4284 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5770 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5557 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4397 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4628 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5020 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4284 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5658 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4313 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4275 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4981 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4501 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4569 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5452 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4331 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4709 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4102 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4563 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4725 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4284 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4102 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4284 2023-10-30 16:47:45.000000 trytond_project_invoice-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2235 2023-10-07 15:40:36.000000 trytond_project_invoice-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    26638 2023-10-07 15:40:36.000000 trytond_project_invoice-7.0.0/project.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3222 2023-04-15 07:12:15.000000 trytond_project_invoice-7.0.0/project.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:34:30.746770 trytond_project_invoice-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4419 2023-10-27 17:38:49.000000 trytond_project_invoice-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:30.743437 trytond_project_invoice-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_project_invoice-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6051 2023-10-07 15:40:36.000000 trytond_project_invoice-7.0.0/tests/scenario_project_invoice_effort.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3307 2023-06-10 11:39:56.000000 trytond_project_invoice-7.0.0/tests/scenario_project_invoice_multiple_party.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6110 2023-10-07 15:40:36.000000 trytond_project_invoice-7.0.0/tests/scenario_project_invoice_progress.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7051 2023-10-07 15:40:36.000000 trytond_project_invoice-7.0.0/tests/scenario_project_invoice_timesheet.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-04-15 07:12:15.000000 trytond_project_invoice-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_project_invoice-7.0.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1743 2023-10-07 15:40:36.000000 trytond_project_invoice-7.0.0/timesheet.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1515 2023-08-21 07:34:17.000000 trytond_project_invoice-7.0.0/timesheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_project_invoice-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      217 2023-10-30 17:10:00.000000 trytond_project_invoice-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:30.743437 trytond_project_invoice-7.0.0/trytond_project_invoice.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3279 2023-10-30 17:34:30.000000 trytond_project_invoice-7.0.0/trytond_project_invoice.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2182 2023-10-30 17:34:30.000000 trytond_project_invoice-7.0.0/trytond_project_invoice.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:34:30.000000 trytond_project_invoice-7.0.0/trytond_project_invoice.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2023-10-30 17:34:30.000000 trytond_project_invoice-7.0.0/trytond_project_invoice.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_project_invoice-7.0.0/trytond_project_invoice.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-10-30 17:34:30.000000 trytond_project_invoice-7.0.0/trytond_project_invoice.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:34:30.000000 trytond_project_invoice-7.0.0/trytond_project_invoice.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:34:30.743437 trytond_project_invoice-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-08-21 07:34:17.000000 trytond_project_invoice-7.0.0/view/timesheet_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1306 2023-04-15 07:12:15.000000 trytond_project_invoice-7.0.0/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-15 07:12:15.000000 trytond_project_invoice-7.0.0/view/work_invoiced_progress_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      365 2023-04-15 07:12:15.000000 trytond_project_invoice-7.0.0/view/work_invoiced_progress_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:15.000000 trytond_project_invoice-7.0.0/view/work_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:48.345907 trytond_project_invoice-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2335 2024-04-29 15:23:08.000000 trytond_project_invoice-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:23:08.000000 trytond_project_invoice-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_project_invoice-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3279 2024-04-29 15:44:48.345907 trytond_project_invoice-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      515 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:48.342573 trytond_project_invoice-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-27 16:30:39.000000 trytond_project_invoice-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:19.000000 trytond_project_invoice-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      229 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4804 2024-04-22 12:14:36.000000 trytond_project_invoice-7.2.0/invoice.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:48.342573 trytond_project_invoice-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4615 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5513 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4284 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5770 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5557 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4397 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4628 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5020 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4284 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5658 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4313 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4275 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4981 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4501 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4569 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5452 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4331 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4709 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4102 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4563 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4725 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4284 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4102 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4284 2024-04-27 16:43:25.000000 trytond_project_invoice-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2235 2024-02-04 18:51:26.000000 trytond_project_invoice-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    26656 2024-04-27 16:30:39.000000 trytond_project_invoice-7.2.0/project.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3160 2024-04-27 16:30:39.000000 trytond_project_invoice-7.2.0/project.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:44:48.345907 trytond_project_invoice-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4419 2024-03-17 11:01:36.000000 trytond_project_invoice-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:48.345907 trytond_project_invoice-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5965 2024-04-22 12:14:36.000000 trytond_project_invoice-7.2.0/tests/scenario_project_invoice_effort.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3272 2024-04-22 12:14:36.000000 trytond_project_invoice-7.2.0/tests/scenario_project_invoice_multiple_party.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6024 2024-04-22 12:14:36.000000 trytond_project_invoice-7.2.0/tests/scenario_project_invoice_progress.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6908 2024-04-22 12:14:36.000000 trytond_project_invoice-7.2.0/tests/scenario_project_invoice_timesheet.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1743 2024-02-04 18:51:26.000000 trytond_project_invoice-7.2.0/timesheet.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1515 2024-01-27 09:58:52.000000 trytond_project_invoice-7.2.0/timesheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:19.000000 trytond_project_invoice-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      217 2024-04-29 15:23:03.000000 trytond_project_invoice-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:48.345907 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3279 2024-04-29 15:44:47.000000 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2164 2024-04-29 15:44:48.000000 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:44:47.000000 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-04-29 15:44:47.000000 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:57.000000 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-04-29 15:44:47.000000 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:44:47.000000 trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:48.345907 trytond_project_invoice-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-01-27 09:58:52.000000 trytond_project_invoice-7.2.0/view/timesheet_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1306 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      520 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/view/work_invoiced_progress_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      365 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/view/work_invoiced_progress_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:15.000000 trytond_project_invoice-7.2.0/view/work_list.xml
```

### Comparing `trytond_project_invoice-7.0.0/CHANGELOG` & `trytond_project_invoice-7.2.0/CHANGELOG`

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

### Comparing `trytond_project_invoice-7.0.0/COPYRIGHT` & `trytond_project_invoice-7.2.0/COPYRIGHT`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2013-2023 Cédric Krier.
-Copyright (C) 2013-2023 B2CK SPRL.
+Copyright (C) 2013-2024 Cédric Krier.
+Copyright (C) 2013-2024 B2CK SPRL.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_project_invoice-7.0.0/LICENSE` & `trytond_project_invoice-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/PKG-INFO` & `trytond_project_invoice-7.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_project_invoice
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module to invoice projects
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_project<7.1,>=7.0
-Requires-Dist: trytond_project_revenue<7.1,>=7.0
-Requires-Dist: trytond_timesheet<7.1,>=7.0
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_project<7.3,>=7.2
+Requires-Dist: trytond_project_revenue<7.3,>=7.2
+Requires-Dist: trytond_timesheet<7.3,>=7.2
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Project Invoice Module
 ######################
 
 The Project Invoice module adds invoice methods on project.
 The methods are:
```

### Comparing `trytond_project_invoice-7.0.0/__init__.py` & `trytond_project_invoice-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/doc/conf.py` & `trytond_project_invoice-7.2.0/doc/conf.py`

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

### Comparing `trytond_project_invoice-7.0.0/invoice.py` & `trytond_project_invoice-7.2.0/invoice.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from trytond.i18n import gettext
 from trytond.model import fields
 from trytond.modules.account_invoice.exceptions import (
     InvoiceLineValidationError)
 from trytond.pool import Pool, PoolMeta
 from trytond.tools import grouped_slice, reduce_ids
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
 
 
 class InvoiceLine(metaclass=PoolMeta):
     __name__ = 'account.invoice.line'
 
     project_invoice_works = fields.One2Many(
         'project.work', 'invoice_line',
@@ -110,18 +110,17 @@
         cls.check_validate_project_invoice_quantity(lines, field_names)
 
     @classmethod
     def delete(cls, lines):
         pool = Pool()
         WorkInvoicedProgress = pool.get('project.work.invoiced_progress')
 
-        # Delete progress using root to skip access rule
         progress = []
         for sub_ids in grouped_slice([l.id for l in lines]):
             progress += WorkInvoicedProgress.search([
                     ('invoice_line', 'in', sub_ids),
                     ])
         if progress:
-            with Transaction().set_user(0):
+            with without_check_access():
                 WorkInvoicedProgress.delete(progress)
 
         super(InvoiceLine, cls).delete(lines)
```

### Comparing `trytond_project_invoice-7.0.0/locale/bg.po` & `trytond_project_invoice-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/ca.po` & `trytond_project_invoice-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/cs.po` & `trytond_project_invoice-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/de.po` & `trytond_project_invoice-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/es.po` & `trytond_project_invoice-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/es_419.po` & `trytond_project_invoice-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/et.po` & `trytond_project_invoice-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/fa.po` & `trytond_project_invoice-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/fi.po` & `trytond_project_invoice-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/fr.po` & `trytond_project_invoice-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/hu.po` & `trytond_project_invoice-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/id.po` & `trytond_project_invoice-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/it.po` & `trytond_project_invoice-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/lo.po` & `trytond_project_invoice-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/lt.po` & `trytond_project_invoice-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/nl.po` & `trytond_project_invoice-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/pl.po` & `trytond_project_invoice-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/pt.po` & `trytond_project_invoice-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/ro.po` & `trytond_project_invoice-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/ru.po` & `trytond_project_invoice-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/sl.po` & `trytond_project_invoice-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/tr.po` & `trytond_project_invoice-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/uk.po` & `trytond_project_invoice-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/locale/zh_CN.po` & `trytond_project_invoice-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/message.xml` & `trytond_project_invoice-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/project.py` & `trytond_project_invoice-7.2.0/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -588,15 +588,15 @@
         invoice_line.type = 'line'
         invoice_line.description = key['description']
         invoice_line.unit_price = key['unit_price']
         invoice_line.quantity = quantity
         invoice_line.unit = key['unit']
         invoice_line.product = product
         invoice_line.on_change_product()
-        if not invoice_line.account:
+        if not getattr(invoice_line, 'account', None):
             if invoice_line.product:
                 raise InvoicingError(
                     gettext(
                         'project_invoice.msg_product_missing_account_revenue',
                         work=self.rec_name,
                         product=invoice_line.product.rec_name))
             else:
```

### Comparing `trytond_project_invoice-7.0.0/project.xml` & `trytond_project_invoice-7.2.0/project.xml`

 * *Files 3% similar despite different names*

#### Comparing `trytond_project_invoice-7.0.0/project.xml` & `trytond_project_invoice-7.2.0/project.xml`

```diff
@@ -17,17 +17,17 @@
     </record>
     <record model="ir.ui.view" id="work_view_form">
       <field name="model">project.work</field>
       <field name="inherit" ref="project.work_view_form"/>
       <field name="name">work_form</field>
     </record>
     <record model="ir.model.button" id="work_invoice_button">
+      <field name="model">project.work</field>
       <field name="name">invoice</field>
       <field name="string">Invoice</field>
-      <field name="model" search="[('model', '=', 'project.work')]"/>
     </record>
     <record model="ir.model.button-res.group" id="work_invoice_button_group_project_invoice">
       <field name="button" ref="work_invoice_button"/>
       <field name="group" ref="group_project_invoice"/>
     </record>
     <record model="ir.ui.view" id="work_invoiced_progress_view_form">
       <field name="model">project.work.invoiced_progress</field>
@@ -36,15 +36,15 @@
     </record>
     <record model="ir.ui.view" id="work_invoiced_progress_view_list">
       <field name="model">project.work.invoiced_progress</field>
       <field name="type">tree</field>
       <field name="name">work_invoiced_progress_list</field>
     </record>
     <record model="ir.model.access" id="access_work_invoiced_progress">
-      <field name="model" search="[('model', '=', 'project.work.invoiced_progress')]"/>
+      <field name="model">project.work.invoiced_progress</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.action.wizard" id="open_invoice">
       <field name="name">Invoices</field>
```

### Comparing `trytond_project_invoice-7.0.0/setup.py` & `trytond_project_invoice-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/tests/scenario_project_invoice_effort.rst` & `trytond_project_invoice-7.2.0/tests/scenario_project_invoice_effort.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 Project Invoice Effort Scenario
 ===============================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.account_invoice.tests.tools import create_payment_term
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     create_payment_term
 
 Activate modules::
 
     >>> config = activate_modules('project_invoice')
 
 Create company::
 
@@ -195,13 +193,13 @@
 
 Try to change invoice line quantity::
 
     >>> set_user(1)
     >>> ProjectWork = Model.get('project.work')
     >>> task = ProjectWork(task.id)
     >>> task.invoice_line.quantity = 1
-    >>> task.invoice_line.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> task.invoice_line.save()
     Traceback (most recent call last):
         ...
     InvoiceLineValidationError: ...
     >>> task.invoice_line.quantity = 5
     >>> task.invoice_line.save()
```

### Comparing `trytond_project_invoice-7.0.0/tests/scenario_project_invoice_multiple_party.rst` & `trytond_project_invoice-7.2.0/tests/scenario_project_invoice_multiple_party.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 Project Invoice Multiple Parties Scenario
 =========================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
 
 Activate modules::
 
     >>> config = activate_modules('project_invoice')
 
 Create company::
```

### Comparing `trytond_project_invoice-7.0.0/tests/scenario_project_invoice_progress.rst` & `trytond_project_invoice-7.2.0/tests/scenario_project_invoice_progress.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 Project Invoice Progress Scenario
 =================================
 
 Imports::
 
     >>> import datetime as dt
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.account_invoice.tests.tools import create_payment_term
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     create_payment_term
 
 Activate modules::
 
     >>> config = activate_modules('project_invoice')
 
 Create company::
 
@@ -198,13 +196,13 @@
 Try to change invoice line quantity::
 
     >>> set_user(1)
     >>> ProjectWork = Model.get('project.work')
     >>> task = ProjectWork(task.id)
     >>> invoice_line = task.invoiced_progress[0].invoice_line
     >>> invoice_line.quantity = 2.
-    >>> invoice_line.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> invoice_line.save()
     Traceback (most recent call last):
         ...
     InvoiceLineValidationError: ...
     >>> invoice_line.quantity = 2.5
     >>> invoice_line.save()
```

### Comparing `trytond_project_invoice-7.0.0/tests/scenario_project_invoice_timesheet.rst` & `trytond_project_invoice-7.2.0/tests/scenario_project_invoice_timesheet.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 ==================================
 Project Invoice Timesheet Scenario
 ==================================
 
 Imports::
 
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
-    >>> from proteus import Model, Wizard
+
+    >>> from proteus import Model
+    >>> from trytond.modules.account.tests.tools import create_chart, get_accounts
+    >>> from trytond.modules.account_invoice.tests.tools import create_payment_term
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules, set_user
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
-    >>> from trytond.modules.account.tests.tools import create_chart, \
-    ...     get_accounts
-    >>> from trytond.modules.account_invoice.tests.tools import \
-    ...     create_payment_term
 
     >>> today = dt.date.today()
     >>> yesterday = today - dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('project_invoice')
@@ -228,13 +225,13 @@
 
 Try to change invoice line quantity::
 
     >>> set_user(1)
     >>> TimesheetLine = Model.get('timesheet.line')
     >>> line = TimesheetLine(line.id)
     >>> line.invoice_line.quantity = 5
-    >>> line.invoice_line.save()  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> line.invoice_line.save()
     Traceback (most recent call last):
         ...
     InvoiceLineValidationError: ...
     >>> line.invoice_line.quantity = 4
     >>> line.invoice_line.save()
```

### Comparing `trytond_project_invoice-7.0.0/timesheet.py` & `trytond_project_invoice-7.2.0/timesheet.py`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/timesheet.xml` & `trytond_project_invoice-7.2.0/timesheet.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/tox.ini` & `trytond_project_invoice-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/trytond_project_invoice.egg-info/PKG-INFO` & `trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-project-invoice
-Version: 7.0.0
+Name: trytond_project_invoice
+Version: 7.2.0
 Summary: Tryton module to invoice projects
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql>=0.4
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_project<7.1,>=7.0
-Requires-Dist: trytond_project_revenue<7.1,>=7.0
-Requires-Dist: trytond_timesheet<7.1,>=7.0
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_account_invoice<7.1,>=7.0
-Requires-Dist: trytond_account_product<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_project<7.3,>=7.2
+Requires-Dist: trytond_project_revenue<7.3,>=7.2
+Requires-Dist: trytond_timesheet<7.3,>=7.2
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_account_invoice<7.3,>=7.2
+Requires-Dist: trytond_account_product<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
 
 Project Invoice Module
 ######################
 
 The Project Invoice module adds invoice methods on project.
 The methods are:
```

### Comparing `trytond_project_invoice-7.0.0/trytond_project_invoice.egg-info/SOURCES.txt` & `trytond_project_invoice-7.2.0/trytond_project_invoice.egg-info/SOURCES.txt`

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
 exceptions.py
```

### Comparing `trytond_project_invoice-7.0.0/view/work_form.xml` & `trytond_project_invoice-7.2.0/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_project_invoice-7.0.0/view/work_invoiced_progress_form.xml` & `trytond_project_invoice-7.2.0/view/work_invoiced_progress_form.xml`

 * *Files identical despite different names*

