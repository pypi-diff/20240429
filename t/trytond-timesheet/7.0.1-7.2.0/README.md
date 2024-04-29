# Comparing `tmp/trytond_timesheet-7.0.1.tar.gz` & `tmp/trytond_timesheet-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_timesheet-7.0.1.tar", last modified: Sun Mar  3 12:14:59 2024, max compression
+gzip compressed data, was "trytond_timesheet-7.2.0.tar", last modified: Mon Apr 29 15:53:44 2024, max compression
```

## Comparing `trytond_timesheet-7.0.1.tar` & `trytond_timesheet-7.2.0.tar`

### file list

```diff
@@ -1,81 +1,80 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:14:59.017357 trytond_timesheet-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)     3216 2024-03-03 12:14:56.000000 trytond_timesheet-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-03-03 12:14:56.000000 trytond_timesheet-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3292 2024-03-03 12:14:59.017357 trytond_timesheet-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      919 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      693 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:14:59.010688 trytond_timesheet-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2810 2024-02-05 16:24:27.000000 trytond_timesheet-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      919 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1387 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/doc/user_application.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:14:59.010688 trytond_timesheet-7.0.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/icons/tryton-timesheet.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      986 2024-02-29 11:40:05.000000 trytond_timesheet-7.0.1/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11744 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/line.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14834 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/line.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:14:59.014023 trytond_timesheet-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     9957 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10720 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9166 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11001 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10808 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9081 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9903 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11142 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9153 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10859 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9704 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8944 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9679 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10856 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9214 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10536 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9454 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10451 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9369 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10099 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10216 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9249 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12208 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10331 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      931 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4563 2024-02-05 16:24:27.000000 trytond_timesheet-7.0.1/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-03-03 12:14:59.017357 trytond_timesheet-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4372 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:14:59.014023 trytond_timesheet-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1498 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/timesheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      146 2024-02-05 16:24:27.000000 trytond_timesheet-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:14:59.017357 trytond_timesheet-7.0.1/trytond_timesheet.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3292 2024-03-03 12:14:58.000000 trytond_timesheet-7.0.1/trytond_timesheet.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2277 2024-03-03 12:14:58.000000 trytond_timesheet-7.0.1/trytond_timesheet.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-03-03 12:14:58.000000 trytond_timesheet-7.0.1/trytond_timesheet.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-03-03 12:14:58.000000 trytond_timesheet-7.0.1/trytond_timesheet.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:08:20.000000 trytond_timesheet-7.0.1/trytond_timesheet.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       91 2024-03-03 12:14:58.000000 trytond_timesheet-7.0.1/trytond_timesheet.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-03-03 12:14:58.000000 trytond_timesheet-7.0.1/trytond_timesheet.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/user.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:14:59.017357 trytond_timesheet-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/view/hours_employee_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/view/hours_employee_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/view/hours_employee_monthly_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      274 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/view/hours_employee_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/view/hours_employee_weekly_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/view/line_enter_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      522 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/view/line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/view/line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/view/work_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      681 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/view/work_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/view/work_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/view/work_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-10-30 17:06:39.000000 trytond_timesheet-7.0.1/view/work_list_report.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6303 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/work.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5388 2023-10-30 17:06:38.000000 trytond_timesheet-7.0.1/work.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:44.455218 trytond_timesheet-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3216 2024-04-29 15:29:41.000000 trytond_timesheet-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:29:40.000000 trytond_timesheet-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_timesheet-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3292 2024-04-29 15:53:44.455218 trytond_timesheet-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      919 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      693 2024-02-04 18:51:27.000000 trytond_timesheet-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:44.448552 trytond_timesheet-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3072 2024-04-27 16:30:39.000000 trytond_timesheet-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      919 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:38.000000 trytond_timesheet-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1387 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/doc/user_application.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:44.448552 trytond_timesheet-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      376 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/icons/tryton-timesheet.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      988 2024-04-29 13:17:17.000000 trytond_timesheet-7.2.0/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11826 2024-04-27 16:30:39.000000 trytond_timesheet-7.2.0/line.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14558 2024-04-27 16:30:39.000000 trytond_timesheet-7.2.0/line.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:44.451885 trytond_timesheet-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     9957 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10720 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9166 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11001 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10808 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9081 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9903 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11142 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9153 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10859 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9704 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8944 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9679 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10856 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9214 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10536 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9454 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10451 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10591 2024-04-29 13:17:17.000000 trytond_timesheet-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10099 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10216 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9249 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12208 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10331 2024-04-27 16:43:28.000000 trytond_timesheet-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      931 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4582 2024-04-22 12:14:36.000000 trytond_timesheet-7.2.0/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:53:44.455218 trytond_timesheet-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4372 2024-03-17 11:01:36.000000 trytond_timesheet-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:44.451885 trytond_timesheet-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1498 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/timesheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:38.000000 trytond_timesheet-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      146 2024-04-29 15:29:36.000000 trytond_timesheet-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:44.455218 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3292 2024-04-29 15:53:43.000000 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2259 2024-04-29 15:53:44.000000 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:53:43.000000 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-04-29 15:53:43.000000 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:56.000000 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       91 2024-04-29 15:53:43.000000 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:53:43.000000 trytond_timesheet-7.2.0/trytond_timesheet.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      420 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/user.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:53:44.455218 trytond_timesheet-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-01-16 14:00:21.000000 trytond_timesheet-7.2.0/view/hours_employee_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2023-01-16 14:00:21.000000 trytond_timesheet-7.2.0/view/hours_employee_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/view/hours_employee_monthly_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      274 2024-01-27 09:58:52.000000 trytond_timesheet-7.2.0/view/hours_employee_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/view/hours_employee_weekly_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-09-12 21:17:04.000000 trytond_timesheet-7.2.0/view/line_enter_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      522 2023-01-16 14:00:21.000000 trytond_timesheet-7.2.0/view/line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2024-01-27 09:58:52.000000 trytond_timesheet-7.2.0/view/line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-01-16 14:00:21.000000 trytond_timesheet-7.2.0/view/work_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      681 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/view/work_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-01-16 14:00:21.000000 trytond_timesheet-7.2.0/view/work_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/view/work_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_timesheet-7.2.0/view/work_list_report.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6303 2024-01-27 09:58:52.000000 trytond_timesheet-7.2.0/work.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5319 2024-04-27 16:30:39.000000 trytond_timesheet-7.2.0/work.xml
```

### Comparing `trytond_timesheet-7.0.1/CHANGELOG` & `trytond_timesheet-7.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Version 7.0.1 - 2024-03-03
+Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
```

### Comparing `trytond_timesheet-7.0.1/LICENSE` & `trytond_timesheet-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/PKG-INFO` & `trytond_timesheet-7.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_timesheet
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module with timesheets
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
@@ -49,17 +49,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_company_work_time<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_company_work_time<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Timesheet Module
 ################
 
 The timesheet module allow to track the time spent by employees on
 various works. This module also comes with several reports that show
 the time spent by employees on works following various time periods.
```

### Comparing `trytond_timesheet-7.0.1/README.rst` & `trytond_timesheet-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/__init__.py` & `trytond_timesheet-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/doc/conf.py` & `trytond_timesheet-7.2.0/doc/conf.py`

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

### Comparing `trytond_timesheet-7.0.1/doc/index.rst` & `trytond_timesheet-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/doc/user_application.rst` & `trytond_timesheet-7.2.0/doc/user_application.rst`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/icons/LICENSE` & `trytond_timesheet-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/ir.py` & `trytond_timesheet-7.2.0/ir.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,14 @@
         User = pool.get('res.user')
         context = super()._get_context(model_name)
         if model_name in _EMPLOYEES_RULE_MODELS:
             context['employees'] = User.get_employees()
         return context
 
     @classmethod
-    def _get_cache_key(cls, model_name):
+    def _get_cache_key(cls, model_names):
         pool = Pool()
         User = pool.get('res.user')
-        key = super()._get_cache_key(model_name)
-        if model_name in _EMPLOYEES_RULE_MODELS:
+        key = super()._get_cache_key(model_names)
+        if model_names & _EMPLOYEES_RULE_MODELS:
             key = (*key, User.get_employees())
         return key
```

### Comparing `trytond_timesheet-7.0.1/line.py` & `trytond_timesheet-7.2.0/line.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,19 @@
 
 class Line(ModelSQL, ModelView):
     'Timesheet Line'
     __name__ = 'timesheet.line'
     company = fields.Many2One('company.company', 'Company', required=True,
         help="The company on which the time is spent.")
     employee = fields.Many2One(
-        'company.employee', "Employee", required=True, domain=[
+        'company.employee', "Employee", required=True,
+        search_context={
+            'active_test': False,
+            },
+        domain=[
             ('company', '=', Eval('company', -1)),
             ['OR',
                 ('start_date', '=', None),
                 ('start_date', '<=', Eval('date', None)),
                 ],
             ['OR',
                 ('end_date', '=', None),
```

### Comparing `trytond_timesheet-7.0.1/line.xml` & `trytond_timesheet-7.2.0/line.xml`

 * *Files 4% similar despite different names*

#### Comparing `trytond_timesheet-7.0.1/line.xml` & `trytond_timesheet-7.2.0/line.xml`

```diff
@@ -46,35 +46,35 @@
     <record model="ir.action.keyword" id="act_line_form_work_keyword1">
       <field name="keyword">form_relate</field>
       <field name="model">timesheet.work,-1</field>
       <field name="action" ref="act_line_form_work"/>
     </record>
     <record model="ir.rule.group" id="rule_group_line_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'timesheet.line')]"/>
+      <field name="model">timesheet.line</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_line_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_line_companies"/>
     </record>
     <record model="ir.rule.group" id="rule_group_line">
       <field name="name">Own timesheet line</field>
-      <field name="model" search="[('model', '=', 'timesheet.line')]"/>
+      <field name="model">timesheet.line</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="True"/>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.rule" id="rule_line">
       <field name="domain" eval="[('employee', 'in', Eval('employees', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_line"/>
     </record>
     <record model="ir.rule.group" id="rule_group_line_admin">
       <field name="name">Any timesheet line</field>
-      <field name="model" search="[('model', '=', 'timesheet.line')]"/>
+      <field name="model">timesheet.line</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="False"/>
     </record>
     <record model="ir.rule.group-res.group" id="rule_group_line_admin_group_timesheet_admin">
       <field name="rule_group" ref="rule_group_line_admin"/>
       <field name="group" ref="group_timesheet_admin"/>
     </record>
@@ -112,35 +112,35 @@
       <field name="sequence" eval="20"/>
       <field name="view" ref="hours_employee_view_graph"/>
       <field name="act_window" ref="act_hours_employee_form"/>
     </record>
     <menuitem parent="menu_reporting" action="act_hours_employee_form" sequence="50" id="menu_hours_employee"/>
     <record model="ir.rule.group" id="rule_group_hours_employees">
       <field name="name">Own hours</field>
-      <field name="model" search="[('model', '=', 'timesheet.hours_employee')]"/>
+      <field name="model">timesheet.hours_employee</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_hours_employees">
       <field name="domain" eval="[('employee', 'in', Eval('employees', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_hours_employees"/>
     </record>
     <record model="ir.rule.group" id="rule_group_hours_supervised_employees">
       <field name="name">Supervised employee's hours</field>
-      <field name="model" search="[('model', '=', 'timesheet.hours_employee')]"/>
+      <field name="model">timesheet.hours_employee</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_hours_supervised_employees">
       <field name="domain" eval="[('employee.supervisor', 'in', Eval('employees', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_hours_supervised_employees"/>
     </record>
     <record model="ir.rule.group" id="rule_group_hours_employee_admin">
       <field name="name">Any employee hours</field>
-      <field name="model" search="[('model', '=', 'timesheet.hours_employee')]"/>
+      <field name="model">timesheet.hours_employee</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="False"/>
     </record>
     <record model="ir.rule.group-res.group" id="rule_group_hours_employee_admin_group_timesheet_admin">
       <field name="rule_group" ref="rule_group_hours_employee_admin"/>
       <field name="group" ref="group_timesheet_admin"/>
     </record>
@@ -162,35 +162,35 @@
       <field name="sequence" eval="10"/>
       <field name="view" ref="hours_employee_weekly_view_tree"/>
       <field name="act_window" ref="act_hours_employee_weekly_form"/>
     </record>
     <menuitem parent="menu_reporting" action="act_hours_employee_weekly_form" sequence="50" id="menu_hours_employee_open_weekly"/>
     <record model="ir.rule.group" id="rule_group_hours_employee_weekly">
       <field name="name">Own hours</field>
-      <field name="model" search="[('model', '=', 'timesheet.hours_employee_weekly')]"/>
+      <field name="model">timesheet.hours_employee_weekly</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_hours_employee_weekly">
       <field name="domain" eval="[('employee', 'in', Eval('employees', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_hours_employee_weekly"/>
     </record>
     <record model="ir.rule.group" id="rule_group_hours_supervised_employees_weekly">
       <field name="name">Supervised employee's hours</field>
-      <field name="model" search="[('model', '=', 'timesheet.hours_employee_weekly')]"/>
+      <field name="model">timesheet.hours_employee_weekly</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_hours_supervised_employees_weekly">
       <field name="domain" eval="[('employee.supervisor', 'in', Eval('employees', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_hours_supervised_employees_weekly"/>
     </record>
     <record model="ir.rule.group" id="rule_group_hours_employee_weekly_admin">
       <field name="name">Any employee hours</field>
-      <field name="model" search="[('model', '=', 'timesheet.hours_employee_weekly')]"/>
+      <field name="model">timesheet.hours_employee_weekly</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="False"/>
     </record>
     <record model="ir.rule.group-res.group" id="rule_group_hours_employee_weekly_admin_group_timesheet_admin">
       <field name="rule_group" ref="rule_group_hours_employee_weekly_admin"/>
       <field name="group" ref="group_timesheet_admin"/>
     </record>
@@ -207,35 +207,35 @@
       <field name="sequence" eval="10"/>
       <field name="view" ref="hours_employee_monthly_view_tree"/>
       <field name="act_window" ref="act_hours_employee_monthly_form"/>
     </record>
     <menuitem parent="menu_reporting" action="act_hours_employee_monthly_form" sequence="50" id="menu_hours_employee_open_monthly"/>
     <record model="ir.rule.group" id="rule_group_hours_employee_monthly">
       <field name="name">Own hours</field>
-      <field name="model" search="[('model', '=', 'timesheet.hours_employee_monthly')]"/>
+      <field name="model">timesheet.hours_employee_monthly</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_hours_employee_monthly">
       <field name="domain" eval="[('employee', 'in', Eval('employees', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_hours_employee_monthly"/>
     </record>
     <record model="ir.rule.group" id="rule_group_hours_supervised_employees_monthly">
       <field name="name">Supervised employee's hours</field>
-      <field name="model" search="[('model', '=', 'timesheet.hours_employee_monthly')]"/>
+      <field name="model">timesheet.hours_employee_monthly</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_hours_supervised_employees_monthly">
       <field name="domain" eval="[('employee.supervisor', 'in', Eval('employees', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_hours_supervised_employees_monthly"/>
     </record>
     <record model="ir.rule.group" id="rule_group_hours_employee_monthly_admin">
       <field name="name">Any employee hours</field>
-      <field name="model" search="[('model', '=', 'timesheet.hours_employee_monthly')]"/>
+      <field name="model">timesheet.hours_employee_monthly</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="False"/>
     </record>
     <record model="ir.rule.group-res.group" id="rule_group_hours_employee_monthly_admin_group_timesheet_admin">
       <field name="rule_group" ref="rule_group_hours_employee_monthly_admin"/>
       <field name="group" ref="group_timesheet_admin"/>
     </record>
```

### Comparing `trytond_timesheet-7.0.1/locale/bg.po` & `trytond_timesheet-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/ca.po` & `trytond_timesheet-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/cs.po` & `trytond_timesheet-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/de.po` & `trytond_timesheet-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/es.po` & `trytond_timesheet-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/es_419.po` & `trytond_timesheet-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/et.po` & `trytond_timesheet-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/fa.po` & `trytond_timesheet-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/fi.po` & `trytond_timesheet-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/fr.po` & `trytond_timesheet-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/hu.po` & `trytond_timesheet-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/id.po` & `trytond_timesheet-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/it.po` & `trytond_timesheet-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/lo.po` & `trytond_timesheet-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/lt.po` & `trytond_timesheet-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/nl.po` & `trytond_timesheet-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/pl.po` & `trytond_timesheet-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/pt.po` & `trytond_timesheet-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/ro.po` & `trytond_timesheet-7.2.0/locale/zh_CN.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,389 +1,401 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:timesheet.hours_employee,duration:"
 msgid "Duration"
-msgstr "Durata"
+msgstr "持续时间"
 
 msgctxt "field:timesheet.hours_employee,employee:"
 msgid "Employee"
-msgstr "Angajat"
+msgstr "雇员"
 
 msgctxt "field:timesheet.hours_employee.context,end_date:"
 msgid "End Date"
-msgstr "Data Sfărşit"
+msgstr "结束日期"
 
 msgctxt "field:timesheet.hours_employee.context,start_date:"
 msgid "Start Date"
-msgstr "Data Început"
+msgstr "开始日期"
 
 msgctxt "field:timesheet.hours_employee_monthly,duration:"
 msgid "Duration"
-msgstr "Durata"
+msgstr "持续时间"
 
 msgctxt "field:timesheet.hours_employee_monthly,employee:"
 msgid "Employee"
-msgstr "Angajat"
+msgstr "雇员"
 
 msgctxt "field:timesheet.hours_employee_monthly,month:"
 msgid "Month"
-msgstr "Luna"
+msgstr "月"
 
 msgctxt "field:timesheet.hours_employee_monthly,year:"
 msgid "Year"
-msgstr "An"
+msgstr "年"
 
 msgctxt "field:timesheet.hours_employee_weekly,duration:"
 msgid "Duration"
-msgstr "Durata"
+msgstr "持续时间"
 
 msgctxt "field:timesheet.hours_employee_weekly,employee:"
 msgid "Employee"
-msgstr "Angajat"
+msgstr "雇员"
 
 msgctxt "field:timesheet.hours_employee_weekly,week:"
 msgid "Week"
-msgstr "Săptămâna"
+msgstr "周"
 
 msgctxt "field:timesheet.hours_employee_weekly,year:"
 msgid "Year"
-msgstr "An"
+msgstr "年"
 
 msgctxt "field:timesheet.line,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr "公司"
 
 msgctxt "field:timesheet.line,date:"
 msgid "Date"
-msgstr "Data"
+msgstr "日期"
 
 msgctxt "field:timesheet.line,description:"
 msgid "Description"
-msgstr "Descriere"
+msgstr "描述"
 
 msgctxt "field:timesheet.line,duration:"
 msgid "Duration"
-msgstr "Durata"
+msgstr "持续时间"
 
 msgctxt "field:timesheet.line,employee:"
 msgid "Employee"
-msgstr "Angajat"
+msgstr "雇员"
 
 msgctxt "field:timesheet.line,uuid:"
 msgid "UUID"
 msgstr "UUID"
 
 msgctxt "field:timesheet.line,work:"
 msgid "Work"
-msgstr "Muncă"
+msgstr "工作"
 
 msgctxt "field:timesheet.line.enter.start,date:"
 msgid "Date"
-msgstr "Data"
+msgstr "日期"
 
 msgctxt "field:timesheet.line.enter.start,employee:"
 msgid "Employee"
-msgstr "Angajat"
+msgstr "雇员"
 
 msgctxt "field:timesheet.work,company:"
 msgid "Company"
-msgstr "Companie"
+msgstr "公司"
 
 msgctxt "field:timesheet.work,duration:"
 msgid "Timesheet Duration"
-msgstr "Durata Foaie Pontaj"
+msgstr "时间表持续时间"
 
 msgctxt "field:timesheet.work,name:"
 msgid "Name"
-msgstr "Nume"
+msgstr "名称"
 
 msgctxt "field:timesheet.work,origin:"
 msgid "Origin"
-msgstr "Origine"
+msgstr "来源"
 
 msgctxt "field:timesheet.work,timesheet_end_date:"
 msgid "Timesheet End"
-msgstr "Foaie Pontaj Sfârșit"
+msgstr "时间表结束"
 
 msgctxt "field:timesheet.work,timesheet_lines:"
 msgid "Timesheet Lines"
-msgstr "Rânduri Foaie Pontaj"
+msgstr "时间表明细"
 
 msgctxt "field:timesheet.work,timesheet_start_date:"
 msgid "Timesheet Start"
-msgstr "Foaie Pontaj Început"
+msgstr "时间表开始"
 
 msgctxt "field:timesheet.work,work:"
 msgid "Work"
-msgstr "Muncă"
+msgstr "工作"
 
 msgctxt "field:timesheet.work.context,from_date:"
 msgid "From Date"
-msgstr "De la Data"
+msgstr "从日期"
 
 msgctxt "field:timesheet.work.context,to_date:"
 msgid "To Date"
-msgstr "Până la Data"
+msgstr "到日期"
 
 msgctxt "help:timesheet.line,company:"
 msgid "The company on which the time is spent."
-msgstr "Compania al cărei timp a fost folosit."
+msgstr "消耗时间的公司."
 
 msgctxt "help:timesheet.line,date:"
 msgid "When the time is spent."
-msgstr "Când a fost folosit timp."
+msgstr "时间消耗的时候."
 
 msgctxt "help:timesheet.line,description:"
 msgid "Additional description of the work done."
-msgstr "Descriere adițională al muncii efectuate."
+msgstr "完成工作的附加说明."
 
 msgctxt "help:timesheet.line,employee:"
 msgid "The employee who spends the time."
-msgstr "Angajatul care foloseşte timp."
+msgstr "消耗时间的雇员."
 
 msgctxt "help:timesheet.line,work:"
 msgid "The work on which the time is spent."
-msgstr "Muncă pe care este cheltuit timp."
+msgstr "消耗时间的工作."
 
 msgctxt "help:timesheet.line.enter.start,date:"
 msgid "When the time is spent."
-msgstr "Când este folosit timp."
+msgstr "消耗时间的时候."
 
 msgctxt "help:timesheet.line.enter.start,employee:"
 msgid "The employee who spends the time."
-msgstr "Angajatul care foloseşte timp."
+msgstr "消耗时间的雇员."
 
 msgctxt "help:timesheet.work,company:"
 msgid "Make the work belong to the company."
-msgstr "Atribuire Muncă la compania."
+msgstr "让这项工作属于公司."
 
 msgctxt "help:timesheet.work,duration:"
 msgid "Total time spent on this work."
-msgstr "Timp total folosit pentru muncă."
+msgstr "消耗在这项工作上的总时间."
 
 msgctxt "help:timesheet.work,name:"
 msgid "The main identifier of the work."
-msgstr "Identificatorul principal pentru muncă."
+msgstr "工作的主标识符."
 
 msgctxt "help:timesheet.work,origin:"
 msgid "Use to relate the time spent to other records."
-msgstr "Utilizaţi pentru a lega timpul folosit de alte înregistrări."
+msgstr "用于将所花费的时间与其他记录相关联."
 
 msgctxt "help:timesheet.work,timesheet_end_date:"
 msgid "Restrict adding lines after the date."
-msgstr ""
+msgstr "限制只允许在日期之后添加行."
 
 msgctxt "help:timesheet.work,timesheet_lines:"
 msgid "Spend time on this work."
-msgstr ""
+msgstr "此项工作消耗的时间."
 
 msgctxt "help:timesheet.work,timesheet_start_date:"
 msgid "Restrict adding lines before the date."
-msgstr ""
+msgstr "限制只允许在日期之前添加行."
 
 msgctxt "help:timesheet.work.context,from_date:"
 msgid "Do not take into account lines before the date."
-msgstr ""
+msgstr "不考虑日期之前的行."
 
 msgctxt "help:timesheet.work.context,to_date:"
 msgid "Do not take into account lines after the date."
-msgstr ""
+msgstr "不考虑日期之后的行."
 
 msgctxt "model:ir.action,name:act_hours_employee_form"
 msgid "Hours per Employee"
-msgstr ""
+msgstr "雇员工作小时数"
 
 msgctxt "model:ir.action,name:act_hours_employee_monthly_form"
 msgid "Hours per Employee per Month"
-msgstr ""
+msgstr "雇员月工作小时数"
 
 msgctxt "model:ir.action,name:act_hours_employee_weekly_form"
 msgid "Hours per Employee per Week"
-msgstr ""
+msgstr "雇员周工作小时数"
 
 msgctxt "model:ir.action,name:act_line_enter"
 msgid "Enter Timesheet"
-msgstr ""
+msgstr "输入时间表"
 
+#, fuzzy
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Lines"
-msgstr ""
+msgstr "输入行"
 
 msgctxt "model:ir.action,name:act_line_form_work"
 msgid "Timesheet Lines"
-msgstr ""
+msgstr "时间表明细"
 
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works"
-msgstr "Manopera"
+msgstr "工作"
 
 msgctxt "model:ir.action,name:act_work_report"
 msgid "Works"
-msgstr "Manopera"
+msgstr "工作"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_all"
 msgid "All"
-msgstr "Toate"
+msgstr ""
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_open"
 msgid "Open"
-msgstr "Deschis"
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_line_duration_positive"
 msgid "The duration of line \"%(line)s\" must be positive."
-msgstr ""
+msgstr "持续时间明细 \"%(line)s\" 必须为正."
 
 msgctxt "model:ir.message,text:msg_line_uuid_unique"
 msgid "The UUID of timesheet line must be unique."
-msgstr ""
+msgstr "时间表的 UUID 不能重复."
 
 msgctxt "model:ir.message,text:msg_work_company_different_origin"
 msgid "The companies associated with work \"%(work)s\" and its origin differ."
-msgstr ""
+msgstr "工作\"%(work)s\"关联的公司与其来源关联的公司不一致."
 
 msgctxt "model:ir.message,text:msg_work_origin_unique_company"
 msgid "Work origin must be unique by company."
-msgstr ""
+msgstr "工作来源必须按公司唯一."
 
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
-msgstr ""
+msgstr "任意雇员工时"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
 msgid "Own hours"
-msgstr ""
+msgstr "自有雇员工时"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
 msgid "Any employee hours"
-msgstr ""
+msgstr "任意雇员工时"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
 msgid "Own hours"
-msgstr ""
+msgstr "自有雇员工时"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
 msgid "Any employee hours"
-msgstr ""
+msgstr "任意雇员工时"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
 msgid "Own hours"
-msgstr ""
+msgstr "自有雇员工时"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
 msgid "Supervised employee's hours"
-msgstr ""
+msgstr "任意雇员工时"
 
+#, fuzzy
 msgctxt ""
 "model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
 msgid "Supervised employee's hours"
-msgstr ""
+msgstr "任意雇员工时"
 
+#, fuzzy
 msgctxt ""
 "model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
 msgid "Supervised employee's hours"
-msgstr ""
+msgstr "任意雇员工时"
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
-msgstr ""
+msgstr "自有雇员时间表明细"
 
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
 msgid "Any timesheet line"
-msgstr ""
+msgstr "任意雇员工时间表明细"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_line_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "公司中的用户"
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
-msgstr ""
+msgstr "公司中的用户"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configurare"
+msgstr "设置"
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee"
 msgid "Hours per Employee"
-msgstr ""
+msgstr "雇员工作小时数"
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_monthly"
 msgid "Hours per Employee per Month"
-msgstr ""
+msgstr "雇员月工作小时数"
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_weekly"
 msgid "Hours per Employee per Week"
-msgstr ""
+msgstr "雇员周工作小时数"
 
 msgctxt "model:ir.ui.menu,name:menu_line_enter"
 msgid "Enter Timesheet"
-msgstr ""
+msgstr "输入时间表"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_form"
 msgid "Lines"
-msgstr ""
+msgstr "输入行"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "Raportare"
+msgstr "报告"
 
 msgctxt "model:ir.ui.menu,name:menu_timesheet"
 msgid "Timesheet"
-msgstr ""
+msgstr "时间表"
 
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
-msgstr ""
+msgstr "工作"
 
 msgctxt "model:ir.ui.menu,name:menu_work_report"
 msgid "Works"
-msgstr ""
+msgstr "工作"
 
 msgctxt "model:res.group,name:group_timesheet_admin"
 msgid "Timesheet Administration"
-msgstr ""
+msgstr "时间表管理"
 
 msgctxt "model:timesheet.hours_employee,name:"
 msgid "Hours per Employee"
-msgstr ""
+msgstr "雇员工作小时数"
 
 msgctxt "model:timesheet.hours_employee.context,name:"
 msgid "Hours per Employee Context"
-msgstr ""
+msgstr "雇员的工作时间"
 
 msgctxt "model:timesheet.hours_employee_monthly,name:"
 msgid "Hours per Employee per Month"
-msgstr ""
+msgstr "雇员月工作小时数"
 
 msgctxt "model:timesheet.hours_employee_weekly,name:"
 msgid "Hours per Employee per Week"
-msgstr ""
+msgstr "雇员周工作小时数"
 
 msgctxt "model:timesheet.line,name:"
 msgid "Timesheet Line"
-msgstr ""
+msgstr "时间表明细"
 
 msgctxt "model:timesheet.line.enter.start,name:"
 msgid "Enter Lines"
-msgstr ""
+msgstr "输入行"
 
 msgctxt "model:timesheet.work,name:"
 msgid "Work"
-msgstr ""
+msgstr "工作"
 
 msgctxt "model:timesheet.work.context,name:"
 msgid "Work Context"
-msgstr ""
+msgstr "工作环境"
 
 msgctxt "selection:res.user.application,application:"
 msgid "Timesheet"
-msgstr ""
+msgstr "时间表"
 
 msgctxt "wizard_button:timesheet.line.enter,start,end:"
 msgid "Cancel"
-msgstr ""
+msgstr "取消"
 
 msgctxt "wizard_button:timesheet.line.enter,start,enter:"
 msgid "Enter"
-msgstr ""
+msgstr "输入"
```

### Comparing `trytond_timesheet-7.0.1/locale/ru.po` & `trytond_timesheet-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/sl.po` & `trytond_timesheet-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/tr.po` & `trytond_timesheet-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/uk.po` & `trytond_timesheet-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/locale/zh_CN.po` & `trytond_timesheet-7.2.0/locale/ro.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,401 +1,403 @@
 #
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:timesheet.hours_employee,duration:"
 msgid "Duration"
-msgstr "持续时间"
+msgstr "Durata"
 
 msgctxt "field:timesheet.hours_employee,employee:"
 msgid "Employee"
-msgstr "雇员"
+msgstr "Angajat"
 
 msgctxt "field:timesheet.hours_employee.context,end_date:"
 msgid "End Date"
-msgstr "结束日期"
+msgstr "Data Sfărşit"
 
 msgctxt "field:timesheet.hours_employee.context,start_date:"
 msgid "Start Date"
-msgstr "开始日期"
+msgstr "Data Început"
 
 msgctxt "field:timesheet.hours_employee_monthly,duration:"
 msgid "Duration"
-msgstr "持续时间"
+msgstr "Durata"
 
 msgctxt "field:timesheet.hours_employee_monthly,employee:"
 msgid "Employee"
-msgstr "雇员"
+msgstr "Angajat"
 
 msgctxt "field:timesheet.hours_employee_monthly,month:"
 msgid "Month"
-msgstr "月"
+msgstr "Luna"
 
 msgctxt "field:timesheet.hours_employee_monthly,year:"
 msgid "Year"
-msgstr "年"
+msgstr "An"
 
 msgctxt "field:timesheet.hours_employee_weekly,duration:"
 msgid "Duration"
-msgstr "持续时间"
+msgstr "Durata"
 
 msgctxt "field:timesheet.hours_employee_weekly,employee:"
 msgid "Employee"
-msgstr "雇员"
+msgstr "Angajat"
 
 msgctxt "field:timesheet.hours_employee_weekly,week:"
 msgid "Week"
-msgstr "周"
+msgstr "Săptămâna"
 
 msgctxt "field:timesheet.hours_employee_weekly,year:"
 msgid "Year"
-msgstr "年"
+msgstr "An"
 
 msgctxt "field:timesheet.line,company:"
 msgid "Company"
-msgstr "公司"
+msgstr "Companie"
 
 msgctxt "field:timesheet.line,date:"
 msgid "Date"
-msgstr "日期"
+msgstr "Data"
 
 msgctxt "field:timesheet.line,description:"
 msgid "Description"
-msgstr "描述"
+msgstr "Descriere"
 
 msgctxt "field:timesheet.line,duration:"
 msgid "Duration"
-msgstr "持续时间"
+msgstr "Durata"
 
 msgctxt "field:timesheet.line,employee:"
 msgid "Employee"
-msgstr "雇员"
+msgstr "Angajat"
 
 msgctxt "field:timesheet.line,uuid:"
 msgid "UUID"
 msgstr "UUID"
 
 msgctxt "field:timesheet.line,work:"
 msgid "Work"
-msgstr "工作"
+msgstr "Muncă"
 
 msgctxt "field:timesheet.line.enter.start,date:"
 msgid "Date"
-msgstr "日期"
+msgstr "Data"
 
 msgctxt "field:timesheet.line.enter.start,employee:"
 msgid "Employee"
-msgstr "雇员"
+msgstr "Angajat"
 
 msgctxt "field:timesheet.work,company:"
 msgid "Company"
-msgstr "公司"
+msgstr "Companie"
 
 msgctxt "field:timesheet.work,duration:"
 msgid "Timesheet Duration"
-msgstr "时间表持续时间"
+msgstr "Durata Foaie Pontaj"
 
 msgctxt "field:timesheet.work,name:"
 msgid "Name"
-msgstr "名称"
+msgstr "Nume"
 
 msgctxt "field:timesheet.work,origin:"
 msgid "Origin"
-msgstr "来源"
+msgstr "Origine"
 
 msgctxt "field:timesheet.work,timesheet_end_date:"
 msgid "Timesheet End"
-msgstr "时间表结束"
+msgstr "Foaie Pontaj Sfârșit"
 
 msgctxt "field:timesheet.work,timesheet_lines:"
 msgid "Timesheet Lines"
-msgstr "时间表明细"
+msgstr "Rânduri Foaie Pontaj"
 
 msgctxt "field:timesheet.work,timesheet_start_date:"
 msgid "Timesheet Start"
-msgstr "时间表开始"
+msgstr "Foaie Pontaj Început"
 
 msgctxt "field:timesheet.work,work:"
 msgid "Work"
-msgstr "工作"
+msgstr "Muncă"
 
 msgctxt "field:timesheet.work.context,from_date:"
 msgid "From Date"
-msgstr "从日期"
+msgstr "De la Data"
 
 msgctxt "field:timesheet.work.context,to_date:"
 msgid "To Date"
-msgstr "到日期"
+msgstr "Până la Data"
 
 msgctxt "help:timesheet.line,company:"
 msgid "The company on which the time is spent."
-msgstr "消耗时间的公司."
+msgstr "Compania al cărei timp a fost folosit."
 
 msgctxt "help:timesheet.line,date:"
 msgid "When the time is spent."
-msgstr "时间消耗的时候."
+msgstr "Când a fost folosit timp."
 
 msgctxt "help:timesheet.line,description:"
 msgid "Additional description of the work done."
-msgstr "完成工作的附加说明."
+msgstr "Descriere adițională al muncii efectuate."
 
 msgctxt "help:timesheet.line,employee:"
 msgid "The employee who spends the time."
-msgstr "消耗时间的雇员."
+msgstr "Angajatul care foloseşte timp."
 
 msgctxt "help:timesheet.line,work:"
 msgid "The work on which the time is spent."
-msgstr "消耗时间的工作."
+msgstr "Muncă pe care este cheltuit timp."
 
 msgctxt "help:timesheet.line.enter.start,date:"
 msgid "When the time is spent."
-msgstr "消耗时间的时候."
+msgstr "Când este folosit timp."
 
 msgctxt "help:timesheet.line.enter.start,employee:"
 msgid "The employee who spends the time."
-msgstr "消耗时间的雇员."
+msgstr "Angajatul care foloseşte timp."
 
 msgctxt "help:timesheet.work,company:"
 msgid "Make the work belong to the company."
-msgstr "让这项工作属于公司."
+msgstr "Atribuire Muncă la compania."
 
 msgctxt "help:timesheet.work,duration:"
 msgid "Total time spent on this work."
-msgstr "消耗在这项工作上的总时间."
+msgstr "Timp total folosit pentru muncă."
 
 msgctxt "help:timesheet.work,name:"
 msgid "The main identifier of the work."
-msgstr "工作的主标识符."
+msgstr "Identificatorul principal pentru muncă."
 
 msgctxt "help:timesheet.work,origin:"
 msgid "Use to relate the time spent to other records."
-msgstr "用于将所花费的时间与其他记录相关联."
+msgstr "Utilizaţi pentru a lega timpul folosit de alte înregistrări."
 
 msgctxt "help:timesheet.work,timesheet_end_date:"
 msgid "Restrict adding lines after the date."
-msgstr "限制只允许在日期之后添加行."
+msgstr "Restricționați adăugarea de rânduri după dată."
 
+#, fuzzy
 msgctxt "help:timesheet.work,timesheet_lines:"
 msgid "Spend time on this work."
-msgstr "此项工作消耗的时间."
+msgstr "Petrece timp pe această lucrare."
 
 msgctxt "help:timesheet.work,timesheet_start_date:"
 msgid "Restrict adding lines before the date."
-msgstr "限制只允许在日期之前添加行."
+msgstr "Restricționați adăugarea de rânduri înainte de dată."
 
 msgctxt "help:timesheet.work.context,from_date:"
 msgid "Do not take into account lines before the date."
-msgstr "不考虑日期之前的行."
+msgstr "Nu luați în considerare rândurile dinainte de dată."
 
 msgctxt "help:timesheet.work.context,to_date:"
 msgid "Do not take into account lines after the date."
-msgstr "不考虑日期之后的行."
+msgstr "Nu luați în considerare rândurile de după dată."
 
 msgctxt "model:ir.action,name:act_hours_employee_form"
 msgid "Hours per Employee"
-msgstr "雇员工作小时数"
+msgstr "Ore per Angajat"
 
 msgctxt "model:ir.action,name:act_hours_employee_monthly_form"
 msgid "Hours per Employee per Month"
-msgstr "雇员月工作小时数"
+msgstr "Ore per Angajat per Luna"
 
 msgctxt "model:ir.action,name:act_hours_employee_weekly_form"
 msgid "Hours per Employee per Week"
-msgstr "雇员周工作小时数"
+msgstr "Ore per Angajat per Saptamana"
 
 msgctxt "model:ir.action,name:act_line_enter"
 msgid "Enter Timesheet"
-msgstr "输入时间表"
+msgstr "Introduceți Foaia de pontaj"
 
-#, fuzzy
 msgctxt "model:ir.action,name:act_line_form"
 msgid "Lines"
-msgstr "输入行"
+msgstr "Rânduri"
 
 msgctxt "model:ir.action,name:act_line_form_work"
 msgid "Timesheet Lines"
-msgstr "时间表明细"
+msgstr "Rânduri Foaie Pontaj"
 
 msgctxt "model:ir.action,name:act_work_list"
 msgid "Works"
-msgstr "工作"
+msgstr "Manopera"
 
 msgctxt "model:ir.action,name:act_work_report"
 msgid "Works"
-msgstr "工作"
+msgstr "Manopera"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_all"
 msgid "All"
-msgstr ""
+msgstr "Toate"
 
 msgctxt "model:ir.action.act_window.domain,name:act_work_list_domain_open"
 msgid "Open"
-msgstr ""
+msgstr "Deschis"
 
 msgctxt "model:ir.message,text:msg_line_duration_positive"
 msgid "The duration of line \"%(line)s\" must be positive."
-msgstr "持续时间明细 \"%(line)s\" 必须为正."
+msgstr ""
 
 msgctxt "model:ir.message,text:msg_line_uuid_unique"
 msgid "The UUID of timesheet line must be unique."
-msgstr "时间表的 UUID 不能重复."
+msgstr "UUID-ul rândului foii de pontaj trebuie să fie unic."
 
 msgctxt "model:ir.message,text:msg_work_company_different_origin"
 msgid "The companies associated with work \"%(work)s\" and its origin differ."
-msgstr "工作\"%(work)s\"关联的公司与其来源关联的公司不一致."
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_work_origin_unique_company"
 msgid "Work origin must be unique by company."
-msgstr "工作来源必须按公司唯一."
+msgstr "Originea muncii trebuie să fie unică pentru companie."
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_admin"
 msgid "Any employee hours"
-msgstr "任意雇员工时"
+msgstr "Orice program de angajat"
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly"
 msgid "Own hours"
-msgstr "自有雇员工时"
+msgstr "Programul propriu"
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_monthly_admin"
 msgid "Any employee hours"
-msgstr "任意雇员工时"
+msgstr "Orice program de angajat"
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly"
 msgid "Own hours"
-msgstr "自有雇员工时"
+msgstr "Programul propriu"
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_employee_weekly_admin"
 msgid "Any employee hours"
-msgstr "任意雇员工时"
+msgstr "Orice program de angajat"
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_employees"
 msgid "Own hours"
-msgstr "自有雇员工时"
+msgstr "Programul propriu"
 
 #, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_hours_supervised_employees"
 msgid "Supervised employee's hours"
-msgstr "任意雇员工时"
+msgstr "Programul de lucru al angajatului supravegheat"
 
 #, fuzzy
 msgctxt ""
 "model:ir.rule.group,name:rule_group_hours_supervised_employees_monthly"
 msgid "Supervised employee's hours"
-msgstr "任意雇员工时"
+msgstr "Programul de lucru al angajatului supravegheat"
 
 #, fuzzy
 msgctxt ""
 "model:ir.rule.group,name:rule_group_hours_supervised_employees_weekly"
 msgid "Supervised employee's hours"
-msgstr "任意雇员工时"
+msgstr "Programul de lucru al angajatului supravegheat"
 
 msgctxt "model:ir.rule.group,name:rule_group_line"
 msgid "Own timesheet line"
-msgstr "自有雇员时间表明细"
+msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_line_admin"
 msgid "Any timesheet line"
-msgstr "任意雇员工时间表明细"
+msgstr "Orice rând de foaie de pontaj"
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_line_companies"
 msgid "User in companies"
-msgstr "公司中的用户"
+msgstr "Utilizator în companii"
 
-#, fuzzy
 msgctxt "model:ir.rule.group,name:rule_group_work_companies"
 msgid "User in companies"
-msgstr "公司中的用户"
+msgstr "Utilizator în companii"
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "设置"
+msgstr "Configurare"
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee"
 msgid "Hours per Employee"
-msgstr "雇员工作小时数"
+msgstr "Ore per Angajat"
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_monthly"
 msgid "Hours per Employee per Month"
-msgstr "雇员月工作小时数"
+msgstr "Ore per Angajat per Luna"
 
 msgctxt "model:ir.ui.menu,name:menu_hours_employee_open_weekly"
 msgid "Hours per Employee per Week"
-msgstr "雇员周工作小时数"
+msgstr "Ore per Angajat per Saptamana"
 
 msgctxt "model:ir.ui.menu,name:menu_line_enter"
 msgid "Enter Timesheet"
-msgstr "输入时间表"
+msgstr "Introduceți Foaia de pontaj"
 
-#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_line_form"
 msgid "Lines"
-msgstr "输入行"
+msgstr "Rânduri"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
-msgstr "报告"
+msgstr "Raportare"
 
 msgctxt "model:ir.ui.menu,name:menu_timesheet"
 msgid "Timesheet"
-msgstr "时间表"
+msgstr "Foaia de pontaj"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_list"
 msgid "Works"
-msgstr "工作"
+msgstr "Lucrări"
 
+#, fuzzy
 msgctxt "model:ir.ui.menu,name:menu_work_report"
 msgid "Works"
-msgstr "工作"
+msgstr "Lucrări"
 
 msgctxt "model:res.group,name:group_timesheet_admin"
 msgid "Timesheet Administration"
-msgstr "时间表管理"
+msgstr ""
 
 msgctxt "model:timesheet.hours_employee,name:"
 msgid "Hours per Employee"
-msgstr "雇员工作小时数"
+msgstr "Ore per Angajat"
 
 msgctxt "model:timesheet.hours_employee.context,name:"
 msgid "Hours per Employee Context"
-msgstr "雇员的工作时间"
+msgstr ""
 
 msgctxt "model:timesheet.hours_employee_monthly,name:"
 msgid "Hours per Employee per Month"
-msgstr "雇员月工作小时数"
+msgstr "Ore per Angajat per Luna"
 
 msgctxt "model:timesheet.hours_employee_weekly,name:"
 msgid "Hours per Employee per Week"
-msgstr "雇员周工作小时数"
+msgstr "Ore per Angajat per Saptamana"
 
 msgctxt "model:timesheet.line,name:"
 msgid "Timesheet Line"
-msgstr "时间表明细"
+msgstr "Rând Foaie Pontaj"
 
 msgctxt "model:timesheet.line.enter.start,name:"
 msgid "Enter Lines"
-msgstr "输入行"
+msgstr "Introduceți rânduri"
 
 msgctxt "model:timesheet.work,name:"
 msgid "Work"
-msgstr "工作"
+msgstr ""
 
 msgctxt "model:timesheet.work.context,name:"
 msgid "Work Context"
-msgstr "工作环境"
+msgstr ""
 
 msgctxt "selection:res.user.application,application:"
 msgid "Timesheet"
-msgstr "时间表"
+msgstr "Foaie de pontaj"
 
 msgctxt "wizard_button:timesheet.line.enter,start,end:"
 msgid "Cancel"
-msgstr "取消"
+msgstr "Anulare"
 
 msgctxt "wizard_button:timesheet.line.enter,start,enter:"
 msgid "Enter"
-msgstr "输入"
+msgstr "Introducere"
```

### Comparing `trytond_timesheet-7.0.1/message.xml` & `trytond_timesheet-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/routes.py` & `trytond_timesheet-7.2.0/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
 
 from trytond.protocols.wrappers import (
     Response, abort, allow_null_origin, user_application, with_pool,
     with_transaction)
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
 from trytond.wsgi import app
 
 timesheet_application = user_application('timesheet')
 
 
 @app.route('/<database_name>/timesheet/employees', methods=['GET'])
 @allow_null_origin
@@ -119,15 +119,15 @@
                 lines = Line.search([('id', '=', int(line))])
                 if not lines:
                     return Response(None, 204)
                 line, = lines
                 Line.write(lines, data)
         return line.to_json()
     else:
-        with Transaction().set_user(0):
+        with without_check_access():
             lines = Line.search([('id', '=', line)])
         if lines:
             line, = lines
             with Transaction().set_context(
                     company=line.company.id, employee=line.employee.id):
                 lines = Line.search([('id', '=', line.id)])
                 Line.delete(lines)
```

### Comparing `trytond_timesheet-7.0.1/setup.py` & `trytond_timesheet-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/timesheet.xml` & `trytond_timesheet-7.2.0/timesheet.xml`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/tox.ini` & `trytond_timesheet-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/trytond_timesheet.egg-info/PKG-INFO` & `trytond_timesheet-7.2.0/trytond_timesheet.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_timesheet
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module with timesheets
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
@@ -49,17 +49,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: python-sql
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_company_work_time<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_company_work_time<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 
 Timesheet Module
 ################
 
 The timesheet module allow to track the time spent by employees on
 various works. This module also comes with several reports that show
 the time spent by employees on works following various time periods.
```

### Comparing `trytond_timesheet-7.0.1/trytond_timesheet.egg-info/SOURCES.txt` & `trytond_timesheet-7.2.0/trytond_timesheet.egg-info/SOURCES.txt`

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
 exceptions.py
```

### Comparing `trytond_timesheet-7.0.1/view/line_form.xml` & `trytond_timesheet-7.2.0/view/line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/view/work_form.xml` & `trytond_timesheet-7.2.0/view/work_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/work.py` & `trytond_timesheet-7.2.0/work.py`

 * *Files identical despite different names*

### Comparing `trytond_timesheet-7.0.1/work.xml` & `trytond_timesheet-7.2.0/work.xml`

 * *Files 3% similar despite different names*

#### Comparing `trytond_timesheet-7.0.1/work.xml` & `trytond_timesheet-7.2.0/work.xml`

```diff
@@ -66,31 +66,31 @@
     <record model="ir.action.act_window.view" id="act_work_report_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="work_view_graph"/>
       <field name="act_window" ref="act_work_report"/>
     </record>
     <menuitem parent="menu_reporting" action="act_work_report" sequence="10" id="menu_work_report"/>
     <record model="ir.model.access" id="access_work">
-      <field name="model" search="[('model', '=', 'timesheet.work')]"/>
+      <field name="model">timesheet.work</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_work_admin">
-      <field name="model" search="[('model', '=', 'timesheet.work')]"/>
+      <field name="model">timesheet.work</field>
       <field name="group" ref="group_timesheet_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_work_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'timesheet.work')]"/>
+      <field name="model">timesheet.work</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_work_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_work_companies"/>
     </record>
     <record model="ir.ui.view" id="work_context_view_form">
```

