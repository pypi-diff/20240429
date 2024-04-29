# Comparing `tmp/trytond_attendance-7.0.1.tar.gz` & `tmp/trytond_attendance-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_attendance-7.0.1.tar", last modified: Sun Mar  3 12:24:00 2024, max compression
+gzip compressed data, was "trytond_attendance-7.2.0.tar", last modified: Mon Apr 29 15:38:11 2024, max compression
```

## Comparing `trytond_attendance-7.0.1.tar` & `trytond_attendance-7.2.0.tar`

### file list

```diff
@@ -1,76 +1,75 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:24:00.573439 trytond_attendance-7.0.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-03-03 12:23:57.000000 trytond_attendance-7.0.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      730 2024-03-03 12:23:57.000000 trytond_attendance-7.0.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35310 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2356 2024-03-03 12:24:00.573439 trytond_attendance-7.0.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      557 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15214 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/attendance.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14062 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/attendance.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:24:00.566773 trytond_attendance-7.0.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2811 2024-02-05 16:24:27.000000 trytond_attendance-7.0.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      523 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:24:00.566773 trytond_attendance-7.0.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/icons/tryton-attendance.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      915 2024-02-29 11:39:56.000000 trytond_attendance-7.0.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:24:00.570106 trytond_attendance-7.0.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6277 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6530 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6252 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6374 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5700 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5281 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6201 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5093 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5146 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6205 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5161 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5117 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1030 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-03-03 12:24:00.573439 trytond_attendance-7.0.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4445 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:24:00.570106 trytond_attendance-7.0.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2372 2024-02-05 16:24:27.000000 trytond_attendance-7.0.1/tests/scenario_attendance.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2541 2024-02-05 16:24:27.000000 trytond_attendance-7.0.1/tests/scenario_attendance_sheet.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2425 2024-02-05 16:24:27.000000 trytond_attendance-7.0.1/tests/scenario_attendance_timesheet.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      120 2024-02-05 16:24:27.000000 trytond_attendance-7.0.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:24:00.573439 trytond_attendance-7.0.1/trytond_attendance.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2356 2024-03-03 12:24:00.000000 trytond_attendance-7.0.1/trytond_attendance.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2223 2024-03-03 12:24:00.000000 trytond_attendance-7.0.1/trytond_attendance.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-03-03 12:24:00.000000 trytond_attendance-7.0.1/trytond_attendance.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-03-03 12:24:00.000000 trytond_attendance-7.0.1/trytond_attendance.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:07:43.000000 trytond_attendance-7.0.1/trytond_attendance.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       98 2024-03-03 12:24:00.000000 trytond_attendance-7.0.1/trytond_attendance.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-03-03 12:24:00.000000 trytond_attendance-7.0.1/trytond_attendance.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-03-03 12:24:00.573439 trytond_attendance-7.0.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/view/attendance_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/view/attendance_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/view/period_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/view/sheet_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/view/sheet_form_timesheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      456 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/view/sheet_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/view/sheet_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/view/sheet_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-10-30 17:06:38.000000 trytond_attendance-7.0.1/view/sheet_list_timesheet.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:11.632949 trytond_attendance-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      820 2024-04-29 15:18:00.000000 trytond_attendance-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      730 2024-04-29 15:17:59.000000 trytond_attendance-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35310 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2356 2024-04-29 15:38:11.632949 trytond_attendance-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)       13 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      557 2024-02-04 18:51:26.000000 trytond_attendance-7.2.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15288 2024-04-27 16:30:39.000000 trytond_attendance-7.2.0/attendance.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13717 2024-04-27 16:30:39.000000 trytond_attendance-7.2.0/attendance.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:11.629616 trytond_attendance-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-27 16:30:39.000000 trytond_attendance-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      523 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:04.000000 trytond_attendance-7.2.0/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:11.629616 trytond_attendance-7.2.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/icons/tryton-attendance.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      917 2024-04-29 13:17:17.000000 trytond_attendance-7.2.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:11.629616 trytond_attendance-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6277 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6530 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6252 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6374 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5700 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5281 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6201 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5093 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6223 2024-04-29 13:17:17.000000 trytond_attendance-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6205 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5161 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5117 2024-04-27 16:43:22.000000 trytond_attendance-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1030 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:38:11.632949 trytond_attendance-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4445 2024-03-17 11:01:36.000000 trytond_attendance-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:11.629616 trytond_attendance-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2351 2024-04-22 12:14:36.000000 trytond_attendance-7.2.0/tests/scenario_attendance.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2472 2024-04-22 12:14:36.000000 trytond_attendance-7.2.0/tests/scenario_attendance_sheet.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2348 2024-04-22 12:14:36.000000 trytond_attendance-7.2.0/tests/scenario_attendance_timesheet.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:04.000000 trytond_attendance-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      120 2024-04-29 15:17:55.000000 trytond_attendance-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:11.632949 trytond_attendance-7.2.0/trytond_attendance.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2356 2024-04-29 15:38:11.000000 trytond_attendance-7.2.0/trytond_attendance.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2205 2024-04-29 15:38:11.000000 trytond_attendance-7.2.0/trytond_attendance.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:38:11.000000 trytond_attendance-7.2.0/trytond_attendance.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-29 15:38:11.000000 trytond_attendance-7.2.0/trytond_attendance.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:59.000000 trytond_attendance-7.2.0/trytond_attendance.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       98 2024-04-29 15:38:11.000000 trytond_attendance-7.2.0/trytond_attendance.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:38:11.000000 trytond_attendance-7.2.0/trytond_attendance.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:38:11.632949 trytond_attendance-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      396 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/attendance_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/attendance_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      508 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/period_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/sheet_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/sheet_form_timesheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      456 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/sheet_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      424 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/sheet_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/sheet_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_attendance-7.2.0/view/sheet_list_timesheet.xml
```

### Comparing `trytond_attendance-7.0.1/CHANGELOG` & `trytond_attendance-7.2.0/CHANGELOG`

 * *Files 12% similar despite different names*

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

### Comparing `trytond_attendance-7.0.1/COPYRIGHT` & `trytond_attendance-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright (C) 2020-2024 Sergi Almacellas Abellana
-Copyright (C) 2020-2023 B2CK
-Copyright (C) 2020-2023 Cédric Krier
+Copyright (C) 2020-2024 B2CK
+Copyright (C) 2020-2024 Cédric Krier
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_attendance-7.0.1/LICENSE` & `trytond_attendance-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/PKG-INFO` & `trytond_attendance-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_attendance
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for recording employee attendance
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
@@ -44,14 +44,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_timesheet<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_timesheet<7.3,>=7.2; extra == "test"
 
 doc/index.rst
```

### Comparing `trytond_attendance-7.0.1/__init__.py` & `trytond_attendance-7.2.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/attendance.py` & `trytond_attendance-7.2.0/attendance.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 class Line(ModelSQL, ModelView):
     "Attendance Line"
     __name__ = 'attendance.line'
 
     company = fields.Many2One('company.company', "Company", required=True,
         help="The company which the employee attended.")
     employee = fields.Many2One('company.employee', "Employee", required=True,
+        search_context={
+            'active_test': False,
+            },
         domain=[
             ('company', '=', Eval('company')),
             ['OR',
                 ('start_date', '=', None),
                 ('start_date', '<=', Eval('date', None)),
                 ],
             ['OR',
```

### Comparing `trytond_attendance-7.0.1/attendance.xml` & `trytond_attendance-7.2.0/attendance.xml`

 * *Files 14% similar despite different names*

#### Comparing `trytond_attendance-7.0.1/attendance.xml` & `trytond_attendance-7.2.0/attendance.xml`

```diff
@@ -43,42 +43,42 @@
       <field name="sequence" eval="20"/>
       <field name="view" ref="attendance_view_form"/>
       <field name="act_window" ref="act_attendance"/>
     </record>
     <menuitem action="act_attendance" parent="menu_main_attendance" sequence="10" id="menu_attendance"/>
     <record model="ir.rule.group" id="rule_group_attendance_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'attendance.line')]"/>
+      <field name="model">attendance.line</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_attendance_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_attendance_companies"/>
     </record>
     <record model="ir.model.access" id="access_attendance">
-      <field name="model" search="[('model', '=', 'attendance.line')]"/>
+      <field name="model">attendance.line</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.rule.group" id="rule_group_attendance">
       <field name="name">Own attendance</field>
-      <field name="model" search="[('model', '=', 'attendance.line')]"/>
+      <field name="model">attendance.line</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="True"/>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.rule" id="rule_attendance">
       <field name="domain" eval="[('employee', 'in', Eval('employees', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_attendance"/>
     </record>
     <record model="ir.rule.group" id="rule_group_attendance_admin">
       <field name="name">Any attendance</field>
-      <field name="model" search="[('model', '=', 'attendance.line')]"/>
+      <field name="model">attendance.line</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="False"/>
     </record>
     <record model="ir.rule.group-res.group" id="rule_group_attendance_admin_group_employee_admin">
       <field name="rule_group" ref="rule_group_attendance_admin"/>
       <field name="group" ref="group_attendance_admin"/>
     </record>
@@ -105,80 +105,80 @@
       <field name="sequence" eval="20"/>
       <field name="view" ref="period_view_form"/>
       <field name="act_window" ref="act_period_list"/>
     </record>
     <menuitem action="act_period_list" parent="menu_configuration" sequence="10" id="menu_period_list"/>
     <record model="ir.rule.group" id="rule_group_period_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'attendance.period')]"/>
+      <field name="model">attendance.period</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_period_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_period_companies"/>
     </record>
     <record model="ir.model.access" id="access_period">
-      <field name="model" search="[('model', '=', 'attendance.period')]"/>
+      <field name="model">attendance.period</field>
       <field name="perm_read" eval="False"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_period_admin">
-      <field name="model" search="[('model', '=', 'attendance.period')]"/>
+      <field name="model">attendance.period</field>
       <field name="group" ref="group_attendance_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
     <record model="ir.model.button" id="period_draft_button">
+      <field name="model">attendance.period</field>
       <field name="name">draft</field>
       <field name="string">Draft</field>
-      <field name="model" search="[('model', '=', 'attendance.period')]"/>
     </record>
     <record model="ir.model.button" id="period_close_button">
+      <field name="model">attendance.period</field>
       <field name="name">close</field>
       <field name="string">Close</field>
-      <field name="model" search="[('model', '=', 'attendance.period')]"/>
     </record>
     <record model="ir.ui.view" id="sheet_line_view_form">
       <field name="model">attendance.sheet.line</field>
       <field name="type">form</field>
       <field name="name">sheet_line_form</field>
     </record>
     <record model="ir.ui.view" id="sheet_line_view_list">
       <field name="model">attendance.sheet.line</field>
       <field name="type">tree</field>
       <field name="name">sheet_line_list</field>
     </record>
     <record model="ir.rule.group" id="rule_group_sheet_line_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'attendance.sheet.line')]"/>
+      <field name="model">attendance.sheet.line</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_sheet_line_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_sheet_line_companies"/>
     </record>
     <record model="ir.rule.group" id="rule_group_sheet_line">
       <field name="name">Own attendance sheet line</field>
-      <field name="model" search="[('model', '=', 'attendance.sheet.line')]"/>
+      <field name="model">attendance.sheet.line</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="True"/>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.rule" id="rule_sheet_line">
       <field name="domain" eval="[('employee', 'in', Eval('employees', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_sheet_line"/>
     </record>
     <record model="ir.rule.group" id="rule_group_sheet_line_admin">
       <field name="name">Any attendance sheet line</field>
-      <field name="model" search="[('model', '=', 'attendance.sheet.line')]"/>
+      <field name="model">attendance.sheet.line</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="False"/>
     </record>
     <record model="ir.rule.group-res.group" id="rule_group_sheet_line_admin_group_employee_admin">
       <field name="rule_group" ref="rule_group_sheet_line_admin"/>
       <field name="group" ref="group_attendance_admin"/>
     </record>
@@ -204,35 +204,35 @@
     <record model="ir.action.act_window.view" id="act_sheet_view2">
       <field name="sequence" eval="20"/>
       <field name="view" ref="sheet_view_form"/>
       <field name="act_window" ref="act_sheet"/>
     </record>
     <record model="ir.rule.group" id="rule_group_sheet_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'attendance.sheet')]"/>
+      <field name="model">attendance.sheet</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_sheet_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_sheet_companies"/>
     </record>
     <record model="ir.rule.group" id="rule_group_sheet">
       <field name="name">Own attendance sheet</field>
-      <field name="model" search="[('model', '=', 'attendance.sheet')]"/>
+      <field name="model">attendance.sheet</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="True"/>
       <field name="perm_read" eval="False"/>
     </record>
     <record model="ir.rule" id="rule_sheet">
       <field name="domain" eval="[('employee', 'in', Eval('employees', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_sheet"/>
     </record>
     <record model="ir.rule.group" id="rule_group_sheet_admin">
       <field name="name">Any attendance sheet</field>
-      <field name="model" search="[('model', '=', 'attendance.sheet')]"/>
+      <field name="model">attendance.sheet</field>
       <field name="global_p" eval="False"/>
       <field name="default_p" eval="False"/>
     </record>
     <record model="ir.rule.group-res.group" id="rule_group_sheet_admin_group_employee_admin">
       <field name="rule_group" ref="rule_group_sheet_admin"/>
       <field name="group" ref="group_attendance_admin"/>
     </record>
```

### Comparing `trytond_attendance-7.0.1/doc/conf.py` & `trytond_attendance-7.2.0/doc/conf.py`

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

### Comparing `trytond_attendance-7.0.1/doc/index.rst` & `trytond_attendance-7.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/icons/LICENSE` & `trytond_attendance-7.2.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/ir.py` & `trytond_attendance-7.2.0/ir.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,14 @@
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

### Comparing `trytond_attendance-7.0.1/locale/bg.po` & `trytond_attendance-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/ca.po` & `trytond_attendance-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/cs.po` & `trytond_attendance-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/de.po` & `trytond_attendance-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/es.po` & `trytond_attendance-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/es_419.po` & `trytond_attendance-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/et.po` & `trytond_attendance-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/fa.po` & `trytond_attendance-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/fi.po` & `trytond_attendance-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/fr.po` & `trytond_attendance-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/hu.po` & `trytond_attendance-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/id.po` & `trytond_attendance-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/it.po` & `trytond_attendance-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/lo.po` & `trytond_attendance-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/lt.po` & `trytond_attendance-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/nl.po` & `trytond_attendance-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/pl.po` & `trytond_attendance-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/pt.po` & `trytond_attendance-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/ro.po` & `trytond_attendance-7.2.0/locale/uk.po`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 msgctxt "model:ir.action,name:act_attendance"
 msgid "Attendances"
 msgstr ""
 
 msgctxt "model:ir.action,name:act_period_list"
 msgid "Periods"
-msgstr "Perioade"
+msgstr ""
 
 msgctxt "model:ir.action,name:act_sheet"
 msgid "Sheets"
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_close_period_previous_open"
 msgid "To close period \"%(period)s\" you must first close \"%(other_period)s\"."
@@ -142,19 +142,19 @@
 
 msgctxt "model:ir.message,text:msg_modify_period_close"
 msgid "To modify attendance \"%(attendance)s\" you must reopen period \"%(period)s\"."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
-msgstr "Închidere"
+msgstr "Закрити"
 
 msgctxt "model:ir.model.button,string:period_draft_button"
 msgid "Draft"
-msgstr "Draft"
+msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_attendance"
 msgid "Own attendance"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_attendance_admin"
 msgid "Any attendance"
@@ -162,15 +162,15 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_attendance_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_period_companies"
 msgid "User in companies"
-msgstr "Utilizator în companii"
+msgstr "Користувач у компаніях"
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet"
 msgid "Own attendance sheet"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet_admin"
 msgid "Any attendance sheet"
@@ -194,23 +194,23 @@
 
 msgctxt "model:ir.ui.menu,name:menu_attendance"
 msgid "Attendances"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Configurare"
+msgstr "Налаштування"
 
 msgctxt "model:ir.ui.menu,name:menu_main_attendance"
 msgid "Attendance"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_period_list"
 msgid "Periods"
-msgstr "Perioade"
+msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_sheet"
 msgid "Sheets"
 msgstr ""
 
 msgctxt "model:res.group,name:group_attendance_admin"
 msgid "Attendance Administration"
```

### Comparing `trytond_attendance-7.0.1/locale/ru.po` & `trytond_attendance-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/sl.po` & `trytond_attendance-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/tr.po` & `trytond_attendance-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/locale/uk.po` & `trytond_attendance-7.2.0/locale/zh_CN.po`

 * *Files 2% similar despite different names*

```diff
@@ -142,19 +142,19 @@
 
 msgctxt "model:ir.message,text:msg_modify_period_close"
 msgid "To modify attendance \"%(attendance)s\" you must reopen period \"%(period)s\"."
 msgstr ""
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
-msgstr "Закрити"
+msgstr "结账"
 
 msgctxt "model:ir.model.button,string:period_draft_button"
 msgid "Draft"
-msgstr ""
+msgstr "草案"
 
 msgctxt "model:ir.rule.group,name:rule_group_attendance"
 msgid "Own attendance"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_attendance_admin"
 msgid "Any attendance"
@@ -162,15 +162,15 @@
 
 msgctxt "model:ir.rule.group,name:rule_group_attendance_companies"
 msgid "User in companies"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_period_companies"
 msgid "User in companies"
-msgstr "Користувач у компаніях"
+msgstr "公司中的用户"
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet"
 msgid "Own attendance sheet"
 msgstr ""
 
 msgctxt "model:ir.rule.group,name:rule_group_sheet_admin"
 msgid "Any attendance sheet"
@@ -194,15 +194,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_attendance"
 msgid "Attendances"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
-msgstr "Налаштування"
+msgstr "设置"
 
 msgctxt "model:ir.ui.menu,name:menu_main_attendance"
 msgid "Attendance"
 msgstr ""
 
 msgctxt "model:ir.ui.menu,name:menu_period_list"
 msgid "Periods"
```

### Comparing `trytond_attendance-7.0.1/message.xml` & `trytond_attendance-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/setup.py` & `trytond_attendance-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/tests/scenario_attendance.rst` & `trytond_attendance-7.2.0/tests/scenario_attendance.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 ===================
 Attendance Scenario
 ===================
 
 Imports::
 
     >>> import datetime as dt
+
     >>> from dateutil.relativedelta import relativedelta
+
     >>> from proteus import Model
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual, assertTrue
+
     >>> now = dt.datetime.now()
     >>> tomorrow = now + relativedelta(days=1)
     >>> next_week = now + relativedelta(days=7)
 
 Activate attendance.line module::
 
     >>> config = activate_modules('attendance')
@@ -40,18 +42,16 @@
     >>> attendance = Attendance()
     >>> attendance.type
     'in'
     >>> attendance.employee = employee
     >>> attendance.at = now
     >>> attendance.save()
 
-    >>> attendance.date == now.date()
-    True
-    >>> bool(attendance.rec_name)
-    True
+    >>> assertEqual(attendance.date, now.date())
+    >>> assertTrue(attendance.rec_name)
 
 When creating a new attendance the type is automatically set::
 
     >>> attendance = Attendance()
     >>> attendance.employee = employee
     >>> attendance.at = now + relativedelta(hours=2)
     >>> attendance.type
@@ -72,24 +72,23 @@
 
 You can't create attendances in closed periods::
 
     >>> attendance = Attendance()
     >>> attendance.employee = employee
     >>> attendance.at = now
     >>> attendance.type = 'in'
-    >>> attendance.save() # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> attendance.save()
     Traceback (most recent call last):
         ...
     PeriodClosedError: ...
 
 But it is possible in open periods::
 
     >>> attendance.at = tomorrow
     >>> attendance.save()
 
 Update attendance date time, update its date::
 
     >>> attendance.at = next_week
     >>> attendance.save()
 
-    >>> attendance.date == next_week.date()
-    True
+    >>> assertEqual(attendance.date, next_week.date())
```

### Comparing `trytond_attendance-7.0.1/tests/scenario_attendance_sheet.rst` & `trytond_attendance-7.2.0/tests/scenario_attendance_sheet.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 =========================
 Attendance Sheet Scenario
 =========================
 
 Imports::
 
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
+
     >>> from proteus import Model
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
     >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
 
 Activate attendance.line module::
 
     >>> config = activate_modules('attendance')
 
 Create a company::
 
@@ -51,38 +50,37 @@
     >>> present(employee1, 'in', dt.datetime(2020, 4, 1, 15))
     >>> present(employee1, 'out', dt.datetime(2020, 4, 1, 18))
 
 Check attendance sheet::
 
     >>> Sheet = Model.get('attendance.sheet')
     >>> sheet, = Sheet.find([])
-    >>> sheet.duration == dt.timedelta(hours=8)
-    True
+    >>> sheet.duration
+    datetime.timedelta(seconds=28800)
     >>> sheet.date
     datetime.date(2020, 4, 1)
     >>> len(sheet.lines)
     3
-    >>> (sum([l.duration for l in sheet.lines], dt.timedelta()) ==
-    ...     dt.timedelta(hours=8))
-    True
+    >>> sum([l.duration for l in sheet.lines], dt.timedelta())
+    datetime.timedelta(seconds=28800)
 
 Fill attendance over 1 day::
 
     >>> present(employee1, 'in', dt.datetime(2020, 4, 2, 20))
     >>> present(employee1, 'out', dt.datetime(2020, 4, 3, 6))
 
 Check attendance sheet::
 
     >>> sheet, = Sheet.find([('date', '=', dt.date(2020, 4, 2))])
-    >>> sheet.duration == dt.timedelta(hours=10)
-    True
+    >>> sheet.duration
+    datetime.timedelta(seconds=36000)
 
 Add attendance for other employee::
 
     >>> present(employee2, 'in', dt.datetime(2020, 4, 1, 10))
     >>> present(employee2, 'out', dt.datetime(2020, 4, 1, 16))
 
 Check attendance sheet::
 
     >>> sheet, = Sheet.find([('employee', '=', employee2.id)])
-    >>> sheet.duration == dt.timedelta(hours=6)
-    True
+    >>> sheet.duration
+    datetime.timedelta(seconds=21600)
```

### Comparing `trytond_attendance-7.0.1/tests/scenario_attendance_timesheet.rst` & `trytond_attendance-7.2.0/tests/scenario_attendance_timesheet.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 =============================
 Attendance Timesheet Scenario
 =============================
 
 Imports::
 
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
+
     >>> from proteus import Model
     >>> from trytond import backend
-    >>> from trytond.tests.tools import activate_modules
-    >>> from trytond.modules.company.tests.tools import create_company, \
-    ...     get_company
+    >>> from trytond.modules.company.tests.tools import create_company, get_company
+    >>> from trytond.tests.tools import activate_modules, assertEqual
 
 Activate attendance.line module::
 
     >>> config = activate_modules(['attendance', 'timesheet'])
 
 Create a company::
 
@@ -53,29 +52,26 @@
 
 Fill time sheet::
 
     >>> Timesheet = Model.get('timesheet.line')
     >>> def spend(employee, work, date, duration):
     ...     timesheet = Timesheet(employee=employee, work=work)
     ...     timesheet.date = date
-    ...     timesheet.duration =duration
+    ...     timesheet.duration = duration
     ...     timesheet.save()
 
     >>> spend(employee, work, dt.date(2020, 4, 1), dt.timedelta(hours=7))
     >>> spend(employee, work, dt.date(2020, 4, 2), dt.timedelta(hours=2))
 
 Check attendance time sheet::
 
     >>> Sheet = Model.get('attendance.sheet')
     >>> sheet, = Sheet.find([('date', '=', dt.date(2020, 4, 1))])
-    >>> sheet.duration == dt.timedelta(hours=8)
-    True
-    >>> sheet.timesheet_duration == dt.timedelta(hours=7)
-    True
+    >>> sheet.duration
+    datetime.timedelta(seconds=28800)
+    >>> sheet.timesheet_duration
+    datetime.timedelta(seconds=25200)
 
     >>> if backend.name != 'sqlite':
     ...     sheet, = Sheet.find([('date', '=', dt.date(2020, 4, 2))])
     ...     sheet.duration
-    ...     sheet.timesheet_duration == dt.timedelta(hours=2)
-    ... else:
-    ...     True
-    True
+    ...     assertEqual(sheet.timesheet_duration, dt.timedelta(hours=2))
```

### Comparing `trytond_attendance-7.0.1/tox.ini` & `trytond_attendance-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_attendance-7.0.1/trytond_attendance.egg-info/PKG-INFO` & `trytond_attendance-7.2.0/trytond_attendance.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_attendance
-Version: 7.0.1
+Version: 7.2.0
 Summary: Tryton module for recording employee attendance
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
@@ -44,14 +44,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: proteus<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_timesheet<7.1,>=7.0; extra == "test"
+Requires-Dist: proteus<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_timesheet<7.3,>=7.2; extra == "test"
 
 doc/index.rst
```

### Comparing `trytond_attendance-7.0.1/trytond_attendance.egg-info/SOURCES.txt` & `trytond_attendance-7.2.0/trytond_attendance.egg-info/SOURCES.txt`

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
 attendance.py
```

